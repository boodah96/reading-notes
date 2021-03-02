


- Form attributes:

action = "url : the data will be sent to the specified url / if none to the same page.
method = "GET" : the data will be sent as a request in the header. (url/?key=value&key2=value2).
method = "POST" : the data will be sent as a request in the body. (more secure, better for lonfer data, and sending files).


- The web browser sends a request using the HTTP protocol to the server, then the server gets the request.

- The GET method is the method used by the browser to ask the server to send back a given resource, In this case, the browser sends an empty body. Because the body is empty if a form is sent using this method the data sent to the server is appended to the URL.

- The POST method is a little different. It's the method the browser uses to talk to the server when asking for a response that takes into account the data provided in the body of the HTTP request. If a form is sent using this method, the data is appended to the body of the HTTP request.


