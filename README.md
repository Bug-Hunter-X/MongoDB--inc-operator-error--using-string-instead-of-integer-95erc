# MongoDB $inc Operator Error: Using String Instead of Integer

This repository demonstrates a common error when using the `$inc` operator in MongoDB update operations. The error occurs when a string is provided as the increment value instead of a number.

## Problem
The `$inc` operator is designed to increment a numeric field in a document.  If a string is passed as the increment value, the update operation will likely fail without throwing an explicit error, leading to unexpected and difficult-to-debug issues.

## Solution
Ensure that the value provided to the `$inc` operator is an integer or a number.  Avoid using strings.

## Code Example
The `bug.js` file shows the incorrect usage of the `$inc` operator. The `bugSolution.js` file demonstrates the corrected approach.
