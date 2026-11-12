
# Exercise 4. Infinitely Many Solutions

## Question

Solve the following system:

$$
\begin{cases}
x+y+z=2, \\
2x+2y+2z=4, \\
x-y+z=0.
\end{cases}
$$

Give the solution in parametric form, identify a free variable, and check that the resulting point satisfies the system for one chosen parameter value.

---

## Solution

### Step 1. Construct the Augmented Matrix

The augmented matrix is

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 2 \\
2 & 2 & 2 & \mid & 4 \\
1 & -1 & 1 & \mid & 0 \\
\end{pmatrix}
$$

### Step 2. Apply Gaussian Elimination

Apply the row operations:

- $R_2 \to R_2-2R_1$
- $R_3 \to R_3-R_1$

The matrix becomes

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 2 \\
0 & 0 & 0 & \mid & 0 \\
0 & -2 & 0 & \mid & -2 \\
\end{pmatrix}
$$

Swap the second and third rows:

$$
R_2 \leftrightarrow R_3
$$

We obtain

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 2 \\
0 & -2 & 0 & \mid & -2 \\
0 & 0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

Divide the second row by $-2$:

$$
R_2 \to -\frac{1}{2}R_2
$$

The matrix becomes

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 2 \\
0 & 1 & 0 & \mid & 1 \\
0 & 0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

Finally, eliminate the entry above the second pivot:

$$
R_1 \to R_1-R_2
$$

The reduced matrix is

$$
\begin{pmatrix}
1 & 0 & 1 & \mid & 1 \\
0 & 1 & 0 & \mid & 1 \\
0 & 0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

### Step 3. Find the Parametric Solution

The reduced matrix represents

$$
x+z=1
$$

$$
y=1
$$

There are three variables and two pivot columns. Therefore, one variable is free.

Let

$$
z=t,\qquad t\in\mathbb{R}
$$

Then

$$
x=1-t
$$

$$
y=1
$$

The general solution is

$$
(x,y,z)=(1-t,1,t),\qquad t\in\mathbb{R}
$$

### Step 4. Verify the Solution

Choose $t=0$.

Then

$$
x=1,\qquad y=1,\qquad z=0
$$

Substitute these values into the original equations.

**Equation 1:**

$$
1+1+0=2
$$

**Equation 2:**

$$
2(1)+2(1)+2(0)=4
$$

**Equation 3:**

$$
1-1+0=0
$$

All three equations are satisfied.

---

## Final Answer

The general solution is

$$
(x,y,z)=(1-t,1,t),\qquad t\in\mathbb{R}
$$

**Free variable:** $z=t$

**Number of solutions:** Infinitely many.

**Example solution:** $(1,1,0)$

**Conclusion:**

Gaussian elimination produces two pivot variables and one free variable. Since the system is consistent and the free variable can take any real value, the system has infinitely many solutions.
