# [6 Reasons for Pair Programming](https://www.codefellows.org/blog/6-reasons-for-pair-programming/)

## How does pair programming work and why even do it?

Usually there are two different roles in pair programming. One person is the **driver** and the other is the **navigator**. The navigator does not actually write any of the code, but makes the decisions in determining what code needs to be written to achieve the bigger picture. Navigators are also looking out for any potential issues like typos and bugs. The driver actually writes the code given by the navigator, and maneuvers through different files-carrying out the typical tasks necessary to actually get the code down.

Through paired programming, individuals take turns in each role and get to work on important skills necessary in learning a programming language.

- Listening
- Talking about code
- Reading
- Writing

### 6 good reasons to practice pair programming

**Greater efficiency**

When two individuals work together discussing code and solutions out loud it can result in higher quality code. Two eyes and two minds are better than one sometimes.

**Engaged collaboration**

Individuals learn to work together with problem solving and helping to keep one another focused on the task at hand.

**Learning from each other**

People have different understandings and methods of writing code. Sharing insight with another can help improves learning for both parties.

**Social skills**

Learning how to work well with another person with a different coding style and way of communicating is a good way to learn the social skills many employers want in an employee. They want to hire on people who work well with others through any differences.

**Interview readiness**

Some interviews have applicants pair program with an employee to see how well they will work on a team and can share their technical skills.

**Work environment readiness**

Having skills in paired programming will get you ready for work environments that utilize this practice of programming.

# JavaScript&JQuery by Duckett

## 293-301

### What is JQuery?
It is a JS filed included on web pages that uses css-style selectors to *find* elements and **JQuery Methods** to do something with the element.

There are multiple methods that can be used with a JQuery **object** that assigns tasks to elements.

### To use JQuery

1. Add JQuery **script** to html page *before* the closing `body` tag.
2. Include JS file that indludes JQuery *selectors and methods* to update content in HTML.

### Why use it?

JQuery makes coding more simple, sometimes even requiring less code.

1. Simple selectors
2. Using less code for common tasks
3. Cross-browser compatibility using **feature** detection to find best way for a task

## 306-331

### Selecting 1 or more elements will return a JQuery Object

Single element - `$('ul')`

Multiple elements - `$('li')`

### Using JQuery methods to `get` and `set` data

Get - `$('').html();` *(will get info for first element only)*

Set - `$('').html('what you update the element with')`

**When a selection is created, it stores *reference* to corresponding nodes in DOM tree not ~~copies~~**
(so the *location* of where information is stored in the browser memory is stored)

### Storing reference to an object through caching

1. Find matching nodes in DOM tree
2. Create object
3. Store reference to nodes in object using a variable

### Looping & Chaining

Looping(implicit iteration) - using a `class` attribute to all elements **getting** the element. *unless* the selector returns multiple elements

Chaining - Several methods in the *same* selector

**.ready()** = method that checks page is ready to work with code.

**OR**

use `.each()` method pp.324-325

### Getting the content of an element

`.html()` - the HTML *inside* of *first* element **and** *descendants* of that element

`.text()` - returns content from *selection* **and** text from *descendants*


### Updating elements

`.html()` and `.text()` - used as *setters* to update content of each element

`replaceWith()` and `.remove()` - *replace* **and** *remove* matching elements, their content **and** *child elements*

`.html()`/`.text()`/.`replaceWith()` - can take **strings**. Strings can be stored in a variable and can **contain markup**

### Inserting elements and adding new content

- `.before()`
- `.after()`
- `.prepend()`
- `.append()`

### Getting&Setting attribute values

- `.attr()`
- `.removeAttr()`
- `.addClass()`
- `.removeClass()`

### Getting&Setting CSS properties

`var yo = $('p').css('color');`
to **get** and **store** the **color** in variable

`%('p').css('color', '#292929');
to **set** the color

### Event Object

**Event handling function** gets an **event** object that has *methods* and *properties* related to the event.

1. The **event object** is named in the () of a function.
2. That **name** used in the function() is used *inside* of function to get the **event object**.

#### additional parameters for event handlers

`.on()`

- filter jquery selection to respond to subset of elements
- pass additional info to the event handler using **obj literal notation**

## 354-357

### How to include JQuery in your page

- Load from a CDN (*content delivery network)
- Locates server *nearby* and sends files from it
- Have a **fallback version** in case you to load from CDN

**Loading JQuery from CDN example: page 355**

**place** scripts at end of page **before** closing `</body>` tag. If placed in the `<head>`, it can slow down how quickly the page loads.

**HTML** should be loaded in DOM tree *before* script can access HTML within page.
