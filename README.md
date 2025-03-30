# Multicases

This project demonstrates the usage of the `multicases` package in LaTeX, which provides an environment for typesetting cases with multiple columns. This is useful for displaying piecewise functions with additional annotations or explanations in separate columns.

## Usage

The `multicases` environment takes two optional arguments:
- The number of columns (default is 2).
- The alignment specification for the columns (default is the first column centered and the rest left-aligned). The alignment characters are `l`, `c`, `r`, and `a` (for `align`-like behaviour).

### Example

Here is an example of how to use the `multicases` environment:

```latex
\begin{multicases}[3][cla]
    x^2 + \sum{a_{x}^3}        & \text{if $x<0$}  & 0~&(\text{negative}) \\[1em]
    \displaystyle\frac{1}{x^2} & \text{if $x>0$}  & 1/x~&(\text{positive}) \\[1em]
    0                          & \text{otherwise} & 0~&(\text{zero})
\end{multicases}
```

For more details and examples, please refer to the [sample.pdf](sample.pdf).
