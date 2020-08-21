# Producer Consumer Console

## Command

    # Producer
    kafka-console-producer --topic example-topic --broker-list broker:9092\
        --property parse.key=true\
        --property key.separator=":"

    # Consumer
    kafka-console-consumer --topic example-topic --bootstrap-server broker:9092 \
        --from-beginning \
        --property print.key=true \
        --property key.separator="-"

## Reference
https://kafka-tutorials.confluent.io/kafka-console-consumer-producer-basics/kafka.html