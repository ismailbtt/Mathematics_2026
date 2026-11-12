
# Exercise 5. A 3×3 Matrix — Solution

## Given Matrix

We are given the following matrix:

$$
A=
\begin{pmatrix}
1 & 1 & 0 \\
0 & 1 & 1 \\
1 & 0 & 1
\end{pmatrix}
$$

The task is to find the inverse of matrix $A$ using the Gauss–Jordan elimination method and verify the result by multiplication.

## Step 1. Construct the Augmented Matrix

We begin by writing the augmented matrix $[A \mid I]$, where $I$ is the $3 \times 3$ identity matrix.

$$
I=
\begin{pmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{pmatrix}
$$

The augmented matrix is:

$$
[A \mid I]=
\left[
\begin{array}{ccc|ccc}
1 & 1 & 0 & 1 & 0 & 0 \\
0 & 1 & 1 & 0 & 1 & 0 \\
1 & 0 & 1 & 0 & 0 & 1
\end{array}
\right]
$$

Our goal is to transform the left side into the identity matrix using elementary row operations.

## Step 2. Eliminate the Element Below the First Pivot

The first pivot is $1$ in the first row.

We eliminate the element $1$ in the third row, first column.

Apply the row operation:

$$
R_3 \rightarrow R_3-R_1
$$

Calculate the new third row:

$$
R_3=(1,0,1,0,0,1)-(1,1,0,1,0,0)
$$

$$
R_3=(0,-1,1,-1,0,1)
$$

The augmented matrix becomes:

$$
\left[
\begin{array}{ccc|ccc}
1 & 1 & 0 & 1 & 0 & 0 \\
0 & 1 & 1 & 0 & 1 & 0 \\
0 & -1 & 1 & -1 & 0 & 1
\end{array}
\right]
$$

The elements below the first pivot are now zero.

## Step 3. Eliminate the Element Below the Second Pivot

The second pivot is $1$ in the second row.

We need to eliminate the element $-1$ in the third row, second column.

Apply:

$$
R_3 \rightarrow R_3+R_2
$$

Calculate the new third row:

$$
R_3=(0,-1,1,-1,0,1)+(0,1,1,0,1,0)
$$

$$
R_3=(0,0,2,-1,1,1)
$$

The augmented matrix becomes:

$$
\left[
\begin{array}{ccc|ccc}
1 & 1 & 0 & 1 & 0 & 0 \\
0 & 1 & 1 & 0 & 1 & 0 \\
0 & 0 & 2 & -1 & 1 & 1
\end{array}
\right]
$$

The matrix is now in upper triangular form on the left side.

## Step 4. Make the Third Pivot Equal to 1

The third pivot is currently $2$.

To make it equal to $1$, divide the third row by $2$.

Apply:

$$
R_3 \rightarrow \frac{1}{2}R_3
$$

The new third row becomes:

$$
R_3=
\left(
0,0,1,-\frac{1}{2},\frac{1}{2},\frac{1}{2}
\right)
$$

The augmented matrix is now:

$$
\left[
\begin{array}{ccc|ccc}
1 & 1 & 0 & 1 & 0 & 0 \\
0 & 1 & 1 & 0 & 1 & 0 \\
0 & 0 & 1 & -\frac{1}{2} & \frac{1}{2} & \frac{1}{2}
\end{array}
\right]
$$

All three diagonal elements on the left side are now equal to $1$.

## Step 5. Eliminate the Element Above the Third Pivot

We eliminate the element $1$ in the second row, third column.

Apply:

$$
R_2 \rightarrow R_2-R_3
$$

Calculate the new second row:

$$
R_2=(0,1,1,0,1,0)
-
\left(
0,0,1,-\frac{1}{2},\frac{1}{2},\frac{1}{2}
\right)
$$

Therefore:

$$
R_2=
\left(
0,1,0,\frac{1}{2},\frac{1}{2},-\frac{1}{2}
\right)
$$

The augmented matrix becomes:

$$
\left[
\begin{array}{ccc|ccc}
1 & 1 & 0 & 1 & 0 & 0 \\
0 & 1 & 0 & \frac{1}{2} & \frac{1}{2} & -\frac{1}{2} \\
0 & 0 & 1 & -\frac{1}{2} & \frac{1}{2} & \frac{1}{2}
\end{array}
\right]
$$

## Step 6. Eliminate the Element Above the Second Pivot

The remaining nonzero element outside the main diagonal is $1$ in the first row, second column.

Apply:

$$
R_1 \rightarrow R_1-R_2
$$

Calculate the new first row:

$$
R_1=(1,1,0,1,0,0)
-
\left(
0,1,0,\frac{1}{2},\frac{1}{2},-\frac{1}{2}
\right)
$$

Therefore:

$$
R_1=
\left(
1,0,0,\frac{1}{2},-\frac{1}{2},\frac{1}{2}
\right)
$$

The final augmented matrix becomes:

$$
\left[
\begin{array}{ccc|ccc}
1 & 0 & 0 & \frac{1}{2} & -\frac{1}{2} & \frac{1}{2} \\
0 & 1 & 0 & \frac{1}{2} & \frac{1}{2} & -\frac{1}{2} \\
0 & 0 & 1 & -\frac{1}{2} & \frac{1}{2} & \frac{1}{2}
\end{array}
\right]
$$

The left side is now the identity matrix.

Therefore, the Gauss–Jordan elimination process is complete.

## Step 7. Identify the Inverse Matrix

The final augmented matrix has the form:

$$
[I \mid A^{-1}]
$$

The right side gives the inverse matrix:

$$
A^{-1}=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} & \frac{1}{2} \\
\frac{1}{2} & \frac{1}{2} & -\frac{1}{2} \\
-\frac{1}{2} & \frac{1}{2} & \frac{1}{2}
\end{pmatrix}
$$

