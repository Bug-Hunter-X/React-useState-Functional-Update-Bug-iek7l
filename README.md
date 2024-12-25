# React useState Functional Update Bug

This repository demonstrates a common bug in React applications involving the incorrect usage of functional updates within the `useState` hook.  The bug arises from not properly using the previous state value within the update function, leading to unexpected behavior and potential inconsistencies in application state.

## Bug Description

The `bug.js` file shows an example where the `incrementCount` function attempts to directly update the `count` state with `count + 1`. This approach creates a stale closure problem where the component doesn't react to state changes correctly. 

The solution demonstrates proper use of functional updates, ensuring the component reacts correctly to the updated state.

## How to Reproduce

1. Clone this repository.
2. Navigate to the project directory.
3. Run `npm install` to install dependencies.
4. Run `npm start` to start the development server.
5. Observe the incorrect increment behavior in the `bug.js` example and the corrected behavior in the `bugSolution.js` example.
