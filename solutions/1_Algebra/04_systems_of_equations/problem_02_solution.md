
# Exercise 2. Gaussian Elimination — One Solution

## Question

Solve the following system using Gaussian elimination:

$$
\begin{cases}
x+y+z=6, \\
2x-y+z=3, \\
x+2y-z=2.
\end{cases}
$$

After solving, substitute the result into all equations and check consistency.

---

## Solution

### Step 1. Construct the Augmented Matrix

The augmented matrix of the system is

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
2 & -1 & 1 & \mid & 3 \\
1 & 2 & -1 & \mid & 2 \\
\end{pmatrix}
$$

### Step 2. Apply Gaussian Elimination

Eliminate the entries below the first pivot using the row operations:

- $R_2 \to R_2-2R_1$
- $R_3 \to R_3-R_1$

The resulting matrix is

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
0 & -3 & -1 & \mid & -9 \\
0 & 1 & -2 & \mid & -4 \\
\end{pmatrix}
$$

Swap the second and third rows to obtain a simpler pivot:

$$
R_2 \leftrightarrow R_3
$$

The matrix becomes

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
0 & 1 & -2 & \mid & -4 \\
0 & -3 & -1 & \mid & -9 \\
\end{pmatrix}
$$

Next, eliminate the entry below the second pivot:

$$
R_3 \to R_3+3R_2
$$

We obtain

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
0 & 1 & -2 & \mid & -4 \\
0 & 0 & -7 & \mid & -21 \\
\end{pmatrix}
$$

The matrix is now in row echelon form.

### Step 3. Back Substitution

From the third row:

$$
-7z=-21
$$

Therefore,

$$
z=3
$$

From the second row:

$$
y-2z=-4
$$

Substituting $z=3$:

$$
y-6=-4
$$

$$
y=2
$$

From the first row:

$$
x+y+z=6
$$

Substituting $y=2$ and $z=3$:

$$
x+2+3=6
$$

$$
x=1
$$

### Step 4. Verify the Solution

Substitute $x=1$, $y=2$, and $z=3$ into the original equations.

**Equation 1:**

$$
1+2+3=6
$$

**Equation 2:**

$$
2(1)-2+3=3
$$

**Equation 3:**

$$
1+2(2)-3=2
$$

All three equations are satisfied.

---

## Final Answer

The solution is

$$
x=1,\qquad y=2,\qquad z=3
$$

**Number of solutions:** Exactly one.

**Conclusion:**

Gaussian elimination produces three nonzero pivots, so the system has a unique solution.

Substitution confirms that the solution satisfies all three original equations. Therefore, the system is consistent.

