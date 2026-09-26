# StorageLearn

一个从 **物理介质 → SSD/NVMe → 文件系统 → Block/File/Object → 数据库/缓存/搜索/消息 → 数据仓库/数据湖 → 分布式存储与一致性** 的完整学习站点。

## 已覆盖

### 1. 存储介质与底层设备
- SRAM / DRAM
- NAND / NOR Flash
- HDD / Tape / Optical
- SSD、FTL、GC、Wear Leveling、TRIM
- SATA / NVMe / PCIe

### 2. 三大存储模型
- Block Storage
- File Storage
- Object Storage

### 3. 文件系统
- APFS / NTFS / ext4 / XFS / ZFS / Btrfs
- inode
- Journal
- Copy-on-Write
- Page Cache / Dirty Page / fsync

### 4. 数据软件体系
- SQL：MySQL / PostgreSQL
- Key-Value：Redis / RocksDB / DynamoDB
- Document：MongoDB
- Wide Column：Cassandra / HBase / Bigtable
- Graph：Neo4j
- Time Series：InfluxDB / Prometheus
- Search：Elasticsearch / OpenSearch
- Messaging：Kafka / Pulsar / RabbitMQ / RocketMQ
- OLAP：ClickHouse / Snowflake / BigQuery
- Data Lake / Lakehouse：S3 / Parquet / Iceberg / Delta / Hudi
- Vector DB：Milvus / Qdrant / Weaviate / pgvector

### 5. 五条深度主线
1. SSD / NVMe / 文件系统 / Page Cache
2. MySQL：B+Tree、Buffer Pool、Redo、Undo、MVCC、Lock、Binlog
3. Redis：缓存、穿透/击穿/雪崩、分布式锁、RDB/AOF、Cluster
4. Kafka：Partition、Offset、Consumer Group、消息语义、Replication
5. 分布式存储：Sharding、Replication、Quorum、Raft、CAP

### 6. 架构串联
- 消费金融额度申请端到端数据链路
- 故障推演
- 技术选型矩阵
- 自测题

## 本地运行

零依赖静态站点：

```bash
python3 -m http.server 8080
```

浏览器访问：

```
http://localhost:8080
```

## 学习方法

始终用 5 个问题理解任何存储技术：

1. 数据真正存在哪里？
2. 什么时候算写成功？
3. 机器挂了怎么恢复？
4. 并发冲突怎么解决？
5. 单机撑不住后怎么扩展？
