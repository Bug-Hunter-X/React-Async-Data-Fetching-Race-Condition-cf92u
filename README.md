# React Async Data Fetching Race Condition

This repository demonstrates a common bug in React applications involving asynchronous data fetching and race conditions.  The `bug.js` file contains a component with a flawed implementation that can lead to stale data being rendered when the data fetching function is called multiple times in quick succession.

The solution, provided in `bugSolution.js`, addresses this issue using techniques such as promises and state management to ensure that only the most recent data update is applied.

## How to Reproduce

1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `npm start` to start the development server.
4. Observe the behavior of the component, particularly when rapidly triggering data refetches (e.g., by clicking a button that calls `fetchData` repeatedly).