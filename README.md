# Intermittent 500 Error in Node.js Server

This repository demonstrates a common issue in Node.js applications where asynchronous operations are not handled properly, leading to intermittent 500 errors.  The `bug.js` file shows the problematic code, while `bugSolution.js` provides a corrected version with robust error handling.

## Problem
The server simulates an asynchronous task that randomly succeeds or fails. If it fails, a 500 error is sent to the client without any mechanism for graceful handling or logging. This makes debugging and user experience unreliable.

## Solution
The solution uses try...catch blocks to handle potential errors during the asynchronous operation.  Proper logging is added to facilitate debugging, and a more informative error message is sent to the client, if needed.