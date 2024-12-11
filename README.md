# Unexpected Behavior in Nested CSS `calc()` Functions

This repository demonstrates an uncommon bug related to unexpected behavior in nested CSS `calc()` functions, specifically when combining percentage-based calculations with subtractions. The bug manifests as layout inconsistencies and potential rounding errors across different browsers.

## Bug Description

The issue arises when using nested `calc()` functions where an inner calculation subtracts a pixel value from a percentage-based width, before the result is used in another calculation. This may lead to discrepancies in the rendered dimensions due to the order of operations or inherent rounding issues within the `calc()` function's implementation across different browsers.

## Reproduction

The `bug.css` file contains the CSS code that reproduces the bug.  Inspect the dimensions of the `.nested` element to observe the inconsistencies.

## Solution

The `bugSolution.css` file demonstrates a potential solution or workaround for this problem.  This solution aims to mitigate these discrepancies by using an alternative approach to the calculation, ensuring greater consistency across browsers.