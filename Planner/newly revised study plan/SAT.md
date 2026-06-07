# SAT — Math Crunch Day
**Location:** Home. **Exam countdown:** Math in 2 days. Physics in 3 days.
**Tonight's job:** Lock in every math topic from the exam list. No new Physics tonight.

---

## THE SYSTEM (read once, never again)

Each block is a **closed loop**. The loop is non-negotiable.

```
READ → CLOSE → WRITE COLD → CHECK → FIX (3× anything wrong) → MOVE ON
```

**Hard rules:**
- 3 minutes stuck on a blank = note it, move on. You are not failing, you are flagging.
- Never re-read a block you already checked. That's re-consumption, not consolidation.
- Every block ends with a **GATE**. Pass it or note the miss. Either way, you move forward.

**ADHD override:** If you've been sitting for 25+ minutes and feel the drift — stand up immediately. Do not negotiate. The break is built into the schedule.

---

## SCHEDULE OVERVIEW

| Time | Block | Topic |
|------|-------|-------|
| 4:30pm | MATH 1 | Determinants |
| 5:00pm | MATH 2 | Matrix Inversion |
| 5:30pm | — | Break |
| 5:45pm | MATH 3 | Gaussian Elimination + Rank/Nullity |
| 6:20pm | MATH 4 | Complex Numbers: forms + polar |
| 6:55pm | — | Break |
| 7:10pm | MATH 5 | Complex Numbers: De Moivre + roots |
| 7:40pm | MATH 6 | Linear Transformations |
| 8:15pm | — | Break |
| 8:30pm | MATH 7 | Curvilinear Coordinates |
| 9:00pm | MATH 8 | Curvature + Parametric Curves |
| 9:30pm | MATH 9 | Timed Gauntlet (all topics, no notes) |
| 10:15pm | — | STOP. Eat. No more math tonight. |

> Start at whatever time you're actually reading this. The relative order is what matters, not the clock times above.

---

## MATH 1 — 25 min | Determinants

### READ

**2×2:**
$$\det\begin{pmatrix}a&b\\c&d\end{pmatrix} = ad - bc$$

**3×3 cofactor expansion (row 1):**
$$\det(A) = a_1(b_2c_3 - b_3c_2) - a_2(b_1c_3 - b_3c_1) + a_3(b_1c_2 - b_2c_1)$$

**Sign grid — draw this before every 3×3, no exceptions:**
$$\begin{pmatrix}+&-&+\\-&+&-\\+&-&+\end{pmatrix} \quad C_{ij} = (-1)^{i+j}$$

The middle term is always negative. This is where people drop marks. Not the arithmetic — the sign.

**Sarrus' rule (3×3 shortcut):** Copy columns 1–2 to the right. Three diagonals down-right = positive. Three down-left = negative. Sum all six.

**Properties that examiners test:**

| Row operation | Effect on det |
|---------------|---------------|
| Swap two rows | Flips sign |
| Row of zeros | det = 0 |
| Row = multiple of another row | det = 0 |
| Scale one row by $k$ | det × $k$ |
| $\det(AB)$ | $= \det(A)\cdot\det(B)$ |
| $\det(A^T)$ | $= \det(A)$ |

### CLOSE. WRITE COLD.
- 2×2 formula
- 3×3 expansion (with sign grid drawn first)
- All 6 properties

### GATE
Write the 3×3 expansion one more time from scratch. Is the middle term negative? Is your sign grid correct?

If you missed either → write the expansion 3× before moving on.

---

## MATH 2 — 25 min | Matrix Inversion

### READ

**Before anything:** Check $\det(A) \neq 0$. If $\det(A) = 0$ → singular, no inverse, state this and stop. Proceeding anyway = zero marks for the question.

**2×2 shortcut:**
$$\begin{pmatrix}a&b\\c&d\end{pmatrix}^{-1} = \frac{1}{ad-bc}\begin{pmatrix}d&-b\\-c&a\end{pmatrix}$$

Pattern: swap diagonal, negate off-diagonal, divide by det.

**General method (any size):**
1. Compute $\det(A)$
2. Build cofactor matrix $C$: entry $C_{ij} = (-1)^{i+j} \cdot M_{ij}$ where $M_{ij}$ = det of submatrix with row $i$, col $j$ deleted
3. Transpose: $\text{adj}(A) = C^T$
4. $A^{-1} = \dfrac{\text{adj}(A)}{\det(A)}$

