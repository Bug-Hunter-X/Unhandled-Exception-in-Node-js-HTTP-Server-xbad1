# Unhandled Exception in Node.js HTTP Server

This repository demonstrates a common error in Node.js where an unhandled exception causes the server to crash.  The `bug.js` file shows the problematic code, while `bugSolution.js` provides a corrected version with proper error handling.

## Problem

The original code lacks error handling, so any unexpected issues within the request processing lead to the server crashing. This is poor practice and results in application instability.

## Solution

The solution involves using a `try...catch` block to gracefully handle exceptions. This prevents the server from crashing and allows for more robust error reporting and recovery.

## How to reproduce

1. Clone this repository.
2. Run `node bug.js` (Expect it to work initially, then force an error). 
3. Run `node bugSolution.js` (The improved version)