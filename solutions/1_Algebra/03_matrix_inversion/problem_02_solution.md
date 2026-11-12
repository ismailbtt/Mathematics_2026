
# Exercise 2. Formula for a 2×2 Matrix — Detailed Solution

## Given Matrix

We are given the following matrix:

$$
A=
\begin{pmatrix}
3 & 2 \\
5 & 4
\end{pmatrix}.
$$

The task is to find the inverse of matrix $A$ using the formula for a $2 \times 2$ matrix.

After finding the inverse, we must verify our result by multiplying the original matrix by its inverse.

## Step 1. Recall the Formula for the Inverse of a 2×2 Matrix

For a general $2 \times 2$ matrix

$$
A=
\begin{pmatrix}
a & b \\
c & d
\end{pmatrix},
$$

the inverse is calculated using the following formula:

$$
A^{-1}=
\frac{1}{ad-bc}
\begin{pmatrix}
d & -b \\
-c & a
\end{pmatrix}.
$$

Here,

$$
\det(A)=ad-bc
$$

is the determinant of matrix $A$.

An inverse exists only if the determinant is not equal to zero:

$$
\det(A)\neq 0.
$$

If the determinant is zero, the matrix is singular and does not have an inverse.

Therefore, before applying the inverse formula, we must calculate the determinant of the given matrix.

## Step 2. Identify the Elements of Matrix A

Our matrix is

$$
A=
\begin{pmatrix}
3 & 2 \\
5 & 4
\end{pmatrix}.
$$

Comparing it with the general form

$$
A=
\begin{pmatrix}
a & b \\
c & d
\end{pmatrix},
$$

we identify the following values:

$$
a=3,\qquad b=2,
$$

$$
c=5,\qquad d=4.
$$

These values will be substituted into the determinant and inverse formulas.

## Step 3. Calculate the Determinant

The determinant formula for a $2 \times 2$ matrix is

$$
\det(A)=ad-bc.
$$

Substituting the values gives

$$
\det(A)=(3)(4)-(2)(5).
$$

First, calculate the products:

$$
(3)(4)=12
$$

and

$$
(2)(5)=10.
$$

Therefore,

$$
\det(A)=12-10.
$$

Hence,

$$
\boxed{\det(A)=2}.
$$

Since

$$
2\neq 0,
$$

the determinant is nonzero.

This means that matrix $A$ is invertible, so its inverse exists.

We can now apply the inverse formula.

## Step 4. Apply the Inverse Matrix Formula

Recall the formula:

$$
A^{-1}=
\frac{1}{ad-bc}
\begin{pmatrix}
d & -b \\
-c & a
\end{pmatrix}.
$$

To construct the inverse matrix, we perform the following operations:

1. Exchange the positions of the diagonal elements $a$ and $d$.
2. Change the signs of the off-diagonal elements $b$ and $c$.
3. Multiply the resulting matrix by the reciprocal of the determinant.

For the given matrix,

$$
A=
\begin{pmatrix}
3 & 2 \\
5 & 4
\end{pmatrix},
$$

we exchange the diagonal elements $3$ and $4$.

We also change $2$ to $-2$ and $5$ to $-5$.

Therefore, the resulting matrix is

$$
\begin{pmatrix}
4 & -2 \\
-5 & 3
\end{pmatrix}.
$$

Since the determinant is $2$, we obtain

$$
A^{-1}=
\frac{1}{2}
\begin{pmatrix}
4 & -2 \\
-5 & 3
\end{pmatrix}.
$$

## Step 5. Simplify the Inverse Matrix

We now multiply every element of the matrix by $\frac{1}{2}$:

$$
A^{-1}=
\begin{pmatrix}
\frac{4}{2} & \frac{-2}{2} \\
\frac{-5}{2} & \frac{3}{2}
\end{pmatrix}.
$$

Simplifying each entry gives

$$
A^{-1}=
\begin{pmatrix}
2 & -1 \\
-\frac{5}{2} & \frac{3}{2}
\end{pmatrix}.
$$

Thus, the inverse of matrix $A$ is

$$
\boxed{
A^{-1}=
\begin{pmatrix}
2 & -1 \\
-\frac{5}{2} & \frac{3}{2}
\end{pmatrix}
}.
$$

