# Data Modeling

**1. Name 3 advantages to Test Driven Development**

Practicing how to write modularized code, having code that is easier to maintain because it has been broken down and collaborating with others is more efficient.

**2. In what case would you need to use `beforeEach()` or `afterEach()` in a test suite?**

When your test needs to handle asynchronous code  and test against conditions before and after functions. [src](https://jestjs.io/docs/en/setup-teardown)

**3. What is one downside of Test Driven Development**

It's harder to write tests when code is broken down into smaller chunks.

**4. What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?**

Classes can be instantiated at runtime and a constructor/prototype is the object instance.[src](https://www.toptal.com/javascript/es6-class-chaos-keeps-js-developer-up#:~:text=Prototypes%20vs.,is%20itself%20an%20object%20instance.&text=A%20class%20constructor%20creates%20an%20instance%20of%20the%20class.)

**5. Why REST?**

REST is less rigid and faster than SOAP which is more old-school and only works with XML.

### Terms

**functional programming** - Programming style to that avoids "side affects" when running functions?

**object-oriented programming (OOP)** - Programming where objects represent things that would be held in a database, the preference for modeling real world scenarios.[src](https://medium.com/@shaistha24/functional-programming-vs-object-oriented-programming-oop-which-is-better-82172e53a526)

**class** - Syntactic sugar for creating objects

**super** - Keyword that can access/call function on parent of object.[src](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/super)

**this** - refers to the object it is related to

**Test Driven Development (TDD)** - Style of programming focused on modularizing code,testing and design/structuring.

**Jest** - a framework used for tests

**Continuous Integration (CI)** - Style of programming that helps avoid issues when collaborating on a project.

**REST** - representational state transfer

**Data Model** - Represent how data is organized and related.

[SQL vs NoSQL](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool)

**SQL**

- Relational db
- uses tables/columns and rows
- Schemas are hardcoded/predefined
- Ex: MySql, Oracle, Postgres

**NoSQL**

- Non relational
- holds key value pairs
- dynamic schemas
- better for hierarchal data storage
- Ex: MongoDB, CouchDB, Redis

[NoSQL Data Modeling Techniques](https://highlyscalable.wordpress.com/2012/03/01/nosql-data-modeling-techniques/)

1. Denormalization - copying the same data into multiple docs/tables to make the query processing more simple or store data in specific model.
2. Aggregates - uses key-values + graphs to store data. No rules for what values can be. Supports "soft schemas"


