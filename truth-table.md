# Truth Tables

In digital electronics and computer science, truth tables reduce Boolean operations to straightforward mappings of inputs to outputs [^1].

A truth table has one column per input variable — in our case, `X`, `Y`, and `Z` — plus a final column showing the result of the logical operation.

## Project Objective

Design a decoder for the letter _n_ and the last three digits of your 900 number, displaying the results on a seven-segment display.

1. Write the truth table for all possible inputs and their corresponding outputs.
2. Draw K-maps for each segment `a` through `g` and derive a simplified Boolean expression for each output.

## My Truth Table

|  X  |  Y  |  Z  | Display |  a  |  b  |  c  |  d  |  e  |  f  |  g  |
| :-: | :-: | :-: | :-----: | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|  0  |  0  |  0  |   `n`   |  0  |  0  |  1  |  0  |  1  |  0  |  1  |
|  0  |  0  |  1  |   `6`   |  1  |  0  |  1  |  1  |  1  |  1  |  1  |
|  0  |  1  |  0  |   `9`   |  1  |  1  |  1  |  0  |  1  |  1  |  1  |
|  0  |  1  |  1  |   `3`   |  1  |  1  |  1  |  0  |  0  |  1  |  1  |
|  1  |  0  |  0  |   `-`   |  0  |  0  |  0  |  0  |  0  |  0  |  1  |
|  1  |  0  |  1  |   `-`   |  0  |  0  |  0  |  0  |  0  |  0  |  1  |
|  1  |  1  |  0  |   `-`   |  0  |  0  |  0  |  0  |  0  |  0  |  1  |
|  1  |  1  |  1  |   `-`   |  0  |  0  |  0  |  0  |  0  |  0  |  1  |

### Observations

1. Segment g is always on
2. Segment c = X’ → requires only a single NOT gate
3. Segment b=X’Y → requires one AND gate (with X inverted)

---

### References

[^1]: https://en.wikipedia.org/wiki/Truth_table
