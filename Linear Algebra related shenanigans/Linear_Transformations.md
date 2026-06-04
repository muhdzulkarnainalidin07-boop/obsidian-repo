# Linear Transformations

## What makes something a linear transformation?

$T: \mathbb{R}^n \to \mathbb{R}^m$ is linear if it satisfies:

**Additivity**

$$T(\mathbf{u} + \mathbf{v}) = T(\mathbf{u}) + T(\mathbf{v})$$

**Homogeneity**

$$T(c\mathbf{u}) = cT(\mathbf{u})$$

**Zero maps to zero**

$$T(\mathbf{0}) = \mathbf{0}$$

**Any linear transformation can be written as $T(\mathbf{v}) = A\mathbf{v}$, where $A$ is an $m \times n$ matrix. The columns of $A$ are where the standard basis vectors land.**

---

## Finding the image of a curve or region

Two approaches when $T(\mathbf{v}) = A\mathbf{v}$:

**Inverse method**
1. Compute $A^{-1}$ (requires $\det(A) \neq 0$)
2. Express $x, y$ in terms of $x', y'$ using $\begin{bmatrix} x \\ y \end{bmatrix} = A^{-1}\begin{bmatrix} x' \\ y' \end{bmatrix}$
3. Substitute into the original curve equation

**Parametric (forward) method**
1. Write the original curve in parametric form
2. Apply the transformation: $\begin{bmatrix} x' \\ y' \end{bmatrix} = A \begin{bmatrix} \text{parametric expression} \end{bmatrix}$
3. Eliminate the parameter to get the image equation

**Area scaling**

$$\text{Image area} = |\det(A)| \times \text{original area}$$

$\det(A) = 0 \implies$ transformation collapses everything to a lower dimension.

---

## Rotation

Anti-clockwise rotation by angle $\alpha$:

$$R_\alpha = \begin{pmatrix} \cos\alpha & -\sin\alpha \\ \sin\alpha & \cos\alpha \end{pmatrix}$$

**For clockwise rotation by $\alpha$, use $R_{-\alpha}$: negate the $\sin\alpha$ terms.**

Rotation is orthogonal: $R^{-1} = R^\top$, $\det(R) = 1$.

---

## Reflection

**Through the $y$-axis**

$$M_y = \begin{pmatrix} -1 & 0 \\ 0 & 1 \end{pmatrix}$$

**Through the $x$-axis**

$$M_x = \begin{pmatrix} 1 & 0 \\ 0 & -1 \end{pmatrix}$$

Reflection is orthogonal ($M^{-1} = M^\top$) with $\det(M) = -1$. It is its own inverse.

---

## Projection

**Projection onto the $x$-axis**

$$P_x = \begin{pmatrix} 1 & 0 \\ 0 & 0 \end{pmatrix}$$

Projection is NOT invertible ($\det = 0$) — once projected, the $y$-coordinate information is lost.

---

## Composition of transformations

Apply right-to-left: if $S$ then $T$, the combined matrix is $C = TS$ (not $ST$).

$$\det(TS) = \det(T) \cdot \det(S)$$

---

## Invertibility and orthogonality

$T$ is invertible iff $\det(A) \neq 0$. The inverse transformation $T^{-1}$ has matrix $A^{-1}$.

**Orthogonal transformation**

Preserves distances:

$$A^\top A = A A^\top = I \implies A^{-1} = A^\top$$

Rotations and reflections are orthogonal. Projections are not.
