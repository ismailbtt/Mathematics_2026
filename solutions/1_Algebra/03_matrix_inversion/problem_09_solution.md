
# Exercise 9 – Cross Product and Perpendicularity

## Question

Given the vectors:

- u = (1, 2, 0)
- v = (0, 1, 3)

Complete the following tasks:

1. Compute the cross product u × v.
2. Use dot products to check whether the result is perpendicular to both vectors.
3. Compute v × u.
4. Compare the results of u × v and v × u.

---

## Solution

### Step 1. Calculate the Cross Product

Given:

```text
u = (1, 2, 0)
v = (0, 1, 3)
```

The cross product is calculated using the determinant:

```text
u × v = |  i   j   k  |
        |  1   2   0  |
        |  0   1   3  |
```

Expanding the determinant:

```text
u × v = i(2 × 3 - 0 × 1)
      - j(1 × 3 - 0 × 0)
      + k(1 × 1 - 2 × 0)
```

Calculate each component:

```text
u × v = i(6) - j(3) + k(1)
```

Therefore:

```text
u × v = (6, -3, 1)
```

### Step 2. Check Perpendicularity to Vector u

Two vectors are perpendicular if their dot product is zero.

Calculate:

```text
u · (u × v) = (1, 2, 0) · (6, -3, 1)
```

```text
= (1 × 6) + (2 × -3) + (0 × 1)
```

```text
= 6 - 6 + 0
= 0
```

Therefore, the cross product is perpendicular to vector u.

### Step 3. Check Perpendicularity to Vector v

Calculate:

```text
v · (u × v) = (0, 1, 3) · (6, -3, 1)
```

```text
= (0 × 6) + (1 × -3) + (3 × 1)
```

```text
= 0 - 3 + 3
= 0
```

Therefore, the cross product is also perpendicular to vector v.

### Step 4. Calculate the Reverse Cross Product

Now calculate:

```text
v × u
```

Using the cross product formula:

```text
v × u = |  i   j   k  |
        |  0   1   3  |
        |  1   2   0  |
```

Expanding:

```text
v × u = i(1 × 0 - 3 × 2)
      - j(0 × 0 - 3 × 1)
      + k(0 × 2 - 1 × 1)
```

Simplifying:

```text
v × u = (-6, 3, -1)
```

### Step 5. Compare the Results

We obtained:

```text
u × v = (6, -3, 1)

v × u = (-6, 3, -1)
```

Comparing the two results:

```text
v × u = -(u × v)
```

The cross product is not commutative. Reversing the order of the vectors changes the direction of the result but keeps its magnitude the same.

---

## Final Answers

**1. Cross Product:**

```text
u × v = (6, -3, 1)
```

**2. Perpendicularity Checks:**

```text
u · (u × v) = 0

v · (u × v) = 0
```

The cross product is perpendicular to both original vectors.

**3. Reverse Cross Product:**

```text
v × u = (-6, 3, -1)
```

**4. Comparison:**

```text
v × u = -(u × v)
```

**Conclusion:**

The cross product produces a vector perpendicular to both original vectors. Reversing the order of the vectors changes the direction of the cross product, resulting in the negative of the original vector.
