
# Exercise 3 – Vector Normalization

## Question

For v = (3, 4), find a unit vector e with the same direction and orientation.

Check that ||e|| = 1, reconstruct v in the form v = ||v||e, and explain what changes during normalization and what remains unchanged.

---

## Solution

### 1. Calculate the Length of the Vector

The length formula in R² is:

||v|| = sqrt(x² + y²)

Substitute:

||v|| = sqrt(3² + 4²)

= sqrt(9 + 16)

= sqrt(25)

**Result:**

||v|| = 5

### 2. Find the Unit Vector

To normalize a vector, divide each component by its length.

Formula:

e = v / ||v||

Substitute:

e = (3/5, 4/5)

**Result:**

e = (3/5, 4/5)

### 3. Verify That the Unit Vector Has Length 1

Calculate:

||e|| = sqrt((3/5)² + (4/5)²)

= sqrt(9/25 + 16/25)

= sqrt(25/25)

**Result:**

||e|| = 1

The vector is a unit vector.

### 4. Reconstruct the Original Vector

We know:

v = ||v||e

Substitute:

v = 5(3/5, 4/5)

= (3, 4)

**Result:**

v = (3, 4)

The original vector is reconstructed correctly.

### 5. Geometric Interpretation

Normalization changes the length of a vector to 1 while preserving its direction and orientation.

The original vector has length 5, while the normalized vector has length 1.

The direction remains unchanged.

---

## Final Answers

- Original vector: v = (3, 4)
- Length: ||v|| = 5
- Unit vector: e = (3/5, 4/5)
- Verification: ||e|| = 1
- Reconstruction: 5e = (3, 4)
