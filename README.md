# Module-5-R-programming

The reason why solve(A) and det(A) work is because the dimensions are square, which are one of the requirments needed for it to run sucessfully. In addition,
we see that the matrix is single because the output put out is 0.

In comparison, the reason why operations on B fail (non‑square matrix) is because one of the requirements needed to run Solve() and det() is that it must be square.
because the dimensions for b are not, it returns an error.

lastly, for notes on numeric stability or performance, i notice that it performs better if I used trycatch for A to run, otherwise it gives an error and won't run.

here is the output:

#now here is me calling each one to compare answers
> invA
<simpleError in solve.default(A): Lapack routine dgesv: system is exactly singular: U[6,6] = 0>
> detA
[1] 0
> invB
<simpleError in solve.default(B): 'a' (10 x 100) must be square>
> detB
<simpleError in determinant.matrix(x, logarithm = TRUE, ...): 'x' must be a square matrix>
