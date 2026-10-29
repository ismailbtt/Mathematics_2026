
## Exercise 11: When Do Matrices Commute?

Given:

$$
A=\begin{pmatrix}
1&1\\
0&1
\end{pmatrix}
$$

$$
B=\begin{pmatrix}
a&b\\
c&d
\end{pmatrix}
$$

We need to find the conditions under which AB = BA.

### Step 1: Calculate AB

$$
AB=
\begin{pmatrix}
1&1\\
0&1
\end{pmatrix}
\begin{pmatrix}
a&b\\
c&d
\end{pmatrix}
$$

Multiplying rows by columns:

$$
AB=
\begin{pmatrix}
a+c&b+d\\
c&d
\end{pmatrix}
$$

### Step 2: Calculate BA

$$
BA=
\begin{pmatrix}
a&b\\
c&d
\end{pmatrix}
\begin{pmatrix}
1&1\\
0&1
\end{pmatrix}
$$

Multiplying rows by columns:

$$
BA=
\begin{pmatrix}
a&a+b\\
c&c+d
\end{pmatrix}
$$

### Step 3: Find the Conditions for AB = BA

For the matrices to be equal, their corresponding entries must be equal.

Therefore:

$$
a+c=a
$$

$$
b+d=a+b
$$

$$
c=c
$$

$$
d=c+d
$$

From the first equation:

$$
c=0
$$

From the second equation:

$$
d=a
$$

The third equation is always true, and the fourth equation also gives c = 0.

Therefore, the conditions are:

$$
\boxed{c=0,\quad d=a}
$$

### Step 4: General Form of B

Substituting these conditions into B:

$$
\boxed{
B=\begin{pmatrix}
a&b\\
0&a
\end{pmatrix}
}
$$

Here, a and b can be any real numbers.

### Explanation

Matrix multiplication is generally not commutative, meaning AB is not always equal to BA.

However, in this example, the matrices commute when c = 0 and d = a.

Therefore, B must be an upper triangular matrix with equal diagonal entries.

### Verification

Substitute the general form of B:

$$
B=\begin{pmatrix}
a&b\\
0&a
\end{pmatrix}
$$

Calculate AB:

$$
AB=
\begin{pmatrix}
1&1\\
0&1
\end{pmatrix}
\begin{pmatrix}
a&b\\
0&a
\end{pmatrix}
$$

$$
AB=\begin{pmatrix}
a&a+b\\
0&a
\end{pmatrix}
$$

Calculate BA:

$$
BA=
\begin{pmatrix}
a&b\\
0&a
\end{pmatrix}
\begin{pmatrix}
1&1\\
0&1
\end{pmatrix}
$$

$$
BA=\begin{pmatrix}
a&a+b\\
0&a
\end{pmatrix}
$$

Thus:

$$
\boxed{AB=BA}
$$

### Final Answer

The conditions are:

$$
\boxed{c=0,\quad d=a}
$$

The general form of all matrices B that commute with A is:

$$
\boxed{
B=\begin{pmatrix}
a&b\\
0&a
\end{pmatrix}
}
$$

where a and b are arbitrary real numbers.
