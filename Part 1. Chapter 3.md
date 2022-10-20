> Chapter 3 Storage and Retrieval

#### 1. Data Structures That Power Your Database
* Hash Indexes
* SSTables and LSM - Trees ```Constructing and maintaining SSTables``` ```Making an LSM-tree out of SSTables``` ```performance optimizations``` 
* B-Trees ```Making B-trees reliable``` ```B-tree optimizations``` 
* Comparing B-Trees and LSM-Trees ```Advantage of LSM trees``` ```Downside of LSM trees``` 
* Other Indexing Structures ```Storing values within the index``` ```Multi-column indexes``` ```Full-text search and fuzzy indexes``` ```Keeping everything in memory```
#### 2. Transaction Processing or Analytics?
* Data Warehousing ```The Divergence between OLTP database and data warehouses``` 
* Stars and Snowflakes: Schemas for Analytics
#### 3. Column-Oriented Storage
* Column compression ``` Memory bandwidth and vectorized processing ```
* Sort order in Column storage ``` Several different sort orders ```
* Writing to Column-Oriented storage
* Aggregation: Data Cubes and Materialized Views
