## **React and Forms.**
### **React Docs - Forms**
- ### *What is a ‘Controlled Component’?*
### In HTML, form elements such as **&lt;input&gt;**, **&lt;textarea&gt;**, and **&lt;select&gt;** typically maintain their own state and update it based on user input. In React, mutable state is typically kept in the state property of components, and only updated with setState(). We can combine the two by making the React state be the “single source of truth”. Then the React component that renders a form also controls what happens in that form on subsequent user input. An input form element whose value is controlled by React in this way is called a “controlled component”. [source](https://reactjs.org/docs/forms.html)
<>
- ### *Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.*
### I did not get it very well, I suppose to updating the state with the responses as soon as they enter them. Since handleChange runs on every keystroke to update the React state, the displayed value will update as the user types.
<>
- ### *How do we target what the user is entering if we have an event handler on an input field?*
### When we need to handle multiple controlled input elements, you can add a name attribute to each element and let the handler function choose what to do based on the value of event.target.name.
<>
### **The Conditional (Ternary) Operator Explained.**
- ### Why would we use a ternary operator?
### Use the ternary operator to simplify your if-else statements that are used to assign values to variables. The ternary operator is commonly used when assigning post data or validating forms.
<>
- ### Rewrite the following statement using a ternary statement:
### if(x===y){ console.log(true); } else { console.log(false); }

### x===y?console.log(true):console.log(false);