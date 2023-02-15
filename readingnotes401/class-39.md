# React Context

React context allows us to share data saved in state through our componentds more easily.  Great use would be to pass data used in many if not all components in your app. Examples include Themes, User data, Location-Specific data. The context data should not need to be updated often thus they are similar as global variables for React.

Props drilling means passing down props multiple levels to a nested component through cojmponents not dependant on it.

Here is an example of how props drilling works:

```python
export default function App({ theme }) {
  return (
    <>
      <Header theme={theme} />
      <Main theme={theme} />
      <Sidebar theme={theme} />
      <Footer theme={theme} />
    </>
  );
}

function Header({ theme }) {
  return (
    <>
      <User theme={theme} />
      <Login theme={theme} />
      <Menu theme={theme} />
    </>
  );
}
```

React context is the API built to avoid the use of props drilling by calling the createContext method. It will take the context, wrap the provider around the component tree, through the value prop it will add value to it then read the value in any component by usung the context consumer.

The basic example of how that looks is below:

```python
import React from 'react';

export const UserContext = React.createContext();

export default function App() {
  return (
    <UserContext.Provider value="Reed">
      <User />
    </UserContext.Provider>
  )
}

function User() {
  return (
    <UserContext.Consumer>
      {value => <h1>{value}</h1>} 
      {/* prints: Reed */}
    </UserContext.Consumer>
  )
}
```

## Things I want to know more about

### Resources

[NextJS](https://nextjs.org/learn/basics/create-nextjs-app)

[React Context for Beginners](https://www.freecodecamp.org/news/react-context-for-beginners/)

### Links

- >[Advanced Software Development](README.md)
