
# Exercise 1. From a System to a Matrix

## Question

Write the system

```text
2x - y + z = 4
x + 3y - 2z = 1
3x + y + z = 7
```

in the form Ax = b.

Identify the coefficient matrix, the vector of unknowns, and the right-hand side vector. Explain how each row of the matrix corresponds to one equation.

---

## Solution

### Step 1. Identify the Coefficient Matrix

The coefficient matrix A contains the coefficients of x, y, and z.

```text
    [ 2  -1   1 ]
A = [ 1   3  -2 ]
    [ 3   1   1 ]
```

### Step 2. Identify the Unknown Vector

The unknown vector contains the variables:

```text
    [ x ]
X = [ y ]
    [ z ]
```

### Step 3. Identify the Right-Hand Side Vector

The vector b contains the constants from the equations.

```text
    [ 4 ]
b = [ 1 ]
    [ 7 ]
```

### Step 4. Write the Matrix Equation

The system can be written as:

$$
AX=b
$$

Substituting the matrices:

```text
[ 2  -1   1 ] [ x ]   [ 4 ]
[ 1   3  -2 ] [ y ] = [ 1 ]
[ 3   1   1 ] [ z ]   [ 7 ]
```

### Step 5. Verify the Representation

Multiplying the coefficient matrix by the unknown vector gives:

```text
[ 2x - y + z  ]   [ 4 ]
[ x + 3y - 2z ] = [ 1 ]
[ 3x + y + z  ]   [ 7 ]
```

Each row corresponds to one equation:

- Row 1: 2x - y + z = 4
- Row 2: x + 3y - 2z = 1
- Row 3: 3x + y + z = 7

## Final Answer

The matrix representation is:

```text
[ 2  -1   1 ] [ x ]   [ 4 ]
[ 1   3  -2 ] [ y ] = [ 1 ]
[ 3   1   1 ] [ z ]   [ 7 ]
```

**Conclusion:**

The system is correctly represented in the form AX = b.

Each row of A contains the coefficients of one equation, X contains the unknowns, and b contains the constants.

