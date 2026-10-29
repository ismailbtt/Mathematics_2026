
## Exercise 15: Associativity of Multiplication and Different Calculation Paths

Given:

```math
A=\begin{pmatrix}
1&2&0\\
0&1&1
\end{pmatrix}
```

```math
B=\begin{pmatrix}
1&0\\
2&1\\
-1&3
\end{pmatrix}
```

```math
C=\begin{pmatrix}
2&1\\
0&-1
\end{pmatrix}
```

We need to calculate (AB)C and A(BC), compare the results and the number of intermediate operations, and explain the associative property of matrix multiplication.

### Step 1: Calculate AB

First, multiply A by B:

```math
AB=
\begin{pmatrix}
1&2&0\\
0&1&1
\end{pmatrix}
\begin{pmatrix}
1&0\\
2&1\\
-1&3
\end{pmatrix}
```

Using row-by-column multiplication:

```math
AB=
\begin{pmatrix}
1(1)+2(2)+0(-1)&1(0)+2(1)+0(3)\\
0(1)+1(2)+1(-1)&0(0)+1(1)+1(3)
\end{pmatrix}
```

Simplifying:

```math
AB=
\begin{pmatrix}
5&2\\
1&4
\end{pmatrix}
```

### Step 2: Calculate (AB)C

Now multiply AB by C:

```math
(AB)C=
\begin{pmatrix}
5&2\\
1&4
\end{pmatrix}
\begin{pmatrix}
2&1\\
0&-1
\end{pmatrix}
```

Multiplying:

```math
(AB)C=
\begin{pmatrix}
5(2)+2(0)&5(1)+2(-1)\\
1(2)+4(0)&1(1)+4(-1)
\end{pmatrix}
```

Simplifying:

```math
(AB)C=
\begin{pmatrix}
10&3\\
2&-3
\end{pmatrix}
```

Therefore:

```math
\boxed{
(AB)C=
\begin{pmatrix}
10&3\\
2&-3
\end{pmatrix}
}
```

### Step 3: Calculate BC

Now calculate the product B times C:

```math
BC=
\begin{pmatrix}
1&0\\
2&1\\
-1&3
\end{pmatrix}
\begin{pmatrix}
2&1\\
0&-1
\end{pmatrix}
```

Using row-by-column multiplication:

```math
BC=
\begin{pmatrix}
1(2)+0(0)&1(1)+0(-1)\\
2(2)+1(0)&2(1)+1(-1)\\
-1(2)+3(0)&-1(1)+3(-1)
\end{pmatrix}
```

Simplifying:

```math
BC=
\begin{pmatrix}
2&1\\
4&1\\
-2&-4
\end{pmatrix}
```

### Step 4: Calculate A(BC)

Now multiply A by BC:

```math
A(BC)=
\begin{pmatrix}
1&2&0\\
0&1&1
\end{pmatrix}
\begin{pmatrix}
2&1\\
4&1\\
-2&-4
\end{pmatrix}
```

Multiplying:

```math
A(BC)=
\begin{pmatrix}
1(2)+2(4)+0(-2)&1(1)+2(1)+0(-4)\\
0(2)+1(4)+1(-2)&0(1)+1(1)+1(-4)
\end{pmatrix}
```

Simplifying:

```math
A(BC)=
\begin{pmatrix}
10&3\\
2&-3
\end{pmatrix}
```

Therefore:

```math
\boxed{
A(BC)=
\begin{pmatrix}
10&3\\
2&-3
\end{pmatrix}
}
```

### Step 5: Compare the Results

From the first calculation:

```math
(AB)C=
\begin{pmatrix}
10&3\\
2&-3
\end{pmatrix}
```

From the second calculation:

```math
A(BC)=
\begin{pmatrix}
10&3\\
2&-3
\end{pmatrix}
```

Both results are identical.

Therefore:

```math
\boxed{(AB)C=A(BC)}
```

This verifies the associative property of matrix multiplication.

### Step 6: Compare the Number of Operations

We compare the number of scalar multiplications required for each method.

**Method 1: (AB)C**

First calculate AB:

- A has size 2 × 3.
- B has size 3 × 2.
- AB has size 2 × 2.
- Number of scalar multiplications: 2 × 3 × 2 = 12.

Then calculate (AB)C:

- AB has size 2 × 2.
- C has size 2 × 2.
- Number of scalar multiplications: 2 × 2 × 2 = 8.

Total:

```math
12+8=20
```

**Method 2: A(BC)**

First calculate BC:

- B has size 3 × 2.
- C has size 2 × 2.
- BC has size 3 × 2.
- Number of scalar multiplications: 3 × 2 × 2 = 12.

Then calculate A(BC):

- A has size 2 × 3.
- BC has size 3 × 2.
- Number of scalar multiplications: 2 × 3 × 2 = 12.

Total:

```math
12+12=24
```

**Comparison:**

| Method | Scalar Multiplications |
|--------|------------------------|
| (AB)C | 20 |
| A(BC) | 24 |

Therefore, calculating (AB)C requires fewer scalar multiplications.

```math
24-20=4
```

The first method saves 4 scalar multiplications.

### Step 7: Explanation

Matrix multiplication is associative.

This means that when multiplying three compatible matrices, changing the grouping does not change the final result.

Mathematically:

```math
\boxed{(AB)C=A(BC)}
```

However, the number of intermediate calculations can be different.

In this example, calculating AB first is more efficient because it requires fewer scalar multiplications.

Associativity is important because it allows us to choose the most efficient order of calculations without changing the result.

### Step 8: Verification

We calculated both expressions independently:

```math
(AB)C=
\begin{pmatrix}
10&3\\
2&-3
\end{pmatrix}
```

```math
A(BC)=
\begin{pmatrix}
10&3\\
2&-3
\end{pmatrix}
```

Since all corresponding entries are equal, the results are identical.

Thus:

```math
\boxed{(AB)C=A(BC)}
```

### Final Answer

The final result is:

```math
\boxed{
(AB)C=A(BC)=
\begin{pmatrix}
10&3\\
2&-3
\end{pmatrix}
}
```

The number of scalar multiplications is:

- (AB)C: 20 multiplications.
- A(BC): 24 multiplications.

**Conclusion:** Matrix multiplication is associative, meaning that changing the grouping of matrices does not change the final result. However, different calculation paths may require different numbers of operations. In this example, (AB)C is more efficient than A(BC).