We can also write:

$$
A^{-1}=
\frac{1}{2}
\begin{pmatrix}
1 & -1 & 1 \\
1 & 1 & -1 \\
-1 & 1 & 1
\end{pmatrix}
$$

## Step 8. Verify the Result by Multiplication

To verify the inverse, we calculate:

$$
AA^{-1}=I
$$

Substituting the matrices:

$$
AA^{-1}=
\begin{pmatrix}
1 & 1 & 0 \\
0 & 1 & 1 \\
1 & 0 & 1
\end{pmatrix}
\frac{1}{2}
\begin{pmatrix}
1 & -1 & 1 \\
1 & 1 & -1 \\
-1 & 1 & 1
\end{pmatrix}
$$

Performing matrix multiplication:

$$
AA^{-1}=
\frac{1}{2}
\begin{pmatrix}
1+1+0 & -1+1+0 & 1-1+0 \\
0+1-1 & 0+1+1 & 0-1+1 \\
1+0-1 & -1+0+1 & 1+0+1
\end{pmatrix}
$$

Simplifying:

$$
AA^{-1}=
\frac{1}{2}
\begin{pmatrix}
2 & 0 & 0 \\
0 & 2 & 0 \\
0 & 0 & 2
\end{pmatrix}
$$

Therefore:

$$
AA^{-1}=
\begin{pmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{pmatrix}
=I
$$

Since the product equals the identity matrix, our inverse is correct.

## Step 9. Explain Why the Method Works

The Gauss–Jordan method transforms the original matrix into the identity matrix using elementary row operations.

Each row operation is equivalent to multiplication by an invertible elementary matrix.

When the combined row operations transform $A$ into $I$, the same operations transform the identity matrix into $A^{-1}$.

Therefore:

$$
[A \mid I]
\longrightarrow
[I \mid A^{-1}]
$$

This explains why obtaining the identity matrix on the left produces the inverse matrix on the right.

## Final Answer

The Gauss–Jordan row operations were:

$$
R_3 \rightarrow R_3-R_1
$$

$$
R_3 \rightarrow R_3+R_2
$$

$$
R_3 \rightarrow \frac{1}{2}R_3
$$

$$
R_2 \rightarrow R_2-R_3
$$

$$
R_1 \rightarrow R_1-R_2
$$

After applying these operations, we obtained the inverse:

$$
A^{-1}=
\frac{1}{2}
\begin{pmatrix}
1 & -1 & 1 \\
1 & 1 & -1 \\
-1 & 1 & 1
\end{pmatrix}
$$

**Verification:**

$$
AA^{-1}=
\begin{pmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{pmatrix}
=I
$$

**Conclusion:**

The inverse of the given $3 \times 3$ matrix was successfully calculated using Gauss–Jordan elimination.

All elementary row operations were applied to the augmented matrix until the left side became the identity matrix.

The resulting inverse was verified by multiplication, confirming that the solution is correct.
