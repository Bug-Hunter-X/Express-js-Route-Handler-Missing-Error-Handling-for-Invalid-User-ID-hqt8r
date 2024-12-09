# Express.js Route Handler Missing Error Handling for Invalid User ID

This repository demonstrates a common error in Express.js route handlers: the lack of error handling for invalid input.  Specifically, the provided code attempts to parse a user ID from the request parameters as an integer without checking for potential errors, like a non-numeric ID being passed in.

The `bug.js` file shows the problematic code. The `bugSolution.js` file presents a corrected version with proper error handling.

## How to Reproduce

1. Clone this repository.
2. Run `npm install express` to install Express.js
3. Run `node bug.js` and make a request to `/users/abc` (non-numeric ID).
4. Observe the error.
5. Then run `node bugSolution.js` and make the same request to see the improved behavior.