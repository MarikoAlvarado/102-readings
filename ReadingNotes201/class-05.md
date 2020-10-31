### [HOME](README.md)

# Duckett HTML book: Chapter 5: “Images” (pp.94-125)

## Adding Images

Use **< img src="urlhere" alt="description of image here" title="title of image"/ >**

**height** and **width** can be used as well to make adjustments to image size
**align** can also be used within < img / > to designate alignment *right*,*left*, *top*, **middle*, or *bottom*

*How* and image is displayed depends on where it is place in HTML code.

Some examples of placement:

- before *< p >*

- inside *< p >*

- middle of *< p >*

Only block elements will appear on a new line, *not* inline elements

## Formatting Images

**GIF** and **PNG** when using image with few colors or an image of mostly the same color

*save* image at same specified dimensions that they will be on page

*crop* images carefully

set image by *pixels* vs centimeters and inches

*vector* images are usually created with adobe illustrator. *bitmap* version of a vector image are needed.

can also use **animate gif** and **transparent** gifs

## Optimizing Images

Check to see what size an image already on a webpage is before replacing it by looking at its *properties*.

Image can be included within a **< figure >** caption, or include a caption for an image from a separate element.

# Duckett HTML book: Chapter 11: “Color” (pp.246-263)

Use a *color picker*!

In CSS, color can be specified by:

- RGB values

- RGBA values for opacity

-HSL/HSLA gives control for *hue, saturation* and *lightness* of color

- Name

- Hex Code

**Be mindful of contrast so text can be clearly read**.

# Duckett HTML book: Chapter 12: “Text” (pp.264-299)

## Typeface

Text plays a major part in how easy it is to read a page

Can be:

- **regular**

- **bold** / **font-weight**

- **italic** / **font-style**
while keeping text size.

can be styled by **weight,style** and **stretch**

Options of:

- **text-align**

- **vertical-align**

- **letter-spacing**

- **word-spacing**

- **text-decoration**

- **text-transform**

- **line-height** / *leading*

- **text-indent**

- **text-shadow**

**Can make specific changes to only *:first-letter* and/or *:first-line* hint: remember CSS Diner???

### Typeface Terms

- SERIF

- SANS-SERIF

- MONOSPACE

**Choose typeface according to which is supported by user browser**

**many typefaces can only be used with a LICENSE**

Specify your Typeface using **font-family**

Specify size using **font-size** in:

- Pixels

- Percentages

- EMS

If using a font that **is not** installed on user browser use **@font-face**. **(pp.277)** - be mindful of this!!!

### [HOME](README.md)