# [Shay Howe's intro to Responsive Web Design](https://learn.shayhowe.com/advanced-html-css/responsive-web-design/)

Responsive web design is how a website is built to display suitably on any device or screen size.

**Responsive vs Adaptive vs Mobile**

*responsive* and *adaptive* mean pretty much the same thing. Both refer to the design of a website made to be capable of *changing* or becoming *modified*. 
**adaptive** websites are created with a groupe of *preset factors*.
**responsive** will response in accordance to different factors for example, *viewport* width.

**mobile** is to create a separate site specifically for mobile devices. (not usually ideal because it comes with many obstacles).

## Flexible Layouts

**Flexible layout** is on of three main components of a flexible website.

*flexible grid*:

- dynamically resizes in accordance to *any* width
- built with *relative length units* (**%** or **em**)
- relative lengths are used for common property values ``width``, ``margin`` or ``padding``

**new** units for *relative length*

- ``vw`` viewports width
- ``vwmin`` minimum of the viewports *height* and *width*
- ``vh`` viweport height
- ``vmax`` max of vieworts *height* and *width*

don't use ~~fixed measurements~~ for for flexible layouts. Layouts need to be able to adapt. 

## Media Queries

**Media Queries** is another of the three main components of a flexible website. Media queries allow the ability to specify styling for individual *browser* and *devices*. It as the ability to apply **targeted styling*

**initializing media queries**:

- ``@media`` *inside* of existing stylesheet
- ``@import`` to import *new* stylesheet or to link to a separate stylesheet.
``@media`` **preferred**

**common media** *types*:

- ``all``
- ``screen``
- ``print``
- ``tv``
- ``braille``

**logical operators in media queries**

- ``and`` allows additional conditions to be added
- ``not`` specifies a query **but not** the one specifically identified
- ``only`` hides styles from devices or browsers that don't support media queries(HTML4)

using ``not`` and ``only``, media *type* can be left off because the media type will be defaulted to **all**

**height & width media features**

- ``height`` and ``width`` will find proper dimensions for device/browser inputs. Height and width features are based off of the viewport rendering area/browser window and can be *prefixed* for example, using ``min`` or ``max`` for width/height.

**orientation** feature: determines if device is *landscape* or *portrait*

**aspect ratio**

``aspect-ratio``/ ``device-aspect-ratio`` specifies pixel ratio of width/height for rendering are/output device.

**resolution**

``resolution`` does not accept min and max prefixed and will accept *dots per pixel*, or *dots per inch*

**other media features**

- ``color``
- ``color-index``
- ``monochrome``
*identify available output colors*

**using** *mobile first* **media queries**

using styles for smaller viewports as default for website, then adding styles *as the window grows* using media queries. There is a risk of "wasting bandwidth" by having to adapt *for* mobile from styles other than because many users want a "snappy website".

**identifying and using vieport**

- using ``viewport`` meta tag with height/width will define them for the viewport. You can use ``device-height`` for example.
- control how website is scaled for devices. For example ``minimum-scale`` or ``initial-scale`` or ``user-scalable``
- viewport *resolution* using ``dpi`` when pixel control is needed.

## Flexible Media 

**Flexible Media** is the third of the three main components of a flexible website. It's important that the media on a website will adjust with other styling properties as they adapt to viewports.

**quick fix** ! = use ``max-width: 100%`` to make sure the media will scale down in accordance to its *containers width* as the viewport size changes.

**Flexible Embedded Media**

``max-width`` won't work for all media, specifically iframe and embedded media like Youtube. To make it work the element should be **absolutely positioned** within the parent element. The *parent element* need a ``width`` of **100%**  so it's scaled to width of viewport and also need ``height`` of **0** to trigger ``hasLayout`` when in internet explorer. Set ``padding`` of bottom of parent element with a *value* of the same *aspect ratio* of the video.e.g. video with aspect ratio of 16:9 divided by 16 = .5625 and will need parent element bottom padding set at 56.25% not ~~top~~.


# [All About Floats](https://css-tricks.com/all-about-floats/)

``float`` is a positioning property that can dictate how *text flow* happens around the element. The element that is floated *remains* part of the flow of the entire webpage, being different from an element given absolute position which doesn't affect the positioning of elements, nor will they be affected.

**What floats are used for**

- can create an entire web layout
- helpful for smaller instances of layouts like when a image changes size, the text in the box with it will *reflow* in accordance.

**Clearing the Float**

A **sister** property of float is ``clear``. An element with this property will not move up, but *down* past the flow.

*valid values for ``clear``*

- ``both`` clearing floats coming from either direction
- ``left``/``right`` clearing a float from a specific direction
- ``none`` being the default, usually necessary only when removing a clear value from a cascade.
- ``inherit`` not supported by **IE** clears *only* the left or right float.

**Preventing "collapsing"**

If a parent element only contains floated elements, it's height will collapse. Be mindful of this because it is not always obvious. To fix it, clear the float *after* floated element but *before* the close of the container.

**Techniques to Clear Floats**

- if the *succeeding* element is known use ``clear:both``
- **empty div method**, create an empty div, sometimes might need to use ``<br>`` or another element.
- **overflow method** set the overflow property on a parent element. set to auto or hidden and it will expand to contain the floats.
- **easy clearing method* apply ``clearfix`` selector, followed by ``:after``

**some problems with floats**

- *pushdown* when an element *inside* of the floated element has a set width wider than the float... Use ``overlow:hidden`` to fix this issue.
- *double margin bug* in IE6, if a margin is set in the same direction as the float it will result in a *double margin*. To fix this use ``display:inline``.
- *3px jog* the text next to a floated element gets "kicked away".To fix this, set a width or height on the text.
- *bottom margin bug* in IE7 when a floated parent has floated children, the bottom margin of children is ignored by parent element. To fix this use ``bottom padding`` on the parent element.
