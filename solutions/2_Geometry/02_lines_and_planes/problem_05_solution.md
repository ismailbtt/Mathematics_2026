
# Exercise 5 – Relative Position of Two Lines

## Question

Analyze the position of:

L₁: (x, y, z) = (1, 1, 0) + t(1, 2, 1)

L₂: (x, y, z) = (2, 0, 1) + s(0, 1, -1)

If they intersect, give the intersection point.

If not, determine whether they are parallel or skew.

Justify the classification.

## Solution

### Step 1: Identify the Direction Vectors

For the first line:

v₁ = (1, 2, 1)

For the second line:

v₂ = (0, 1, -1)

### Step 2: Check Whether the Lines Are Parallel

Two lines are parallel if their direction vectors are scalar multiples of each other.

Here:

v₁ = (1, 2, 1)

v₂ = (0, 1, -1)

The vectors are not scalar multiples because their first coordinates are different (1 and 0).

Therefore, the lines are not parallel.

### Step 3: Check Whether the Lines Intersect

Write the parametric equations.

For L₁:

x = 1 + t
y = 1 + 2t
z = t

For L₂:

x = 2
y = s
z = 1 - s

To find an intersection, equate the corresponding coordinates.

From the x-coordinates:

1 + t = 2

t = 1

From the z-coordinates:

t = 1 - s

Substitute t = 1:

1 = 1 - s

s = 0

Now check the y-coordinates:

1 + 2(1) = 0

3 = 0

This is impossible.

Therefore, the lines do not intersect.

### Step 4: Classify the Relative Position

We have established that:

- The direction vectors are not scalar multiples, so the lines are not parallel.
- The coordinate equations have no common solution, so the lines do not intersect.

Two lines in three-dimensional space that neither intersect nor are parallel are called skew lines.

## Final Answer

The two lines are skew.

**Reason:**

1. They are not parallel because their direction vectors are not scalar multiples.
2. They do not intersect because the coordinate equations lead to the contradiction 3 = 0.

Therefore, the lines are skew and have no intersection point.
