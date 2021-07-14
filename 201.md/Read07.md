## **Domain Modeling**.
### Domain modeling is the process of creating a conceptual model for a specific problem. And a domain model that's articulated well can verify and validate your understanding of that problem.Here's some tips to follow when building your own domain models:
- ### When modeling a single entity that'll have many instances, build self-contained objects with the same attributes and behaviors.
- ### Model its attributes with a constructor function that defines and initializes properties.
- ### Model its behaviors with small methods that focus on doing one job well.
- ### Create instances using the new keyword followed by a call to a constructor function.
- ### Store the newly created object in a variable so you can access its properties and methods from outside.
- ### Use the this variable within methods so you can access the object's properties and methods from inside.

## **Ch. 6 Tables.**
### HTML tables allow web developers to arrange data into rows and columns.
### The **&lt;table&gt;** tag defines an HTML table. Each table row is defined with a **&lt;tr&gt;** tag. Each table header is defined with a **&lt;th&gt;** tag. Each table data/cell is defined with a **&lt;td&gt;** tag. By default, the text in **&lt;th&gt;** elements are bold and centered. By default, the text in **&lt;td&gt;** elements are regular and left-aligned.

![table](https://gocoding.org/wp-content/uploads/2020/06/HTML-Table-Syntax.png)

## **Ch. 3 Functions, Methods, and Objects**.
### In JavaScript a function is considered as an object.
- ### **Primitives (string, number, null, boolean, undefined, symbol)**: these are immutable data types. They are not objects, don’t have methods and they are stored in memory by value.
- ### **Non-Primitives (functions, arrays and objects):** these are mutable data types. They are objects and they are stored in memory by reference.

![methods](https://res.cloudinary.com/academind-gmbh/image/upload/f_auto,q_auto/c_fit,dpr_3.0,g_center,w_500/v1/academind.com/content/tutorials/javascript-functions-are-objects/functions-are-objects)

- ### JavaScript methods are actions that can be performed on objects. A JavaScript method is a property containing a function definition.

![methods](https://cf.ppt-online.org/files/slide/z/ZQB7W6CTo0jgKzhF5VLlfNdbm1HPD2exvrSG9q/slide-41.jpg)