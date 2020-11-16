# [EJS](https://www.youtube.com/playlist?list=PL7sCSgsRZ-slYARh3YJIqPGZqtGVqZRGt)

**Getting Started With EJS**

1. `npm init -y`
2. `npm i express` `body-parser` `cors` `ejs`
3. set up path/built in core module for node
4. Set up express, body parser, cors
5. set up instance of express
6. Set up app.use for bodyParser and cors
7. Path doesn't need to be installed. 
8. Line 11 @ 3:29 takes two paths and joins them

**Evaluate and Injected Variable**

How to inject a value into EJS view and how to evaluate the variable.

- `response.render` takes three variables, uses:
  - view
  - object of local variables

- `<%=  %>`  will evaluate a variable for you similar to handlebar brackets.
  
  **Iterate over an array value in ejs**

- create a for() loop inside .ejs and don't forget that the value needs to be evaluated using ejs tag as well!

**using if/else in ejs**

- also need ejs tag!!
- use this to determine what value will be evaluated and show on page.

**Layouts**

- not native to ejs
- useful to wrap information in file as you switch views between URLs
- add them by ``npm i --save express ejs-layouts``
- add in js example @1:50
- make sure there is an `app.use` for expresslayouts
- Use this to wrap content in a way which designate what will show on each webpage.

**Partials**

- *are* native to ejs
- useful for:
   - nav bar
   - footer
   - reusable/static piece of text
- Example * 50sec

### Helpful Resources

#### [Working With Volumes](https://developers.google.com/books/docs/v1/using#WorkingVolumes)


#### [EJS Tutorial](https://www.digitalocean.com/community/tutorials/how-to-use-ejs-to-template-your-node-application)


##### [source code for tutorial](https://github.com/scotch-io/node-ejs)










