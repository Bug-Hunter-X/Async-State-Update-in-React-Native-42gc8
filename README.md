# Async State Update in React Native

This repository demonstrates a common issue in React Native related to asynchronous state updates. The problem arises when attempting to log or use the updated state value immediately after calling `setState` or a similar state update function.  The `console.log` statement often shows the *previous* value of the state instead of the newly updated value because the update is performed asynchronously.

The provided code examples showcase the bug and a solution that uses the `useEffect` hook to ensure the updated state is accessed correctly.