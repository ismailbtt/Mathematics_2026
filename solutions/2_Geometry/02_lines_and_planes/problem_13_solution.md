
# Exercise 13 – Closest Point on a Plane

## Question

Find the point on the plane:

x + 2y + 2z = 4

closest to:

P = (3, 0, 0)

Give the distance and check that the segment joining the two points is perpendicular to the plane.

## Solution

### Step 1: Identify the Given Information

The given point is:

P = (3, 0, 0)

The plane equation is:

x + 2y + 2z = 4

We can identify the normal vector from the coefficients of x, y, and z:

n = (1, 2, 2)

The closest point on a plane to a given point is its orthogonal projection onto the plane.

The projection lies in the normal direction.

### Step 2: Write the Projection Formula

For a plane of the form:

n · x = d

the orthogonal projection H of a point P is:

H = P - [(n · P - d) / ||n||²]n

In this exercise:

n = (1, 2, 2)

P = (3, 0, 0)

d = 4

We need to calculate the dot product and the squared magnitude of the normal vector.

### Step 3: Calculate the Dot Product

Calculate:

n · P = (1)(3) + (2)(0) + (2)(0)

n · P = 3

Therefore:

n · P - d = 3 - 4 = -1

### Step 4: Calculate the Squared Magnitude of the Normal Vector

The magnitude is:

||n|| = √(1² + 2² + 2²)

||n|| = √(1 + 4 + 4)

||n|| = √9 = 3

Therefore:

||n||² = 9

### Step 5: Calculate the Orthogonal Projection

Substitute the values into the projection formula:

H = P - [(-1) / 9]n

H = P + (1/9)n

Substitute P and n:

H = (3, 0, 0) + (1/9)(1, 2, 2)

Calculate each coordinate:

H = (3 + 1/9, 0 + 2/9, 0 + 2/9)

Therefore:

H = (28/9, 2/9, 2/9)

This is the closest point on the plane to P.

### Step 6: Calculate the Distance

The distance from a point to a plane is:

distance = |n · P - d| / ||n||

Substitute:

distance = |3 - 4| / 3

distance = 1/3

Therefore, the shortest distance is:

d = 1/3

### Step 7: Verify That the Projection Lies on the Plane

Substitute H = (28/9, 2/9, 2/9) into the plane equation:

x + 2y + 2z = 4

28/9 + 2(2/9) + 2(2/9) = 4

28/9 + 4/9 + 4/9 = 4

36/9 = 4

4 = 4

Therefore, H lies on the plane.

### Step 8: Check Perpendicularity

Calculate the vector from P to H:

PH = H - P

PH = (28/9 - 3, 2/9 - 0, 2/9 - 0)

PH = (1/9, 2/9, 2/9)

Recall that the normal vector is:

n = (1, 2, 2)

We can see that:

PH = (1/9)n

Therefore, PH is a scalar multiple of the normal vector.

This proves that the segment PH is perpendicular to the plane.

## Final Answer

**Closest point on the plane:**

H = (28/9, 2/9, 2/9)

**Shortest distance:**

d = 1/3

**Normal vector:**

n = (1, 2, 2)

**Perpendicularity verification:**

PH = (1/9)n

Therefore, the segment joining P and H is perpendicular to the plane, and H is the closest point.
