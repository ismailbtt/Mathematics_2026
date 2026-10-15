
# Exercise 6. Transpose

## Question

Given

$$
A=
\begin{pmatrix}
1 & 2 & 3\\
4 & 5 & 6
\end{pmatrix},
\qquad
B=
\begin{pmatrix}
1 & 0\\
2 & 1\\
-1 & 3
\end{pmatrix}
$$

1. Compute $A^T$.
2. Compute $B^T$.
3. Compute $AB$.
4. Verify that:

$$
(AB)^T=B^TA^T
$$

---

## Solution 1. Calculate A Transpose

First, we find the transpose of matrix A.

$$
A=
\begin{pmatrix}
1 & 2 & 3\\
4 & 5 & 6
\end{pmatrix}
$$

The transpose of a matrix is obtained by changing its rows into columns.

### Step 1. Identify the Rows

The first row of A is:

$$
R_1=(1,2,3)
$$

The second row of A is:

$$
R_2=(4,5,6)
$$

### Step 2. Convert Rows into Columns

The first row becomes the first column.

The second row becomes the second column.

Therefore:

$$
\boxed{
A^T=
\begin{pmatrix}
1 & 4\\
2 & 5\\
3 & 6
\end{pmatrix}
}
$$

**Explanation:** Matrix A has dimensions $2\times3$, so its transpose has dimensions $3\times2$.

---

## Solution 2. Calculate B Transpose

Now, we calculate the transpose of matrix B.

$$
B=
\begin{pmatrix}
1 & 0\\
2 & 1\\
-1 & 3
\end{pmatrix}
$$

### Step 1. Identify the Rows

The rows of B are:

$$
R_1=(1,0)
$$

$$
R_2=(2,1)
$$

$$
R_3=(-1,3)
$$

### Step 2. Convert Rows into Columns

Each row becomes a column in the transpose.

Therefore:

$$
\boxed{
B^T=
\begin{pmatrix}
1 & 2 & -1\\
0 & 1 & 3
\end{pmatrix}
}
$$

**Explanation:** Matrix B has dimensions $3\times2$, so its transpose has dimensions $2\times3$.

---

## Solution 3. Calculate AB

We multiply matrix A by matrix B.

$$
AB=
\begin{pmatrix}
1 & 2 & 3\\
4 & 5 & 6
\end{pmatrix}
\begin{pmatrix}
1 & 0\\
2 & 1\\
-1 & 3
\end{pmatrix}
$$

First, check the dimensions.

$$
(2\times3)(3\times2)=2\times2
$$

The inner dimensions are equal, so multiplication is possible.

### Step 1. First Row, First Column

$$
1(1)+2(2)+3(-1)
$$

$$
=1+4-3
$$

$$
=2
$$

### Step 2. First Row, Second Column

$$
1(0)+2(1)+3(3)
$$

$$
=0+2+9
$$

$$
=11
$$

### Step 3. Second Row, First Column

$$
4(1)+5(2)+6(-1)
$$

$$
=4+10-6
$$

$$
=8
$$

### Step 4. Second Row, Second Column

$$
4(0)+5(1)+6(3)
$$

$$
=0+5+18
$$

$$
=23
$$

### Final Answer

$$
\boxed{
AB=
\begin{pmatrix}
2 & 11\\
8 & 23
\end{pmatrix}
}
$$

**Explanation:** Matrix multiplication is performed by multiplying the rows of the first matrix by the columns of the second matrix.

---

## Solution 4. Verify the Transpose Property

We need to verify:

$$
(AB)^T=B^TA^T
$$

### Step 1. Calculate (AB) Transpose

From Solution 3:

$$
AB=
\begin{pmatrix}
2 & 11\\
8 & 23
\end{pmatrix}
$$

Exchange rows and columns.

Therefore:

$$
\boxed{
(AB)^T=
\begin{pmatrix}
2 & 8\\
11 & 23
\end{pmatrix}
}
$$

### Step 2. Calculate B Transpose Times A Transpose

We already calculated:

$$
B^T=
\begin{pmatrix}
1 & 2 & -1\\
0 & 1 & 3
\end{pmatrix}
$$

and

$$
A^T=
\begin{pmatrix}
1 & 4\\
2 & 5\\
3 & 6
\end{pmatrix}
$$

Now multiply:

$$
B^TA^T=
\begin{pmatrix}
1 & 2 & -1\\
0 & 1 & 3
\end{pmatrix}
\begin{pmatrix}
1 & 4\\
2 & 5\\
3 & 6
\end{pmatrix}
$$

### Step 3. First Row, First Column

$$
1(1)+2(2)+(-1)(3)
$$

$$
=1+4-3
$$

$$
=2
$$

### Step 4. First Row, Second Column

$$
1(4)+2(5)+(-1)(6)
$$

$$
=4+10-6
$$

$$
=8
$$

### Step 5. Second Row, First Column

$$
0(1)+1(2)+3(3)
$$

$$
=0+2+9
$$

$$
=11
$$

### Step 6. Second Row, Second Column

$$
0(4)+1(5)+3(6)
$$

$$
=0+5+18
$$

$$
=23
$$

Therefore:

$$
\boxed{
B^TA^T=
\begin{pmatrix}
2 & 8\\
11 & 23
\end{pmatrix}
}
$$

---

## Mathematical Verification

Now, we compare both results.

First:

$$
(AB)^T=
\begin{pmatrix}
2 & 8\\
11 & 23
\end{pmatrix}
$$

Second:

$$
B^TA^T=
\begin{pmatrix}
2 & 8\\
11 & 23
\end{pmatrix}
$$

All corresponding entries are equal.

Therefore:

$$
\boxed{(AB)^T=B^TA^T}
$$

The transpose property is verified.

---

## Explanation

The transpose of a matrix changes rows into columns and columns into rows.

For matrix multiplication, the transpose property is:

$$
\boxed{(AB)^T=B^TA^T}
$$

Notice that the order of the matrices is reversed.

We write $B^TA^T$, not $A^TB^T$.

This is an important property of matrix transposition.

---

## Final Answers

**1. Transpose of A:**

$$
\boxed{
A^T=
\begin{pmatrix}
1 & 4\\
2 & 5\\
3 & 6
\end{pmatrix}
}
$$

**2. Transpose of B:**

$$
\boxed{
B^T=
\begin{pmatrix}
1 & 2 & -1\\
0 & 1 & 3
\end{pmatrix}
}
$$

**3. Matrix multiplication AB:**

$$
\boxed{
AB=
\begin{pmatrix}
2 & 11\\
8 & 23
\end{pmatrix}
}
$$

**4. Verification:**

$$
\boxed{
(AB)^T=B^TA^T=
\begin{pmatrix}
2 & 8\\
11 & 23
\end{pmatrix}
}
$$

## Conclusion

We successfully calculated the transposes of A and B, multiplied the matrices, and verified the transpose property.

The main rule is:

**The transpose of a matrix product equals the product of the transposes in reverse order.**
