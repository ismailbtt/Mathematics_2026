
## Exercise 14: A System of Equations and the Determinant

### Given Matrix

Consider the system:

$$
Ax=b
$$

where:

$$
A=
\begin{pmatrix}
1&2\\
k&4
\end{pmatrix}
$$

We need to determine:

1. For which values of k the system has exactly one solution for every b.
2. For the remaining value of k, give an example where the system has infinitely many solutions.
3. Give an example where the system has no solution.

### Step 1: Calculate the Determinant

For a 2×2 matrix:

$$
A=
\begin{pmatrix}
a&b\\
c&d
\end{pmatrix}
$$

The determinant formula is:

$$
\det(A)=ad-bc
$$

Applying the formula:

$$
\det(A)=1(4)-2(k)
$$

Therefore:

$$
\boxed{\det(A)=4-2k}
$$

### Step 2: Find the Values for a Unique Solution

A square system Ax = b has exactly one solution for every b if and only if A is invertible.

A matrix is invertible when its determinant is nonzero.

Therefore:

$$
\det(A)\neq0
$$

Substitute:

$$
4-2k\neq0
$$

Solving:

$$
2k\neq4
$$

$$
\boxed{k\neq2}
$$

Thus, the system has exactly one solution for every b whenever k is not equal to 2.

### Step 3: Investigate the Case k = 2

Substitute k = 2 into A:

$$
A=
\begin{pmatrix}
1&2\\
2&4
\end{pmatrix}
$$

The determinant becomes:

$$
\det(A)=1(4)-2(2)
$$

$$
=4-4=0
$$

Therefore, A is not invertible.

Notice that the second row is twice the first row:

$$
R_2=2R_1
$$

This means the equations are linearly dependent on the left-hand side.

Depending on b, the system may have infinitely many solutions or no solution.

### Step 4: Example with Infinitely Many Solutions

Choose:

$$
b=
\begin{pmatrix}
1\\
2
\end{pmatrix}
$$

The system becomes:

$$
\begin{pmatrix}
1&2\\
2&4
\end{pmatrix}
\begin{pmatrix}
x\\
y
\end{pmatrix}
=
\begin{pmatrix}
1\\
2
\end{pmatrix}
$$

This gives the equations:

$$
x+2y=1
$$

$$
2x+4y=2
$$

The second equation is exactly twice the first equation.

Therefore, both equations represent the same line.

We can express x in terms of y:

$$
x=1-2y
$$

Let:

$$
y=t
$$

Then:

$$
x=1-2t
$$

The general solution is:

$$
\boxed{
\begin{pmatrix}
x\\
y
\end{pmatrix}
=
\begin{pmatrix}
1-2t\\
t
\end{pmatrix},
\quad t\in\mathbb{R}
}
$$

Since t can take infinitely many values, the system has infinitely many solutions.

### Step 5: Example with No Solution

Now choose:

$$
b=
\begin{pmatrix}
1\\
3
\end{pmatrix}
$$

The system becomes:

$$
\begin{pmatrix}
1&2\\
2&4
\end{pmatrix}
\begin{pmatrix}
x\\
y
\end{pmatrix}
=
\begin{pmatrix}
1\\
3
\end{pmatrix}
$$

This gives:

$$
x+2y=1
$$

$$
2x+4y=3
$$

Multiply the first equation by 2:

$$
2x+4y=2
$$

But the second equation requires:

$$
2x+4y=3
$$

This is a contradiction:

$$
2\neq3
$$

Therefore, the system has no solution.

$$
\boxed{\text{No solution}}
$$

### Step 6: Explanation

The determinant determines whether a square matrix is invertible.

If:

$$
\det(A)\neq0
$$

the matrix is invertible, and the system has exactly one solution for every right-hand side b.

If:

$$
\det(A)=0
$$

the matrix is singular.

In this exercise, when k = 2, the two rows of A are linearly dependent.

If the right-hand side follows the same relationship, the system has infinitely many solutions.

If the right-hand side does not follow the same relationship, the system is inconsistent and has no solution.

### Step 7: Verification

**Case 1: Unique solution**

For k different from 2:

$$
\det(A)=4-2k\neq0
$$

Therefore, A is invertible and every system Ax = b has exactly one solution.

**Case 2: Infinitely many solutions**

For k = 2 and:

$$
b=\begin{pmatrix}1\\2\end{pmatrix}
$$

Substitute:

$$
x=1-2t,\quad y=t
$$

Into the first equation:

$$
(1-2t)+2t=1
$$

Into the second equation:

$$
2(1-2t)+4t=2
$$

Both equations hold for every real t.

**Case 3: No solution**

For k = 2 and:

$$
b=\begin{pmatrix}1\\3\end{pmatrix}
$$

The equations require:

$$
2x+4y=2
$$

and:

$$
2x+4y=3
$$

These cannot both be true.

Therefore, no solution exists.

### Final Answer

The system has exactly one solution for every b when:

$$
\boxed{k\neq2}
$$

For k = 2:

**Infinitely many solutions:**

Choose:

$$
\boxed{
b=\begin{pmatrix}
1\\
2
\end{pmatrix}
}
$$

The solution set is:

$$
\boxed{
(x,y)=(1-2t,t),\quad t\in\mathbb{R}
}
$$

**No solution:**

Choose:

$$
\boxed{
b=\begin{pmatrix}
1\\
3
\end{pmatrix}
}
$$

This system is inconsistent.

**Conclusion:** The determinant is 4 - 2k. When k is not equal to 2, the matrix is invertible and the system has exactly one solution for every b. When k = 2, the matrix is singular, and the system can have either infinitely many solutions or no solution, depending on the right-hand side.
