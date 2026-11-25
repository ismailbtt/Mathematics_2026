
# Exercise 11 – Plane Containing a Line and a Point

## Question

Find the equation of the plane containing:

(x, y, z) = (1, 0, 2) + t(1, 1, -1)

and the point:

P = (0, 2, 1)

Check that both the entire line and the point lie in the plane you obtain.

## Solution

### Step 1: Identify the Given Information

The line is:

L: (x, y, z) = (1, 0, 2) + t(1, 1, -1)

From this equation, we identify a point on the line:

A = (1, 0, 2)

The direction vector of the line is:

v = (1, 1, -1)

We are also given another point:

P = (0, 2, 1)

We need to construct a plane containing the entire line and point P.

### Step 2: Construct a Second Direction Vector

A plane requires two linearly independent direction vectors.

The first direction vector is already given:

v = (1, 1, -1)

We construct another vector using points A and P:

AP = P - A

AP = (0 - 1, 2 - 0, 1 - 2)

Therefore:

AP = (-1, 2, -1)

This vector also lies in the required plane because it connects two points that must belong to the plane.

### Step 3: Calculate the Normal Vector

The normal vector is perpendicular to both direction vectors.

We calculate it using the cross product:

n = v × AP

Substitute:

n = (1, 1, -1) × (-1, 2, -1)

Using the cross product formula:

n = (1(-1) - (-1)(2),
     (-1)(-1) - 1(-1),
     1(2) - 1(-1))

Simplify:

n = (-1 + 2, 1 + 1, 2 + 1)

Therefore:

n = (1, 2, 3)

### Step 4: Construct the Plane Equation

The general equation of a plane is:

a(x - x₀) + b(y - y₀) + c(z - z₀) = 0

We use:

Normal vector = (1, 2, 3)

Point A = (1, 0, 2)

Substitute:

1(x - 1) + 2(y - 0) + 3(z - 2) = 0

Expand:

x - 1 + 2y + 3z - 6 = 0

Simplify:

x + 2y + 3z - 7 = 0

Therefore, the plane equation is:

x + 2y + 3z = 7

### Step 5: Verify the Given Point

Substitute P = (0, 2, 1):

0 + 2(2) + 3(1) = 7

0 + 4 + 3 = 7

7 = 7

Therefore, point P lies in the plane.

### Step 6: Verify the Entire Line

The line is:

x = 1 + t
y = t
z = 2 - t

Substitute these expressions into the plane equation:

x + 2y + 3z = 7

(1 + t) + 2t + 3(2 - t) = 7

Expand:

1 + t + 2t + 6 - 3t = 7

Simplify:

7 + 0t = 7

This identity is true for every value of t.

Therefore, the entire line lies in the plane.

## Final Answer

**Plane equation:**

x + 2y + 3z - 7 = 0

**Normal vector:**

n = (1, 2, 3)

**Verification:**

- Point P = (0, 2, 1) satisfies the plane equation.
- Every point on the given line satisfies the plane equation.

Therefore, the plane contains both the entire line and the given point.
