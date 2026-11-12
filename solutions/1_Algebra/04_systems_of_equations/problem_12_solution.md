
# Exercise 12. Homogeneous System

## Question

Solve the following homogeneous system:

$$
\begin{cases}
x+2y-z=0, \\
2x+4y-2z=0, \\
x-y+2z=0.
\end{cases}
$$

Give all solutions in parametric form and explain why $(0,0,0)$ always satisfies a homogeneous system.

---

## Solution

### Step 1. Construct the Augmented Matrix

The augmented matrix is

$$
\begin{pmatrix}
1 & 2 & -1 & \mid & 0 \\
2 & 4 & -2 & \mid & 0 \\
1 & -1 & 2 & \mid & 0 \\
\end{pmatrix}
$$

### Step 2. Apply Gaussian Elimination

Eliminate the entries below the first pivot using:

- $R_2 \to R_2-2R_1$
- $R_3 \to R_3-R_1$

The resulting matrix is

$$
\begin{pmatrix}
1 & 2 & -1 & \mid & 0 \\
0 & 0 & 0 & \mid & 0 \\
0 & -3 & 3 & \mid & 0 \\
\end{pmatrix}
$$

Swap the second and third rows:

$$
R_2 \leftrightarrow R_3
$$

We obtain

$$
\begin{pmatrix}
1 & 2 & -1 & \mid & 0 \\
0 & -3 & 3 & \mid & 0 \\
0 & 0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

Divide the second row by $-3$:

$$
R_2 \to -\frac{1}{3}R_2
$$

The matrix becomes

$$
\begin{pmatrix}
1 & 2 & -1 & \mid & 0 \\
0 & 1 & -1 & \mid & 0 \\
0 & 0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

Finally, eliminate the second entry of the first row:

$$
R_1 \to R_1-2R_2
$$

The reduced matrix is

$$
\begin{pmatrix}
1 & 0 & 1 & \mid & 0 \\
0 & 1 & -1 & \mid & 0 \\
0 & 0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

### Step 3. Find the Parametric Solution

The reduced matrix represents

$$
x+z=0
$$

$$
y-z=0
$$

There are three variables and two pivot columns, so one variable is free.

Let

$$
z=t,\qquad t\in\mathbb{R}
$$

Then

$$
x=-t
$$

$$
y=t
$$

Therefore, the general solution is

$$
(x,y,z)=(-t,t,t),\qquad t\in\mathbb{R}
$$

### Step 4. Verify the Solution

Substitute $x=-t$, $y=t$, and $z=t$ into the original equations.

**Equation 1:**

$$
-t+2t-t=0
$$

**Equation 2:**

$$
2(-t)+4t-2t=0
$$

**Equation 3:**

$$
-t-t+2t=0
$$

All three equations are satisfied for every real value of $t$.

### Step 5. Explain the Zero Solution

A homogeneous system has the form

$$
Ax=0
$$

When all variables are zero, every equation is automatically satisfied because the left-hand side becomes zero.

Therefore, $(0,0,0)$ always satisfies a homogeneous system.

In this example, choosing $t=0$ gives the zero solution.

---

## Final Answer

The general solution is

$$
(x,y,z)=(-t,t,t),\qquad t\in\mathbb{R}
$$

**Free variable:** $z=t$

**Number of solutions:** Infinitely many.

**Zero solution:** $(0,0,0)$

**Conclusion:**

Gaussian elimination produces two pivot variables and one free variable. The system therefore has infinitely many solutions.

The zero solution always exists because the right-hand side of every equation in a homogeneous system is zero.

Substitution confirms that the parametric solution satisfies all three equations.
