
## Exercise 1: Determinant of a 2×2 Matrix

### Given Matrices

```math
A=\begin{pmatrix}
3 & -2\\
5 & 4
\end{pmatrix}
```

```math
B=\begin{pmatrix}
1 & 7\\
2 & 14
\end{pmatrix}
```

We need to calculate the determinants of both matrices and determine which matrix is invertible.

### Step 1: Determinant Formula

For a 2×2 matrix:

```math
M=\begin{pmatrix}
a & b\\
c & d
\end{pmatrix}
```

The determinant is calculated using:

```math
\det(M)=ad-bc
```

### Step 2: Calculate det(A)

```math
\det(A)=
\begin{vmatrix}
3 & -2\\
5 & 4
\end{vmatrix}
```

Using the formula:

```math
\det(A)=3(4)-(-2)(5)
```

```math
=12+10
```

Therefore:

```math
\boxed{\det(A)=22}
```

### Step 3: Calculate det(B)

```math
\det(B)=
\begin{vmatrix}
1 & 7\\
2 & 14
\end{vmatrix}
```

Using the formula:

```math
\det(B)=1(14)-7(2)
```

```math
=14-14
```

Therefore:

```math
\boxed{\det(B)=0}
```

### Step 4: Determine Invertibility

A square matrix is invertible if and only if its determinant is not zero.

For matrix A:

```math
\det(A)=22\neq0
```

Therefore, matrix A is invertible.

For matrix B:

```math
\det(B)=0
```

Therefore, matrix B is not invertible.

### Step 5: Verification

We can verify that matrix B is not invertible by examining its rows.

The second row is twice the first row:

```math
(2,14)=2(1,7)
```

This means the rows are linearly dependent, so the determinant must be zero.

For matrix A, we can also verify invertibility using the inverse formula:

```math
A^{-1}=
\frac{1}{22}
\begin{pmatrix}
4 & 2\\
-5 & 3
\end{pmatrix}
```

Multiplying A by its inverse gives:

```math
AA^{-1}=
\begin{pmatrix}
1 & 0\\
0 & 1
\end{pmatrix}
```

This confirms that A is invertible.

### Final Answer

```math
\boxed{\det(A)=22}
```

```math
\boxed{\det(B)=0}
```

**Conclusion:**

Matrix A is invertible because its determinant is nonzero.

Matrix B is not invertible because its determinant is zero and its rows are linearly dependent.
