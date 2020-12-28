# Event Driven Architecture

**1.What’s the difference between a FIFO and a standard queue?**

A standard queue is less organized in the way and number of times it delivers a message while a FIFO queue is more strict with how messages are sent and received. The main difference is the [TFO - Transactions Per Second](https://medium.com/awesome-cloud/aws-difference-between-sqs-standard-and-fifo-first-in-first-out-queues-28d1ea5e153)

**2.How can the server be assured a message was properly received?**

A confirmation is sent back from the receiving end.

**3.What classic design pattern is best represented by event driven programming?**

Subscribe/observer pattern

**4.How do you test an event driven system?**

Create a test that uses an [automation process that scaffold up the unit testing environment](https://blog.gurock.com/event-driven-application-architectures/)


## Terms

**FIFO Queue** - Messages are sent and received in the same order and each message is guaranteed to be delivered at least once, while duplicates are removed.[source](https://medium.com/awesome-cloud/aws-difference-between-sqs-standard-and-fifo-first-in-first-out-queues-28d1ea5e153)

**Pub/Sub** - A design pattern used for building dynamic applications where modules can communicate back and forth without being reliant on one another.[source](https://jsmanifest.com/the-publish-subscribe-pattern-in-javascript/)

### PREP MATERIALS

[AWS SNS and SQS](https://www.youtube.com/watch?v=mXk0MNjlO7A)

[Azure Event Hubs](https://www.youtube.com/watch?v=DDDjFQSQyF4)

[FIFO Queues within AWS and Azure](https://medium.com/@vunvulear/fifo-and-queues-inside-aws-and-azure-d21145473d5a)
