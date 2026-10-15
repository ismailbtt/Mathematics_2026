
# Exercise 4. Matrix Multiplication and Noncommutativity

## Question

Given the matrices:

$$
A=
\begin{pmatrix}
1 & 2\\
0 & 1
\end{pmatrix},
\qquad
B=
\begin{pmatrix}
2 & 0\\
3 & 1
\end{pmatrix}
$$

1. Compute $AB$.
2. Compute $BA$.
3. Is $AB=BA$?
4. Use this example to explain what noncommutativity of matrix multiplication means.

---

## Solution 1. Calculate AB

First, we multiply matrix A by matrix B.

$$
AB=
\begin{pmatrix}
1 & 2\\
0 & 1
\end{pmatrix}
\begin{pmatrix}
2 & 0\\
3 & 1
\end{pmatrix}
$$

We multiply the rows of A by the columns of B and add the results.

### Step 1. First Row, First Column

$$
1(2)+2(3)=2+6=8
$$

### Step 2. First Row, Second Column

$$
1(0)+2(1)=0+2=2
$$

### Step 3. Second Row, First Column

$$
0(2)+1(3)=0+3=3
$$

### Step 4. Second Row, Second Column

$$
0(0)+1(1)=0+1=1
$$

### Final Answer

$$
\boxed{
AB=
\begin{pmatrix}
8 & 2\\
3 & 1
\end{pmatrix}
}
$$

**Explanation:** Matrix multiplication is performed by multiplying each row of the first matrix by each column of the second matrix.

---

## Solution 2. Calculate BA

Now, we change the order and multiply matrix B by matrix A.

$$
BA=
\begin{pmatrix}
2 & 0\\
3 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 2\\
0 & 1
\end{pmatrix}
$$

### Step 1. First Row, First Column

$$
2(1)+0(0)=2+0=2
$$

### Step 2. First Row, Second Column

$$
2(2)+0(1)=4+0=4
$$

### Step 3. Second Row, First Column

$$
3(1)+1(0)=3+0=3
$$

### Step 4. Second Row, Second Column

$$
3(2)+1(1)=6+1=7
$$

### Final Answer

$$
\boxed{
BA=
\begin{pmatrix}
2 & 4\\
3 & 7
\end{pmatrix}
}
$$

**Explanation:** We use the same multiplication method, but the order of the matrices is reversed.

---

## Solution 3. Is AB = BA?

We compare the two results.

$$
AB=
\begin{pmatrix}
8 & 2\\
3 & 1
\end{pmatrix}
$$

$$
BA=
\begin{pmatrix}
2 & 4\\
3 & 7
\end{pmatrix}
$$

Two matrices are equal only if all corresponding entries are equal.

For example, compare the first entries:

$$
(AB)_{11}=8
$$

$$
(BA)_{11}=2
$$

Since:

$$
8\neq2
$$

the matrices are not equal.

### Final Answer

$$
\boxed{AB\neq BA}
$$

**Explanation:** Changing the order of multiplication produces a different result.

---

## Solution 4. Explain Noncommutativity

Noncommutativity means that the order of multiplication matters.

For ordinary numbers:

$$
2\times3=3\times2=6
$$

This is called the commutative property.

However, matrix multiplication is generally not commutative.

In this exercise:

$$
AB=
\begin{pmatrix}
8 & 2\\
3 & 1
\end{pmatrix}
$$

and

$$
BA=
\begin{pmatrix}
2 & 4\\
3 & 7
\end{pmatrix}
$$

Therefore:

$$
\boxed{AB\neq BA}
$$

This demonstrates noncommutativity.

**Explanation:** Multiplying A by B is not necessarily the same as multiplying B by A. Some matrices commute, but matrix multiplication is not commutative in general.

---

## Mathematical Verification

We can verify that the products are different by calculating their difference.

$$
AB-BA=
\begin{pmatrix}
8 & 2\\
3 & 1
\end{pmatrix}
-
\begin{pmatrix}
2 & 4\\
3 & 7
\end{pmatrix}
$$

Subtract the corresponding entries:

$$
AB-BA=
\begin{pmatrix}
8-2 & 2-4\\
3-3 & 1-7
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
6 & -2\\
0 & -6
\end{pmatrix}
$$

Because this is not the zero matrix:

$$
AB-BA\neq0
$$

Therefore:

$$
\boxed{AB\neq BA}
$$

The result is verified.

---

## Final Answers

**1. Product AB:**

$$
\boxed{
AB=
\begin{pmatrix}
8 & 2\\
3 & 1
\end{pmatrix}
}
$$

**2. Product BA:**

$$
\boxed{
BA=
\begin{pmatrix}
2 & 4\\
3 & 7
\end{pmatrix}
}
$$

**3. Are AB and BA equal?**

$$
\boxed{AB\neq BA}
$$

**4. What is noncommutativity?**

Matrix multiplication is generally noncommutative because changing the order of the matrices can change the result.

**Conclusion:** The order of matrix multiplication matters.

