
# Exercise 14 – A Matrix That Is Its Own Inverse

## Question

We are given a square matrix A satisfying:

A² = I

1. Prove that A⁻¹ = A.
2. Provide a 2 × 2 example different from I and -I.
3. Verify your example by matrix multiplication.

## Solution

### Step 1: Prove That A⁻¹ = A

By definition, the inverse of a square matrix A satisfies:

AA⁻¹ = A⁻¹A = I

We are given:

A² = I

Since A² = AA, we have:

AA = I

Thus, multiplying A by itself produces the identity matrix.

Therefore, A is its own inverse:

A⁻¹ = A

Such a matrix is called an involutory matrix.

### Step 2: Provide an Example

Consider the matrix:

```text
A = [ 0  1 ]
    [ 1  0 ]
```

This matrix is different from both I and -I.

We will verify that it satisfies A² = I.

### Step 3: Verify by Multiplication

Calculate:

A² = AA

Substituting the matrix:

```text
A² = [ 0  1 ] [ 0  1 ]
     [ 1  0 ] [ 1  0 ]
```

Performing matrix multiplication:

```text
A² = [ 0(0)+1(1)  0(1)+1(0) ]
     [ 1(0)+0(1)  1(1)+0(0) ]
```

Simplifying:

```text
A² = [ 1  0 ]
     [ 0  1 ] = I
```

Therefore:

A² = I

Since AA = I, the matrix is its own inverse:

A⁻¹ = A

## Final Answer

If a square matrix satisfies:

A² = I

then:

A⁻¹ = A

An example is:

```text
A = [ 0  1 ]
    [ 1  0 ]
```

Verification:

```text
A² = [ 1  0 ] = I
     [ 0  1 ]
```

Conclusion:

The condition A² = I proves that a matrix is its own inverse.

The given example satisfies this condition and is different from both I and -I.

Therefore, the statement is verified.
