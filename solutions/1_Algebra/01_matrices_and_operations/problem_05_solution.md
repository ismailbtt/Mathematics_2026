
# Exercise 5. Matrix Times Vector

## Question

Let

$$
A=
\begin{pmatrix}
2 & -1\\
1 & 3
\end{pmatrix},
\qquad
x=
\begin{pmatrix}
4\\
2
\end{pmatrix}
$$

1. Compute $Ax$.
2. Express $Ax$ as a linear combination of the columns of $A$, with coefficients coming from the vector $x$.

---

## Solution 1. Calculate Ax

First, we multiply matrix A by vector x.

$$
Ax=
\begin{pmatrix}
2 & -1\\
1 & 3
\end{pmatrix}
\begin{pmatrix}
4\\
2
\end{pmatrix}
$$

Matrix A has dimensions $2\times2$, and vector x has dimensions $2\times1$.

$$
(2\times2)(2\times1)=2\times1
$$

Therefore, multiplication is possible, and the result will be a column vector with two entries.

### Step 1. First Row

Multiply the first row of A by the vector x.

$$
2(4)+(-1)(2)
$$

$$
=8-2
$$

$$
=6
$$

### Step 2. Second Row

Multiply the second row of A by the vector x.

$$
1(4)+3(2)
$$

$$
=4+6
$$

$$
=10
$$

### Final Answer

$$
\boxed{
Ax=
\begin{pmatrix}
6\\
10
\end{pmatrix}
}
$$

**Explanation:** In matrix-vector multiplication, we multiply each row of the matrix by the vector and add the products.

---

## Solution 2. Linear Combination of Columns

Now, we express $Ax$ as a linear combination of the columns of A.

The matrix A is:

$$
A=
\begin{pmatrix}
2 & -1\\
1 & 3
\end{pmatrix}
$$

### Step 1. Identify the Columns

The first column is:

$$
a_1=
\begin{pmatrix}
2\\
1
\end{pmatrix}
$$

The second column is:

$$
a_2=
\begin{pmatrix}
-1\\
3
\end{pmatrix}
$$

The vector x is:

$$
x=
\begin{pmatrix}
4\\
2
\end{pmatrix}
$$

The entries of x are the coefficients 4 and 2.

### Step 2. Write the Linear Combination

$$
Ax=4a_1+2a_2
$$

Substitute the column vectors:

$$
Ax=
4\begin{pmatrix}
2\\
1
\end{pmatrix}
+
2\begin{pmatrix}
-1\\
3
\end{pmatrix}
$$

### Step 3. Multiply Each Column by Its Coefficient

$$
4\begin{pmatrix}
2\\
1
\end{pmatrix}
=
\begin{pmatrix}
8\\
4
\end{pmatrix}
$$

$$
2\begin{pmatrix}
-1\\
3
\end{pmatrix}
=
\begin{pmatrix}
-2\\
6
\end{pmatrix}
$$

### Step 4. Add the Vectors

$$
Ax=
\begin{pmatrix}
8\\
4
\end{pmatrix}
+
\begin{pmatrix}
-2\\
6
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
8-2\\
4+6
\end{pmatrix}
$$

### Final Answer

$$
\boxed{
Ax=
\begin{pmatrix}
6\\
10
\end{pmatrix}
}
$$

**Explanation:** Matrix-vector multiplication can be understood as multiplying each column of the matrix by the corresponding entry of the vector and adding the results.

---

## Mathematical Verification

We calculated Ax using two different methods.

**Method 1: Row-by-column multiplication**

$$
Ax=
\begin{pmatrix}
2(4)+(-1)(2)\\
1(4)+3(2)
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
6\\
10
\end{pmatrix}
$$

**Method 2: Linear combination of columns**

$$
Ax=
4\begin{pmatrix}
2\\
1
\end{pmatrix}
+
2\begin{pmatrix}
-1\\
3
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
6\\
10
\end{pmatrix}
$$

Both methods give the same result.

Therefore, the answer is verified.

---

## Final Answers

**1. Matrix-vector multiplication:**

$$
\boxed{
Ax=
\begin{pmatrix}
6\\
10
\end{pmatrix}
}
$$

**2. Linear combination of columns:**

$$
\boxed{
Ax=
4\begin{pmatrix}
2\\
1
\end{pmatrix}
+
2\begin{pmatrix}
-1\\
3
\end{pmatrix}
=
\begin{pmatrix}
6\\
10
\end{pmatrix}
}
$$

## Conclusion

Matrix-vector multiplication can be calculated in two equivalent ways:

1. Multiplying the rows of the matrix by the vector.
2. Taking a linear combination of the columns of the matrix.

Both methods produce the same result.

