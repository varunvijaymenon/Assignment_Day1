### HTTP/1.1

1.   HTTP/1.1 allowed for persistent connections. 
2.   It allowed multiple requests/responses per TCP connection.
3.   Provided support for chunk transfers that allowed streaming of content dynamically as chunks and for additional headers to be sent after the message body.
4.   Pipelining was implemented for lower delay of response times.
5.   Content negotiation was implemented to serve different versions of a resource at the same URI.
6.   Cache control was used to specify caching policies in both requests and responses.

### HTTP/2

1.   It introduces the concept of a server push where the server anticipates the resources that will be required by the client and pushes them prior to the client making requests. The client retains the authority to deny the server push; however, in most cases, this feature adds a lot of efficiency to the process.
2.   Introduces the concept of multiplexing that interleaves the requests and responses without head-of-line blocking and does so over a single TCP connection.
3.   It is a binary protocol i.e. only binary commands in the form of 0s and 1s are transmitted over the wire. The binary framing layer divides the message into frames that are segregated based on their type – Data or Header. This feature greatly increases efficiency in terms of security, compression and multiplexing.
4.   HTTP/2 uses HPACK header compression algorithm that is resilient to attacks like CRIME and utilizes static Huffman encoding.
