
# Exercise 8 – Linear Combination and Checking the Result

Given:

w = (5, 1)

u = (1, 1)

v = (2, -1)

We need to check whether w can be written as:

w = au + bv

## 1. Set Up the Equations

Substitute the vectors into the equation:

(5, 1) = a(1, 1) + b(2, -1)

Multiply the scalars:

(5, 1) = (a, a) + (2b, -b)

Add the components:

(5, 1) = (a + 2b, a - b)

This gives us a system of two equations:

a + 2b = 5

a - b = 1

## 2. Solve the System of Equations

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

## 3. Reconstruct the Vector

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

## 4. Geometric Interpretation

A linear combination means multiplying vectors by scalars and adding the resulting vectors.

Here, the coefficients a and b determine how much of each vector is used.

Since we found coefficients that produce w, the vector w can be expressed as a linear combination of u and v.

Geometrically, the vectors u and v span the entire plane because they are not parallel.

Therefore, every vector in R² can be expressed as a linear combination of these two vectors.

## Final Answers

- a = 7/3
- b = 4/3
- w = (7/3)u + (4/3)v
- Reconstructed vector: w = (5, 1)
- The vector w can be expressed as a linear combination of u and v.


