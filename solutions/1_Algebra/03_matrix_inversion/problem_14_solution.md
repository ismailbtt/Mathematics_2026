
# Exercise 14. A Matrix That Is Its Own Inverse — Solution

## Given Condition

We are given a square matrix $A$ satisfying:

$$
A^2=I
$$

The task is to prove that $A^{-1}=A$ and provide a $2 \times 2$ example different from $I$ and $-I$.

## Step 1. Prove That A^{-1} = A

By definition, the inverse of a square matrix $A$ satisfies:

$$
AA^{-1}=A^{-1}A=I
$$

We are given:

$$
A^2=I
$$

Since $A^2=AA$, we have:

$$
AA=I
$$

Thus, multiplying $A$ by itself produces the identity matrix.

Therefore, $A$ is its own inverse:

$$
\boxed{A^{-1}=A}
$$

Such a matrix is called an involutory matrix.

## Step 2. Provide an Example

Consider the matrix:

$$
A=\begin{pmatrix}0 & 1 \\ 1 & 0\end{pmatrix}
$$

This matrix is different from both $I$ and $-I$.

We will verify that it satisfies $A^2=I$.

## Step 3. Verify by Multiplication

Calculate:

$$
A^2=AA
$$

Substituting the matrix:

$$
A^2=\begin{pmatrix}0 & 1 \\ 1 & 0\end{pmatrix}\begin{pmatrix}0 & 1 \\ 1 & 0\end{pmatrix}
$$

Performing matrix multiplication:

$$
A^2=\begin{pmatrix}0(0)+1(1) & 0(1)+1(0) \\ 1(0)+0(1) & 1(1)+0(0)\end{pmatrix}
$$

Simplifying:

$$
A^2=\begin{pmatrix}1 & 0 \\ 0 & 1\end{pmatrix}=I
$$

Therefore:

$$
\boxed{A^2=I}
$$

Since $AA=I$, the matrix is its own inverse:

$$
\boxed{A^{-1}=A}
$$

## Final Answer

If a square matrix satisfies:

$$
A^2=I
$$

then:

$$
\boxed{A^{-1}=A}
$$

An example is:

$$
\boxed{A=\begin{pmatrix}0 & 1 \\ 1 & 0\end{pmatrix}}
$$

**Verification:**

$$
A^2=\begin{pmatrix}1 & 0 \\ 0 & 1\end{pmatrix}=I
$$

**Conclusion:**

The condition $A^2=I$ proves that a matrix is its own inverse.

The given example satisfies this condition and is different from both $I$ and $-I$.

Therefore, the statement is verified.
