[[HTTP/1.0 GET request]]
[[Port Numbers]]
[[Part I- implementing a sequential web proxy]]
[[Error Handling]]

Proxy - intermediary between clients making requests and a server to satisfy requests. can act as a firewall.
First part is checkpoint. 
Proxy to accept incoming connections, reads, and parse requets, forwards requests to web servers, reads the servers' responses, and forwards the responses to the corresponding clients. 

Need basic HTTP operations, sockets to communicate over a net work.

Debug using PxyDrive, a testing framework.


