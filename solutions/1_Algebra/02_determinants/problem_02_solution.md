
## Exercise 2: Determinant of a 3×3 Matrix

### Given Matrix

```math
A=
\begin{pmatrix}
1 & 2 & -1\\
0 & 3 & 4\\
2 & 1 & 5
\end{pmatrix}
```

We need to calculate the determinant of matrix A using Sarrus' rule and verify the result using a determinant property.

### Step 1: Sarrus' Rule

For a 3×3 matrix:

```math
A=
\begin{pmatrix}
a & b & c\\
d & e & f\\
g & h & i
\end{pmatrix}
```

The determinant is:

```math
\det(A)=aei+bfg+cdh-ceg-bdi-afh
```

This means we add the products of the three downward diagonals and subtract the products of the three upward diagonals.

### Step 2: Apply Sarrus' Rule

For our matrix:

```math
A=
\begin{pmatrix}
1 & 2 & -1\\
0 & 3 & 4\\
2 & 1 & 5
\end{pmatrix}
```

Using the formula:

```math
\det(A)=
(1)(3)(5)+(2)(4)(2)+(-1)(0)(1)
-
(-1)(3)(2)-(2)(0)(5)-(1)(4)(1)
```

Calculate the positive diagonal products:

```math
(1)(3)(5)=15
```

```math
(2)(4)(2)=16
```

```math
(-1)(0)(1)=0
```

Their sum is:

```math
15+16+0=31
```

Now calculate the negative diagonal products:

```math
(-1)(3)(2)=-6
```

```math
(2)(0)(5)=0
```

```math
(1)(4)(1)=4
```

Their sum is:

```math
-6+0+4=-2
```

Therefore:

```math
\det(A)=31-(-2)
```

```math
\det(A)=31+2
```

### Step 3: Final Determinant

```math
\boxed{\det(A)=33}
```

### Step 4: Verification Using a Determinant Property

We can verify the result using a row operation.

Adding a multiple of one row to another row does not change the determinant.

Apply:

```math
R_3\leftarrow R_3-2R_1
```

Calculate the new third row:

```math
(2,1,5)-2(1,2,-1)=(0,-3,7)
```

The new matrix is:

```math
A'=
\begin{pmatrix}
1 & 2 & -1\\
0 & 3 & 4\\
0 & -3 & 7
\end{pmatrix}
```

Since this row operation does not change the determinant:

```math
\det(A')=\det(A)
```

Expand along the first column, which now contains two zeros:

```math
\det(A')=
1\begin{vmatrix}
3 & 4\\
-3 & 7
\end{vmatrix}
```

Using the 2×2 determinant formula:

```math
\det(A')=1(3\cdot7-4\cdot(-3))
```

```math
=21+12
```

```math
\boxed{\det(A')=33}
```

The result matches our calculation using Sarrus' rule.

Therefore, the determinant is verified.

### Step 5: Explanation

Sarrus' rule is a method for calculating the determinant of a 3×3 matrix using diagonal products.

A useful determinant property is that adding a multiple of one row to another does not change the determinant.

In this exercise, we used this property to create zeros and verify our result with a smaller 2×2 determinant.

### Final Answer

```math
\boxed{
\det\begin{pmatrix}
1 & 2 & -1\\
0 & 3 & 4\\
2 & 1 & 5
\end{pmatrix}=33
}
```

**Conclusion:** The determinant of matrix A is 33. The result was calculated using Sarrus' rule and independently verified using a row operation and determinant expansion.
