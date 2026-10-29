
## Exercise 14: Rotation Matrices

Given the rotation matrix:

```math
R(\theta)=
\begin{pmatrix}
\cos\theta & -\sin\theta\\
\sin\theta & \cos\theta
\end{pmatrix}
```

We need to calculate R(α)R(β), prove that it equals R(α+β), and explain the result geometrically.

### Step 1: Write the Rotation Matrices

For angle α:

```math
R(\alpha)=
\begin{pmatrix}
\cos\alpha & -\sin\alpha\\
\sin\alpha & \cos\alpha
\end{pmatrix}
```

For angle β:

```math
R(\beta)=
\begin{pmatrix}
\cos\beta & -\sin\beta\\
\sin\beta & \cos\beta
\end{pmatrix}
```

### Step 2: Calculate R(α)R(β)

Multiply the two matrices:

```math
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos\alpha & -\sin\alpha\\
\sin\alpha & \cos\alpha
\end{pmatrix}
\begin{pmatrix}
\cos\beta & -\sin\beta\\
\sin\beta & \cos\beta
\end{pmatrix}
```

Using row-by-column multiplication:

```math
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos\alpha\cos\beta-\sin\alpha\sin\beta &
-\cos\alpha\sin\beta-\sin\alpha\cos\beta\\
\sin\alpha\cos\beta+\cos\alpha\sin\beta &
-\sin\alpha\sin\beta+\cos\alpha\cos\beta
\end{pmatrix}
```

### Step 3: Apply the Angle-Sum Formulas

The trigonometric angle-sum identities are:

```math
\cos(\alpha+\beta)=
\cos\alpha\cos\beta-\sin\alpha\sin\beta
```

```math
\sin(\alpha+\beta)=
\sin\alpha\cos\beta+\cos\alpha\sin\beta
```

Using these identities:

```math
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos(\alpha+\beta) & -\sin(\alpha+\beta)\\
\sin(\alpha+\beta) & \cos(\alpha+\beta)
\end{pmatrix}
```

### Step 4: Compare with R(α+β)

By definition:

```math
R(\alpha+\beta)=
\begin{pmatrix}
\cos(\alpha+\beta) & -\sin(\alpha+\beta)\\
\sin(\alpha+\beta) & \cos(\alpha+\beta)
\end{pmatrix}
```

Both matrices are identical.

Therefore:

```math
\boxed{R(\alpha)R(\beta)=R(\alpha+\beta)}
```

### Step 5: Geometrical Explanation

A rotation matrix represents a counterclockwise rotation of a vector in the plane.

When two rotations are applied consecutively, their angles are added.

For example:

- First rotate a vector by 30 degrees.
- Then rotate the resulting vector by 60 degrees.
- The total rotation is 90 degrees.

Mathematically:

```math
R(60^\circ)R(30^\circ)=R(90^\circ)
```

This means that applying two consecutive rotations is equivalent to applying one rotation by the sum of their angles.

### Step 6: Verification with a Numerical Example

Let:

```math
\alpha=30^\circ,\quad \beta=60^\circ
```

We know:

```math
\cos30^\circ=\frac{\sqrt3}{2},
\quad
\sin30^\circ=\frac12
```

```math
\cos60^\circ=\frac12,
\quad
\sin60^\circ=\frac{\sqrt3}{2}
```

Therefore:

```math
R(30^\circ)=
\begin{pmatrix}
\frac{\sqrt3}{2} & -\frac12\\
\frac12 & \frac{\sqrt3}{2}
\end{pmatrix}
```

```math
R(60^\circ)=
\begin{pmatrix}
\frac12 & -\frac{\sqrt3}{2}\\
\frac{\sqrt3}{2} & \frac12
\end{pmatrix}
```

Multiplying:

```math
R(30^\circ)R(60^\circ)=
\begin{pmatrix}
0 & -1\\
1 & 0
\end{pmatrix}
```

Now calculate R(90°):

```math
R(90^\circ)=
\begin{pmatrix}
\cos90^\circ & -\sin90^\circ\\
\sin90^\circ & \cos90^\circ
\end{pmatrix}
```

Since:

```math
\cos90^\circ=0,\quad\sin90^\circ=1
```

We obtain:

```math
R(90^\circ)=
\begin{pmatrix}
0 & -1\\
1 & 0
\end{pmatrix}
```

Thus:

```math
\boxed{R(30^\circ)R(60^\circ)=R(90^\circ)}
```

The numerical verification confirms the general formula.

### Final Answer

The product of two rotation matrices is:

```math
\boxed{
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos(\alpha+\beta) & -\sin(\alpha+\beta)\\
\sin(\alpha+\beta) & \cos(\alpha+\beta)
\end{pmatrix}
}
```

Therefore:

```math
\boxed{R(\alpha)R(\beta)=R(\alpha+\beta)}
```

**Conclusion:** The composition of two counterclockwise rotations is equivalent to a single rotation through the sum of their angles. This demonstrates the connection between matrix multiplication and geometric transformations.

