# Random Operators and How to Use Them

Random operators are important to know when you have lists, games or app’s hat require a random element to be selected.

## Random Operators

### Randint

Import random to use it then decide method needed based on data type.

This method will generate a random integer.

```
 random.randint()
```

This will generate a random integer between 1-5 and the first value should be less then the second.

```
print random.randint (0,5) 
```

### Random

This method is used for larger integers. You can multiply with this method and you will be able to get a larger range to generate numbers in.

```
random.random() * 100
```

### Choice

This method will give you a choice when you are using multiple data types or string data types. Create a list and call the choice method with the list argument.

```
new_list = [1, 70, ‘string’, 3, True, ‘Booleans_too’]
random.choice(new_list) 
```

Another example:

```
Random.choice([‘red’, ‘orange’, ‘yellow’, ‘green’, ‘blue’, violet’])
```

### Shuffle

This method shuffles the elements in a random place in an existing list. An example of this is seen below:

```
from random import shuffle
n = [[i] for i in range(15)]
shuffle(n)
```

### Randrange

This method will generate a random element from a range. It will use the start, stop and a step in the list.

```
random.randrange(start, stop[, step])

import random
for i in range(3)
    print random.randrange(0, 3, 5)
```

## Things I want to know more about

I would love to find out how to generate random information using the random operators when dealing with API information.

## Resources

>[How to use the Random Module in Python](https://www.pythonforbeginners.com/random/how-to-use-the-random-module-in-python)
>[What is Risk Analysis in Software Testing and how to perform it?](https://www.edureka.co/blog/risk-analysis-in-software-testing/)
>[TestCoverage](https://martinfowler.com/bliki/TestCoverage.html)

## Links

- >[Advanced Software Development](README.md)
