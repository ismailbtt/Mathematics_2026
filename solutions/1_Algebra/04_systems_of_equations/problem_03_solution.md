
# Exercise 3. Inconsistent System

## Question

Solve or show that the following system is inconsistent:

$$
\begin{cases}
x+2y=3, \\
2x+4y=7.
\end{cases}
$$

Show how the contradiction appears in the matrix after elimination and interpret it in terms of equations.

---

## Solution

### Step 1. Construct the Augmented Matrix

The augmented matrix is

$$
\begin{pmatrix}
1 & 2 & \mid & 3 \\
2 & 4 & \mid & 7 \\
\end{pmatrix}
$$

### Step 2. Apply Gaussian Elimination

To eliminate the first element of the second row, apply the row operation:

$$
R_2 \to R_2-2R_1
$$

The resulting matrix is

$$
\begin{pmatrix}
1 & 2 & \mid & 3 \\
0 & 0 & \mid & 1 \\
\end{pmatrix}
$$

### Step 3. Identify the Contradiction

The second row represents the equation

$$
0x+0y=1
$$

which simplifies to

$$
0=1
$$

This is impossible. Therefore, the system is inconsistent and has no solution.

### Step 4. Interpret the Original Equations

The first equation is

$$
x+2y=3
$$

Multiplying both sides by 2 gives

$$
2x+4y=6
$$

However, the second equation requires

$$
2x+4y=7
$$

The same expression cannot equal both 6 and 7.

Therefore, no values of $x$ and $y$ can satisfy both equations simultaneously.

---

## Final Answer

After Gaussian elimination, the augmented matrix becomes

$$
\begin{pmatrix}
1 & 2 & \mid & 3 \\
0 & 0 & \mid & 1 \\
\end{pmatrix}
$$

The second row gives the contradiction

$$
0=1
$$

**Number of solutions:** No solution.

**Conclusion:**

The system is inconsistent because Gaussian elimination produces a contradictory equation.

Geometrically, the two equations represent distinct parallel lines that never intersect.