**Always verify:** $A \cdot A^{-1} = I$. If it doesn't equal $I$, you find the exact step that broke — not "arithmetic error" but which specific step.

**Worked example:**
$$A = \begin{pmatrix}3&1\\5&2\end{pmatrix}, \quad \det = 6-5 = 1$$
$$A^{-1} = \begin{pmatrix}2&-1\\-5&3\end{pmatrix}, \quad \text{verify: } AA^{-1} = I\ ✓$$

### CLOSE. WRITE COLD.
- Check-det-first rule
- 2×2 shortcut (pattern in words, then formula)
- 4 general steps
- Do a full inversion with your own numbers. Verify.

### GATE
Did you check $\det \neq 0$ before starting? Did $A \cdot A^{-1} = I$?

Miss on either → identify the exact broken step and write it 3×.

---

*BREAK — 15 min. Stand. Walk. No screen.*

---

## MATH 3 — 35 min | Gaussian Elimination + Rank/Nullity

### READ

**Three row operations. Label every single one as you go:**
1. $R_i \leftrightarrow R_j$ — swap rows
2. $R_i \to kR_i$ — scale a row (k ≠ 0)
3. $R_i \to R_i + kR_j$ — add a multiple of another row

If you don't label, you lose marks and lose your place. Label everything.

**Row Echelon Form (REF):**
- Zero rows at the bottom
- Each pivot is strictly right of the pivot above it

**Reduced REF (RREF):** Same + all pivots = 1 + pivot columns otherwise all zero.

**Rank and Nullity:**
$$\text{rank}(A) = \text{number of pivots in echelon form}$$
$$\text{nullity}(A) = n - \text{rank}(A) \quad (n = \text{number of columns})$$
$$\text{rank} + \text{nullity} = n \quad \text{[Rank-Nullity Theorem]}$$

**Solution types — this is what the exam asks:**

| Condition                                  | Solutions                        |
| ------------------------------------------ | -------------------------------- |
| $\text{rank}(A) = \text{rank}([A\|b]) = n$ | Unique                           |
| $\text{rank}(A) = \text{rank}([A\|b]) < n$ | Infinitely many (free variables) |
| $\text{rank}(A) \neq \text{rank}([A\|b])$  | None (inconsistent)              |

Plain language version: if augmenting creates a new pivot that wasn't in $A$ alone → contradiction → no solution.

### CLOSE. WRITE COLD.
- Three operations (names and notation)
- Rank formula, nullity formula, rank-nullity theorem
- Solution type table
- Set up a $[A|b]$ system, row reduce fully, state rank, state nullity, state solution type out loud.

### GATE
After your system: say rank, nullity, and what they imply — out loud, no formulas, plain words.

---

## MATH 4 — 35 min | Complex Numbers: Forms + Polar

### READ

**Three equivalent forms:**
$$z = a + bi \quad \text{[Cartesian]}$$
$$z = r(\cos\theta + i\sin\theta) \quad \text{[Polar]}$$
$$z = re^{i\theta} \quad \text{[Exponential — Euler: } e^{i\theta} = \cos\theta + i\sin\theta\text{]}$$

**Converting Cartesian → Polar:**
$$r = \sqrt{a^2 + b^2} \quad \text{(always positive)}$$
$$\theta = \arctan(b/a) \quad \text{— then CHECK QUADRANT}$$

**Quadrant table — marks live and die here:**

| Quadrant | a, b signs | Correct θ |
|----------|-----------|-----------|
| Q1 | a > 0, b > 0 | arctan(b/a) — calculator is right |
| Q2 | a < 0, b > 0 | π − arctan(\|b/a\|) |
| Q3 | a < 0, b < 0 | −π + arctan(\|b/a\|) — negative result |
| Q4 | a > 0, b < 0 | arctan(b/a) — calculator gives negative, correct |

**Verify after converting:** $r\cos\theta$ must give $a$. $r\sin\theta$ must give $b$. If not, wrong quadrant.

**Multiplication in exponential form:**
$$z_1 \cdot z_2 = r_1r_2 \cdot e^{i(\theta_1+\theta_2)}$$

Multiply moduli, add arguments. Faster than Cartesian for powers.

