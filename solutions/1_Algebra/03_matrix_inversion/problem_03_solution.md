
# Exercise 3. When Does the Inverse Not Exist? — Detailed Solution

## Given Matrix

We are given the following matrix:

$$
A=
\begin{pmatrix}
2 & 4 \\
1 & 2
\end{pmatrix}.
$$

The task is to explain why the inverse matrix $A^{-1}$ does not exist.

We must demonstrate this using two different methods:

1. By calculating the determinant of matrix $A$.
2. By examining the linear dependence between the rows of matrix $A$.

Both methods will show that matrix $A$ is singular, meaning that it is not invertible.

## Step 1. Recall the Condition for Invertibility

A square matrix $A$ is invertible if there exists another matrix $A^{-1}$ such that

$$
AA^{-1}=A^{-1}A=I,
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

An important property of square matrices states that a matrix is invertible if and only if its determinant is nonzero.

Mathematically,

$$
A^{-1}\text{ exists}
\iff
\det(A)\neq 0.
$$

Conversely,

$$
\det(A)=0
\implies
A^{-1}\text{ does not exist}.
$$

Another important condition is that the rows and columns of an invertible matrix must be linearly independent.

If one row can be expressed as a linear combination of the other rows, the matrix is not invertible.

We will now apply these two conditions to the given matrix.

---

## Method 1. Using the Determinant

### Step 2. Recall the Determinant Formula

For a general $2 \times 2$ matrix

$$
A=
\begin{pmatrix}
a & b \\
c & d
\end{pmatrix},
$$

the determinant is calculated using the formula

$$
\det(A)=ad-bc.
$$

The determinant helps us determine whether a square matrix has an inverse.

If

$$
\det(A)\neq 0,
$$

the matrix is invertible.

However, if

$$
\det(A)=0,
$$

the matrix is singular and its inverse does not exist.

### Step 3. Identify the Matrix Elements

The given matrix is

$$
A=
\begin{pmatrix}
2 & 4 \\
1 & 2
\end{pmatrix}.
$$

Comparing it with the general form

$$
A=
\begin{pmatrix}
a & b \\
c & d
\end{pmatrix},
$$

we identify

$$
a=2,\qquad b=4,
$$

$$
c=1,\qquad d=2.
$$

We substitute these values into the determinant formula.

### Step 4. Calculate the Determinant

Using

$$
\det(A)=ad-bc,
$$

we obtain

$$
\det(A)=(2)(2)-(4)(1).
$$

First, calculate the individual products:

$$
(2)(2)=4
$$

and

$$
(4)(1)=4.
$$

Therefore,

$$
\det(A)=4-4.
$$

Hence,

$$
\boxed{\det(A)=0}.
$$

### Step 5. Interpret the Determinant

The determinant of matrix $A$ is zero.

We know that a square matrix has an inverse only when its determinant is nonzero.

Since

$$
\det(A)=0,
$$

matrix $A$ is singular.

Therefore,

$$
\boxed{A^{-1}\text{ does not exist}.}
$$

This completes the first method.

### Step 6. Explain Why the Inverse Formula Cannot Be Used

The inverse formula for a $2 \times 2$ matrix is

$$
A^{-1}=
\frac{1}{ad-bc}
\begin{pmatrix}
d & -b \\
-c & a
\end{pmatrix}.
$$

For our matrix, this becomes

$$
A^{-1}=
\frac{1}{(2)(2)-(4)(1)}
\begin{pmatrix}
2 & -4 \\
-1 & 2
\end{pmatrix}.
$$

Since the determinant is zero,

$$
A^{-1}=
\frac{1}{0}
\begin{pmatrix}
2 & -4 \\
-1 & 2
\end{pmatrix}.
$$

However, division by zero is undefined.

Therefore, the inverse formula cannot produce a valid inverse matrix.

This confirms our conclusion:

$$
\boxed{A^{-1}\text{ does not exist}.}
$$

---

## Method 2. Using Linear Dependence Between Rows

### Step 7. Recall the Definition of Linear Dependence

The rows of a matrix are linearly dependent if at least one row can be written as a linear combination of the other rows.

For a matrix with two rows, linear dependence occurs when one row is a scalar multiple of the other.

Consider the two row vectors

$$
R_1=(a,b)
$$

and

$$
R_2=(c,d).
$$

If there exists a scalar $k$ such that

$$
R_1=kR_2,
$$

then the two rows are linearly dependent.

A square matrix with linearly dependent rows is not invertible.

This happens because the rows do not provide enough independent information to represent a full-dimensional linear transformation.

### Step 8. Identify the Rows of Matrix A

The given matrix is

$$
A=
\begin{pmatrix}
2 & 4 \\
1 & 2
\end{pmatrix}.
$$

Its first row is

$$
R_1=(2,4).
$$

Its second row is

$$
R_2=(1,2).
$$

We now check whether one row is a scalar multiple of the other.

### Step 9. Compare the Two Rows

Multiply the second row by $2$:

$$
2R_2=2(1,2).
$$

Performing the multiplication gives

$$
2R_2=(2,4).
$$

But

$$
R_1=(2,4).
$$

