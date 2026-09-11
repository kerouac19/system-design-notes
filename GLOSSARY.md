# 术语表

系统设计面试笔记中文稿的用词与格式约定。各章 `README.zh.md` 与 `images-zh/` 必须遵守。

## 硬约定

- 中文为主。某一术语在**该章第一次**出现时括注英文，后文只用中文。范围是每一章，不是全书。
- 缩写不译：`QPS`、`WAL`、`CDN`、`API`、`CAP`、`HTTP`、`JSON`、`SQL`、`TTL`、`DoS`、`FIFO` 等。
- 代码、路径、字段名、URL、图片文件名不译。
- 产品名 / 语言名不译：`Redis`、`Lua`、`MySQL`、`Kafka`、`YouTube`、`Google Drive`、`Google Maps`、`S3` 等。
- HTTP 状态码保留数字（如 `429`）；原因短语可译（`429: 请求过多`）。
- `C:` / `I:` 写成「候选人：…」和「面试官：…」。示例：候选人：限流器是做在客户端还是服务端？ / 面试官：做服务端 API 限流器。

- 图内文字用下表中文名，图上不括注英文；需要时写在 `alt`。
- 时间戳（`1:00:00`）、百分数（`70%`）不改。
- 明显笔误只改中文稿，不改英文文件。
- 表里已有的中文名，后面章节必须沿用。要改译，先改本表再全局替换。
- 只收会跨章出现的词。一章里的一次性说法不必进表，但同一章内要前后一致。

## 永不翻译

| 原文 | 原因 |
|------|------|
| `API` `HTTP` `DoS` `FIFO` `QPS` `CDN` `WAL` `CAP` `JSON` `SQL` `TTL` | 缩写 |
| `Redis` `Lua` `MySQL` `Kafka` `YouTube` `Google Drive` `Google Maps` `S3` | 产品 / 品牌 / 语言 |
| `DNS` `LRU` `SPOF` `SLA` `MAU` `DAU` `NoSQL` `PostgreSQL` `GeoDNS` | 缩写 / 产品 |
| `UUID` `WebSocket` `SHA-1` `DAG` `BFS` `DFS` `ZooKeeper` `Cassandra` `Dynamo` `Akamai` `Maglev` | 缩写 / 产品 / 算法名 |
| `GPS` `SMTP` `IMAP` `PSP` `ISR` `TCC` `Saga` `Raft` `Geohash` `S2` `Stripe` `Grafana` `InfluxDB` `RocksDB` `CQRS` | 缩写 / 产品 / 协议 |
| `429` | HTTP 状态码 |
| 路径、文件名、URL、代码标识符 | 总原则 |

## 对照表

| 英文 | 中文 | 备注 |
|------|------|------|
| rate limiter / rate limiting | 限流器 / 限流 | 名词用「限流器」，动作/泛称用「限流」 |
| throttle / throttled | 限流 / 被限流 | 不另造「节流」 |
| token bucket | 令牌桶 | |
| leaking bucket | 漏桶 | 不用「泄漏桶」 |
| fixed window counter | 固定窗口计数器 | |
| sliding window log | 滑动窗口日志 | |
| sliding window counter | 滑动窗口计数器 | |
| middleware | 中间件 | |
| API gateway | API 网关 | |
| client | 客户端 | 图内同此 |
| API servers | API 服务器 | |
| cache / cached rules | 缓存 / 缓存规则 | 图上 `CACHE` 写成「缓存」 |
| workers | 工作节点 | |
| rules | 规则 | |
| message queue | 消息队列 | |
| race condition | 竞态条件 | |
| eventual consistency | 最终一致性 | |
| burst | 突发流量 | |
| queue | 队列 | |
| refiller | 补充器 | |
| rolling minute | 滚动分钟 | |
| rate limited request | 被限流的请求 | |
| successful request | 成功的请求 | |
| load balancer | 负载均衡器 | |
| vertical scaling | 垂直扩展 | |
| horizontal scaling | 水平扩展 | |
| master / slave | 主库 / 从库 | 图内同此 |
| shard / sharding | 分片 | |
| stateless | 无状态 | |
| stateful | 有状态 | |
| web server | Web 服务器 | |
| web tier | Web 层 | |
| data tier | 数据层 | |
| producer / publisher | 生产者 / 发布者 | |
| consumer / subscriber | 消费者 / 订阅者 | |
| origin server | 源站 | |
| session | 会话 | |
| consistent hashing | 一致性哈希 | |
| news feed | 信息流 | |
| high availability | 高可用 | |
| single point of failure | 单点故障 | 括注 `SPOF` |
| celebrity problem | 热点问题 | |
| denormalization | 反规范化 | |
| user | 用户 | 图内同此 |
| rehashing | 重哈希 | |
| hash ring | 哈希环 | |
| virtual node | 虚拟节点 | |
| hotspot | 热点 | |
| key-value store | 键值存储 | |
| CAP theorem | CAP 定理 | `CAP` 三字母不译 |
| quorum | 法定人数 | |
| gossip protocol | Gossip 协议 | Gossip 保留 |
| merkle tree | Merkle 树 | 英文文件名 `merkel-tree.png` 不改 |
| vector clock | 向量时钟 | |
| hinted handoff | 暗示移交 | |
| sloppy quorum | 宽松法定人数 | |
| ticket server | 票据服务器 | |
| hash function | 哈希函数 | |
| URL shortener | 短链系统 | |
| web crawler | 网络爬虫 | |
| URL frontier | URL 前沿 | |
| fan-out / fanout | 扇出 | |
| long polling | 长轮询 | |
| polling | 轮询 | |
| presence | 在线状态 | |
| autocomplete | 自动补全 | |
| trie | 字典树 | 首次可写 字典树（trie） |
| transcoding | 转码 | |
| metadata | 元数据 | |
| delta sync | 增量同步 | |
| notification | 通知 | |
| heartbeat | 心跳 | |
| service discovery | 服务发现 | |
| 301 / 302 | 301 / 302 | 状态码不译 |
| Bloom filter | 布隆过滤器 | |
| coordinator | 协调者 | |
| replica | 副本 | |
| strong consistency | 强一致性 | |
| commit log | 提交日志 | |
| data center | 数据中心 | |
| geohash | Geohash | 不译算法名；正文可写 Geohash |
| quadtree | 四叉树 | |
| pub/sub | 发布/订阅 | |
| map tile | 地图瓦片 | |
| broker | Broker | 消息队列场景保留 Broker |
| topic | 主题 | |
| partition | 分区 | 已有 shard/分片；消息队列用「分区」 |
| consumer group | 消费者组 | |
| in-sync replica | 同步副本 | 括注 ISR |
| watermark | 水位线 | |
| tumbling window | 滚动窗口 | |
| idempotency | 幂等 | |
| optimistic locking | 乐观锁 | |
| pessimistic locking | 悲观锁 | |
| object storage | 对象存储 | |
| erasure coding | 纠删码 | |
| leaderboard | 排行榜 | |
| sorted set | 有序集合 | |
| double-entry ledger | 复式记账 | |
| reconciliation | 对账 | |
| event sourcing | 事件溯源 | |
| matching engine | 撮合引擎 | |
| order book | 订单簿 | |
| multicast | 组播 | |
| colocation | 托管 | |
| geospatial index | 地理空间索引 | |
| availability zone | 可用区 | |
| geofence / geofencing | 地理围栏 | |
| exactly-once | 精确一次 | |
| at-least-once | 至少一次 | |
| at-most-once | 至多一次 | |
