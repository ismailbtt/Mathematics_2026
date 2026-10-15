
# Exercise 7. Identity Matrix, Zero Matrix, and Powers

## Question

Given

$$
A=
\begin{pmatrix}
2 & 1\\
0 & 2
\end{pmatrix}
$$

Compute:

1. $AI$
2. $IA$
3. $A+0$
4. $A^2$
5. $A^3$

Explain the roles of the identity matrix $I$ and the zero matrix $0$.

Describe the pattern observed in successive powers of $A$.

---

## Solution 1. Calculate AI

First, we define the identity matrix.

$$
I=
\begin{pmatrix}
1 & 0\\
0 & 1
\end{pmatrix}
$$

Now multiply matrix A by I.

$$
AI=
\begin{pmatrix}
2 & 1\\
0 & 2
\end{pmatrix}
\begin{pmatrix}
1 & 0\\
0 & 1
\end{pmatrix}
$$

### Step 1. First Row, First Column

$$
2(1)+1(0)=2
$$

### Step 2. First Row, Second Column

$$
2(0)+1(1)=1
$$

### Step 3. Second Row, First Column

$$
0(1)+2(0)=0
$$

### Step 4. Second Row, Second Column

$$
0(0)+2(1)=2
$$

### Final Answer

$$
\boxed{
AI=
\begin{pmatrix}
2 & 1\\
0 & 2
\end{pmatrix}
}
$$

**Explanation:** Multiplying a matrix by the identity matrix does not change the original matrix.

---

## Solution 2. Calculate IA

Now, we change the multiplication order.

$$
IA=
\begin{pmatrix}
1 & 0\\
0 & 1
\end{pmatrix}
\begin{pmatrix}
2 & 1\\
0 & 2
\end{pmatrix}
$$

### Step 1. First Row, First Column

$$
1(2)+0(0)=2
$$

### Step 2. First Row, Second Column

$$
1(1)+0(2)=1
$$

### Step 3. Second Row, First Column

$$
0(2)+1(0)=0
$$

### Step 4. Second Row, Second Column

$$
0(1)+1(2)=2
$$

### Final Answer

$$
\boxed{
IA=
\begin{pmatrix}
2 & 1\\
0 & 2
\end{pmatrix}
}
$$

Therefore:

$$
\boxed{AI=IA=A}
$$

**Explanation:** The identity matrix is the multiplicative identity because multiplying by it on either side leaves A unchanged.

---

## Solution 3. Calculate A+0

First, we define the zero matrix.

$$
0=
\begin{pmatrix}
0 & 0\\
0 & 0
\end{pmatrix}
$$

Now add A and the zero matrix.

$$
A+0=
\begin{pmatrix}
2 & 1\\
0 & 2
\end{pmatrix}
+
\begin{pmatrix}
0 & 0\\
0 & 0
\end{pmatrix}
$$

We add corresponding entries.

$$
=
\begin{pmatrix}
2+0 & 1+0\\
0+0 & 2+0
\end{pmatrix}
$$

### Final Answer

$$
\boxed{
A+0=
\begin{pmatrix}
2 & 1\\
0 & 2
\end{pmatrix}
}
$$

Therefore:

$$
\boxed{A+0=A}
$$

**Explanation:** The zero matrix is the additive identity because adding it does not change the matrix.

---

## Solution 4. Calculate A²

The square of a matrix means multiplying the matrix by itself.

$$
A^2=A\cdot A
$$

$$
A^2=
\begin{pmatrix}
2 & 1\\
0 & 2
\end{pmatrix}
\begin{pmatrix}
2 & 1\\
0 & 2
\end{pmatrix}
$$

### Step 1. First Row, First Column

$$
2(2)+1(0)
$$

$$
=4+0=4
$$

### Step 2. First Row, Second Column

$$
2(1)+1(2)
$$

$$
=2+2=4
$$

### Step 3. Second Row, First Column

$$
0(2)+2(0)
$$

$$
=0
$$

### Step 4. Second Row, Second Column

$$
0(1)+2(2)
$$

$$
=0+4=4
$$

### Final Answer

$$
\boxed{
A^2=
\begin{pmatrix}
4 & 4\\
0 & 4
\end{pmatrix}
}
$$

**Explanation:** Matrix powers are calculated by repeated matrix multiplication, not by squaring each entry separately.

---

## Solution 5. Calculate A³

The third power of A is:

$$
A^3=A^2A
$$

We already calculated:

$$
A^2=
\begin{pmatrix}
4 & 4\\
0 & 4
\end{pmatrix}
$$

Now multiply:

$$
A^3=
\begin{pmatrix}
4 & 4\\
0 & 4
\end{pmatrix}
\begin{pmatrix}
2 & 1\\
0 & 2
\end{pmatrix}
$$

