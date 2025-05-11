## 1. How much data your publisher program will send to the message broker in one run?
The publisher program will send 5 pieces of data (messages) to the message broker in one run.

## 2. The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber program, what does it mean?
When both the publisher and subscriber use the same URL like `amqp://guest:guest@localhost:5672`, they are connecting to the same RabbitMQ broker running locally. This allows them to send and receive messages through shared queues or exchanges on that broker.

![alt text](PublisherSS1.png)

- The publisher sent 5 event to the message broker. Those event later consumed and processed by the subscriber. 
![alt text](PublisherSS2.png)

- The spike in the graph indicates the message rate, which measures how many messages are sent to the channel within a given time interval. Since the publisher sends several messages to the message broker, the message rate increases, resulting in a spike on the graph.
![alt text](PublisherSS3.png)