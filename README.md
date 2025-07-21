
# React Documentation

---

## Version History

| Author      | Created on | Version   | Last updated by | Internal Reviewer |
|-------------|------------|-----------|------------------|--------------------|
| Anuj Jain   | 17-07-25   | version 1 | N/A              | Prashnat           |

---


## Table of Contents

1. [What is React?](#what-is-react)
2. [Why Use React?](#why-use-react)
3. [Key Features of React](#key-features-of-react)
4. [Setting Up React](#setting-up-react)
5. [JSX: JavaScript + XML](#jsx)
6. [React Components](#react-components)
7. [Props and State](#props-and-state)
8. [Lifecycle Methods](#lifecycle-methods)
9. [React Developer Tools](#react-developer-tools)
10. [References](#references)

---

## What is React?

**React** is a JavaScript library developed by **Meta (Facebook)** for building user interfaces, especially single-page applications. It allows developers to create reusable UI components.

---

## Why Use React?

* Declarative and component-based
* Fast and efficient rendering using Virtual DOM
* Strong community and ecosystem
* Reusable components promote DRY (Don't Repeat Yourself) principles

---

## Key Features of React

* **Virtual DOM:** Optimizes rendering performance
* **JSX:** Syntax extension for mixing HTML with JavaScript
* **Component-Based:** UI is built using independent components
* **One-Way Data Binding:** Data flows in one direction, improving predictability

---

## Setting Up React

You can set up React using various methods:

### 1. Using CDN (For quick prototyping)

```html
<script src="https://unpkg.com/react@18/umd/react.development.js"></script>
<script src="https://unpkg.com/react-dom@18/umd/react-dom.development.js"></script>
```

### 2. Using `create-react-app` (For full project setup)

```bash
npx create-react-app my-app
cd my-app
npm start
```

---

## JSX

JSX stands for **JavaScript XML**. It allows writing HTML-like code inside JavaScript.

```jsx
const element = <h1>Hello, React!</h1>;
```

JSX is transpiled to `React.createElement()` behind the scenes.

---

## React Components

React apps are built using components.

### Function Component

```jsx
function Welcome() {
  return <h1>Hello, World!</h1>;
}
```

### Class Component

```jsx
class Welcome extends React.Component {
  render() {
    return <h1>Hello, World!</h1>;
  }
}
```

---

## Props and State

* **Props:** Short for “properties” – used to pass data from parent to child.

```jsx
function Greeting(props) {
  return <h1>Hello, {props.name}</h1>;
}
```

* **State:** Data maintained within the component.

```jsx
const [count, setCount] = useState(0);
```

---

## Lifecycle Methods

Used in class components to run code at specific points in a component’s life:

| Method                 | Purpose                           |
| ---------------------- | --------------------------------- |
| `componentDidMount`    | Called after the component mounts |
| `componentDidUpdate`   | Called after updates              |
| `componentWillUnmount` | Called before removal             |

In function components, `useEffect()` hook is used.

---

## React Developer Tools

React DevTools is a browser extension that allows:

* Inspecting component hierarchy
* Viewing state and props
* Debugging performance

Install from: [React Developer Tools - Chrome](https://chrome.google.com/webstore/detail/react-developer-tools)

---

## Contact Information

| Name      | Email Address                                               |
| --------- | ----------------------------------------------------------- |
| Anuj Jain | [anuj.jain@mygurukulam.co](mailto:anuj.jain@mygurukulam.co) |

---


## References

* **Official Website:** [https://react.dev](https://react.dev)
* **React GitHub Repo:** [https://github.com/facebook/react](https://github.com/facebook/react)
* **JSX Docs:** [https://react.dev/learn/writing-markup-with-jsx](https://react.dev/learn/writing-markup-with-jsx)
* **create-react-app Guide:** [https://create-react-app.dev/docs/getting-started/](https://create-react-app.dev/docs/getting-started/)
* **React Hooks:** [https://react.dev/learn/state-a-component](https://react.dev/learn/state-a-component)

---

