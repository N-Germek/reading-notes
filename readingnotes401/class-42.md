# Pythonic Dunder Methods

## Why are they needed and what are some of them?

For empty classes, dunder methods are the way to perform the task. 

__len__ () is the dunder length method for the length of a string. 

__getitem__() is to enable string slicing. 

__init__() is to initialize an instance. 

__repr__() the official strong representation of a string object. 

__str__() endusers informal or nicely printed string method. 

__reversed__() is to iterate in reverse. 

Use the functions.totalordering decorator to be able to utilize any of the below without using all of the below. 

```python

>>> dir('a')
['__add__',
...
'__eq__',    <---------------
'__format__',
'__ge__',    <---------------
'__getattribute__',
'__getitem__',
'__getnewargs__',
'__gt__',    <---------------
...]
```

## Things I want to know more about

### Resources

[Dunder Methods](https://dbader.org/blog/python-dunder-methods)

### Links

- >[Advanced Software Development](README.md)
