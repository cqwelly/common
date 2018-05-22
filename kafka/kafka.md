## 启动kafka
- bin/kafka-server-start.sh config/server.properties
- bin/kafka-server-start.sh config/server-1.properties
- bin/kafka-server-start.sh config/server-2.properties

## 常用命令
- 查看消费组
  bin/kafka-run-class.sh kafka.admin.ConsumerGroupCommand --list --new-consumer --bootstrap-server localhost:9092
- 查看topic信息
  bin/kafka-topics.sh --zookeeper localhost:2181/kafka  --describe --topic topic_name


## kafka 监控
- kafka-eagle 
  - https://github.com/smartloli/kafka-eagle
  - https://github.com/linkedin/kafka-monitor
