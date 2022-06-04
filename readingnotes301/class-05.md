# Readings: Putting It All Together

## React Docs

What is the single responsibility principle and how does it apply to components?
The component should ideally only do one thing. If it grows too large with too much data, it should be broken down into smaller components.

What does it mean to build a ‘static’ version of your application? State is used for interactivity. To have a static app you have components that are able to change by re-using other components by passing data through props.

Once you have a static application, what do you need to add?
Once your app is static, you will need to call it through setState().

What are the three questions you can ask to determine if something is state?

1. Is it passed in from a parent via props? If so, it probably isn’t state.
2. Does it remain unchanged over time? If so, it probably isn’t state.
3. Can you compute it based on any other state or props in your component?

How can you identify where state needs to live?
State shoule live in a single component that all other components can access through props. Having one single component manage your state allows the rest to maintain their single responsibility principle.

## Higher-Order Functions

What is a “higher-order function”?
Higher order functions are functions that take in other functions as arguments or by returning them.

Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?
Line two is creating an arrow function that is setting the value of m to be less then n in the return statement.

Explain how either map or reduce operates, with regards to higher-order functions.
.map is a loop method that will transform the values of your entire array and return a new array with those values. It can be used to filter through an array and search for a specific key element of the array when organizing.
.reduce will take the first value of an array and reduce the element into the second value throughout the length of the array.  The return of this method is an array with the summary of the reduced index value.

- > [Table Of Contents](READING-NOTES/README.md)

- > [Home Page](README.md)

### Resources

- > [Thinking in React](https://reactjs.org/docs/thinking-in-react.html)

- > [Higher-Order Functions](https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK)
