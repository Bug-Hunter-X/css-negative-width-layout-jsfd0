# CSS `calc()` Unexpected Behavior

This repository demonstrates an uncommon CSS bug related to the `calc()` function. When calculating widths or heights using `calc()`, unexpected behavior can occur when the calculated value results in a negative number. This typically happens when subtracting a large fixed value from a percentage-based value in a small container.

The `bug.css` file showcases the problematic code, and `bugSolution.css` presents the solution.

## Reproducing the Bug

1. Open `bug.html` in a browser.
2. Observe the unexpected width of the div element.

## Solution

The solution involves adding a `max-width` or using `min()` to ensure the calculated value doesn't become negative. See `bugSolution.css` for an example.