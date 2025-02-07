# CSS `calc()` Gotchas

This repository demonstrates some uncommon but potentially problematic scenarios when using the CSS `calc()` function.  Specifically, it highlights issues with nested `calc()` expressions and the importance of including units in calculations.  The `bug.css` file contains the problematic code, while `bugSolution.css` presents the corrected versions.

## Issues:

* **Nested `calc()`:**  Multiple nested `calc()` calls can lead to unexpected parsing and potentially different behavior across browsers.  Simplifying these expressions is recommended.
* **Missing Units:** Forgetting to specify units (like `px`, `em`, `%`, etc.) within `calc()` expressions will frequently result in errors or unexpected behavior.

## Solutions:

The `bugSolution.css` file demonstrates how to fix these issues by:

1. **Simplifying nested expressions:** Combining operations to reduce nesting.
2. **Ensuring units are consistently included:**  Always specify the appropriate units for all values within the `calc()` function.