# Unhandled Promise Rejection in Node.js Asynchronous Code
This repository demonstrates a common error in Node.js asynchronous programming: unhandled promise rejections.  The `bug.js` file contains code that simulates an asynchronous operation which may throw an error.  The `bugSolution.js` file shows how to properly handle this error using async/await and try...catch.

## Problem
Asynchronous operations are essential in Node.js, but errors within them aren't always handled properly.  If a promise rejects without a `.catch()` handler, Node.js will emit a warning to the console (or potentially crash in stricter environments) and your application might behave unpredictably. 

## Solution
The solution involves using async/await and try...catch.  This approach makes error handling clearer and easier to read.