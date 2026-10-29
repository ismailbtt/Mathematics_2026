
## Exercise 13: Determinant by Elimination

### Given Matrix

$$
A=
\begin{pmatrix}
1&2&3\\
2&5&7\\
1&0&2
\end{pmatrix}
$$

We need to calculate the determinant using Gaussian elimination and record how each row operation affects the determinant.

### Step 1: Recall the Row Operation Properties

There are three elementary row operations:

1. Swapping two rows changes the sign of the determinant.
2. Multiplying a row by a nonzero scalar multiplies the determinant by that scalar.
3. Adding a multiple of one row to another row does not change the determinant.

We will use the third property to transform the matrix into an upper triangular matrix.

### Step 2: Eliminate the First Entry of Row 2

Apply:

$$
R_2\leftarrow R_2-2R_1
$$

Calculate the new second row:

$$
(2,5,7)-2(1,2,3)
$$

$$
=(2-2,\ 5-4,\ 7-6)
$$

$$
=(0,1,1)
$$

The resulting matrix is:

$$
A_1=
\begin{pmatrix}
1&2&3\\
0&1&1\\
1&0&2
\end{pmatrix}
$$

**Effect on the determinant:**

Subtracting a multiple of one row from another does not change the determinant.

Therefore:

$$
\boxed{\det(A_1)=\det(A)}
$$

### Step 3: Eliminate the First Entry of Row 3

Apply:

$$
R_3\leftarrow R_3-R_1
$$

Calculate the new third row:

$$
(1,0,2)-(1,2,3)
$$

$$
=(1-1,\ 0-2,\ 2-3)
$$

$$
=(0,-2,-1)
$$

The resulting matrix is:

$$
A_2=
\begin{pmatrix}
1&2&3\\
0&1&1\\
0&-2&-1
\end{pmatrix}
$$

**Effect on the determinant:**

This operation does not change the determinant.

Therefore:

$$
\boxed{\det(A_2)=\det(A_1)=\det(A)}
$$

### Step 4: Eliminate the Second Entry of Row 3

Apply:

$$
R_3\leftarrow R_3+2R_2
$$

Calculate the new third row:

$$
(0,-2,-1)+2(0,1,1)
$$

$$
=(0,-2,-1)+(0,2,2)
$$

$$
=(0,0,1)
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

**Effect on the determinant:**

Adding a multiple of one row to another does not change the determinant.

Therefore:

$$
\boxed{\det(A_3)=\det(A_2)=\det(A)}
$$

### Step 5: Calculate the Determinant

The resulting matrix is upper triangular:

$$
A_3=
\begin{pmatrix}
1&2&3\\
0&1&1\\
0&0&1
\end{pmatrix}
$$

For a triangular matrix, the determinant equals the product of its diagonal entries.

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
| 1 | R₂ ← R₂ - 2R₁ | No change |
| 2 | R₃ ← R₃ - R₁ | No change |
| 3 | R₃ ← R₃ + 2R₂ | No change |

All operations are of the form:

$$
R_i\leftarrow R_i+kR_j
$$

Therefore:

$$
\det(A)=\det(A_1)=\det(A_2)=\det(A_3)
$$

No row swaps or row scaling operations were necessary.

### Step 7: Verification

We can verify the result using cofactor expansion along the first row.

$$
\det(A)=
1\begin{vmatrix}
5&7\\
0&2
\end{vmatrix}
-
2\begin{vmatrix}
2&7\\
1&2
\end{vmatrix}
+
3\begin{vmatrix}
2&5\\
1&0
\end{vmatrix}
$$

Calculate the first minor:

$$
5(2)-7(0)=10
$$

Calculate the second minor:

$$
2(2)-7(1)=4-7=-3
$$

Calculate the third minor:

$$
2(0)-5(1)=-5
$$

Substitute the results:

$$
\det(A)=1(10)-2(-3)+3(-5)
$$

Simplifying:

$$
\det(A)=10+6-15
$$

$$
\boxed{\det(A)=1}
$$

The verification matches the result obtained using elimination.

### Step 8: Explanation

Gaussian elimination simplifies determinant calculations by creating zeros below the main diagonal.

In this exercise, we used three elementary row operations to transform the original matrix into an upper triangular matrix.

Each operation involved adding or subtracting a multiple of one row from another, so the determinant remained unchanged.

Once the matrix became upper triangular, we calculated the determinant by multiplying its diagonal entries.

Because the determinant is nonzero, the matrix is also invertible.

### Final Answer

$$
\boxed{
\det\begin{pmatrix}
1&2&3\\
2&5&7\\
1&0&2
\end{pmatrix}=1
}
$$

**Conclusion:** Using Gaussian elimination, we transformed the matrix into an upper triangular matrix with diagonal entries 1, 1, and 1. All three row operations preserved the determinant. Therefore, the determinant is 1, which was also confirmed using cofactor expansion.
