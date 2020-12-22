# Socket.io

**1. What is the benefit of transforming data into packets?**

It's more efficient and reliable because there's a lesser chance of losing bits of data while it is transmitted.[source](https://smallbusiness.chron.com/technology-pros-packetswitching-network-62589.html)

**2. UDP is often referred to as a connectionless protocol. Why is this?**

It is a way of transmitting data whether or not the receiver is ready or exits.[source](https://www.techopedia.com/definition/18513/connectionless-protocol)

**3. Can a socket server application have multiple socket connections?**

Yes, as long as they are associated with different client IP/Ports.[source](https://stackoverflow.com/questions/11129212/tcp-can-two-different-sockets-share-a-port/11129641)

**4. Can a socket connection application be connected to multiple socket servers?**

yes. I'm not sure.

**5. Can an application be both a socket server and a socket connection?**

yes, if you use different ports for the server.


## Terms

**Observer Pattern** - a pattern where an object is referenced as `subject` which keeps a lists of dependents called `observers` that are updated if there is any change.[source](https://webdevstudios.com/2019/02/19/observable-pattern-in-javascript/#:~:text=The%20observer%20pattern%20is%20a,calling%20one%20of%20their%20methods.&text=When%20one%20object%20updates%2C%20it,that%20it%20has%20been%20updated.)

**Listener**- what waits for an event to occur.

**Event Handler** - Runs code after an event occurs.

**Event Driven Programming** - A series of events must occur, all correlating with one another in order to take their turn.

**Event Loop** - moves events from the queue to the call stack so each event will run in turn.

**Event Queue** - a series of events/functions waiting to be called.

**Call Stack** - and order or lineup of events/functions.

**Emit/Raise/Trigger** - What triggers an event once certain conditions are met.

**Subscribe** - similar to a promise/catch but responds to observer methods? not sure.

**database** - where data is organized and stored either relationally or un-relationally .

### resources/prep

[Web Sockets](https://en.wikipedia.org/wiki/WebSocket)

[Socket.io Tutorial](https://www.tutorialspoint.com/socket.io/)

[Socket.io vs Web Sockets](https://www.educba.com/websocket-vs-socket-io/)

#### bookmarked

[Socket.io Docs](https://socket.io/docs/)

[Socket.io Server API](https://socket.io/docs/server-api)

[Socket.io Client API](https://socket.io/docs/client-api)

[Socket Testing Tool](https://amritb.github.io/socketio-client-tool/)