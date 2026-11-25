
# Exercise 14 – Contrast: Intersection and Parallelism

## Question

From the point:

P = (0, 0, 1)

two lines are drawn with direction vectors:

v₁ = (2, 1, -1)

v₂ = (2, 1, 0)

For each line, analyze its position relative to the plane:

z = 0

For the line that intersects the plane, find the intersection point.

For the other line, explain how you can recognize parallelism without solving an equation.

## Solution

### Step 1: Identify the Plane's Normal Vector

The plane is:

z = 0

We can write it as:

0x + 0y + 1z = 0

Therefore, its normal vector is:

n = (0, 0, 1)

The given starting point is:

P = (0, 0, 1)

Both lines pass through this point.

### Step 2: Analyze the First Line

The first direction vector is:

v₁ = (2, 1, -1)

The line equation is:

L₁ = (0, 0, 1) + t(2, 1, -1)

Its parametric equations are:

x = 2t

y = t

z = 1 - t

To determine its relationship with the plane, calculate the dot product:

v₁ · n = (2)(0) + (1)(0) + (-1)(1)

v₁ · n = -1

Since the dot product is not zero, the direction vector is not parallel to the plane.

Therefore, the line intersects the plane at exactly one point.

### Step 3: Find the Intersection Point of the First Line

The plane equation is:

z = 0

Substitute the line's z-coordinate:

1 - t = 0

t = 1

Now substitute t = 1 into the other coordinates:

x = 2(1) = 2

y = 1

z = 0

Therefore, the intersection point is:

Q = (2, 1, 0)

### Step 4: Verify the Intersection Point

Check the point on the line:

(0, 0, 1) + 1(2, 1, -1)

= (2, 1, 0)

Check the point on the plane:

z = 0

The point Q = (2, 1, 0) satisfies the plane equation.

Therefore, the intersection is correct.

### Step 5: Analyze the Second Line

The second direction vector is:

v₂ = (2, 1, 0)

The line equation is:

L₂ = (0, 0, 1) + t(2, 1, 0)

Its parametric equations are:

x = 2t

y = t

z = 1

Calculate the dot product with the plane's normal vector:

v₂ · n = (2)(0) + (1)(0) + (0)(1)

v₂ · n = 0

Since the dot product is zero, the direction vector is perpendicular to the normal vector.

Therefore, the line is parallel to the plane or lies entirely in it.

### Step 6: Determine Whether the Second Line Lies in the Plane

The starting point is:

P = (0, 0, 1)

Substitute it into the plane equation:

z = 0

1 ≠ 0

Therefore, the starting point does not lie in the plane.

Since the line is parallel to the plane and its starting point is not on the plane, the line has no common points with the plane.

Thus, the second line is parallel to the plane.

## Final Answer

**First line:**

L₁ = (0, 0, 1) + t(2, 1, -1)

- Dot product: v₁ · n = -1
- Relative position: Intersects the plane at one point.
- Intersection point: Q = (2, 1, 0)

**Second line:**

L₂ = (0, 0, 1) + t(2, 1, 0)

- Dot product: v₂ · n = 0
- Starting point does not belong to the plane.
- Relative position: Parallel to the plane with no common points.

The dot product allows us to recognize the relative position of a line and a plane before calculating an intersection.
