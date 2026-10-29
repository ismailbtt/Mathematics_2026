
## Exercise 15: Combining Determinant Properties

### Given Information

Let A and B be invertible 2×2 matrices such that:

$$
\det(A)=-2
$$

$$
\det(B)=3
$$

We need to calculate:

$$
\det(B^{-1}A^TB)
$$

without knowing the individual entries of the matrices.

We will use determinant properties to simplify the expression.

### Step 1: Recall the Determinant Properties

We will use the following properties:

**Property 1: Determinant of a Product**

For square matrices A and B:

$$
\det(AB)=\det(A)\det(B)
$$

**Property 2: Determinant of an Inverse**

For an invertible matrix B:

$$
\det(B^{-1})=\frac{1}{\det(B)}
$$

**Property 3: Determinant of a Transpose**

For any square matrix A:

$$
\det(A^T)=\det(A)
$$

These properties allow us to calculate the determinant without multiplying the matrices directly.

### Step 2: Apply the Product Property

Start with:

$$
\det(B^{-1}A^TB)
$$

Using the determinant product property:

$$
\det(B^{-1}A^TB)
=
\det(B^{-1})\det(A^T)\det(B)
$$

We can now calculate each factor separately.

### Step 3: Calculate the Determinant of B⁻¹

Since:

$$
\det(B)=3
$$

and B is invertible:

$$
\det(B^{-1})=\frac{1}{\det(B)}
$$

Substitute:

$$
\det(B^{-1})=\frac{1}{3}
$$

Therefore:

$$
\boxed{\det(B^{-1})=\frac{1}{3}}
$$

### Step 4: Calculate the Determinant of Aᵀ

The determinant of a matrix is equal to the determinant of its transpose.

Therefore:

$$
\det(A^T)=\det(A)
$$

Since:

$$
\det(A)=-2
$$

We obtain:

$$
\boxed{\det(A^T)=-2}
$$

### Step 5: Substitute the Determinant Values

Recall:

$$
\det(B^{-1}A^TB)
=
\det(B^{-1})\det(A^T)\det(B)
$$

Substitute the known values:

$$
=\frac{1}{3}\cdot(-2)\cdot3
$$

Simplifying:

$$
=\frac{-6}{3}
$$

Therefore:

$$
\boxed{\det(B^{-1}A^TB)=-2}
$$

### Step 6: Explain Why the B Factors Cancel

We know:

$$
\det(B^{-1})=\frac{1}{\det(B)}
$$

Therefore:

$$
\det(B^{-1})\det(B)
=
\frac{1}{\det(B)}\det(B)
$$

Since B is invertible, its determinant is nonzero.

Thus:

$$
\det(B^{-1})\det(B)=1
$$

Consequently:

$$
\det(B^{-1}A^TB)
=
1\cdot\det(A^T)
$$

And because:

$$
\det(A^T)=\det(A)
$$

We obtain:

$$
\boxed{\det(B^{-1}A^TB)=\det(A)}
$$

Therefore:

$$
\boxed{\det(B^{-1}A^TB)=-2}
$$

### Step 7: Mathematical Verification

We can also verify the result using the identity matrix.

By associativity of matrix multiplication:

$$
B^{-1}A^TB
$$

Taking determinants:

$$
\det(B^{-1}A^TB)
=
\det(A^T)\det(BB^{-1})
$$

Since:

$$
BB^{-1}=I
$$

and:

$$
\det(I)=1
$$

We obtain:

$$
\det(B^{-1}A^TB)
=
\det(A^T)\cdot1
$$

Therefore:

$$
\det(B^{-1}A^TB)=\det(A^T)
$$

Using the transpose property:

$$
\det(A^T)=\det(A)=-2
$$

Thus:

$$
\boxed{\det(B^{-1}A^TB)=-2}
$$

The result is verified.

### Step 8: Explanation

This exercise combines three important determinant properties.

First, the determinant of a product equals the product of the determinants.

Second, the determinant of an inverse is the reciprocal of the original determinant.

Third, transposing a matrix does not change its determinant.

The factors involving B cancel because:

$$
\det(B^{-1})\det(B)=1
$$

Therefore, the determinant of the entire expression depends only on the determinant of A.

This is also an example of determinant invariance under a similarity transformation.

### Final Answer

Given:

$$
\det(A)=-2,\quad\det(B)=3
$$

We calculate:

$$
\det(B^{-1}A^TB)
=
\frac{1}{3}\cdot(-2)\cdot3
$$

Therefore:

$$
\boxed{\det(B^{-1}A^TB)=-2}
$$

**Conclusion:** Using the product, inverse, and transpose properties of determinants, we find that the determinant is -2. The factors involving B cancel because their determinants multiply to 1. No matrix entries or direct matrix multiplication are needed.
