> Chapter 7 Transactions
`The chapter applies to both single node and distributed databases`

#### 1.The Slippery Concept of a Transaction
* The meaning of ACID

`Automicity: It is not related to concurrency. Describes if a client wants to
make several writes, but a fault occurs after some of the writes have been processed.
If the writes grouped together into an atomic transaction, and the txn cannot be
completed (committed) due to a fault, then the txn is aborted and the database must
discard or undo any writes it has made so far in the txn.` 

`Consistency: You have certain statements about your data(invariants) that should always be true. For example, when you transfer money from one account to another, the total amount of money of the two accounts added together should always remain the same.`

`Isolation: Concurrently(In parallel) executing transactions are isolated from each other`

`Durability: Once a transaction has been committed successfully, any data that has written will not be forgotten, even if there is a hardware fault or the database crashes`

* Single-Object and Multi-Object Operations `Single object writes` `The need for multi-object transactions`  `Handling error and aborts` 

#### 2.Weak Isolation Levels
* Read Committed `No dirty reads` `No dirty writes` `Implementing read committed` 
* Snapshot Isolation and repeatable read
* Preventing Lost Updates
* Write skew and Phantoms
#### 3.Serializability
* Actual Serial Execution
* Two-phase locking (2PL)
* Serializable Snapshot Isolation(SSL)
`  `
