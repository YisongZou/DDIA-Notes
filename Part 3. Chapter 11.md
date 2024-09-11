> Chapter 11 Stream Processing

`Processing every event as it happens`

#### 1.Transmitting Event Streams
* Messaging Systems `Direct messaging from producers to consumers` `Message Brokers(Message queue)` `Message brokers compared to databases`
`Multiple consumers` `Acknowledgments and redelivery`
* Partitioned Logs: Log based message brokers(Eg:Apache Kafka) `Using logs for message storage` `Logs compared to traditional messaging`  `Consumer offsets` 
`Disk Space Usage` `When consumers cannot keep up with producers` `Replaying old messages` 

#### 2.Database and Streams
* Keeping Systems in Sync
* Change Data Capture `Implementing change data capture` `Initial snapshot` `Log compaction` `API support for change streams` 
* Event Sourcing `Deriving current state from the event log` `Command and events` 
* State, Streams, and Immutability `Advantages of immutable events` `Deriving several views from the same event log` `Limitations of immutability`

#### 3.Processing Streams
* Use of Stream Processing
* Reasoning About Time
* Stream Joins
* Fault Tolerance
