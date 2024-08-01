> Part3: Derived Data 

> Chapter 10 Batch Processing

```
Three different types of systems
Services(online systems)
Batch processing systems(offline systems)
Stream processing systems(near-real-time systems)
```

#### 1.Batch processing with Unix tools
* Simple log Analysis `Chain of commands versus custom program` `Sorting versus in-memory aggregation`
* The Unix Philosophy `A uniform interface` `Separation of logic and wiring` `Transparency and experimentation`

#### 2.MapReduce and Distributed Filesystems
* MapReduce job Execution `Distributed execution of MapReduce`  `MapReduce workflows` 
* Reduce-side Joins and Grouping `Example: analysis of user activity events` `Sort-merge joins` `Bringing related data together in the same place` `Group by` `Handling skew`
* Map-side Joins `Broadcast hash joins` `Partitioned hash joins` `Map-side merge joins` `MapReduce workflows with map-side joins` 
* The Output of Batch Workflows `Building search indexes` `Key-value stores as batch process output` `Philosophy of batch process outputs`
* Comparing Hadoop to Distributed database `Diversity of storage` `Diversity of processing models` `Designing for frequent faults` <-Here

#### 3.Beyond MapReduce
* Materialization of Intermediate State
* Graphs and Iterative Processing
* High-Level APIs and Languages
