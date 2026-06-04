# Vectors

## Vector basics

A vector carries both magnitude and direction. In 3D:

$$\mathbf{v} = v_1\hat{i} + v_2\hat{j} + v_3\hat{k}$$

**Magnitude**

$$|\mathbf{v}| = \sqrt{v_1^2 + v_2^2 + v_3^2}$$

**Unit vector**

$$\hat{v} = \frac{\mathbf{v}}{|\mathbf{v}|} \quad \text{(normalised — magnitude = 1)}$$

**Vector from A to B**

$$\overrightarrow{AB} = \overrightarrow{OB} - \overrightarrow{OA}$$

**Direction cosines** $l, m, n$

$$l = \frac{x}{r}, \quad m = \frac{y}{r}, \quad n = \frac{z}{r} \quad \text{where } r = |\mathbf{v}|$$

These are the cosines of the angles the vector makes with each axis. Always:

$$l^2 + m^2 + n^2 = 1$$

---

## Linear independence and span

Vectors are linearly dependent if one can be written as a combination of the others.

**Test using determinant:** Form matrix $A$ with vectors as columns.

$$\det(A) = 0 \implies \text{dependent}, \quad \det(A) \neq 0 \implies \text{independent}$$

Also: $\text{rank}(A) < \text{number of vectors} \implies$ dependent; $\text{rank}(A) = \text{number of vectors} \implies$ independent.

**The span of a set of vectors is all possible linear combinations. A basis is the minimum linearly independent set that spans the whole space.**

In $\mathbb{R}^3$, any 4 or more vectors must be linearly dependent. Three coplanar vectors in 3D are also dependent.

---

## Dot product (scalar product)

Gives a scalar — measures how much two vectors point in the same direction.

**Geometric form**

$$\mathbf{a} \cdot \mathbf{b} = |\mathbf{a}||\mathbf{b}|\cos\theta$$

**Component form**

$$\mathbf{a} \cdot \mathbf{b} = a_1 b_1 + a_2 b_2 + a_3 b_3$$

**Angle between vectors**

$$\theta = \arccos\!\left(\frac{\mathbf{a} \cdot \mathbf{b}}{|\mathbf{a}||\mathbf{b}|}\right)$$

**Projection of $\mathbf{u}$ onto $\mathbf{v}$**

$$\text{proj}_{\mathbf{v}}\,\mathbf{u} = \frac{\mathbf{u} \cdot \mathbf{v}}{|\mathbf{v}|^2}\,\mathbf{v}$$

**If $\mathbf{a} \cdot \mathbf{b} = 0$, the vectors are perpendicular. $\hat{i}\cdot\hat{i} = 1$, $\hat{i}\cdot\hat{j} = 0$.**

Real application: $W = \mathbf{F} \cdot \mathbf{d}$. Only the force component along the direction of motion does work.

Orthonormal basis: all basis vectors have unit length and are mutually perpendicular. The Gram–Schmidt process converts any independent set into an orthonormal basis.

---

## Cross product (vector product)

Gives a vector perpendicular to both inputs. Its magnitude equals the area of the parallelogram spanned by the two vectors.

**Geometric form**

$$|\mathbf{a} \times \mathbf{b}| = |\mathbf{a}||\mathbf{b}|\sin\theta \quad \text{(direction by right-hand rule)}$$

**Component form (expand the determinant)**

$$\mathbf{a} \times \mathbf{b} = \begin{vmatrix} \hat{i} & \hat{j} & \hat{k} \\ a_1 & a_2 & a_3 \\ b_1 & b_2 & b_3 \end{vmatrix} = \hat{i}(a_2 b_3 - a_3 b_2) - \hat{j}(a_1 b_3 - a_3 b_1) + \hat{k}(a_1 b_2 - a_2 b_1)$$

**$\mathbf{a} \times \mathbf{b} = -(\mathbf{b} \times \mathbf{a})$ — order matters! $\mathbf{a} \times \mathbf{a} = \mathbf{0}$. NOT commutative.**

**Scalar triple product**

$$\mathbf{a} \cdot (\mathbf{b} \times \mathbf{c}) = \det[\mathbf{a};\, \mathbf{b};\, \mathbf{c}]$$

$= 0$ if the three vectors are coplanar. Otherwise equals the signed volume of the parallelepiped.

**Vector triple product**

$$\mathbf{a} \times (\mathbf{b} \times \mathbf{c}) = \mathbf{b}(\mathbf{a} \cdot \mathbf{c}) - \mathbf{c}(\mathbf{a} \cdot \mathbf{b})$$

---

## Engineering applications of vectors

**Area of triangle $ABC$**

$$\text{Area} = \frac{1}{2}\left|\overrightarrow{AB} \times \overrightarrow{AC}\right|$$

**Angular velocity**

$$\mathbf{v} = \boldsymbol{\omega} \times \mathbf{r} \quad \text{(velocity = angular velocity cross position)}$$

**Moment of force**

$$\mathbf{M} = \mathbf{r} \times \mathbf{F}$$