## Step 6. Verify the Result by Matrix Multiplication

To verify that our answer is correct, we use the definition of an inverse matrix.

A matrix multiplied by its inverse must give the identity matrix:

$$
AA^{-1}=I.
$$

The identity matrix of order $2$ is

$$
I=
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}.
$$

We now calculate

$$
AA^{-1}=
\begin{pmatrix}
3 & 2 \\
5 & 4
\end{pmatrix}
\begin{pmatrix}
2 & -1 \\
-\frac{5}{2} & \frac{3}{2}
\end{pmatrix}.
$$

We multiply each row of the first matrix by each column of the second matrix.

### Calculate the first row, first column

$$
(AA^{-1})_{11}
=
3(2)+2\left(-\frac{5}{2}\right).
$$

Simplifying,

$$
=6-5.
$$

Therefore,

$$
(AA^{-1})_{11}=1.
$$

### Calculate the first row, second column

$$
(AA^{-1})_{12}
=
3(-1)+2\left(\frac{3}{2}\right).
$$

Simplifying,

$$
=-3+3.
$$

Therefore,

$$
(AA^{-1})_{12}=0.
$$

### Calculate the second row, first column

$$
(AA^{-1})_{21}
=
5(2)+4\left(-\frac{5}{2}\right).
$$

Simplifying,

$$
=10-10.
$$

Therefore,

$$
(AA^{-1})_{21}=0.
$$

### Calculate the second row, second column

$$
(AA^{-1})_{22}
=
5(-1)+4\left(\frac{3}{2}\right).
$$

Simplifying,

$$
=-5+6.
$$

Therefore,

$$
(AA^{-1})_{22}=1.
$$

### Combine the Results

Substituting all calculated values into the product gives

$$
AA^{-1}=
\begin{pmatrix}
3(2)+2(-\frac{5}{2}) &
3(-1)+2(\frac{3}{2}) \\
5(2)+4(-\frac{5}{2}) &
5(-1)+4(\frac{3}{2})
\end{pmatrix}.
$$

After simplifying,

$$
AA^{-1}=
\begin{pmatrix}
6-5 & -3+3 \\
10-10 & -5+6
\end{pmatrix}.
$$

Therefore,

$$
AA^{-1}=
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}.
$$

Hence,

$$
\boxed{AA^{-1}=I}.
$$

The product is equal to the identity matrix, which confirms that our calculated inverse is correct.

## Step 7. Explain the Result

We have shown that

$$
\det(A)=2\neq 0.
$$

Therefore, matrix $A$ is invertible.

Using the inverse formula, we obtained

$$
A^{-1}=
\begin{pmatrix}
2 & -1 \\
-\frac{5}{2} & \frac{3}{2}
\end{pmatrix}.
$$

We then verified our result by computing

$$
AA^{-1}=I.
$$

This confirms that the matrix we calculated is indeed the inverse of $A$.

The determinant is important because it determines whether an inverse exists.

A nonzero determinant guarantees that a square matrix is invertible.

The verification step is also important because it confirms the correctness of the calculation using the definition of the inverse.

## Final Answer

For the matrix

$$
A=
\begin{pmatrix}
3 & 2 \\
5 & 4
\end{pmatrix},
$$

the determinant is

$$
\boxed{\det(A)=2}.
$$

Since the determinant is nonzero, the inverse exists.

Using the formula for a $2 \times 2$ matrix, we obtain

$$
\boxed{
A^{-1}=
\frac{1}{2}
\begin{pmatrix}
4 & -2 \\
-5 & 3
\end{pmatrix}
=
\begin{pmatrix}
2 & -1 \\
-\frac{5}{2} & \frac{3}{2}
\end{pmatrix}
}.
$$

Verification:

$$
\boxed{
AA^{-1}=
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
=I
}.
$$

**Conclusion:**

The inverse of matrix $A$ was successfully calculated using the standard $2 \times 2$ inverse formula.

The determinant was found to be nonzero, proving that the inverse exists.

Finally, multiplying the original matrix by its calculated inverse produced the identity matrix.

Therefore, the solution is mathematically verified and correct.
