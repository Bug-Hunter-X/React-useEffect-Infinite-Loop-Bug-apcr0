# React useEffect Infinite Loop Bug

This repository demonstrates a common React bug: an infinite loop caused by a missing dependency array in the `useEffect` hook.

## Bug Description

The `useEffect` hook in `bug.js` is missing a dependency array.  This means it runs after every render, causing the `setCount` function to be called repeatedly and resulting in an infinite loop of re-renders.

## Solution

The solution (`bugSolution.js`) shows how to correctly specify the `count` state variable as a dependency in the `useEffect` hook. This ensures that the effect only runs when the `count` variable changes.