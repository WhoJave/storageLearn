# StorageLearn

一个面向软件开发者 / 架构学习者的深度存储体系学习页面。

核心学习主线：

1. SSD / NVMe / 文件系统 / Page Cache
2. MySQL：B+Tree、Buffer Pool、Redo/Undo、MVCC、锁、Binlog
3. Redis：缓存、数据结构、分布式锁、持久化、Cluster
4. Kafka：Partition、Offset、Consumer Group、可靠性语义、复制
5. 分布式存储：Sharding、Replication、Quorum、Raft、CAP

## 本地运行

这是零依赖静态站点，直接打开 `index.html` 即可。推荐：

```bash
python3 -m http.server 8080
```

然后访问 `http://localhost:8080`。

## 设计目标

不是罗列产品名，而是围绕五个底层问题建立知识框架：

- 数据真正存在哪里？
- 什么时候算写成功？
- 机器挂了怎么恢复？
- 并发冲突怎么解决？
- 单机撑不住以后怎么扩展？

页面包含分层总览、端到端数据链路、五条主线深度拆解、故障推演、技术对比与自测问题。
