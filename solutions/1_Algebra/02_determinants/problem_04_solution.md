
## Exercise 3: Swapping Two Rows

### Given Matrix

```math
A=
\begin{pmatrix}
1 & 2 & 0\\
0 & 3 & 1\\
2 & 1 & 1
\end{pmatrix}
```

We need to calculate det(A), swap the first and second rows to obtain matrix B, predict det(B), and verify the result.

### Step 1: Calculate det(A)

Using Sarrus' rule:

```math
\det(A)=
\begin{vmatrix}
1 & 2 & 0\\
0 & 3 & 1\\
2 & 1 & 1
\end{vmatrix}
```

For a 3×3 matrix, Sarrus' rule is:

```math
\det(A)=aei+bfg+cdh-ceg-bdi-afh
```

Substituting the entries:

```math
\det(A)=
(1)(3)(1)+(2)(1)(2)+(0)(0)(1)
-
(0)(3)(2)-(2)(0)(1)-(1)(1)(1)
```

Calculate the positive diagonal products:

```math
(1)(3)(1)=3
```

```math
(2)(1)(2)=4
```

```math
(0)(0)(1)=0
```

Their sum is:

```math
3+4+0=7
```

Calculate the negative diagonal products:

```math
(0)(3)(2)=0
```

```math
(2)(0)(1)=0
```

```math
(1)(1)(1)=1
```

Their sum is:

```math
0+0+1=1
```

Therefore:

```math
\det(A)=7-1
```

```math
\boxed{\det(A)=6}
```

### Step 2: Swap the First and Second Rows

Apply the row operation:

```math
R_1\leftrightarrow R_2
```

The new matrix B is:

```math
B=
\begin{pmatrix}
0 & 3 & 1\\
1 & 2 & 0\\
2 & 1 & 1
\end{pmatrix}
```

### Step 3: Predict det(B)

An important determinant property states:

**Swapping two rows of a matrix changes the sign of its determinant.**

Therefore:

```math
\det(B)=-\det(A)
```

Since:

```math
\det(A)=6
```

We predict:

```math
\det(B)=-6
```

Thus:

```math
\boxed{\det(B)=-6}
```

### Step 4: Verify det(B) by Calculation

Using Sarrus' rule:

```math
\det(B)=
\begin{vmatrix}
0 & 3 & 1\\
1 & 2 & 0\\
2 & 1 & 1
\end{vmatrix}
```

Substituting the entries:

```math
\det(B)=
(0)(2)(1)+(3)(0)(2)+(1)(1)(1)
-
(1)(2)(2)-(3)(1)(1)-(0)(0)(1)
```

Calculate the positive products:

```math
0+0+1=1
```

Calculate the negative products:

```math
4+3+0=7
```

Therefore:

```math
\det(B)=1-7
```

```math
\boxed{\det(B)=-6}
```

### Step 5: Compare the Results

We calculated:

```math
\det(A)=6
```

And:

```math
\det(B)=-6
```

Therefore:

```math
\boxed{\det(B)=-\det(A)}
```

The direct calculation confirms our prediction.

### Step 6: Explanation

The determinant changes sign when two rows of a square matrix are interchanged.

This property applies to matrices of any size.

Swapping two rows reverses the orientation represented by the determinant, but does not change its absolute value.

In this example:

```math
|\det(A)|=6
```

```math
|\det(B)|=6
```

Both matrices are invertible because their determinants are nonzero.

### Final Answer

Original matrix:

```math
\boxed{\det(A)=6}
```

After swapping the first and second rows:

```math
\boxed{\det(B)=-6}
```

The determinant property is verified:

```math
\boxed{\det(B)=-\det(A)}
```

**Conclusion:** Interchanging two rows changes the sign of the determinant without changing its absolute value. Our direct calculations confirm this property.
