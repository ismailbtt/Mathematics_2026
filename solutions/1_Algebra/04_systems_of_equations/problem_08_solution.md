
# Exercise 8. Two Systems with the Same Coefficient Matrix

## Question

Solve by elimination the following two systems.

**System 1**

$$
\begin{cases}
2x+y=5, \\
x-y=1.
\end{cases}
$$

**System 2**

$$
\begin{cases}
2x+y=1, \\
x-y=4.
\end{cases}
$$

Compare the successive elimination steps. Which part of the calculation is the same in both cases, and why?

---

## Solution

### Step 1. Solve System 1

The augmented matrix is

$$
\begin{pmatrix}
2 & 1 & \mid & 5 \\
1 & -1 & \mid & 1 \\
\end{pmatrix}
$$

Swap the two rows:

$$
R_1 \leftrightarrow R_2
$$

We obtain

$$
\begin{pmatrix}
1 & -1 & \mid & 1 \\
2 & 1 & \mid & 5 \\
\end{pmatrix}
$$

Eliminate the first entry of the second row:

$$
R_2 \to R_2-2R_1
$$

The matrix becomes

$$
\begin{pmatrix}
1 & -1 & \mid & 1 \\
0 & 3 & \mid & 3 \\
\end{pmatrix}
$$

From the second row,

$$
3y=3
$$

Therefore,

$$
y=1
$$

From the first row,

$$
x-y=1
$$

Substituting $y=1$ gives

$$
x=2
$$

The solution of System 1 is

$$
(x,y)=(2,1)
$$

### Step 2. Solve System 2

The augmented matrix is

$$
\begin{pmatrix}
2 & 1 & \mid & 1 \\
1 & -1 & \mid & 4 \\
\end{pmatrix}
$$

Apply the same row operations as in System 1.

First, swap the rows:

$$
R_1 \leftrightarrow R_2
$$

$$
\begin{pmatrix}
1 & -1 & \mid & 4 \\
2 & 1 & \mid & 1 \\
\end{pmatrix}
$$

Next, eliminate the first entry of the second row:

$$
R_2 \to R_2-2R_1
$$

We obtain

$$
\begin{pmatrix}
1 & -1 & \mid & 4 \\
0 & 3 & \mid & -7 \\
\end{pmatrix}
$$

From the second row,

$$
3y=-7
$$

Therefore,

$$
y=-\frac{7}{3}
$$

From the first row,

$$
x-y=4
$$

Substituting the value of $y$ gives

$$
x+\frac{7}{3}=4
$$

Therefore,

$$
x=\frac{5}{3}
$$

The solution of System 2 is

$$
(x,y)=\left(\frac{5}{3},-\frac{7}{3}\right)
$$

### Step 3. Verify the Solutions

**System 1**

Substitute $x=2$ and $y=1$:

$$
2(2)+1=5
$$

$$
2-1=1
$$

Both equations are satisfied.

**System 2**

Substitute $x=\frac{5}{3}$ and $y=-\frac{7}{3}$:

$$
2\left(\frac{5}{3}\right)-\frac{7}{3}=1
$$

$$
\frac{5}{3}+\frac{7}{3}=4
$$

Both equations are satisfied.

### Step 4. Compare the Elimination Steps

Both systems have the same coefficient matrix:

$$
A=
\begin{pmatrix}
2 & 1 \\
1 & -1 \\
\end{pmatrix}
$$

Therefore, the same elimination operations are used:

1. Swap $R_1$ and $R_2$.
2. Apply $R_2 \to R_2-2R_1$.

The coefficient matrix is reduced to the same row echelon form:

$$
\begin{pmatrix}
1 & -1 \\
0 & 3 \\
\end{pmatrix}
$$

However, the right-hand side vectors are different.

As a result, the final equations and solutions are different.

---

## Final Answer

**System 1:**

$$
(x,y)=(2,1)
$$

**System 2:**

$$
(x,y)=\left(\frac{5}{3},-\frac{7}{3}\right)
$$

**Conclusion:**

Both systems require the same Gaussian elimination operations because they share the same coefficient matrix.

Only the right-hand side values change, producing different solutions.

This demonstrates that the elimination steps for the coefficient matrix can be reused when solving systems with different right-hand sides.
