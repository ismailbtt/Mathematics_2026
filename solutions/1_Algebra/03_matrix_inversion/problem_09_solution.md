
# Exercise 9. Matrix Equation — Solution

## Given Matrices

We are given:

$$
A=\begin{pmatrix}1 & 2 \\ 0 & 1\end{pmatrix}
$$

$$
B=\begin{pmatrix}3 & 1 \\ 2 & 4\end{pmatrix}
$$

The task is to solve the matrix equation:

$$
AX=B
$$

## Step 1. Determine the Correct Multiplication Side

To isolate $X$, we must multiply both sides by $A^{-1}$ from the left.

$$
A^{-1}AX=A^{-1}B
$$

Since $A^{-1}A=I$, we obtain:

$$
X=A^{-1}B
$$

The multiplication must be performed from the left because matrix multiplication is generally not commutative.

## Step 2. Find the Inverse of A

First, calculate the determinant:

$$
\det(A)=(1)(1)-(2)(0)=1
$$

Since the determinant is nonzero, the inverse exists.

Using the inverse formula:

$$
A^{-1}=\frac{1}{1}\begin{pmatrix}1 & -2 \\ 0 & 1\end{pmatrix}
$$

Therefore:

$$
A^{-1}=\begin{pmatrix}1 & -2 \\ 0 & 1\end{pmatrix}
$$

## Step 3. Calculate X

Using the equation:

$$
X=A^{-1}B
$$

Substitute the matrices:

$$
X=\begin{pmatrix}1 & -2 \\ 0 & 1\end{pmatrix}\begin{pmatrix}3 & 1 \\ 2 & 4\end{pmatrix}
$$

Performing matrix multiplication:

$$
X=\begin{pmatrix}3-4 & 1-8 \\ 2 & 4\end{pmatrix}
$$

Therefore:

$$
X=\begin{pmatrix}-1 & -7 \\ 2 & 4\end{pmatrix}
$$

## Step 4. Verify the Result

To verify the solution, calculate $AX$:

$$
AX=\begin{pmatrix}1 & 2 \\ 0 & 1\end{pmatrix}\begin{pmatrix}-1 & -7 \\ 2 & 4\end{pmatrix}
$$

Performing matrix multiplication:

$$
AX=\begin{pmatrix}-1+4 & -7+8 \\ 2 & 4\end{pmatrix}
$$

Therefore:

$$
AX=\begin{pmatrix}3 & 1 \\ 2 & 4\end{pmatrix}=B
$$

The result satisfies the original matrix equation.

## Final Answer

$$
\boxed{X=\begin{pmatrix}-1 & -7 \\ 2 & 4\end{pmatrix}}
$$

**Verification:**

$$
AX=B
$$

**Conclusion:**

The matrix equation was solved by multiplying both sides by $A^{-1}$ from the left.

The calculated matrix satisfies $AX=B$, confirming that the solution is correct.
