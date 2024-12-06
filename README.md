# React useEffect Infinite Loop Bug
This repository demonstrates a common bug in React applications involving the `useEffect` hook.  The example shows an infinite loop caused by a missing dependency in the `useEffect`'s dependency array.

## Bug Description
The `useEffect` hook is designed to perform side effects after a component renders. However, if it's called without specifying the relevant dependencies, it will run after every render, potentially causing unexpected behavior (like an infinite loop in this case).

## How to Reproduce
1. Clone the repository.
2. Run `npm install` to install the dependencies.
3. Run `npm start` to start the development server.
4. Observe the console output and the infinite loop.

## Solution
The solution involves correctly specifying the `count` variable as a dependency in the `useEffect` hook's dependency array.