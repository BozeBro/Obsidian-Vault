[[HTTP/1.0 GET request]]
[[Port Numbers]]

Handle HTTP/1.0 GET requests. Don't need to handle POST requests. 

1. Listen to incoming connections on a part specified by cmd line. 
2. Read entirety of request from the client and parse the request.
	1. Determine if request is valid.
3. If valid, establish connection to web server
4. request specified object
5. Readd server's response and forwards to client.

