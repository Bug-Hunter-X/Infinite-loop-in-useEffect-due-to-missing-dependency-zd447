# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React's `useEffect` hook: an infinite loop caused by a missing dependency.

## Bug Description
The `useEffect` hook in `bug.js` has a missing dependency, causing it to re-render continuously. This leads to an infinite loop and potential performance issues.

## Bug Solution
The `bugSolution.js` file fixes the issue by including the `count` variable in the dependency array of `useEffect`. This ensures the effect runs only when the `count` value changes.

## How to Reproduce
1. Clone the repository.
2. Navigate to the repository in your terminal.
3. Run `npm install` to install dependencies.
4. Run `npm start` to start the development server.
5. Observe the continuous re-rendering in the browser's console.

## Solution
The solution lies in adding the `count` state variable as a dependency in the `useEffect` hook. This limits the effect's execution to only when the count changes.