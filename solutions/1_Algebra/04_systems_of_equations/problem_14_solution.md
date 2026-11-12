
# Exercise 14. A Small Change in the Right-Hand Side

## Question

Compare the following two systems.

**System 1**

$$
\begin{cases}
x+y=2, \\
2x-y=1, \\
3x=3.
\end{cases}
$$

**System 2**

$$
\begin{cases}
x+y=2, \\
2x-y=1, \\
3x=3.1.
\end{cases}
$$

Check the consistency of each system and explain why a small change in one number can change the type of the system.

---

## Solution

### Step 1. Analyze System 1

The augmented matrix is

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
2 & -1 & \mid & 1 \\
3 & 0 & \mid & 3 \\
\end{pmatrix}
$$

Apply the row operations:

- $R_2 \to R_2-2R_1$
- $R_3 \to R_3-3R_1$

The matrix becomes

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & -3 & \mid & -3 \\
0 & -3 & \mid & -3 \\
\end{pmatrix}
$$

Next, apply

$$
R_3 \to R_3-R_2
$$

We obtain

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & -3 & \mid & -3 \\
0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

From the second row,

$$
-3y=-3
$$

Therefore,

$$
y=1
$$

From the first row,

$$
x+1=2
$$

Thus,

$$
x=1
$$

The third row gives $0=0$, so the system is consistent.

**Verification:**

$$
1+1=2
$$

$$
2(1)-1=1
$$

$$
3(1)=3
$$

All equations are satisfied.

Therefore, System 1 has exactly one solution.

### Step 2. Analyze System 2

The augmented matrix is

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
2 & -1 & \mid & 1 \\
3 & 0 & \mid & 3.1 \\
\end{pmatrix}
$$

Apply the same row operations:

- $R_2 \to R_2-2R_1$
- $R_3 \to R_3-3R_1$

The matrix becomes

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & -3 & \mid & -3 \\
0 & -3 & \mid & -2.9 \\
\end{pmatrix}
$$

Next, apply

$$
R_3 \to R_3-R_2
$$

We obtain

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & -3 & \mid & -3 \\
0 & 0 & \mid & 0.1 \\
\end{pmatrix}
$$

The third row represents

$$
0=0.1
$$

This is a contradiction.

Therefore, System 2 is inconsistent and has no solution.

### Step 3. Compare the Systems

Both systems have the same coefficient matrix:

$$
A=
\begin{pmatrix}
1 & 1 \\
2 & -1 \\
3 & 0 \\
\end{pmatrix}
$$

Only the third constant changes from $3$ to $3.1$.

In System 1, the third equation is consistent with the first two equations.

In System 2, the first two equations still require $x=1$, but the third equation requires

$$
x=\frac{3.1}{3}
$$

These conditions cannot both hold.

Therefore, even a small change in the right-hand side can make a previously consistent system inconsistent.

---

## Final Answer

**System 1:**

$$
(x,y)=(1,1)
$$

**Number of solutions:** Exactly one.

**System 2:**

The system produces the contradiction

$$
0=0.1
$$

**Number of solutions:** No solution.

**Conclusion:**

System 1 is consistent and has a unique solution.

System 2 is inconsistent because the small change from $3$ to $3.1$ creates a contradiction between the equations.

This demonstrates that changing a right-hand side value can change the consistency of a linear system, even when the coefficient matrix remains unchanged.
