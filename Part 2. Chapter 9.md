> Chapter 9 Consistency and consensus

#### 1.Consistency Guarantees
(Summarize this chapter, basically talks about distributed consistency models.
Unlike chapter 7 which talks about transaction isolation levels)

#### 2.Linearizability
* What makes a system linearizable?`The difference between linearizability(About different nodes) and serializability(About transactions)`
* Relying on Linearizability`Locking and leader election` `Constraints and uniqueness guarantees`
  `Cross-channel timing dependencies` 
* Implementing linearizable systems`Linearizability and quorums`
* The cost of Linearizability`The cap theorem` `Linearizability and network delays`

#### 3.Ordering Guarantees(The issue of ordering events in distributed system）
* Ordering and casuality `The causal order is not a total order` `linearizability is stronger than causal
consistency` `Capturing causal dependencies` 
* Sequence number ordering `Noncausal sequence number generators` `Lamport timestamps`
`Timestamp ordering is not sufficient`
* Total order Broadcast `Using total order broadcast` `Implementing linearizable storage using total order broadcast`
`Implementing total order broadcast using linearizable storage`

#### 4.Distributed Transactions and Consensus(How to atomically commit a distributed transaction)
* Automic Commit and Two-Phase commit(2PC) `From single-node to distributed automic commit`
  `Introducing to two-phase commit` `A System of promises` `Coordinator failure` `Three phae commit`
* Distributed transactions in practice `Exactly-once message procesing` `XA transactions` `Holding locks while in doubt` `Recovering from coordinator failure` `Limitations for distributed transactions`
* Fault-Tolerant Consensus ` Conesensus algorithm satisfy the following: Uniform agreement, Integrity, Validity, Termination` ` Conesensus algorithms and total order broadcast` ` Single leader replication and consensus`
`Epoch numbering and quorums` `Limitations of consensus` 
* Membership and Coordination Services `Allocating work to nodes` ` Service discovery` `Membership services`

