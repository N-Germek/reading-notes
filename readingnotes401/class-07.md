# Global and Non-local

## LEGB Rules

Local
Enclosing
Global
Built-in

The LEGB rules are the rules that determine the sequence at which code is ran.

The importance of scope when deciding variable names are partially for identifying which part of your code you are working on. Additionally, during debugging being able to distinguish which script or module the errors are being thrown from.

## Scope Definitions

Global variables are ones in which all parts of your code can access. Modules themselves are usually set in the global scope. Local scope variables are available locally to the part of your code that you write them for. When calling a function, you are creating a new local scope. This in and of itself acts as a pointer for specific places that your code could have broken. Enclosing scope is the scope that encapsulates inner or nested functions. Built-in scope is a python scope in which your code is run at the initiation of your script or when you open an interactive session.

## Things I Want to Learn More About

I am still trying to understand the mathematics in BigO. I still need to write them down each time and look at it in the form of a formula before I can deduce what is the BigO of a project.

## Resources

[Python Scope](https://realpython.com/python-scope-legb-rule/)

## Links

- >[Advanced Software Development](README.md)
