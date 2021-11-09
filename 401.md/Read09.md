# Dunder Methods in Python


### What Are Dunder Methods?

- They are a special set of predefined methods that you can use to enrich your classes. They are easy to recognize because they start and end with double underscores.

Example:
```
__init__ or __str__
```

### Why Do We Use Dunder Methods in Python ?

- We used under methods in Python to define overloaded behaviours of predefined operators in Python.


### Example of a Class That Has Dunder Methods:

```python
class Account:
    """A simple account class"""

    def __init__(self, owner, amount=0):
        """
        This is the constructor that lets us create
        objects from this class
        """
        self.owner = owner
        self.amount = amount
        self._transactions = []
    
    def __repr__(self):
        return 'Account({!r}, {!r})'.format(self.owner, self.amount)

    def __str__(self):
        return 'Account of {} with starting amount: {}'.format(
            self.owner, self.amount)
```

And if we invoke those methods, we will get the following output:

```python
>>> str(acc)
'Account of bob with starting amount: 10'

>>> print(acc)
"Account of bob with starting amount: 10"

>>> repr(acc)
"Account('bob', 10)"
```

# Statistics - Probability


### What is probability?

-In short, "what is the chance of event to happen ?" and an event is some outcome of interest. 

Real life Example:
```
Coin Toss
its either going to be Heads or Tails, 50% chance for each to happen.
```

### How can we calculate the probability ?

Using the example above, first we count how many times are event of interest can occur (say flipping heads) and dividing it by the sample space. Thus, probability will tell us that an ideal coin will have a 1-in-2 chance of being heads or tails.


### From statistics to probability:

![statistics to probability image](https://i.imgur.com/GtbawRt.jpg)


In Code:

```python
import random
def coin_trial():
heads = 0
for i in range(100):
if random.random() <= 0.5:
heads +=1
return headsdef simulate(n):
trials = [] for i in range(n):
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


[Go Back](https://musaabshalaldeh.github.io/reading-notes/)