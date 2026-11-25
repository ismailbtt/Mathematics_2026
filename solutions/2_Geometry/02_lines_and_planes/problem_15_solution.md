
# Exercise 15 – Complete Classification of a Line Relative to a Plane

## Question

Let:

L: p + tv

Π: n · x = d

State the conditions distinguishing the three cases:

1. One intersection point.
2. Parallel with no common points.
3. The line contained in the plane.

Then illustrate each case with your own simple numerical example.

## Solution

### Step 1: Understand the Given Equations

The general parametric equation of a line is:

L: x = p + tv

Where:

- p is a point on the line.
- v is the direction vector of the line.
- t is a real parameter.

The general equation of a plane is:

Π: n · x = d

Where:

- n is the normal vector of the plane.
- x represents a point on the plane.
- d is a constant.

The normal vector determines the orientation of the plane.

To classify the relative position of the line and the plane, we calculate the dot product:

n · v

This dot product tells us whether the line's direction is perpendicular to the normal vector.

### Step 2: Substitute the Line into the Plane Equation

We know that:

x = p + tv

Substitute this expression into the plane equation:

n · (p + tv) = d

Using the distributive property of the dot product:

n · p + t(n · v) = d

Rearrange:

t(n · v) = d - n · p

This equation is the key to classifying the three possible cases.

### Step 3: Case 1 – One Intersection Point

If:

n · v ≠ 0

Then we can solve for t:

t = (d - n · p) / (n · v)

There is exactly one value of t.

Therefore, the line intersects the plane at exactly one point.

The intersection point is found by substituting this value of t into:

x = p + tv

**Example:**

Consider the plane:

Π: z = 0

Its normal vector is:

n = (0, 0, 1)

Consider the line:

L: (x, y, z) = (1, 2, 3) + t(0, 0, 1)

Its starting point is:

p = (1, 2, 3)

Its direction vector is:

v = (0, 0, 1)

Calculate the dot product:

n · v = (0)(0) + (0)(0) + (1)(1)

n · v = 1

Since the dot product is not zero, the line intersects the plane at one point.

The parametric equations are:

x = 1

y = 2

z = 3 + t

Substitute into the plane equation:

z = 0

3 + t = 0

t = -3

Substitute t = -3 into the line:

x = 1

y = 2

z = 3 - 3 = 0

Therefore, the intersection point is:

Q = (1, 2, 0)

### Step 4: Case 2 – Parallel with No Common Points

If:

n · v = 0

Then the direction vector is perpendicular to the normal vector.

This means the line is parallel to the plane or lies entirely inside it.

To distinguish these possibilities, check the starting point p.

If:

n · p ≠ d

Then the starting point does not lie in the plane.

Since the line is parallel to the plane and starts outside it, there are no common points.

**Example:**

Consider the plane:

Π: z = 0

Its normal vector is:

n = (0, 0, 1)

Consider the line:

L: (x, y, z) = (1, 2, 3) + t(1, 0, 0)

Its direction vector is:

v = (1, 0, 0)

Calculate the dot product:

n · v = (0)(1) + (0)(0) + (1)(0)

n · v = 0

Therefore, the line is parallel to the plane or contained in it.

Now check the starting point:

p = (1, 2, 3)

Substitute into the plane equation:

z = 0

3 ≠ 0

Therefore, the starting point is not on the plane.

The line has no common points with the plane.

Its z-coordinate always remains equal to 3, while every point on the plane has z = 0.

Thus, the line is parallel to the plane and does not intersect it.

### Step 5: Case 3 – The Line Is Contained in the Plane

If:

n · v = 0

and:

n · p = d

Then the direction vector is parallel to the plane and the starting point lies in the plane.

Since every point on the line is obtained by moving in a direction parallel to the plane, the entire line lies in the plane.

**Example:**

Consider the plane:

Π: z = 0

Its normal vector is:

n = (0, 0, 1)

Consider the line:

L: (x, y, z) = (1, 2, 0) + t(1, 0, 0)

Its starting point is:

p = (1, 2, 0)

Its direction vector is:

v = (1, 0, 0)

First, calculate the dot product:

n · v = (0)(1) + (0)(0) + (1)(0)

n · v = 0

Next, check the starting point:

n · p = (0)(1) + (0)(2) + (1)(0)

n · p = 0

Since the plane has d = 0:

n · p = d

Both conditions are satisfied.

We can also verify the line directly.

Its parametric equations are:

x = 1 + t

y = 2

z = 0

Every point on the line has z = 0.

Therefore, every point satisfies the plane equation.

The entire line is contained in the plane.

### Step 6: Summarize the Three Conditions

The relative position of a line and a plane can be determined using two conditions:

1. Calculate n · v.
2. If n · v = 0, check whether n · p = d.

The complete classification is:

**Case 1: One intersection point**

n · v ≠ 0

There is exactly one intersection point.

**Case 2: Parallel with no common points**

n · v = 0

n · p ≠ d

The line is parallel to the plane but does not lie in it.

**Case 3: The line is contained in the plane**

n · v = 0

n · p = d

Every point on the line belongs to the plane.

## Final Answer

For the line:

L: x = p + tv

and the plane:

Π: n · x = d

the three possible cases are:

**1. One intersection point:**

n · v ≠ 0

**2. Parallel with no common points:**

n · v = 0

n · p ≠ d

**3. The line is contained in the plane:**

n · v = 0

n · p = d

These conditions provide a complete classification of the relative position of a line and a plane.

The dot product n · v determines whether the line crosses the plane or is parallel to it. The condition n · p = d determines whether a parallel line is contained in the plane.
