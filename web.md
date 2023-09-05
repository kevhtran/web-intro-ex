# Conceptual Exercise

### Part One: Solidify Terminology
In your own terms, define the following terms:

- What is HTTP?
>HYPERTEXT TRANSFER PROTOCOL. This is how browsers and servers communicate. 
- What is a URL?
>UNIFORM RESOURCE LOCATOR. This is the address for some internet resource.
- What is DNS?
>DOMAIN NAME SYSTEM. Takes URLs and converts them into IP Addressess. 
- What is a query string?
>Provides extra information into the URL passed by key-value pairs. It follows ? and can contain:  
Arguments, which are seperated by &  

- What are two HTTP verbs and how are they different?
>These are HTTP methods.  
GET - get some data from the server.  
POST - send some data to the server.  
- What is an HTTP request?
> A request from the client to a server which follows the HTTP protocol. 
- What is an HTTP response?
> A response from the server to a client which follows the HTTP protocol.
- What is an HTTP header? Give a couple examples of request and response headers you have seen.
> Headers provide additional information about the request or the response. Here are some examples:  
Request headers: Host, User-Agent, Accept, Cookie, Cache-Control  
Response headers: Content-Type, Last-Modified, Set-Cookie, Cache-Control  
- What are the processes that happen when you type “http://somesite.com/some/page.html” into a browser?
>Your browser “resolves” the name into an IP address using DNS  
Your browser makes a request to that IP address, including headers (info about browser, any previous cookies, and other things)  
The server sends a response (typically, HTML, with a status code (200 if it was sucessful)
The browser makes a DOM from that HTML, and finds any other resources needed (images, CSS, JavaScript, etc)  
The browser makes separate HTTP requests for those resources and receives response from the server for each  

### Part One: Solidify Terminology
Using curl, make a GET request to the icanhazdadjoke.com API to find all jokes involving the word “pirate”
> curl -X GET https://icanhazdadjoke.com/search?term=pirates
Use dig to find what the IP address is for icanhazdadjoke.com
>dig icanhazdagjoke.com
>SERVER: 172.17.0.1#53(172.17.0.1) (UDP)