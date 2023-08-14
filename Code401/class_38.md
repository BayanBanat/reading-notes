# Class 38
## React 2
**Reading Questions :**

## Lifting State Up

Lifting state up is a fundamental concept in React that involves moving state from a child component to its parent component. This approach simplifies data flow and offers several benefits:

- **Single Source of Truth:** Centralizing state management in a higher-level component establishes a single source of truth for shared data.
- **Easier Data Flow:** Passing state as props from parent to child components enhances data flow clarity and understandability.
- **Separation of Concerns:** Lifting state up separates UI rendering from data management, promoting better code organization.
- **Simpler Updates:** Centralized state management minimizes state inconsistencies and potential bugs.
- **Reusability:** Components become more reusable across different parts of the application.

## Conditional Rendering in React

Conditional rendering in React enables dynamic content display based on conditions. Here's an example of how to implement conditional rendering:

```jsx
import React from 'react';

function Greeting({ isLoggedIn }) {
  if (isLoggedIn) {
    return <h1>Welcome back!</h1>;
  } else {
    return <h1>Please log in.</h1>;
  }
}

function App() {
  const isLoggedIn = true; // or false
  return (
    <div>
      <Greeting isLoggedIn={isLoggedIn} />
    </div>
  );
}

export default App;
```
# Principles Behind "Thinking in React"

"Thinking in React" is a strategic approach to designing React applications. The key principles include:

- **Break UI Into Components:** Divide the UI into smaller, reusable components to enhance modularity.
- **Single Responsibility Principle:** Each component should serve a single purpose for better maintainability.
- **Data Flow Through Props:** Use props to pass data from parent to child components, ensuring predictable data flow.
- **Manage State at the Right Level:** Lift state up to the appropriate level in the hierarchy to manage data consistently.
- **Top-Down Design:** Design your app starting from top-level components to establish structure and flow.
- **Reuse and Composition:** Reuse existing components and compose them for a scalable architecture.
- **Think in JSX:** Visualize UI structure based on data and express it using JSX.


## Things I want to know more about

