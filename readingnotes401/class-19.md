# Automation and Regex

## Getting started with Regex in Python

To start you will want to import the re library.

Ordinary characters can convert to basic patterns. See example below:

```python

pattern = r"Cookie"
sequence = "Cookie"
if re.match(pattern, sequence):
    print("Match!")
else: print("Not a match!")
```

The “r” at the beginning is a raw string literal so that you can distinguish part of the string versus another code or escape character.

Wild card characters are special characters that don’t match themselves but have a special meaning. The search() function allows you to search and the group() function returns the string matched by re.

- -A. Matches any single characters except beeline characters.
- ^A matches the start of the string.
- $ matches the end of the sting.

## Things I want to know more about

### Resources

[Python Regular Expression Tutorial](https://www.datacamp.com/tutorial/python-regular-expression-tutorial)

[shutil — High-level File Operations](https://pymotw.com/3/shutil/)

[Super quick Python automation ideas](https://www.youtube.com/watch?v=qbW6FRbaSl0&t=69s)

### Links

- >[Advanced Software Development](README.md)
