### [HOME](README.md)

# Duckett JS: JavaScript book, Ch. 10, “Error Handling & Debugging”

Make sure you understand the order of how scripts are processed and how statement are executed to be able to better 
pinpoint problems. remember that JS processes code *line by line*

**Execution Contexts**:

statements in a script exist in either,
- global context ( code in the script yet not a function-only ONE)
- function context (code within function)
- eval context

These contexts have a scope, either a *global scope*(a variable outside of a function or a variable not lead with "var") or *function-level*(variable only working within function). As script enters a new context two things happen.

**prepare**- new scope, variables, functions and arguments are created
**execute** - script can now assign values to variable, call functions to run, and execute statements

To understand **scope** know that each *execution context* posesses it's own variables objection holding functions parameters and variables withing it and parent variables object is accessible as well.

To understand **errors** know that JS will deploy an **exception** which the interpreter stops to look for a handling code for.

### Dealing With Errors
 
When dealing with an error you can find it written in the script.
Handle the error gracefully using statements:
- **try** 
- **catch**
- **throw**
- **finally**

**Dubugging Workflow**

- what does the error message tell you?
- What part of the script is the problem?
- What line number in the code can it be found in
- what kind of error is it?

1. insert "dubugg" in script to run up to a certain point to try and narrow it down
2. use breakpoint

**what is the problem**

1. check the variables, try commenting out parts of code to test specific areas.
2. check the parameter for a function or number of items in array

**CHROME DEV TOOLS**

1. open dev tools/console
2. look at errors and line info (a specified line does not always mean that is where the problem *is*, it can be where the browser first noticed the error.)
3. use **try,catch,finally** blocks with specific code in question inside **example pp.480**

### [HOME](README.md)