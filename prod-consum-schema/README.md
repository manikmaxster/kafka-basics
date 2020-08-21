# Producer Consumer With Schema Registery

## Command
kafka-console-consumer --topic example --bootstrap-server broker:9092 \
 --from-beginning \
 --property print.key=true \
 --property key.separator=" : " \
 --key-deserializer "org.apache.kafka.common.serialization.LongDeserializer" \
 --value-deserializer "org.apache.kafka.common.serialization.DoubleDeserializer"

## Reference
https://kafka-tutorials.confluent.io/kafka-console-consumer-primitive-keys-values/kafka.html