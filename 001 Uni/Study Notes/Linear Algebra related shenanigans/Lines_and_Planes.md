# Lines and Planes

## Lines in 3D — three forms

A line needs a point $C$ and a direction vector $\mathbf{a}$.

**Vector form**

$$\mathbf{r} = \mathbf{c} + t\mathbf{a}$$

**Parametric form**

$$x = c_1 + ta_1, \quad y = c_2 + ta_2, \quad z = c_3 + ta_3$$

**Cartesian form**

$$\frac{x - c_1}{a_1} = \frac{y - c_2}{a_2} = \frac{z - c_3}{a_3}$$

**Given two points $A$ and $B$: direction vector $= \overrightarrow{AB} = \overrightarrow{OB} - \overrightarrow{OA}$. Use either point as $C$.**

---

## Distances and angles — lines

**Angle between two lines**

$$\theta = \arccos\!\left(\frac{\mathbf{a}_1 \cdot \mathbf{a}_2}{|\mathbf{a}_1||\mathbf{a}_2|}\right) \quad \text{(use direction vectors)}$$

**Distance from point $P$ to a line**

$$d = \frac{|\overrightarrow{AP} \times \mathbf{v}|}{|\mathbf{v}|}$$

where $A$ is any point on the line and $\mathbf{v}$ is the direction vector.

---

## Planes in 3D

A plane is defined by a normal vector $\mathbf{n} = a\hat{i} + b\hat{j} + c\hat{k}$, perpendicular to the surface.

**Equation of a plane**

$$ax + by + cz = d$$

**From three points $A$, $B$, $C$**

$$\mathbf{n} = \overrightarrow{AB} \times \overrightarrow{AC} \quad \text{(normal = cross product of two edges)}$$

$$d = \mathbf{n} \cdot \overrightarrow{OA}$$

---

## Distances and angles — planes

**Distance from the origin to a plane**

$$p = \frac{|d|}{\sqrt{a^2 + b^2 + c^2}}$$

**Distance from point $P$ to a plane**

$$\text{dist} = \frac{|a\,p_x + b\,p_y + c\,p_z - d|}{\sqrt{a^2 + b^2 + c^2}}$$

**Angle between two planes**

$$\theta = \arccos\!\left(\frac{\mathbf{n}_1 \cdot \mathbf{n}_2}{|\mathbf{n}_1||\mathbf{n}_2|}\right) \quad \text{(angle between normals)}$$

---

## Intersections

**Line–plane intersection**

Substitute the parametric line equations into the plane equation. Solve for $t$, then substitute back to find the point.

**Plane–plane intersection**

Set up $[A \mid B]$ for both equations and Gaussian eliminate.

- One solution $\to$ a point
- Infinite solutions $\to$ a line
- No solution $\to$ parallel planes

**Two planes always either intersect in a line or are parallel. Three planes intersect at a point when the system has a unique solution.**
