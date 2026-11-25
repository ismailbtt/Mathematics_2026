
# Exercise 11 – Decomposition into Parallel and Perpendicular Components

Given:

u = (3, 4)

v = (1, 2)

We need to decompose u into two components:
- A component parallel to v.
- A component perpendicular to v.

The decomposition formula is:

u = u_parallel + u_perpendicular

## 1. Calculate the Dot Product

Formula:

u · v = x1*x2 + y1*y2

Substitute the coordinates:

u · v = (3*1) + (4*2)

u · v = 3 + 8

**Result:**

u · v = 11

## 2. Calculate the Squared Length of v

Formula:

||v||² = x² + y²

Substitute:

||v||² = 1² + 2²

||v||² = 1 + 4

**Result:**

||v||² = 5

## 3. Find the Parallel Component

The projection formula is:

u_parallel = (u · v / ||v||²) * v

Substitute the values:

u_parallel = (11 / 5) * (1, 2)

Multiply:

**Result:**

u_parallel = (11/5, 22/5)

## 4. Find the Perpendicular Component

The perpendicular component is calculated by subtracting the parallel component from the original vector.

Formula:

u_perpendicular = u - u_parallel

Substitute:

u_perpendicular = (3, 4) - (11/5, 22/5)

Convert the coordinates:

u_perpendicular = (15/5 - 11/5, 20/5 - 22/5)

**Result:**

u_perpendicular = (4/5, -2/5)

## 5. Verify the Decomposition

We need to check:

u = u_parallel + u_perpendicular

Substitute:

u = (11/5, 22/5) + (4/5, -2/5)

Add the components:

u = (15/5, 20/5)

**Result:**

u = (3, 4)

The original vector is reconstructed correctly.

## 6. Verify Perpendicularity

The perpendicular component must have a dot product of zero with v.

Calculate:

u_perpendicular · v = (4/5, -2/5) · (1, 2)

= (4/5 * 1) + (-2/5 * 2)

= 4/5 - 4/5

**Result:**

u_perpendicular · v = 0

Therefore, the perpendicular component is perpendicular to v.

## 7. Geometric Interpretation

The original vector u is divided into two independent components.

The parallel component points in the same direction as v and represents the projection of u onto v.

The perpendicular component represents the remaining part of u and forms a 90-degree angle with v.

Both components together reconstruct the original vector.

The two checks confirm different properties:

1. The reconstruction check confirms that the components add up to the original vector.
2. The perpendicularity check confirms that the second component is orthogonal to v.

Both checks are necessary to verify the decomposition.

## Final Answers

- u_parallel = (11/5, 22/5)
- u_perpendicular = (4/5, -2/5)
- Reconstruction: (11/5, 22/5) + (4/5, -2/5) = (3, 4)
- Perpendicularity: u_perpendicular · v = 0


