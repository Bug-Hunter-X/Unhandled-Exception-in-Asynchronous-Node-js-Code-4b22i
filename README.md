# Unhandled Exception in Asynchronous Node.js

This repository demonstrates a common error in Node.js applications: unhandled exceptions within asynchronous callbacks.  Improper handling of these exceptions can lead to application crashes and unexpected behavior.

The `bug.js` file contains code that simulates an asynchronous operation (using `setTimeout`) which may throw an error.  This error, if not properly handled, will crash the server.

The `bugSolution.js` file provides a corrected version with proper error handling, showcasing best practices for preventing such crashes.

## How to Reproduce the Bug

1. Clone this repository.
2. Navigate to the directory containing `bug.js`.
3. Run the application using `node bug.js`.
4. Refresh the page several times.  You will see it eventually crash when the random number is less than 0.5.

## How to Run the Solution

1. Navigate to the directory containing `bugSolution.js`.
2. Run the application using `node bugSolution.js`.
3. The server will now gracefully handle errors, preventing crashes.