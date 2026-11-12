
# Exercise 10. Inverse of a Diagonal Matrix — Solution

## Given Matrices

We are given two diagonal matrices:

$$
D=\begin{pmatrix}2 & 0 & 0 \\ 0 & -3 & 0 \\ 0 & 0 & 5\end{pmatrix}
$$

$$
E=\begin{pmatrix}2 & 0 & 0 \\ 0 & 0 & 0 \\ 0 & 0 & 5\end{pmatrix}
$$

The task is to determine which matrix is invertible, find its inverse, and verify the result without using Gauss–Jordan elimination.

## Step 1. Determine Invertibility

A diagonal matrix is invertible if and only if all its diagonal elements are nonzero.

For matrix $D$, the determinant is:

$$
\det(D)=2(-3)(5)=-30
$$

Since $\det(D)\neq 0$, matrix $D$ is invertible.

For matrix $E$, the determinant is:

$$
\det(E)=2(0)(5)=0
$$

Since $\det(E)=0$, matrix $E$ is not invertible.

Therefore, only matrix $D$ has an inverse.

## Step 2. Find the Inverse of D

The inverse of an invertible diagonal matrix is obtained by taking the reciprocal of each diagonal element.

The original matrix is:

$$
D=\begin{pmatrix}2 & 0 & 0 \\ 0 & -3 & 0 \\ 0 & 0 & 5\end{pmatrix}
$$

Taking the reciprocals gives:

$$
\boxed{D^{-1}=\begin{pmatrix}\frac{1}{2} & 0 & 0 \\ 0 & -\frac{1}{3} & 0 \\ 0 & 0 & \frac{1}{5}\end{pmatrix}}
$$

## Step 3. Verify the Result

To verify the inverse, calculate $DD^{-1}$:

$$
DD^{-1}=\begin{pmatrix}2 & 0 & 0 \\ 0 & -3 & 0 \\ 0 & 0 & 5\end{pmatrix}\begin{pmatrix}\frac{1}{2} & 0 & 0 \\ 0 & -\frac{1}{3} & 0 \\ 0 & 0 & \frac{1}{5}\end{pmatrix}
$$

Since both matrices are diagonal, their product is also diagonal.

$$
DD^{-1}=\begin{pmatrix}2(\frac{1}{2}) & 0 & 0 \\ 0 & (-3)(-\frac{1}{3}) & 0 \\ 0 & 0 & 5(\frac{1}{5})\end{pmatrix}
$$

Simplifying:

$$
DD^{-1}=\begin{pmatrix}1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1\end{pmatrix}=I
$$

This confirms that the calculated inverse is correct.

## Final Answer

Matrix $D$ is invertible because:

$$
\det(D)=-30\neq 0
$$

Its inverse is:

$$
\boxed{D^{-1}=\begin{pmatrix}\frac{1}{2} & 0 & 0 \\ 0 & -\frac{1}{3} & 0 \\ 0 & 0 & \frac{1}{5}\end{pmatrix}}
$$

Matrix $E$ is not invertible because:

$$
\det(E)=0
$$

**Verification:**

$$
DD^{-1}=I
$$

**Conclusion:**

Only matrix $D$ is invertible because all its diagonal elements are nonzero. Its inverse is obtained by taking the reciprocal of each diagonal element.

Matrix $E$ has no inverse because it contains a zero diagonal element.
