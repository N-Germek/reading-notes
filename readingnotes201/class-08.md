## CSS Layout Deep Dive ## 

The magic of CSS starts in the layout and continues in the specifics of selectors, design, and the standard for defaults.

To understand the display, you will first have to know what all it encompasses. To begin **display** will determine if it is inline or block so the developer will know what type of elements to include in the page build.

- Inline Elements: Sit next to each other and preserve white space. They also can't have a size set in width and height.

- Block elements: Though they are greedy and take up a whole line, they are and can be made precise in size so as not to be a bully to the rest of the code going on. Margin is the only element deserving of such respect.

### Flexbox Versus Grid ###

The two primary layout templates are known as *Flexbox* and *Grid*. Though they are similar, they have two very different objectives to solve two problems.

- Flexbox will align elements next to each other inline with their child elements.  Flexbox can only access one axis on default.  The purpose is to stretch and take as much space as possible within the target element.  Items will not wrap, they will squish to make sure it all will fit on the same axis. Aligning, wrapping and justifying the content or items is needed to override these defaults however, flexbox will address them all as s group instead of individual pieces.

- Grid is designed to access multiple dimensions at once with defaults.  Though you can set specific display parameters in Flexbox to elements, Grid has those elements already embedded in the default code. Grid would be more useful when you are needing to utilize repetitive instructions and target individual pieces of an element. Though the template is a grid, all the parts and pieces of it are individual items that can be manipulated.

### What is the standard layout? ###

The simple answer: Flow layout.  Flow layout is the standard layout for CSS.  To make adjustments to elements displayed in normal flow, the defaults of those elements determine the layout.  Layout methods can target specific elements and that is how changes are made. Inline blocks and floats are an example of methods to control design layout in normal flow.

## Now where do we put it? ##

Well now we are looking at positioning. Position is another layout tool used and generally needed to help define a page stylistically. Where you plan to put text, what direction of the element you plan to adjust and how you want the parts to be visually stimulating and engaging all rely on your positioning.  For your intended user, will they be able to tell where the context ends or will it get mixed in with the data from an example.  Those answers can all be determined by utilization of positioning so the user can clearly see what part of the page is part of which.  

> [Home Page](README.md)
