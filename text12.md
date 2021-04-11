## Socket.io
- 1.What is the benefit of transforming data into packets?
Allows for data to be transferred fast and efficiently over the network and minimizes the transmission latency

- 2.UDP is often refereed to as a connectionless protocol. Why is this?

No connection needs to be established between the source and destination before you transmit data.

- 3.Can a socket server application have multiple socket connections?
server socket listens on a single port. but Multiple connections on the same server can share the same server-side IP/Port pair as long as they are associated with different client-side IP/Port pairs, and the server would be able to handle as many clients as available system resources allow it to
- 4.Can a socket connection application be connected to multiple socket servers?

If your program is a client to multiple servers, use one socket per server.

- 5.Can an application be both a socket server and a socket connection?
Yes.

#### Term
- `Observer Pattern:`is a software design pattern in which an object, named the subject, maintains a list of its dependents, called observers, and notifies them automatically of any state changes, usually by calling one of their methods.

- `Listener`: is a procedure or function in a computer program that waits for an event to occur. The listener is programmed to react to an input or signal by calling the event’s handler. The term event listener is often specific to Java and JavaScript.

- `Event Handler`: is a callback routine that operates asynchronously and handles inputs received into a program.
Event Driven Programming: is a programming paradigm in which the flow of the program is determined by events such as user actions (mouse clicks, key presses), sensor outputs, or message passing from other programs or threads.

- `Event Loop`: is a programming construct or design pattern that waits for and dispatches events or messages in a program. The event loop works by making a request to some internal or external “event provider” (that generally blocks the request until an event has arrived), then calls the relevant event handler (“dispatches the event”). The event loop is also sometimes referred to as the message dispatcher, message loop, message pump, or run loop.

- ` Event Queue`: is a repository where events from an application are held prior to being processed by a receiving program or system. Event queues are often used in the context of an enterprise messaging system.

- `Call Stack`: is a stack data structure that stores information about the active subroutines of a computer program. This kind of stack is also known as an execution stack, program stack, control stack, run-time stack, or machine stack, and is often shortened to just “the stack”

### Socket.IO
 - enables real-time bidirectional event-based communication.
 - It works on every platform, browser or device, focusing equally on reliability and speed.
 - It is built on top of the WebSockets API (Client side) and Node.js, it is one of the most depended upon library on npm.
 - It automatically upgrades the requirement to WebSocket if needed.
 - It is a custom real-time transport protocol implementation on top of other protocols.

**Difference Between WebSocket and Socket.io**
- WebSocket is the communication Protocol that provides bidirectional communication between the Client and the Server over a TCP connection; WebSocket remains open all the time, so they allow real-time data transfer. When clients trigger the request to the server, it does not close the connection on receiving the response; it rather persists and waits for the Client or server to terminate the request.


- Socket.IO is a library that enables real-time and full-duplex communication between the Client and the Web servers. It uses the WebSocket protocol to provide the interface. Generally, it is divided into two parts; both WebSocket vs Socket.io are event-driven libraries.