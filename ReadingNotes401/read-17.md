# AWS: S3 and Lambda

**1.What’s the difference between a FIFO and a standard queue?**

A standard queue is less organized in how it delivers messages and might send duplicates, it has a higher TFO while a FIFO queue is strict and will successfully deliver a message at least once and has lower TFO.

**2.How can the server be assured a message was properly received?**

It receives confirmation.

**3.What classic design pattern is best represented by event driven programming?**

Subscribe/observer pattern

**4.How do you test an event driven system?**

Create a test for each event handler

## Terms

**Server Instances** - A collection of SQL Server DB's that are run by a single SQL Server service or instance. Details of each server instance can be viewed in the service console which can be web-based or command-line based.[source](https://www.techopedia.com/definition/32149/server-instance#:~:text=A%20server%20instance%20is%20a,based%20or%20command%2Dline%20based.)

**Containers** - A unit of software that holds code and it's dependencies so that an application can run quickly and more reliably.

**Cloud Services** - External services from a provider/giant server that allocates as much space for data that your application will need as it grows.

**Cloud Architecture** - front en, back end, cloud based deliver + network.[source](https://en.wikipedia.org/wiki/Cloud_computing_architecture)

**AWS** - Amazon Web Services(cloud service)

**EC2/Beanstalk vs Heroku** - EC2/Beanstalk are AWS services while Heroku uses AWS. EC2/Beanstalk has the ability to support resized applications while Heroku is limited.

### PREP MATERIALS

[AWS S3](https://aws.amazon.com/s3/)

[AWS Lambda Basics](https://www.serverless.com/aws-lambda)

[AWS Lambda Functions](https://aws.amazon.com/lambda/)

[CDN](https://cyberhoot.com/cybrary/content-delivery-network-cdn/)

# AWS: S3 and Lambda

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

**Serverless Function** - 

### PREP MATERIALS

[AWS S3](https://aws.amazon.com/s3/)

[AWS Lambda Basics](https://www.serverless.com/aws-lambda)

[AWS Lambda Functions](https://aws.amazon.com/lambda/)

[CDN](https://cyberhoot.com/cybrary/content-delivery-network-cdn/)