
# Exercise 15. Two Methods for Solving the Same System — Solution

## Given

We are given the system:

$$
Ax=b
$$

where:

$$
A=\begin{pmatrix}2 & 1 \\ 1 & 3\end{pmatrix}
$$

$$
b=\begin{pmatrix}7 \\ 8\end{pmatrix}
$$

The task is to solve the system using two methods:

1. The inverse matrix method.
2. Gaussian elimination.

We will compare the methods and verify the solution.

## Method 1. Using the Inverse Matrix

### Step 1. Calculate the Determinant

The determinant of $A$ is:

$$
\det(A)=(2)(3)-(1)(1)
$$

$$
\det(A)=6-1=5
$$

Since $\det(A)\neq 0$, the inverse exists.

### Step 2. Find the Inverse

Using the inverse formula:

$$
A^{-1}=\frac{1}{5}\begin{pmatrix}3 & -1 \\ -1 & 2\end{pmatrix}
$$

### Step 3. Calculate x

The solution is:

$$
x=A^{-1}b
$$

Substituting:

$$
x=\frac{1}{5}\begin{pmatrix}3 & -1 \\ -1 & 2\end{pmatrix}\begin{pmatrix}7 \\ 8\end{pmatrix}
$$

Performing matrix multiplication:

$$
x=\frac{1}{5}\begin{pmatrix}21-8 \\ -7+16\end{pmatrix}
$$

$$
x=\frac{1}{5}\begin{pmatrix}13 \\ 9\end{pmatrix}
$$

Therefore:

$$
\boxed{x=\begin{pmatrix}\frac{13}{5} \\ \frac{9}{5}\end{pmatrix}}
$$

## Method 2. Using Gaussian Elimination

### Step 1. Construct the Augmented Matrix

The system is:

$$
2x_1+x_2=7
$$

$$
x_1+3x_2=8
$$

The augmented matrix is:

$$
\left[\begin{array}{cc|c}2 & 1 & 7 \\ 1 & 3 & 8\end{array}\right]
$$

### Step 2. Swap the Rows

Apply:

$$
R_1\leftrightarrow R_2
$$

The matrix becomes:

$$
\left[\begin{array}{cc|c}1 & 3 & 8 \\ 2 & 1 & 7\end{array}\right]
$$

### Step 3. Eliminate the First Element of Row 2

Apply:

$$
R_2\rightarrow R_2-2R_1
$$

The matrix becomes:

$$
\left[\begin{array}{cc|c}1 & 3 & 8 \\ 0 & -5 & -9\end{array}\right]
$$

Divide the second row by $-5$:

$$
R_2\rightarrow -\frac{1}{5}R_2
$$

Therefore:

$$
\left[\begin{array}{cc|c}1 & 3 & 8 \\ 0 & 1 & \frac{9}{5}\end{array}\right]
$$

### Step 4. Find the Solution

Eliminate the element above the second pivot:

$$
R_1\rightarrow R_1-3R_2
$$

The resulting matrix is:

$$
\left[\begin{array}{cc|c}1 & 0 & \frac{13}{5} \\ 0 & 1 & \frac{9}{5}\end{array}\right]
$$

Therefore:

$$
\boxed{x_1=\frac{13}{5},\qquad x_2=\frac{9}{5}}
$$

The solution vector is:

$$
\boxed{x=\begin{pmatrix}\frac{13}{5} \\ \frac{9}{5}\end{pmatrix}}
$$

## Step 5. Verify the Solution

To verify, substitute the result into the original equation:

$$
Ax=b
$$

$$
\begin{pmatrix}2 & 1 \\ 1 & 3\end{pmatrix}\begin{pmatrix}\frac{13}{5} \\ \frac{9}{5}\end{pmatrix}
$$

Performing matrix multiplication:

$$
=\begin{pmatrix}\frac{26}{5}+\frac{9}{5} \\ \frac{13}{5}+\frac{27}{5}\end{pmatrix}
$$

$$
=\begin{pmatrix}\frac{35}{5} \\ \frac{40}{5}\end{pmatrix}
$$

$$
=\begin{pmatrix}7 \\ 8\end{pmatrix}=b
$$

The solution satisfies the original system.

## Step 6. Compare the Two Methods

**Inverse Matrix Method:**

- Requires calculating the determinant.
- Requires finding the inverse matrix.
- Uses matrix multiplication to obtain the solution.

**Gaussian Elimination:**

- Uses elementary row operations.
- Does not require calculating the inverse.
- Directly reduces the system to obtain the unknown variables.

In this example, Gaussian elimination required one row swap and three additional row operations.

The inverse matrix method required a determinant calculation, construction of the inverse, and matrix multiplication.

Both methods are straightforward for this small system, but Gaussian elimination is slightly simpler because it avoids calculating the inverse matrix.

## Final Answer

Both methods give the same solution:

$$
\boxed{x=\begin{pmatrix}\frac{13}{5} \\ \frac{9}{5}\end{pmatrix}}
$$

**Verification:**

$$
Ax=\begin{pmatrix}7 \\ 8\end{pmatrix}=b
$$

**Conclusion:**

Both the inverse matrix method and Gaussian elimination produce the same correct solution.

Gaussian elimination is slightly more efficient in this example because it solves the system directly without computing the inverse matrix.

Therefore, Gaussian elimination is the simpler method for this particular system.
