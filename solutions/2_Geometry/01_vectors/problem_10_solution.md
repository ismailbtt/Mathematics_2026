
# Exercise 10 – Triangle Area from Vectors

Given three points:

A = (0, 0, 0)

B = (2, 1, 0)

C = (1, 3, 2)

We need to calculate the area of the parallelogram using the cross product and then find the area of the triangle.

## 1. Construct the Vector AB

To find the vector from A to B, subtract the coordinates of A from B.

Formula:

AB = B - A

AB = (2 - 0, 1 - 0, 0 - 0)

**Result:**

AB = (2, 1, 0)

## 2. Construct the Vector AC

Formula:

AC = C - A

AC = (1 - 0, 3 - 0, 2 - 0)

**Result:**

AC = (1, 3, 2)

## 3. Calculate the Cross Product AB × AC

The cross product formula is:

AB × AC = (y1*z2 - z1*y2, z1*x2 - x1*z2, x1*y2 - y1*x2)

Substitute the coordinates:

AB × AC = (1*2 - 0*3, 0*1 - 2*2, 2*3 - 1*1)

Calculate:

AB × AC = (2, -4, 5)

**Result:**

AB × AC = (2, -4, 5)

## 4. Calculate the Area of the Parallelogram

The area of a parallelogram formed by two vectors is equal to the length of their cross product.

Formula:

Area = ||AB × AC||

Calculate the length:

Area = √(2² + (-4)² + 5²)

Area = √(4 + 16 + 25)

**Result:**

Area = √45 = 3√5

Approximately:

Area ≈ 6.71

## 5. Calculate the Area of the Triangle

A triangle formed by the same two vectors has half the area of the parallelogram.

Formula:

Triangle Area = (1/2) * ||AB × AC||

Substitute:

Triangle Area = (1/2) * 3√5

**Result:**

Triangle Area = 3√5 / 2

Approximately:

Triangle Area ≈ 3.35

## 6. Geometric Interpretation

Two vectors starting from the same point form a parallelogram.

The magnitude of their cross product gives the area of this parallelogram.

A diagonal divides a parallelogram into two equal triangles.

Therefore, the area of the triangle is half the area of the parallelogram.

## Final Answers

- AB = (2, 1, 0)
- AC = (1, 3, 2)
- AB × AC = (2, -4, 5)
- Parallelogram area = 3√5 ≈ 6.71
- Triangle area = 3√5 / 2 ≈ 3.35