### Step 1. First Row, First Column

$$
4(2)+4(0)
$$

$$
=8
$$

### Step 2. First Row, Second Column

$$
4(1)+4(2)
$$

$$
=4+8=12
$$

### Step 3. Second Row, First Column

$$
0(2)+4(0)
$$

$$
=0
$$

### Step 4. Second Row, Second Column

$$
0(1)+4(2)
$$

$$
=8
$$

### Final Answer

$$
\boxed{
A^3=
\begin{pmatrix}
8 & 12\\
0 & 8
\end{pmatrix}
}
$$

---

## Solution 6. Identify the Pattern

We have calculated:

$$
A^1=
\begin{pmatrix}
2 & 1\\
0 & 2
\end{pmatrix}
$$

$$
A^2=
\begin{pmatrix}
4 & 4\\
0 & 4
\end{pmatrix}
$$

$$
A^3=
\begin{pmatrix}
8 & 12\\
0 & 8
\end{pmatrix}
$$

### Step 1. Observe the Diagonal Entries

The diagonal entries follow powers of 2.

$$
2,\ 4,\ 8,\ 16,\ldots
$$

Therefore, the diagonal entries of $A^n$ are:

$$
2^n
$$

### Step 2. Observe the Upper-Right Entry

The upper-right entries are:

$$
1,\ 4,\ 12,\ldots
$$

They follow the pattern:

$$
n2^{n-1}
$$

For example:

When $n=1$:

$$
1\cdot2^0=1
$$

When $n=2$:

$$
2\cdot2^1=4
$$

When $n=3$:

$$
3\cdot2^2=12
$$

### General Formula

Therefore, the general formula is:

$$
\boxed{
A^n=
\begin{pmatrix}
2^n & n2^{n-1}\\
0 & 2^n
\end{pmatrix}
}
$$

for every positive integer $n$.

---

## Mathematical Verification

We can verify the formula by calculating $A^4$.

Using the general formula:

$$
A^4=
\begin{pmatrix}
2^4 & 4\cdot2^3\\
0 & 2^4
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
16 & 32\\
0 & 16
\end{pmatrix}
$$

Now verify using matrix multiplication:

$$
A^4=A^3A
$$

$$
=
\begin{pmatrix}
8 & 12\\
0 & 8
\end{pmatrix}
\begin{pmatrix}
2 & 1\\
0 & 2
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
8(2)+12(0) & 8(1)+12(2)\\
0(2)+8(0) & 0(1)+8(2)
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
16 & 32\\
0 & 16
\end{pmatrix}
$$

Both methods give the same result.

Therefore, the formula is verified for $n=4$.

---

## Explanation of Identity and Zero Matrices

### Identity Matrix

The identity matrix has ones on the main diagonal and zeros everywhere else.

$$
I=
\begin{pmatrix}
1 & 0\\
0 & 1
\end{pmatrix}
$$

It satisfies:

$$
\boxed{AI=IA=A}
$$

It plays the same role as the number 1 in ordinary multiplication.

### Zero Matrix

The zero matrix contains only zeros.

$$
0=
\begin{pmatrix}
0 & 0\\
0 & 0
\end{pmatrix}
$$

It satisfies:

$$
\boxed{A+0=A}
$$

It plays the same role as the number 0 in ordinary addition.

---

## Final Answers

**1. Calculate AI:**

$$
\boxed{
AI=
\begin{pmatrix}
2 & 1\\
0 & 2
\end{pmatrix}
}
$$

**2. Calculate IA:**

$$
\boxed{
IA=
\begin{pmatrix}
2 & 1\\
0 & 2
\end{pmatrix}
}
$$

**3. Calculate A+0:**

$$
\boxed{
A+0=
\begin{pmatrix}
2 & 1\\
0 & 2
\end{pmatrix}
}
$$

**4. Calculate A²:**

$$
\boxed{
A^2=
\begin{pmatrix}
4 & 4\\
0 & 4
\end{pmatrix}
}
$$

**5. Calculate A³:**

$$
\boxed{
A^3=
\begin{pmatrix}
8 & 12\\
0 & 8
\end{pmatrix}
}
$$

**6. General Pattern:**

$$
\boxed{
A^n=
\begin{pmatrix}
2^n & n2^{n-1}\\
0 & 2^n
\end{pmatrix}
}
$$

---

## Conclusion

The identity matrix does not change a matrix under multiplication.

The zero matrix does not change a matrix under addition.

Successive powers of A follow a predictable pattern.

The diagonal entries become powers of 2, while the upper-right entry follows the formula $n2^{n-1}$.
