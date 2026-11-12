
# Exercise 4. Infinitely Many Solutions

## Question

Solve the system:

```text
x + y + z = 2
2x + 2y + 2z = 4
x - y + z = 0
```

Give the solution in parametric form, identify a free variable, and for one chosen parameter value check that the resulting point satisfies the system.

---

## Solution

### Step 1. Construct the Augmented Matrix

```text
[ 1   1   1 | 2 ]
[ 2   2   2 | 4 ]
[ 1  -1   1 | 0 ]
```

### Step 2. Apply Gaussian Elimination

Apply:

**R2 → R2 - 2R1**

**R3 → R3 - R1**

The matrix becomes:

```text
[ 1   1   1 |  2 ]
[ 0   0   0 |  0 ]
[ 0  -2   0 | -2 ]
```

Swap the second and third rows:

**R2 ↔ R3**

```text
[ 1   1   1 |  2 ]
[ 0  -2   0 | -2 ]
[ 0   0   0 |  0 ]
```

Divide the second row by -2:

**R2 → (-1/2)R2**

```text
[ 1   1   1 | 2 ]
[ 0   1   0 | 1 ]
[ 0   0   0 | 0 ]
```

Eliminate the second element of the first row:

**R1 → R1 - R2**

```text
[ 1   0   1 | 1 ]
[ 0   1   0 | 1 ]
[ 0   0   0 | 0 ]
```

### Step 3. Find the Parametric Solution

The reduced matrix represents:

$$
x+z=1
$$

$$
y=1
$$

There are three variables and two pivots, so one variable is free.

Let:

$$
z=t,\quad t\in\mathbb{R}
$$

Then:

$$
x=1-t
$$

$$
y=1
$$

Therefore:

$$
\boxed{x=1-t,\quad y=1,\quad z=t}
$$

### Step 4. Verify the Solution

Choose t = 0.

Then:

$$
x=1,\quad y=1,\quad z=0
$$

Substitute into the original equations.

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

## Final Answer

The general solution is:

$$
\boxed{(x,y,z)=(1-t,1,t),\quad t\in\mathbb{R}}
$$

**Free variable:** z = t

**Number of solutions:** Infinitely many.

**Example solution:** (1, 1, 0)

**Conclusion:**

Gaussian elimination produces two pivot variables and one free variable.

The system is consistent, and every real value of t gives a valid solution.

Therefore, the system has infinitely many solutions.

