# MON — Math Exam Day + Physics: First Revision Pass
**Location:** Outside.
**Today:** Math exam. After that, physics revision — not new learning.
**Key rule:** Minimum 2 hours off after the math exam. Non-negotiable.

---

## BEFORE MATH EXAM — Morning activation (max 60 min, stop 30 min before)

This is warm-up, not new input. You are waking up what's already there.

### Write these on paper right now:

**Sign grid (for 3×3 determinants):**
$$\begin{pmatrix}+&-&+\\-&+&-\\+&-&+\end{pmatrix}$$

**Composition rule:**
"Apply S first, then T" → matrix is $TS$ — rightmost acts first.

**Spherical coordinates from geometry (if you blank in the exam):**
- ρ = distance from origin
- θ = angle down from z-axis (north pole direction)
- φ = azimuthal angle around equator
- x and y carry $\sin\theta$ (projection onto xy-plane first), cosφ/sinφ split them
- z carries $\cos\theta$ (direct projection onto z-axis)
$$x = \rho\sin\theta\cos\phi, \quad y = \rho\sin\theta\sin\phi, \quad z = \rho\cos\theta$$

### Cold drill — write each once:
- 2×2 determinant formula
- Middle term in 3×3 expansion: positive or negative?
- 2×2 inversion: what happens to the diagonal, what happens to the off-diagonal?
- Rank-nullity theorem
- Three forms of a complex number
- Q2 complex number: what do you do to arctan(|b/a|)?
- Rotation matrix $R(\theta)$
- Composition: "apply S first then T" → which matrix goes on the right?

For anything blank: check your notes once. Fix. Move on.

### 30 minutes before exam: STOP all input.

---

## IN THE MATH EXAM — First action per question

| Question type | Write this before touching the problem |
|--------------|---------------------------------------|
| 3×3 determinant | Draw sign grid $\begin{pmatrix}+&-&+\\-&+&-\\+&-&+\end{pmatrix}$ |
| Matrix inversion | Check $\det(A) \neq 0$ first. If zero: write "singular — no inverse exists" and stop. |
| Gaussian elimination | Label every row op ($R_2 \to R_2 - 2R_1$). After echelon form: state rank, state nullity, state solution type explicitly. |
| Complex number | Write $r$ and $\theta$ on separate lines. Draw which quadrant your number is in. Verify: $r\cos\theta = a$, $r\sin\theta = b$. |
| Linear transformations | Write "rightmost acts first" in working before multiplying. Det check: $+1$ = rotation, $-1$ = reflection. |
| Spherical | Reconstruct from geometric meaning if blank. |

---

## POST-EXAM BUFFER — Minimum 2 hours off

No Physics. No notes. No reviewing what went wrong.

Eat something real. Walk. Your brain ran a sustained sprint. Forcing new content immediately produces near-zero retention — the prefrontal cortex is already depleted. The physics session tonight works precisely because you gave it space first.

---

## PHYSICS — Afternoon/Evening (start when buffer is done)

This is your first full revision pass through yesterday's new content. You're not re-reading the SUN file — you're testing what stuck and shoring up what didn't.

**Before starting:** note anything from Sunday that felt unstable. Those blocks go first.

---

### PHY-REV 1 — 25 min | Forces cold drill

No reading. Write cold, check after each item.

1. Draw a FBD for a box on a 30° slope — label all forces
2. Write the two gravity components on a slope (formulas and what direction)
3. For that box: $m = 4\ \text{kg}$, $\mu_k = 0.25$. Find $N$, $f_k$, and acceleration.

Check. Fix anything wrong — identify exact step, write correct version 3×.

**Answer check:** $N = 4 \times 9.8 \times \cos30° = 33.95\ \text{N}$. $f_k = 0.25 \times 33.95 = 8.49\ \text{N}$. $F_\text{net} = 4 \times 9.8 \times \sin30° - 8.49 = 19.6 - 8.49 = 11.11\ \text{N}$. $a = 11.11/4 = 2.78\ \text{m/s}^2$.

---

### PHY-REV 2 — 25 min | Energy cold drill

1. Write the master equation from memory (all four terms, what each is)
2. Write the spring work formula (initial minus final — why does it matter?)
3. **Problem:** 5 kg block, spring $k = 300\ \text{N/m}$, compressed 0.15 m. Released on surface with $\mu_k = 0.1$. Find speed after sliding 0.4 m.

Work it fully. Check.

**Answer check:** Spring PE = $\frac{1}{2}(300)(0.15)^2 = 3.375\ \text{J}$. $\Delta E_\text{th} = 0.1 \times 5 \times 9.8 \times 0.4 = 1.96\ \text{J}$. $KE_f = 3.375 - 1.96 = 1.415\ \text{J}$. $v = \sqrt{2 \times 1.415/5} \approx 0.75\ \text{m/s}$.

---

### BREAK — 15 min

---

### PHY-REV 3 — 30 min | Rotation cold drill

1. Write the full linear-rotational parallel table (no notes)
2. Write all 6 $I$ formulas
3. Write the parallel-axis theorem + when it applies
4. **Problem:** Solid sphere, $M = 3\ \text{kg}$, $R = 0.15\ \text{m}$, rolls from rest down a ramp, height $h = 0.8\ \text{m}$. Find speed at bottom.

