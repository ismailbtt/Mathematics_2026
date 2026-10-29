
## Exercise 10: Detecting Dependence

### Given Matrix

$$
A=
\begin{pmatrix}
1 & 2 & 3\\
2 & 4 & 6\\
0 & 1 & 5
\end{pmatrix}
$$

We need to explain why the determinant is zero without performing a full determinant calculation, identify the dependence between the rows, and explain why the matrix is not invertible.

### Step 1: Examine the Rows

The rows of matrix A are:

$$
R_1=(1,2,3)
$$

$$
R_2=(2,4,6)
$$

$$
R_3=(0,1,5)
$$

Observe that the second row is twice the first row.

$$
R_2=2R_1
$$

Verification:

$$
2(1,2,3)=(2,4,6)
$$

Therefore:

$$
\boxed{R_2=2R_1}
$$

### Step 2: Identify Linear Dependence

Two rows are linearly dependent when one row can be expressed as a scalar multiple of another row.

In this matrix:

$$
R_2-2R_1=(0,0,0)
$$

This is a nontrivial linear relationship between the rows.

Therefore, the rows of matrix A are linearly dependent.

### Step 3: Apply the Determinant Property

An important determinant property states:

**If two rows of a square matrix are linearly dependent, its determinant is zero.**

Since the second row is twice the first row:

$$
R_2=2R_1
$$

We immediately conclude:

$$
\boxed{\det(A)=0}
$$

No full determinant expansion is necessary.

### Step 4: Verification Using a Row Operation

We can verify the result using an elementary row operation.

Apply:

$$
R_2\leftarrow R_2-2R_1
$$

The resulting matrix is:

$$
A'=
\begin{pmatrix}
1 & 2 & 3\\
0 & 0 & 0\\
0 & 1 & 5
\end{pmatrix}
$$

Adding a multiple of one row to another does not change the determinant.

Therefore:

$$
\det(A')=\det(A)
$$

Since A' contains an entire row of zeros, its determinant must be zero.

Thus:

$$
\boxed{\det(A')=\det(A)=0}
$$

This confirms the result.

### Step 5: Connection with Invertibility

A square matrix is invertible if and only if its determinant is nonzero.

The condition is:

$$
\det(A)\neq0
$$

However, we found:

$$
\det(A)=0
$$

Therefore, matrix A is not invertible.

$$
\boxed{A^{-1}\text{ does not exist}}
$$

Such a matrix is called a singular matrix.

### Step 6: Explanation

The determinant provides information about whether the rows or columns of a square matrix are linearly independent.

If one row is a multiple of another row, the rows are linearly dependent.

This means that the matrix does not have full rank.

For this matrix:

$$
R_2=2R_1
$$

Therefore, the rows cannot all be linearly independent.

As a result:

- The determinant is zero.
- The matrix is singular.
- The matrix is not invertible.
- The matrix does not have full rank.

### Final Answer

The second row is twice the first row:

$$
\boxed{R_2=2R_1}
$$

Therefore, the rows are linearly dependent.

Using the determinant property:

$$
\boxed{
\det\begin{pmatrix}
1 & 2 & 3\\
2 & 4 & 6\\
0 & 1 & 5
\end{pmatrix}=0
}
$$

Since the determinant is zero:

$$
\boxed{A\text{ is not invertible}}
$$

**Conclusion:** The determinant is zero because the second row is a scalar multiple of the first row. This linear dependence makes the matrix singular and noninvertible. The result can be determined directly without a full determinant calculation.
