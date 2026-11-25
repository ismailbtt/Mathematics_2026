
# Exercise 4 – Plane Through Three Points

## Question

Find the equation of the plane through:

A = (1, 0, 0)
B = (0, 1, 0)
C = (0, 0, 1)

First construct two vectors lying in the plane, and then use the cross product.

Check the resulting equation on all three points.

## Solution

### Step 1: Construct Two Vectors in the Plane

We calculate:

AB = B - A

AB = (0 - 1, 1 - 0, 0 - 0)

AB = (-1, 1, 0)

Next:

AC = C - A

AC = (0 - 1, 0 - 0, 1 - 0)

AC = (-1, 0, 1)

Therefore:

AB = (-1, 1, 0)

AC = (-1, 0, 1)

### Step 2: Calculate the Normal Vector Using the Cross Product

The normal vector is:

n = AB × AC

```text
n = (-1, 1, 0) × (-1, 0, 1)

n = (1, 1, 1)
```

Therefore:

n = (1, 1, 1)

### Step 3: Find the Plane Equation

The general equation of a plane is:

a(x - x₀) + b(y - y₀) + c(z - z₀) = 0

Using point A = (1, 0, 0) and normal vector n = (1, 1, 1):

(x - 1) + y + z = 0

Simplifying:

x + y + z - 1 = 0

Therefore:

x + y + z = 1

### Step 4: Verify All Three Points

For A = (1, 0, 0):

1 + 0 + 0 = 1

For B = (0, 1, 0):

0 + 1 + 0 = 1

For C = (0, 0, 1):

0 + 0 + 1 = 1

All three points satisfy the plane equation.

## Final Answer

**Plane equation:**

x + y + z = 1

**Normal vector:**

n = (1, 1, 1)

**Vectors in the plane:**

AB = (-1, 1, 0)

AC = (-1, 0, 1)

All three given points lie on the plane.
