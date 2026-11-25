
# Exercise 10 – Inverse of a Diagonal Matrix

## Question

Given the following diagonal matrices:

```text
D = | 2   0   0 |
    | 0  -3   0 |
    | 0   0   5 |

E = | 2   0   0 |
    | 0   0   0 |
    | 0   0   5 |
```

Complete the following tasks:

1. Determine which matrix is invertible.
2. Find the inverse of the invertible matrix.
3. Verify the result without using Gauss–Jordan elimination.

---

## Solution

### Step 1. Determine Invertibility

A diagonal matrix is invertible if and only if all its diagonal elements are nonzero.

For matrix D, calculate the determinant:

```text
det(D) = 2 × (-3) × 5

det(D) = -30
```

Since:

```text
det(D) ≠ 0
```

Matrix D is invertible.

For matrix E, calculate the determinant:

```text
det(E) = 2 × 0 × 5

det(E) = 0
```

Since:

```text
det(E) = 0
```

Matrix E is not invertible.

Therefore, only matrix D has an inverse.

### Step 2. Find the Inverse of D

The inverse of an invertible diagonal matrix is obtained by taking the reciprocal of each diagonal element.

The original matrix is:

```text
D = | 2   0   0 |
    | 0  -3   0 |
    | 0   0   5 |
```

Take the reciprocal of each diagonal element:

```text
2  →  1/2

-3 → -1/3

5  →  1/5
```

Therefore:

```text
D^(-1) = | 1/2    0      0   |
         |  0    -1/3    0   |
         |  0     0     1/5  |
```

### Step 3. Verify the Result

To verify the inverse, calculate:

```text
D × D^(-1)
```

Substitute the matrices:

```text
| 2   0   0 |   | 1/2    0      0   |
| 0  -3   0 | × |  0    -1/3    0   |
| 0   0   5 |   |  0     0     1/5  |
```

Since both matrices are diagonal, their product is also diagonal.

Multiply the corresponding diagonal elements:

```text
D × D^(-1) = | 2 × 1/2       0          0      |
             |     0      (-3) × (-1/3)  0      |
             |     0          0       5 × 1/5  |
```

Simplifying:

```text
D × D^(-1) = | 1   0   0 |
             | 0   1   0 |
             | 0   0   1 |
```

This is the identity matrix:

```text
D × D^(-1) = I
```

The calculated inverse is correct.

---

## Final Answer

**Matrix D is invertible because:**

```text
det(D) = -30 ≠ 0
```

**Its inverse is:**

```text
D^(-1) = | 1/2    0      0   |
         |  0    -1/3    0   |
         |  0     0     1/5  |
```

**Matrix E is not invertible because:**

```text
det(E) = 0
```

**Verification:**

```text
D × D^(-1) = I
```

**Conclusion:**

Only matrix D is invertible because all its diagonal elements are nonzero. Its inverse is obtained by taking the reciprocal of each diagonal element.

Matrix E has no inverse because it contains a zero diagonal element.
