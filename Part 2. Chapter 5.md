> Part2: Distributed Data 

> Chapter 5 Replication (Assuming the dataset is small and each machine can hold a copy of entire dataset)

` Three popular algorithms for replicating changes between nodes: single-leader, multi-leader, and leaderless `
#### 1.Leaders and followers
* Synchronous Versus Asynchronous Replication
* Setting up New Followers
* Handling Node Outages
* Implementation of Replication Logs

#### 2.Problems with replication lag
* Reading your own Writes
* Monotonic Reads
* Consistent Prefix Reads
* Solutions for Replication Lag

#### 3.Multi-Leader Replication
* Use Cases for Multi-Leader Replication
* Handling Write Conflicts
* Multi-Leader Replication Topologies

#### 4.Leaderless Replication
* Writing to the Database when a node is down
* Limitations of Quorum Consistency
* Sloppy Quorums and Hinted Handoff
* Detecting Concurrent Writes