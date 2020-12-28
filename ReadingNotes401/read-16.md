# AWS:Cloud Servers

**1.What’s the difference between a FIFO and a standard queue?**

A standard queue is less organized in how it delivers messages and might send duplicates, it has a higher TFO while a FIFO queue is strict and will successfully deliver a message at least once and has lower TFO.

**2.How can the server be assured a message was properly received?**

It receives confirmation.

**3.What classic design pattern is best represented by event driven programming?**

Subscribe/observer pattern

**4.How do you test an event driven system?**

Create a test for each event handler


## Terms

**Server** - a program that connects to, receives and sends information to the client

**Pub/Sub** - A design pattern used for building dynamic applications where modules can communicate back and forth without being reliant on one another.[source](https://jsmanifest.com/the-publish-subscribe-pattern-in-javascript/)

**WRRC** - Web Request Response Cycle

### PREP MATERIALS

[Virtual Machines](https://www.youtube.com/watch?v=yIVXjl4SwVo)

[VMS and the Cloud](https://www.youtube.com/watch?v=l0DfHUWMjsU)

[AWS EC2](https://aws.amazon.com/ec2/)

[EC2 for Humans](https://www.youtube.com/watch?v=lZMkgOMYYIg)

[Elastic Beanstalk](https://www.youtube.com/watch?v=SrwxAScdyT0)