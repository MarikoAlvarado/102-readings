# Authentication

**1. Explain what a “Singleton” is (in Computer Science terms)**

Singleton is a design pattern that restricts multiple instantiations of a class to a singe object. So it's a more specific way of modularizing code within it's block..? [source](https://www.geeksforgeeks.org/singleton-design-pattern/)

**2.Explain how the Singleton pattern can be used with Node modules, specifically with classes**

When instantiating a class, using CONST will keep the methods within from changing and will keep new properties from being added. Node modules can help keep similar chunks of code organized and for us so we know where to find it and are able to export it to work with other areas of our code.

**3.If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?**

I would design the middleware in a way that it would look for certain properties of a request and make additions/changes before it moves on through other functions so they can better carry out tasks? I'm not entirely sure.

## Terms

**Router Middleware** - Takes a request, performs tasks using the information and passes it along.

**Dynamic Module Loading** - Loading modules only when necessary by using it with an async function. [source](https://gist.github.com/Rich-Harris/ea561810900eedd2a8e9afbc78ddd566)

**Singleton Pattern** - A design pattern restricts multiple instantiations of a class to a single object.

**CRUD -> REST Method Matches** - GET = READ, PUT=UPDATE/REPLACE, PATCH = UPDATE/MODIFY A PART OF INFORMATION, DELETE = DELETE, POST = CREATE.

**Mock Testing** - Using objects to mock the behavior of dependencies in order to test code. [source](https://devopedia.org/mock-testing#:~:text=Mock%20testing%20is%20an%20approach,behaviour%20of%20the%20real%20ones.)

1. Which 3 things had you heard about previously and now have better clarity on?

- mongoDB

- Linked Lists

- Writing tests

2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

- Linked Lists

- Big O

- Classes

3. What are you most excited about trying to implement or see how it works?

Implementing linked lists in our labs/project

## [Securing Passwords](https://thehackernews.com/2014/04/securing-passwords-with-bcrypt-hashing.html)

Cryptographics - Hash algorithms used to take in large amounts of data as wuickly as possible.

Hashing - Keeps hackers from having access to stored passwords in plain text.

GP Has Functions - used to check for data integrity

BCrypt - Slower, uses *key stretching*. Different amounts of data passed to function will result in different amounts of time it will take to generate hash values.

## [Basic Access Authentication](https://en.wikipedia.org/wiki/Basic_access_authentication)

HTTP Basic Authentication - Most simple technique to enforce access controls for web resources.
  - does not require:
    - cookies
    - session identifiers
    - login page

Security - Coded using **Base64**, not encryption or hashing. Used with HTTPS.

Server side - HTTP 401 Unauthorized status + WWW-Authenticate Field /w charset param. Ex `charset="UTF-8"`

Client side - sending authentication credentials from User -> Server:
  - username:pass
  - result = string encoded into *octet sequence*. US-ASCII/UTF-8 if charset param is included
  - result = string encoded as Base64
  - Authorization *method* + *`<space>`* is *prepended* to encoded string.

URL Encoding - Prepending `username:pass` to hostname in url. For basic authorization. **no go** and unsupported by modern browsers, keeping password from being sent and seen as plain text.

**BOOKMARKED**

[OWASP AUTH CHEATSHEET](https://www.owasp.org/index.php/Authentication_Cheat_Sheet)

[BCRYPT DOCS](https://www.npmjs.com/package/bcrypt)

