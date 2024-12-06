# React Native: TypeError: Cannot read properties of undefined (reading '...')

This repository demonstrates a common React Native error: `TypeError: Cannot read properties of undefined (reading '...')`.  This error typically arises when attempting to access a property of an object that is currently undefined or null. This often happens when working with asynchronous data fetching where the component renders before the data has fully loaded.

## Bug Description
The bug showcases a scenario where a component attempts to render data from an API before the `fetch` request completes.  This leads to an error because the `userData` object is initially `null` and accessing its properties will cause the error.

## Solution
The provided solution uses optional chaining (`?.`) and nullish coalescing (`??`) operators to gracefully handle cases where `userData` might be null or undefined.

## How to reproduce the bug
1. Clone this repository.
2. Run `npm install`.
3. Run the app using a React Native emulator or device.
4. Observe the error in the console.