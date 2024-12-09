# Express.js Route Parameter Handling Bug

This repository demonstrates a common bug in Express.js route parameter handling and provides a solution.

## Bug Description
The provided Express.js code snippet has a vulnerability. It fails to handle non-numeric user IDs correctly, which can lead to unexpected errors or allow malicious users to potentially access unintended data or functionality.

## Bug Reproduction
1. Clone this repository.
2. Run `npm install` to install Express.js.
3. Run `node bug.js` to start the server.
4. Send a request to `/users/abc` (or any non-numeric ID).  The server may crash or show unexpected behavior.

## Solution
The `bugSolution.js` file shows the corrected code.  It explicitly checks and sanitizes input, preventing potential errors and vulnerabilities.

## Mitigation
Always validate and sanitize user inputs before using them in database queries or other sensitive operations to prevent common vulnerabilities like SQL injection.