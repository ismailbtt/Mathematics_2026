
# Exercise 12. Finding Inverses Without Starting from Scratch — Solution

## Given Matrix

We are given:

$$
A^{-1}=\begin{pmatrix}2 & -1 \\ -3 & 2\end{pmatrix}
$$

The task is to calculate $(3A)^{-1}$, $(A^T)^{-1}$, and $(A^2)^{-1}$ without finding the original matrix $A$.

## Step 1. Calculate (3A)^{-1}

For a nonzero scalar $k$, the inverse property is:

$$
(kA)^{-1}=\frac{1}{k}A^{-1}
$$

Using $k=3$:

$$
(3A)^{-1}=\frac{1}{3}A^{-1}
$$

Substituting the given matrix:

$$
(3A)^{-1}=\frac{1}{3}\begin{pmatrix}2 & -1 \\ -3 & 2\end{pmatrix}
$$

Therefore:

$$
\boxed{(3A)^{-1}=\begin{pmatrix}\frac{2}{3} & -\frac{1}{3} \\ -1 & \frac{2}{3}\end{pmatrix}}
$$

## Step 2. Calculate (A^T)^{-1}

The inverse of a transpose follows the property:

$$
(A^T)^{-1}=(A^{-1})^T
$$

This means we transpose the given inverse matrix.

$$
(A^{-1})^T=\begin{pmatrix}2 & -3 \\ -1 & 2\end{pmatrix}
$$

Therefore:

$$
\boxed{(A^T)^{-1}=\begin{pmatrix}2 & -3 \\ -1 & 2\end{pmatrix}}
$$

## Step 3. Calculate (A^2)^{-1}

The inverse of a product follows the property:

$$
(AB)^{-1}=B^{-1}A^{-1}
$$

Since $A^2=AA$, we have:

$$
(A^2)^{-1}=A^{-1}A^{-1}=(A^{-1})^2
$$

Substituting the given inverse matrix:

$$
(A^2)^{-1}=\begin{pmatrix}2 & -1 \\ -3 & 2\end{pmatrix}\begin{pmatrix}2 & -1 \\ -3 & 2\end{pmatrix}
$$

Performing matrix multiplication:

$$
(A^2)^{-1}=\begin{pmatrix}4+3 & -2-2 \\ -6-6 & 3+4\end{pmatrix}
$$

Therefore:

$$
\boxed{(A^2)^{-1}=\begin{pmatrix}7 & -4 \\ -12 & 7\end{pmatrix}}
$$

## Step 4. Verification

We can verify the results using inverse matrix properties without calculating $A$.

**For $(3A)^{-1}$:**

$$
(3A)\left(\frac{1}{3}A^{-1}\right)=AA^{-1}=I
$$

**For $(A^T)^{-1}$:**

$$
A^T(A^{-1})^T=(A^{-1}A)^T=I
$$

**For $(A^2)^{-1}$:**

$$
A^2(A^{-1})^2=AAA^{-1}A^{-1}=I
$$

All three expressions produce the identity matrix, confirming the results.

## Final Answer

**1. Inverse of 3A:**

$$
\boxed{(3A)^{-1}=\begin{pmatrix}\frac{2}{3} & -\frac{1}{3} \\ -1 & \frac{2}{3}\end{pmatrix}}
$$

**2. Inverse of the transpose:**

$$
\boxed{(A^T)^{-1}=\begin{pmatrix}2 & -3 \\ -1 & 2\end{pmatrix}}
$$

**3. Inverse of A squared:**

$$
\boxed{(A^2)^{-1}=\begin{pmatrix}7 & -4 \\ -12 & 7\end{pmatrix}}
$$

**Conclusion:**

All three inverses were calculated using inverse matrix properties without finding the original matrix $A$.

The results were verified using the identity $AA^{-1}=I$, confirming that the calculations are correct.
