

# Exercise 3. Inconsistent System

## Question

Solve or show that the following system is inconsistent:

```text
x + 2y = 3
2x + 4y = 7
```

Show how the contradiction appears in the matrix after elimination and interpret it in terms of equations.

---

## Solution

### Step 1. Construct the Augmented Matrix

```text
[ 1   2 | 3 ]
[ 2   4 | 7 ]
```

### Step 2. Apply Gaussian Elimination

Apply the row operation:

**R2 → R2 - 2R1**

Calculating the second row:

```text
[ 2   4 | 7 ] - 2[ 1   2 | 3 ]

= [ 0   0 | 1 ]
```

The resulting augmented matrix is:

```text
[ 1   2 | 3 ]
[ 0   0 | 1 ]
```

### Step 3. Identify the Contradiction

The second row represents:

$$
0x+0y=1
$$

Therefore:

$$
0=1
$$

This is impossible.

Hence, the system is inconsistent.

### Step 4. Interpret the Original Equations

The first equation is:

$$
x+2y=3
$$

Multiplying by 2:

$$
2x+4y=6
$$

However, the second equation states:

$$
2x+4y=7
$$

The same expression cannot equal both 6 and 7.

Therefore, no values of x and y can satisfy both equations.

## Final Answer

The reduced augmented matrix is:

```text
[ 1   2 | 3 ]
[ 0   0 | 1 ]
```

The contradiction is:

$$
\boxed{0=1}
$$

**Number of solutions: No solution.**

**Conclusion:**

The system is inconsistent because Gaussian elimination produces a contradictory equation.

Geometrically, the equations represent two distinct parallel lines that never intersect.

