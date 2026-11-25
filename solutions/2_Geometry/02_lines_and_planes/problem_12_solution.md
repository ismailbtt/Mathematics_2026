
# Exercise 12 – Intersection Line of Two Planes

## Question

Find a parametric equation of the line that is the intersection of:

x + y + z = 3

x - y + z = 1

Find its direction vector in two ways:

1. From the system of equations.
2. From the cross product of the normal vectors.

Compare the results.

## Solution

### Step 1: Identify the Normal Vectors

The first plane is:

Π₁: x + y + z = 3

Its normal vector is:

n₁ = (1, 1, 1)

The second plane is:

Π₂: x - y + z = 1

Its normal vector is:

n₂ = (1, -1, 1)

The intersection of two non-parallel planes is a line.

### Step 2: Find the Direction Vector Using the Cross Product

The direction vector of the intersection line must be perpendicular to both normal vectors.

Therefore:

v = n₁ × n₂

Substitute:

v = (1, 1, 1) × (1, -1, 1)

Calculate each component:

First component:

1(-1) - 1(1) = -2

Second component:

1(1) - 1(1) = 0

Third component:

1(-1) - 1(1) = -2

Therefore:

v = (-2, 0, -2)

We can simplify by dividing by -2:

v = (1, 0, 1)

This is a valid direction vector.

### Step 3: Find the Direction Vector Using the System of Equations

We have:

x + y + z = 3

x - y + z = 1

Subtract the second equation from the first:

(x + y + z) - (x - y + z) = 3 - 1

2y = 2

Therefore:

y = 1

Substitute y = 1 into the first equation:

x + 1 + z = 3

x + z = 2

Let:

x = t

Then:

z = 2 - t

Therefore, the parametric equations are:

x = t

y = 1

z = 2 - t

### Step 4: Write the Parametric Equation of the Intersection Line

The line can be written as:

(x, y, z) = (0, 1, 2) + t(1, 0, -1)

A direction vector is:

v = (1, 0, -1)

Notice that the cross product gave (1, 0, 1) in Step 2, which does not match the direction obtained from the system.

We must correct the cross product.

Recalculate:

n₁ × n₂:

```text
n₁ × n₂ = (1, 1, 1) × (1, -1, 1)

         = (1×1 - 1×(-1),
            1×1 - 1×1,
            1×(-1) - 1×1)

         = (2, 0, -2)

         = 2(1, 0, -1)
```

Therefore, the correct cross product direction is:

v = (1, 0, -1)

Both methods now give the same direction.

### Step 5: Verify the Parametric Line

The line is:

x = t

y = 1

z = 2 - t

Substitute into the first plane:

t + 1 + 2 - t = 3

3 = 3

Substitute into the second plane:

t - 1 + 2 - t = 1

1 = 1

Both equations are satisfied for every t.

## Final Answer

**Intersection line:**

(x, y, z) = (0, 1, 2) + t(1, 0, -1)

**Direction vector:**

v = (1, 0, -1)

**Two methods:**

- Solving the system gives (1, 0, -1).
- The cross product of the normal vectors gives (2, 0, -2), which is a scalar multiple of (1, 0, -1).

Therefore, both methods produce the same direction.
