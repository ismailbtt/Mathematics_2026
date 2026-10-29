## Exercise 10: Columns of a Matrix Product

Given:

$$
A=\begin{pmatrix}
1&2&0\\
0&1&1
\end{pmatrix}
$$

$$
B=\begin{pmatrix}
1&2\\
-1&0\\
3&1
\end{pmatrix}
$$

The columns of B are:

$$
b_1=\begin{pmatrix}1\\-1\\3\end{pmatrix},
\quad
b_2=\begin{pmatrix}2\\0\\1\end{pmatrix}
$$

### Step 1: Calculate Ab₁

$$
Ab_1=
\begin{pmatrix}
1&2&0\\
0&1&1
\end{pmatrix}
\begin{pmatrix}1\\-1\\3\end{pmatrix}
$$

$$
=\begin{pmatrix}
1(1)+2(-1)+0(3)\\
0(1)+1(-1)+1(3)
\end{pmatrix}
$$

$$
=\begin{pmatrix}1-2+0\\0-1+3\end{pmatrix}
$$

$$
\boxed{Ab_1=\begin{pmatrix}-1\\2\end{pmatrix}}
$$

### Step 2: Calculate Ab₂

$$
Ab_2=
\begin{pmatrix}
1&2&0\\
0&1&1
\end{pmatrix}
\begin{pmatrix}2\\0\\1\end{pmatrix}
$$

$$
=\begin{pmatrix}
1(2)+2(0)+0(1)\\
0(2)+1(0)+1(1)
\end{pmatrix}
$$

$$
=\begin{pmatrix}2\\1\end{pmatrix}
$$

$$
\boxed{Ab_2=\begin{pmatrix}2\\1\end{pmatrix}}
$$

### Step 3: Calculate AB

$$
AB=
\begin{pmatrix}
1&2&0\\
0&1&1
\end{pmatrix}
\begin{pmatrix}
1&2\\
-1&0\\
3&1
\end{pmatrix}
$$

Multiplying rows by columns:

$$
AB=
\begin{pmatrix}
1(1)+2(-1)+0(3)&1(2)+2(0)+0(1)\\
0(1)+1(-1)+1(3)&0(2)+1(0)+1(1)
\end{pmatrix}
$$

Therefore:

$$
\boxed{
AB=\begin{pmatrix}
-1&2\\
2&1
\end{pmatrix}
}
$$

### Step 4: Compare the Results

Previously, we found:

$$
Ab_1=\begin{pmatrix}-1\\2\end{pmatrix}
$$

$$
Ab_2=\begin{pmatrix}2\\1\end{pmatrix}
$$

Combining these vectors as columns:

$$
\begin{pmatrix}Ab_1&Ab_2\end{pmatrix}
=
\begin{pmatrix}-1&2\\2&1\end{pmatrix}
$$

This is exactly the matrix AB.

### Explanation

Matrix multiplication can be understood as multiplying the first matrix by each column of the second matrix separately.

In general, if:

$$
B=\begin{pmatrix}b_1&b_2&\cdots&b_n\end{pmatrix}
$$

then:

$$
\boxed{
AB=\begin{pmatrix}Ab_1&Ab_2&\cdots&Ab_n\end{pmatrix}
}
$$

### Verification

The first column of AB is:

$$
\begin{pmatrix}-1\\2\end{pmatrix}=Ab_1
$$

The second column of AB is:

$$
\begin{pmatrix}2\\1\end{pmatrix}=Ab_2
$$

Therefore, the columns of AB are exactly Ab₁ and Ab₂, as required.
