
# Exercise 12 – Finding Inverses Without Starting from Scratch

## Question

Given the inverse matrix:

```text
A^(-1) = |  2  -1 |
         | -3   2 |
```

Without finding the original matrix A, calculate:

1. (3A)^(-1)
2. (A^T)^(-1)
3. (A²)^(-1)

Verify your results using inverse matrix properties.

---

## Solution

### Step 1. Calculate (3A)^(-1)

For a nonzero scalar k, the inverse property is:

```text
(kA)^(-1) = (1/k) × A^(-1)
```

Using k = 3:

```text
(3A)^(-1) = (1/3) × A^(-1)
```

Substitute the given matrix:

```text
(3A)^(-1) = (1/3) × |  2  -1 |
                       | -3   2 |
```

Multiply each element by 1/3:

```text
(3A)^(-1) = |  2/3  -1/3 |
            |   -1   2/3 |
```

Therefore:

```text
(3A)^(-1) = |  2/3  -1/3 |
            |   -1   2/3 |
```

### Step 2. Calculate (A^T)^(-1)

The inverse of a transpose follows this property:

```text
(A^T)^(-1) = (A^(-1))^T
```

This means we transpose the given inverse matrix by switching its rows and columns.

Original matrix:

```text
A^(-1) = |  2  -1 |
         | -3   2 |
```

After transposing:

```text
(A^(-1))^T = |  2  -3 |
             | -1   2 |
```

Therefore:

```text
(A^T)^(-1) = |  2  -3 |
             | -1   2 |
```

### Step 3. Calculate (A²)^(-1)

The inverse of a product follows the property:

```text
(AB)^(-1) = B^(-1) × A^(-1)
```

Since A² = A × A:

```text
(A²)^(-1) = A^(-1) × A^(-1)
```

Therefore:

```text
(A²)^(-1) = (A^(-1))²
```

Substitute the given inverse matrix:

```text
(A²)^(-1) = |  2  -1 | × |  2  -1 |
            | -3   2 |   | -3   2 |
```

Perform matrix multiplication:

```text
(A²)^(-1) = | (2×2)+(-1×-3)   (2×-1)+(-1×2) |
            | (-3×2)+(2×-3)  (-3×-1)+(2×2) |
```

Simplify:

```text
(A²)^(-1) = | 4+3    -2-2 |
            | -6-6    3+4 |
```

Therefore:

```text
(A²)^(-1) = |  7  -4 |
            | -12   7 |
```

### Step 4. Verification

We can verify the results using inverse matrix properties without calculating the original matrix A.

**For (3A)^(-1):**

```text
(3A) × ((1/3) × A^(-1))

= A × A^(-1)

= I
```

**For (A^T)^(-1):**

```text
A^T × (A^(-1))^T

= (A^(-1) × A)^T

= I
```

**For (A²)^(-1):**

```text
A² × (A^(-1))²

= A × A × A^(-1) × A^(-1)

= A × I × A^(-1)

= A × A^(-1)

= I
```

All three expressions produce the identity matrix, confirming the results.

---

## Final Answer

**1. Inverse of 3A:**

```text
(3A)^(-1) = |  2/3  -1/3 |
            |   -1   2/3 |
```

**2. Inverse of the transpose:**

```text
(A^T)^(-1) = |  2  -3 |
             | -1   2 |
```

**3. Inverse of A squared:**

```text
(A²)^(-1) = |  7  -4 |
            | -12   7 |
```

**Conclusion:**

All three inverses were calculated using inverse matrix properties without finding the original matrix A.

The results were verified using the identity A × A^(-1) = I, confirming that the calculations are correct.

