> Part2: Distributed Data 

> Chapter 5 Replication (Assuming the dataset is small and each machine can hold a copy of entire dataset)

` Three popular algorithms for replicating changes between nodes: single-leader, multi-leader, and leaderless `
#### 1.Leaders and followers
* Synchronous Versus Asynchronous Replication
* Setting up New Followers
* Handling Node Outages
` Follower failure: Catch-up recovery` `Leader failure: Failover` 
* Implementation of Replication Logs
` Statement-based replication(Not used that much recently ` ` Write-ahead log (WAL) shipping ` ` Logical (row-based) log replication `
` Trigger-based replication`

#### 2.Problems with replication lag
* Reading your own Writes
` Need read-after-write consistency, listed possible techniques` 
* Monotonic Reads
* Consistent Prefix Reads
* Solutions for Replication Lag

#### 3.Multi-Leader Replication
* Use Cases for Multi-Leader Replication
` Multi-datacenter operation ` ` Clients with offline operation ` `Collaborative editing `
* Handling Write Conflicts
` Synchronous versus asynchronous conflict detection ` ` conflict avoidance ` ` Converging toward a consistent state ` `Custom conflict resolution logic `
` What is a conflict `
* Multi-Leader Replication Topologies

#### 4.Leaderless Replication
* Writing to the Database when a node is down
` Read repair and anti-entropy ` `  Quorums for reading and writing `
* Limitations of Quorum Consistency
` Monitoring staleness ` 
* Sloppy Quorums and Hinted Handoff
` Multi-datacenter operation `
* Detecting Concurrent Writes

