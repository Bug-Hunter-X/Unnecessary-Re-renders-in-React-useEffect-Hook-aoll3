# Unnecessary Re-renders in React useEffect Hook

This example demonstrates an inefficient use of the `useEffect` hook in React. The effect runs after every render, leading to unnecessary re-renders and console logs.  This can impact performance, especially with complex components.

**The Problem:** The `useEffect` hook is called after every render.  A more efficient approach is to specify dependencies, ensuring the effect runs only when those dependencies change.

**Solution:** Add an array as the second argument to `useEffect` to specify dependencies.  In this case, only when the `count` changes will the useEffect run.