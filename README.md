# Unhandled Error in Express.js Route Handler for Invalid User ID

This repository demonstrates a common error in Express.js route handlers:  failure to handle cases where user input (in this case, a user ID) is not in the expected format. The provided code attempts to parse a user ID as an integer without checking for potential errors, leading to unexpected behavior or crashes if the ID is not a valid number.  The solution demonstrates how to implement proper error handling using try-catch blocks and input validation.

## Bug Description
The `bug.js` file contains an Express.js route handler that fetches a user by ID. However, it lacks proper error handling. If a non-numeric value is provided as the user ID, `parseInt()` will return `NaN`, leading to potential crashes or unexpected behavior.

## Solution
The `bugSolution.js` file corrects this by adding a `try...catch` block to handle potential `NaN` values and provides a more robust solution by validating the input before parsing it.
