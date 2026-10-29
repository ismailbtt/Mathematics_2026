
## Exercise 11: Shortening the Calculation with Row Operations

### Given Matrix

$$
A=
\begin{pmatrix}
1&2&3\\
1&3&4\\
1&4&6
\end{pmatrix}
$$

We need to calculate the determinant using row operations to create as many zeros as possible and explain which operations preserve the determinant.

### Step 1: Row Operation Property

An important determinant property states:

**Adding or subtracting a multiple of one row to another row does not change the determinant.**

In general:

$$
R_i\leftarrow R_i+kR_j
$$

This operation preserves the determinant.

We will use this property to transform the matrix into an upper triangular matrix.

### Step 2: Eliminate the First Entry of Row 2

Apply the row operation:

$$
R_2\leftarrow R_2-R_1
$$

Calculate the new second row:

$$
(1,3,4)-(1,2,3)=(0,1,1)
$$

The resulting matrix is:

$$
A_1=
\begin{pmatrix}
1&2&3\\
0&1&1\\
1&4&6
\end{pmatrix}
$$

This operation does not change the determinant.

Therefore:

$$
\det(A_1)=\det(A)
$$

### Step 3: Eliminate the First Entry of Row 3

Apply:

$$
R_3\leftarrow R_3-R_1
$$

Calculate:

$$
(1,4,6)-(1,2,3)=(0,2,3)
$$

The resulting matrix is:

$$
A_2=
\begin{pmatrix}
1&2&3\\
0&1&1\\
0&2&3
\end{pmatrix}
$$

This operation also preserves the determinant.

Therefore:

$$
\det(A_2)=\det(A_1)=\det(A)
$$

### Step 4: Eliminate the Second Entry of Row 3

Apply:

$$
R_3\leftarrow R_3-2R_2
$$

Calculate:

$$
(0,2,3)-2(0,1,1)=(0,0,1)
$$

The resulting matrix is:

$$
A_3=
\begin{pmatrix}
1&2&3\\
0&1&1\\
0&0&1
\end{pmatrix}
$$

This is now an upper triangular matrix.

The operation does not change the determinant.

Therefore:

$$
\det(A_3)=\det(A_2)=\det(A)
$$

### Step 5: Calculate the Determinant

For an upper triangular matrix, the determinant equals the product of the diagonal entries.

The diagonal entries are:

$$
1,\quad1,\quad1
$$

Therefore:

$$
\det(A_3)=1\cdot1\cdot1
$$

$$
\boxed{\det(A_3)=1}
$$

Since all row operations preserved the determinant:

$$
\boxed{\det(A)=1}
$$

### Step 6: Summary of Row Operations

| Step | Row Operation | Effect on Determinant |
|------|---------------|-----------------------|
| 1 | R₂ ← R₂ - R₁ | No change |
| 2 | R₃ ← R₃ - R₁ | No change |
| 3 | R₃ ← R₃ - 2R₂ | No change |

All three operations are of the form:

$$
R_i\leftarrow R_i+kR_j
$$

Such operations do not change the determinant.

Therefore:

$$
\det(A)=\det(A_1)=\det(A_2)=\det(A_3)=1
$$

### Step 7: Verification

We can verify the result using cofactor expansion along the first row.

$$
\det(A)=
1\begin{vmatrix}
3&4\\
4&6
\end{vmatrix}
-
2\begin{vmatrix}
1&4\\
1&6
\end{vmatrix}
+
3\begin{vmatrix}
1&3\\
1&4
\end{vmatrix}
$$

Calculate the first minor:

$$
3(6)-4(4)=18-16=2
$$

Calculate the second minor:

$$
1(6)-4(1)=6-4=2
$$

Calculate the third minor:

$$
1(4)-3(1)=4-3=1
$$

Substitute the results:

$$
\det(A)=1(2)-2(2)+3(1)
$$

$$
=2-4+3
$$

$$
\boxed{\det(A)=1}
$$

The verification matches the result obtained using row operations.

### Step 8: Explanation

Row operations make determinant calculations easier by creating zeros.

In this exercise, we used three row operations to transform the original matrix into an upper triangular matrix.

Since we only subtracted multiples of rows from other rows, the determinant remained unchanged.

For a triangular matrix, the determinant is simply the product of the diagonal entries.

This method avoids a lengthy determinant expansion.

### Final Answer

$$
\boxed{
\det\begin{pmatrix}
1&2&3\\
1&3&4\\
1&4&6
\end{pmatrix}=1
}
$$

**Conclusion:** By using determinant-preserving row operations, we transformed the matrix into an upper triangular matrix with diagonal entries 1, 1, and 1. Therefore, its determinant is 1. The result was verified using cofactor expansion.
