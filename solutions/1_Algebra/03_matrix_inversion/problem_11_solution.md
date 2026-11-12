
# Exercise 11. Parameter and Invertibility — Solution

## Given Matrix

We are given the matrix:

$$
A(t)=\begin{pmatrix}1 & t \\ t & 1\end{pmatrix}
$$

The task is to determine all values of $t$ for which $A(t)$ is invertible and find a formula for its inverse.

We must also explain what happens at the excluded values.

## Step 1. Calculate the Determinant

For a $2 \times 2$ matrix, the determinant is:

$$
\det(A)=ad-bc
$$

Applying this formula:

$$
\det(A(t))=(1)(1)-(t)(t)
$$

Therefore:

$$
\det(A(t))=1-t^2
$$

A matrix is invertible if its determinant is nonzero.

Thus:

$$
1-t^2\neq 0
$$

Factoring:

$$
(1-t)(1+t)\neq 0
$$

Therefore:

$$
\boxed{t\neq 1 \quad \text{and} \quad t\neq -1}
$$

The matrix is invertible for all real values of $t$ except $1$ and $-1$.

## Step 2. Find the Inverse Matrix

The inverse formula for a $2 \times 2$ matrix is:

$$
A^{-1}=\frac{1}{ad-bc}\begin{pmatrix}d & -b \\ -c & a\end{pmatrix}
$$

Substituting the elements of $A(t)$:

$$
A(t)^{-1}=\frac{1}{1-t^2}\begin{pmatrix}1 & -t \\ -t & 1\end{pmatrix}
$$

Therefore:

$$
\boxed{A(t)^{-1}=\frac{1}{1-t^2}\begin{pmatrix}1 & -t \\ -t & 1\end{pmatrix}}
$$

This formula is valid only when $t\neq 1$ and $t\neq -1$.

## Step 3. Examine the Excluded Values

**Case 1: When $t=1$**

$$
A(1)=\begin{pmatrix}1 & 1 \\ 1 & 1\end{pmatrix}
$$

Its determinant is:

$$
\det(A(1))=1-1=0
$$

The two rows are identical, so the matrix is not invertible.

**Case 2: When $t=-1$**

$$
A(-1)=\begin{pmatrix}1 & -1 \\ -1 & 1\end{pmatrix}
$$

Its determinant is:

$$
\det(A(-1))=1-(-1)^2=0
$$

The second row is the negative of the first row, so the matrix is not invertible.

At both excluded values, the denominator $1-t^2$ becomes zero. Therefore, the inverse formula is undefined.

## Step 4. Verify the Result

To verify the inverse, calculate:

$$
A(t)A(t)^{-1}
$$

Substituting:

$$
A(t)A(t)^{-1}=\frac{1}{1-t^2}\begin{pmatrix}1 & t \\ t & 1\end{pmatrix}\begin{pmatrix}1 & -t \\ -t & 1\end{pmatrix}
$$

Performing matrix multiplication:

$$
=\frac{1}{1-t^2}\begin{pmatrix}1-t^2 & 0 \\ 0 & 1-t^2\end{pmatrix}
$$

For $t\neq \pm 1$, simplifying gives:

$$
A(t)A(t)^{-1}=\begin{pmatrix}1 & 0 \\ 0 & 1\end{pmatrix}=I
$$

This confirms that the inverse formula is correct.

## Final Answer

The matrix is invertible when:

$$
\boxed{t\in\mathbb{R}\setminus\{-1,1\}}
$$

For these values, its inverse is:

$$
\boxed{A(t)^{-1}=\frac{1}{1-t^2}\begin{pmatrix}1 & -t \\ -t & 1\end{pmatrix}}
$$

**Conclusion:**

The matrix is invertible for all real values of $t$ except $t=1$ and $t=-1$.

At these excluded values, the determinant becomes zero, the rows are linearly dependent, and the inverse does not exist.

The inverse formula was verified by multiplication, confirming that the result is correct.
