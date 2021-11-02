## **Classes and Objects.**
### Objects are an encapsulation of variables and functions into a single entity. Objects get their variables and functions from classes. Classes are essentially a template to create your objects.
### Also, we can access class functions and methods in order to execute code inside them, and that is extremly useful in Object Oriented Programming, so how can we access an variable or a method inside a class/object ?
### To access an variable or a method inside a class, we simply use notation objName.Variable / objName.method().
<br>

## **Thinking Recursively.**
### A problem may have many wrong roots from a point where it grows initially until it become a tough error.
### **Thinking Recrusively essentionally breaking down problems into smaller chucks that are easier to solve.**
### On other hand the Recurion Technique show us the steps to investigate errors, Also If the current problem represents a simple case, solve it. If not, divide it into subproblems and apply the same strategy to them.
### **A recursive function is a function defined in terms of itself via self-referential expressions.**
<br>

## **Recursive Functions in Python**
### **All recursive functions share a common structure made up of two parts: base case and recursive case**
### **A recursive function will continue to call itself and repeat its behavior until some condition is met to return a result.**
- ### Decompose the original problem into simpler instances of the same problem. This is the recursive case:
### n! = n x (n−1) x (n−2) x (n−3) ⋅⋅⋅⋅ x 3 x 2 x 1
### n! = n x (n−1)!
- ### As the large problem is broken down into successively less complex ones, those subproblems must eventually become so simple that they can be solved without further subdivision.
### n! = n x (n−1)! 
### n! = n x (n−1) x (n−2)!
### n! = n x (n−1) x (n−2) x (n−3)!
### ⋅
### ⋅
### n! = n x (n−1) x (n−2) x (n−3) ⋅⋅⋅⋅ x 3!
### n! = n x (n−1) x (n−2) x (n−3) ⋅⋅⋅⋅ x 3 x 2!
### n! = n x (n−1) x (n−2) x (n−3) ⋅⋅⋅⋅ x 3 x 2 x 1!

![gif](https://files.realpython.com/media/stack.9c4ba62929cf.gif)

<br>

## **Maintaining State**
### When dealing with recursive functions, keep in mind that each recursive call has its own execution context, so to maintain state during recursion you have to either:

- ### Thread the state through each recursive call so that the current state is part of the current call’s execution context
- ### Keep the state in global scope
<br>

## **Recursive Data Structures in Python**
### **A data structure is recursive if it can be deﬁned in terms of a smaller version of itself.**