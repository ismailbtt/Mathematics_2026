
# Exercise 3. When Can Matrices Be Multiplied?

## Question

The matrix sizes are:

$$
A_{2\times3},\qquad
B_{3\times4},\qquad
C_{4\times2},\qquad
D_{2\times2}
$$

For the products

$$
AB,\ BA,\ BC,\ CB,\ AC,\ CA,\ AD,\ DA
$$

determine whether they are defined.

If so, state the size of the result.

Justify each decision using the dimension compatibility condition.

---

## Multiplication Rule

Two matrices can be multiplied only when the number of columns of the first matrix equals the number of rows of the second matrix.

The general rule is:

$$
(m\times n)(n\times p)=m\times p
$$

The inner dimensions must be equal.

The outer dimensions determine the size of the resulting matrix.

---

## Solution 1. Product AB

Matrix A has size 2×3.

Matrix B has size 3×4.

$$
AB=(2\times3)(3\times4)
$$

The inner dimensions are both 3.

$$
3=3
$$

Therefore, multiplication is possible.

**Final Answer:**

$$
\boxed{AB:2\times4}
$$

---

## Solution 2. Product BA

Matrix B has size 3×4.

Matrix A has size 2×3.

$$
BA=(3\times4)(2\times3)
$$

The inner dimensions are 4 and 2.

$$
4\neq2
$$

Therefore, multiplication is not possible.

**Final Answer:**

$$
\boxed{BA:\text{Undefined}}
$$

---

## Solution 3. Product BC

Matrix B has size 3×4.

Matrix C has size 4×2.

$$
BC=(3\times4)(4\times2)
$$

The inner dimensions are both 4.

$$
4=4
$$

Therefore, multiplication is possible.

**Final Answer:**

$$
\boxed{BC:3\times2}
$$

---

## Solution 4. Product CB

Matrix C has size 4×2.

Matrix B has size 3×4.

$$
CB=(4\times2)(3\times4)
$$

The inner dimensions are 2 and 3.

$$
2\neq3
$$

Therefore, multiplication is not possible.

**Final Answer:**

$$
\boxed{CB:\text{Undefined}}
$$

---

## Solution 5. Product AC

Matrix A has size 2×3.

Matrix C has size 4×2.

$$
AC=(2\times3)(4\times2)
$$

The inner dimensions are 3 and 4.

$$
3\neq4
$$

Therefore, multiplication is not possible.

**Final Answer:**

$$
\boxed{AC:\text{Undefined}}
$$

---

## Solution 6. Product CA

Matrix C has size 4×2.

Matrix A has size 2×3.

$$
CA=(4\times2)(2\times3)
$$

The inner dimensions are both 2.

$$
2=2
$$

Therefore, multiplication is possible.

**Final Answer:**

$$
\boxed{CA:4\times3}
$$

---

## Solution 7. Product AD

Matrix A has size 2×3.

Matrix D has size 2×2.

$$
AD=(2\times3)(2\times2)
$$

The inner dimensions are 3 and 2.

$$
3\neq2
$$

Therefore, multiplication is not possible.

**Final Answer:**

$$
\boxed{AD:\text{Undefined}}
$$

---

## Solution 8. Product DA

Matrix D has size 2×2.

Matrix A has size 2×3.

$$
DA=(2\times2)(2\times3)
$$

The inner dimensions are both 2.

$$
2=2
$$

Therefore, multiplication is possible.

**Final Answer:**

$$
\boxed{DA:2\times3}
$$

---

## Final Answers

| Product | Defined? | Result Size |
|---|---|---|
| AB | Yes | 2×4 |
| BA | No | Undefined |
| BC | Yes | 3×2 |
| CB | No | Undefined |
| AC | No | Undefined |
| CA | Yes | 4×3 |
| AD | No | Undefined |
| DA | Yes | 2×3 |

---

## Mathematical Verification

We can check the four defined products using the general matrix multiplication rule.

$$
AB=(2\times3)(3\times4)
\Rightarrow 2\times4
$$

$$
BC=(3\times4)(4\times2)
\Rightarrow 3\times2
$$

$$
CA=(4\times2)(2\times3)
\Rightarrow 4\times3
$$

$$
DA=(2\times2)(2\times3)
\Rightarrow 2\times3
$$

In all four cases, the inner dimensions match.

Therefore, these products are correctly defined.

---

## Explanation

Matrix multiplication depends on the order of the matrices.

For example:

$$
AB:\text{Defined}
$$

But:

$$
BA:\text{Undefined}
$$

This happens because the inner dimensions are different when the order is reversed.

**Conclusion:** Before multiplying matrices, always check that the number of columns of the first matrix equals the number of rows of the second matrix.
