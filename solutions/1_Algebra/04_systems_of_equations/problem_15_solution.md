
# Exercise 15. Classifying Three Systems

## Question

For each of the following systems, perform only as much elimination as necessary to recognize its type.

**System 1**

$$
\begin{cases}
x+y=2, \\
x-y=0.
\end{cases}
$$

**System 2**

$$
\begin{cases}
x+y=2, \\
2x+2y=4.
\end{cases}
$$

**System 3**

$$
\begin{cases}
x+y=2, \\
2x+2y=5.
\end{cases}
$$

For each system, justify the classification: one solution, infinitely many solutions, or no solution.

---

## Solution

### Step 1. System 1 — Exactly One Solution

The augmented matrix is

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
1 & -1 & \mid & 0 \\
\end{pmatrix}
$$

Apply the row operation

$$
R_2 \to R_2-R_1
$$

The resulting matrix is

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & -2 & \mid & -2 \\
\end{pmatrix}
$$

From the second row,

$$
-2y=-2
$$

Therefore,

$$
y=1
$$

Substitute into the first equation:

$$
x+1=2
$$

Thus,

$$
x=1
$$

**Verification:**

$$
1+1=2
$$

$$
1-1=0
$$

Both equations are satisfied.

Therefore, System 1 has exactly one solution.

### Step 2. System 2 — Infinitely Many Solutions

The augmented matrix is

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
2 & 2 & \mid & 4 \\
\end{pmatrix}
$$

Apply the row operation

$$
R_2 \to R_2-2R_1
$$

The resulting matrix is

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

The second row represents $0=0$, which is always true.

The system reduces to

$$
x+y=2
$$

Let $y=t$, where $t\in\mathbb{R}$.

Then

$$
x=2-t
$$

**Verification:**

$$
(2-t)+t=2
$$

$$
2(2-t)+2t=4
$$

Both equations are satisfied for every real value of $t$.

Therefore, System 2 has infinitely many solutions.

### Step 3. System 3 — No Solution

The augmented matrix is

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
2 & 2 & \mid & 5 \\
\end{pmatrix}
$$

Apply the row operation

$$
R_2 \to R_2-2R_1
$$

The resulting matrix is

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & 0 & \mid & 1 \\
\end{pmatrix}
$$

The second row represents the contradiction

$$
0=1
$$

Therefore, the system is inconsistent and has no solution.

---

## Final Answer

**System 1:**

$$
(x,y)=(1,1)
$$

Number of solutions: Exactly one.

**System 2:**

$$
(x,y)=(2-t,t),\qquad t\in\mathbb{R}
$$

Number of solutions: Infinitely many.

**System 3:**

$$
0=1
$$

Number of solutions: No solution.

**Conclusion:**

Gaussian elimination identifies the three fundamental cases of linear systems:

- System 1 has a unique solution because both variables have pivot positions.
- System 2 has infinitely many solutions because one variable is free and no contradiction occurs.
- System 3 has no solution because elimination produces a contradiction.

All three systems are correctly classified.
