# 简介
TiDB 是 PingCAP 公司设计的开源分布式 HTAP (Hybrid Transactional and Analytical Processing) 数据库，结合了传统的 RDBMS 和 NoSQL 的最佳特性。TiDB 兼容 MySQL，支持无限的水平扩展，具备强一致性和高可用性。TiDB 的目标是为 OLTP (Online Transactional Processing) 和 OLAP (Online Analytical Processing) 场景提供一站式的解决方案。

# 特性
TIDB具有如下特性：
- 高度兼容MySQL    
    大多数情况下，无需修改代码就可从MySQL轻松迁移至TIDB，分库分表后的MYSQL集群亦可通过TIDB工具进行实时迁移
- 水平弹性扩展    
    通过简单地增加新节点实现Tidb的水平扩展，按照扩展吞吐或存储，轻松应对高并发、海量数据场景
- 分布式事务    
    TIDB 100% 支持标准ACID事务
- 真正金融级高可用    
     相比于传统主从 (M-S) 复制方案，基于 Raft 的多数派选举协议可以提供金融级的 100% 数据强一致性保证，且在不丢失大多数副本的前提下，可以实现故障的自动恢复 (auto-failover)，无需人工介入。
- 一站式HTAP解决方案    
    TiDB 作为典型的 OLTP 行存数据库，同时兼具强大的 OLAP 性能，配合 TiSpark，可提供一站式 HTAP 解决方案，一份存储同时处理 OLTP & OLAP，无需传统繁琐的 ETL 过程。
- 云原生SQL数据库</br>
    TiDB 是为云而设计的数据库，支持公有云、私有云和混合云，使部署、配置和维护变得十分简单。

# 部署方式
TIDB可以部署在本地和云平台睡觉啊姑娘，支持公有云、私有云和混合云。部署TIDB集群方式有：    
- 使用Ansible部署
- 使用Ansible离线部署
- 使用Docker Compose部署
- 使用Docker部署

# 项目源码
TIDB集群所有组建的源码均可从GitHub上直接访问：
- [TIDB](https://github.com/pingcap/tidb)
- [TIKV](https://github.com/tikv/tikv)
- [PD](https://github.com/pingcap/pd)
- [TiSpark](https://github.com/pingcap/tispark)
- [TIDB Operator](https://github.com/pingcap/tidb-operator)

