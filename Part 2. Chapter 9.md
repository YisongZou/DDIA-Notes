> Chapter 9 Consistency and consensus

#### 1.Consistency Guarantees
(Summarize this chapter, basically talks about distributed consistency models.
Unlike chapter 7 which talks about transaction isolation levels)

#### 2.Linearizability
* What makes a system linearizable?`The difference between linearizability and serializability`
* Relying on Linearizability`Locking and leader election` `Constraints and uniqueness guarantees`
  `Cross-channel timing dependencies` 
* Implementing linearizable systems`Linearizability and quorums`
* The cost of Linearizability`The cap theorem` `Linearizability and network delays`

#### 3.Ordering Guarantees(The issue of ordering events in distributed system)<-start from here next time
* Ordering and casuality
* Sequence number ordering
* Total order Broadcast

#### 4.Distributed Transactions and Consensus(How to atomically commit a distributed transaction)
* Automic Commit and Two-Phase commit(2PC)
* Distributed transactions in practice
* Fault-Tolerant Consensus
* Membership and Coordination Services

