
# Exercise 2. Gaussian Elimination — One Solution

## Question

Solve using Gaussian elimination:

```text
x + y + z = 6
2x - y + z = 3
x + 2y - z = 2
```

After solving, substitute the result into all equations and check consistency.

---

## Solution

### Step 1. Construct the Augmented Matrix

```text
[ 1   1   1 | 6 ]
[ 2  -1   1 | 3 ]
[ 1   2  -1 | 2 ]
```

### Step 2. Apply Gaussian Elimination

Apply:

**R2 → R2 - 2R1**

**R3 → R3 - R1**

The matrix becomes:

```text
[ 1   1   1 |  6 ]
[ 0  -3  -1 | -9 ]
[ 0   1  -2 | -4 ]
```

Swap the second and third rows:

**R2 ↔ R3**

```text
[ 1   1   1 |  6 ]
[ 0   1  -2 | -4 ]
[ 0  -3  -1 | -9 ]
```

Apply:

**R3 → R3 + 3R2**

```text
[ 1   1   1 |   6 ]
[ 0   1  -2 |  -4 ]
[ 0   0  -7 | -21 ]
```

The matrix is now in row echelon form.

### Step 3. Back Substitution

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

$$
y-2(3)=-4
$$

$$
y=2
$$

From the first row:

$$
x+y+z=6
$$

$$
x+2+3=6
$$

$$
x=1
$$

### Step 4. Verify the Solution

Substitute x = 1, y = 2, and z = 3.

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

$$
\boxed{x=1,\quad y=2,\quad z=3}
$$

**Conclusion:**

Gaussian elimination gives exactly one solution.

The coefficient matrix has three pivot positions, so there are no free variables.

Substitution confirms that the solution satisfies all three equations.
