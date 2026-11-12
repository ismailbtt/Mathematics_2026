
# Exercise 3. Inconsistent System — Solution

## Given System

We are given the following system of linear equations:

```text
x + 2y = 3
2x + 4y = 7
```

The task is to determine whether the system has a solution using Gaussian elimination.

## Step 1. Construct the Augmented Matrix

The augmented matrix is:

```text
[ 1   2 | 3 ]
[ 2   4 | 7 ]
```

## Step 2. Apply Gaussian Elimination

To eliminate the first element of the second row, apply:

**R2 → R2 - 2R1**

The new second row is:

```text
[ 2   4 | 7 ] - 2[ 1   2 | 3 ]
= [ 0   0 | 1 ]
```

The augmented matrix becomes:

```text
[ 1   2 | 3 ]
[ 0   0 | 1 ]
```

## Step 3. Interpret the Result

The second row represents the equation:

$$
0x+0y=1
$$

This simplifies to:

$$
0=1
$$

This is a contradiction because zero cannot equal one.

Therefore, the system is inconsistent and has no solution.

## Step 4. Explain Using the Original Equations

The original equations are:

$$
x+2y=3
$$

$$
2x+4y=7
$$

Multiplying the first equation by 2 gives:

$$
2x+4y=6
$$

However, the second equation requires:

$$
2x+4y=7
$$

The same expression cannot equal both 6 and 7.

Therefore, no values of $x$ and $y$ can satisfy both equations simultaneously.

## Final Answer

The final augmented matrix is:

```text
[ 1   2 | 3 ]
[ 0   0 | 1 ]
```

The second row produces the contradiction:

$$
\boxed{0=1}
$$

Therefore:

**The system has no solution.**

**Conclusion:**

Gaussian elimination produces a contradictory equation, proving that the system is inconsistent.

Geometrically, the two equations represent distinct parallel lines. Since they never intersect, the system has no solution.
