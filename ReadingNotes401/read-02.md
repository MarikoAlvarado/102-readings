# Express

**1.What is the difference between`PUT` and `PATCH`?**

A `PUT` request replaces data or creates new data where specified. `PATCH` will only partially update data without affecting anything else. [source](https://rapidapi.com/blog/put-vs-patch/)

**2. Links to 3 services/tools that allow you to "mock" and API for development like `json-server`**

[Mockserver](https://www.mock-server.com/)

[Postman](https://learning.postman.com/docs/designing-and-developing-your-api/mocking-data/setting-up-mock/)

[Beeceptor](https://beeceptor.com/)

[*source*](https://nordicapis.com/10-tools-to-mock-http-requests/)

**3. Swagger vs APIDoc.js Status codes**

- **Swagger** [source](https://swagger.io/docs/specification/describing-responses/)

  - `200` = successful
  - `400` = bad request
  - `401` = missing or invalid authorization information
  - `404` = User ID not found
  - `5XX` = Unexpected error

- **Apidocsjs** [source](https://apidocjs.com/)

  - Object response ex:

    ```
    {
      "error": " " ,
      "route": " ",
      "message": 
    }
    ```

**4. SOAP vs REST**

REST was created to make up for what SOAP (more old school and relies on XML) lacks. SOAP messaging patterns are more strict while REST is more flexible and does not require processing. Both are used to access web services. [source](https://smartbear.com/blog/test-and-monitor/soap-vs-rest-whats-the-difference/)

**5. TERMS**

***Web Server***

  - hardware and/or software using HTTP requests/responses from client providing functionality.[source](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/What_is_a_web_server)

***Express***

  - A library/framework node module for creating servers

***Routing***

  - Endpoints that calls functions in response to a request from client

***WRRC***

  - Web Request Response Cycle. The process of (http) requests made to server from client where tasks are carried out to provide a response back to client.

  ## [Express/Node Introduction](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Express_Nodejs/Introduction)

  **Node**

   - environment that allows the use of server-side tools and apps using JS. Node modules can be managed in a package for libraries of tools that can be used to create an application.

   **Express**

   - popular node framework that allows handlers to be written for HTTP request from different routes, setting up a port for the server, rendering responses and processes middleware withing handling of requests.

  ## [NPM](https://docs.npmjs.com/about-npm)

  Software registry where developers around the world can share and borrow packages.
  
   NPM has 3 components:

  - the web
    
    - find packages, set up profiles

  - CLI (command line interface)

    - how devs interact with npm and install packages

  - the registry

    - huge, public db of JS software and meta-info that surrounds it.

## [TDD](https://www.agilealliance.org/glossary/tdd/#q=~(infinite~false~filters~(postType~(~'page~'post~'aa_book~'aa_event_session~'aa_experience_report~'aa_glossary~'aa_research_paper~'aa_video)~tags~(~'tdd))~searchTerm~'~sort~false~sortDirection~'asc~page~1))

TDD = Test-Driven Development

Coding + Testing + Design. Uses **1** unit test to describe aspect of program. If program lack feature the test will fail so write enough code that it passes and refactor the code to become more simple.

## [Continuous Integration and Continuous Delivery/Deployment](https://www.youtube.com/watch?v=xSv_m3KhUO8)

CI - workflow strategy that helps integrates multiple changes to a project. Helps catch bugs and reduce merge conflicts.

CD - Delivery is a strategy where you can deploy anytime. Deployment extends off of delivery where you can deploy the new features quickly.




