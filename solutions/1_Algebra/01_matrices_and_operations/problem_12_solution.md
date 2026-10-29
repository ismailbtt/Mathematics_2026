
## Exercise 12: Formula for a Matrix Power

Given:

$$
A=\begin{pmatrix}
1&1\\
0&1
\end{pmatrix}
$$

We need to calculate A², A³, and A⁴, find a general formula for Aⁿ, and prove it using mathematical induction.

### Step 1: Calculate A²

$$
A^2=A\cdot A
$$

$$
A^2=
\begin{pmatrix}
1&1\\
0&1
\end{pmatrix}
\begin{pmatrix}
1&1\\
0&1
\end{pmatrix}
$$

Multiplying rows by columns:

$$
A^2=
\begin{pmatrix}
1(1)+1(0)&1(1)+1(1)\\
0(1)+1(0)&0(1)+1(1)
\end{pmatrix}
$$

Therefore:

$$
\boxed{
A^2=\begin{pmatrix}
1&2\\
0&1
\end{pmatrix}
}
$$

### Step 2: Calculate A³

$$
A^3=A^2A
$$

$$
A^3=
\begin{pmatrix}
1&2\\
0&1
\end{pmatrix}
\begin{pmatrix}
1&1\\
0&1
\end{pmatrix}
$$

$$
A^3=
\begin{pmatrix}
1(1)+2(0)&1(1)+2(1)\\
0(1)+1(0)&0(1)+1(1)
\end{pmatrix}
$$

Therefore:

$$
\boxed{
A^3=\begin{pmatrix}
1&3\\
0&1
\end{pmatrix}
}
$$

### Step 3: Calculate A⁴

$$
A^4=A^3A
$$

$$
A^4=
\begin{pmatrix}
1&3\\
0&1
\end{pmatrix}
\begin{pmatrix}
1&1\\
0&1
\end{pmatrix}
$$

$$
A^4=
\begin{pmatrix}
1(1)+3(0)&1(1)+3(1)\\
0(1)+1(0)&0(1)+1(1)
\end{pmatrix}
$$

Therefore:

$$
\boxed{
A^4=\begin{pmatrix}
1&4\\
0&1
\end{pmatrix}
}
$$

### Step 4: Find the General Formula

From the previous calculations:

$$
A^1=\begin{pmatrix}
1&1\\
0&1
\end{pmatrix}
$$

$$
A^2=\begin{pmatrix}
1&2\\
0&1
\end{pmatrix}
$$

$$
A^3=\begin{pmatrix}
1&3\\
0&1
\end{pmatrix}
$$

$$
A^4=\begin{pmatrix}
1&4\\
0&1
\end{pmatrix}
$$

We observe that the diagonal entries remain equal to 1, the lower-left entry remains 0, and the upper-right entry increases by 1 with each power.

Therefore, we conjecture:

$$
\boxed{
A^n=\begin{pmatrix}
1&n\\
0&1
\end{pmatrix}
}
$$

### Step 5: Proof by Mathematical Induction

**Base Case: n = 1**

For n = 1:

$$
A^1=\begin{pmatrix}
1&1\\
0&1
\end{pmatrix}
$$

The formula is correct for n = 1.

**Inductive Hypothesis**

Assume the formula is true for some positive integer n:

$$
A^n=\begin{pmatrix}
1&n\\
0&1
\end{pmatrix}
$$

**Inductive Step**

We must prove that the formula is true for n + 1.

Start with:

$$
A^{n+1}=A^nA
$$

Substitute the inductive hypothesis:

$$
A^{n+1}=
\begin{pmatrix}
1&n\\
0&1
\end{pmatrix}
\begin{pmatrix}
1&1\\
0&1
\end{pmatrix}
$$

Multiply the matrices:

$$
A^{n+1}=
\begin{pmatrix}
1(1)+n(0)&1(1)+n(1)\\
0(1)+1(0)&0(1)+1(1)
\end{pmatrix}
$$

Simplifying:

$$
\boxed{
A^{n+1}=\begin{pmatrix}
1&n+1\\
0&1
\end{pmatrix}
}
$$

This is exactly the required formula for n + 1.

Therefore, by mathematical induction, the formula holds for every positive integer n.

### Step 6: Verification

To verify the formula, consider n = 5.

Using the general formula:

$$
A^5=\begin{pmatrix}
1&5\\
0&1
\end{pmatrix}
$$

Now calculate directly:

$$
A^5=A^4A
$$

$$
A^5=
\begin{pmatrix}
1&4\\
0&1
\end{pmatrix}
\begin{pmatrix}
1&1\\
0&1
\end{pmatrix}
$$

$$
A^5=\begin{pmatrix}
1&5\\
0&1
\end{pmatrix}
$$

Both methods give the same result.

### Final Answer

The general formula for the nth power of A is:

$$
\boxed{
A^n=\begin{pmatrix}
1&n\\
0&1
\end{pmatrix}
}
$$

This formula is valid for all positive integers n and has been proven using mathematical induction.
