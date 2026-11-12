
# Exercise 2. Gaussian Elimination — One Solution

## Given System

We are given the following system of linear equations:

```text
x + y + z = 6
2x - y + z = 3
x + 2y - z = 2
```

The task is to solve the system using Gaussian elimination and verify the solution by substitution.

## Step 1. Construct the Augmented Matrix

The augmented matrix is:

```text
[ 1   1   1 | 6 ]
[ 2  -1   1 | 3 ]
[ 1   2  -1 | 2 ]
```

## Step 2. Eliminate the First Column

Apply the following row operations:

- R2 → R2 - 2R1
- R3 → R3 - R1

The resulting matrix is:

```text
[ 1   1   1 |  6 ]
[ 0  -3  -1 | -9 ]
[ 0   1  -2 | -4 ]
```

Swap the second and third rows to obtain a simpler pivot:

**R2 ↔ R3**

```text
[ 1   1   1 |  6 ]
[ 0   1  -2 | -4 ]
[ 0  -3  -1 | -9 ]
```

## Step 3. Eliminate the Second Column

Apply the row operation:

**R3 → R3 + 3R2**

The matrix becomes:

```text
[ 1   1   1 |   6 ]
[ 0   1  -2 |  -4 ]
[ 0   0  -7 | -21 ]
```

The matrix is now in row echelon form.

## Step 4. Back Substitution

From the third row:

$$
-7z=-21
$$

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

Therefore, the solution is:

- **x = 1**
- **y = 2**
- **z = 3**

## Step 5. Verify the Solution

Substitute the values into all three original equations.

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

## Final Answer

The solution is:

$$
\boxed{x=1,\quad y=2,\quad z=3}
$$

**Conclusion:**

Gaussian elimination reduces the system to row echelon form. Back substitution gives the unique solution $x=1$, $y=2$, and $z=3$.

All three equations are satisfied, confirming that the solution is correct.
