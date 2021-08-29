## **State and Props.**
### *React: Component Lifecycle Events.*
![React lifcycle](https://maksimivanov.com/static/23f4fad25265022b5672d95cadab1f88/bc3a8/lifecycle_methods.jpg)
### **Mounting, Updating, and Unmounting are the three phases of the component lifecycle.**
<>
- ### Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?

### The render as it in the render phase, may be paused, aborted or restarted by React.
<>
- ### What is the very first thing to happen in the lifecycle of React?
### Mounting: When an instance of a component is being created and inserted into the DOM it occurs during the mounting phase. 
<>
- ### Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates.
### the correct order is:
### 1- Constructor.
### 2- React Updates.
### 3- Render.
### 4- ComponentDidMount.
### 5- ComponentWillUnmount.
<>
- ### What does componentDidMount do?
### This method is invoked immediately after a component is mounted. If you need to load anything using a network request or initialize the DOM, it should go here. This method is a good place to set up any subscriptions. If you do that, don’t forget to unsubscribe in componentWillUnmount().
<>
## **React State Vs Props.**
![props vs state](https://static.wixstatic.com/media/3a60df_ecdf74102fd04ee0ab40c50ecee52020~mv2.png/v1/fit/w_800%2Ch_420%2Cal_c/file.png)
- ### What types of things can you pass in the props?
### The intiliazation of a component. Also let's say a Tile or Heading it can pass a sub title or sub heading to it.
<>
- ### What is the big difference between props and state?
### Props can pass data outside of a component whereas a satate will pass data inside of it.
<>
- ### When do we re-render our application?
### WHen a change is occured through a state.
<>
- ### What are some examples of things that we could store in state?
### To store data that will be updated based on user input (such as in Forms), as for rerender purpose also. 