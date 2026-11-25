
# Exercise 11 – Decomposition into Parallel and Perpendicular Components

## Question

Decompose u = (3, 4) into components parallel and perpendicular to v = (1, 2).

Check:

u = u_parallel + u_perpendicular

u_perpendicular · v = 0

Explain why these are two independent checks of correctness.

---

## Solution

Given:

u = (3, 4)

v = (1, 2)

### 1. Calculate the Dot Product

Formula:

u · v = x1*x2 + y1*y2

Substitute:

u · v = (3*1) + (4*2)

= 3 + 8

**Result:**

u · v = 11

### 2. Calculate the Squared Length of v

Formula:

||v||² = x² + y²

Substitute:

||v||² = 1² + 2²

= 1 + 4

**Result:**

||v||² = 5

### 3. Find the Parallel Component

The projection formula is:

u_parallel = (u · v / ||v||²) * v

Substitute:

u_parallel = (11/5) * (1, 2)

**Result:**

u_parallel = (11/5, 22/5)

### 4. Find the Perpendicular Component

Formula:

u_perpendicular = u - u_parallel

Substitute:

u_perpendicular = (3, 4) - (11/5, 22/5)

= (15/5 - 11/5, 20/5 - 22/5)

**Result:**

u_perpendicular = (4/5, -2/5)

### 5. Verify the Decomposition

We need to check:

u = u_parallel + u_perpendicular

Substitute:

u = (11/5, 22/5) + (4/5, -2/5)

= (15/5, 20/5)

**Result:**

u = (3, 4)

The original vector is reconstructed correctly.

### 6. Verify Perpendicularity

Two vectors are perpendicular if their dot product is zero.

Calculate:

u_perpendicular · v = (4/5, -2/5) · (1, 2)

= (4/5 * 1) + (-2/5 * 2)

= 4/5 - 4/5

**Result:**

u_perpendicular · v = 0

Therefore, the perpendicular component is perpendicular to v.

### 7. Geometric Interpretation

The original vector u is divided into two components:

- The parallel component points in the direction of v.
- The perpendicular component forms a 90-degree angle with v.

Together, these components reconstruct the original vector.

The two checks are independent because:

1. Reconstruction verifies that the two components add up to u.
2. Perpendicularity verifies that the second component is orthogonal to v.

Both conditions are necessary to confirm the correct decomposition.

---

## Final Answers

- u_parallel = (11/5, 22/5)
- u_perpendicular = (4/5, -2/5)
- Reconstruction: (3, 4)
- Perpendicularity: u_perpendicular · v = 0
