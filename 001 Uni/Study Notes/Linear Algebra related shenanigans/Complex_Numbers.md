# Complex Numbers

## Complex number basics

A complex number: $z = x + iy$, where $x$ = real part, $y$ = imaginary part, $i = \sqrt{-1}$.

**Conjugate**

$$\bar{z} = x - iy \quad \text{(flip sign of imaginary part)}$$

**Modulus**

$$|z| = \sqrt{x^2 + y^2} \quad \text{and} \quad z\cdot\bar{z} = |z|^2 = x^2 + y^2$$

**Powers of $i$ cycle with period 4:** $i^1 = i,\; i^2 = -1,\; i^3 = -i,\; i^4 = 1,\; i^5 = i, \ldots$

---

## Arithmetic in Cartesian form

**Addition**

$$z_1 + z_2 = (x_1 + x_2) + i(y_1 + y_2)$$

**Multiplication**

$$z_1 z_2 = (x_1 x_2 - y_1 y_2) + i(x_1 y_2 + x_2 y_1)$$

**Division**

$$\frac{z_1}{z_2} = \frac{z_1 \cdot \bar{z}_2}{z_2 \cdot \bar{z}_2}$$

Multiply top and bottom by the conjugate of the denominator.

Geometric region: $|z - z_0| = r$ is a circle. $|z - z_0| \leq r$ is a filled disk. Both centred at $z_0$ with radius $r$.

---

## Polar form and the Argand diagram

Plot $z = x + iy$ as the point $(x, y)$ on the complex plane (Argand diagram).

**Polar form**

$$z = r(\cos\theta + i\sin\theta) = r\operatorname{cis}\theta$$

**Modulus and argument**

$$r = |z| = \sqrt{x^2 + y^2}$$

$$\theta = \begin{cases} \arctan(y/x) & \text{if } x > 0 \quad \text{(Q1, Q4)} \\ \arctan(y/x) + \pi & \text{if } x < 0,\; y \geq 0 \quad \text{(Q2)} \\ \arctan(y/x) - \pi & \text{if } x < 0,\; y < 0 \quad \text{(Q3)} \end{cases}$$

Principal argument: $\theta \in (-\pi, \pi]$

**Multiplication in polar form**

$$z_1 z_2 = r_1 r_2 \operatorname{cis}(\theta_1 + \theta_2) \quad \to \text{multiply moduli, add arguments}$$

**Division in polar form**

$$\frac{z_1}{z_2} = \frac{r_1}{r_2}\operatorname{cis}(\theta_1 - \theta_2) \quad \to \text{divide moduli, subtract arguments}$$

---

## Powers and roots — De Moivre's theorem

Raises a complex number to any power.

**De Moivre's theorem**

$$z^n = r^n \operatorname{cis}(n\theta) = r^n(\cos n\theta + i\sin n\theta)$$

**$n$th roots** ($n$ distinct roots for $w^n = z$)

$$w_k = r^{1/n} \cdot \operatorname{cis}\!\left(\frac{\theta + 2\pi k}{n}\right), \quad k = 0, 1, \ldots, n-1$$

**The $n$ roots are equally spaced around a circle of radius $r^{1/n}$, separated by angle $2\pi/n$. Always sketch the Argand diagram.**

Fundamental theorem of algebra: any degree-$n$ polynomial has exactly $n$ roots in $\mathbb{C}$. This is why complex numbers exist — real polynomials don't always have real roots.

---

## Euler's formula and exponential form

**Euler's formula**

$$e^{i\theta} = \cos\theta + i\sin\theta$$

**Exponential form**

$$z = r\,e^{i\theta}$$

**General complex exponential**

$$e^{x+iy} = e^x(\cos y + i\sin y)$$

Famous identity (plug $\theta = \pi$ into Euler's formula):

$$e^{i\pi} + 1 = 0$$

Exponential form makes multiplication and powers trivial — just use exponent rules.

---

## Engineering application — Impedance (AC circuits)

Impedance combines resistance $R$, inductance $L$, and capacitance $C$ into one complex number ($j = i$ in engineering notation).

**Angular frequency**

$$\omega = 2\pi f$$

**Impedance**

$$Z = R + j\!\left(\omega L - \frac{1}{\omega C}\right)$$

$|Z|$ = magnitude of impedance. $\arg(Z)$ = phase angle $\varphi$.

**Current**

$$I = \frac{V_0}{|Z|}\sin(\omega t - \varphi)$$

If $\varphi > 0$ (inductive): current lags voltage. If $\varphi < 0$ (capacitive): current leads voltage. The angle tells you the timing relationship between voltage and current.
