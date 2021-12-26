# Pythonisms



# Dunder Methods



### What Are Dunder Methods?
In Python, special methods are a set of predefined methods you can use to enrich your classes. They are easy to recognize because they start and end with double underscores, for example __init__ or __str__.

As it quickly became tiresome to say under-under-method-under-under Pythonistas adopted the term “dunder methods”, a short form of “double under.”

These “dunders” or “special methods” in Python are also sometimes called “magic methods.” But using this terminology can make them seem more complicated than they really are—at the end of the day there’s nothing “magical” about them. You should treat these methods like a normal language feature.

Dunder methods let you emulate the behavior of built-in types. For example, to get the length of a string you can call len('string'). But an empty class definition doesn’t support this behavior out of the box:

```python
class NoLenSupport:
    pass

>>> obj = NoLenSupport()
>>> len(obj)
TypeError: "object of type 'NoLenSupport' has no len()"
```

To fix this, you can add a __len__ dunder method to your class:

```python
class LenSupport:
    def __len__(self):
        return 42

>>> obj = LenSupport()
>>> len(obj)
42
```

### What are the magic methods available in python?

- __new__(self) return a new object (an instance of that class). It is called before __init__ method.
- __init__(self) is called when the object is initialized. It is the constructor of a class.
- __del__(self) for del() function. Called when the object is to be destroyed. Can be used to commit unsaved data or close connections.
- __repr__(self) for repr() function. It returns a string to print the object. Intended for developers to debug. Must be implemented in any class.
- __str__(self) for str() function. Return a string to print the object. Intended for users to see a pretty and useful output. If not implemented, __repr__ will be used as a fallback.
- __bytes__(self) for bytes() function. Return a byte object which is the byte string representation of the object.
- __format__(self) for format() function. Evaluate formatted string literals like % for percentage format and ‘b’ for binary.
- __lt__(self, anotherObj) for < operator.
- __le__(self, anotherObj) for <= operator.
- __eq__(self, anotherObj) for == operator.
- __ne__(self, anotherObj) for != operator.
- __gt__(self, anotherObj)for > operator.
- __ge__(self, anotherObj)for >= operator.
Arithmetic Operators
- __add__(self, anotherObj) for + operator.
- __sub__(self, anotherObj) for – operation on object.
- __mul__(self, anotherObj) for * operation on object.
- __matmul__(self, anotherObj) for @ operator (numpy matrix multiplication).
- __truediv__(self, anotherObj) for simple / division operation on object.
- __floordiv__(self, anotherObj) for // floor division operation on object.
Type Conversion
- __abs__(self) make support for abs() function. Return absolute value.
- __int__(self) support for int() function. Returns the integer value of the object.
- __float__(self) for float() function support. Returns float equivalent of the object.
- __complex__(self) for complex() function support. Return complex value representation of the object.
- __round__(self, nDigits) for round() function. Round off float type to 2 digits and return it.
- __trunc__(self) for trunc() function of math module. Returns the real value of the object.
- __ceil__(self) for ceil() function of math module. The ceil function Return ceiling value of the object.
- __floor__(self) for floor() function of math module. Return floor value of the object.
Emulating Container Types
- __len__(self) for len() function. Returns the total number in any container.
- __getitem__(self, key) to support indexing. LIke container[index] calls container.__getitem(key)explicitly.
- __setitem__(self, key, value) makes item mutable (items can be changed by index), like container[index] = otherElement.
- __delitem__(self, key) for del() function. Delete the value at the index key.
- __iter__(self) returns an iterator when required that iterates all values in the container.



# Iterators

### what is python Iterator? 

Python has a dedicated object called iterators used for iterating over iterable objects. These iterators are implemented using two methods, iter()iter() and next()next(), that are commonly known as iterator protocol. The task of iter()iter() is to initialize the method; whereas, next()next() is used to perform an iteration over the iterable object.

### Example of a simple loop in python syntax:

```python
numbers = [1, 2, 3]
for n in numbers:
    print(n)
```
### How do for-in loops work in Python?

our Repeater class that apparently supports the iterator protocol, and we just ran a for-in loop to prove it:

```python
repeater = Repeater('Hello')
for item in repeater:
    print(item)
```
Now, what does this for-in loop really do behind the scenes? How does it communicate with the repeater object to fetch new elements from it?

To dispel some of that “magic” we can expand this loop into a slightly longer code snippet that gives the same result:

```python
repeater = Repeater('Hello')
iterator = repeater.__iter__()
while True:
    item = iterator.__next__()
    print(item)
```
As you can see, the for-in was just syntactic sugar for a simple while loop:

It first prepared the repeater object for iteration by calling its __iter__ method. This returned the actual iterator object.
After that, the loop repeatedly calls the iterator object’s __next__ method to retrieve values from it.


# Generators

### What are Generators? 

A generator is a routine that can be used to control the iteration behaviour of a loop. All generators are also iterators. A generator is very similar to a function that returns an array, in that a generator has parameters, can be called, and generates a sequence of values.

> A generator is always an iterator but not every iterator is an generator.

### Differences between Generator function and Normal function
Here is how a generator function differs from a normal function.

- Generator function contains one or more yield statements.
- When called, it returns an object (iterator) but does not start execution immediately.
- Methods like __iter__() and __next__() are implemented automatically. So we can iterate through the items using next().
- Once the function yields, the function is paused and the control is transferred to the caller.
- Local variables and their states are remembered between successive calls.
- Finally, when the function terminates, StopIteration is raised automatically on further calls.



### Create Generators in Python
It is fairly simple to create a generator in Python. It is as easy as defining a normal function, but with a yield statement instead of a return statement.

If a function contains at least one yield statement (it may contain other yield or return statements), it becomes a generator function. Both yield and return will return some value from a function.

The difference is that while a return statement terminates a function entirely, yield statement pauses the function saving all its states and later continues from there on successive calls.


