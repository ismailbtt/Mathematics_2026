
### Exercise 2. Formula for a 2×2 Matrix — Solution

**Given:**

$$
A=
\begin{pmatrix}
3 & 2 \\
5 & 4
\end{pmatrix}
$$

We need to find the inverse of matrix $A$ using the formula for a $2 \times 2$ matrix and verify the result by multiplication.

### Step 1. Calculate the Determinant

For a $2 \times 2$ matrix, the determinant is calculated as:

$$
\det(A)=ad-bc
$$

Substituting the values:

$$
\det(A)=(3)(4)-(2)(5)
$$

$$
\det(A)=12-10=2
$$

Since $\det(A)=2\neq 0$, the matrix is invertible.

### Step 2. Find the Inverse

The inverse formula is:

$$
A^{-1}=\frac{1}{ad-bc}
\begin{pmatrix}
d & -b \\
-c & a
\end{pmatrix}
$$

Substituting the values:

$$
A^{-1}=\frac{1}{2}
\begin{pmatrix}
4 & -2 \\
-5 & 3
\end{pmatrix}
$$

Multiplying each element by $\frac{1}{2}$:

$$
A^{-1}=
\begin{pmatrix}
2 & -1 \\
-\frac{5}{2} & \frac{3}{2}
\end{pmatrix}
$$

### Step 3. Verify the Result

To verify the inverse, we calculate $AA^{-1}$.

$$
AA^{-1}=
\begin{pmatrix}
3 & 2 \\
5 & 4
\end{pmatrix}
\begin{pmatrix}
2 & -1 \\
-\frac{5}{2} & \frac{3}{2}
\end{pmatrix}
$$

Performing matrix multiplication:

$$
AA^{-1}=
\begin{pmatrix}
6-5 & -3+3 \\
10-10 & -5+6
\end{pmatrix}
$$

Therefore:

$$
AA^{-1}=
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
=I
$$

### Final Answer

$$
A^{-1}=
\begin{pmatrix}
2 & -1 \\
-\frac{5}{2} & \frac{3}{2}
\end{pmatrix}
$$

**Conclusion:**

Since the determinant is nonzero, the inverse exists. The multiplication $AA^{-1}=I$ confirms that the calculated inverse is correct.
