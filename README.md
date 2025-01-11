# React 19 useEffect Hook Missing Dependency

This repository demonstrates a common error in React's `useEffect` hook and its solution.  The bug involves an infinite render loop caused by a missing dependency in the `useEffect` hook's dependency array.  The solution shows how to correctly add the dependency to resolve this problem. 

## Bug
The bug is in `bug.js`. The component renders infinitely because the `useEffect` hook is missing the `count` variable in its dependency array.  This causes the effect to run on every render, leading to an infinite loop. 

## Solution
The solution is provided in `bugSolution.js`. By adding `count` to the dependency array, `useEffect` now only runs when the value of `count` changes.  This prevents the infinite loop and ensures proper functionality.