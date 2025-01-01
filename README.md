# React useEffect Infinite Loop Bug

This repository demonstrates a common bug in React applications where an infinite loop is caused by the `useEffect` hook.

## Bug Description

The `useEffect` hook is used to perform side effects in functional components. However, if the dependency array is not used correctly, it can lead to infinite loops. In this case, the count is always changing, causing the useEffect to run constantly and update the count again, creating an infinite loop. 

## How to Reproduce

1. Clone this repository.
2. Run `npm install` to install the dependencies.
3. Run `npm start` to start the development server.
4. Observe the console, it will be filled with errors and warnings.

## Solution

The solution involves correctly specifying the dependency array for useEffect to prevent the infinite loop.