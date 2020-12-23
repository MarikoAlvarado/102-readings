# Message Queues

**1.What does it mean that web sockets are bidirectional? Why is this useful?**

It means that they move data from a server to a client therefor it must be handled on both sides. This is useful because you can continuously transmit data on the same connection[souce](https://stackoverflow.com/questions/12366651/how-the-websocket-bi-directional-concept-work)

**2.Does socket.io use HTTP? Why?** 

Yes, because it uses an HTTP request, for example the local host address to create new endpoint/namespaces to transmit data between clients and server.

**3.What happens when a client emits an event?**

When a client emits an event, it travels to a specific endpoint in the server where there is a listener and events/data can be re-emitted.

**4.What happens when a server emits an event?**

When a server emits an event, it can either broadcast data globally or to a specific client.

**5.What happens if a client “misses” an event?**

If a client misses an event it will be ignored.[source](https://stackoverflow.com/questions/32816290/what-happens-with-unhandled-socket-io-events)

**6.How can we mitigate this?**

Have events run continuously until they are handled using a sort of interval?Not sure.

## Terms

**Socket** - an endpoint up on a server with a port number.

**Web Socket** - a socket on the client side.

**Socket.io** - a js library that allows data transmission between a server and client.

**Client** - the web browser where requests from a user are sent to the server

**Server** - a program that connects to, receives and sends information to the client

**OSI Model** - Open Systems Interconnection Model/framework that translates telecommunication.[source](https://en.wikipedia.org/wiki/OSI_model)

**TCP Model** - A more concise/specific version of the OSI model[source](https://www.geeksforgeeks.org/tcp-ip-model/)

**TCP** - Transmission Control Protocol

**UDP** - User Datagram Protocol, send packets of data over the network.

**Packets** - Holds small amounts of data sent through UDP.

### [Prep Materials]

[Socket.io Chat Example](https://socket.io/get-started/chat/)

[Rooms and Namespaces](https://socket.io/docs/rooms-and-namespaces/)

[Socket.io Emit Cheatsheet](https://socket.io/docs/emit-cheatsheet/)