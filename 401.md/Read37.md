# React I



# ES6 Syntax

### What is ES6?

- ES6 Refers to version 6 of the ECMA Script programming language. It is a major enhancement to the JavaScript language, and adds many more features intended to make large-scale software development easier.

### Some Examples of ES6 Pracices:

> Declaring variables in js:
```js
// normal variable
let x = 0

// constant variable
const CONST_IDENTIFIER = 0
```

> Arrow functions
```js
let func = (a) => {} // parentheses optional with one parameter
let func = (a, b, c) => {} // parentheses required with multiple parameters
```

> Template literals
```js
let str = `Release Date: ${date}`
```

> Implicit returns
```js
let func = (a, b, c) => a + b + c // curly brackets must be omitted
```

> Key/property shorthand
```js
let obj = {
  a,
  b,
}
```

- For full ES6  [here](https://www.taniarascia.com/es6-syntax-and-feature-overview/#multi-line-strings)

### How to render Hello World with React?

```js
ReactDOM.render(
  <h1>Hello, world!</h1>,
  document.getElementById('root')
);
```

### What is JSX?

- It is a syntax extension to JavaScript. We recommend using it with React to describe what the UI should look like.

### Why JSX?

Instead of artificially separating technologies by putting markup and logic in separate files, React separates concerns with loosely coupled units called “components” that contain both. We will come back to components in a further section, but if you’re not yet comfortable putting markup in JS, this talk might convince you otherwise.

React doesn’t require using JSX, but most people find it helpful as a visual aid when working with UI inside the JavaScript code. It also allows React to show more useful error and warning messages.

### Example of JSX:

```js
function formatName(user) {
  return user.firstName + ' ' + user.lastName;
}

const user = {
  firstName: 'Harper',
  lastName: 'Perez'
};

const element = (
  <h1>
    Hello, {formatName(user)}!
  </h1>
);

ReactDOM.render(
  element,
  document.getElementById('root')
);
```

### What are react components and what do they do?

- Components let you split the UI into independent, reusable pieces, and think about each piece in isolation. This page provides an introduction to the idea of components. 

### What are the two types of components in react?

1. function based components.
```js
function Welcome(props) {
  return <h1>Hello, {props.name}</h1>;
}
```

2. class based components.
```js
class Welcome extends React.Component {
  render() {
    return <h1>Hello, {this.props.name}</h1>;
  }
}
```

### What are states in React?

- State is a plain JavaScript object used by React to represent an information about the component's current situation. It's managed in the component (just like any variable declared in a function).

### Example of handling events in React:

```js
class Toggle extends React.Component {
  constructor(props) {
    super(props);
    this.state = {isToggleOn: true};

    // This binding is necessary to make `this` work in the callback
    this.handleClick = this.handleClick.bind(this);
  }

  handleClick() {
    this.setState(prevState => ({
      isToggleOn: !prevState.isToggleOn
    }));
  }

  render() {
    return (
      <button onClick={this.handleClick}>
        {this.state.isToggleOn ? 'ON' : 'OFF'}
      </button>
    );
  }
}

ReactDOM.render(
  <Toggle />,
  document.getElementById('root')
);
```

### What is tailwind?

- Tailwind CSS is basically a utility-first CSS framework for rapidly building custom user interfaces. It is a highly customizable, low-level CSS framework that gives you all of the building blocks you need to build bespoke designs without any annoying opinionated styles you have to fight to override.

### What is Next.js?

- Next.js is an open-source development framework built on top of Node.js enabling React based web applications functionalities such as server-side rendering and generating static websites.

