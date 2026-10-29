
## Exercise 6: Parameter and Invertibility

### Given Matrix

```math
A(t)=
\begin{pmatrix}
t & 1\\
2 & t
\end{pmatrix}
```

We need to find all values of t for which the matrix is not invertible and explain the relationship between invertibility and the determinant.

### Step 1: Determinant Formula

For a 2×2 matrix:

```math
A=
\begin{pmatrix}
a & b\\
c & d
\end{pmatrix}
```

The determinant is:

```math
\det(A)=ad-bc
```

A square matrix is invertible if and only if its determinant is nonzero.

Therefore, the matrix is not invertible when:

```math
\det(A)=0
```

### Step 2: Calculate the Determinant

Given:

```math
A(t)=
\begin{pmatrix}
t & 1\\
2 & t
\end{pmatrix}
```

Apply the determinant formula:

```math
\det(A(t))=t\cdot t-1\cdot2
```

Simplifying:

```math
\boxed{\det(A(t))=t^2-2}
```

### Step 3: Find the Values of t

The matrix is not invertible when its determinant equals zero.

Therefore:

```math
t^2-2=0
```

Move 2 to the other side:

```math
t^2=2
```

Taking the square root:

```math
t=\pm\sqrt{2}
```

Thus:

```math
\boxed{t=\sqrt{2}\quad\text{or}\quad t=-\sqrt{2}}
```

### Step 4: Explain Invertibility

A matrix is invertible if its determinant is different from zero.

For our matrix:

```math
\det(A(t))=t^2-2
```

When:

```math
t=\sqrt{2}
```

we obtain:

```math
\det(A(\sqrt{2}))=(\sqrt{2})^2-2
```

```math
=2-2=0
```

Similarly, when:

```math
t=-\sqrt{2}
```

we obtain:

```math
\det(A(-\sqrt{2}))=(-\sqrt{2})^2-2
```

```math
=2-2=0
```

Therefore, the matrix is not invertible for these two values.

For every other real value of t, the determinant is nonzero, so the matrix is invertible.

### Step 5: Verification

The inverse formula for a 2×2 matrix is:

```math
A^{-1}=
\frac{1}{ad-bc}
\begin{pmatrix}
d & -b\\
-c & a
\end{pmatrix}
```

Applying this formula:

```math
A(t)^{-1}=
\frac{1}{t^2-2}
\begin{pmatrix}
t & -1\\
-2 & t
\end{pmatrix}
```

This inverse exists only when:

```math
t^2-2\neq0
```

Therefore:

```math
t\neq\pm\sqrt{2}
```

When t equals either positive or negative square root of 2, the denominator becomes zero, so the inverse does not exist.

This confirms our result.

### Final Answer

The matrix is not invertible when:

```math
\boxed{t=\pm\sqrt{2}}
```

The matrix is invertible for:

```math
\boxed{t\in\mathbb{R}\setminus\{-\sqrt{2},\sqrt{2}\}}
```

**Conclusion:** The determinant of the matrix is t² - 2. A square matrix is not invertible exactly when its determinant equals zero. Therefore, the matrix is singular for t = √2 and t = -√2, and invertible for all other real values of t.
