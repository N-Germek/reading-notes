# Passing Functions and Props

What does .map() return?
If I want to loop through an array and display each value in JSX, how do I do that in React? The short answer to this is to use curly braces with the map function, you would return an ***li*** element for each value, assign a ***ul*** element to an entire list variable that you create. An example of what this would look like is:

> const numArray = [1, 2, 3, 4, 5];

> const listArray = numArray.map((number) =>
***li***{number}***/li***);

>***ul***{listArray}***/ul***

Each list item needs a unique **key** such as an **ID**.

What is the purpose of a key? The purpose of a key is to be able to properly select the right sibling or child element. It is more specific.

What is the spread operator?
The spread operator is the syntax used to expand an iterrable object into the list of arguments. this is seen as the ellipsis **(...)**.

List 4 things that the spread operator can do.
The spread operator can copy an array, combine objects, add state in React, concatenating or combining arrays.

Give an example of using the spread operator to combine two arrays.

>const coffeeBeans = ['whole','ground','coarseGround','fineGround','espresso']
const moreBeans = [...coffeeBeans];
console.log(coffeeBeans) 
// Array(5) [ "" ]
fruits[0] = 'whole'
console.log(...[...coffeeBeans,'...',...moreBeans]) //  'whole','ground','coarseGround','fineGround','espresso' ... 'whole','ground','coarseGround','fineGround','espresso'

Give an example of using the spread operator to add a new item to an array.

Give an example of using the spread operator to combine two objects into one.
