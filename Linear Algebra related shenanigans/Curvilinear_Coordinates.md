# Curvilinear Coordinates

## Polar coordinates (2D)

Instead of $(x, y)$, describe a point by its distance $r$ from the origin and angle $\theta$ from the $x$-axis.

**Polar → Cartesian**

$$x = r\cos\theta, \quad y = r\sin\theta$$

**Cartesian → Polar**

$$r = \sqrt{x^2 + y^2}$$

$$\theta = \begin{cases} \arctan(y/x) & \text{if } x > 0 \quad \text{(Q1, Q4)} \\ \arctan(y/x) + \pi & \text{if } x < 0,\; y \geq 0 \quad \text{(Q2)} \\ \arctan(y/x) - \pi & \text{if } x < 0,\; y < 0 \quad \text{(Q3)} \end{cases}$$

To convert a polar equation to Cartesian: use $r^2 = x^2 + y^2$, $r\cos\theta = x$, $r\sin\theta = y$.  
To go the other way: substitute $x = r\cos\theta$, $y = r\sin\theta$ into the Cartesian equation.

---

## Cylindrical coordinates (3D)

Polar in the $xy$-plane, plus $z$ for height. Suits cylinders and any geometry with rotational symmetry about the $z$-axis.

**Cylindrical → Cartesian**

$$x = r\cos\theta, \quad y = r\sin\theta, \quad z = z$$

**Cartesian → Cylindrical**

$$r = \sqrt{x^2 + y^2}, \quad \theta = \arctan\!\left(\frac{y}{x}\right), \quad z = z$$

---

## Spherical coordinates (3D)

$\rho$ = distance from origin, $\theta$ = azimuth angle in $xy$-plane, $\varphi$ = polar angle from $z$-axis.

**Spherical → Cartesian**

$$x = \rho\sin\varphi\cos\theta, \quad y = \rho\sin\varphi\sin\theta, \quad z = \rho\cos\varphi$$

$$\theta \in [0, 2\pi], \quad \varphi \in [0, \pi]$$

**Cartesian → Spherical**

$$\rho = \sqrt{x^2 + y^2 + z^2}$$

**$\varphi$ is measured from the $z$-axis ($0$ = north pole, $\pi$ = south pole), not from the $xy$-plane. Don't mix up $\theta$ and $\varphi$.**

---

## Parametric curves

Define $x$, $y$ (and $z$) each as a function of a parameter $t$.

**2D**

$$x = f(t), \quad y = g(t)$$

**3D position vector**

$$\mathbf{r}(t) = x(t)\,\hat{i} + y(t)\,\hat{j} + z(t)\,\hat{k}$$

**Velocity**

$$\mathbf{v} = \frac{d\mathbf{r}}{dt}$$

**Acceleration**

$$\mathbf{a} = \frac{d^2\mathbf{r}}{dt^2}$$

**Projectile motion example** (fired from origin at speed $v_0$, angle $\alpha$):

$$\mathbf{r}(t) = (v_0\cos\alpha \cdot t)\,\hat{i} + \!\left(v_0\sin\alpha \cdot t - \tfrac{1}{2}gt^2\right)\hat{j}$$

Hits ground when the $\hat{j}$-component $= 0$.

**Lissajous curves:** $x = a\sin(mt + \varepsilon_1)$, $y = b\sin(nt + \varepsilon_2)$. Used in electronics to compare two frequencies on an oscilloscope.

---

## Curvature

Measures how sharply a curve bends at a point. Radius of curvature $R = 1/\kappa$ — large $R$ means a gentle bend.

**For $y = f(x)$**

$$\kappa = \frac{|y''|}{(1 + y'^2)^{3/2}}$$

**For parametric $\mathbf{r}(t)$**

$$\kappa = \frac{|\mathbf{r}'(t) \times \mathbf{r}''(t)|}{|\mathbf{r}'(t)|^3}$$

**Centre of curvature** $(h, k)$ — centre of the best-fit circle at that point:

$$h = x - R\sin\theta, \quad k = y + R\cos\theta$$

where $\theta = \arctan(y')$ and $R = \dfrac{(1 + y'^2)^{3/2}}{y''}$
