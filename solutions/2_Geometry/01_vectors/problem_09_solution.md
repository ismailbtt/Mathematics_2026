
# Exercise 9 – Cross Product as a Perpendicular Direction

## Question

For:

u = (1, 2, 0)

v = (0, 1, 3)

Compute u × v.

Use dot products to check perpendicularity to both vectors, compute v × u, and compare the results.

---

## Solution

### 1. Calculate the Cross Product u × v

The cross product formula is:

u × v = (
    u2*v3 - u3*v2,
    u3*v1 - u1*v3,
    u1*v2 - u2*v1
)

Substitute:

u × v = (
    2*3 - 0*1,
    0*0 - 1*3,
    1*1 - 2*0
)

Calculate:

u × v = (6, -3, 1)

**Result:**

u × v = (6, -3, 1)

### 2. Verify Perpendicularity to u

Calculate the dot product:

(u × v) · u = (6, -3, 1) · (1, 2, 0)

= (6*1) + (-3*2) + (1*0)

= 6 - 6 + 0

**Result:**

(u × v) · u = 0

Therefore, the cross product is perpendicular to u.

### 3. Verify Perpendicularity to v

Calculate:

(u × v) · v = (6, -3, 1) · (0, 1, 3)

= (6*0) + (-3*1) + (1*3)

= 0 - 3 + 3

**Result:**

(u × v) · v = 0

Therefore, the cross product is also perpendicular to v.

### 4. Calculate the Reversed Cross Product v × u

The cross product changes its sign when the order of the vectors is reversed.

Formula:

v × u = -(u × v)

Substitute:

v × u = -(6, -3, 1)

**Result:**

v × u = (-6, 3, -1)

### 5. Compare the Results

We obtained:

u × v = (6, -3, 1)

v × u = (-6, 3, -1)

The two results have the same length but opposite directions.

This demonstrates that the cross product is not commutative.

Instead:

u × v = -(v × u)

### 6. Geometric Interpretation

The cross product produces a new vector perpendicular to both original vectors.

Its direction is determined by the right-hand rule.

Reversing the order of the original vectors changes the direction of the resulting vector but does not change its length.

---

## Final Answers

- u × v = (6, -3, 1)
- (u × v) · u = 0
- (u × v) · v = 0
- v × u = (-6, 3, -1)
- u × v = -(v × u)
