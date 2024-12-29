# React useEffect Infinite Loop Bug

This repository demonstrates a common bug in React applications involving the `useEffect` hook. The bug causes an infinite loop due to improper use of the dependencies array in `useEffect`.

## Bug Description

The `bug.js` file contains a component that uses `useEffect` to update a state variable (`count`) without specifying any dependencies. This leads to an infinite loop because the effect runs after every render, causing the state to constantly change and trigger another render.

## Solution

The `bugSolution.js` file provides a corrected version of the component. It includes `count` in the dependency array, ensuring that the effect only runs when the `count` value changes. This resolves the infinite loop and prevents excessive re-renders.

## How to Reproduce

1. Clone the repository.
2. Navigate to the directory in your terminal.
3. Run `npm install` to install dependencies.
4. Run `npm start` to start the development server.
5. Observe the error in the console and the infinite loop in the browser.
6. Open the `bugSolution.js` file to see how the bug is fixed.