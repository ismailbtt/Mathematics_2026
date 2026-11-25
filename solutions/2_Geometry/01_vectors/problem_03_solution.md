
# Exercise 3 – Vector Normalization

Given:

v = (3, 4)

We need to find a unit vector e with the same direction and orientation as v.

## 1. Calculate the Length of the Vector

The length of a vector in R² is calculated using:

||v|| = √(x² + y²)

Substitute the coordinates:

||v|| = √(3² + 4²)

||v|| = √(9 + 16)

||v|| = √25

**Result:**

||v|| = 5

## 2. Find the Unit Vector

To normalize a vector, divide each component by its length.

Formula:

e = v / ||v||

Substitute the values:

e = (3/5, 4/5)

**Result:**

e = (3/5, 4/5)

## 3. Verify That the Unit Vector Has Length 1

Calculate the length of e:

||e|| = √((3/5)² + (4/5)²)

||e|| = √(9/25 + 16/25)

||e|| = √(25/25)

**Result:**

||e|| = 1

The vector is a unit vector.

## 4. Reconstruct the Original Vector

We know that:

v = ||v|| * e

Substitute the values:

v = 5 * (3/5, 4/5)

v = (3, 4)

**Result:**

v = (3, 4)

The original vector is reconstructed correctly.

## 5. Geometric Interpretation

Normalization changes the length of a vector to 1 while preserving its direction and orientation.

The vector becomes shorter or longer, but it still points in the same direction.

The original vector has length 5, while the normalized vector has length 1.

## Final Answers

- Original vector: v = (3, 4)
- Length: ||v|| = 5
- Unit vector: e = (3/5, 4/5)
- Verification: ||e|| = 1
- Reconstruction: 5 * e = (3, 4)
