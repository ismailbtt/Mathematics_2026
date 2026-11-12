
# Exercise 1. From a System to a Matrix — Solution

## Given System

We are given the following system of linear equations:

$$
\begin{cases}
2x-y+z=4 \\
x+3y-2z=1 \\
3x+y+z=7
\end{cases}
$$

The task is to express the system in matrix form $Ax=b$ and identify its components.

## Step 1. Identify the Coefficient Matrix

The coefficient matrix $A$ contains the coefficients of the variables $x$, $y$, and $z$ in each equation.

$$
A=\begin{pmatrix}2 & -1 & 1 \\ 1 & 3 & -2 \\ 3 & 1 & 1\end{pmatrix}
$$

Each row represents the coefficients of one equation.

## Step 2. Identify the Unknown Vector

The vector of unknowns contains the variables:

$$
x=\begin{pmatrix}x \\ y \\ z\end{pmatrix}
$$

## Step 3. Identify the Right-Hand Side Vector

The vector $b$ contains the constant terms from the right-hand side of each equation.

$$
b=\begin{pmatrix}4 \\ 1 \\ 7\end{pmatrix}
$$

## Step 4. Write the Matrix Equation

The system can now be expressed as:

$$
\boxed{Ax=b}
$$

Substituting the matrices:

$$
\begin{pmatrix}2 & -1 & 1 \\ 1 & 3 & -2 \\ 3 & 1 & 1\end{pmatrix}
\begin{pmatrix}x \\ y \\ z\end{pmatrix}
=
\begin{pmatrix}4 \\ 1 \\ 7\end{pmatrix}
$$

## Step 5. Verify the Matrix Representation

Multiplying the coefficient matrix by the unknown vector gives:

$$
Ax=\begin{pmatrix}2x-y+z \\ x+3y-2z \\ 3x+y+z\end{pmatrix}
$$

Therefore, we recover the original equations:

- Row 1: $2x-y+z=4$
- Row 2: $x+3y-2z=1$
- Row 3: $3x+y+z=7$

This confirms that the matrix equation correctly represents the given system.

## Final Answer

The system in matrix form is:

$$
\boxed{
\begin{pmatrix}2 & -1 & 1 \\ 1 & 3 & -2 \\ 3 & 1 & 1\end{pmatrix}
\begin{pmatrix}x \\ y \\ z\end{pmatrix}
=
\begin{pmatrix}4 \\ 1 \\ 7\end{pmatrix}
}
$$

**Conclusion:**

The system is successfully written in the form $Ax=b$.

Each row of the coefficient matrix corresponds to one equation, the unknown vector contains the variables, and the right-hand side vector contains the constants.
