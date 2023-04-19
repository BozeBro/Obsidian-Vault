elements of [[1.0 GET request]] [[Port Numbers]]

headers - key-value pairs provided line-by-line following the first requeest of an HTTP request. each key,pair is separated by a colon. 
#### Important Headers
1. Host (Required)
2. User-Agent 
	1. Use `User-Agent: Mozilla/5.0 (X11; Linux x86_64; rv:3.10.0) Gecko/20230411 Firefox/63.01\r\n`
	2. Should be sent as a single line
	3. Identifies the client.
3. Connection
	4. use `close\r\n`
4. Proxy-Connection
	1. use `close\r\n`
Connection and Proxy-connection, what to do after req/res finishes.

Besides Host, ignore the above headers of client.


