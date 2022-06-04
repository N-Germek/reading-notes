# React State Versus Props

Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’? Render happens first.

What is the very first thing to happen in the lifecycle of React?
Mounting is the first stage to happen in.

Put the following things in the order that they happen:
componentDidMount, render, constructor, componentWillUnmount, React Updates.
constructor, render, componentDidMount, React Updates, then componentWillUnmount if needed.

What does componentDidMount do? This method is used to load anything using a network request or the DOM and is invoked immediately after the component is mounted.

Methods used on components are called lifecycle events.

## React State vs Props

What types of things can you pass in the props? Arguments to a function.

What is the big difference between props and state? Props you pass into a component and state is handled outside of the component. State is solely inside that component.

When do we re-render our application? When you change the state of the application, then it will re-render. In props, you will need to render it manually.

What are some examples of things that we could store in state? When we change something in our application, like a form from user input, that is when we would be able to continually update information. Any input elements or checkboxes are when you are needing state.

- > [Home Page](README.md)

References:

> [YouTube React State Vs Props](https://www.youtube.com/watch?v=IYvD9oBCuJI)

> [React: Component Lifecycle Events](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)
