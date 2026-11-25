
# Exercise 8 – Linear Combination and Checking the Result

## Question

Check whether w = (5, 1) can be written as:

w = au + bv

where:

u = (1, 1)

v = (2, -1)

If so, find a and b, reconstruct w from them, and explain the geometric meaning of the existence of such coefficients.

---

## Solution

### 1. Set Up the Equations

Substitute the vectors into the equation:

(5, 1) = a(1, 1) + b(2, -1)

Multiply the scalars:

(5, 1) = (a, a) + (2b, -b)

Add the components:

(5, 1) = (a + 2b, a - b)

This gives a system of two equations:

a + 2b = 5

a - b = 1

### 2. Solve the System of Equations

From the second equation:

a - b = 1

a = 1 + b

Substitute into the first equation:

(1 + b) + 2b = 5

1 + 3b = 5

3b = 4

**Result:**

b = 4/3

Now calculate a:

a = 1 + b

a = 1 + 4/3

**Result:**

a = 7/3

### 3. Reconstruct the Vector

We found:

a = 7/3

b = 4/3

Substitute these values:

w = (7/3)u + (4/3)v

w = (7/3)(1, 1) + (4/3)(2, -1)

Multiply:

w = (7/3, 7/3) + (8/3, -4/3)

Add the components:

w = (15/3, 3/3)

**Result:**

w = (5, 1)

The original vector is reconstructed correctly.

### 4. Geometric Interpretation

A linear combination means multiplying vectors by scalars and adding the resulting vectors.

The coefficients a and b determine how much of each vector is used.

Since we found coefficients that produce w, the vector w can be expressed as a linear combination of u and v.

The vectors u and v are not parallel because they are not scalar multiples of each other.

Therefore, they span the entire plane R².

Every vector in R² can be expressed as a linear combination of these two vectors.

---

## Final Answers

- a = 7/3
- b = 4/3
- w = (7/3)u + (4/3)v
- Reconstructed vector: w = (5, 1)
- The vector w can be expressed as a linear combination of u and v.
