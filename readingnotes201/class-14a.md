## CSS Transforms; Time to Animate ##

The transform property in CSS is how animation truly starts. Transform can be two-dimensional or three-dimensional yet they all start at the *transform origin* since it is exactly 50% horizontal and vertical on the element targeted. Though browser supports fight sometimes, they are becoming closer allies in the dev's toolbelt.

Here is your starting code with browser overrides:

>>div {
  -webkit-transform: scale(1.5);
    -moz-transform: scale(1.5);
      -o-transform: scale(1.5);
         transform: scale(1.5);
}

2D transformations include rotate, scale, cube, skew and translate. translateX targets the x - axis, while translateY targets the y - axis and to target both, start with the x - axis.

It is important to remember that you can combine transforms, yet if improperly placed, the cascade effect of CSS will over-write your work.

Perspective are necesesary to activate 3D animations. 

source: [CSS Transforms](https://learn.shayhowe.com/advanced-html-css/css-transforms/)