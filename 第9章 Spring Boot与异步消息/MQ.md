# 第9章 Spring Boot与异步消息

消息队列作为高并发系统的核心组件之一，能够帮助业务系统解构提升开发效率和系统稳定性。主要具有以下优势：

- 削峰填谷（主要解决瞬时写压力大于应用服务能力导致消息丢失、系统奔溃等问题）
- 系统解耦（解决不同重要程度、不同能力级别系统之间依赖导致一死全死）
- 提升性能（当存在一对多调用时，可以发一条消息给消息系统，让消息系统通知相关系统）
- 蓄流压测（线上有些链路不好压测，可以通过堆积一定量消息再放开来压测）

目前主流的MQ主要是RocketMQ、kafka、RabbitMQ

 

**Kafka**是由[Apache软件基金会](https://baike.baidu.com/item/Apache软件基金会)开发的一个开源流处理平台，由[Scala](https://baike.baidu.com/item/Scala)和[Java](https://baike.baidu.com/item/Java/85979)编写。Kafka是一种高吞吐量的[分布式](https://baike.baidu.com/item/分布式/19276232)发布订阅消息系统，它可以处理消费者在网站中的所有动作流数据。 这种动作（网页浏览，搜索和其他用户的行动）是在现代网络上的许多社会功能的一个关键因素。 这些数据通常是由于吞吐量的要求而通过处理日志和日志聚合来解决。 对于像[Hadoop](https://baike.baidu.com/item/Hadoop)一样的[日志](https://baike.baidu.com/item/日志/2769135)数据和离线分析系统，但又要求实时处理的限制，这是一个可行的解决方案。Kafka的目的是通过[Hadoop](https://baike.baidu.com/item/Hadoop)的并行加载机制来统一线上和离线的消息处理，也是为了通过[集群](https://baike.baidu.com/item/集群/5486962)来提供实时的消息。