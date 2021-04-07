
# Event Driven Applications

- ### Why is access control important?

Access control is a fundamental component of security compliance programs that ensures security technology and access control policies are in place to protect confidential information, such as customer data.
- ### Describe an application that would need access control.
  - Account management;
  - Mapping of user rights to business and process requirements;
  - Mechanisms that enforce policies over information flow;
  - Limits on the number of concurrent sessions;
  - Session lock after a period of inactivity;

- ### What is a role used for?
it used to restriction the capabilities of some users so some can (read,write,update and delete) and som can only do some of these capabilities


- ### Why is role based access control more scalable than discretionary or mandatory access control?
  - Role Based Access Control (RBAC), also known as Non discretionary Access Control, takes more of a real world approach to structuring access control. Access under RBAC is based on a user's job function within the organization to which the computer system belongs.
  - Unlike Mandatory Access Control (MAC) where access to system resources is controlled by the operating system (under the control of a system administrator), Discretionary Access Control (DAC) allows each user to control access to their own data. DAC is typically the default access control mechanism for most desktop operating systems.


### TREM
**Authorization**: giving permission to access data based on some criteria or applying set of rules the controls the access of something.

**Role Based Access Control**: rules and policies that controls the access of data based on roles of websites visitors.

**Capabilities**: the things that visitors can do in a website.


### Event-Driven Programming 

- Event-Driven Programming is a logical pattern that we can choose to confine our programming within to avoid issues of complexity and collision.

- Event-Driven Programming makes use of the following concepts:

    - An Event Handler is a callback function that will be called when an event is triggered.
    - A Main Loop listens for event triggers and calls the associated event handler for that event. 

- The Object Oriented approach promotes the idea that all behavior of an individual unit (or object) be handled from code within that unit. Using this approach, applications are built with many different units that all speak to and interact with each other.

### REFERNCES
- https://owasp.org/www-community/Access_Control
- https://www.digitalocean.com/community/tutorials/nodejs-event-driven-programming