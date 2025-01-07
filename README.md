# Unhandled Async Error in Node.js HTTP Server

This repository demonstrates an example of an unhandled error in an asynchronous Node.js HTTP server and provides a solution for handling such errors gracefully.

## Bug

The `bug.js` file contains a simple HTTP server that simulates an asynchronous operation.  This operation might throw an error randomly.  If an error occurs, the server crashes without any indication of the error to the user.

## Solution

The `bugSolution.js` file demonstrates how to handle this asynchronous error using a `try...catch` block inside the asynchronous operation and using error event listener for the server.  This ensures that the server does not crash and allows for better error management.