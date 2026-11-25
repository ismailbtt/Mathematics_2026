
# Exercise 14 – Closest Point on a Line

## Question

Given a point:

P = (4, 1)

And a line through the origin with direction:

v = (1, 2)

Using projection, find the closest point on the line, the distance from P to the line, and verify that the appropriate vector is perpendicular to the direction of the line.

---

## Solution

### 1. Calculate the Dot Product

We need to project P onto the direction vector v.

Formula:

P · v = x1*x2 + y1*y2

Substitute:

P · v = (4*1) + (1*2)

= 4 + 2

**Result:**

P · v = 6

### 2. Calculate the Squared Length of v

Formula:

||v||² = x² + y²

Substitute:

||v||² = 1² + 2²

= 1 + 4

**Result:**

||v||² = 5

### 3. Find the Closest Point on the Line

The closest point is the projection of P onto v.

Formula:

Q = proj_v(P) = (P · v / ||v||²) * v

Substitute:

Q = (6/5) * (1, 2)

**Result:**

Q = (6/5, 12/5)

This is the closest point on the line to P.

### 4. Calculate the Distance from P to the Line

The distance is the length of the perpendicular vector from Q to P.

Formula:

d = ||P - Q||

Substitute:

P - Q = (4, 1) - (6/5, 12/5)

= (20/5 - 6/5, 5/5 - 12/5)

= (14/5, -7/5)

Now calculate its length:

d = sqrt((14/5)² + (-7/5)²)

= sqrt(196/25 + 49/25)

= sqrt(245/25)

= sqrt(245)/5

= 7*sqrt(5)/5

**Result:**

d = 7*sqrt(5)/5 ≈ 3.13

### 5. Verify Perpendicularity

The vector from Q to P must be perpendicular to the direction vector v.

Calculate:

(P - Q) · v = (14/5, -7/5) · (1, 2)

= (14/5*1) + (-7/5*2)

= 14/5 - 14/5

**Result:**

(P - Q) · v = 0

Therefore, the shortest displacement is perpendicular to the line.

### 6. Geometric Interpretation

The closest point on a line is the projection of the given point onto that line.

The shortest distance from a point to a line is always measured along a perpendicular direction.

The projection creates a right angle between the line and the displacement from Q to P.

---

## Final Answers

- Closest point: Q = (6/5, 12/5)
- Perpendicular vector: P - Q = (14/5, -7/5)
- Distance: d = 7*sqrt(5)/5 ≈ 3.13
- Verification: (P - Q) · v = 0