Therefore,

$$
\boxed{R_1=2R_2}.
$$

This shows that the first row is exactly twice the second row.

Equivalently,

$$
R_2=\frac{1}{2}R_1.
$$

Thus, the two rows are not independent.

They are linearly dependent.

### Step 10. Demonstrate Linear Dependence Algebraically

A set of vectors is linearly dependent if there exist coefficients, not all equal to zero, such that their linear combination equals the zero vector.

For our two rows, consider

$$
R_1-2R_2.
$$

Substituting the row vectors,

$$
R_1-2R_2=(2,4)-2(1,2).
$$

Therefore,

$$
R_1-2R_2=(2,4)-(2,4).
$$

Hence,

$$
R_1-2R_2=(0,0).
$$

We have obtained

$$
\boxed{R_1-2R_2=0}.
$$

The coefficients $1$ and $-2$ are not both zero.

Therefore, this equation proves that the rows are linearly dependent.

### Step 11. Explain Why Linear Dependence Prevents Invertibility

An invertible $2 \times 2$ matrix must have two linearly independent rows.

However, in our matrix,

$$
R_1=2R_2.
$$

This means that the first row does not provide any new independent information compared with the second row.

Consequently, the rank of the matrix is less than $2$.

Since the second row is nonzero and the first row is its scalar multiple, the matrix has exactly one linearly independent row.

Therefore,

$$
\operatorname{rank}(A)=1.
$$

For a $2 \times 2$ matrix to be invertible, its rank must be $2$.

Since

$$
\operatorname{rank}(A)=1<2,
$$

matrix $A$ is not invertible.

Thus,

$$
\boxed{A^{-1}\text{ does not exist}.}
$$

This completes the second method.

---

## Step 12. Additional Verification Using Row Reduction

We can also confirm the linear dependence by applying an elementary row operation.

Start with

$$
A=
\begin{pmatrix}
2 & 4 \\
1 & 2
\end{pmatrix}.
$$

Apply the row operation

$$
R_1\rightarrow R_1-2R_2.
$$

This gives

$$
\begin{pmatrix}
2 & 4 \\
1 & 2
\end{pmatrix}
\longrightarrow
\begin{pmatrix}
2-2(1) & 4-2(2) \\
1 & 2
\end{pmatrix}.
$$

Simplifying,

$$
\begin{pmatrix}
2 & 4 \\
1 & 2
\end{pmatrix}
\longrightarrow
\begin{pmatrix}
0 & 0 \\
1 & 2
\end{pmatrix}.
$$

The resulting matrix contains an entire row of zeros.

This shows that the two original rows were linearly dependent.

Furthermore, a matrix with a zero row cannot be transformed into the identity matrix using elementary row operations alone.

Therefore, matrix $A$ cannot be reduced to

$$
I=
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}.
$$

This provides another confirmation that the inverse does not exist.

---

## Step 13. Explain the Connection Between the Two Methods

The two methods are closely related.

In Method 1, we calculated

$$
\det(A)=0.
$$

In Method 2, we showed that

$$
R_1=2R_2.
$$

These results describe the same mathematical property from different perspectives.

The determinant measures whether a square matrix represents a transformation that preserves nonzero area or volume up to a scaling factor.

For a $2 \times 2$ matrix, a determinant of zero means that the corresponding linear transformation collapses the plane into a lower-dimensional space.

In this example, the rows are linearly dependent, so the matrix has rank $1$ rather than rank $2$.

As a result, the transformation loses information and cannot be reversed uniquely.

This explains why no inverse matrix exists.

The equivalence can be summarized as follows:

$$
\det(A)=0
$$

$$
\Updownarrow
$$

$$
\text{Rows are linearly dependent}
$$

$$
\Updownarrow
$$

$$
\operatorname{rank}(A)<2
$$

$$
\Updownarrow
$$

$$
\text{Matrix }A\text{ is not invertible}.
$$

Thus, the determinant condition and the linear dependence condition are two equivalent ways of recognizing noninvertibility.

---

## Final Answer

We are given

$$
A=
\begin{pmatrix}
2 & 4 \\
1 & 2
\end{pmatrix}.
$$

We have shown that $A^{-1}$ does not exist using two different methods.

### Method 1: Determinant

The determinant is

$$
\det(A)=(2)(2)-(4)(1).
$$

Therefore,

$$
\boxed{\det(A)=0}.
$$

Since the determinant is zero, matrix $A$ is singular and has no inverse.

### Method 2: Linear Dependence

The rows of matrix $A$ are

$$
R_1=(2,4),
\qquad
R_2=(1,2).
$$

Since

$$
\boxed{R_1=2R_2},
$$

the rows are linearly dependent.

Therefore, the matrix does not have full rank and cannot be inverted.

### Conclusion

Both methods lead to the same result:

$$
\boxed{
A^{-1}\text{ does not exist}.
}
$$

The determinant method shows that the matrix is singular because its determinant is zero.

The linear dependence method explains why this happens: one row is a scalar multiple of the other, so the matrix does not contain two independent rows.

Therefore, matrix $A$ is noninvertible, and the two methods are mathematically consistent.
