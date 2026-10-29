
## Exercise 13: A Recurrence Written in Matrix Form

Given:

$$
F=\begin{pmatrix}
1&1\\
1&0
\end{pmatrix}
$$

We need to calculate F², F³, F⁴, and F⁵, compare the results with the Fibonacci sequence, and explain how matrix multiplication performs a recurrence step.

### Step 1: Calculate F²

$$
F^2=F\cdot F
$$

$$
F^2=
\begin{pmatrix}
1&1\\
1&0
\end{pmatrix}
\begin{pmatrix}
1&1\\
1&0
\end{pmatrix}
$$

Multiplying rows by columns:

$$
F^2=
\begin{pmatrix}
1(1)+1(1)&1(1)+1(0)\\
1(1)+0(1)&1(1)+0(0)
\end{pmatrix}
$$

Therefore:

$$
\boxed{
F^2=\begin{pmatrix}
2&1\\
1&1
\end{pmatrix}
}
$$

### Step 2: Calculate F³

$$
F^3=F^2F
$$

$$
F^3=
\begin{pmatrix}
2&1\\
1&1
\end{pmatrix}
\begin{pmatrix}
1&1\\
1&0
\end{pmatrix}
$$

$$
F^3=
\begin{pmatrix}
2(1)+1(1)&2(1)+1(0)\\
1(1)+1(1)&1(1)+1(0)
\end{pmatrix}
$$

Therefore:

$$
\boxed{
F^3=\begin{pmatrix}
3&2\\
2&1
\end{pmatrix}
}
$$

### Step 3: Calculate F⁴

$$
F^4=F^3F
$$

$$
F^4=
\begin{pmatrix}
3&2\\
2&1
\end{pmatrix}
\begin{pmatrix}
1&1\\
1&0
\end{pmatrix}
$$

$$
F^4=
\begin{pmatrix}
3(1)+2(1)&3(1)+2(0)\\
2(1)+1(1)&2(1)+1(0)
\end{pmatrix}
$$

Therefore:

$$
\boxed{
F^4=\begin{pmatrix}
5&3\\
3&2
\end{pmatrix}
}
$$

### Step 4: Calculate F⁵

$$
F^5=F^4F
$$

$$
F^5=
\begin{pmatrix}
5&3\\
3&2
\end{pmatrix}
\begin{pmatrix}
1&1\\
1&0
\end{pmatrix}
$$

$$
F^5=
\begin{pmatrix}
5(1)+3(1)&5(1)+3(0)\\
3(1)+2(1)&3(1)+2(0)
\end{pmatrix}
$$

Therefore:

$$
\boxed{
F^5=\begin{pmatrix}
8&5\\
5&3
\end{pmatrix}
}
$$

### Step 5: Compare with the Fibonacci Sequence

The Fibonacci sequence is:

$$
0,1,1,2,3,5,8,\ldots
$$

Each number is the sum of the two previous numbers.

The recurrence relation is:

$$
f_{n+1}=f_n+f_{n-1}
$$

where:

$$
f_0=0,\quad f_1=1
$$

From our calculations:

$$
F^2=\begin{pmatrix}2&1\\1&1\end{pmatrix}
$$

$$
F^3=\begin{pmatrix}3&2\\2&1\end{pmatrix}
$$

$$
F^4=\begin{pmatrix}5&3\\3&2\end{pmatrix}
$$

$$
F^5=\begin{pmatrix}8&5\\5&3\end{pmatrix}
$$

We observe that the entries of these matrices are consecutive Fibonacci numbers.

The general formula is:

$$
\boxed{
F^n=\begin{pmatrix}
f_{n+1}&f_n\\
f_n&f_{n-1}
\end{pmatrix}
}
$$

This formula holds for all positive integers n.

### Step 6: Multiply F by a Vector

Given:

$$
v=\begin{pmatrix}a\\b\end{pmatrix}
$$

Calculate:

$$
Fv=
\begin{pmatrix}
1&1\\
1&0
\end{pmatrix}
\begin{pmatrix}
a\\
b
\end{pmatrix}
$$

Multiplying:

$$
Fv=
\begin{pmatrix}
1(a)+1(b)\\
1(a)+0(b)
\end{pmatrix}
$$

Therefore:

$$
\boxed{
Fv=\begin{pmatrix}
a+b\\
a
\end{pmatrix}
}
$$

### Step 7: Explanation of the Recurrence

The matrix F transforms the vector containing two consecutive terms into a new vector.

The first component becomes the sum of the two terms.

The second component keeps the previous first term.

For example:

$$
F\begin{pmatrix}1\\0\end{pmatrix}
=
\begin{pmatrix}1\\1\end{pmatrix}
$$

Applying F again:

$$
F\begin{pmatrix}1\\1\end{pmatrix}
=
\begin{pmatrix}2\\1\end{pmatrix}
$$

Again:

$$
F\begin{pmatrix}2\\1\end{pmatrix}
=
\begin{pmatrix}3\\2\end{pmatrix}
$$

Again:

$$
F\begin{pmatrix}3\\2\end{pmatrix}
=
\begin{pmatrix}5\\3\end{pmatrix}
$$

This process generates consecutive Fibonacci numbers.

### Step 8: Verification

Using the formula:

$$
F^5=\begin{pmatrix}
f_6&f_5\\
f_5&f_4
\end{pmatrix}
$$

From the Fibonacci sequence:

$$
f_4=3,\quad f_5=5,\quad f_6=8
$$

Therefore:

$$
F^5=\begin{pmatrix}
8&5\\
5&3
\end{pmatrix}
$$

This matches our direct calculation.

### Final Answer

The matrix powers are:

$$
\boxed{F^2=\begin{pmatrix}2&1\\1&1\end{pmatrix}}
$$

$$
\boxed{F^3=\begin{pmatrix}3&2\\2&1\end{pmatrix}}
$$

$$
\boxed{F^4=\begin{pmatrix}5&3\\3&2\end{pmatrix}}
$$

$$
\boxed{F^5=\begin{pmatrix}8&5\\5&3\end{pmatrix}}
$$

The general relationship is:

$$
\boxed{
F^n=\begin{pmatrix}
f_{n+1}&f_n\\
f_n&f_{n-1}
\end{pmatrix}
}
$$

And the recurrence step is:

$$
\boxed{
F\begin{pmatrix}a\\b\end{pmatrix}
=
\begin{pmatrix}a+b\\a\end{pmatrix}
}
$$

Therefore, matrix multiplication provides a way to generate Fibonacci numbers using repeated applications of the same transformation.
