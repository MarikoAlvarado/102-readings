### [HOME](README.md)

# From the Duckett HTML: Chapter 7: “Forms” (pp.144-175)

Forms are a way of sending data input from users to the server. Various elements HTML are used to collect information through form.

When user submits form information, the names of *form controls* is sent to the **server** with the values (name attributes). Programming language is used to process that information in the server and can also store information in database. Depending on the information recieved and process, the server will create and send back a page dependent on the input.

**form controls** = **name**=**value**

### Form Controls

- **text** text input, number input, password input, text area (larger portions of text input)
- **making choices** radio buttons, checkboxes, drop-down boxes
- **submitting** submit button, image button, file uplad

**< form >** requires an *action* and *method*
**< input >** requires *type=text* , *name* and *maxlength*
refer to pp.153- 168

# From Duckett HTML Chapter 14: “Lists, Tables & Forms” (pp.330-357)

**list-style-type**/**list-style** gives different types of appearances for list marker.

*style-type* - bullet point style (disc,circle square)
*style- image* - little tiny images (think chocolate pizza assignment type SMALL)
*style-position* - inside/outside
*list-style* = shorthand

### properties of a table!!!

- width

- padding

- text-transform

- letter-spacing, font-size

- border-top, border - bottom

- text-align

- background- color (contrast is VERY useful especially with table data)

- :hover (highlight table row when "hovered" over!)

**NOTE: *very* cool infor on table styling pp 339-348**

- table cells can be made to be consistent style across browser. This matters because the borders and spacing can change.

 -vertically align *form* controls with **CSS**, styles can make forms more interactive.



# From the Duckett JS : Chapter 6: “Events” (pp.243-292)

Whenever a user interacts with a webpage in a specific way, the browswer registers what **event** has occured and sets off whichever code is created to react. While DOM (think creating a data table) updated a page in response to an event, a form can trigger an event as well.

Some examples of **events**:

- UI- loading,scrolling, resizing, errors, unloading
- KEYS- keydown,keyup,keypress
- MOUSE- click, double click, mousedown, mouseup

**events** triggering JS

- specifying the element the script should respond to -**element**

- specify the event to trigger a response -**event**

- specify the code which will run in accordance to event **call code**

DOM Handlers and DOM level 2 events *bind* events to an element. Event handlers and listeners cannot have () after the function name.

The **event object** delivers information about an event and its element.

**REMEMBER** to change default behavior(tossing information from event)

- preventDefault() - keep information
- stopPropogation() - keep event from affecting prior elements
- can use both of these.
**Event Delegation** example pp.268

Event Object can tell you if event occured on screen,page of screen or client with specific properties such as *x/y* to pin position of where mouse was

**Mutation Events and Observers** - when elements are added or removed from DOM the structure *mutates*

### [HOME](README.md)