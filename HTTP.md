INTRODUCTION.

=> In 1989, Tim Berners-Lee invented HTTP
=> HTTP stands for hypertext transfer protocol
=> It is the basis for almost all web applications.
=> HTTP is the method computers and servers use to request and send information
=>Years later, the IETF, Google, Microsoft, and Facebook released the fully-comprehensive 
    and well-tested newer version of HTTP in 2015.

WHAT IS HTTP 1.1

=> The first usable version of HTTP was created in 1997
=> HTTP/1 was known to have poor response time
=> This first version of HTTP was called HTTP/1.1. This version is still in use on the web.

WHAT IS HTTP 2

=> HTTP/2, based on SPDY protocol, was developed to address the inherent limitations of HTTP/1.1 and
     further progress the Internet.
=> In 2015, a new version of HTTP called HTTP/2 was created
=> HTTP/2 is much faster and more efficient than HTTP/1.1

HTTP/1.1 and HTTP/2 Main Differences

=> Launching of the HTTP/2 was an attempt to overcome the limitations of HTTP/1.1 and 
    make it a more efficient web protocol 
=>  So, the major differences in these two are mainly the additions or upgrades applied in HTTP/2

THE BACKGROUND
HTTP1.1
=> HTTP protocol was developed in 1989 as the common language that enables client and server machines’ interaction

=> The client (browser) has to send a request to the server using the method (GET/POST).
=> Server responds with the requested resource, for example – image, 
    alongside the status of what it did to the client’s request.

HTTP/2

=> HTTP/2 was released at Google as the significant improvement of its predecessor
=> It was initially modeled after the SPDY protocol and went through significant changes to include features like multiplexing,
     header compression, and stream prioritization to minimize page load latency
=>  After its release, Google announced that it would not provide support for SPDY in favor of HTTP/2.
=> The major feature that differentiates HTTP/2 from HTTP/1.1 is the binary framing layer.
=> Unlike HTTP/1.1, HTTP/2 uses a binary framing layer
=> This feature of HTTP/2 enables gRPC to use lesser resources.

![alt text](<6149cc3eca0fb2c370604259_http1 vs http2 responce time.png>)

DELIVERY MODEL 

=> HTTP/1.1 sends messages as plain text
=> HTTP/2 encodes them into binary data and arranges them carefully

HTTP/1.1

=> HTTP/1.1 addresses this problem by creating a persistent connection between server and client
    For example – If a request at the queue head cannot retrieve its required resources, it can block all requests behind it.
     This phenomenon is called head-of-line blocking (HOL blocking).

HTTP/2

=> HTTP/2 developers introduced a binary framing layer
=> This layer partitions requests and responses in tiny data packets and encodes them

RESPONE TIME 

HTTP1.1 & HTTP2


ADVANTAGE AND DISADVANTAGE OF HTTP2

ADVANTAGE 

=> HTTP/2 supports full multiplexing for requests as well as responses over a single TCP connection
=> Lower page load times are achieved by removing needless latency and improving the overall capacity of network alongside its availability.
=> All modern browsers support HTTP/2 over HTTPS with the SSL certificate installation
=> To open HTTPS capable invisible proxy ports on every relevant port, OWASP ZAP or its alternatives could be used.
=> The use of the HPACK algorithm enables HTTP/2 to overcome the common API security threats.

DIS-ADVANTAGE

=> While HTTP/2 mitigated the effects of HOL blocking in its predecessor, TCP-level block still causes problems.
=> For client machines operating on a slow network, data packets drop bit by bit, and the network quality gets degraded 
    to a single HTTP/2 connection. Due to this, the entire process slows down, thereby blocking a lot of data transfer.
=> The cookie security failure is still not addressed in HTTP/2 like its precursor
=> Cookies are .txt files containing client data obtained by the server and website 
=> However, these cookies may get stolen or tampered with by hackers, who can access personal user data, even without passwords.
‍
![alt text](<6149cc01573487fea0af8519_http1 vs http2 vs http3.png>)

