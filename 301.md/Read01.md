## **Introduction to React and Components.**
### ***Component Based Architecture.***
### A set of frameworks such as COM/DCOM, JavaBean, EJB, CORBA, .NET, web services, and grid services. Which are mainly focused on the decomposition of the design into individual functional or logical components that represent well-defined communication interfaces.
![components](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2020/09/component-based-architecture.jpg)
<>
### ***What is a component?***
### Imagine a single building block of a wall, then a  software component can be defined as a unit of composition with a contractually specified interface and explicit context dependencies only. That is, a software component can be deployed independently and is subject to composition by third parties. In other words a component is a group of related functionality that resides behind a nice and clean interface.
<>
### ***What are the charactistics of a component?***
- ### **Reusability**: Components are usually designed to be reused in different situations in different applications.
- ### **Replaceable**: Means that components can take each other places.
- ### **Not context specific**: It can operates in different environments.
- ### **Extensible**: Also it can be extended to contain a new behaviour.
- ### **Encapsulated**: I think it means more safe operations that so the component does not expose details of the internal processes or any internal variables or state.
- ### **Independent**: Components are designed to have minimal dependencies on other components.
<>
### ***What are the advantages of using component based architecture?***
### The three main advantages are:
- ### **More Control and Lower Maintenance Costs**: Components enable to focus on specific pieces of code. Because code is in one place, developers have more control over it. And, every time there’s an update or a fix, every implementation of their code will be updated and bug-free.
- ### **Faster Development to Save Time and Increase Revenue**:Because of the reusability aspect, a component-based architecture reduces the number of developers needed to quickly create amazing apps, freeing your team to focus on more impactful business requirements. Logic components are context-free and front-end components already have great UX and UI.
![skills](https://www.outsystems.com/blog/-/media/images/blog/posts/component-architecture/component-architecture-02.png?h=299&w=512&updated=20201022122707)
- ### **Take Advantage of Specialized Skills**: With components developers can visit other developer communities and search their repositories for the component that suits their project well. It means that use of components allows more innovative & diverse coding skills to be shared among others.
<>
## **Props and How to Use it in React**
### Before we dive in Props lets Recall what is a component.
### **So a React Component is a set of blocks that defines & viewed to the user interface, imagine a lego blocks that is composed to shape an object. Eventually A component is an independent, reusable code block, which divides the UI into smaller pieces.**
![React](https://miro.medium.com/max/2400/1*y6C4nSvy2Woe0m7bWEn4BA.png)
<>
### **React is a library that used to pass data between components**
### ***What is props short for?***
### **Props** is a special keyword in React, which stands for properties and is being used for passing data from one component to another.
<>
### ***How are props used in React?***
- ### Firstly, define an attribute and its value(data).
- ### Then pass it to child component(s) by using Props.
- ### Finally, render the Props Data.
<>
![props vs state](https://i.stack.imgur.com/wqvF2.png)
### ***What is the flow of props?***
- ### **To Child From Parent**: The Parent passes the data to its child as a prop.
- ### **To Parent from Child**: Parents have state to hold the data and sends the child the setState function nested in another function. The child then passes the data to this function to update the state in the parent.




