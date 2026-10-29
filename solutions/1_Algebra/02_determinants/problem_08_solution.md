
## Exercise 8: Determinant of a Product

### Given Information

Let A and B be square matrices such that:

$$
\det(A)=3
$$

$$
\det(B)=-5
$$

We need to calculate:

$$
\det(AB),\quad \det(BA),\quad \det(A^{-1}B)
$$

We will use determinant properties to find the results.

### Step 1: Calculate det(AB)

The determinant of a product of two square matrices is equal to the product of their determinants.

The property is:

$$
\det(AB)=\det(A)\det(B)
$$

Substitute the given values:

$$
\det(AB)=3(-5)
$$

Therefore:

$$
\boxed{\det(AB)=-15}
$$

### Step 2: Calculate det(BA)

Using the same determinant property:

$$
\det(BA)=\det(B)\det(A)
$$

Substitute the values:

$$
\det(BA)=(-5)(3)
$$

Therefore:

$$
\boxed{\det(BA)=-15}
$$

### Step 3: Calculate det(A⁻¹B)

First, we need to determine whether the inverse of A exists.

A square matrix is invertible if its determinant is nonzero.

Since:

$$
\det(A)=3\neq0
$$

Matrix A is invertible, so A⁻¹ exists.

The determinant of an inverse matrix is:

$$
\det(A^{-1})=\frac{1}{\det(A)}
$$

Therefore:

$$
\det(A^{-1})=\frac{1}{3}
$$

Now use the determinant product property:

$$
\det(A^{-1}B)=\det(A^{-1})\det(B)
$$

Substitute:

$$
\det(A^{-1}B)=\frac{1}{3}(-5)
$$

Therefore:

$$
\boxed{\det(A^{-1}B)=-\frac{5}{3}}
$$

### Step 4: Explain Why det(AB) = det(BA)

Matrix multiplication is generally not commutative.

This means:

$$
AB\neq BA
$$

However, determinants satisfy the multiplication property:

$$
\det(AB)=\det(A)\det(B)
$$

And:

$$
\det(BA)=\det(B)\det(A)
$$

Since multiplication of real numbers is commutative:

$$
\det(A)\det(B)=\det(B)\det(A)
$$

Therefore:

$$
\boxed{\det(AB)=\det(BA)}
$$

Even though the matrices AB and BA may be different, their determinants are equal.

### Step 5: Verification

We can verify the results using the given determinant values.

For AB:

$$
\det(AB)=3(-5)=-15
$$

For BA:

$$
\det(BA)=(-5)(3)=-15
$$

Thus:

$$
\det(AB)=\det(BA)=-15
$$

For the inverse product:

$$
\det(A^{-1}B)=\frac{-5}{3}
$$

We can verify this using:

$$
A(A^{-1}B)=B
$$

Taking determinants:

$$
\det(A)\det(A^{-1}B)=\det(B)
$$

Substituting:

$$
3\left(-\frac{5}{3}\right)=-5
$$

The equality holds, confirming our result.

### Step 6: Determinant Properties Used

**Property 1: Determinant of a Product**

$$
\det(AB)=\det(A)\det(B)
$$

**Property 2: Determinant of an Inverse**

$$
\det(A^{-1})=\frac{1}{\det(A)}
$$

This property applies when A is invertible.

**Property 3: Invertibility Condition**

$$
\det(A)\neq0
$$

A nonzero determinant guarantees that the inverse matrix exists.

### Final Answer

| Expression | Result |
|------------|--------|
| det(AB) | -15 |
| det(BA) | -15 |
| det(A⁻¹B) | -5/3 |

Therefore:

$$
\boxed{\det(AB)=-15}
$$

$$
\boxed{\det(BA)=-15}
$$

$$
\boxed{\det(A^{-1}B)=-\frac{5}{3}}
$$

**Conclusion:** The determinant of a matrix product equals the product of the individual determinants. Therefore, det(AB) and det(BA) are equal even though matrix multiplication is generally not commutative. Since det(A) is nonzero, A is invertible, and det(A⁻¹B) exists and equals -5/3.
