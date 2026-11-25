
# Exercise 12 – A Normal Vector to a Plane

## Question

Given:

A = (1, 0, 2)

B = (2, 1, 0)

C = (0, 3, 1)

Construct two vectors lying in the plane, find a vector perpendicular to both, and check the perpendicularity using dot products.

---

## Solution

### 1. Construct the First Vector AB

To find the vector from A to B:

AB = B - A

AB = (2 - 1, 1 - 0, 0 - 2)

**Result:**

AB = (1, 1, -2)

### 2. Construct the Second Vector AC

To find the vector from A to C:

AC = C - A

AC = (0 - 1, 3 - 0, 1 - 2)

**Result:**

AC = (-1, 3, -1)

Both vectors lie in the plane determined by A, B, and C.

### 3. Find a Normal Vector Using the Cross Product

A vector perpendicular to both AB and AC can be found using the cross product.

Formula:

n = AB × AC

Substitute:

n = (1, 1, -2) × (-1, 3, -1)

Calculate each component:

n = (
    1*(-1) - (-2*3),
    (-2)*(-1) - 1*(-1),
    1*3 - 1*(-1)
)

n = (-1 + 6, 2 + 1, 3 + 1)

**Result:**

n = (5, 3, 4)

### 4. Verify Perpendicularity to AB

Calculate the dot product:

n · AB = (5, 3, 4) · (1, 1, -2)

= (5*1) + (3*1) + (4*(-2))

= 5 + 3 - 8

**Result:**

n · AB = 0

Therefore, n is perpendicular to AB.

### 5. Verify Perpendicularity to AC

Calculate:

n · AC = (5, 3, 4) · (-1, 3, -1)

= (5*(-1)) + (3*3) + (4*(-1))

= -5 + 9 - 4

**Result:**

n · AC = 0

Therefore, n is also perpendicular to AC.

### 6. Geometric Interpretation

The vectors AB and AC lie in the same plane.

Their cross product produces a normal vector perpendicular to both directions.

The normal vector is useful for describing the orientation of a plane in three-dimensional space.

Since both dot products are zero, the normal vector is perpendicular to the plane's two constructed directions.

---

## Final Answers

- AB = (1, 1, -2)
- AC = (-1, 3, -1)
- Normal vector: n = (5, 3, 4)
- n · AB = 0
- n · AC = 0
