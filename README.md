# React 19 useEffect Bug

This repository demonstrates a potential issue where a `useEffect` hook in React 19 might run on every render, even with an empty dependency array.  This is unexpected behavior and can lead to performance problems.

## Bug Description

The `useEffect` hook with an empty dependency array should only run once after the initial render.  However, in some cases with React 19, this might not be the case.

## Reproduction Steps

1. Clone this repository.
2. Install dependencies: `npm install`
3. Run the app: `npm start`
4. Observe the console logs. You'll see that the effect runs more frequently than expected.

## Solution

The provided solution ensures that the `useEffect` hook behaves as expected, running only once after the initial render.