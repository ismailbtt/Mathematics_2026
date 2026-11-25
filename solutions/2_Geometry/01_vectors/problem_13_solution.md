
# Exercise 13 – Do Four Points Lie in One Plane?

## Question

Given:

A = (0, 0, 0)

B = (1, 2, 0)

C = (0, 1, 1)

D = (2, 5, 1)

1. Construct AB and AC.
2. Find n = AB × AC.
3. Construct AD and check whether AD · n = 0.
4. Decide whether D lies in the plane determined by A, B, and C, and justify the criterion.

---

## Solution

### 1. Construct the Vectors AB and AC

First, calculate AB:

AB = B - A

AB = (1 - 0, 2 - 0, 0 - 0)

**Result:**

AB = (1, 2, 0)

Now calculate AC:

AC = C - A

AC = (0 - 0, 1 - 0, 1 - 0)

**Result:**

AC = (0, 1, 1)

### 2. Find the Normal Vector n

The cross product gives a vector perpendicular to both AB and AC.

Formula:

n = AB × AC

Substitute:

n = (1, 2, 0) × (0, 1, 1)

Calculate:

n = (
    2*1 - 0*1,
    0*0 - 1*1,
    1*1 - 2*0
)

n = (2, -1, 1)

**Result:**

n = (2, -1, 1)

### 3. Construct the Vector AD

Calculate:

AD = D - A

AD = (2 - 0, 5 - 0, 1 - 0)

**Result:**

AD = (2, 5, 1)

### 4. Check Whether AD · n = 0

Calculate the dot product:

AD · n = (2, 5, 1) · (2, -1, 1)

= (2*2) + (5*(-1)) + (1*1)

= 4 - 5 + 1

**Result:**

AD · n = 0

### 5. Determine Whether D Lies in the Plane

A point lies in the plane determined by A, B, and C if its displacement vector from A is perpendicular to the plane's normal vector.

The condition is:

AD · n = 0

We calculated:

AD · n = 0

Therefore, D lies in the same plane as A, B, and C.

**Result:**

The four points are coplanar.

### 6. Geometric Interpretation

The cross product AB × AC produces a normal vector to the plane determined by A, B, and C.

If the vector AD has a dot product of zero with this normal vector, AD lies in the plane.

Since the dot product is zero, point D belongs to the same plane.

---

## Final Answers

- AB = (1, 2, 0)
- AC = (0, 1, 1)
- n = (2, -1, 1)
- AD = (2, 5, 1)
- AD · n = 0
- The four points are coplanar.
