# CSS calc() Negative Value Bug

This repository demonstrates a subtle bug related to using `calc()` in CSS with negative values. Some browsers may not handle negative results from `calc()` consistently, leading to unexpected layout or rendering issues.

## Bug Description

The `calc()` function in CSS is powerful for dynamic calculations. However, when the calculation results in a negative value, the behavior can differ across browsers. This inconsistency can cause unpredictable layout problems, especially concerning dimensions (width, height, margin, padding).

## Reproduction

1. Open `bug.css` to see the problematic CSS code.
2. Observe how different browsers render the element with the negative `calc()` value.
3. Compare this to the corrected version in `bugSolution.css`.

## Solution

The solution involves using `max()` or `min()` to constrain the calculated value to be non-negative. This ensures consistent rendering across different browsers.

## Conclusion

This example highlights an uncommon but important CSS bug. Always be mindful of the potential for negative values when using `calc()` and consider using `max()` or `min()` functions to handle such cases appropriately.