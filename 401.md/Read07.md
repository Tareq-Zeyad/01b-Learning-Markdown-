# Scopes in Python

There are 2 types of scopes in Python and in other programming languages in general

### Global Scope Variable(s)

-A variable declared outside of the function. This means that a global variable can be accessed inside or outside of the function.

Example:

```python
x = "global"

def foo():
    print("x inside:", x)


foo()
print("x outside:", x)
```

output will be: 
```
x inside: global
x outside: global
```

### Local Scope Variable(s)

-A variable declared inside the function's body or in the local scope is known as a local variable.

Example:

```python
def foo():
    y = "local"
    print(y)

foo()
```

output will be:
```
local
```



# Nonlocal Variables

What are Nonlocal Variables and where are they used ?

-Nonlocal variables are used in nested functions whose local scope is not defined. This means that the variable can be neither in the local nor the global scope.

Example:

```python
def outer():
    x = "local"

    def inner():
        nonlocal x
        x = "nonlocal"
        print("inner:", x)

    inner()
    print("outer:", x)

outer()
```


Output:
```
Output

inner: nonlocal
outer: nonlocal
```










[Go Back](https://musaabshalaldeh.github.io/reading-notes/)