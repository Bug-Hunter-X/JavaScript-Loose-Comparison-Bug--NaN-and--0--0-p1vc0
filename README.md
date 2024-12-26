# JavaScript Loose Comparison Bug: NaN and +0/-0

This repository demonstrates a common JavaScript error related to loose comparison using the `==` operator when dealing with special values like `NaN` (Not a Number) and positive/negative zero (`+0` and `-0`).

**Problem:**

JavaScript's loose equality (`==`) does not always behave as expected when comparing `NaN` and `+0/-0`.  `NaN` is never equal to itself, and `+0` is loosely equal to `-0`.

**Solution:**

Always use strict equality (`===`) for comparisons to avoid these issues. Strict equality will not perform type coercion and will correctly identify differences between these values.

**Example:**

The `bug.js` file shows the unexpected behavior with loose comparison. The `bugSolution.js` file shows the correct use of strict equality.

Feel free to clone this repository and experiment with the code.