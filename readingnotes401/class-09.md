# Dunder Methods and Statistical Probabilities

What are dunder methods?

Dunder methods aka magic methods are special predefined methods used to enrich your classes. They start with and end with double underscores.

Dunder methods emulate built-in methods. They enable building on empty classes when some methods aren’t able to do so. For example the *len(‘string’)* method isn’t able to run in an empty class so the *__len__* method can be implemented on the empty class instead.

An example of this behavior is below:

```python

class NoLenSupport:
    pass

>>> obj = NoLenSupport()
>>> len(obj)
TypeError: "object of type 'NoLenSupport' has no len()"
```

Versus:

```python

class LenSupport:
    def __len__(self):
        return 42

>>> obj = LenSupport()
>>> len(obj)
42
```

Slicing is another example with by implementing the *__getitem__* method you can use Python's list slicing syntax.

## Statistics: Probability

Probability in statistics is the process of identifying what the chances of an event to happen. An example is the formula of gaining an average of an event having a repeated pattern as an end result. Adding all the identical events then dividing by the amount of their occurance is the basic formula to identify the average amount of it happening.  

An example often coin tosses showing the probability of landing on heads versus tails is below:

```python
import random
def coin_trial():
heads = 0
for i in range(100):
    if random.random() <= 0.5:
        heads +=1
    return heads
def simulate(n):
    trials = []
    for i in range(n):
        trials.append(coin_trial())
    return(sum(trials)/n)
simulate(10)
>>> 5.4
simulate(100)
>>> 4.83
simulate(1000)
>>> 5.055
simulate(1000000)
>>> 4.999781
```

Normal distribution in data science is the distribition of probability across all events. The statistical image of it similar to a hill. The x-axis: values of events we want to know probability of. The y-axis: the probability associated with each event, from 0 to 1. both are evaluated simultaniously to determine the probability of an event.

## Statistics: Central Limit Theorem

This is the theory that the distribution of probability across repeated estimates will look like a normal distribution. The average mean of many trials will come closer to the true mean of the event.

## Statistics: Three Sigma Rule

The empirical rule (68-95-99) and governs how many of the observations fall within the distance of the mean for our event when given a normal distribution. 68% of observations will fall between one standard deviation of the mean, 95% will fall within two deviations and 99.7% will fall within thre deviations. Basically it governs how much data is contained under diferent intervals of a normal distribution.

## Things I want to know more about

Statistics in general are fascinating to me.  How and if can BigO be affected by the statistics of probability when you are testing your efficiency in your problem domain?  If it does not affect it, would there ever be a time in which BigO is not absolute for your calculation of function or method efficiency?

## Resources

[Enriching Your Python Classes With Dunder (Magic, Special) Methods](https://dbader.org/blog/python-dunder-methods)

[Tutorial: Basic Statistics in Python — Probability](https://www.dataquest.io/blog/basic-statistics-in-python-probability/)

## Links

- >[Advanced Software Development](README.md)

- >[Parsing Example](quotes.txt)
