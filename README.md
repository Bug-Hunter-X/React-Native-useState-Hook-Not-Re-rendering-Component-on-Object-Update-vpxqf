# React Native useState Hook Not Re-rendering Component on Object Update

This repository demonstrates a common issue in React Native where the `useState` hook doesn't trigger a re-render when an object or array in the state is updated, even though the value has changed.  The problem stems from React's shallow comparison of state values; if the object reference remains the same, React might not detect the change. 

The `bug.js` file contains the problematic code, showcasing this unexpected behavior.  The solution, demonstrated in `bugSolution.js`, explains and implements a fix using the `useMemo` hook or immutable state update techniques to ensure that React detects the state change and triggers a re-render.