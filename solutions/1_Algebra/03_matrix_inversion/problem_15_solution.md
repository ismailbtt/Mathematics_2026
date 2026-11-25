
# Exercise 15 – Two Methods for Solving the Same System

## Question

We are given the system:

Ax = b

where:

```text
A = [ 2  1 ]       b = [ 7 ]
    [ 1  3 ]           [ 8 ]
```

The task is to solve the system using two methods:

1. The inverse matrix method.
2. Gaussian elimination.

We will compare the methods and verify the solution.

## Solution

## Method 1: Using the Inverse Matrix

### Step 1: Calculate the Determinant

The determinant of A is:

det(A) = (2)(3) - (1)(1)

det(A) = 6 - 1 = 5

Since det(A) ≠ 0, the inverse exists.

### Step 2: Find the Inverse

Using the inverse formula:

```text
A⁻¹ = 1/5 [  3  -1 ]
          [ -1   2 ]
```

### Step 3: Calculate x

The solution is:

x = A⁻¹b

Substituting:

```text
x = 1/5 [  3  -1 ] [ 7 ]
        [ -1   2 ] [ 8 ]
```

Performing matrix multiplication:

```text
x = 1/5 [ 21 - 8 ]
        [ -7 + 16 ]

x = 1/5 [ 13 ]
        [  9 ]
```

Therefore:

```text
x = [ 13/5 ]
    [  9/5 ]
```

## Method 2: Using Gaussian Elimination

### Step 1: Construct the Augmented Matrix

The system is:

2x₁ + x₂ = 7

x₁ + 3x₂ = 8

The augmented matrix is:

```text
[ 2  1 | 7 ]
[ 1  3 | 8 ]
```

### Step 2: Swap the Rows

Apply:

R₁ ↔ R₂

The matrix becomes:

```text
[ 1  3 | 8 ]
[ 2  1 | 7 ]
```

### Step 3: Eliminate the First Element of Row 2

Apply:

R₂ → R₂ - 2R₁

The matrix becomes:

```text
[ 1  3 |  8 ]
[ 0 -5 | -9 ]
```

Divide the second row by -5:

R₂ → (-1/5)R₂

Therefore:

```text
[ 1  3 |   8 ]
[ 0  1 | 9/5 ]
```

### Step 4: Find the Solution

Eliminate the element above the second pivot:

R₁ → R₁ - 3R₂

The resulting matrix is:

```text
[ 1  0 | 13/5 ]
[ 0  1 |  9/5 ]
```

Therefore:

x₁ = 13/5

x₂ = 9/5

The solution vector is:

```text
x = [ 13/5 ]
    [  9/5 ]
```

## Step 5: Verify the Solution

To verify, substitute the result into the original equation:

Ax = b

```text
[ 2  1 ] [ 13/5 ] 
[ 1  3 ] [  9/5 ]
```

Performing matrix multiplication:

```text
= [ 26/5 + 9/5  ]
  [ 13/5 + 27/5 ]

= [ 35/5 ]
  [ 40/5 ]

= [ 7 ]
  [ 8 ] = b
```

The solution satisfies the original system.

## Step 6: Compare the Two Methods

**Inverse Matrix Method:**

- Requires calculating the determinant.
- Requires finding the inverse matrix.
- Uses matrix multiplication to obtain the solution.

**Gaussian Elimination:**

- Uses elementary row operations.
- Does not require calculating the inverse.
- Directly reduces the system to obtain the unknown variables.

In this example, Gaussian elimination required one row swap and three additional row operations.

The inverse matrix method required a determinant calculation, construction of the inverse, and matrix multiplication.

Both methods are straightforward for this small system, but Gaussian elimination is slightly simpler because it avoids calculating the inverse matrix.

## Final Answer

Both methods give the same solution:

```text
x = [ 13/5 ]
    [  9/5 ]
```

**Verification:**

Ax = [ 7 ] = b
    [ 8 ]

**Conclusion:**

Both the inverse matrix method and Gaussian elimination produce the same correct solution.

Gaussian elimination is slightly more efficient in this example because it solves the system directly without computing the inverse matrix.

Therefore, Gaussian elimination is the simpler method for this particular system.
