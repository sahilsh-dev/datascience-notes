The Hadoop Distributed File System (HDFS) is a scalable, fault-tolerant storage system designed for storing large datasets. It divides data into blocks and distributes them across a cluster, ensuring redundancy and high availability.

## Components of HDFS

- **NameNode (Master Node):** Manages metadata and directory structure.
- **DataNodes:** Store and retrieve data blocks as directed by the NameNode.
- **Secondary NameNode:** Handles periodic snapshots of metadata.

![[Pasted image 20250206032341.png]]
## HDFS Features

- Fault-tolerance through replication.
- Scalability to handle petabytes of data.
- High throughput for large-scale applications.
- Portability across commodity hardware.
