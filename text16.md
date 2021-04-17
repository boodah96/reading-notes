## AWS: Cloud Servers

### What’s the difference between a FIFO and a standard queue?

FIFO queues have essentially the same features as standard queues, but provide the added benefits of supporting ordering and exactly-once processing. FIFO queues provide additional features that help prevent unintentional duplicates from being sent by message producers or from being received by message consumers.
### How can the server be assured a message was properly received?
By having the client emit a “received” event back to the server upon receipt of the message

### What classic design pattern is best represented by event driven programming?
The observer pattern is a software design pattern in which an object, named the subject, maintains a list of its dependents, called observers, and notifies them automatically of any state changes, usually by calling one of their methods. It is mainly used for implementing distributed event handlingsystems, in "event driven" software.

### sHow do you test an event driven system?
 Integration tests show the pieces come together successfully, but we can't always test every interaction. The big assumption is if the unit tests passed, the pieces should work well together regardless of what they're doing.

 ## Terms
`Server`: a device that manages and provide services to the network.

`Pub/Sub`: stands for publish/subscribe, it's a real time, flexible, and reliable messaging service to publish and subscribe to asynchronous events.

`WRRC`: stands for web response request cycle, it's a graph that represent outgoing and incoming requests and responses from each device in a certain application.

### Virtual Machines:
 it's a machine that runs simultaneously on another device by sharing its resources with the original device. This service can be provided by multiple companies where you can setup your machine (operating system, memory, processor, .... etc) and you can run it as if it was a device between your hands.

### AMAZON EC2: 
stands for elastic computing cloud, it's web services provided by amazon where you can setup your instances that suites your application and run them as normal machines.


## AWS

Cloud computing gives you access to servers, storage, databases, and a broad set of application services over the Internet. A cloud services provider such as Amazon Web Services, owns and maintains the network-connected hardware required for these application services, while you provision and use what you need via a web application.

Types of Cloud Computing. Cloud computing has three main types that are commonly referred to as Infrastructure as a Service (IaaS), Platform as a Service (PaaS), and Software as a Service (SaaS). .

Amazon Web Services (AWS), Google Cloud Platform (GCP), and Microsoft Azure are among the best players in the cloud computing world.

 ## references
 - https://aws.amazon.com/ar/ec2/?ec2-whats-new.sort-by=item.additionalFields.postDateTime&ec2-whats-new.sort-order=desc
 - https://www.youtube.com/watch?v=lZMkgOMYYIg
 - https://en.wikipedia.org/wiki/Virtual_machine