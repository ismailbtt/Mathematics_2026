
# Exercise 10. A Polynomial Through Three Points

## Question

Find a polynomial

$$
p(x)=ax^2+bx+c
$$

whose graph passes through the points $(0,1)$, $(1,3)$, and $(2,9)$.

Reduce the problem to a system of linear equations and check the result by substituting all three points.

---

## Solution

### Step 1. Construct the System of Equations

The polynomial is

$$
p(x)=ax^2+bx+c
$$

Substitute each given point.

**Point $(0,1)$:**

$$
a(0)^2+b(0)+c=1
$$

Therefore,

$$
c=1
$$

**Point $(1,3)$:**

$$
a(1)^2+b(1)+c=3
$$

Therefore,

$$
a+b+c=3
$$

**Point $(2,9)$:**

$$
a(2)^2+b(2)+c=9
$$

Therefore,

$$
4a+2b+c=9
$$

The resulting system is

$$
\begin{cases}
c=1, \\
a+b+c=3, \\
4a+2b+c=9.
\end{cases}
$$

### Step 2. Solve the System

Since $c=1$, substitute it into the remaining equations.

$$
a+b+1=3
$$

$$
4a+2b+1=9
$$

Simplifying,

$$
\begin{cases}
a+b=2, \\
4a+2b=8.
\end{cases}
$$

Multiply the first equation by $2$:

$$
2a+2b=4
$$

Subtract it from the second equation:

$$
2a=4
$$

Therefore,

$$
a=2
$$

Substitute $a=2$ into $a+b=2$:

$$
2+b=2
$$

Thus,

$$
b=0
$$

We have obtained

$$
a=2,\qquad b=0,\qquad c=1
$$

### Step 3. Write the Polynomial

Substitute the coefficients into the polynomial:

$$
p(x)=2x^2+0x+1
$$

Therefore,

$$
p(x)=2x^2+1
$$

### Step 4. Verify the Result

Check all three points.

**Point $(0,1)$:**

$$
p(0)=2(0)^2+1=1
$$

**Point $(1,3)$:**

$$
p(1)=2(1)^2+1=3
$$

**Point $(2,9)$:**

$$
p(2)=2(2)^2+1=9
$$

All three points satisfy the polynomial.

---

## Final Answer

The coefficients are

$$
a=2,\qquad b=0,\qquad c=1
$$

The required polynomial is

$$
p(x)=2x^2+1
$$

**Conclusion:**

The three given points produce a system of three linear equations in the unknown coefficients $a$, $b$, and $c$.

Solving this system gives the polynomial $p(x)=2x^2+1$.

Substitution confirms that the polynomial passes through all three points.
