# CSS Specificity and Inheritance Bug

This repository demonstrates a subtle bug related to CSS specificity and inheritance.  In certain situations, a more specific CSS rule might not override an inherited style due to the way the browser handles specificity and inheritance.

## Bug Description

A nested element's style may unexpectedly inherit properties from an ancestor even when a more specific selector targets it. This can lead to unexpected styling that defies typical specificity rules.

## How to Reproduce

1. Clone this repository.
2. Open `bug.html` in your browser.
3. Observe that the paragraph text is red, not green as expected.

## Solution

The solution involves understanding and carefully applying CSS specificity rules, and potentially using the `!important` flag (though this is generally discouraged).

See `bugSolution.css` for a corrected version.