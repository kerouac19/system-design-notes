# [System Design Interview - An Insider's Guide (Vol 1 and 2)](https://bytebytego.com/courses/system-design-interview)

这些笔记基于 System Design Interview 两卷：[Vol 1 and Vol 2 2nd Ed](https://www.goodreads.com/book/show/54109255-system-design-interview-an-insider-s-guide)

在线版：https://pagefy.io/system-design/system-design-interview-by-alex-xu

**说明：** 原文笔记仍在完善；中文稿按章推进。第 5 章及之后的中文链接会随翻译补齐。

 * [第 1 章 - 从零扩展到百万用户](./01.%20Scaling/README.zh.md)
 * [第 2 章 - 粗略估算](./02.%20Back%20Of%20the%20Envelope%20Estimation/README.zh.md)
 * [第 3 章 - 系统设计面试框架](./03.%20System%20Design%20Framework/README.zh.md)
 * [第 4 章 - 设计限流器](./04.%20Rate%20Limiter/README.zh.md)
 * [第 5 章 - 设计一致性哈希](./05.%20Consistent%20Hashing/README.zh.md)
 * [第 6 章 - 设计键值存储](./06.%20Key-Value%20Store/README.zh.md)
 * [第 7 章 - 设计分布式唯一 ID 生成器](./07.%20Unique-Id%20Generator/README.zh.md)
 * [第 8 章 - 设计短链系统](./08.%20URL%20Shortener/README.zh.md)
 * [第 9 章 - 设计网络爬虫](./09.%20Web%20Crawler/README.zh.md)
 * [第 10 章 - 设计通知系统](./10.%20Notification%20System/README.zh.md)
 * [第 11 章 - 设计信息流系统](./11.%20News%20Feed%20System/README.zh.md)
 * [第 12 章 - 设计聊天系统](./12.%20Chat%20System/README.zh.md)
 * [第 13 章 - 设计搜索自动补全](./13.%20Search%20Autocomplete/README.zh.md)
 * [第 14 章 - 设计 YouTube](./14.%20Youtube/README.zh.md)
 * [第 15 章 - 设计 Google Drive](./15.%20Google%20Drive/README.zh.md)
 * [第 16 章 - 设计邻近服务](./16.%20Proximity%20Service/README.zh.md)
 * [第 17 章 - 设计附近的好友](./17.%20Nearby%20Friends/README.zh.md)
 * [第 18 章 - 设计 Google Maps](./18.%20Google%20Maps/README.zh.md)
 * [第 19 章 - 设计分布式消息队列](./19.%20Distributed%20Message%20Queue/README.zh.md)
 * [第 20 章 - 设计指标监控与告警系统](./20.%20Metrics%20Monitoring%20and%20Alerting%20System/README.zh.md)
 * [第 21 章 - 设计广告点击事件聚合](./21.%20Ad%20Click%20Event%20Aggregation/README.zh.md)
 * [第 22 章 - 设计酒店预订系统](./22.%20Hotel%20Reservation%20System/README.zh.md)
 * [第 23 章 - 设计分布式邮件服务](./23.%20Distributed%20Email%20Service/README.zh.md)
 * [第 24 章 - 设计类 S3 对象存储](./24.%20S3-like%20Object%20Storage/README.zh.md)
 * [第 25 章 - 设计实时游戏排行榜](./25.%20Real-time%20Gaming%20Leaderboard/README.zh.md)
 * [第 26 章 - 设计支付系统](./26.%20Payment%20System/README.zh.md)
 * [第 27 章 - 设计数字钱包](./27.%20%20Digital%20Wallet/README.zh.md)
 * [第 28 章 - 设计证券交易所](./28.%20Stock%20Exchange/README.zh.md)

# 延伸阅读

### 限流
- [熔断算法](https://martinfowler.com/bliki/CircuitBreaker.html)
- [Uber 限流器](https://github.com/uber-go/ratelimit/blob/master/ratelimit.go)

### 一致性哈希
- [一致性哈希](https://tom-e-white.com/2007/11/consistent-hashing.html)
- [CS168: 引言与一致性哈希](http://theory.stanford.edu/~tim/s16/l/l1.pdf)
- [Apache Cassandra](http://www.cs.cornell.edu/Projects/ladis2009/papers/Lakshman-ladis2009.PDF)
- [Scaling Discord](https://blog.discord.com/scaling-elixir-f9b8e1e7c29b)
- [Google Maglev](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44824.pdf)

### 键值存储
- [Amazon Dynamo](https://www.allthingsdistributed.com/files/amazon-dynamo-sosp2007.pdf)
- [Cassandra 架构](https://docs.datastax.com/en/archived/cassandra/3.0/cassandra/architecture/archIntro.html)
- [Google BigTable 架构](https://static.googleusercontent.com/media/research.google.com/en//archive/bigtable-osdi06.pdf)
- [Amazon Dynamo DB 内部](https://www.allthingsdistributed.com/2007/10/amazons_dynamo.html)
- [Amazon Dynamo DB 中的设计模式](https://www.youtube.com/watch?v=HaEPXoXVf2k)
- [Amazon Dynamo DB 内部机制](https://www.youtube.com/watch?v=yvBR71D0nAQ)

### 唯一 ID 生成器
- [Ticket Servers: 低成本的分布式唯一主键](https://code.flickr.net/2010/02/08/ticket-servers-distributed-unique-primary-keys-on-the-cheap)
- [Snowflake](https://blog.twitter.com/engineering/en_us/a/2010/announcing-snowflake.html)

### 网络爬虫
- [Web Crawling](http://infolab.stanford.edu/~olston/publications/crawling_survey.pdf)
- [Google 动态渲染](https://developers.google.com/search/docs/guides/dynamic-rendering)

### 聊天系统
- [Discord 如何存储数十亿条消息](https://discord.com/blog/how-discord-stores-billions-of-messages)
- [Flannel：让 Slack 能扩展的应用层边缘缓存](https://slack.engineering/flannel-an-application-level-edge-cache-to-make-slack-scale/)

### 搜索自动补全
- [我们如何构建 Prefixy](https://medium.com/@prefixyteam/how-we-built-prefixy-a-scalable-prefix-search-service-for-powering-autocomplete-c20f98e2eff1)
- [Prefix Hash Tree](https://people.eecs.berkeley.edu/~sylvia/papers/pht.pdf)

### YouTube
- [YouTube 架构](http://highscalability.com/youtube-architecture)
- [YouTube 扩展性 2012](https://www.youtube.com/watch?v=w5WVu624fY8)
- [大规模转码](https://www.egnyte.com/blog/2018/12/transcoding-how-we-serve-videos-at-scale/)
- [Facebook 视频直播](https://engineering.fb.com/ios/under-the-hood-broadcasting-live-video-to-millions/)
- [Netflix 大规模视频编码](https://netflixtechblog.com/high-quality-video-encoding-at-scale-d159db052746)
- [Netflix 基于镜头的编码](https://netflixtechblog.com/optimized-shot-based-encodes-now-streaming-4b9464204830)

### Google Drive
- [差分同步](https://neil.fraser.name/writing/sync/)
- [差分同步视频](https://www.youtube.com/watch?v=S2Hp_1jqpY8)
- [Dropbox 如何扩展](https://www.youtube.com/watch?v=PE4gwstWhmc&feature=youtu.be)
