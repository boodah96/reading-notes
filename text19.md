#  AWS: Events

### What’s the difference between a FIFO and a standard queue?
FIFO queues have essentially the same features as standard queues, but provide the added benefits of supporting ordering and exactly-once processing and ensure the order in which messages are sent and received is strictly preserved
### How can the server be assured a message was properly received?
When having an event in the client side to emit what received from the server.
### What classic design pattern is best represented by event driven programming?
Most modern programming-languages comprise built-in “event” constructs implementing the observer-pattern components.
### How do you test an event driven system?
Event-driven programming is a paradigm that is widely used in many fields. This paper proposes a method for unit-testing event-driven Processing programs. It allows writing testable Processing programs and test programs in Java. It presents case studies on testing whether mouse and key events are correctly handled.


# Term

- `Serverless API`:API Gateway allows you to build RESTful APIs for real-time two-way communication applications. It also supports containerized and serverless workloads, as well as web applications (source: AWS API Gateway
- `Triggers`:function may have several causes, which are AWS Lambda resources or resources in other services that you customize to invoke your function in response to lifecycle incidents, external requests, or on a timetable
- `Dynamo vs Mongo`: Mongo can be installed anywhere, but Dynamo is only accessible on Amazon Web Services. Dynamo is a small key-value database with JSON support, while Mongo is a JSON-based text store. Dynamo is a key-value query language, while Mongo is a rich query language.
- `Dynamoose vs Mongoose`:  Dynamoose is a Mongoose-style DynamoDB API that allows one to provide a schema and perform CRUD operations on a DynamoDB table. It’s installed via node and configured by task.


 ## Amazon SNS
- Amazon Simple Notification Service (Amazon SNS) is a web service that enables you to build distributed web-enabled applications. Applications can use Amazon SNS to easily push real-time notification messages to interested subscribers over multiple delivery protocols.

- works closely with Amazon Simple Queue Service (Amazon SQS). These services provide different benefits for developers. Amazon SNS allows applications to send time-critical messages to multiple subscribers through a “push” mechanism, eliminating the need to periodically check or “poll” for updates. Amazon SQS is a message queue service used by distributed applications to exchange messages through a polling model, and can be used to decouple sending and receiving components—without requiring each component to be concurrently available. Using Amazon SNS and Amazon SQS together, messages can be delivered to applications that require immediate notification of an event, and also persisted in an Amazon SQS queue for other applications to process at a later time.

#### REFERENCES:
- https://docs.aws.amazon.com/sns/latest/dg/sns-sqs-as-subscriber.html
- https://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/SNS.html