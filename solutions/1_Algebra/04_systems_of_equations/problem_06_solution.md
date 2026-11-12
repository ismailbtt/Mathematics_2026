
# Exercise 6. A System with a Parameter — Which Cases Actually Occur?

## Question

Analyze the following system depending on the parameter $a$:

$$
\begin{cases}
x+y=2, \\
ax+ay=4.
\end{cases}
$$

Among the three possibilities — exactly one solution, infinitely many solutions, and no solution — determine which actually occur and for which values of $a$.

If one type cannot occur, explain why.

---

## Solution

### Step 1. Construct the Augmented Matrix

The augmented matrix is

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
a & a & \mid & 4 \\
\end{pmatrix}
$$

### Step 2. Apply Gaussian Elimination

Eliminate the first entry of the second row using

$$
R_2 \to R_2-aR_1
$$

The resulting matrix is

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & 0 & \mid & 4-2a \\
\end{pmatrix}
$$

The number of solutions depends on the value of $a$.

### Step 3. Analyze the Parameter

**Case 1: When $a=2$**

Substituting $a=2$ gives

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

The second row represents $0=0$, which is always true.

Therefore, the system reduces to

$$
x+y=2
$$

Let $y=t$, where $t\in\mathbb{R}$.

Then

$$
x=2-t
$$

Thus, the system has infinitely many solutions:

$$
(x,y)=(2-t,t),\qquad t\in\mathbb{R}
$$

**Case 2: When $a\neq 2$**

Since $a\neq 2$,

$$
4-2a\neq 0
$$

The second row represents

$$
0=4-2a
$$

This is a contradiction.

Therefore, the system is inconsistent and has no solution.

### Step 4. Explain Why a Unique Solution Cannot Occur

The coefficient matrix is

$$
A=
\begin{pmatrix}
1 & 1 \\
a & a \\
\end{pmatrix}
$$

Its determinant is

$$
\det A=(1)(a)-(1)(a)=0
$$

The determinant is zero for every value of $a$.

Therefore, the coefficient matrix is never invertible, and the system cannot have exactly one solution.

---

## Final Answer

**When $a=2$:**

The system has infinitely many solutions:

$$
(x,y)=(2-t,t),\qquad t\in\mathbb{R}
$$

**When $a\neq 2$:**

The system has no solution because the equations are inconsistent.

**Exactly one solution:**

This case never occurs because

$$
\det A=0
$$

for all values of $a$.

**Conclusion:**

The system has infinitely many solutions when $a=2$ and no solution when $a\neq 2$.

A unique solution is impossible because the coefficient matrix is singular for every value of the parameter.
