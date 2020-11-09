# [What is Node and When Should I Use It?](https://www.sitepoint.com/an-introduction-to-node-js/)

**What is it?**

- Built on Google Chrome's V8, open-source JS Engine

- Compiles JS direct to machine code made executable for the computer

- *JS runtime*

Simply put: **Event-based,non-blocking,asynchronous I/O runtime using google v8 JS engine + libuv library**

**Installation**

Installation of multiple versions to switch back and forth

[how to install multiple version using nvm](https://www.sitepoint.com/quick-tip-multiple-versions-node-nvm/)

- check for installation with ``node -v`` 

- should result in a version number

- check for proof of life

**Node.js support for modern JS**

Since only one time is target for V8 engine you can write JS with the most current syntax and shouldn't have to worry about compatibility issues.

**npm-the JS package manager**

To check:

- ``npm -v``

To install:

- ``npm install -g jshint`` to instal jshint package globally on **system**

Run linting on file:

- example ``jshint esversion: 6 */``

- fix ES6 errors by adding ``/* jshint esversion: 6 */``

- [linting refresher](https://www.sitepoint.com/comparison-javascript-linting-tools/)

**installing packages **locally** to project instead of globally**

- ``npm init -y`` to autopopulate a **package.json** file in the designated folder

- ``npm install lodash --save`` to save as a **project dependency**

- create a test.js fild and add 

    ``
      const _ = require('lodash');

      const arr = [0, 1, false, 2, '', 3];
      console.log(_.compact(arr));

    ``
- run script in terminal with ``node test.js``

- should see appropriate output of [1, 2, 3 ]

**working with package.json file**

- inside of ``test`` directory should be a folder called ``node_modules`` where npm saves **lodash** and the libraries which it depends on.

- ``node_modules`` ~~shouldn't~~ be checked in to version control

- re-create node_modules anytime by running ``npm install`` from project **root**

**What is Node.js used for?**

- Node.js is most often used for installing (npm) and running (node) tools for modern JS app.

- Let's us run JS on server

**how?**

- Node.js = single-threaded

- Event-driven

- Node = asynchronous (non-blocking) if event request is blocked by I/O operation and will register *callback* before next event processing.

[refer to site for visual of Node.js event loop](https://www.sitepoint.com/an-introduction-to-node-js/)

[video about event loop](https://www.youtube.com/watch?v=8aGhZQkoFbQ)

ex:
- test it by creating a **servertest.js** 

    ``
      const http = require('http');

      http.createServer((request, response) => {
      response.writeHead(200);
      response.end('Hello, World!');
      }).listen(3000);

      console.log('Server running on http://localhost:3000');

      ``

- then run it with ``node servertest.js``

- got to ``http://localhost:3000`` to check for proof of life

**Most suitable uses for node.js**

- real time apps for interaction/collaboration

- building APIs

- data streaming

**Its advantages**

- Speed

- Scalability

- Ability to do everything with one language

- understands JSON

- As a scripting language, automating frequent/error prone tasks

- create a command line tool
