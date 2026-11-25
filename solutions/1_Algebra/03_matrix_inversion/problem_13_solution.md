
# Exercise 13 – Checking Whether Four Points Are Coplanar

## Question

Given four points:

A = (0, 0, 0)
B = (1, 2, 0)
C = (0, 1, 1)
D = (2, 5, 1)

Determine whether the four points are coplanar.

Follow these steps:
1. Calculate vectors AB and AC.
2. Calculate the normal vector n = AB × AC.
3. Calculate vector AD.
4. Check whether AD · n = 0.
5. Determine whether point D lies in the plane ABC.

## Solution

### Step 1: Calculate vectors AB and AC

AB = B - A

AB = (1 - 0, 2 - 0, 0 - 0)

AB = (1, 2, 0)

AC = C - A

AC = (0 - 0, 1 - 0, 1 - 0)

AC = (0, 1, 1)

### Step 2: Calculate the normal vector

The normal vector is:

n = AB × AC

n = (1, 2, 0) × (0, 1, 1)

Using the cross product:

n = (2 × 1 - 0 × 1,
     0 × 0 - 1 × 1,
     1 × 1 - 2 × 0)

n = (2, -1, 1)

### Step 3: Calculate vector AD

AD = D - A

AD = (2 - 0, 5 - 0, 1 - 0)

AD = (2, 5, 1)

### Step 4: Calculate the dot product

AD · n = (2, 5, 1) · (2, -1, 1)

AD · n = (2 × 2) + (5 × -1) + (1 × 1)

AD · n = 4 - 5 + 1

AD · n = 0

### Step 5: Determine whether the points are coplanar

Since:

AD · n = 0

Point D lies in the plane ABC.

Therefore, all four points are coplanar.

## Final Answer

The four points A, B, C, and D are coplanar because the dot product of AD and the normal vector n is equal to zero.

