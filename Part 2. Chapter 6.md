> Chapter 6 Partitioning

#### 1.Partitioning and Replication

#### 2.Partitioning of Key-Value Data
* Partitioning by Key Range
* Partitioning by Hash of Key
` Cassandra compound primary key approach `
* Skewed Workloads and Relieving Hot Spots

#### 2.Partitioning and secondary indexes
* Partitioning secondary indexes by Document
* Partitioning secondary indexes by Term

#### 3. Rebalancing Partitions
* Stategies for Rebalancing
` How not to do it: hash mod N ` ` Fixed number of partitions ` ` Dynamic partitioning ` `Partitioning proportionally to nodes ` 
* Operations: Automatic or Manual Rebalancing

#### 4. Request Routing
* Parallel Query Execution
