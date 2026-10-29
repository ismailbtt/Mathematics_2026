
## Exercise 9: Area and the Determinant

### Given Vectors

We are given two vectors:

$$
u=\begin{pmatrix}
3\\
1
\end{pmatrix}
$$

$$
v=\begin{pmatrix}
1\\
4
\end{pmatrix}
$$

These vectors span a parallelogram.

We need to calculate its area using a determinant, reverse the order of the vectors, and explain what changes.

### Step 1: Construct the Matrix

Place the vectors as columns of a matrix:

$$
A=\begin{pmatrix}
3&1\\
1&4
\end{pmatrix}
$$

The area of the parallelogram is the absolute value of the determinant:

$$
\text{Area}=|\det(A)|
$$

### Step 2: Calculate the Determinant

For a 2×2 matrix:

$$
A=\begin{pmatrix}
a&b\\
c&d
\end{pmatrix}
$$

The determinant formula is:

$$
\det(A)=ad-bc
$$

Applying this formula:

$$
\det(A)=3(4)-1(1)
$$

$$
=12-1
$$

Therefore:

$$
\boxed{\det(A)=11}
$$

### Step 3: Calculate the Area

The area is the absolute value of the determinant.

$$
\text{Area}=|11|
$$

Therefore:

$$
\boxed{\text{Area}=11}
$$

The parallelogram has an area of 11 square units.

### Step 4: Reverse the Order of the Vectors

Now place vector v in the first column and vector u in the second column.

The new matrix is:

$$
B=\begin{pmatrix}
1&3\\
4&1
\end{pmatrix}
$$

Calculate its determinant:

$$
\det(B)=1(1)-3(4)
$$

$$
=1-12
$$

Therefore:

$$
\boxed{\det(B)=-11}
$$

### Step 5: Calculate the New Area

The area is always the absolute value of the determinant.

$$
\text{Area}=|\det(B)|
$$

$$
=|-11|
$$

Therefore:

$$
\boxed{\text{Area}=11}
$$

The area remains unchanged.

### Step 6: Compare the Results

Original order:

$$
\det(u,v)=11
$$

Reversed order:

$$
\det(v,u)=-11
$$

Therefore:

$$
\boxed{\det(v,u)=-\det(u,v)}
$$

However:

$$
|\det(u,v)|=|\det(v,u)|
$$

$$
\boxed{11=11}
$$

This shows that reversing the order of the vectors changes the sign of the determinant but does not change the area.

### Step 7: Geometrical Explanation

The determinant of two vectors in the plane represents the signed area of the parallelogram they span.

A positive determinant indicates one orientation, while a negative determinant indicates the opposite orientation.

When we reverse the order of the vectors, the orientation changes.

However, the geometric area cannot be negative.

Therefore, we use the absolute value of the determinant to calculate the area.

### Step 8: Verification

We can verify the area using the geometric formula:

$$
\text{Area}=|u_1v_2-u_2v_1|
$$

Substituting:

$$
\text{Area}=|3(4)-1(1)|
$$

$$
=|12-1|
$$

$$
=|11|
$$

Therefore:

$$
\boxed{\text{Area}=11}
$$

Reversing the vectors:

$$
\text{Area}=|1(1)-4(3)|
$$

$$
=|1-12|
$$

$$
=|-11|
$$

$$
\boxed{\text{Area}=11}
$$

Both calculations give the same area.

### Final Answer

The original determinant is:

$$
\boxed{\det(u,v)=11}
$$

After reversing the vectors:

$$
\boxed{\det(v,u)=-11}
$$

The parallelogram area is:

$$
\boxed{\text{Area}=11\text{ square units}}
$$

**Conclusion:** Reversing the order of the vectors changes the sign of the determinant because the orientation is reversed. However, the absolute value remains the same, so the area of the parallelogram does not change.
