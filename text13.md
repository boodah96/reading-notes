### Message Queues

1- What does it mean that web sockets are bidirectional? Why is this useful?
Data flows both ways (full-duplex), a web socket can both send and receive which is useful because it allows data to be sent and received on the same channel.

2- Does socket.io use HTTP? Why?
The server take that emit message and the paylod and resopond with and action or another emit message.

3- What happens when a client emits an event?
The event gets passed to the server through websockets. Its a tcp connection from the browser to the server. The connection is full duplex meaning the server can send real time data to the client and vise versa.

4- What happens when a server emits an event?
Whatever client is listening for the event (maybe all, or maybe one specific client) will respond

5- What happens if a client “misses” an event?
Unhandled messages are ignored,the application will still run.
6- How can we mitigate this?
Can avoid missing an event by always having handlers installed and then deciding in the handlers whether to do anything with the message or not


#### Terms:
`Socket`: is one endpoint of a two-way communication link between two programs running on the network. A socket is bound to a port number so that the TCP layer can identify the application that data is destined to be sent to. An endpoint is a combination of an IP address and a port number.

`Web Socket`: is a computer communications protocol, providing full-duplex communication channels over a single TCP connection. The WebSocket protocol was standardized by the IETF as RFC 6455 in 2011, and the WebSocket API in Web IDL is being standardized by the W3C.

`Socket.io`: is a JavaScript library for real-time web applications. It enables real-time, bi-directional communication between web clients and servers. It has two parts: a client-side library that runs in the browser, and a server-side library for node.js. Both components have an identical API.

`Client`: is a piece of computer hardware or software that accesses a service made available by a server as part of the client–server model of computer networks. The server is often (but not always) on another computer system, in which case the client accesses the service by way of a network.

`Server`: is a computer that serves information to other computers. These computers, called clients, can connect to a server through either a local area network or a wide area network, such as the internet. A server is a vital piece of your IT infrastructure.

`OSI Model`: (Open Systems Interconnection Model) is a conceptual framework used to describe the functions of a networking system. The OSI model characterizes computing functions into a universal set of rules and requirements in order to support interoperability between different products and software. In the OSI reference model, the communications between a computing system are split into seven different abstraction 

`layers`: Physical, Data Link, Network, Transport, Session, Presentation, and Application.

`TCP Model`: is not exactly similar to the OSI model. The TCP/IP model consists of five layers: the application layer, transport layer, network layer, data link layer and physical layer. … TCP/IP is a hierarchical protocol made up of interactive modules, and each of them provides specific functionality.

`TCP`: Transmission Control Protocol

`UDP`: User Datagram Protocol is one of the core members of the Internet protocol suite. With UDP, computer applications can send messages, in this case referred to as datagrams, to other hosts on an Internet Protocol (IP) network. Prior communications are not required in order to set up communication channels or data paths.

`Packets`: is a small amount of data sent over a network, such as a LAN or the Internet. Similar to a real-life package, each packet includes a source and destination as well as the content (or data) being transferred.

### Socket
-Reserved events
On each side, the following events are reserved and should not be used as event names by your application:

``connect
connect_error
disconnect
disconnecting
newListener
removeListener
``
-A room is an arbitrary channel that sockets can join and leave. It can be used to broadcast events to a subset of clients

## references
- https://socket.io/docs/v3/rooms/index.html
- https://socket.io/docs/v3/emit-cheatsheet/index.html
- https://en.wikipedia.org/wiki/Internet_protocol_suite