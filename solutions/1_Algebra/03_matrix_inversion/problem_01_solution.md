
# Exercise 1. Definition of the Inverse — Detailed Solution

## Given Matrices

We are given the following two matrices:

$$
A=
\begin{pmatrix}
2 & 1 \\
1 & 1
\end{pmatrix},
\qquad
B=
\begin{pmatrix}
1 & -1 \\
-1 & 2
\end{pmatrix}.
$$

The task is to determine whether $B$ is the inverse of $A$ without using the formula for the inverse of a $2 \times 2$ matrix.

We must calculate both matrix products, $AB$ and $BA$, and compare them with the identity matrix.

## Step 1. Recall the Definition of an Inverse Matrix

For a square matrix $A$, its inverse is denoted by $A^{-1}$.

A matrix $B$ is the inverse of $A$ if and only if

$$
AB=BA=I,
$$

where $I$ is the identity matrix.

For a $2 \times 2$ matrix, the identity matrix is

$$
I=
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}.
$$

The identity matrix has the property that multiplying any compatible matrix by it does not change the original matrix.

In particular,

$$
AI=IA=A.
$$

Therefore, to verify that $B=A^{-1}$, we will calculate both $AB$ and $BA$.

If both products are equal to $I$, then $B$ is the inverse of $A$.

## Step 2. Calculate the Product $AB$

We begin by multiplying matrix $A$ by matrix $B$:

$$
AB=
\begin{pmatrix}
2 & 1 \\
1 & 1
\end{pmatrix}
\begin{pmatrix}
1 & -1 \\
-1 & 2
\end{pmatrix}.
$$

Matrix multiplication is performed by multiplying each row of the first matrix by each column of the second matrix and adding the corresponding products.

The resulting matrix will also have dimensions $2 \times 2$.

### Calculate the first row, first column

Multiply the first row of $A$ by the first column of $B$:

$$
(AB)_{11}=2(1)+1(-1).
$$

$$
(AB)_{11}=2-1=1.
$$

### Calculate the first row, second column

Multiply the first row of $A$ by the second column of $B$:

$$
(AB)_{12}=2(-1)+1(2).
$$

$$
(AB)_{12}=-2+2=0.
$$

### Calculate the second row, first column

Multiply the second row of $A$ by the first column of $B$:

$$
(AB)_{21}=1(1)+1(-1).
$$

$$
(AB)_{21}=1-1=0.
$$

### Calculate the second row, second column

Multiply the second row of $A$ by the second column of $B$:

$$
(AB)_{22}=1(-1)+1(2).
$$

$$
(AB)_{22}=-1+2=1.
$$

### Combine the results

Substituting the calculated elements into the resulting matrix gives

$$
AB=
\begin{pmatrix}
2(1)+1(-1) & 2(-1)+1(2) \\
1(1)+1(-1) & 1(-1)+1(2)
\end{pmatrix}.
$$

After simplifying,

$$
AB=
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}.
$$

Therefore,

$$
\boxed{AB=I}.
$$

The first condition for $B$ to be the inverse of $A$ is satisfied.

## Step 3. Calculate the Product $BA$

Next, we multiply matrix $B$ by matrix $A$ in the reverse order:

$$
BA=
\begin{pmatrix}
1 & -1 \\
-1 & 2
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
1 & 1
\end{pmatrix}.
$$

We use the same row-by-column multiplication method.

### Calculate the first row, first column

Multiply the first row of $B$ by the first column of $A$:

$$
(BA)_{11}=1(2)+(-1)(1).
$$

$$
(BA)_{11}=2-1=1.
$$

### Calculate the first row, second column

Multiply the first row of $B$ by the second column of $A$:

$$
(BA)_{12}=1(1)+(-1)(1).
$$

$$
(BA)_{12}=1-1=0.
$$

### Calculate the second row, first column

Multiply the second row of $B$ by the first column of $A$:

$$
(BA)_{21}=(-1)(2)+2(1).
$$

$$
(BA)_{21}=-2+2=0.
$$

### Calculate the second row, second column

Multiply the second row of $B$ by the second column of $A$:

$$
(BA)_{22}=(-1)(1)+2(1).
$$

$$
(BA)_{22}=-1+2=1.
$$

### Combine the results

Substituting the calculated values gives

$$
BA=
\begin{pmatrix}
1(2)+(-1)(1) & 1(1)+(-1)(1) \\
(-1)(2)+2(1) & (-1)(1)+2(1)
\end{pmatrix}.
$$

Simplifying each entry, we obtain

$$
BA=
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}.
$$

Therefore,

$$
\boxed{BA=I}.
$$

The second condition for $B$ to be the inverse of $A$ is also satisfied.

## Step 4. Compare Both Results with the Definition

From our calculations, we have obtained

$$
AB=
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
$$

and

$$
BA=
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}.
$$

Thus,

$$
AB=BA=I.
$$

According to the definition of an inverse matrix, this means that $A$ and $B$ are inverses of each other.

Consequently,

$$
B=A^{-1}.
$$

It also follows that

$$
A=B^{-1}.
$$

Both multiplication orders were checked because, in general, matrix multiplication is not commutative:

$$
AB \neq BA
$$

for arbitrary matrices.

However, when two square matrices are inverses of each other, multiplying them in either order produces the identity matrix.

## Final Answer

We have verified directly by matrix multiplication that

$$
AB=I
$$

and

$$
BA=I.
$$

Therefore,

$$
\boxed{
B=A^{-1}=
\begin{pmatrix}
1 & -1 \\
-1 & 2
\end{pmatrix}
}.
$$

**Conclusion:**

The matrix $B$ is the inverse of matrix $A$ because both $AB$ and $BA$ are equal to the $2 \times 2$ identity matrix.

This result follows directly from the definition of an inverse matrix, without using the inverse formula.

Hence, the statement $B=A^{-1}$ is **true**.
