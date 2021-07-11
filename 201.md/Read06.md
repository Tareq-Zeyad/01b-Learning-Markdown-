## **Problem Domain, Objects, and the DOM**.

### As myself a beginner into programming there are a  lot of difficulties I face during code such as:
### - Learning a new technology
### - Naming things
### - Testing your code
### - Fixing bugs
### - Making software maintainable
### - To predict the behaviour of the code before running it.

## *So  basically what problem domain is the procedure that a software follows to solve a problem, so in cases a one problem can be solved a various ways of codes like I can use for loop, maybe someone else will do it manually, I want to use If statements, others will use Switch. So it is all about the best practical solution & in order to do it a software enginner must a do planning very well to describe all problem possibilites to convert it into script coding.*

## **Ch. 3 Object Literals**.

### A JavaScript object literal is a comma-separated list of name-value pairs wrapped in curly braces. Object literals contain data, enclosing it in a tidy package. This minimizes the use of global variables which can cause problems when combining code. Literal notation is the easiest and most popular way to create objects. Here’s an example code as taken from the text. This code starts by creating an object using literal notation.

![object](https://image.slidesharecdn.com/javascript-110725163050-phpapp01/95/javascript-literacy-3-728.jpg?cb=1311612096)

## **Ch. 5 Document Object Model**.
### *Document Object Model specifies how a browsers should create a model of the HTML page and how javscript can access and update its content. The DOM cover two major areas:*
- ### Making the model of the HTML page.
- ### Accessing and changing the HTML page.

### A browser takes a snapshot of a webpage’s DOM and stores it in it’s memory. This is called a DOM tree. This is what it looks like (like an org chart):
![tree](https://res.cloudinary.com/practicaldev/image/fetch/s--B2Ts1hyb--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/http://i67.tinypic.com/2nqegt2.jpg)

### **The DOM tree has four types of nodes:**
- ### The document node - repersenting the entire page with every element on it.
- ### The elements node - To access the DOM tree yo start by looking for element. When they are found you can acces its text and attribute node.
- ### The attribute node - You can acces the attribute node to change css values.
- ### Text node - Once you have access to the element node you can access the text nodes.