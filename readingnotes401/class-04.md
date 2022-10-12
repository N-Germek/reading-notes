# Classes, Objects, Recursive Thinking and Pytest Fixtures and Coverage

## Classes and Objects

Objects are the entirety of functions and variables into a singular entity. Objects get their variables from classes which are basically the template for items in your files.

Ways to target items in objects through Python are as follows:

```
class This_Class:
    variable = 'this_variable'

    def function(self):
        print("This is a message inside the class.") 

<!-- This assigns the class to the object -->

this_object = This_Class()   

<!-- This will access the variable -->

this_object.variable

<!-- To access the variable as a string -->

print(this_object.variable)

<!-- this is how you can create multiple objects to the same class with different strings in them -->

this_object = This_Class()
that_object = This_Class()

that_object.variable = 'that_variable'

print(this_object.variable)
print(that_object.variable)

<!-- To access object functions -->

this_object.function()
```

__init__() is a function that is called when the class is being initiated and it assignes values in a class.

## Things I want to learn more about

When would you need to utilize a class in a realworld application versus simply accessing the object or function?

### Resources

> [Classes and Objects](https://www.learnpython.org/en/Classes_and_Objects)

>[Thinking Recursively](https://realpython.com/python-thinking-recursively/)

>[Python Testing with pytest: Fixtures and Coverage](https://www.linuxjournal.com/content/python-testing-pytest-fixtures-and-coverage)

### Links

- > [Advanced Software Development](README.md)
