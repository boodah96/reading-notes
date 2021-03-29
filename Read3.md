1-  3 real world use cases where you’d want to change the request with custom middleware:
- Data management
- Error handling
- Authentication
2- True or false: The route handler is middleware? 
False

3- In what ways can a middleware function end the process and send data to the browser?
 if a middleware needs to end the request-response early, simply do not call next() but make sure that the middleware really ends the request-response by calling res.end, res.send, res.render or any method that implicitely calls res.end
 4- At what point in the request lifecycle can you “inject” middleware?
 befor the main handler function and after the rout
 
 Terms:
 Middleware: Any functionality that sits in between request/response, but does not send out response itself.
 Request Object: Represents the information in the HTTP request from the client to the server. 
 Response Object:  Information in the HTTP response from the server to the client.
Application Middleware: Middleware that plays a role in the function of the application.
Routing Middleware: Middleware that plays a role in path routing.
TDD: Style of programming in which three activities are tightly interwoven - coding, testing (unit tests), and design.
Behavioral Testing: Testing of the external behavior of the program (also known as black-box testing), usually a functional testing