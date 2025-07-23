
# Introduction to React.js

## Version History

| Author      | Created on | Version   | Last updated by | Internal Reviewer |
|-------------|------------|-----------|------------------|--------------------|
| Anuj Jain   | 17-07-25   | version 1 | N/A              | Prashant           |

---

##  Table of Contents

1. [What is React?](#1-what-is-react)
2. [Why Use React?](#2-why-use-react)
3. [React vs Traditional JS](#3-react-vs-traditional-js)
4. [Setting Up a React App](#4-setting-up-a-react-app)
5. [JSX – JavaScript XML](#5-jsx--javascript-xml)
6. [Components in React](#6-components-in-react)
7. [Props and State](#7-props-and-state)
8. [Handling Events](#8-handling-events)
9. [React Hooks (useState, useEffect)](#9-react-hooks-usestate-useeffect)
10. [Folder Structure Explanation](#10-folder-structure-explanation)
11. [Conclusion](#11-conclusion)

---

## 1. What is React?

React is a **JavaScript library** for building **user interfaces**, especially single-page applications where fast interaction is important.
It is maintained by **Meta (Facebook)** and has a large community.

>  Think of React as a LEGO game. You build UI using small reusable pieces (components).

---

## 2. Why Use React?

* **Component-Based**: Reusable blocks of code.
* **Virtual DOM**: Faster updates to the UI.
* **One-Way Data Binding**: More predictable behavior.
* **Large Ecosystem**: Tons of support libraries.

---

## 3. React vs Traditional JS

| Feature          | Traditional JS (Vanilla) | React                   |
| ---------------- | ------------------------ | ----------------------- |
| UI Updates       | Manual DOM manipulation  | Virtual DOM             |
| Code Reusability | Hard                     | Component-based         |
| Performance      | Slower                   | Faster with Virtual DOM |
| Learning Curve   | Easy                     | Moderate                |

---

## 4. Setting Up a React App

**Step 1**: Install Node.js
[https://nodejs.org/](https://nodejs.org/)

**Step 2**: Install create-react-app

```bash
npm install -g create-react-app
```

**Step 3**: Create a new project

```bash
npx create-react-app my-first-app
cd my-first-app
npm start
```

 You’ll now see your app at: `http://localhost:3000`

---

## 5. JSX – JavaScript XML

JSX allows writing HTML inside JavaScript:

```jsx
const element = <h1>Hello, world!</h1>;
```

> JSX makes your code more readable and closer to HTML. Under the hood, it becomes `React.createElement()`.

**Important Rules:**

* Only return one parent element
* Use `className` instead of `class`
* Use `{}` to embed JS in JSX

---

## 6. Components in React

There are **two types**:

1. **Functional Components**
2. **Class Components** (older)

### Example: Functional Component

```jsx
function Greet() {
  return <h2>Hello, Anuj!</h2>;
}
```

**Usage:**

```jsx
<Greet />
```

---

## 7. Props and State

### Props (Short for Properties)

* Used to pass data **from parent to child**
* Read-only

```jsx
function Welcome(props) {
  return <h1>Hello, {props.name}</h1>;
}
```

**Usage:**

```jsx
<Welcome name="Anuj" />
```

---

### State

* Managed **within the component**
* Can be changed (mutable)

```jsx
import { useState } from 'react';

function Counter() {
  const [count, setCount] = useState(0);
  return (
    <div>
      <p>You clicked {count} times</p>
      <button onClick={() => setCount(count + 1)}>Click Me</button>
    </div>
  );
}
```

---

## 8. Handling Events

React handles events like JS but with camelCase and JSX.

```jsx
<button onClick={handleClick}>Click Me</button>
```

```js
function handleClick() {
  alert("Button clicked!");
}
```

---

## 9. React Hooks (useState, useEffect)

### useState

To maintain state in functional components.

```jsx
const [value, setValue] = useState(0);
```

### useEffect

To run side-effects (e.g., API call, timer, DOM update).

```jsx
useEffect(() => {
  console.log("Component mounted!");
}, []);
```

---

## 10. Folder Structure Explanation

When you create a React app using `create-react-app`, you get:

```
my-first-app/
├── public/
│   └── index.html   --> Single HTML file
├── src/
│   ├── App.js       --> Root component
│   ├── index.js     --> ReactDOM.render() here
│   └── ...your files
├── package.json     --> Project config & dependencies
```

---

## 11. Conclusion

React helps you build **modular, scalable, and fast** UIs with ease.
It may seem tricky at first, but once you understand **components, props, and state**, the rest is just practice!

---

## Contact Information

| Name      | Email Address                                               |
| --------- | ----------------------------------------------------------- |
| Anuj Jain | [anuj.jain@mygurukulam.co](mailto:anuj.jain@mygurukulam.co) |

---


##  Bonus Resources

* React Official Docs: [https://reactjs.org](https://reactjs.org)
* JSX Docs: [https://reactjs.org/docs/introducing-jsx.html](https://reactjs.org/docs/introducing-jsx.html)
* Create React App Guide: [https://create-react-app.dev](https://create-react-app.dev)

---

