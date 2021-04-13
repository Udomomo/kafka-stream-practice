# kafka-streams-practice
This is a practice of kafka-stream programming with spring-cloud-stream framework.

## Run
- Create fat jar file by `bootJar` task
- Run with configuration
    - If you run Kafka broker in `localhost:9092` (same as default), you don't need to specify the broker address.
    - You can also write configuration in `application.properties`
```
java -jar kafkastream-0.0.1-SNAPSHOT.jar --spring.cloud.stream.bindings.process-in-0.destination=<topic name for consuming> --spring.cloud.stream.kafka.binder.brokers=<broker address>
```

