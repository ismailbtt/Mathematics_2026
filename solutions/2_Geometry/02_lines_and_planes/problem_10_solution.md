
# Exercise 10 – Projection of a Point onto a Plane

## Question

Find the orthogonal projection of P = (2, 1, 3) onto the plane:

x + y + z = 3

Then find the reflection of P across this plane.

Check that the midpoint of the segment joining the point and its reflection lies on the plane.

## Solution

### Step 1: Identify the Normal Vector

The plane is:

x + y + z = 3

Its normal vector is:

n = (1, 1, 1)

The given point is:

P = (2, 1, 3)

### Step 2: Calculate the Projection

The orthogonal projection of a point onto a plane is:

H = P - [(n · P - d) / ||n||²]n

Here:

n = (1, 1, 1)

d = 3

Calculate the dot product:

n · P = (1)(2) + (1)(1) + (1)(3)

n · P = 2 + 1 + 3 = 6

Calculate the squared magnitude:

||n||² = 1² + 1² + 1²

||n||² = 3

Substitute into the formula:

H = (2, 1, 3) - [(6 - 3) / 3](1, 1, 1)

H = (2, 1, 3) - (1, 1, 1)

Therefore:

H = (1, 0, 2)

### Step 3: Verify the Projection

Substitute H = (1, 0, 2) into the plane equation:

1 + 0 + 2 = 3

The projection lies on the plane.

### Step 4: Find the Reflection

The projection H is the midpoint between the original point P and its reflection P'.

Therefore:

P' = 2H - P

Substitute:

P' = 2(1, 0, 2) - (2, 1, 3)

P' = (2, 0, 4) - (2, 1, 3)

Therefore:

P' = (0, -1, 1)

### Step 5: Check the Midpoint

Calculate the midpoint of P and P':

M = (P + P') / 2

M = [(2, 1, 3) + (0, -1, 1)] / 2

M = (2, 0, 4) / 2

M = (1, 0, 2)

This is exactly the projection point H.

Check whether M lies on the plane:

1 + 0 + 2 = 3

Therefore, the midpoint lies on the plane.

## Final Answer

**Orthogonal projection:**

H = (1, 0, 2)

**Reflection:**

P' = (0, -1, 1)

**Midpoint verification:**

M = (1, 0, 2)

Since 1 + 0 + 2 = 3, the midpoint lies on the plane.

Therefore, the projection and reflection are correct.
