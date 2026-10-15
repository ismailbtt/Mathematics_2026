 
# Exercise 2. Addition and Scalar Multiplication

## Question

Given

$$
A=
\begin{pmatrix}
1 & 2\\
-1 & 3
\end{pmatrix},
\qquad
B=
\begin{pmatrix}
4 & -2\\
0 & 5
\end{pmatrix}
$$

Compute:

1. $A+B$
2. $A-B$
3. $3A-2B$

Explain why matrix addition is possible only for matrices of the same size.

---

## Solution 1. Calculate A+B

We add the corresponding entries of both matrices.

$$
A+B=
\begin{pmatrix}
1 & 2\\
-1 & 3
\end{pmatrix}
+
\begin{pmatrix}
4 & -2\\
0 & 5
\end{pmatrix}
$$

Step by step:

$$
A+B=
\begin{pmatrix}
1+4 & 2+(-2)\\
-1+0 & 3+5
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
5 & 0\\
-1 & 8
\end{pmatrix}
$$

**Final Answer:**

$$
\boxed{
A+B=
\begin{pmatrix}
5 & 0\\
-1 & 8
\end{pmatrix}
}
$$

---

## Solution 2. Calculate A-B

We subtract the corresponding entries.

$$
A-B=
\begin{pmatrix}
1 & 2\\
-1 & 3
\end{pmatrix}
-
\begin{pmatrix}
4 & -2\\
0 & 5
\end{pmatrix}
$$

Step by step:

$$
A-B=
\begin{pmatrix}
1-4 & 2-(-2)\\
-1-0 & 3-5
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
-3 & 4\\
-1 & -2
\end{pmatrix}
$$

**Final Answer:**

$$
\boxed{
A-B=
\begin{pmatrix}
-3 & 4\\
-1 & -2
\end{pmatrix}
}
$$

---

## Solution 3. Calculate 3A-2B

First, multiply every entry of matrix A by 3.

$$
3A=
3\begin{pmatrix}
1 & 2\\
-1 & 3
\end{pmatrix}
$$

$$
3A=
\begin{pmatrix}
3 & 6\\
-3 & 9
\end{pmatrix}
$$

Next, multiply every entry of matrix B by 2.

$$
2B=
2\begin{pmatrix}
4 & -2\\
0 & 5
\end{pmatrix}
$$

$$
2B=
\begin{pmatrix}
8 & -4\\
0 & 10
\end{pmatrix}
$$

Now subtract the matrices.

$$
3A-2B=
\begin{pmatrix}
3 & 6\\
-3 & 9
\end{pmatrix}
-
\begin{pmatrix}
8 & -4\\
0 & 10
\end{pmatrix}
$$

Step by step:

$$
=
\begin{pmatrix}
3-8 & 6-(-4)\\
-3-0 & 9-10
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
-5 & 10\\
-3 & -1
\end{pmatrix}
$$

**Final Answer:**

$$
\boxed{
3A-2B=
\begin{pmatrix}
-5 & 10\\
-3 & -1
\end{pmatrix}
}
$$

---

## Explanation

Matrix addition and subtraction are performed entry by entry.

Both matrices must have the same number of rows and columns.

In this exercise:

$$
A:2\times2
$$

$$
B:2\times2
$$

Therefore, addition and subtraction are possible.

If the dimensions were different, corresponding entries would not exist for every position.

---

## Mathematical Verification

We can verify the third result using:

$$
3A-2B=3(A-B)+B
$$

We already calculated:

$$
A-B=
\begin{pmatrix}
-3 & 4\\
-1 & -2
\end{pmatrix}
$$

Multiply by 3:

$$
3(A-B)=
\begin{pmatrix}
-9 & 12\\
-3 & -6
\end{pmatrix}
$$

Now add B:

$$
3(A-B)+B=
\begin{pmatrix}
-9 & 12\\
-3 & -6
\end{pmatrix}
+
\begin{pmatrix}
4 & -2\\
0 & 5
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
-5 & 10\\
-3 & -1
\end{pmatrix}
$$

This matches our original calculation.

Therefore, the result is correct.

---

## Final Answers

$$
\boxed{
A+B=
\begin{pmatrix}
5 & 0\\
-1 & 8
\end{pmatrix}
}
$$

$$
\boxed{
A-B=
\begin{pmatrix}
-3 & 4\\
-1 & -2
\end{pmatrix}
}
$$

$$
\boxed{
3A-2B=
\begin{pmatrix}
-5 & 10\\
-3 & -1
\end{pmatrix}
}
$$
