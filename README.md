# DevStack.
## React Questions and Answers

### 1. What is JSX, and why is it used in React?

JSX is a syntax that lets us write HTML-like code inside JavaScript. React uses JSX to make it easier to describe what the user interface should look like.

### 2. What is the difference between props and state?

**Props** are data passed from a parent component to a child component. **State** is data managed inside a component that can change over time.

### 3. What does the `useState` hook do, and where did you use it in this project?

`useState` lets a React component store and update data. In this project, I used it to manage the application data, such as the stack/items and their current state.

### 4. What does the `useEffect` hook do, and why did you need it to load the JSON data?

`useEffect` runs code when something in a component changes or when the component loads. I used it to load the JSON data when the project starts.

### 5. Why does every item in a `.map()` list need a unique `key` prop?

The `key` helps React identify each item in a list. This allows React to update the list efficiently when items are added, removed, or changed.

### 6. What is conditional rendering? Show one place you used it.

Conditional rendering means showing different content depending on a condition. For example, I used it to show an empty stack message when there are no items:

```jsx
{stack.length === 0 && <p>The stack is empty.</p>}
```

### 7. How do you pass data from a parent component to a child component, and how does a child send something back to the parent?

A parent passes data to a child using **props**. To send something back, the parent can pass a function as a prop, and the child can call that function with the required data.
