# FileIO and Exceptions

## Reading files in Python

Files are the meat of your content in python. They start with a header, then have contents or data, finally they have the end of file.  Files should always be opened using file = open('file_name.txt') method and closed after use with the close method of file.close().  By using a try method you can assure yourself that the file will be closed even if an error occurs. An example on how this can look in pseudocode is below.

```
file = open('file_name.txt')
try:
    # if error occurs, continue to close file
finally:
    file.close()
```

Another method to close is to use the with method as seen below in pseudocode.

```
with open('file_name.txt') as file:
try:
    # if error occurs, continue to close file
# the file is automatically closed at this point.
```

## Exceptions

File exceptions are when a file is created that is syntactically correct, yet the results from your code render an error.  The last line will let you know what the error is. Raising an exception is another way to force it when testing your code. Some examples of methods that can be used to ensure proper error handling of exceptions in your code are to use try/except, try/except/else or try/except/else/finally as assertions.

## Things I want to learn more about

I am curious if you can create a base case to stop a loop while still being able to error test and force one.

### Resources

> [Read and Write Files in Python](https://realpython.com/read-write-files-python/)

>[Exceptions in Python](https://realpython.com/python-exceptions/)

>[Read & Write Files in Python - Companion Video](https://realpython.com/lessons/reading-and-writing-files-python-overview/)

### Links

- > [Advanced Software Development](README.md)
