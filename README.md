# React useEffect: Missing Dependency causing Unexpected Re-renders

This repository demonstrates a common issue encountered when using the `useEffect` hook in React: unexpected re-renders due to missing or incorrect dependencies in the dependency array.

## Bug Description:
The `useEffect` hook is used to perform side effects.  If a value used inside the `useEffect` isn't included in the dependency array, the effect will not re-run when that value changes, leading to stale closures and incorrect behavior. This specific example shows a counter that unintentionally re-renders more frequently than expected.