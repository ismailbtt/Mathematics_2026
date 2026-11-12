
# Exercise 1. From a System to a Matrix — Solution

## Given System

We are given the following system of linear equations:

```text
2x - y + z = 4
x + 3y - 2z = 1
3x + y + z = 7
```

The task is to express the system in matrix form Ax = b and identify the coefficient matrix, the vector of unknowns, and the right-hand side vector.

## Step 1. Identify the Coefficient Matrix

The coefficient matrix A contains the coefficients of the variables x, y, and z from each equation.

```text
    [ 2  -1   1 ]
A = [ 1   3  -2 ]
    [ 3   1   1 ]
```

Each row corresponds to one equation in the original system.

## Step 2. Identify the Unknown Vector

The unknown vector contains the variables x, y, and z.

```text
    [ x ]
X = [ y ]
    [ z ]
```

## Step 3. Identify the Right-Hand Side Vector

The vector b contains the constant terms from the right-hand side of each equation.

```text
    [ 4 ]
b = [ 1 ]
    [ 7 ]
```

## Step 4. Write the Matrix Equation

The system can be expressed in the form:

$$
AX=b
$$

Substituting the matrices:

```text
[ 2  -1   1 ] [ x ]   [ 4 ]
[ 1   3  -2 ] [ y ] = [ 1 ]
[ 3   1   1 ] [ z ]   [ 7 ]
```

## Step 5. Verify the Matrix Representation

Multiplying the coefficient matrix by the unknown vector gives:

```text
[ 2x - y + z  ]   [ 4 ]
[ x + 3y - 2z ] = [ 1 ]
[ 3x + y + z  ]   [ 7 ]
```

This corresponds exactly to the original system.

- **Row 1:** 2x - y + z = 4
- **Row 2:** x + 3y - 2z = 1
- **Row 3:** 3x + y + z = 7

Therefore, the matrix representation is correct.

## Final Answer

The coefficient matrix is:

```text
    [ 2  -1   1 ]
A = [ 1   3  -2 ]
    [ 3   1   1 ]
```

The unknown vector is:

```text
    [ x ]
X = [ y ]
    [ z ]
```

The right-hand side vector is:

```text
    [ 4 ]
b = [ 1 ]
    [ 7 ]
```

The matrix equation is:

$$
\boxed{AX=b}
$$

**Conclusion:**

The system has been successfully expressed in matrix form. Each row of the coefficient matrix represents one equation, the unknown vector contains the variables, and the right-hand side vector contains the constants.

