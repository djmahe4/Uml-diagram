
```
# Uml-diagram
+---------------------+          +----------------+            +----------------------+
|       Bank          |          |       ATM      |            |     DebitCard         |
+---------------------+          +----------------+            +----------------------+
| - bankName          |          | - location     |            | - cardNumber          |
| - branch            |          | - ATMID        |            | - expiryDate          |
| - IFSCCode          |          +----------------+            | - CVV                |
+---------------------+          | + validateCard()|           +----------------------+
| + manageATM()       |          | + processTransaction()|     | + verifyCard()        |
| + addAccount()      |          | + checkBalance()  |          | + blockCard()         |
| + closeAccount()    |          +-----------------+            +----------------------+
+---------------------+                                       
        |                                                          |
        |                                                          |
        |                    +-------------------+                 |
        +--------------------|    Customer       |<----------------+
                              +-------------------+
                              | - customerID      |
                              | - name            |
                              | - address         |
                              | - phoneNumber     |
                              +-------------------+
                              | + deposit()       |
                              | + withdraw()      |
                              | + checkBalance()  |
                              +-------------------+
                                       |
                                       |
                        +----------------------------+
                        |         Account            |
                        +----------------------------+
                        | - accountNumber            |
                        | - accountType              |
                        | - balance                  |
                        +----------------------------+
                        | + deposit()                |
                        | + withdraw()               |
                        | + checkBalance()           |
                        +----------------------------+
                                       |
                                       |
                        +----------------------------+
                        |     ATMTransaction         |
                        +----------------------------+
                        | - transactionID            |
                        | - transactionType          |
                        | - transactionDate          |
                        | - amount                   |
                        +----------------------------+
                        | + recordTransaction()      |
                        +----------------------------+
```
