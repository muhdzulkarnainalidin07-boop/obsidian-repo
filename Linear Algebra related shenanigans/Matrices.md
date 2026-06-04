# Matrices

## Matrices — the basics

A matrix is a rectangular grid of numbers. Its order is $m \times n$ (rows $\times$ columns).

**Transpose ($A^\top$)**

Flip rows and columns. $(A^\top)^\top = A$. $I^\top = I$.

Special types to know: Square ($m = n$), Identity (diagonal of 1s), Diagonal, Symmetric ($A^\top = A$), Anti-symmetric ($A^\top = -A$), Triangular (upper/lower).

---

## Matrix arithmetic

**Addition / Subtraction**

Only works on same-order matrices. Add element by element.

$$A + B = B + A \quad \text{(commutative)}$$

**Scalar multiplication**

Multiply every element by the scalar. $3A$ triples every entry.

**Matrix multiplication**

$$A_{m \times n} \times B_{n \times p} = C_{m \times p}$$

Inner dimensions must match. Each entry = dot product of a row of $A$ with a column of $B$.

**$AB \neq BA$ in general — multiplication is NOT commutative.**

But: $A(BC) = (AB)C$. And $(AB)^\top = B^\top A^\top$ (order reverses on transpose).

---

## Determinants

A single number per square matrix. Tells you if the matrix is invertible and how much it scales area/volume.

**$2 \times 2$**

$$\det(A) = ad - bc \quad \text{for } A = \begin{pmatrix} a & b \\ c & d \end{pmatrix}$$

**$3 \times 3$ (cofactor expansion)**

$$\det(A) = a_{11}C_{11} + a_{12}C_{12} + a_{13}C_{13}$$

Cofactor: $C_{ij} = (-1)^{i+j} \cdot M_{ij}$

$M_{ij}$ = determinant of the matrix with row $i$ and column $j$ removed.

Sign pattern for cofactors:

$$\begin{pmatrix} + & - & + \\ - & + & - \\ + & - & + \end{pmatrix}$$

**Key properties:**

- $\det(AB) = \det(A)\cdot\det(B)$
- $\det(A^\top) = \det(A)$
- $\det(I) = 1$
- Swapping two rows negates the determinant
- If any row is a multiple of another, $\det = 0$

**Vectors are linearly dependent $\iff \det$ of the matrix they form $= 0$.**

---

## Matrix inversion

$A^{-1}$ undoes $A$: $AA^{-1} = A^{-1}A = I$. Only exists when $\det(A) \neq 0$.

**$2 \times 2$ shortcut**

$$A^{-1} = \frac{1}{\det A}\begin{pmatrix} d & -b \\ -c & a \end{pmatrix}$$

**General ($n \times n$)**

$$A^{-1} = \frac{\text{adj}(A)}{\det(A)}$$

where $\text{adj}(A) = C^\top$ (transpose of the cofactor matrix).

**Rules:**
- $(A^{-1})^{-1} = A$
- $(AB)^{-1} = B^{-1}A^{-1}$ (order reverses!)
- $(A^\top)^{-1} = (A^{-1})^\top$

---

## Solving linear systems — 3 methods

Any system $A\mathbf{x} = \mathbf{b}$ can be solved three ways.

**Method 1 — Matrix inversion**

$$\mathbf{x} = A^{-1}\mathbf{b}$$

Clean but only works when $A$ is invertible.

**Method 2 — Cramer's rule**

$$x_i = \frac{\det(A_i)}{\det(A)}$$

where $A_i = A$ with its $i$-th column replaced by $\mathbf{b}$. Good for small systems only.

**Method 3 — Gaussian elimination**

Form $(A \mid \mathbf{b})$ and use row operations to reach row echelon form, then back-substitute.

Allowed row ops: swap rows · multiply a row by a non-zero scalar · add a multiple of one row to another.

- One solution $\to$ unique pivot in each variable column
- No solution $\to$ row like $\begin{pmatrix} 0 & 0 & 0 & \mid & k \end{pmatrix}$ with $k \neq 0$
- Infinite solutions $\to$ free variable (set it $= t$, express others in terms of $t$)

---

## Rank and Nullity

Row-reduce to echelon form, then count:

**Rank**

$$\text{rank}(A) = \text{number of non-zero rows in echelon form}$$

**Nullity**

$$\text{nullity}(A) = \text{number of columns} - \text{rank}(A)$$

**$\text{rank}(A) = \text{rank}(A^\top)$ always.**