### CLOSE. WRITE COLD.
- All three forms
- r and θ formulas
- Full quadrant table
- Pick a Q3 number. Convert to polar and exponential. Verify both components.

### GATE
Did your θ land in the correct quadrant? Verified $r\cos\theta = a$ and $r\sin\theta = b$?

---

*BREAK — 15 min.*

---

## MATH 5 — 30 min | Complex Numbers: De Moivre + nth Roots

### READ

**De Moivre:**
$$(re^{i\theta})^n = r^n e^{in\theta}$$
$$\leftrightarrow$$
$$\quad (r(\cos\theta + i\sin\theta))^n = r^n(\cos n\theta + i\sin n\theta)$$

Use for: convert to polar → apply power → convert back.

**Finding n distinct nth roots of $z = re^{i\theta}$:**
$$z_k = r^{1/n} \cdot e^{i\frac{\theta + 2\pi k}{n}}, \quad k = 0, 1, \ldots, n-1$$

Geometry: all roots share modulus $r^{1/n}$, equally spaced at $\frac{2\pi}{n}$ apart on a circle. First root at $\theta/n$.

**Worked example — cube roots of $8i$:**
$$8i = 8e^{i\pi/2}$$
$$r^{1/3} = 2, \quad \text{spacing} = 120°$$
$$k=0: 2e^{i\pi/6} = \sqrt{3}+i \quad k=1: 2e^{i5\pi/6} = -\sqrt{3}+i \quad k=2: 2e^{i3\pi/2} = -2i$$

Draw the Argand diagram. Three points, equally spaced. If not equally spaced, arithmetic is wrong.

### CLOSE. WRITE COLD.
- De Moivre's theorem (both forms)
- nth root formula
- Pick your own number, find cube roots, draw Argand diagram.

### GATE
Are your roots equally spaced on the diagram? Does $k=0$ sit at $\theta/n$?

---

## MATH 6 — 35 min | Linear Transformations

### READ

**Definition — $T: \mathbb{R}^n \to \mathbb{R}^m$ is linear if:**
$$T(\mathbf{u}+\mathbf{v}) = T(\mathbf{u})+T(\mathbf{v}) \quad \text{and} \quad T(c\mathbf{u}) = cT(\mathbf{u})$$

Every linear transformation can be written as $T(\mathbf{x}) = A\mathbf{x}$.

**Rotation matrix (anticlockwise by θ):**
$$R(\theta) = \begin{pmatrix}\cos\theta&-\sin\theta\\\sin\theta&\cos\theta\end{pmatrix}$$

**Reflection matrices:**

| About | Matrix |
|-------|--------|
| x-axis | $\begin{pmatrix}1&0\\0&-1\end{pmatrix}$ |
| y-axis | $\begin{pmatrix}-1&0\\0&1\end{pmatrix}$ |
| y = x | $\begin{pmatrix}0&1\\1&0\end{pmatrix}$ |
| y = −x | $\begin{pmatrix}0&-1\\-1&0\end{pmatrix}$ |

**Determinant check:**
$$\det(\text{rotation}) = +1 \quad \text{[orientation preserved]}$$
$$\det(\text{reflection}) = -1 \quad \text{[orientation reversed]}$$

**Composition — THE order trap:**
$$\text{"Apply S first, then T"} \implies \text{matrix is } TS \quad \text{(rightmost acts first)}$$
$$(T \circ S)(\mathbf{x}) = T(S(\mathbf{x})) = (TS)\mathbf{x}$$

Write **"rightmost acts first"** before every composition problem.

**Image and pre-image:**
- $\text{Im}(T)$ = column space of $A$
- Pre-image of $\mathbf{b}$: solve $A\mathbf{x} = \mathbf{b}$ via Gaussian elimination

**Composition order matters:**
$$TS \neq ST \quad \text{in general — always verify both}$$

### CLOSE. WRITE COLD.
- Linear transformation definition (words + formulas)
- Rotation matrix
- All 4 reflection matrices
- Composition rule (write the sentence before writing the formula)
- Do one composition where $TS \neq ST$. Show both products.

### GATE
Apply $R(90°)$ to $[1, 0]^T$. Should give $[0, 1]^T$. Does it?

---

*BREAK — 15 min.*

---

## MATH 7 — 30 min | Curvilinear Coordinates

### READ

