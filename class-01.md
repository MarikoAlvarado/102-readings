# Introduction to HTML and Javascript Reading Notes

## Duckett: HTML&CSS CH1

### Structure

How a well a webpage is structured will determine the success in catching and keeping the attention of the audience. When creating a structure, it is important to do so with the goal of clearly stating and portraying the message to be delivered, and making the different pages easily accessible and relevent to the overal goal. 

The structure of a webpage first, consists of organizing bodies of texts, photos and other information into headings, subheading, paragraphs and a footing.

HTML code within angled brackets **<>** which makes them *elements*. Elements are made up by **tags** showing as opening and closing. For example **<> </>**. When a bunch of HTML elements are put together, the structure of a webpage and the contents within each section will begin to show form by *priority*

This is the start of creating a webpage's wireframe.

## Duckett: HTML&CSS CH8

### DOCTYPES

Relays to browser which version of HTML is being used to creat a page.

### <!--COMMENT--!>

Adds comments to code.

### **id** and **class**

Allows the creator to identify particular elements, this helps with edit through CSS.

### <div><span>

Lets creators group 'block-level' and 'inline' elements together.

### <iframes>

Awesome, this element makes a *window* on a page where another page can be shown.

### <meta>

Using this, creators can include information about the webbpage

### Different Versions of HTML 

#### HTML 4 - 1997

No longer recommended to be used by modern day creators. it's pretty out of date.

#### XHTML 1.0 - 2000

XHTML was created to follow the rules of XML from 1998 which made stricter rules for writing markup. Some other versions of XHTML 1.0 are,
- Strict XHTML 1.0
- Transitional XHTML 1.0
- XHTML 1.0 Frameset

#### HTML5 - In progress

In this version, creators will **not** need to close all tags. New elements and attributes are in the mix as well. Although it is not yet complete, creators can use some of the features as long as we are mindful of how users with older browsers, may or may not be able to view webpages.


## Duckett: HTML&CSS CH17

### HTML5

HTML5 is introducing new elements that result in clearer code and the ability to better show and describe a the overall structure of a webbpage.

Older browsers won't recognize these newer element and must be told which elements are "block-level".

Extra JS needs to be installed in Internet Explorers 8 and older in order for the new HTML5 elements to work.

## Duckett:HTML&CSS CH18

### Designing My Website

#### Who is my target audience?

- Is it a company, or an individual? Age? Gender? Where do they live? What level of Education do they have? What kind of device are they using to view the site? etc.
- What are visitors looking for? What is the goal?
- Do I need to include information so they can contact me?
- What information do they need? Am I telling them about a project, service or sharing general information?
- *how often do I need to update my website?*
- Do I need to include a nav bar? How should I organize the site into sections or pages while maintaing focus on the goals?

##### Creating a wireframe for my website

##### Where to start?

- Make a sketch of how the site should appear
- Where are my headings? Subheadings?
- Where will I place the bodies of text?
- Will there be photos?

##### When making the rough draft/basic layout

- header
- footer
- main 
- mian+body= the content which shows 

##### Consider the visual design to help get the message across

- Logos?
- Nav bar?
- Links to related content?
- Subscription/Comment boxes?
- Links to related content?

##### Navigation needs to be...

- Concise
- Clear
- Selective *make sure it aligns with contents/information to be found on each page*
- Context
- Interactive
- *CONSISTENCY*

##### Be sure to prioritize content of website

- Make sure the main messages can stand out. Some parts of the webbpage should look distinct in comparison to other parts of the page. Creat a *visual hierarchy* to help draw and keep the attention of visitors.

##### Visual hierarchy

- Size
- Color
- Style
- Visual contrast

##### How should it all be organized?

- *Group* together pieces of content which relate by making *blocks* or *chunks*. It should be easy for visitors to identify each group and the information within it. Be mindful of appearance and maintain a visual style.

##### Grouping and consistent visual style

- Proximity
- Closure
- Continuance
- White space
- Color
- Borders
- Headings
- *CONSISTENCY*



# JAVASCRIPT Reading Notes

## Duckett: JS&JQUERY Intro + CH1: The ABC's of Programming

## Pages 1-24

### How does Javascript make your webpage more interactive?

- It can be used to access from an HTML page by referencing elements

- JS can be used to add or remove elements and attributes from an HTML page

- Rules can be made giving a browser step by step instructions for how contents of page will work

- JS can be told to reacts a certain way when there are certain actions taken by users like clicking a button or moving the cursor over an HTML element 

### Writing Javascript

1. Start by writing out your goal like *tell a robot how to put on a hoodie*

2. Break down that goal by a series of tasks like *pick up hoodie, lift over head...*

3. Create a code for each step in Javascript

### Taking it from steps to code

- understand JS language

- **Vocabulary** - what can the computer understand?

- **Syntax** - How can the words be put together as instructions that the computer can understand?

- **Programmatic Approach** - Computers problem solve by following a directions, in order or as instructed.

**LEARN TO THINK LIKE A COMPUTER!!**

*REMEMBER*

- Sketch out tasks in a flow-chart

- design the goal and design the script!

## Pages 25-42: How Computers Fit in the World Around Them

Programmers create models using **data** to instruct a computer in carrying out tasks.

- **OBJECTS** - Each object has it's own *properties, events and methods*

- **Properties** are the characteristics of each object, and each property has it's own *name* and *value*

- **Events** - When a program is created. Specific **events* result in specific *script* to run.

- **Methods** - A combination of instructions to represent a single task. Just know the right questions to ask to understand which answer is given in return.

*So*, events trigger methods, methods call/update the properties of an object.

**objects are combined and build programs which can create web browsers**

**document object** access and change the visible page and the possibilites of interactions with users *on* that page.

## Pages 43-52: Writing Script for a Web Page 

JavaScript is just one of the multiple layers which build a webpage, the other layers in most cases is HTML and CSS and together they are **progressive enhancement** in page building.

#### Creating Javascript

Javascript is written in plain text like HTML and CSS.

- It is a *.js* file

-JS files can live in folders **js., scripts or javascript**

- In HTML, JS is used within the **<script></script>** element

#### Objects and Methods

**document** = represents the entire webpage
**write('*message here*')** = the content can be written on the page where *script* element is

- together it shows as *document. write('message here);*

JS code is embedded directly into the HTML code.
