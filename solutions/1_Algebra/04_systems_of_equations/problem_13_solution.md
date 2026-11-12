
# Exercise 13. Does Every Equation Add New Information?

## Question

Consider the system

$$
\begin{cases}
x_1+x_2=10, \\
x_2+x_3=8, \\
x_1-x_3=2.
\end{cases}
$$

Solve it and check whether all three equations are independently necessary to describe the solution set.

If one equation follows from the others, show this by calculation.

---

## Solution

### Step 1. Construct the Augmented Matrix

The augmented matrix is

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 10 \\
0 & 1 & 1 & \mid & 8 \\
1 & 0 & -1 & \mid & 2 \\
\end{pmatrix}
$$

### Step 2. Apply Gaussian Elimination

Eliminate the first entry of the third row:

$$
R_3 \to R_3-R_1
$$

The resulting matrix is

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 10 \\
0 & 1 & 1 & \mid & 8 \\
0 & -1 & -1 & \mid & -8 \\
\end{pmatrix}
$$

Next, apply

$$
R_3 \to R_3+R_2
$$

We obtain

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 10 \\
0 & 1 & 1 & \mid & 8 \\
0 & 0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

The third row becomes zero, indicating that one equation is redundant.

### Step 3. Find the Parametric Solution

The remaining equations are

$$
x_1+x_2=10
$$

$$
x_2+x_3=8
$$

There are three variables and two pivot columns, so one variable is free.

Let

$$
x_2=t,\qquad t\in\mathbb{R}
$$

Then

$$
x_1=10-t
$$

$$
x_3=8-t
$$

Therefore, the general solution is

$$
(x_1,x_2,x_3)=(10-t,t,8-t),\qquad t\in\mathbb{R}
$$

### Step 4. Identify the Redundant Equation

Subtract the second equation from the first:

$$
(x_1+x_2)-(x_2+x_3)=10-8
$$

Simplifying,

$$
x_1-x_3=2
$$

This is exactly the third equation.

Therefore, the third equation follows from the first two and does not provide new information.

### Step 5. Verify the Solution

Substitute the parametric solution into all three equations.

**Equation 1:**

$$
(10-t)+t=10
$$

**Equation 2:**

$$
t+(8-t)=8
$$

**Equation 3:**

$$
(10-t)-(8-t)=2
$$

All three equations are satisfied for every real value of $t$.

---

## Final Answer

The general solution is

$$
(x_1,x_2,x_3)=(10-t,t,8-t),\qquad t\in\mathbb{R}
$$

**Free variable:** $x_2=t$

**Number of solutions:** Infinitely many.

**Redundant equation:**

$$
x_1-x_3=2
$$

**Conclusion:**

The third equation is redundant because it can be obtained by subtracting the second equation from the first.

Only two equations are independent. Since the system has three variables and one free variable, it has infinitely many solutions.

The parametric solution satisfies all three equations.
