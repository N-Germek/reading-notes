## CSS Transforms; Time to Animate ##

The transform property in CSS is how animation truly starts. Transform can be two-dimensional or three-dimensional yet they all start at the *transform origin* since it is exactly 50% horizontal and vertical on the element targeted. Though browser supports fight sometimes, they are becoming closer allies in the dev's toolbelt.

Here is your starting code with browser overrides:

>div {
  -webkit-transform: scale(1.5);
    -moz-transform: scale(1.5);
      -o-transform: scale(1.5);
         transform: scale(1.5);
}

2D transformations include rotate, scale, cube, skew and translate. translateX targets the x - axis, while translateY targets the y - axis and to target both, start with the x - axis.

It is important to remember that you can combine transforms, yet if improperly placed, the cascade effect of CSS will over-write your work.

Perspective are necesesary to activate 3D animations. Perspective depth value are set none or a length measurement with higher values being further for the figure. *Perspective origin* is similar to transform origin, yet the difference is perspective origin determines where the coordinates are used to change the item. Using rotateZ we access the *z* axis for 3D rotations. Other elements can also be used for 3D similar to 2D. Those elements include 3D scale, 3D translate.  3D Skew is not a possible transformation.

Backface visiablility is a transform element used to make the back of an image visiable or not. Imagine flipping a card over, you see the designs on the back as the standard, with backface visiability, you can determine if you turn it over and it is mirrored or see through.

Transitional properties as seen below, are a handful of properties that developers now have access to complere using CSS3 without needing to uses JS or HTML.

>"background-color, background-position, border-color, border-width, border-spacing, bottom, clip, color, cropfont-size, font-weight, height, left, letter-spacing, line-height, margin, max-height, max-width, min-height, min-width, opacity, outline-color, outline-offset, outline-width, padding, right, text-indent, text-shadow, topvertical- align, visibility, width, word-spacing, z-index"

Duration, timing, delay are all speed elements that can transform. *@keyframe* is where you set animation name breakpoints and properties for the animation to ppick up where the transition left off.

Other then the tips and tricks listd above, there are 8 other transformations that give instant gratification and captivate your users.  Those are: fade in, change color, grow, shrink, rotate, square to circle, 3D shadow, swing and inset border.

Here is example code for transform using nested elements:

CSS
>.rotate {
  transform: perspective(200px) rotateY(45deg);
}
.three-d {
  transform-style: preserve-3d;
}
.box {
  transform: rotateX(15deg) translateZ(20px);
  transform-origin: 0 0;
}

## Things I want to learn more about: ##

There are many ways to engage your users and how to gain their interest. One thing I want to learn more about is weather there is a maximum amount of style choices you can put on one element without overeriding a prior style choice.

source: [CSS Transforms](https://learn.shayhowe.com/advanced-html-css/css-transforms/)

source: [8 SIMPLE CSS3 TRANSITIONS THAT WILL WOW YOUR USERS](https://www.webdesignerdepot.com/2014/05/8-simple-css3-transitions-that-will-wow-your-users)
