
# Exercise 11 – Parameter and Invertibility

## Question

Given the parameter-dependent matrix:

```text
A(t) = | 1  t |
       | t  1 |
```

Complete the following tasks:

1. Determine all values of t for which A(t) is invertible.
2. Find a formula for the inverse matrix A(t)^(-1).
3. Explain what happens at the excluded values of t.
4. Verify the inverse formula by matrix multiplication.

---

## Solution

### Step 1. Calculate the Determinant

For a 2 × 2 matrix, the determinant is calculated using:

```text
det(A) = ad - bc
```

Applying this formula:

```text
det(A(t)) = (1 × 1) - (t × t)
```

Therefore:

```text
det(A(t)) = 1 - t²
```

A matrix is invertible if its determinant is not zero.

Thus:

```text
1 - t² ≠ 0
```

Factor the expression:

```text
(1 - t)(1 + t) ≠ 0
```

Therefore:

```text
t ≠ 1
t ≠ -1
```

The matrix is invertible for all real values of t except 1 and -1.

### Step 2. Find the Inverse Matrix

The inverse formula for a 2 × 2 matrix is:

```text
A^(-1) = 1/(ad - bc) × |  d  -b |
                         | -c   a |
```

Substitute the elements of A(t):

```text
A(t)^(-1) = 1/(1 - t²) × |  1  -t |
                          | -t   1 |
```

Therefore:

```text
A(t)^(-1) = 1/(1 - t²) × |  1  -t |
                          | -t   1 |
```

This formula is valid only when:

```text
t ≠ 1 and t ≠ -1
```

### Step 3. Examine the Excluded Values

**Case 1: When t = 1**

Substitute t = 1 into the original matrix:

```text
A(1) = | 1  1 |
       | 1  1 |
```

Calculate the determinant:

```text
det(A(1)) = 1 - 1²

det(A(1)) = 0
```

The two rows are identical.

Therefore, the matrix is not invertible.

**Case 2: When t = -1**

Substitute t = -1:

```text
A(-1) = |  1  -1 |
        | -1   1 |
```

Calculate the determinant:

```text
det(A(-1)) = 1 - (-1)²

det(A(-1)) = 0
```

The second row is the negative of the first row.

Therefore, the matrix is not invertible.

At both excluded values, the denominator 1 - t² becomes zero. Therefore, the inverse formula is undefined.

### Step 4. Verify the Result

To verify the inverse, calculate:

```text
A(t) × A(t)^(-1)
```

Substitute the matrices:

```text
= 1/(1 - t²) × | 1   t | × |  1  -t |
               | t   1 |   | -t   1 |
```

Perform matrix multiplication:

```text
= 1/(1 - t²) × | (1 × 1) + (t × -t)   (1 × -t) + (t × 1) |
               | (t × 1) + (1 × -t)   (t × -t) + (1 × 1) |
```

Simplify:

```text
= 1/(1 - t²) × | 1 - t²    0     |
               |    0     1 - t² |
```

For t ≠ 1 and t ≠ -1, simplify:

```text
A(t) × A(t)^(-1) = | 1  0 |
                   | 0  1 |
```

This is the identity matrix:

```text
A(t) × A(t)^(-1) = I
```

The inverse formula is correct.

---

## Final Answer

**The matrix is invertible when:**

```text
t ∈ ℝ \ {-1, 1}
```

**The inverse matrix is:**

```text
A(t)^(-1) = 1/(1 - t²) × |  1  -t |
                          | -t   1 |
```

**Excluded values:**

```text
t = 1  →  det(A) = 0

t = -1 →  det(A) = 0
```

**Verification:**

```text
A(t) × A(t)^(-1) = I
```

**Conclusion:**

The matrix is invertible for all real values of t except t = 1 and t = -1.

At these excluded values, the determinant becomes zero, the rows are linearly dependent, and the inverse does not exist.

The inverse formula was verified by matrix multiplication, confirming that the result is correct.
