# AWS: API, Dynamo

**1.What’s the difference between a FIFO and a standard queue?**

A standard queue is less organized in how it delivers messages and might send duplicates, it has a higher TFO while a FIFO queue is strict and will successfully deliver a message at least once and has lower TFO.

**2.How can the server be assured a message was properly received?**

It receives confirmation.

**3.What classic design pattern is best represented by event driven programming?**

Subscribe/observer pattern

**4.How do you test an event driven system?**

Create a test for each event handler

## Terms

**Serverless Function** - event driven functions (lambda) that can be used directly in AWS/third servers.

**Cloud Storage** - Storage that is external from local environment that is flexible in storage space depending on how much you want to pay.

**CDN** - Content Delivery Network(servers that work together to quickly deliver internet content)[source](https://www.cloudflare.com/learning/cdn/what-is-a-cdn/)

### PREP MATERIALS

[AWS API Gateway Overview](https://www.serverless.com/amazon-api-gateway)

[AWS API Gateway](https://aws.amazon.com/api-gateway/)

[AWS DynamoDB Guide](https://www.dynamodbguide.com/what-is-dynamo-db/)

[AWS DynamoDB](https://aws.amazon.com/dynamodb/)

[Dynamoose](https://dynamoosejs.com/getting_started/Introduction)