$I_\text{sphere} = \frac{2}{5}MR^2$. Total KE = $\frac{1}{2}mv^2 + \frac{1}{2}I\omega^2$. Use $v = R\omega$.

**Answer check:** $\frac{1}{2}mv^2 + \frac{1}{2}(\frac{2}{5}mR^2)(\frac{v}{R})^2 = mgh$ → $\frac{1}{2}v^2 + \frac{1}{5}v^2 = gh$ → $\frac{7}{10}v^2 = gh$ → $v = \sqrt{\frac{10gh}{7}} = \sqrt{\frac{10 \times 9.8 \times 0.8}{7}} \approx 3.33\ \text{m/s}$.

---

### PHY-REV 4 — 25 min | SHM cold drill

1. Write the SHM condition ($a = -\omega^2 x$)
2. Derive $\omega = \sqrt{k/m}$ from $F = ma$ (show steps)
3. Derive $\omega = \sqrt{g/L}$ from the torque equation (show steps)
4. **Problem:** Spring $k = 180\ \text{N/m}$, mass $m = 0.8\ \text{kg}$. Find $\omega$, $T$, $f$. If amplitude is 0.05 m, find $v_\text{max}$.

**Answer check:** $\omega = \sqrt{180/0.8} = \sqrt{225} = 15\ \text{rad/s}$. $T = 2\pi/15 \approx 0.42\ \text{s}$. $f \approx 2.39\ \text{Hz}$. $v_\text{max} = \omega x_m = 15 \times 0.05 = 0.75\ \text{m/s}$.

---

### BREAK — 15 min

---

### PHY-REV 5 — 25 min | Waves cold drill

1. Write the wave equation with all symbols labelled
2. Write all 6 derived quantity formulas
3. **Extraction drill — under 2 minutes:** Given $y(x,t) = 0.06\sin(5x - 200t)$ m, extract $y_m$, $k$, $\omega$, $\lambda$, $T$, $f$, $v_\text{wave}$, $u_\text{max}$, $a_\text{max}$.

**Answer check:** $y_m = 0.06$, $k = 5$, $\omega = 200$, $\lambda = 2\pi/5 \approx 1.26\ \text{m}$, $T \approx 0.031\ \text{s}$, $f \approx 31.8\ \text{Hz}$, $v = 40\ \text{m/s}$, $u_\text{max} = 12\ \text{m/s}$, $a_\text{max} = 2400\ \text{m/s}^2$.

---

### PHY-REV 6 — 30 min | Thermodynamics cold drill

1. Write $\Delta U = Q - W$ + sign conventions
2. Write the four-process table (all columns)
3. Write both heat formulas + when each applies
4. Write ideal gas law
5. Write $C_V$, $C_p$, $\gamma$ for monoatomic and diatomic
6. **Problem:** 2 mol monoatomic ideal gas, isothermal expansion, does 400 J of work. Find Q and $\Delta U$.

**Answer check:** Isothermal → $\Delta U = 0$. Therefore $Q = W = 400\ \text{J}$.

---

### PHY-REV 7 — 25 min | Fluids cold drill

1. Write Archimedes' principle formula
2. Write Bernoulli's equation
3. Write continuity equation
4. Write Pascal's trap in one sentence (where to equate pressures and why)
5. **Problem:** Water (density $\rho = 1000\ \text{kg/m}^3$) flows through a pipe. At point 1: $A_1 = 0.02\ \text{m}^2$, $v_1 = 2\ \text{m/s}$, $P_1 = 150000\ \text{Pa}$, $h_1 = 0\ \text{m}$. At point 2: $A_2 = 0.01\ \text{m}^2$, $h_2 = 0\ \text{m}$. Find $v_2$ and $P_2$.

**Answer check:** Continuity: $v_2 = A_1v_1/A_2 = 0.02 \times 2 / 0.01 = 4\ \text{m/s}$. Bernoulli: $P_2 = P_1 + \frac{1}{2}\rho(v_1^2 - v_2^2) = 150000 + \frac{1}{2}(1000)(4-16) = 150000 - 6000 = 144000\ \text{Pa}$.

---

### FINAL WRITE — 20 min | Compression sheet

On one piece of paper, write from memory in one line each:

- SHM condition
- $\omega$ for spring (with derivation marker: from $F=ma$)
- $\omega$ for pendulum (with derivation marker: from torque)
- Master energy equation
- Spring work trap (initial minus final)
- $\Delta E_\text{th}$ formula
- Wave equation
- $v_\text{wave}$ formula, $u_\text{max}$ formula (both — they're different)
- Wave speed on string + unit trap reminder
- $\Delta U = Q - W$
- Isothermal: what's zero
- Adiabatic: what's zero
- $C_V$ for monoatomic and diatomic
- Archimedes formula
- Bernoulli equation
- Continuity equation

Anything blank = note it. Tomorrow morning patches it.

---

## STOP

Physics exam is tomorrow. Consolidation happens during sleep — not during extra study hours.

Eat. Sleep.

---
