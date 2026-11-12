
# Exercise 5. Row Echelon Form and Number of Solutions

## Question

For the augmented matrix

```text
[ 1   2  -1 | 3 ]
[ 0   1   2 | 1 ]
[ 0   0   0 | 0 ]
```

determine the number of solutions and write them in parametric form. Explain how you know how many variables may be chosen freely.

---

## Solution

### Step 1. Interpret the Matrix

The augmented matrix represents the system:

$$
x+2y-z=3
$$

$$
y+2z=1
$$

$$
0=0
$$

There are three unknowns and two pivot columns. The third row does not introduce any additional restriction.

Therefore, one variable is free, and the system has infinitely many solutions.

### Step 2. Find the Parametric Solution

From the second equation:

$$
y+2z=1
$$

Let $z=t$, where $t\in\mathbb{R}$.

Then:

$$
y=1-2t
$$

Substitute into the first equation:

$$
x+2(1-2t)-t=3
$$

Simplifying:

$$
x+2-5t=3
$$

Therefore:

$$
x=1+5t
$$

The general solution is:

$$
\boxed{x=1+5t,\quad y=1-2t,\quad z=t}
$$

### Step 3. Verify the Solution

Choose $t=0$.

Then:

$$
x=1,\quad y=1,\quad z=0
$$

Substituting into the original equations:

$$
1+2(1)-0=3
$$

$$
1+2(0)=1
$$

Both equations are satisfied.

## Final Answer

$$
\boxed{(x,y,z)=(1+5t,1-2t,t),\quad t\in\mathbb{R}}
$$

**Number of solutions:** Infinitely many.

**Free variable:** $z=t$.

**Conclusion:**

The system has three variables and two pivot columns, so exactly one variable is free. Because the system is consistent, every real value of $t$ gives a solution.
