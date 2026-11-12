
# Exercise 11. A Parameter in a System of Three Equations

## Question

Analyze the number of solutions depending on $t$:

$$
\begin{cases}
x+y+z=1, \\
x+ty+z=2, \\
x+y+tz=3.
\end{cases}
$$

Use elimination and separately analyze the parameter values for which a standard calculation step ceases to be valid.

---

## Solution

### Step 1. Construct the Augmented Matrix

The augmented matrix is

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 1 \\
1 & t & 1 & \mid & 2 \\
1 & 1 & t & \mid & 3 \\
\end{pmatrix}
$$

### Step 2. Apply Gaussian Elimination

Eliminate the entries below the first pivot using:

- $R_2 \to R_2-R_1$
- $R_3 \to R_3-R_1$

The resulting matrix is

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 1 \\
0 & t-1 & 0 & \mid & 1 \\
0 & 0 & t-1 & \mid & 2 \\
\end{pmatrix}
$$

The number of solutions depends on whether $t-1$ is zero.

### Step 3. Case 1 — When $t\neq 1$

Since $t-1\neq 0$, both remaining pivots are nonzero.

From the second row,

$$
(t-1)y=1
$$

Therefore,

$$
y=\frac{1}{t-1}
$$

From the third row,

$$
(t-1)z=2
$$

Therefore,

$$
z=\frac{2}{t-1}
$$

Substitute these values into the first equation:

$$
x+y+z=1
$$

$$
x+\frac{1}{t-1}+\frac{2}{t-1}=1
$$

Simplifying,

$$
x=1-\frac{3}{t-1}
$$

Therefore,

$$
x=\frac{t-4}{t-1}
$$

The system has exactly one solution when $t\neq 1$.

### Step 4. Case 2 — When $t=1$

Substituting $t=1$ into the reduced matrix gives

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 1 \\
0 & 0 & 0 & \mid & 1 \\
0 & 0 & 0 & \mid & 2 \\
\end{pmatrix}
$$

The second and third rows represent

$$
0=1
$$

$$
0=2
$$

Both equations are contradictions.

Therefore, the system is inconsistent and has no solution when $t=1$.

### Step 5. Verify the Solution

For $t\neq 1$, the solution is

$$
x=\frac{t-4}{t-1},\qquad
y=\frac{1}{t-1},\qquad
z=\frac{2}{t-1}
$$

**Equation 1:**

$$
x+y+z=\frac{t-4+1+2}{t-1}=1
$$

**Equation 2:**

$$
x+ty+z=\frac{t-4+t+2}{t-1}=2
$$

**Equation 3:**

$$
x+y+tz=\frac{t-4+1+2t}{t-1}=3
$$

All three equations are satisfied for $t\neq 1$.

---

## Final Answer

**Case 1: When $t\neq 1$**

The system has exactly one solution:

$$
(x,y,z)=
\left(
\frac{t-4}{t-1},
\frac{1}{t-1},
\frac{2}{t-1}
\right)
$$

**Case 2: When $t=1$**

The system has no solution because elimination produces contradictory equations.

**Infinitely many solutions:**

This case never occurs.

**Conclusion:**

For every $t\neq 1$, Gaussian elimination produces three nonzero pivots, giving a unique solution.

When $t=1$, the system becomes inconsistent.

Therefore, the system has exactly one solution for $t\neq 1$ and no solution for $t=1$.
