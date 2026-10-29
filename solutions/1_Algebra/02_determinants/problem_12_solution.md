
## Exercise 12: A Parameter Revealed by a Row Operation

### Given Matrix

$$
A(t)=
\begin{pmatrix}
1&2&3\\
2&4&t\\
0&1&1
\end{pmatrix}
$$

We need to find all values of t for which the matrix is not invertible.

Before calculating the determinant, we will perform the given row operation and examine the resulting matrix.

### Step 1: Apply the Row Operation

The required operation is:

$$
R_2\leftarrow R_2-2R_1
$$

Calculate the new second row:

$$
(2,4,t)-2(1,2,3)
$$

$$
=(2-2,\ 4-4,\ t-6)
$$

$$
=(0,0,t-6)
$$

The resulting matrix is:

$$
A_1(t)=
\begin{pmatrix}
1&2&3\\
0&0&t-6\\
0&1&1
\end{pmatrix}
$$

### Step 2: Effect on the Determinant

Adding a multiple of one row to another row does not change the determinant.

Therefore:

$$
\det(A_1(t))=\det(A(t))
$$

We can calculate the determinant using the simplified matrix.

### Step 3: Calculate the Determinant

Expand along the second row, which contains two zeros.

The only nonzero entry in this row is:

$$
a_{23}=t-6
$$

The cofactor sign at position (2,3) is:

$$
(-1)^{2+3}=-1
$$

Therefore:

$$
\det(A(t))=
-(t-6)
\begin{vmatrix}
1&2\\
0&1
\end{vmatrix}
$$

Calculate the 2×2 determinant:

$$
\begin{vmatrix}
1&2\\
0&1
\end{vmatrix}
=1(1)-2(0)=1
$$

Substituting:

$$
\det(A(t))=-(t-6)(1)
$$

Therefore:

$$
\boxed{\det(A(t))=6-t}
$$

### Step 4: Find the Value of t

A square matrix is not invertible when its determinant equals zero.

Therefore:

$$
\det(A(t))=0
$$

Substitute the determinant:

$$
6-t=0
$$

Solving:

$$
\boxed{t=6}
$$

Thus, matrix A(t) is not invertible when t = 6.

### Step 5: Explain the Dependence Between Rows

Substitute t = 6 into the original matrix:

$$
A(6)=
\begin{pmatrix}
1&2&3\\
2&4&6\\
0&1&1
\end{pmatrix}
$$

The first row is:

$$
R_1=(1,2,3)
$$

The second row is:

$$
R_2=(2,4,6)
$$

Notice that:

$$
R_2=2R_1
$$

Therefore, the first and second rows are linearly dependent.

When we apply the row operation:

$$
R_2\leftarrow R_2-2R_1
$$

The second row becomes:

$$
R_2=(0,0,0)
$$

The resulting matrix is:

$$
\begin{pmatrix}
1&2&3\\
0&0&0\\
0&1&1
\end{pmatrix}
$$

A matrix containing a zero row has determinant zero.

Therefore, A(6) is not invertible.

### Step 6: Verification

We can verify the result using direct cofactor expansion of the original matrix.

$$
\det(A(t))=
1\begin{vmatrix}
4&t\\
1&1
\end{vmatrix}
-
2\begin{vmatrix}
2&t\\
0&1
\end{vmatrix}
+
3\begin{vmatrix}
2&4\\
0&1
\end{vmatrix}
$$

Calculate each minor:

$$
4(1)-t(1)=4-t
$$

$$
2(1)-t(0)=2
$$

$$
2(1)-4(0)=2
$$

Substitute:

$$
\det(A(t))=(4-t)-2(2)+3(2)
$$

Simplifying:

$$
=4-t-4+6
$$

$$
\boxed{\det(A(t))=6-t}
$$

This matches the result obtained using row operations.

For t = 6:

$$
\det(A(6))=6-6=0
$$

The result is verified.

### Step 7: Explanation

The determinant determines whether a square matrix is invertible.

If the determinant is zero, the matrix is singular and does not have an inverse.

In this exercise, applying the row operation created two zeros in the second row, making the determinant easier to calculate.

When t = 6, the entire second row becomes zero because the original second row is twice the first row.

This linear dependence explains why the determinant is zero.

### Final Answer

The determinant is:

$$
\boxed{\det(A(t))=6-t}
$$

The matrix is not invertible when:

$$
\boxed{t=6}
$$

For all other real values of t:

$$
\boxed{t\neq6}
$$

the matrix is invertible.

**Conclusion:** The matrix A(t) is singular only when t = 6. At this value, the second row is twice the first row, making the rows linearly dependent and the determinant equal to zero.
