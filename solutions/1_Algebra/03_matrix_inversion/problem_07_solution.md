
# Exercise 7. Inverse of a Product — Solution

## Given Matrices

We are given the following matrices:

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

The task is to calculate $(AB)^{-1}$ and $B^{-1}A^{-1}$, verify that they are equal, and explain why the order of multiplication is reversed.

## Step 1. Calculate the Product AB

First, multiply matrices $A$ and $B$:

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

Performing matrix multiplication:

$$
AB=
\begin{pmatrix}
1(2)+1(0) & 1(0)+1(3) \\
0(2)+1(0) & 0(0)+1(3)
\end{pmatrix}
$$

Therefore:

$$
AB=
\begin{pmatrix}
2 & 3 \\
0 & 3
\end{pmatrix}
$$

## Step 2. Find the Inverse of AB

For a general $2 \times 2$ matrix, the inverse formula is:

$$
M^{-1}=
\frac{1}{ad-bc}
\begin{pmatrix}
d & -b \\
-c & a
\end{pmatrix}
$$

First, calculate the determinant of $AB$:

$$
\det(AB)=(2)(3)-(3)(0)
$$

$$
\det(AB)=6
$$

Since the determinant is nonzero, the inverse exists.

Applying the inverse formula:

$$
(AB)^{-1}=
\frac{1}{6}
\begin{pmatrix}
3 & -3 \\
0 & 2
\end{pmatrix}
$$

Simplifying:

$$
\boxed{
(AB)^{-1}=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & \frac{1}{3}
\end{pmatrix}
}
$$

## Step 3. Calculate the Inverse of A

The matrix $A$ is:

$$
A=
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
$$

Its determinant is:

$$
\det(A)=(1)(1)-(1)(0)=1
$$

Using the inverse formula:

$$
A^{-1}=
\frac{1}{1}
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}
$$

Therefore:

$$
\boxed{
A^{-1}=
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}
}
$$

## Step 4. Calculate the Inverse of B

The matrix $B$ is:

$$
B=
\begin{pmatrix}
2 & 0 \\
0 & 3
\end{pmatrix}
$$

Since $B$ is a diagonal matrix, its inverse is obtained by taking the reciprocal of each nonzero diagonal element.

Therefore:

$$
\boxed{
B^{-1}=
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & \frac{1}{3}
\end{pmatrix}
}
$$

## Step 5. Calculate B^{-1}A^{-1}

Now, multiply the inverse matrices in reverse order:

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
\frac{1}{2}(1)+0(0) & \frac{1}{2}(-1)+0(1) \\
0(1)+\frac{1}{3}(0) & 0(-1)+\frac{1}{3}(1)
\end{pmatrix}
$$

Simplifying:

$$
\boxed{
B^{-1}A^{-1}=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & \frac{1}{3}
\end{pmatrix}
}
$$

## Step 6. Compare the Results

From Step 2, we obtained:

$$
(AB)^{-1}=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & \frac{1}{3}
\end{pmatrix}
$$

From Step 5, we obtained:

$$
B^{-1}A^{-1}=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & \frac{1}{3}
\end{pmatrix}
$$

Both matrices are identical.

Therefore:

$$
\boxed{(AB)^{-1}=B^{-1}A^{-1}}
$$

This confirms the inverse-of-a-product property.

## Step 7. Verify by Multiplication

To verify the result, calculate:

$$
(AB)(B^{-1}A^{-1})
$$

Substituting the matrices:

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

Performing matrix multiplication:

$$
=
\begin{pmatrix}
2(\frac{1}{2})+3(0) & 2(-\frac{1}{2})+3(\frac{1}{3}) \\
0(\frac{1}{2})+3(0) & 0(-\frac{1}{2})+3(\frac{1}{3})
\end{pmatrix}
$$

Simplifying:

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

The multiplication confirms that $B^{-1}A^{-1}$ is the inverse of $AB$.

## Step 8. Explain the Reversed Order

The inverse of a product follows the rule:

$$
(AB)^{-1}=B^{-1}A^{-1}
$$

The order is reversed because matrix multiplication is generally not commutative.

To undo the product $AB$, we must first cancel $B$ and then cancel $A$.

Algebraically:

$$
(AB)(B^{-1}A^{-1})
$$

Using associativity:

$$
=A(BB^{-1})A^{-1}
$$

Since $BB^{-1}=I$:

$$
=AIA^{-1}
$$

$$
=AA^{-1}
$$

$$
=I
$$

Similarly, multiplication in the opposite direction gives:

$$
(B^{-1}A^{-1})(AB)
$$

$$
=B^{-1}(A^{-1}A)B
$$

$$
=B^{-1}IB
$$

$$
=I
$$

Thus, the reversed order guarantees that the factors cancel correctly.

## Final Answer

We calculated:

$$
(AB)^{-1}=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & \frac{1}{3}
\end{pmatrix}
$$

and:

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

**Verification:**

$$
(AB)(B^{-1}A^{-1})=I
$$

**Conclusion:**

Both methods produce the same inverse matrix.

The inverse of a product is obtained by multiplying the individual inverses in reverse order.

This is necessary because matrix multiplication is generally not commutative, and the reversed order allows the original transformations to be undone correctly.
