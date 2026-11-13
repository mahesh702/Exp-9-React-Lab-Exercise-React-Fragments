# Exp 9 – React Lab Exercise: React Fragments

## NAME:  Mahesh N
## REG NO: 2305001017

## Aim
To understand and implement React Fragments to group multiple JSX elements without creating unnecessary HTML elements in the DOM.

## Objectives
- Understand the concept of React Fragments.
- Use Fragment shorthand syntax.
- Use the explicit Fragment syntax.
- Group multiple JSX elements without an extra DOM node.
- Understand the difference between Fragments and div elements.

## Program

### Step 1: Create a React Project

```bash
npm create vite@latest react-fragments
cd react-fragments
npm install
npm run dev
```

Select React as the framework and JavaScript as the variant.

### Step 2: App.jsx – Using Fragment Shorthand

```jsx
function Student() {
  return (
    <>
      <h2>Student Details</h2>

      <h3>Name: Sukhmeet Kaur G</h3>

      <p>Register Number: 2305001032</p>

      <p>Department: Computer Science and Engineering</p>
    </>
  );
}

function App() {
  return (
    <>
      <h1>College Information System</h1>

      <Student />
    </>
  );
}

export default App;
```

### Step 3: Using Explicit Fragment Syntax

```jsx
import { Fragment } from "react";

function Student() {
  return (
    <Fragment>
      <h2>Student Details</h2>
      <p>Name: Sukhmeet Kaur G</p>
      <p>Department: CSE</p>
    </Fragment>
  );
}

function App() {
  return (
    <Fragment>
      <h1>College Information System</h1>
      <Student />
    </Fragment>
  );
}

export default App;
```

## Output

### Fragment Shorthand Syntax

<img width="942" height="365" alt="WhatsApp Image 2026-11-04 at 7 40 53 PM" src="https://github.com/user-attachments/assets/24c30ee6-81fa-44ee-8730-362f2398472e" />

### Explicit Fragment Syntax

<img width="947" height="302" alt="WhatsApp Image 2026-11-04 at 7 35 18 PM" src="https://github.com/user-attachments/assets/95c6bf60-8cf8-4990-89cd-46c5a9c41e3a" />

## Result

Thus, React Fragments were successfully implemented using shorthand and explicit syntax to group multiple JSX elements without creating unnecessary DOM elements.
