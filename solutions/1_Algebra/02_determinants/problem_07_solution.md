
## Exercise 7: Using Properties Instead of Recomputing

### Given Information

Let A be a 3×3 matrix such that:

$$
\det(A)=-4
$$

We need to calculate:

$$
\det(2A),\quad \det(A^T),\quad \det(A^2),\quad \det(-A)
$$

We will use determinant properties instead of calculating the determinants directly.

### Step 1: Calculate det(2A)

For an n×n matrix, multiplying every entry by a scalar k changes the determinant according to:

$$
\det(kA)=k^n\det(A)
$$

Since A is a 3×3 matrix:

$$
\det(2A)=2^3\det(A)
$$

Substitute the given determinant:

$$
\det(2A)=8(-4)
$$

Therefore:

$$
\boxed{\det(2A)=-32}
$$

### Step 2: Calculate det(Aᵀ)

An important determinant property is:

$$
\det(A^T)=\det(A)
$$

The determinant of a matrix is equal to the determinant of its transpose.

Since:

$$
\det(A)=-4
$$

Therefore:

$$
\boxed{\det(A^T)=-4}
$$

### Step 3: Calculate det(A²)

The determinant of a product of two square matrices satisfies:

$$
\det(AB)=\det(A)\det(B)
$$

Since:

$$
A^2=AA
$$

We obtain:

$$
\det(A^2)=\det(A)\det(A)
$$

Substituting:

$$
\det(A^2)=(-4)(-4)
$$

Therefore:

$$
\boxed{\det(A^2)=16}
$$

### Step 4: Calculate det(-A)

The scalar multiplication property states:

$$
\det(kA)=k^n\det(A)
$$

Here, k = -1 and n = 3.

Therefore:

$$
\det(-A)=(-1)^3\det(A)
$$

Substituting:

$$
\det(-A)=(-1)(-4)
$$

Thus:

$$
\boxed{\det(-A)=4}
$$

### Step 5: Verification and Explanation

We used the following determinant properties:

**Property 1: Scalar Multiplication**

$$
\det(kA)=k^n\det(A)
$$

For a 3×3 matrix, multiplying every entry by 2 multiplies the determinant by 8.

**Property 2: Transpose**

$$
\det(A^T)=\det(A)
$$

Transposing a matrix does not change its determinant.

**Property 3: Matrix Product**

$$
\det(AB)=\det(A)\det(B)
$$

Therefore, the determinant of A² equals the square of the determinant of A.

**Property 4: Negative Matrix**

For a 3×3 matrix:

$$
\det(-A)=(-1)^3\det(A)=-\det(A)
$$

This happens because the matrix has an odd number of rows.

### Final Answer

| Expression | Result |
|------------|--------|
| det(2A) | -32 |
| det(Aᵀ) | -4 |
| det(A²) | 16 |
| det(-A) | 4 |

Therefore:

$$
\boxed{\det(2A)=-32}
$$

$$
\boxed{\det(A^T)=-4}
$$

$$
\boxed{\det(A^2)=16}
$$

$$
\boxed{\det(-A)=4}
$$

**Conclusion:** All four determinants can be calculated using determinant properties without knowing the individual entries of A.
