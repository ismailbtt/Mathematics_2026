
## Exercise 5: Row Operations

### Given Matrix

```math
A=
\begin{pmatrix}
1&2&3\\
2&1&0\\
-1&4&2
\end{pmatrix}
```

We need to calculate the determinant of matrix A using row operations and explain how each operation affects the determinant.

### Step 1: Row Operation Rules

There are three elementary row operations:

1. Swapping two rows changes the sign of the determinant.
2. Multiplying a row by a nonzero number multiplies the determinant by that number.
3. Adding a multiple of one row to another row does not change the determinant.

We will use the third operation to simplify the matrix.

### Step 2: Eliminate the First Entry of Row 2

Apply:

```math
R_2\leftarrow R_2-2R_1
```

Calculate the new second row:

```math
(2,1,0)-2(1,2,3)=(0,-3,-6)
```

The resulting matrix is:

```math
A_1=
\begin{pmatrix}
1&2&3\\
0&-3&-6\\
-1&4&2
\end{pmatrix}
```

Adding a multiple of one row to another does not change the determinant.

Therefore:

```math
\det(A_1)=\det(A)
```

### Step 3: Eliminate the First Entry of Row 3

Apply:

```math
R_3\leftarrow R_3+R_1
```

Calculate the new third row:

```math
(-1,4,2)+(1,2,3)=(0,6,5)
```

The resulting matrix is:

```math
A_2=
\begin{pmatrix}
1&2&3\\
0&-3&-6\\
0&6&5
\end{pmatrix}
```

This operation also does not change the determinant.

Therefore:

```math
\det(A_2)=\det(A_1)=\det(A)
```

### Step 4: Eliminate the Second Entry of Row 3

Apply:

```math
R_3\leftarrow R_3+2R_2
```

Calculate:

```math
(0,6,5)+2(0,-3,-6)=(0,0,-7)
```

The resulting matrix is:

```math
A_3=
\begin{pmatrix}
1&2&3\\
0&-3&-6\\
0&0&-7
\end{pmatrix}
```

Again, adding a multiple of one row to another does not change the determinant.

Therefore:

```math
\det(A_3)=\det(A_2)=\det(A)
```

### Step 5: Calculate the Determinant

The resulting matrix is upper triangular.

For a triangular matrix, the determinant is the product of its diagonal entries.

```math
\det(A_3)=1\cdot(-3)\cdot(-7)
```

```math
\det(A_3)=21
```

Since none of the row operations changed the determinant:

```math
\boxed{\det(A)=21}
```

### Step 6: Summary of Row Operations

| Step | Row Operation | Effect on Determinant |
|------|---------------|-----------------------|
| 1 | R₂ ← R₂ - 2R₁ | No change |
| 2 | R₃ ← R₃ + R₁ | No change |
| 3 | R₃ ← R₃ + 2R₂ | No change |

All three operations preserve the determinant.

Therefore:

```math
\det(A)=\det(A_1)=\det(A_2)=\det(A_3)=21
```

### Step 7: Verification

We can verify the result using cofactor expansion along the first row.

```math
\det(A)=
1\begin{vmatrix}
1&0\\
4&2
\end{vmatrix}
-
2\begin{vmatrix}
2&0\\
-1&2
\end{vmatrix}
+
3\begin{vmatrix}
2&1\\
-1&4
\end{vmatrix}
```

Calculate each minor:

```math
1(1\cdot2-0\cdot4)=2
```

```math
-2(2\cdot2-0\cdot(-1))=-8
```

```math
3(2\cdot4-1\cdot(-1))=27
```

Add the results:

```math
\det(A)=2-8+27
```

```math
\boxed{\det(A)=21}
```

The verification gives the same result as row elimination.

### Final Answer

```math
\boxed{
\det\begin{pmatrix}
1&2&3\\
2&1&0\\
-1&4&2
\end{pmatrix}=21
}
```

**Conclusion:** By applying three determinant-preserving row operations, we transformed the original matrix into an upper triangular matrix. The product of the diagonal entries is 21. This result was also verified using cofactor expansion.
