# AWS: API, Dynamo, and Lambda

- ###  What’s the difference between a FIFO and a standard queue?
FIFO queues have essentially the same features as standard queues, but provide the added benefits of supporting ordering and exactly-once processing and ensure the order in which messages are sent and received is strictly preserved
- ### How can the server be assured a message was properly received?
By having an event in the client side to emit what received from the server side.
- ### What classic design pattern is best represented by event driven programming?
The observer pattern
- ### How do you test an event driven system?
Event-driven programming is a paradigm that is widely used in many fields. Processing is a set of programming languages and environments specialized in event-driven programming for interactive graphical applications. It provides only low-level event-handling functions, which imposes difficulty on novice programmers in programming complex behaviors. 

## TERMS
- `Serverless Functions`:An Event-Based Serverless Compute Experience to Accelerate Your Development. $200 Free Credit. Try Popular Products Free. 25+ Products Always Free. Learn by Doing.

- `Cloud Storage`:cloud storage means, you need to grasp what the cloud is. In one line, that’s a resource (usually computing power or storage) that you can access remotely online either for free or for a fee.

- `CDN`: A content delivery network (CDN) refers to a geographically distributed group of servers that work together to provide fast delivery of Internet content

## AWS API Gateway
Amazon API Gateway is a fully managed service that makes it easy for developers to create, publish, maintain, monitor, and secure APIs at any scale. APIs act as the “front door” for applications to access data, business logic, or functionality from your backend services. Using API Gateway, you can create RESTful APIs and WebSocket APIs that enable real-time two-way communication applications. API Gateway supports containerized and serverless workloads, as well as web applications.

## DynamoDB
 is a hosted NoSQL database offered by Amazon Web Services (AWS). It offers: reliable performance even as it scales; a managed experience, so you won't be SSH-ing into servers to upgrade the crypto libraries; a small, simple API allowing for simple key-value access as well as more advanced query patterns.

 ## Refernces:
 - https://www.serverless.com/amazon-api-gateway
 - https://aws.amazon.com/ar/dynamodb/