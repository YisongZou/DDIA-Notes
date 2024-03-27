> Chapter 7 Transactions(There is a race condition type summary inside book summary part)
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
* Read Committed `No dirty reads(A txn should not see the uncommitted result of another txn)(About what a read-only txn can see in the presence of concurrent writes)` `No dirty writes(A txn should not overwrite the uncommitted value of another write txn, however this does not prevent the race condition between two counter increments)` `Implementing read committed` 
* Snapshot Isolationand repeatable read(Those two are the same thing)
(Snapshot Isolation:Each transaction reads from a consistent snapshot of the database) (These two are about what a read-only txn can see in the presence of concurrent writes, eg: someone transfers money from one of his account to another, he happens to read the money amount of account 1 while the txn is not yet committed, after the transfer he will see account 1 money does not change while the money in account 2 has increased by the change )`Implementing snapshot isolation` `Visibility rules for observing a consistent snapshot(MVCC, multi-version concurrency control)`
`Indexes and snapshot isolation` `Repeatable read and naming confusion`  
* Preventing Lost Updates(Write-write conflicts) (Read-modify-write cycle caused data to be lost) Solutions:`Automic write operations` `Explicit locking` `Automatically
detecting lost updates` `Compare and set` `Conflict resolution and replication`
* Write skew and Phantoms `Characterizing write skew` `More examples of write skew` `Phantoms causing write skew` `Materializing conflicts` 
#### 3.Serializability
* Actual Serial Execution `Encapsulating transactions in stored procedures` `Pros and cons of stored procedures` `Partitioning` 
* Two-phase locking (2PL)
* Serializable Snapshot Isolation(SSL)
`  `
