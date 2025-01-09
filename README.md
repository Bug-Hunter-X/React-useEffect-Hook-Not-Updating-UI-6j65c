# React useEffect Hook Not Updating UI

This repository demonstrates a common issue with the React `useEffect` hook where the UI doesn't update even though the state has changed. The problem arises from an incorrect understanding of how dependencies work within the `useEffect` hook.  The solution highlights the importance of including all state variables used within the effect in the dependency array.

## Bug
The `bug.js` file shows a simple counter component where the `useEffect` hook is intended to log the current count to the console and update the UI accordingly. However, the UI doesn't reflect the changes in the `count` state. 

## Solution
The `bugSolution.js` file presents the corrected code. The key change is adding `count` to the dependency array of the `useEffect` hook.  By doing this, the effect re-runs whenever the `count` state changes, ensuring that the UI correctly reflects these changes. 
