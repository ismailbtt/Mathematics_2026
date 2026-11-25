
# Exercise 8 – Inverse of a Transformation

## Question

Given the scaling matrix:

$$
S=
\begin{pmatrix}
2 & 0 \\
0 & \frac{1}{2}
\end{pmatrix}
$$

1. Find the inverse matrix $S^{-1}$.
2. Explain the geometric meaning of the inverse transformation.
3. Verify the result using a simple vector.

---

## Solution

### Step 1. Find the Inverse Matrix

The given matrix is:

$$
S=
\begin{pmatrix}
2 & 0 \\
0 & \frac{1}{2}
\end{pmatrix}
$$

First, calculate the determinant:

$$
\det(S)=2\cdot\frac{1}{2}-0\cdot0
$$

$$
\det(S)=1
$$

Since the determinant is not zero, the inverse matrix exists.

For a diagonal matrix, we take the reciprocal of each diagonal element.

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

### Step 2. Geometric Interpretation

The original transformation is:

$$
S
\begin{pmatrix}
x\\y
\end{pmatrix}
=
\begin{pmatrix}
2x\\
\frac{y}{2}
\end{pmatrix}
$$

This means:

- The x-coordinate is stretched by a factor of 2.
- The y-coordinate is compressed by a factor of 1/2.

The inverse transformation reverses these effects:

$$
S^{-1}
\begin{pmatrix}
x\\y
\end{pmatrix}
=
\begin{pmatrix}
\frac{x}{2}\\
2y
\end{pmatrix}
$$

This means:

- The x-coordinate is compressed by a factor of 1/2.
- The y-coordinate is stretched by a factor of 2.

The inverse transformation restores the original coordinates.

### Step 3. Verify Using a Vector

Consider the vector:

$$
v=
\begin{pmatrix}
2\\
4
\end{pmatrix}
$$

First, apply the original transformation:

$$
Sv=
\begin{pmatrix}
2 & 0\\
0 & \frac{1}{2}
\end{pmatrix}
\begin{pmatrix}
2\\
4
\end{pmatrix}
$$

$$
Sv=
\begin{pmatrix}
4\\
2
\end{pmatrix}
$$

Now apply the inverse transformation:

$$
S^{-1}(Sv)=
\begin{pmatrix}
\frac{1}{2} & 0\\
0 & 2
\end{pmatrix}
\begin{pmatrix}
4\\
2
\end{pmatrix}
$$

$$
S^{-1}(Sv)=
\begin{pmatrix}
2\\
4
\end{pmatrix}
=v
$$

The original vector is recovered.

### Step 4. Verify by Matrix Multiplication

Multiply the original matrix by its inverse:

$$
SS^{-1}=
\begin{pmatrix}
2 & 0\\
0 & \frac{1}{2}
\end{pmatrix}
\begin{pmatrix}
\frac{1}{2} & 0\\
0 & 2
\end{pmatrix}
$$

$$
SS^{-1}=
\begin{pmatrix}
1 & 0\\
0 & 1
\end{pmatrix}
=I
$$

The result is the identity matrix, confirming that the inverse is correct.

---

## Final Answer

The inverse matrix is:

$$
\boxed{
S^{-1}=
\begin{pmatrix}
\frac{1}{2} & 0\\
0 & 2
\end{pmatrix}
}
$$

**Vector Verification:**

$$
\begin{pmatrix}
2\\
4
\end{pmatrix}
\xrightarrow{S}
\begin{pmatrix}
4\\
2
\end{pmatrix}
\xrightarrow{S^{-1}}
\begin{pmatrix}
2\\
4
\end{pmatrix}
$$

**Conclusion:**

The inverse transformation reverses the scaling performed by the original matrix. The vector returns to its initial position, and the identity $SS^{-1}=I$ confirms that the inverse matrix is correct.
