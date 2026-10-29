
## Exercise 8: Row Operations and Their Reversibility

Given:

$$
A=\begin{pmatrix}
1&2&-1\\
2&4&1\\
-1&1&3
\end{pmatrix}
$$

### Step 1: R₂ ← R₂ - 2R₁

$$
R_2=(2,4,1)-2(1,2,-1)=(0,0,3)
$$

Result:

$$
\begin{pmatrix}
1&2&-1\\
0&0&3\\
-1&1&3
\end{pmatrix}
$$

**Inverse operation:**

$$
R_2\leftarrow R_2+2R_1
$$

### Step 2: R₃ ← R₃ + R₁

$$
R_3=(-1,1,3)+(1,2,-1)=(0,3,2)
$$

Result:

$$
\begin{pmatrix}
1&2&-1\\
0&0&3\\
0&3&2
\end{pmatrix}
$$

**Inverse operation:**

$$
R_3\leftarrow R_3-R_1
$$

### Step 3: Interchange R₂ and R₃

Swap the second and third rows.

Final matrix:

$$
\boxed{
\begin{pmatrix}
1&2&-1\\
0&3&2\\
0&0&3
\end{pmatrix}
}
$$

**Inverse operation:**

$$
R_2\leftrightarrow R_3
$$

### Explanation

Elementary row operations are reversible.

- Adding a multiple of one row can be reversed by subtracting the same multiple.
- Interchanging two rows can be reversed by interchanging them again.

### Verification

Apply the inverse operations in reverse order:

1. Swap R₂ and R₃.
2. Apply R₃ ← R₃ - R₁.
3. Apply R₂ ← R₂ + 2R₁.

We obtain:

$$
\begin{pmatrix}
1&2&-1\\
2&4&1\\
-1&1&3
\end{pmatrix}
$$

This is the original matrix A.

Therefore, all three row operations are reversible.
