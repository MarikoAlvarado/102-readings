### [HOME](README.md)

# [Easily Create Stunning Animated Charts With Chart.JS](https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/)

- Use **chart.js** plugin to use HTML canvas to design the chart.
 1. Download Chart.JS and copy Char.min.js from folder into working directory

- create html and import script from file

2. create canvas element in HTML

- add ``<script></script>`` at bottom of body element
- add ``<canvas></canvas>`` element
- instatiate content to chart
- add options 

3. drawing bar chart, similar to previous steps:

- canvas
- retrieve element
- create graph
- add bar chart data

 # [Canvas](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Basic_usage)

 - ``<canvas></canvas>`` only uses ``width`` and ``height`` which can also be set using DOM, either way they are both optional.

 - Canvas ID element is **global** so it is *best* to always us ID so it can be more easily identified

 **FALLBACK CONTENT**

 -provide fallback content so it can be displayed in older browsers by placing alternat conent *inside* of the element

 **RENDERING CONTEXT**

 - rendering contexts create and manipulate the displayed content.

 - to display content, render content using ``getContext`` after getting element by id

**CHECK FOR SUPPORT** by using ``getContext``

# [Drawing Shapes With Canvas](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes)

The **coordinate space**/**grid** uses ``(x,y)`` coordinates for position and rotations

**DRAW USING CANVAS** 

- draw, fill and outline **rectangles** or make them fully tranparent

- Create **paths** using *drawing commands* - then you can **stroke** or **fill** path to render it

[refer to drawing principles](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes)

# [Apply Styles and Colors](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Applying_styles_and_colors)

- Colors = string representing CSS color
- Transparency = draw semi-transparent shapes by setting ``globalAlpha`` propery or assigning style using **RGBA**
- Line Styles = multiple options to assign lines
- Gradients = using ``CanvasGradient`` object can be assignt fill/stroke style properties
- Patterns = instead of using loop to create a pattern you can use ``createPatter()``
- Shadows = uses four properties following ``shadow``. OffsetX, OffsetY, Blur and Color

# [Drawing Text](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_text)

**render** using:

``fillText (text,x,y[, maxWidth])
``strokeText(text, x, y [, maxWidth])

**Style text**

font = value
textAlign = value
textBaseline = value
direction = value

### [HOME](README.md)