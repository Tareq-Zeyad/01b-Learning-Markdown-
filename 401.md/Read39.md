# React III


# Next.js

### Assets

### Assets in Next.js

> Next.js can serve static assets, like images, under the top-level public directory. Files inside public can be referenced from the root of the application similar to pages.


### Example of unoptimized image/asset:

With regular HTML, you would add your profile picture as follows:

```html
<img src="/images/profile.jpg" alt="Your Name" />
```

However, this means you have to manually handle:

* Ensuring your image is responsive on different screen sizes
* Optimizing your images with a third-party tool or library
* Only loading images when they enter the viewport




### Metadata

### How can we modify the metadata of the page, such as the title HTML tag?

title is part of the head HTML tag, so let's dive into how we can modify the head tag in a Next.js page.

Open pages/index.js in your editor and find the following lines:

```jsx
<Head>
  <title>Create Next App</title>
  <link rel="icon" href="/favicon.ico" />
</Head>
```

Notice that Head is used instead of the lowercase head. Head is a React Component that is built into Next.js. It allows you to modify the head of a page.

You can import the Head component from the next/head module.

### CSS Styling

> Styled JSX is a CSS-in-JS library that allows you to write encapsulated and scoped CSS to style your components. The styles you introduce for one component won't affect other components, allowing you to add, change and delete styles without worrying about unintended side effects.

### is Styled JSX included by default in next.js?

> Yes, it is.

### Example:

Adding global styles
Most projects need some global styles to style the body element or provide css resets. Styled JSX allows us to add global styles using <style jsx global>. For example:

```jsx
// pages/index.js
function Home() {
  return (
    <div className="container">
      <h1>Hello Next.js</h1>
      <p>Let's explore different ways to style Next.js apps</p>
      <style jsx>{`
        .container {
          margin: 50px;
        }
        p {
          color: blue;
        }
      `}</style>
      <style jsx global>{`
        p {
          font-size: 20px;
        }
      `}</style>
    </div>
  )
}

export default Home
```

# React Context

### What is React context?
React context allows us to pass down and use (consume) data in whatever component we need in our React app without using props.

### When should you use React context?
React context is great when you are passing data that can be used in any component in your application.

### What problems does React context solve?

React context helps us avoid the problem of props drilling.

Props drilling is a term to describe when you pass props down multiple levels to a nested component, through components that don't need it.

### How do I use React context?
Context is an API that is built into React, starting from React version 16.

This means that we can create and use context directly by importing React in any React project.

There are four steps to using React context:

Create context using the createContext method.
Take your created context and wrap the context provider around your component tree.
Put any value you like on your context provider using the value prop.
Read that value within any component by using the context consumer.

### Does React context replace Redux?
Yes and no.

For many React beginners, Redux is a way of more easily passing around data. This is because Redux comes with React context itself.

