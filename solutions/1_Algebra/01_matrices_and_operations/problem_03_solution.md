### Solution 3. Calculate 3A-2B

First multiply A by 3.

$$
3A=
\begin{pmatrix}3&6\\-3&9\end{pmatrix}
$$

Next multiply B by 2.

$$
2B=
\begin{pmatrix}8&-4\\0&10\end{pmatrix}
$$

Now subtract.

$$
3A-2B=
\begin{pmatrix}
3-8&6-(-4)\\
-3-0&9-10
\end{pmatrix}
$$

$$
\boxed{
3A-2B=
\begin{pmatrix}-5&10\\-3&-1\end{pmatrix}
}
$$

### Explanation

Matrix addition requires equal dimensions because corresponding entries must exist in both matrices.

Both A and B are 2×2, so addition and subtraction are possible.

**Verification:**

$$
3A-2B=3(A-B)+B
$$

$$
=3\begin{pmatrix}-3&4\\-1&-2\end{pmatrix}
+\begin{pmatrix}4&-2\\0&5\end{pmatrix}
$$

$$
=\begin{pmatrix}-5&10\\-3&-1\end{pmatrix}
$$

The result is correct.

---

## Exercise 3. When Can Matrices Be Multiplied?

### Question

Given matrix sizes:

$$
A_{2\times3},\quad
B_{3\times4},\quad
C_{4\times2},\quad
D_{2\times2}
$$

Determine whether the following products are defined:

$$
AB,\ BA,\ BC,\ CB,\ AC,\ CA,\ AD,\ DA
$$

### Solution

**Multiplication Rule:**

For two matrices

$$
X_{m\times n},\quad Y_{n\times p}
$$

multiplication is possible when the inner dimensions are equal.

The result has dimensions:

$$
XY_{m\times p}
$$

### 1. AB

$$
(2\times3)(3\times4)
$$

The inner dimensions are equal.

$$
\boxed{AB:2\times4}
$$

### 2. BA

$$
(3\times4)(2\times3)
$$

Since $4\neq2$, multiplication is not defined.

### 3. BC

$$
(3\times4)(4\times2)
$$

The inner dimensions match.

$$
\boxed{BC:3\times2}
$$

### 4. CB

$$
(4\times2)(3\times4)
$$

Since $2\neq3$, multiplication is not defined.

### 5. AC

$$
(2\times3)(4\times2)
$$

Since $3\neq4$, multiplication is not defined.

### 6. CA

$$
(4\times2)(2\times3)
$$

The inner dimensions match.

$$
\boxed{CA:4\times3}
$$

### 7. AD

$$
(2\times3)(2\times2)
$$

Since $3\neq2$, multiplication is not defined.

### 8. DA

$$
(2\times2)(2\times3)
$$

The inner dimensions match.

$$
\boxed{DA:2\times3}
$$

### Final Answers

| Product | Defined? | Result |
|---|---|---|
| AB | Yes | 2×4 |
| BA | No | Undefined |
| BC | Yes | 3×2 |
| CB | No | Undefined |
| AC | No | Undefined |
| CA | Yes | 4×3 |
| AD | No | Undefined |
| DA | Yes | 2×3 |

**Explanation:** Matrix multiplication depends on dimension compatibility. The number of columns of the first matrix must equal the number of rows of the second matrix.

---
