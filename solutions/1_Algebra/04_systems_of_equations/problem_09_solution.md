
# Exercise 9. A System from a Sum Condition

## Question

Find numbers $x,y$ satisfying

$$
x+y=10
$$

$$
2x+5y=32
$$

Solve the system and explain geometrically why the solution is unique.

---

## Solution

### Step 1. Construct the Augmented Matrix

The augmented matrix is

$$
\begin{pmatrix}
1 & 1 & \mid & 10 \\
2 & 5 & \mid & 32 \\
\end{pmatrix}
$$

### Step 2. Apply Gaussian Elimination

Eliminate the first entry of the second row:

$$
R_2 \to R_2-2R_1
$$

The resulting matrix is

$$
\begin{pmatrix}
1 & 1 & \mid & 10 \\
0 & 3 & \mid & 12 \\
\end{pmatrix}
$$

From the second row,

$$
3y=12
$$

Therefore,

$$
y=4
$$

Substitute $y=4$ into the first equation:

$$
x+4=10
$$

Thus,

$$
x=6
$$

### Step 3. Verify the Solution

Substitute $x=6$ and $y=4$ into the original equations.

**Equation 1:**

$$
6+4=10
$$

**Equation 2:**

$$
2(6)+5(4)=12+20=32
$$

Both equations are satisfied.

### Step 4. Geometric Interpretation

The equations represent two straight lines in the coordinate plane.

The first equation can be written as

$$
y=10-x
$$

The second equation can be written as

$$
y=\frac{32}{5}-\frac{2}{5}x
$$

Their slopes are $-1$ and $-\frac{2}{5}$.

Since the slopes are different, the lines are not parallel and intersect at exactly one point.

That intersection point is $(6,4)$.

---

## Final Answer

The unique solution is

$$
(x,y)=(6,4)
$$

**Number of solutions:** Exactly one.

**Conclusion:**

Gaussian elimination gives $x=6$ and $y=4$.

Geometrically, the system has a unique solution because the two lines have different slopes and intersect at exactly one point.
