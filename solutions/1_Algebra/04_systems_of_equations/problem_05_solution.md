
# Exercise 5. Row Echelon Form and Number of Solutions

## Question

For the augmented matrix

$$
\begin{pmatrix}
1 & 2 & -1 & \mid & 3 \\
0 & 1 & 2 & \mid & 1 \\
0 & 0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

determine the number of solutions and write them in parametric form. Explain how you know how many variables may be chosen freely.

---

## Solution

### Step 1. Interpret the Augmented Matrix

The given matrix is already in row echelon form. It represents the system

$$
\begin{cases}
x+2y-z=3, \\
y+2z=1, \\
0=0.
\end{cases}
$$

The third equation is always true and introduces no additional restriction.

There are three unknowns and two pivot columns. Therefore, one variable is free.

Since there is no contradictory equation, the system is consistent and has infinitely many solutions.

### Step 2. Find the Parametric Solution

From the second equation,

$$
y+2z=1
$$

Choose $z$ as the free variable:

$$
z=t,\qquad t\in\mathbb{R}
$$

Therefore,

$$
y=1-2t
$$

Substitute into the first equation:

$$
x+2(1-2t)-t=3
$$

Simplifying,

$$
x+2-5t=3
$$

Hence,

$$
x=1+5t
$$

The general solution is

$$
(x,y,z)=(1+5t,1-2t,t),\qquad t\in\mathbb{R}
$$

### Step 3. Verify the Solution

Substitute the parametric expressions into the original equations.

**Equation 1:**

$$
\begin{aligned}
x+2y-z &= (1+5t)+2(1-2t)-t \\
&=3
\end{aligned}
$$

**Equation 2:**

$$
\begin{aligned}
y+2z &= (1-2t)+2t \\
&=1
\end{aligned}
$$

**Equation 3:**

$$
0=0
$$

All equations are satisfied for every real value of $t$.

---

## Final Answer

The general solution is

$$
(x,y,z)=(1+5t,1-2t,t),\qquad t\in\mathbb{R}
$$

**Free variable:** $z=t$

**Number of free variables:** $3-2=1$

**Number of solutions:** Infinitely many.

**Conclusion:**

The matrix contains two pivot columns and three unknowns, leaving one free variable. The zero row does not create a contradiction, so the system is consistent. Every real value of $t$ gives a valid solution.
