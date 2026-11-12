
# Exercise 7. Inverse of a Product — Solution

## Given Matrices

We are given:

$$
A=
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix},
\qquad
B=
\begin{pmatrix}
2 & 0 \\
0 & 3
\end{pmatrix}
$$

The task is to calculate $(AB)^{-1}$ and $B^{-1}A^{-1}$, verify that they are equal, and explain why the order is reversed.

## Step 1. Calculate AB

First, multiply the two matrices:

$$
AB=
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
2 & 0 \\
0 & 3
\end{pmatrix}
$$

$$
AB=
\begin{pmatrix}
2 & 3 \\
0 & 3
\end{pmatrix}
$$

## Step 2. Find the Inverse of AB

The determinant is:

$$
\det(AB)=(2)(3)-(3)(0)=6
$$

Since the determinant is nonzero, the inverse exists.

Using the inverse formula:

$$
(AB)^{-1}=
\frac{1}{6}
\begin{pmatrix}
3 & -3 \\
0 & 2
\end{pmatrix}
$$

Therefore:

$$
\boxed{
(AB)^{-1}=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & \frac{1}{3}
\end{pmatrix}
}
$$

## Step 3. Find A^{-1} and B^{-1}

For matrix $A$:

$$
A=
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
$$

Its determinant is:

$$
\det(A)=1
$$

Therefore:

$$
A^{-1}=
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}
$$

For matrix $B$:

$$
B=
\begin{pmatrix}
2 & 0 \\
0 & 3
\end{pmatrix}
$$

Since $B$ is diagonal, its inverse is:

$$
B^{-1}=
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & \frac{1}{3}
\end{pmatrix}
$$

## Step 4. Calculate B^{-1}A^{-1}

Multiply the inverse matrices in reverse order:

$$
B^{-1}A^{-1}=
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & \frac{1}{3}
\end{pmatrix}
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}
$$

Performing matrix multiplication:

$$
B^{-1}A^{-1}=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & \frac{1}{3}
\end{pmatrix}
$$

Therefore:

$$
\boxed{(AB)^{-1}=B^{-1}A^{-1}}
$$

Both methods give the same result.

## Step 5. Verify the Result

To verify, calculate:

$$
(AB)(B^{-1}A^{-1})
$$

$$
=
\begin{pmatrix}
2 & 3 \\
0 & 3
\end{pmatrix}
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & \frac{1}{3}
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
1 & -1+1 \\
0 & 1
\end{pmatrix}
$$

Therefore:

$$
\boxed{
(AB)(B^{-1}A^{-1})=
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
=I
}
$$

This confirms that $B^{-1}A^{-1}$ is the inverse of $AB$.

## Step 6. Explain the Reversed Order

The inverse-of-a-product property is:

$$
(AB)^{-1}=B^{-1}A^{-1}
$$

When the product $AB$ acts on a column vector, matrix $B$ is applied first, followed by matrix $A$.

To undo these transformations, we must reverse their order.

Therefore, we first apply $A^{-1}$ and then $B^{-1}$.

Algebraically:

$$
(AB)(B^{-1}A^{-1})
=A(BB^{-1})A^{-1}
$$

Since $BB^{-1}=I$:

$$
=AIA^{-1}
=AA^{-1}
=I
$$

Similarly:

$$
(B^{-1}A^{-1})(AB)
=B^{-1}(A^{-1}A)B
$$

$$
=B^{-1}IB
=B^{-1}B
=I
$$

Thus, the reversed order is necessary to cancel the matrices correctly.

## Final Answer

We obtained:

$$
\boxed{
(AB)^{-1}=B^{-1}A^{-1}=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & \frac{1}{3}
\end{pmatrix}
}
$$

**Verification:**

$$
(AB)(B^{-1}A^{-1})=I
$$

**Conclusion:**

Both calculations produce the same inverse matrix.

The order is reversed because matrix transformations must be undone in the opposite order in which they are applied.

The result confirms the property:

$$
\boxed{(AB)^{-1}=B^{-1}A^{-1}}
$$

