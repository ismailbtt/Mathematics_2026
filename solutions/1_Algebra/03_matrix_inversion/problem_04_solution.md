
# Exercise 4. Gauss–Jordan Method — Solution

## Given Matrix

We are given the matrix:

$$
A=
\begin{pmatrix}
1 & 2 \\
3 & 5
\end{pmatrix}
$$

The task is to find the inverse of matrix $A$ using the Gauss–Jordan elimination method.

We must show the augmented matrix after each row operation and explain why obtaining the identity matrix on the left gives the inverse matrix on the right.

## Step 1. Construct the Augmented Matrix

The Gauss–Jordan method begins by combining matrix $A$ with the identity matrix $I$.

The identity matrix is:

$$
I=
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
$$

We construct the augmented matrix $[A \mid I]$:

$$
[A \mid I]=
\left[
\begin{array}{cc|cc}
1 & 2 & 1 & 0 \\
3 & 5 & 0 & 1
\end{array}
\right]
$$

Our goal is to transform the left side into the identity matrix using elementary row operations.

The right side will then contain the inverse of $A$.

## Step 2. Eliminate the Element Below the First Pivot

The first pivot is $1$ in the first row.

We want to eliminate the element $3$ below this pivot.

Apply the row operation:

$$
R_2 \rightarrow R_2-3R_1
$$

Calculate the new second row:

$$
R_2=(3,5,0,1)-3(1,2,1,0)
$$

$$
R_2=(3,5,0,1)-(3,6,3,0)
$$

$$
R_2=(0,-1,-3,1)
$$

The augmented matrix becomes:

$$
\left[
\begin{array}{cc|cc}
1 & 2 & 1 & 0 \\
0 & -1 & -3 & 1
\end{array}
\right]
$$

The element below the first pivot is now zero.

## Step 3. Make the Second Pivot Equal to 1

The second pivot is currently $-1$.

To make it equal to $1$, multiply the second row by $-1$.

Apply:

$$
R_2 \rightarrow -R_2
$$

The new second row is:

$$
R_2=(0,1,3,-1)
$$

The augmented matrix becomes:

$$
\left[
\begin{array}{cc|cc}
1 & 2 & 1 & 0 \\
0 & 1 & 3 & -1
\end{array}
\right]
$$

Now both pivot elements are equal to $1$.

## Step 4. Eliminate the Element Above the Second Pivot

We need to eliminate the element $2$ in the first row, second column.

Apply the row operation:

$$
R_1 \rightarrow R_1-2R_2
$$

Calculate the new first row:

$$
R_1=(1,2,1,0)-2(0,1,3,-1)
$$

$$
R_1=(1,2,1,0)-(0,2,6,-2)
$$

$$
R_1=(1,0,-5,2)
$$

The augmented matrix becomes:

$$
\left[
\begin{array}{cc|cc}
1 & 0 & -5 & 2 \\
0 & 1 & 3 & -1
\end{array}
\right]
$$

The left side is now the identity matrix.

Therefore, the Gauss–Jordan elimination process is complete.

## Step 5. Identify the Inverse Matrix

The final augmented matrix is:

$$
[I \mid A^{-1}]=
\left[
\begin{array}{cc|cc}
1 & 0 & -5 & 2 \\
0 & 1 & 3 & -1
\end{array}
\right]
$$

The left side contains the identity matrix, while the right side contains the inverse.

Therefore:

$$
A^{-1}=
\begin{pmatrix}
-5 & 2 \\
3 & -1
\end{pmatrix}
$$

## Step 6. Verify the Result

To check our answer, we multiply the original matrix by its inverse.

The definition of an inverse requires:

$$
AA^{-1}=I
$$

Substituting the matrices:

$$
AA^{-1}=
\begin{pmatrix}
1 & 2 \\
3 & 5
\end{pmatrix}
\begin{pmatrix}
-5 & 2 \\
3 & -1
\end{pmatrix}
$$

Performing matrix multiplication:

$$
AA^{-1}=
\begin{pmatrix}
1(-5)+2(3) & 1(2)+2(-1) \\
3(-5)+5(3) & 3(2)+5(-1)
\end{pmatrix}
$$

Simplifying:

$$
AA^{-1}=
\begin{pmatrix}
-5+6 & 2-2 \\
-15+15 & 6-5
\end{pmatrix}
$$

Therefore:

$$
AA^{-1}=
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
=I
$$

Since the product equals the identity matrix, the calculated inverse is correct.

## Step 7. Explain Why the Method Works

The Gauss–Jordan method uses elementary row operations to transform the original matrix into the identity matrix.

Each elementary row operation is reversible and corresponds to multiplication by an invertible elementary matrix.

If the combined effect of these operations is represented by a matrix $E$, then transforming $A$ into $I$ means:

$$
EA=I
$$

Therefore:

$$
E=A^{-1}
$$

Because the same row operations are applied to the identity matrix on the right side, it becomes:

$$
EI=E=A^{-1}
$$

This explains why the inverse appears on the right side when the left side becomes the identity matrix.

## Final Answer

Using Gauss–Jordan elimination, we obtained:

$$
\left[
\begin{array}{cc|cc}
1 & 2 & 1 & 0 \\
3 & 5 & 0 & 1
\end{array}
\right]
$$

After applying the row operations:

$$
R_2 \rightarrow R_2-3R_1
$$

$$
R_2 \rightarrow -R_2
$$

$$
R_1 \rightarrow R_1-2R_2
$$

We obtained:

$$
\left[
\begin{array}{cc|cc}
1 & 0 & -5 & 2 \\
0 & 1 & 3 & -1
\end{array}
\right]
$$

Thus, the inverse matrix is:

$$
\boxed{
A^{-1}=
\begin{pmatrix}
-5 & 2 \\
3 & -1
\end{pmatrix}
}
$$

**Conclusion:**

The Gauss–Jordan elimination method successfully transformed the original matrix into the identity matrix.

The same row operations transformed the identity matrix on the right into the inverse matrix.

Finally, the result was verified by multiplication:

$$
AA^{-1}=I
$$

Therefore, the calculated inverse is correct.
