# React useEffect Hook Missing Dependency

This repository demonstrates a common error in React applications involving the `useEffect` hook: a missing dependency in the dependency array. This can lead to unexpected behavior and difficult-to-debug issues. 

## The Bug

The `bug.js` file contains a component that uses `useEffect` to update a counter every second. However, the dependency array is empty (`[]`), meaning the effect only runs once after the component mounts.  Subsequent changes to the `count` state variable will not trigger the effect, resulting in the counter not updating correctly.

## The Solution

The `bugSolution.js` file provides a corrected version of the component. By adding `count` to the dependency array, the effect will now run whenever the `count` value changes, ensuring the counter updates correctly.

## How to Reproduce

1. Clone this repository.
2. Run `npm install` to install the necessary packages.
3. Run `npm start` to start the development server.
4. Observe the incorrect behavior in the original component and the correct behavior in the corrected version.
