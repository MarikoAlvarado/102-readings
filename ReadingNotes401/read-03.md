# Express REST API

**1. Name 3 real world use cases where you’d want to change the request with custom middleware.**

Adding the time or date that a request was made. Validating information before it reaches the server for example, checking to see if a username exists or if a phone number consists of numbers vs letters.

**2. True or false: The route handler is middleware**

False, the route handler can force a request to run through middleware before proceeding though.

**3. In what ways can a middleware function end the process and send data to the browser?**

by using `next()` either empty or containing an error.

**4. At what point in the request lifecycle can you “inject” middleware?**
 
 Immediately after the request is made and ideally, before a route handler is called.

 **5. What can cause express to error with “Request headers sent twice, cannot start a second response”**

 A request is made twice? I'm not sure.

 **DEFINITIONS**

**Middleware** - software that can intercept data and make add information, validate and perform other check before allowing it to continue.

**Request Object** - HTTP request from the client that contains properties for req query,params,body and headers[src](https://www.tutorialspoint.com/nodejs/nodejs_request_object.htm) 

**Response Object** - HTTP response from server with results from req.


**Application Middleware** - I'm not sure what the correct definition for this would be vs Middleware.


**Routing Middleware** - Middleware used to interact with data to and from routes?

**Test Driven Development** - Programming style involving three main factors, coding,testing and design. [src](https://www.agilealliance.org/glossary/tdd/)

**Behavioral Testing** - software testing method for internal structure, design and how the item being tested for is applied.[src](https://softwaretestingfundamentals.com/black-box-testing/#:~:text=BLACK%20BOX%20TESTING%2C%20also%20known,%2Dfunctional%2C%20though%20usually%20functional.)

### Prep Readings

- [ES6 Classes](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes)
- [Using Express Routing](https://expressjs.com/en/guide/routing.html)
- [Express Routing](https://scotch.io/tutorials/learn-to-use-the-new-router-in-expressjs-4)