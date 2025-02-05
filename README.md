# JavaScript Null Comparison Bug

This repository demonstrates a common but subtle bug in JavaScript related to comparing numbers with null.  The issue stems from JavaScript's loose typing and how it handles comparisons.

## Bug Description

The `foo` function intends to classify numbers into three categories: negative, zero, and positive. However, due to the loose equality check (`===`), the comparison `x === null` can lead to unexpected results when `x` is a number.

## How to Reproduce

1. Clone this repository.
2. Open `bug.js`.
3. Run the script.  You will observe that `foo(0)` returns 1, which is unexpected. 

## Solution

The solution involves adding explicit type checking before comparing to `null`.  See `bugSolution.js` for a corrected version.

## Contribution

Contributions are welcome!