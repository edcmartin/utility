# kafka shell 命令
1. 创建topic
    ./bin/kafka-topics.sh --zookeeper node:2181 --create --topic topic_name --partitions 2 --replication-factor 2
2. 查看所有topic
    bin/kafka-topics.sh --zookeeper node:2181 --list
3. 指定topic信息
    bin/kafka-topics.sh --zookeeper node:2181 --describe --topic topic_name
4. 控制台向topic生产数据
    bin/kafka-console-producer.sh --broker-list node:9092 --topic topic_name
5. 控制台消费topic的数据
    bin/kafka-console-consumer.sh --zookeeper node0:2181 --topic topic_name
    