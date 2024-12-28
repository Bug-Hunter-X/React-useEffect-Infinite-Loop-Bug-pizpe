# React useEffect Infinite Loop Bug

This repository demonstrates a common React bug: an infinite loop caused by improperly using the `useEffect` hook. The `bug.js` file contains the buggy code.  The `bugSolution.js` file provides a corrected version.

## Bug Description
The `useEffect` hook in `bug.js` attempts to update the state variable `count` within the dependency array. This creates an infinite loop because every render causes the `useEffect` to run again, leading to continuous state updates. 

## Solution
The `bugSolution.js` file demonstrates the correct way to use `useEffect` in this scenario.  The dependency array is modified to avoid infinite loops.