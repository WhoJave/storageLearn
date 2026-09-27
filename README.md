# StorageLearn

一个面向开发者、架构学习者的现代存储系统深度学习站点。

这不是“产品列表”，而是围绕 **数据在哪里、什么时候算写成功、如何恢复、如何处理并发、如何扩展** 建立统一心智模型。

## 页面结构

- `index.html`：完整全景首页，7 层体系、基础技术、五条主线摘要、端到端链路、选型矩阵、自测
- `catalog.html`：完整技术目录，重点回答“市场上有哪些存储介质与存储软件，每类解决什么问题”
- `deep-dive.html`：五条主线深挖
  - SSD / NVMe / 文件系统 / Page Cache
  - MySQL：B+Tree、Buffer Pool、Redo、Undo、MVCC、Lock、Binlog
  - Redis：数据结构、Cache Aside、穿透/击穿/雪崩、锁、RDB/AOF、Cluster
  - Kafka：Partition、Offset、Consumer Group、At-least-once、复制
  - 分布式：Sharding、Replication、Quorum、Raft、CAP
- `scenarios.html`：真实架构与故障推演
  - 消费金融注册 / 授信 / 借款 / 还款
  - 电商多存储组合
  - 日志平台
  - AI / RAG
  - 断电、锁过期、重复消费、主库故障

## 已覆盖的技术范围

### 物理与设备
SRAM、DRAM、NAND、NOR、HDD、Tape、Optical、SSD、FTL、GC、Wear Leveling、TRIM、SATA、SAS、NVMe、PCIe。

### 存储模型
Block Storage、File Storage、Object Storage。

### 文件系统
APFS、NTFS、ext4、XFS、ZFS、Btrfs、inode、Journal、Copy-on-Write、Page Cache、Dirty Page、fsync。

### 数据软件
MySQL、PostgreSQL、Redis、MongoDB、Cassandra、HBase、Neo4j、InfluxDB、Prometheus、Elasticsearch、OpenSearch、Kafka、Pulsar、RabbitMQ、RocketMQ、ClickHouse、Snowflake、BigQuery、Redshift、Doris、StarRocks。

### 数据湖 / AI
S3、HDFS、Parquet、ORC、Iceberg、Delta Lake、Hudi、Milvus、Qdrant、Weaviate、Pinecone、pgvector。

### 分布式与云原生
Ceph、Replication、Erasure Coding、Sharding、Consistent Hashing、Quorum、Raft、CAP、Kubernetes PVC/PV/CSI、Backup、3-2-1、Git Content-Addressed Storage。

## 推荐学习方式

每遇到一个存储技术，都回答 5 个问题：

1. 数据真正存在哪里？
2. 什么时候算写成功？
3. 机器挂了怎么恢复？
4. 并发冲突怎么解决？
5. 单机撑不住后怎么扩展？

然后继续追问：

- 它为了弥补下一层的什么不足而存在？
- 它牺牲了什么换来了什么？
- 如果不用它，系统会在哪个真实场景中出问题？

## 本地运行

```bash
python3 -m http.server 8080
```

访问：

```
http://localhost:8080
```
