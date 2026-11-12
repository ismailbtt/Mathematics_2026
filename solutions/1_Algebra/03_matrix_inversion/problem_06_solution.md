
# Exercise 6. Solving a System Using the Inverse — Solution

## Given

We are given the matrix equation:

$$
Ax=b
$$

where

$$
A=
\begin{pmatrix}
2 & 1 \\
1 & 3
\end{pmatrix}
$$

and

$$
b=
\begin{pmatrix}
5 \\
7
\end{pmatrix}
$$

The task is to solve the system using the inverse matrix method:

$$
x=A^{-1}b
$$

We will then verify the solution by substituting it into the original equation.

## Step 1. Calculate the Determinant

For a general $2 \times 2$ matrix:

$$
A=
\begin{pmatrix}
a & b \\
c & d
\end{pmatrix}
$$

the determinant is:

$$
\det(A)=ad-bc
$$

For our matrix:

$$
\det(A)=(2)(3)-(1)(1)
$$

$$
\det(A)=6-1=5
$$

Since $\det(A)=5\neq 0$, the matrix is invertible.

Therefore, we can use the inverse matrix method.

## Step 2. Find the Inverse Matrix

The formula for the inverse of a $2 \times 2$ matrix is:

$$
A^{-1}=
\frac{1}{ad-bc}
\begin{pmatrix}
d & -b \\
-c & a
\end{pmatrix}
$$

Substituting the values:

$$
A^{-1}=
\frac{1}{5}
\begin{pmatrix}
3 & -1 \\
-1 & 2
\end{pmatrix}
$$

Therefore:

$$
A^{-1}=
\begin{pmatrix}
\frac{3}{5} & -\frac{1}{5} \\
-\frac{1}{5} & \frac{2}{5}
\end{pmatrix}
$$

## Step 3. Solve Using the Inverse Matrix

The original equation is:

$$
Ax=b
$$

Multiplying both sides by $A^{-1}$ from the left gives:

$$
A^{-1}Ax=A^{-1}b
$$

Since $A^{-1}A=I$, we obtain:

$$
Ix=A^{-1}b
$$

Therefore:

$$
x=A^{-1}b
$$

Substituting the matrices:

$$
x=
\frac{1}{5}
\begin{pmatrix}
3 & -1 \\
-1 & 2
\end{pmatrix}
\begin{pmatrix}
5 \\
7
\end{pmatrix}
$$

Performing matrix multiplication:

$$
x=
\frac{1}{5}
\begin{pmatrix}
3(5)+(-1)(7) \\
(-1)(5)+2(7)
\end{pmatrix}
$$

Simplifying:

$$
x=
\frac{1}{5}
\begin{pmatrix}
15-7 \\
-5+14
\end{pmatrix}
$$

$$
x=
\frac{1}{5}
\begin{pmatrix}
8 \\
9
\end{pmatrix}
$$

Thus:

$$
x=
\begin{pmatrix}
\frac{8}{5} \\
\frac{9}{5}
\end{pmatrix}
$$

The solution is:

$$
x_1=\frac{8}{5}, \qquad x_2=\frac{9}{5}
$$

## Step 4. Verify the Solution

To verify the result, we substitute the calculated vector into the original equation:

$$
Ax=b
$$

We have:

$$
A=
\begin{pmatrix}
2 & 1 \\
1 & 3
\end{pmatrix}
$$

and

$$
x=
\begin{pmatrix}
\frac{8}{5} \\
\frac{9}{5}
\end{pmatrix}
$$

Calculate the product:

$$
Ax=
\begin{pmatrix}
2 & 1 \\
1 & 3
\end{pmatrix}
\begin{pmatrix}
\frac{8}{5} \\
\frac{9}{5}
\end{pmatrix}
$$

Performing matrix multiplication:

$$
Ax=
\begin{pmatrix}
2\left(\frac{8}{5}\right)+\frac{9}{5} \\
\frac{8}{5}+3\left(\frac{9}{5}\right)
\end{pmatrix}
$$

Simplifying:

$$
Ax=
\begin{pmatrix}
\frac{16}{5}+\frac{9}{5} \\
\frac{8}{5}+\frac{27}{5}
\end{pmatrix}
$$

$$
Ax=
\begin{pmatrix}
\frac{25}{5} \\
\frac{35}{5}
\end{pmatrix}
$$

Therefore:

$$
Ax=
\begin{pmatrix}
5 \\
7
\end{pmatrix}
=b
$$

The calculated vector satisfies the original equation.

## Final Answer

The inverse matrix is:

$$
A^{-1}=
\frac{1}{5}
\begin{pmatrix}
3 & -1 \\
-1 & 2
\end{pmatrix}
$$

Using $x=A^{-1}b$, we obtain:

$$
\boxed{
x=
\begin{pmatrix}
\frac{8}{5} \\
\frac{9}{5}
\end{pmatrix}
}
$$

**Verification:**

$$
Ax=
\begin{pmatrix}
5 \\
7
\end{pmatrix}
=b
$$

**Conclusion:**

The system was successfully solved using the inverse matrix method.

Since the determinant is nonzero, the inverse exists and the system has a unique solution.

Substituting the calculated vector into the original equation gives the correct right-hand side.

Therefore, the solution is verified.
