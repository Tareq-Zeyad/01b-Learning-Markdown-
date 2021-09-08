## **In memory storage.**
## **Understanding the JavaScript Call Stack.**
<br>

- ### *What is a ‘call’?.*
### The call stack is single, function(s) execution, is done, one at a time, from top to bottom. It means the call stack is synchronous.
<br>

- ### *How many ‘calls’ can happen at once?*
### It is single-threaded. Meaning it can only do one thing at a time.

<br>

- ### *What does LIFO mean?*
### Data structure principle of Last In, First Out, it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.

<br>

- ### *Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.*
### function sum (a, b) { ` return a + b; } function avg(a, b) { return sum (a, b) / 2; } let average = avg(10, 20);

<br>

- ### *What causes a Stack Overflow?*
### A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point.

<br>

## **JavaScript error messages.**
<br>

- ### *What is a ‘refrence error’?*
### This is as simple as when you try to use a variable that is not yet declared so you get this type of errors. 
<br>

- ### *What is a ‘syntax error’?*
### this occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse. Or miss write a keyword.
<br>

- ### *What is a ‘range error’?*
### When manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up.
<br>

- ### *What is a ‘tyep error’?*
### this types of errors show up when the types (number, string, boolean and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable
<br>

- ### *What is a breakpoint?*
### The breakpoint can also be achieved by putting a debugger statement in your code in the line you want to break.
<br>

- ### *What does the word ‘debugger’ do in your code?*
### Debuggers allow users to halt the execution of the program, examine the values of variables, step execution of the program line by line, and set breakpoints on lines or specific functions
<br>


