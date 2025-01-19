# React Native FlatList TypeError: Cannot read properties of null (reading 'name')

This repository demonstrates a common error in React Native when using `FlatList` to render data containing `null` or `undefined` values.  The error, `TypeError: Cannot read properties of null (reading 'name')`, arises when attempting to access a property of an object that is `null` or `undefined` within the `renderItem` function.

The `bug.js` file shows the problematic code, and `bugSolution.js` provides the solution.

## Solution:

The solution involves using optional chaining (`?.`) or nullish coalescing (`??`) operators to gracefully handle `null` or `undefined` values.  This prevents the error by safely accessing the property only if it exists.