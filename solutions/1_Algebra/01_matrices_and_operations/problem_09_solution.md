## Exercise 9: Composing Transformations

Given:

$$
S=\begin{pmatrix}2&0\\0&1\end{pmatrix},
\quad
R=\begin{pmatrix}0&-1\\1&0\end{pmatrix}
$$

$$
x=\begin{pmatrix}1\\2\end{pmatrix}
$$

### Step 1: Calculate RSx

First, multiply S by x:

$$
Sx=
\begin{pmatrix}2&0\\0&1\end{pmatrix}
\begin{pmatrix}1\\2\end{pmatrix}
=
\begin{pmatrix}2\\2\end{pmatrix}
$$

Then, multiply R by the result:

$$
RSx=
\begin{pmatrix}0&-1\\1&0\end{pmatrix}
\begin{pmatrix}2\\2\end{pmatrix}
$$

$$
=\begin{pmatrix}0(2)-1(2)\\1(2)+0(2)\end{pmatrix}
$$

$$
\boxed{RSx=\begin{pmatrix}-2\\2\end{pmatrix}}
$$

### Step 2: Calculate SRx

First, multiply R by x:

$$
Rx=
\begin{pmatrix}0&-1\\1&0\end{pmatrix}
\begin{pmatrix}1\\2\end{pmatrix}
=
\begin{pmatrix}-2\\1\end{pmatrix}
$$

Then, multiply S by the result:

$$
SRx=
\begin{pmatrix}2&0\\0&1\end{pmatrix}
\begin{pmatrix}-2\\1\end{pmatrix}
$$

$$
=\begin{pmatrix}2(-2)+0(1)\\0(-2)+1(1)\end{pmatrix}
$$

$$
\boxed{SRx=\begin{pmatrix}-4\\1\end{pmatrix}}
$$

### Step 3: Compare the Results

$$
RSx=\begin{pmatrix}-2\\2\end{pmatrix}
$$

$$
SRx=\begin{pmatrix}-4\\1\end{pmatrix}
$$

Therefore:

$$
\boxed{RSx\neq SRx}
$$

### Explanation

Matrix S scales the horizontal coordinate by 2, while R rotates a vector 90 degrees counterclockwise.

In RSx, scaling happens first, followed by rotation.

In SRx, rotation happens first, followed by scaling.

The results are different because the order of transformations matters.

### Verification

Calculate the transformation matrices directly:

$$
RS=\begin{pmatrix}0&-1\\2&0\end{pmatrix}
$$

$$
SR=\begin{pmatrix}0&-2\\1&0\end{pmatrix}
$$

Since RS and SR are different, their transformations can produce different results.
