### [HOME](README.md)

# [Transforms](https://learn.shayhowe.com/advanced-html-css/css-transforms/)

``transform`` property can be either *two* or *three* dimensional and either one comes with it's own additional sets of properties and values. 

**transform syntax** example:

div {
  -webkit-transform: scale(1.5);
     -moz-transform: scale(1.5);
       -o-transform: scale(1.5);
          transform: scale(1.5);
}

## 2D Transformss
2D
- works on the x and y axes
- ``rotate``  from (0deg); to (360deg);
- ``scale`` change how big or small the element appears
- ``translateX`` and ``translateY`` changes position either vertically or horizontally on the axis
-  ``skewX`` and ``skewY`` distorts elements on the axis
- transforms can be combined

### Transform Origin

``transform-origin`` can accept 1-2 values, if only one then it will be applied to both x and y axes. Individual values can be specified with numbers or words like ``bottom-right``

### Perspective

``perspective`` value can be set withing ``transform`` property  or can be use on the *parent* element over child elements

**perspective depth value** can be set as *none* or a lenght measurement

## 3D Transforms

- can change elements on x,y and **z** axes for depth.
- can ``rotate`` similarly to 2D but includes z
- can use ``scaleZ``
- can use ``translateZ``
- **cannot** be skewed on **z axes**

### Transform

For 3D, the ``transform-style`` can pair with value ``preserve-3d`` for 3D child elements or ``flat`` to keep them 2D

### Backface Visibility

set ``backface-visibility: hidden;`` to hide elements completely and keep them from showing when they are rotated or turned away. ``visible`` is the **default** value for backface-visibility.

[view demos](https://learn.shayhowe.com/advanced-html-css/css-transforms/)

[Transitions and Animations!!](https://learn.shayhowe.com/advanced-html-css/transitions-animations/)

Transitions and Animations can be written in CSS3 and can be created in a way to change affects when hovered over, targeted, focuses on or is active.

**transition**, determine styles for different states

- ``:hover``
- ``:focus``
- ``:active``
- ``:target``

``transition-property`` determines which specific properties will be alterd. Properties included in an elements different state will be affected by default but transition-property will have a say on what actually transitions.

[popular transitional properties list](https://learn.shayhowe.com/advanced-html-css/transitions-animations/)

**transition duration** timing values can be in seconds ``s`` or milliseconds ``ms`` and can even be fractional using decimals. *multiple* durations can be set.

**transition timing** looks like:

- ``ease-in``/``ease-out``
- ``ease-in-out``

and timing functions have a **cubic-bezier curve** behind whic can be specifically set

- ``cubic-bezier(x1,y1,x2,y2)
-  ``step-start/stop``

can also use ``transition-delay``

### Animations

Animations can hav duration,timing function and dalays. Keyframes for animations need to be declared and assigned to an element. They can be customized with ``iteration-counts`` and be specified in which direction to go like **normal**,**reverse** or **alternate**

Animations can also be given the ``animation-play-state`` property so it can be played or paused with ``running`` and ``paused``

**Animation Fill Mode** how elements should be styled before, during or after the animation is played through.

- ``none``
- ``forwards``
- ``backwards``

[checkout animation demos and specifics](https://learn.shayhowe.com/advanced-html-css/transitions-animations/)

[8 Simple Transitions](http://www.webdesignerdepot.com/2014/05/8-simple-css3-transitions-that-will-wow-your-users/)

- **fade in**
- **change color**
- **grow and shring** (very cool hover effect)
- **rotate elements** left or right for example
- **square to circle**
- **3D Shadow**
- **swing**!!
- **inset border**

(very good quick tip site)

## [6 Buttons Animated](https://codepen.io/retyui/pen/ByoaXV)

## [Animation Keyframes!](https://codepen.io/akshaychauhan/pen/oAfae)

## [Trippy 404 Animation!](https://codepen.io/akshaychauhan/pen/oAfae)

## [CSS Bounce](https://codepen.io/dp_lewis/pen/gCfBv)

[What Google Learned From Its Quest to Build the Perfect Team](https://www.nytimes.com/2016/02/28/magazine/what-google-learned-from-its-quest-to-build-the-perfect-team.html)

Google found that it was hard to determine any specific sort of patterns of what makes a good team of people when it comes to characteristics and habits. Once they more seriously considered norms, formally agreed upon or unwritten it was understood that norms were the key to what grounds a good team. Although there are many types of norms so then came the question of which were the most promising. It was decided that the "right" norms could improve the level of collective intelligence while the "wrong" norm could keep an entire team from succeeding no matter their level of intelligence as individuals. Some of the better behaviors found are that everyone takes turns speaking and carrying along a conversation and a shared level of social sensitivity. Individuals on the better performing teams felt supported and able to speak up without backlash so a healthy level of interpersonal trust and mutual respect is necessary for individuals to feel their opinions and ideas mattered. A sense of psychological safety in a work environment and especially within a team improves not only individual performance but increased levels of team performance as well.

### [HOME](README.md)