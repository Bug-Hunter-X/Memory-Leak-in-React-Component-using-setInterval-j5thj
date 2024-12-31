# React setInterval Memory Leak

This repository demonstrates a common mistake in React applications: using `setInterval` within a `useEffect` hook without proper cleanup. This leads to memory leaks and unexpected behavior.

## Bug
The `bug.js` file contains a React component that uses `setInterval` to update a count every second. However, it lacks the necessary cleanup function to stop the interval when the component unmounts.

## Solution
The `bugSolution.js` file demonstrates the correct way to use `setInterval` within `useEffect`. It includes a cleanup function that uses `clearInterval` to stop the interval when the component unmounts, preventing memory leaks.

## How to Reproduce
1. Clone the repository.
2. Navigate to the directory.
3. Run `npm install` to install dependencies.
4. Run `npm start` to start the development server.
5. Observe the behavior of the component in both files.