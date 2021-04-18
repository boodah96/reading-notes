# AWS: S3 and Lambda

- What’s the difference between a FIFO and a standard queue?
FIFO queues have essentially the same features as standard queues, but provide the added benefits of supporting ordering and exactly-once processing. FIFO queues provide additional features that help prevent unintentional duplicates from being sent by message producers or from being received by message consumers

- How can the server be assured a message was properly received?
A Message Authentication Code (MAC) is a tag attached to a message to ensure the integrity and authenticity of the message. It is derived by applying a MAC algorithm to a message in combination with a secret key.

- What classic design pattern is best represented by event driven programming?
The observer pattern is a software design pattern in which an object, named the subject, maintains a list of dependents, called observers.

- How do you test an event driven system?
Event-driven programming is a paradigm that is widely used in many fields. This paper proposes a method for unit-testing event-driven Processing programs. It allows writing testable Processing programs and test programs in Java. It presents case studies on testing whether mouse and key events are correctly handled.

## TERMS


- `Server Instances`: is a collection of SQL Server databases which are run by a solitary SQL Server service or instance. The details of each server instance can be viewed on the service console which can be web-based or command-line based.

- `Containers`: is a standard unit of software that packages up code and all its dependencies so the application runs quickly and reliably from one computing environment to another. … Available for both Linux and Windows-based applications, containerized software will always run the same, regardless of the infrastructure.

- `Cloud Services`: refers to a wide range of services delivered on demand to companies and customers over the internet.

- `Cloud Architecture`: refers to the various components in terms of databases, software capabilities, applications, etc. engineered to leverage the power of cloud resources to solve business problems. Cloud architecture defines the components as well as the relationships between them.

- `AWS`: Amazon Web Services is the world’s most comprehensive and broadly adopted cloud platform, offering over 200 fully featured services from data centers globally. Millions of customers—including the fastest-growing startups, largest enterprises, and leading government agencies—are using AWS to lower costs, become more agile, and innovate faster.

- `Heroku`: is a platform as a service (PaaS) that enables developers to build, run, and operate applications entirely in the cloud. 
`EC2/Beanstalk`: is an easy-to-use service for deploying and scaling web applications and services developed with Java, . NET, PHP, Node. … At the same time, you retain full control over the AWS resources powering your application and can access the underlying resources at any time.

## AWS Lambda 
AWS Lambda is a serverless compute service that lets you run code without provisioning or managing servers, creating workload-aware cluster scaling logic, maintaining event integrations, or managing runtimes. With Lambda, you can run code for virtually any type of application or backend service - all with zero administration. Just upload your code as a ZIP file or container image, and Lambda automatically and precisely allocates compute execution power and runs your code based on the incoming request or event, for any scale of traffic. You can set up your code to automatically trigger from 140 AWS services or call it directly from any web or mobile app. You can write Lambda functions in your favorite language (Node.js, Python, Go, Java, and more) and use both serverless and container tools, such as AWS SAM or Docker CLI, to build, test, and deploy your functions.

## Amazon S3
Amazon Simple Storage Service (Amazon S3) is an object storage service that offers industry-leading scalability, data availability, security, and performance. This means customers of all sizes and industries can use it to store and protect any amount of data for a range of use cases, such as data lakes, websites, mobile applications, backup and restore, archive, enterprise applications, IoT devices, and big data analytics. Amazon S3 provides easy-to-use management features so you can organize your data and configure finely-tuned access controls to meet your specific business, organizational, and compliance requirement.

## references
- https://aws.amazon.com/ar/s3/
- https://www.serverless.com/aws-lambda