**2D Polar:**
$$x = r\cos\theta, \quad y = r\sin\theta$$
$$r = \sqrt{x^2+y^2}, \quad \theta = \arctan(y/x) \text{ — check quadrant}$$

**Cylindrical:** Same as polar + $z = z$ unchanged.

**Spherical** $(\rho, \theta, \phi)$ — $\rho$: distance from origin, $\theta$: angle from z-axis (0 to π), $\phi$: azimuthal around equator (0 to 2π):
$$x = \rho\sin\theta\cos\phi, \quad y = \rho\sin\theta\sin\phi, \quad z = \rho\cos\theta$$
$$\rho = \sqrt{x^2+y^2+z^2}, \quad \theta = \arccos(z/\rho), \quad \phi = \arctan(y/x)$$

**Why x and y both have sinθ:** You tilt down from the z-axis by θ. The projection onto the xy-plane is $\rho\sin\theta$. Then cosφ and sinφ split that into x and y. z gets cosθ — direct projection onto z-axis.

**Geometric meaning (reconstruct from this if you blank):**
- ρ = how far from origin
- θ = angle down from the north pole
- φ = which way around the equator

### CLOSE. WRITE COLD.
- Polar (both directions)
- Cylindrical (note what changes from polar)
- Spherical (all 6 formulas)
- Say the geometric meaning of ρ, θ, φ aloud.

### GATE
All three coordinate systems written without looking? If you blanked on spherical — wrote it 3×? Move on regardless.

---

## MATH 8 — 30 min | Curvature + Parametric Curves

### READ

**Parametric curve $\mathbf{r}(t) = [x(t), y(t), z(t)]$:**
$$\mathbf{r}'(t) = \text{velocity}, \quad |\mathbf{r}'(t)| = \text{speed}, \quad \mathbf{r}''(t) = \text{acceleration}$$

**Arc length:**
$$L = \int_a^b |\mathbf{r}'(t)|\ dt$$

**Curvature:**
$$\kappa = \frac{|\mathbf{r}'(t) \times \mathbf{r}''(t)|}{|\mathbf{r}'(t)|^3} \quad \text{[3D parametric]}$$
$$\kappa = \frac{|y''|}{(1+y'^2)^{3/2}} \quad \text{[2D: } y = f(x)\text{]}$$

$\kappa = 0$: straight line. $\kappa = 1/R$: circle of radius R. High κ = tight bend.

**Unit tangent:**
$$\hat{T}(t) = \frac{\mathbf{r}'(t)}{|\mathbf{r}'(t)|}$$

**Worked example — parabola $\mathbf{r}(t) = [t, t^2, 0]$:**
$$\mathbf{r}' = [1, 2t, 0], \quad \mathbf{r}'' = [0, 2, 0]$$
$$\mathbf{r}' \times \mathbf{r}'' = [0, 0, 2], \quad |\mathbf{r}' \times \mathbf{r}''| = 2$$
$$\kappa = \frac{2}{(1+4t^2)^{3/2}}$$

At $t=0$: $\kappa = 2$ — max curvature at vertex.

### CLOSE. WRITE COLD.
- Velocity, speed, acceleration formulas
- Arc length
- Both curvature formulas
- Unit tangent
- Redo the parabola example or pick your own parametric curve.

### GATE
Curvature formula correct? Cross product computed correctly?

---

## MATH 9 — 45 min | TIMED GAUNTLET

**No notes. No file. Phone face down. Timer on.**

Write your own question for each topic. ~6 minutes each. Do not check mid-way.

1. **Determinants** — 3×3, cofactor expansion
2. **Inversion** — 2×2, verify with $AA^{-1} = I$
3. **Gaussian** — 3×3 system, row reduce, state rank + nullity + solution type
4. **Complex** — Q2 or Q3 number, all three forms, polar verify
5. **Transformations** — compose two transformations, show $TS \neq ST$
6. **Spherical** — convert a Cartesian point to spherical
7. **Curvature** — find κ for a simple parametric curve

After all 7: open the file and check. **Do not fix anything tonight. Only note what broke.** Errors are information, not failure.

> Write one sentence per error: what was wrong and what the correct step is. That's it. Sleep will process it.

---

## STOP

It's done for tonight. Do not open lecture slides. Do not re-read. The system worked — let it consolidate.

Eat something real.

---
