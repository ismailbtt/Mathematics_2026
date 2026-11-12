
# Exercise 7. Choosing a Method Deliberately

## Question

Do not solve all of the following systems completely. For each situation, choose the method that best uses its structure and justify your choice.

**Case 1: A system with a triangular coefficient matrix**

$$
\begin{cases}
2x-y=3, \\
4y=8.
\end{cases}
$$

**Case 2:** Three systems $Ax=b_i$ with the same invertible matrix $A$, when $A^{-1}$ is already known.

**Case 3:** One $3\times3$ system for which the inverse matrix is not given and the goal is only to find one solution vector.

For Case 1, carry out the chosen method completely. For Cases 2 and 3, describe the plan and indicate which part of the computation would be reusable or unnecessary.

---

## Solution

### Step 1. Case 1 — Back Substitution

The coefficient matrix is

$$
A=
\begin{pmatrix}
2 & -1 \\
0 & 4 \\
\end{pmatrix}
$$

Since the matrix is upper triangular, back substitution is the simplest method.

From the second equation,

$$
4y=8
$$

Therefore,

$$
y=2
$$

Substitute $y=2$ into the first equation:

$$
2x-2=3
$$

$$
2x=5
$$

$$
x=\frac{5}{2}
$$

**Verification:**

$$
2\left(\frac{5}{2}\right)-2=3
$$

$$
4(2)=8
$$

Both equations are satisfied.

The solution is

$$
(x,y)=\left(\frac{5}{2},2\right)
$$

### Step 2. Case 2 — Inverse Matrix Method

We have three systems with the same invertible coefficient matrix:

$$
Ax=b_1,\qquad Ax=b_2,\qquad Ax=b_3
$$

Since $A^{-1}$ is already known, the inverse matrix method is convenient.

The solutions can be calculated directly:

$$
x_1=A^{-1}b_1
$$

$$
x_2=A^{-1}b_2
$$

$$
x_3=A^{-1}b_3
$$

The same inverse matrix is reused for all three systems.

Therefore, calculating the inverse again or performing separate elimination procedures is unnecessary.

### Step 3. Case 3 — Gaussian Elimination

For a single $3\times3$ system with an unknown inverse, Gaussian elimination is the preferred method.

The procedure is:

1. Construct the augmented matrix $[A\mid b]$.
2. Apply elementary row operations to obtain row echelon form.
3. Use back substitution to determine the unknown variables.

Gaussian elimination directly solves the system without calculating $A^{-1}$.

Since only one solution vector is required, computing the full inverse would involve unnecessary work.

---

## Final Answer

**Case 1: Back Substitution**

The triangular structure allows direct calculation.

$$
(x,y)=\left(\frac{5}{2},2\right)
$$

**Case 2: Inverse Matrix Method**

Use the known inverse matrix for each right-hand side:

$$
x_i=A^{-1}b_i,\qquad i=1,2,3
$$

The inverse matrix is reused, avoiding repeated calculations.

**Case 3: Gaussian Elimination**

Use row operations followed by back substitution. Computing the inverse matrix is unnecessary.

**Conclusion:**

The appropriate solution method depends on the structure of the coefficient matrix and the number of right-hand sides.

Back substitution is efficient for triangular systems, a known inverse is useful for multiple right-hand sides, and Gaussian elimination is generally preferable for solving a single system without a known inverse.
