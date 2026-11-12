
# Exercise 8. Inverse of a Transformation — Solution

## Given Matrix

We are given the scaling matrix:

$$
S=
\begin{pmatrix}
2 & 0 \\
0 & \frac{1}{2}
\end{pmatrix}
$$

The task is to find $S^{-1}$, explain its geometric meaning, and verify the transformation using a simple vector.

## Step 1. Find the Inverse Matrix

Since $S$ is a diagonal matrix, its inverse is obtained by taking the reciprocal of each diagonal element.

The determinant is:

$$
\det(S)=2\cdot\frac{1}{2}=1
$$

Since $\det(S)\neq 0$, the inverse exists.

Therefore:

$$
\boxed{
S^{-1}=
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 2
\end{pmatrix}
}
$$

## Step 2. Geometric Interpretation

The original transformation $S$ scales a vector as follows:

$$
S
\begin{pmatrix}
x \\
y
\end{pmatrix}
=
\begin{pmatrix}
2x \\
\frac{y}{2}
\end{pmatrix}
$$

This means that:

- The x-coordinate is stretched by a factor of $2$.
- The y-coordinate is compressed by a factor of $\frac{1}{2}$.

The inverse transformation reverses these effects:

$$
S^{-1}
\begin{pmatrix}
x \\
y
\end{pmatrix}
=
\begin{pmatrix}
\frac{x}{2} \\
2y
\end{pmatrix}
$$

Thus, $S^{-1}$ compresses the x-coordinate by $\frac{1}{2}$ and stretches the y-coordinate by $2$.

## Step 3. Verify Using a Vector

Consider the vector:

$$
v=
\begin{pmatrix}
2 \\
4
\end{pmatrix}
$$

First, apply the original transformation:

$$
Sv=
\begin{pmatrix}
2 & 0 \\
0 & \frac{1}{2}
\end{pmatrix}
\begin{pmatrix}
2 \\
4
\end{pmatrix}
$$

$$
Sv=
\begin{pmatrix}
4 \\
2
\end{pmatrix}
$$

Now apply the inverse transformation:

$$
S^{-1}(Sv)=
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 2
\end{pmatrix}
\begin{pmatrix}
4 \\
2
\end{pmatrix}
$$

$$
S^{-1}(Sv)=
\begin{pmatrix}
2 \\
4
\end{pmatrix}
=v
$$

The original vector is recovered.

## Step 4. Verify by Matrix Multiplication

To confirm the inverse, calculate $SS^{-1}$:

$$
SS^{-1}=
\begin{pmatrix}
2 & 0 \\
0 & \frac{1}{2}
\end{pmatrix}
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 2
\end{pmatrix}
$$

$$
SS^{-1}=
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
=I
$$

Therefore, the inverse matrix is correct.

## Final Answer

$$
\boxed{
S^{-1}=
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 2
\end{pmatrix}
}
$$

**Verification:**

$$
\begin{pmatrix}
2 \\
4
\end{pmatrix}
\xrightarrow{S}
\begin{pmatrix}
4 \\
2
\end{pmatrix}
\xrightarrow{S^{-1}}
\begin{pmatrix}
2 \\
4
\end{pmatrix}
$$

**Conclusion:**

The inverse transformation reverses the scaling performed by $S$. It restores the original vector, and the identity $SS^{-1}=I$ confirms that the inverse is correct.
