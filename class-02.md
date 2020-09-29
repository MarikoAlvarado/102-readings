# Duckett HTML book: Chapter 2: “Text” (pp.40-610)

## Cheat Sheet for Markup Elements and Tags

**elements which describe headings and paragraphs**

| Element/Tag   | Result      |
|---------------|------------ |
|< h1 > - < h6 >| Headings    |
| < p >         | Paragraph   |
| < b >         | Bold        |
| < i >         | Italic      |
| < sup >       | Superscript |
| < sub >       | Subscript   |
| < br / >      | Line Break  |
| < hr / >      | Hrzntl Rule |

## Cheat Sheet for Semantic Markup

**gives extra info for emphasis, quotations, acronyms and such**

| Element/Tag   | Result                               |
|---------------|------------------------------------- |
| < strong >    | bold (important)                     |
| < em >        | emphasis (italic)                    |
| < blockquote >| indents whole text                   |
| < q >         | quotes around short text             |
| < abbr >      | abbreviation/acronym                 |
| < cite >      | italicized citation                  |
| < dfn >       | defining instance for new term       |
| < address >   | italicized contact info              |
| < ins >       | show content inserted in dcmnt       |
| < del >       | show deleted text from dcmnt         |
| < s >         | indicates what is no longer relevant |

# Duckett HTML book Chapter 10: Ch.10 “Introducing CSS” (pp.226-245)

## What's CSS?

CSS allows creators to control how a webpage will appear in accordance with the HTML wireframe. Contents within HTML become categorized within "boxes". CSS *properties* and *values* dictate the appearance or **style** of HTML elements. CSS can be used with HTML externally, yet connected by an insterted *>link<* withing the HTML code. **OR** CSS styles can be included directly *within* HTML code using the **<style>** element.
**It is most common for CSS rules to be made in a separate document rather than within HTML**

There are different types of CSS selectors which allow you to direct *specific* rules at *specific elements* in HTML. For example, a rule for just one of two images within the *same section* of a webpage.

**Declarations** are made up by both element properties and the *value* of properties to be changed.

## Color

- every color we see on the devices we use are made up by different mixes of red, blue and green or **RGB**

- Individual pixels in our screens can be a different color

## Values

- *RGB* values are values expressed by number for the amount of how much red, green and blue are used

- *Hex codes* express RGB values by hexadecimal code

- *Color names* express colors simply by naming them

- *Hue* , *saturation* and *brightness* are how much gray, black and shade are present of a color

# Duckett JS book: Chapter 2: “Basic JavaScript Instructions” (pp.53-84)

**Statements** are individual instructions which make up a script ending with **;**

- *green* is the statement

- *pink* indicate start & end of the codeblock

- *purple* determines which code should run

**Comments** describe for you and others what the code does

- *green* JS code

- *pink* multiple lines of *comments*

- *gray* single line of *comments*

## Variables

Variables are where a scripts data is stored. Data within variables can 'calculate' or 'compute' numbers or other types of data.

**declaring a variable** = *var quantity = 1;*

**numeric data** = *0.45*

**string type data** = *'what is up!'*

**BOOLEAN data** = *true* or *false*

- Variables can store strings which are placed inside of either single or double quotes

- *if using single quotes in the string, surround the entire string and the single quotes with double quotes OR the other way around* 

## Naming Variables

1. Must begin with a letter *$* or **_** - no numbers!

2. Name can contain the same as above but no **-** or **.**

3. No keywords or eserved words (words to be used in the future)

4. Variables are case sensitive! 

5. use a name that describes the information example: **myName**

6. If name is made of more than one word, separate with an uppercase letter after first word as shown above

## Arrays

Arrays store a *list* of values. 
Best used for:
- lists
- related values
**shopping list example** (pages 70-71)

for values:
- number items
- retrieve items by using variable with value set to a specified item in array
- *lengths* hold number of items in array

### Expressions

**expressions result in a single value**

1. Assign a value to a variable **var color = 'black';**

2. A variable might use more that one value to result in a single value **var area = 2 * 400;**

### Operators

*expressions **need** operators which let creators get a single value from one or more values

- Combining strings

- Computing Basic Match

- Comparison operators

- Logical operators

**Arithmetic Operators**

- Addition **+** or Subtraction **-**

- Division **/** or Multiplication **(*)**

- Increments **++** or Decrements **--** either adding one or subtracting one

- Modulus **%** Dividing two values and giving back the remainder

**String Operators**

- you can join together two or more strings using **+** 

**check example on (pages 78-79)**

# Chapter 4: “Decisions and Loops” (pp.145-162)

## Comparison and Logical Operators

- == *is equal to* for numbers, strings or booleans

- != *is not equal to* for numbers, strings or booleans

- === *strict equal to* check if data type and values are same

- !== *strict not equal to* check that data type and values are **not** the same

- *< or >*

- *<= or >=*

### Structuring Comparison Operators

operands are place on the side of the comparison operator
**this example, suing *>* as operator and *time and fail* as operands:**
(time > fail)

### Expressions Using Comparison Operators

operands are enclosed by parenthesis and on the sides of comparison operator
**example:**
(time + fail)>=(time1 + fail)

### Logical Operators
Can compare results of more than one comparison operator by:

- && *to test more than one condition*

- || *to test at least one of the conditions, resulting in all as either true or false*

- ! *inverts a single boolean, if !true returns false, if !false returns true*
