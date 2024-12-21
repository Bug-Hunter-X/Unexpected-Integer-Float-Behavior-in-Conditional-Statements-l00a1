# Julia Integer/Float Conditional Statement Bug

This repository demonstrates a subtle bug related to how Julia handles integers and floating-point numbers within conditional statements.  The `my_function` example appears to correctly handle positive and negative numbers, but exhibits unexpected behavior when the input is zero.

## Bug Description
The `my_function` in `bug.jl` intends to square the input, returning a positive number if positive and a negative number if negative. It fails to handle the case where x is zero, returning 0 instead of the expected 0 (though mathematically correct it is not what the intent was).

## Solution
The solution provided in `bugSolution.jl` addresses the unexpected behavior by explicitly handling the case where x is zero.