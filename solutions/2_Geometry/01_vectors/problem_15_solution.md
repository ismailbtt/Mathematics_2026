
# Exercise 15 – Comparing Directions Using the Cosine of the Angle

## Question

Given:

a = (1, 2, 1)

b = (2, 4, 2)

c = (2, 0, 3)

For each pair, compute:

(u · v) / (||u|| * ||v||)

Order the pairs by increasing angle between the vectors.

Explain why for a and b the value is 1 even though the vectors have different lengths.

---

## Solution

### 1. Calculate the Lengths of the Vectors

For vector a:

||a|| = sqrt(1² + 2² + 1²)

= sqrt(1 + 4 + 1)

**Result:**

||a|| = sqrt(6)

For vector b:

||b|| = sqrt(2² + 4² + 2²)

= sqrt(4 + 16 + 4)

**Result:**

||b|| = sqrt(24) = 2*sqrt(6)

For vector c:

||c|| = sqrt(2² + 0² + 3²)

= sqrt(4 + 0 + 9)

**Result:**

||c|| = sqrt(13)

### 2. Calculate the Cosine for the Pair (a, b)

First, calculate the dot product:

a · b = (1*2) + (2*4) + (1*2)

= 2 + 8 + 2

= 12

Now calculate:

cos(theta_ab) = 12 / (sqrt(6) * 2*sqrt(6))

= 12/12

**Result:**

cos(theta_ab) = 1

Therefore:

theta_ab = 0 degrees

### 3. Calculate the Cosine for the Pair (a, c)

First, calculate the dot product:

a · c = (1*2) + (2*0) + (1*3)

= 2 + 0 + 3

= 5

Now calculate:

cos(theta_ac) = 5 / (sqrt(6) * sqrt(13))

**Result:**

cos(theta_ac) = 5/sqrt(78)

Approximately:

cos(theta_ac) ≈ 0.5661

Therefore:

theta_ac = arccos(5/sqrt(78))

theta_ac ≈ 55.5 degrees

### 4. Calculate the Cosine for the Pair (b, c)

First, calculate the dot product:

b · c = (2*2) + (4*0) + (2*3)

= 4 + 0 + 6

= 10

Now calculate:

cos(theta_bc) = 10 / (sqrt(24) * sqrt(13))

= 10 / sqrt(312)

= 5/sqrt(78)

**Result:**

cos(theta_bc) = 5/sqrt(78)

Approximately:

cos(theta_bc) ≈ 0.5661

Therefore:

theta_bc ≈ 55.5 degrees

### 5. Order the Pairs by Increasing Angle

We obtained:

theta_ab = 0 degrees

theta_ac ≈ 55.5 degrees

theta_bc ≈ 55.5 degrees

Therefore, the order is:

(a, b) < (a, c) = (b, c)

The pair (a, b) has the smallest angle.

The pairs (a, c) and (b, c) have equal angles.

### 6. Explain Why the Cosine for a and b Is 1

We can observe that:

b = 2a

This means that b is a positive scalar multiple of a.

The vectors have the same direction but different lengths.

The cosine formula measures the angle between directions, not the lengths of the vectors.

Therefore:

cos(theta_ab) = 1

This corresponds to an angle of zero degrees.

---

## Final Answers

- ||a|| = sqrt(6)
- ||b|| = 2*sqrt(6)
- ||c|| = sqrt(13)
- cos(theta_ab) = 1
- cos(theta_ac) = 5/sqrt(78) ≈ 0.5661
- cos(theta_bc) = 5/sqrt(78) ≈ 0.5661
- theta_ab = 0 degrees
- theta_ac ≈ 55.5 degrees
- theta_bc ≈ 55.5 degrees

**Increasing angle order:**

(a, b) < (a, c) = (b, c)

