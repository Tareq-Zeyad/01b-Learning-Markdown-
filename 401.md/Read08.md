# List Comprehensions



### What are List Comprehensions ?

- List Comprehension(s) is exactly like any normal lists, except that they are a more compact way of creating lists and are much more flexible than for loops.

### Why use List Comprehensions ?

- To keep your code elegant and readable, as well as saving time and improving productivity. 

### What does the syntax of a list comprehension look like ?

```python
my_new_list = [ expression for item in list ]
```
```
- First is the expression we’d like to carry out. expression inside the square brackets.
- Second is the object that the expression will work on. item inside the square brackets.
- Finally, we need an iterable list of objects to build our new list from. list inside the square brackets.
```

### Code Examples:


#### Example 1: Creating a list with list comprehensions:

```python
# construct a basic list using range() and list comprehensions
# syntax
# [ expression for item in list ]
digits = [x for x in range(10)]

print(digits)
```

Output:
```
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
```

#### Example 2: Comparing list creation methods in Python:

```python
# create a list using a for loop
squares = []

for x in range(10):
    # raise x to the power of 2
    squares.append(x**2)

print(squares)
```

Output:
```
[0, 1, 4, 9, 16, 25, 36, 49, 64, 81]
```

#### Example 3: Multiplication with list comprehensions:

```python
# create a list with list comprehensions
multiples_of_three = [ x*3 for x in range(10) ]

print(multiples_of_three)
```

Output:
```
[0, 3, 6, 9, 12, 15, 18, 21, 24, 27]
```

#### Example 4: Using list comprehensions with strings:

```python
# a list of the names of popular authors
authors = ["Ernest Hemingway","Langston Hughes","Frank Herbert","Toni Morrison",
    "Emily Dickson","Stephen King"]

# create an acronym from the first letter of the author's names
letters = [ name[0] for name in authors ]
print(letters)
```

Output:
```
['E', 'L', 'F', 'T', 'E', 'S']
```




[Go Back](https://musaabshalaldeh.github.io/reading-notes/)