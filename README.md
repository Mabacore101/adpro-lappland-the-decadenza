## 1. How much data your publisher program will send to the message broker in one run?
The publisher program will send 5 data to the message broker in one run.
## 2. The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber program, what does it mean?
When both the publisher and subscriber use the same URL like `amqp://guest:guest@localhost:5672`, they are connecting to the same RabbitMQ broker running locally. This allows them to send and receive messages through shared queues or exchanges on that broker.
