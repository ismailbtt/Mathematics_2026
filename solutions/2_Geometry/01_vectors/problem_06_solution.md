
# Exercise 6 – Projection and Perpendicular Component

Given:

u = (4, 2)

v = (1, 1)

We need to find the projection of u onto v, calculate the perpendicular component, and verify that the result is perpendicular to v.

## 1. Calculate the Dot Product

Formula:

u · v = x1*x2 + y1*y2

Substitute the coordinates:

u · v = (4*1) + (2*1)

u · v = 4 + 2

**Result:**

u · v = 6

## 2. Calculate the Length Squared of v

Formula:

||v||² = x² + y²

Substitute:

||v||² = 1² + 1²

||v||² = 1 + 1

**Result:**

||v||² = 2

## 3. Find the Projection of u onto v

The projection formula is:

proj_v(u) = (u · v / ||v||²) * v

Substitute the values:

proj_v(u) = (6 / 2) * (1, 1)

proj_v(u) = 3 * (1, 1)

**Result:**

proj_v(u) = (3, 3)

## 4. Calculate the Perpendicular Component

The perpendicular component is:

r = u - proj_v(u)

Substitute the values:

r = (4, 2) - (3, 3)

**Result:**

r = (1, -1)

## 5. Verify Perpendicularity

Two vectors are perpendicular if their dot product is zero.

Calculate:

r · v = (1*1) + (-1*1)

r · v = 1 - 1

**Result:**

r · v = 0

Therefore, r is perpendicular to v.

## 6. Geometric Interpretation

The projection (3, 3) represents the component of u in the direction of v.

The vector r = (1, -1) represents the remaining component, which is perpendicular to v.

Together, these two components reconstruct the original vector:

u = proj_v(u) + r

(4, 2) = (3, 3) + (1, -1)

This shows that every vector can be decomposed into parallel and perpendicular components relative to a given direction.

## Final Answers

- Dot product: u · v = 6
- Squared length of v: ||v||² = 2
- Projection: proj_v(u) = (3, 3)
- Perpendicular component: r = (1, -1)
- Verification: r · v = 0

