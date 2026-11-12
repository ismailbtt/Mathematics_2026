
# Exercise 1. From a System to a Matrix

## Question

Write the system

$$
\begin{cases}
2x-y+z=4, \\
x+3y-2z=1, \\
3x+y+z=7.
\end{cases}
$$

in the form $Ax=b$.

Identify the coefficient matrix, the vector of unknowns, and the right-hand side vector. Explain how each row of the matrix corresponds to one equation.

---

## Solution

### Step 1. Identify the Coefficient Matrix

The coefficient matrix $A$ contains the coefficients of the variables $x$, $y$, and $z$.

$$
A=
\begin{pmatrix}
2 & -1 & 1 \\
1 & 3 & -2 \\
3 & 1 & 1 \\
\end{pmatrix}
$$

### Step 2. Identify the Unknown Vector

The vector of unknowns is

$$
x=
\begin{pmatrix}
x \\
y \\
z \\
\end{pmatrix}
$$

### Step 3. Identify the Right-Hand Side Vector

The right-hand side vector contains the constants from the equations.

$$
b=
\begin{pmatrix}
4 \\
1 \\
7 \\
\end{pmatrix}
$$


### Step 4. Write the Matrix Equation

Using the coefficient matrix, unknown vector, and right-hand side vector identified above, the system can be written as

$$
Ax=b
$$

This matrix equation represents all three original equations.

### Step 5. Verify the Representation

Multiplying each row of the coefficient matrix by the unknown vector gives the following equations:

**Row 1:**

$$
2x-y+z=4
$$

**Row 2:**

$$
x+3y-2z=1
$$

**Row 3:**

$$
3x+y+z=7
$$

These equations are identical to the original system.

Therefore, the matrix representation is correct.


### Step 5. Verify the Representation

Multiplying the coefficient matrix by the unknown vector gives

$$
Ax=
\begin{pmatrix}
2x-y+z \\
x+3y-2z \\
3x+y+z \\
\end{pmatrix}
=
\begin{pmatrix}
4 \\
1 \\
7 \\
\end{pmatrix}
$$

Each row corresponds to one equation:

- Row 1 represents $2x-y+z=4$.
- Row 2 represents $x+3y-2z=1$.
- Row 3 represents $3x+y+z=7$.

Therefore, the matrix equation correctly represents the original system.

## Final Answer

The system in matrix form is

$$
Ax=b
$$

where

$$
A=
\begin{pmatrix}
2 & -1 & 1 \\
1 & 3 & -2 \\
3 & 1 & 1 \\
\end{pmatrix}
$$

$$
x=
\begin{pmatrix}
x \\
y \\
z \\
\end{pmatrix}
$$

$$
b=
\begin{pmatrix}
4 \\
1 \\
7 \\
\end{pmatrix}
$$

**Conclusion:**

The system is correctly expressed in matrix form. Each row of $A$ contains the coefficients of one equation, the vector $x$ contains the unknowns, and $b$ contains the constant terms.
