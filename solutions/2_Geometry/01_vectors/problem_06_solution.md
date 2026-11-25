
# Exercise 6 – Projection and Perpendicular Component

## Question

Find the projection of u = (4, 2) onto the direction v = (1, 1).

Then compute:

r = u - proj_v(u)

Verify that r · v = 0 and explain this result geometrically.

---

## Solution

### 1. Calculate the Dot Product

Formula:

u · v = x1*x2 + y1*y2

Substitute:

u · v = (4*1) + (2*1)

= 4 + 2

**Result:**

u · v = 6

### 2. Calculate the Squared Length of v

Formula:

||v||² = x² + y²

Substitute:

||v||² = 1² + 1²

= 2

**Result:**

||v||² = 2

### 3. Find the Projection of u onto v

Projection formula:

proj_v(u) = (u · v / ||v||²) * v

Substitute:

proj_v(u) = (6/2) * (1, 1)

= 3 * (1, 1)

**Result:**

proj_v(u) = (3, 3)

### 4. Calculate the Perpendicular Component

Formula:

r = u - proj_v(u)

Substitute:

r = (4, 2) - (3, 3)

**Result:**

r = (1, -1)

### 5. Verify Perpendicularity

Two vectors are perpendicular if their dot product is zero.

Calculate:

r · v = (1*1) + (-1*1)

= 1 - 1

**Result:**

r · v = 0

Therefore, r is perpendicular to v.

### 6. Geometric Interpretation

The projection (3, 3) represents the component of u in the direction of v.

The vector r = (1, -1) represents the remaining component, which is perpendicular to v.

Together, these components reconstruct the original vector:

u = proj_v(u) + r

(4, 2) = (3, 3) + (1, -1)

---

## Final Answers

- Dot product: u · v = 6
- Squared length of v: ||v||² = 2
- Projection: proj_v(u) = (3, 3)
- Perpendicular component: r = (1, -1)
- Verification: r · v = 0
