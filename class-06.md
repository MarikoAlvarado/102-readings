# Understanding The Problem Domain Is The Hardest Part of Programming

### Some of the hardest things about writing code other than Domain?

- You're having to learn a new technology

- Learning how to name things

- Testing Code

- Debugging

- Knowing how to go about fixing issues/bugs

- Developing software that can be maintained


### Problem Domains are Difficult to understand

Not often do programs recieve all of the information about a problem domain to be able to understand it. Learn *how* to understand The Problem Domain. When you understand the problem domain you will understand what code needs to written for it. 

**How can one understand the problem domain handed to them?**

- **make it easier-simplify it!**

- **improve your understanding of it, as thoroughly as possible!**

# Duckett JS book Chapter 3: “Object Literals” (pp.100-105)


### What's an object?

Objects group up variable and function in order to create models which represent a real world project.

**objects change what variables and functins get *new names***

- *variables* become properties, *properties* describe what the *object* is

- *functions* become methods, *methods* represent tasks that have to do with the *object*

**use hotel example on page 101**

hotel = the object
properties of hotel = name, rooms, booked, gym.
values of properties = strings, numbers, booleans and arrays

method= function of "checkAvailability"

var naming **object**>{**key** with **properties**>**method** with function}

### Creating Object using Literal Notation

the **object** is what is within the curly braces. The object is stored inside of a variable which can use a *literal* name like "hotel". so you could view this literally as **hotel object**

eache**key** within an object is separated from it's value using **:**

### Accesing object and dot notation/creating more object liters

use *dot notation* to access properties or methods of an object. can also use *square brackets* to access properties.
**really good examples page 104-105

# Duckett JS book Chapter 5: “Document Object Model” (pp.183-242)

**DOM AKA Document Object Model** Some folx call this the API

DOM isn't a part of JS *or* HTML

It is used for:

- making a model of HTML page. *how browser should structure the model using DOM tree

- Accessing and changing the HTML page. DOM defines methods and properties  the access necessary to update what users see in browser

- **The DOM tree models the webpage**, it then get's stored in the browsers memory

Has four types of nodes, each notde is an object with methods and properties.

- **document nodes** represents entire page and corresponds with document object

- **element nodes** find the html elements/nodes to *access* DOM tree

- **attribute nodes** represent HTML Attribute

- **text nodes** after accessing element node, text node can be accessed. text nodes cannot have children

**Really good visual on page 187**

### Working with DOM Tree

1. Acces elements within

2. work with the elements using text content, child elements and attribute


**DOM Qeuries** - method to find *elements in a DOM tree. DOM queries will either return single element, *or* a **Node List** with a collection of nodes

To return single element node:

**getElementByID**

**querySelector**

To return one or more elements as a node list

**getElementsByClassName**

**getElementsBytag Name** 

**querySelectorAll**

**page 197**

use **textContent, innerHTML** or DOM manipulation techniques to update and access content from element node

*multiple text nodes and child elements that are related can be contained **within an element node**

DOM might be *inconsistent* in older browsers

**browsers have tools for viewing DOM tree**
