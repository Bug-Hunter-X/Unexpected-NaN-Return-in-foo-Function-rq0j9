# Unexpected NaN Return in foo Function

This repository demonstrates an unexpected behavior in a simple JavaScript function when called with undefined as the parameter. The function is intended to handle null values gracefully but fails to do so with undefined, resulting in NaN.

## Bug Description
The `foo` function is designed to return 0 when the input is null, and add 1 to the input otherwise. When `undefined` is passed, it unexpectedly returns `NaN`.

## Bug Solution
The solution involves adding a check for undefined and handling it appropriately, such as returning 0 or throwing an error. This makes the function's behavior more predictable and robust.

## How to reproduce
1. Clone this repository.
2. Open `bug.js`.
3. Run `node bug.js` to see the unexpected NaN output.
4. Open `bugSolution.js` to see the corrected code.
5. Run `node bugSolution.js` to see the corrected output.