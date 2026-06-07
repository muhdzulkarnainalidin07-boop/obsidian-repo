# SUN — Math Seal + Physics: First Contact
**Location:** Outside.
**Exam countdown:** Math tomorrow. Physics in 2 days.
**Today's split:** ~45 min math patch, then all remaining time is Physics.

---

## THE SYSTEM — MODIFIED FOR ZERO EXPOSURE

Because you have no prior Physics exposure (except kinematics), the loop changes:

```
READ slowly (understand the mechanism, not just the formula)
→ CLOSE
→ WRITE COLD (reproduce what you understood — formulas + the logic behind them)
→ REOPEN + CHECK
→ FIX: write wrong things 3×, say them aloud, write once more
→ MOVE ON regardless
```

**Do not try cold before reading for any Physics block today.** That loop is for revision. You're learning, not recalling. Read first, every time.

**Stuck for more than 4 minutes:** note it, move on. There is no time to spiral.

---

## SCHEDULE OVERVIEW

| Block      | Topic                                  | Approx time  |
| ---------- | -------------------------------------- | ------------ |
| MATH PATCH | Fix one gauntlet error from last night | 45 min       |
| PHY 1      | Forces & Newton's Laws                 | 40 min       |
| —          | Break                                  | 15 min       |
| PHY 2      | Conservation of Energy                 | 45 min       |
| —          | Break                                  | 15 min       |
| PHY 3      | Rotational Motion                      | 45 min       |
| —          | Break                                  | 15 min       |
| PHY 4      | SHM                                    | 40 min       |
| PHY 5      | Transverse Waves                       | 40 min       |
| —          | Break                                  | 15 min       |
| PHY 6      | Thermodynamics                         | 50 min       |
| PHY 7      | Fluids                                 | 40 min       |
|            | Total                                  | 6hrs 45 mins |
|            |                                        |              |

> Fluids is last because it's the most conceptually complex and least buildable from zero. If you run out of time, Fluids is the one to cut — but try to get through at least the Archimedes + Pascal section.

---

## MATH PATCH — 45 min

Pull your gauntlet error notes from last night.

Find **one specific broken step**. Not a whole topic — one step. Examples:
- "Middle term in 3×3 expansion: I kept making it positive"
- "Complex Q3: I put θ in Q2 instead"
- "Composition: I multiplied left-to-right instead of right-to-left"

**The patch:**
1. Write what was wrong
2. Write the correct version 5×
3. Work one cold example using it
4. Write one sentence that captures the rule

If you have two errors from last night, fix both. If you have more than two — pick the two that are most likely to appear in the exam (determinants and complex numbers appear almost every year in this type of course).

### GATE
Can you do the specific broken thing cold, no hesitation? Yes → math is sealed. Move on.

---

## PHY 1 — 40 min | Forces & Newton's Laws

### WHY THIS FIRST

Everything in physics uses forces. Rotation, energy, fluids, SHM — all of them reduce to force analysis at some point. If Newton's laws are clear, every other topic becomes an extension. If they're not, every other topic feels like isolated memorisation.

### READ — take your time here

**The foundation:**

A force is a push or pull. Forces have direction. Newton's second law says the *net* force (sum of all forces) on an object equals mass times acceleration:

$$F_\text{net} = ma$$

**The mandatory first step for any force problem: draw the Free Body Diagram (FBD).**

A FBD is a diagram showing only the object and all the forces acting on it as arrows. Nothing else. No walls, no ground, no other objects — just the object and its force arrows with labels.

Your lecturer explicitly stressed this. It's how you avoid missing forces and how you identify the correct direction of each one.

**Common forces you'll see:**
- Weight: $W = mg$ downward (always)
- Normal force: perpendicular to the surface the object sits on (always away from surface)
- Tension: along a rope or cord, away from the object
- Friction: opposing the direction of motion (or tendency of motion)
- Applied force: whatever the problem gives you

**Worked scenario 1 — sphere suspended by cord at 60° to vertical, horizontal force $F$ pulling it:**

Draw the FBD: three forces on the sphere — tension $T$ along cord (up and left), weight $mg$ downward, horizontal force $F$ to the right.

The cord makes 60° with the vertical. Resolve tension into components:
- Vertical: $T\cos 60°$ upward
- Horizontal: $T\sin 60°$ toward left (opposing $F$)

Write equilibrium equations (acceleration = 0 since it's hanging still):
$$\text{Vertical: } T\cos 60° = mg \implies T = \frac{mg}{\cos 60°}$$
$$\text{Horizontal: } T\sin 60° = F \implies F = T\sin 60°$$

**Worked scenario 2 — box on inclined plane (angle θ):**

This is the classic setup. The trick: align your axes with the slope, not horizontal/vertical. This way, the acceleration (along the slope) is already along one axis.

Gravity $mg$ acts straight down. You need to split it into two components relative to the slope:
- **Along the slope (down-slope):** $mg\sin\theta$
- **Perpendicular to slope (into the surface):** $mg\cos\theta$

Normal force $N = mg\cos\theta$ (balances the perpendicular gravity component).

Friction force (opposing motion): $f_k = \mu_k N = \mu_k mg\cos\theta$

Net force along slope: $F_\text{net} = mg\sin\theta - f_k = mg\sin\theta - \mu_k mg\cos\theta$

Acceleration: $a = g\sin\theta - \mu_k g\cos\theta = g(\sin\theta - \mu_k\cos\theta)$

**Specific numbers — work this fully:**

Box: $m = 5\ \text{kg}$, $\theta = 30°$, $\mu_k = 0.2$, $g = 9.8\ \text{m/s}^2$.

$$N = 5 \times 9.8 \times \cos 30° = 49 \times 0.866 = 42.43\ \text{N}$$
$$f_k = 0.2 \times 42.43 = 8.49\ \text{N}$$
$$F_\text{net} = 5 \times 9.8 \times \sin 30° - 8.49 = 49 \times 0.5 - 8.49 = 24.5 - 8.49 = 16.01\ \text{N}$$
$$a = 16.01 / 5 = 3.20\ \text{m/s}^2$$

### CLOSE. WRITE COLD.
1. FBD rule (in your own words — what it is and why it's the first step)
2. The two gravity components on a slope (formulas with what they represent)
3. Normal force on a slope
4. Friction force formula
5. Redo the inclined plane worked example with your own numbers (different mass and angle)

### GATE
For a box on a slope — which direction does the normal force point? Which component of gravity causes acceleration? Write both. No notes.

---

## BREAK — 15 min

---

## PHY 2 — 45 min | Conservation of Energy

### WHY THIS SECOND

Energy conservation is the most powerful tool in mechanics. It bypasses tracking every force and every acceleration step — instead, you just account for where energy starts and where it ends. Once you have this, a huge number of problems become one-equation setups.

### READ — understand the mechanism first

**What is energy?**

Energy is the capacity to do work. It can change form, but the total never disappears.

**Kinetic energy (KE):** Energy an object has because it's moving.
$$KE = \frac{1}{2}mv^2$$

**Gravitational PE:** Energy stored in position above a reference height.
$$U_g = mgh \quad \text{(set } h = 0 \text{ wherever is convenient — you choose)}$$

**Spring PE (elastic):** Energy stored in a compressed or stretched spring.
$$U_s = \frac{1}{2}kx^2 \quad \text{(x = displacement from natural/rest length)}$$

**The master equation — write this before touching any energy problem:**
$$\Delta K + \Delta U_g + \Delta U_s + \Delta E_\text{th} = W_\text{ext}$$

What each term means:
- $\Delta K = K_f - K_i$ — did the object speed up or slow down?
- $\Delta U_g = mgh_f - mgh_i$ — did it go higher or lower?
- $\Delta U_s = \frac{1}{2}kx_f^2 - \frac{1}{2}kx_i^2$ — did the spring gain or lose stored energy?
- $\Delta E_\text{th} = f_k d$ — friction generates heat; this is always positive, always added
- $W_\text{ext}$ = work done by any external agent (e.g. a motor, a person pushing); zero if nothing external acts

**Most problems set $W_\text{ext} = 0$** (nothing external doing work). The equation then becomes:

$$\Delta K + \Delta U_g + \Delta U_s + \Delta E_\text{th} = 0$$

Meaning: all the changes in energy sum to zero — energy just moves between forms.

**The spring work trap — your lecturer flagged this:**

The *work done by a spring* is:
$$W_s = \frac{1}{2}kx_i^2 - \frac{1}{2}kx_f^2 \quad \text{(initial minus final)}$$

This is the opposite sign from $\Delta U_s$. That's because work done by the spring = decrease in spring PE. If you use the master equation above, you don't need to think about this separately — but if the problem asks specifically for "work done by the spring," use this formula.

**Work done by a constant force:**
$$W = Fd\cos\theta \quad \text{(θ = angle between force and displacement)}$$

- Force in direction of motion: $\theta = 0°$, $W = Fd$ (positive)
- Force opposing motion: $\theta = 180°$, $W = -Fd$ (negative)
- Force perpendicular to motion: $\theta = 90°$, $W = 0$

**Work-KE theorem** (when you only care about speed change, not PE):
$$W_\text{net} = \Delta K$$

**Worked example:**

A 2 kg block compresses a spring ($k = 500\ \text{N/m}$) by $x = 0.3\ \text{m}$, then releases on a frictionless surface. Find speed when spring returns to natural length.

Set up master equation. No height change ($\Delta U_g = 0$). No friction ($\Delta E_\text{th} = 0$). No external work ($W_\text{ext} = 0$).

$$\Delta K + \Delta U_s = 0$$
$$\left(\frac{1}{2}mv_f^2 - 0\right) + \left(0 - \frac{1}{2}kx^2\right) = 0$$
$$\frac{1}{2}(2)v_f^2 = \frac{1}{2}(500)(0.3)^2 = 22.5\ \text{J}$$
$$v_f = \sqrt{\frac{22.5}{1}} = \sqrt{22.5} \approx 4.74\ \text{m/s}$$

**Worked example with friction:**

3 kg block, spring $k = 400\ \text{N/m}$, compressed $x_i = 0.2\ \text{m}$, released. Surface has $\mu_k = 0.15$. Find speed after sliding $d = 0.5\ \text{m}$.

$$\Delta E_\text{th} = f_k d = \mu_k mg \cdot d = 0.15 \times 3 \times 9.8 \times 0.5 = 2.205\ \text{J}$$

Master equation:
$$\Delta K + \Delta U_s + \Delta E_\text{th} = 0$$
$$\frac{1}{2}(3)v_f^2 - \frac{1}{2}(400)(0.2)^2 + 2.205 = 0$$
$$1.5v_f^2 = 8 - 2.205 = 5.795$$
$$v_f = \sqrt{5.795/1.5} \approx 1.96\ \text{m/s}$$

### CLOSE. WRITE COLD.
1. All three energy formulas ($KE$, $U_g$, $U_s$)
2. Master equation (all terms, what each means in one clause)
3. $\Delta E_\text{th}$ formula — when is it nonzero?
4. Spring work formula (initial minus final)
5. Redo the friction example with your own numbers.

### GATE
Write the master equation. Identify which terms are zero in: (a) frictionless spring launch, (b) block sliding down a ramp with friction, no spring. No notes.

---

## BREAK — 15 min

---

## PHY 3 — 45 min | Rotational Motion

### WHY THIS APPROACH

Rotational motion has a direct parallel to everything you already know from linear mechanics. Every formula has an exact equivalent. Once you see the pattern, you're not learning new physics — you're just renaming variables.

### READ

**The parallel — this is the whole topic:**

| Linear concept | Linear formula | → | Rotational concept | Rotational formula |
|---------------|----------------|---|-------------------|-------------------|
| Displacement | $x$ (m) | | Angular displacement | $\theta$ (rad) |
| Velocity | $v$ | | Angular velocity | $\omega$ |
| Acceleration | $a$ | | Angular acceleration | $\alpha$ |
| Force | $F$ | | Torque | $\tau$ |
| Mass (inertia) | $m$ | | Moment of inertia | $I$ |
| Newton's 2nd | $F = ma$ | | Rotational 2nd | $\tau = I\alpha$ |
| Momentum | $p = mv$ | | Angular momentum | $L = I\omega$ |
| Kinetic energy | $\frac{1}{2}mv^2$ | | Rotational KE | $\frac{1}{2}I\omega^2$ |

Connecting both: $v = r\omega$ (tangential speed at radius $r$ from a spinning axis).

**Moment of inertia $I$** — the rotational equivalent of mass. It measures resistance to rotation and depends on how mass is distributed relative to the axis.

Exam-standard shapes:
$$I_\text{point particle} = mr^2$$
$$I_\text{solid disk or cylinder} = \frac{1}{2}MR^2$$
$$I_\text{hoop or ring} = MR^2$$
$$I_\text{solid sphere} = \frac{2}{5}MR^2$$
$$I_\text{rod about centre} = \frac{1}{12}ML^2$$
$$I_\text{rod about end} = \frac{1}{3}ML^2$$

**Parallel-Axis Theorem — the trap flagged by your lecturer:**

These $I$ formulas assume the axis passes through the centre of mass. If the rotation axis is elsewhere:
$$I = I_\text{cm} + Md^2 \quad (d = \text{distance from CM to new axis})$$

Miss this when it applies = wrong answer for the whole question.

**Torque:**
$$\tau = rF\sin\theta$$

$r$ = distance from pivot to where force is applied. $\theta$ = angle **between** the position vector $\vec{r}$ and the force vector $\vec{F}$. Not from horizontal. Not from vertical. Between those two vectors specifically.

- Force perpendicular to lever arm: $\theta = 90°$, maximum torque
- Force pointing toward or away from pivot: $\theta = 0°$ or $180°$, zero torque

**Rolling objects — explicitly repeated by your lecturer:**

An object rolling without slipping has both translational and rotational KE:
$$K_\text{total} = \frac{1}{2}mv_\text{cm}^2 + \frac{1}{2}I\omega^2$$

For rolling: $v_\text{cm} = R\omega$, so you can convert between $v$ and $\omega$.

**Worked example — rolling cylinder down ramp:**

Solid cylinder, $M = 2\ \text{kg}$, $R = 0.1\ \text{m}$, descends height $h = 0.5\ \text{m}$ from rest. No friction loss (rolling without slipping). Find speed at bottom.

Energy conservation: $\Delta K + \Delta U_g = 0$
$$\frac{1}{2}mv^2 + \frac{1}{2}I\omega^2 - mgh = 0$$

$I = \frac{1}{2}MR^2$, $\omega = v/R$:
$$\frac{1}{2}mv^2 + \frac{1}{2}\left(\frac{1}{2}MR^2\right)\left(\frac{v}{R}\right)^2 = mgh$$
$$\frac{1}{2}mv^2 + \frac{1}{4}mv^2 = mgh$$
$$\frac{3}{4}v^2 = gh \implies v = \sqrt{\frac{4gh}{3}} = \sqrt{\frac{4 \times 9.8 \times 0.5}{3}} \approx 2.56\ \text{m/s}$$

### CLOSE. WRITE COLD.
1. Full parallel table (both columns, all 8 rows)
2. All 6 $I$ formulas
3. Parallel-axis theorem (formula + when to use it)
4. Torque formula + what θ is
5. Rolling KE formula
6. Redo the rolling cylinder example with your own numbers.

### GATE
What is $I$ for a solid disk? What's the difference between $I_\text{disk}$ and $I_\text{hoop}$, and why (one sentence, physical reason)?

---

## BREAK — 15 min

---

## PHY 4 — 40 min | Simple Harmonic Motion

### EXAM SCOPE (official — from your screenshots)

Your exam covers **only two SHM systems**: horizontal spring-block and simple pendulum. Damped SHM and torsion pendulums are explicitly excluded. Don't spend time on what's not tested.

### READ

**What is SHM?**

SHM describes any system where the restoring force is proportional to displacement and always directed back toward equilibrium. Pull it left → force pushes right. Push it right → force pushes left.

The mathematical signature:
$$a = -\omega^2 x$$

If you see this relationship in any problem, it's SHM. The $-$ sign is critical — acceleration always opposes displacement.

**System 1: Horizontal spring-block**

A block of mass $m$ on a frictionless surface, attached to a spring with constant $k$.

Newton's second law: the only horizontal force is the spring:
$$F_\text{net} = ma = -kx$$
$$\therefore a = -\frac{k}{m}x$$

Compare to $a = -\omega^2 x$:
$$\omega = \sqrt{\frac{k}{m}}$$

Memorise this by deriving it — don't just write the answer.

**System 2: Simple pendulum**

A point mass on a massless string, length $L$, swinging through small angles.

The restoring torque is $\tau = -mgL\sin\theta$. For small angles, $\sin\theta \approx \theta$, so:
$$I\alpha = -mgL\theta$$

For a point mass on a string: $I = mL^2$:
$$mL^2 \alpha = -mgL\theta \implies \alpha = -\frac{g}{L}\theta = -\omega^2\theta$$
$$\omega = \sqrt{\frac{g}{L}}$$

Period (same structure for both):
$$T = \frac{2\pi}{\omega}$$

**Equations of motion:**
$$x(t) = x_m\cos(\omega t + \phi) \quad \text{[displacement]}$$
$$v(t) = -\omega x_m\sin(\omega t + \phi) \quad \text{[velocity — derivative of x]}$$
$$a(t) = -\omega^2 x_m\cos(\omega t + \phi) = -\omega^2 x(t) \quad \text{[acceleration — derivative of v]}$$

$x_m$ = amplitude (max displacement, always positive). $\phi$ = phase constant (from initial conditions).

**The exam trap:** Given frequency $f$ in Hz, but formula needs $\omega$ (rad/s). Convert:
$$\omega = 2\pi f$$

Always convert before using any formula.

**Worked example:**

Spring with $k = 200\ \text{N/m}$, block $m = 0.5\ \text{kg}$, released from $x = 0.1\ \text{m}$ at $t = 0$.

$$\omega = \sqrt{\frac{200}{0.5}} = \sqrt{400} = 20\ \text{rad/s}$$
$$T = \frac{2\pi}{20} \approx 0.314\ \text{s}$$
$$x(t) = 0.1\cos(20t) \quad \text{(φ = 0 because released from max displacement at t = 0)}$$
$$v_\text{max} = \omega x_m = 20 \times 0.1 = 2\ \text{m/s} \quad \text{(at equilibrium, x = 0)}$$

### CLOSE. WRITE COLD.
1. $a = -\omega^2 x$ and what it means
2. Derive $\omega = \sqrt{k/m}$ from $F = ma$ (show the derivation steps)
3. Derive $\omega = \sqrt{g/L}$ from the torque equation (show the steps)
4. $T = 2\pi/\omega$
5. All three equations of motion
6. Redo the worked example with your own spring and mass.

### GATE
Derive $\omega = \sqrt{k/m}$ from Newton's second law cold. Show every step. No notes.

---

## PHY 5 — 40 min | Transverse Waves

### READ

**What is a transverse wave?**

A wave transfers energy through a medium. In a transverse wave, the medium oscillates perpendicular to the wave's direction of travel. Think of a string: the wave moves along the string, but each piece of string moves up and down.

**The wave equation:**
$$y(x,t) = y_m\sin(kx - \omega t)$$

What each symbol means — label all of these before doing anything:
- $y_m$ = amplitude: maximum displacement from equilibrium (always positive, in metres)
- $k$ = wave number (rad/m) — **not** spring constant
- $\omega$ = angular frequency (rad/s)
- The argument $(kx - \omega t)$ = phase
- **Minus sign** in the phase: wave travels in the $+x$ direction. If it were $+\omega t$, it would travel in $-x$.

**All derived quantities — these are what exam questions ask for:**
$$\lambda = \frac{2\pi}{k} \quad \text{(wavelength — spatial period)}$$
$$T = \frac{2\pi}{\omega} \quad \text{(period — time for one full cycle)}$$
$$f = \frac{1}{T} = \frac{\omega}{2\pi} \quad \text{(frequency)}$$
$$v_\text{wave} = f\lambda = \frac{\omega}{k} \quad \text{(speed of the wave pattern through space)}$$
$$u_\text{max} = \omega y_m \quad \text{(max transverse speed of a particle in the medium)}$$
$$a_\text{max} = \omega^2 y_m \quad \text{(max transverse acceleration of a particle)}$$

**Critical distinction — this is a guaranteed exam trap:**

$v_\text{wave}$ and $u_\text{max}$ are completely different things.
- $v_\text{wave} = \omega/k$: how fast the pattern moves along the x-axis
- $u_\text{max} = \omega y_m$: how fast a single particle of the medium moves up and down (perpendicular to wave direction)

To see why: differentiate $y(x,t)$ with respect to $t$:
$$\frac{\partial y}{\partial t} = -\omega y_m\cos(kx - \omega t)$$

Maximum when cosine = 1: $u_\text{max} = \omega y_m$.

**Wave speed on a string:**
$$v = \sqrt{\frac{\tau}{\mu}}, \quad \mu = \frac{m}{L} \quad \text{(linear mass density, kg/m)}$$

$\tau$ = string tension (N). **Unit trap:** if $\mu$ given in g/m, convert to kg/m first. Getting this wrong gives a speed off by a factor of ~32. Always check units before computing.

**Standing waves — the 3-loop scenario flagged in your exam materials:**

A string of length $L$ vibrating in $n$ loops:
$$n \text{ loops} = \frac{n}{2}\lambda \quad \text{(each loop is half a wavelength)}$$

For $n = 3$, $L = 5\ \text{m}$:
$$\frac{3}{2}\lambda = 5 \implies \lambda = \frac{10}{3}\ \text{m}$$

Then: find $\mu = m/L$ from the string's mass and length, find $v = \sqrt{\tau/\mu}$, then $f = v/\lambda$, then $\omega = 2\pi f$, $k = 2\pi/\lambda$.

**The extraction drill — this is the exact question type:**

Given $y(x,t) = 0.04\sin(2.5x - 120t)$ m:
- $y_m = 0.04\ \text{m}$
- $k = 2.5 \to \lambda = 2\pi/2.5 \approx 2.51\ \text{m}$
- $\omega = 120 \to T = 2\pi/120 \approx 0.052\ \text{s}$, $f \approx 19.1\ \text{Hz}$
- $v_\text{wave} = 120/2.5 = 48\ \text{m/s}$
- $u_\text{max} = 120 \times 0.04 = 4.8\ \text{m/s}$
- $a_\text{max} = 120^2 \times 0.04 = 576\ \text{m/s}^2$

### CLOSE. WRITE COLD.
1. Wave equation with every symbol labelled
2. All 6 derived quantities (formulas and what they represent)
3. One sentence explaining why $v_\text{wave} \neq u_\text{max}$
4. Wave speed on string + the unit trap
5. Make up your own wave equation and do the full extraction drill.

### GATE
Given $y(x,t) = 0.02\sin(3x - 90t)$ m — extract all quantities cold. Under 2 minutes.

---

## BREAK — 15 min

---

## PHY 6 — 50 min | Thermodynamics + Kinetic Theory

### READ — this is the most formula-dense section, go slowly

**First law of thermodynamics:**
$$\Delta U = Q - W$$

This says: the change in internal energy of a system equals heat added to the system minus work done by the system.

**Sign conventions — get these wrong and every answer is wrong:**

| Symbol | Positive when | Negative when |
|--------|--------------|--------------|
| $Q$ | Heat flows **into** system | Heat flows **out** |
| $W$ | System **expands** (does work on surroundings) | System is **compressed** |

**What is internal energy $U$?** The total random kinetic energy of all molecules. Depends only on temperature — not on pressure or volume directly.

**The four special processes — the exam asks: given a process type, what's zero, what does the first law simplify to?**

| Process | Fixed quantity | What's zero | Simplified 1st law |
|---------|---------------|------------|-------------------|
| Isothermal | Temperature (T) | $\Delta U = 0$ | $Q = W$ |
| Adiabatic | No heat exchange | $Q = 0$ | $\Delta U = -W$ |
| Isochoric (constant volume) | Volume (V) | $W = 0$ | $\Delta U = Q$ |
| Isobaric (constant pressure) | Pressure (P) | nothing | $\Delta U = Q - p\Delta V$ |

**Work by a gas:**
$$W_\text{isobaric} = p\Delta V$$
$$W_\text{isothermal} = nRT\ln\frac{V_f}{V_i}$$
$$W_\text{isochoric} = 0$$

**Kelvin rule — underline this:**
$$T(\text{K}) = T(°\text{C}) + 273.15$$

Every gas law calculation uses Kelvin. Celsius gives wrong answers. Convert first, every time.

**Two heat formulas:**
$$Q = mc\Delta T \quad \text{(temperature is changing)}$$
$$Q = Lm \quad \text{(temperature is NOT changing — phase transition)}$$

Why temperature flatlines during a phase change: all energy input goes into breaking molecular bonds, not increasing kinetic energy. Temperature rises again only after the phase change completes.

**Ideal gas law:**
$$pV = nRT \quad (R = 8.314\ \text{J/mol·K},\ n = \text{moles})$$

**Internal energy shortcut — use this on PV diagram problems to bypass integration:**
$$\Delta E_\text{int} = \frac{3}{2}(P_fV_f - P_iV_i) \quad \text{(monoatomic ideal gas)}$$

**Kinetic theory — internal energy:**
$$E_\text{int} = \frac{f}{2}nRT$$

Degrees of freedom $f$: monoatomic gas (He, Ar) → $f = 3$. Diatomic gas (N₂, O₂) → $f = 5$.

**Specific heats and $\gamma$:**

| Gas type | $C_V$ | $C_p = C_V + R$ | $\gamma = C_p/C_V$ |
|----------|-------|----------------|-------------------|
| Monoatomic | $\frac{3}{2}R$ | $\frac{5}{2}R$ | $\frac{5}{3} \approx 1.67$ |
| Diatomic | $\frac{5}{2}R$ | $\frac{7}{2}R$ | $\frac{7}{5} = 1.4$ |

Why $C_p > C_V$ always: at constant pressure, the expanding gas does work on its surroundings. That work energy must also come from the heat input, on top of what's needed to raise temperature. At constant volume, all heat goes straight into $\Delta U$.

**RMS speed:**
$$v_\text{rms} = \sqrt{\frac{3RT}{M}} \quad (M = \text{molar mass in kg/mol})$$

Lighter gas → smaller $M$ → higher $v_\text{rms}$ at same temperature.

**Adiabatic relations:**
$$pV^\gamma = \text{const} \quad \text{(use when given } p \text{ and } V\text{)}$$
$$TV^{\gamma-1} = \text{const} \quad \text{(use when given } T \text{ and } V\text{)}$$

### CLOSE. WRITE COLD.
1. $\Delta U = Q - W$ + sign convention table
2. Four-process table (all four columns)
3. Work formula for each process
4. Both heat formulas + when each applies (one sentence per)
5. Ideal gas law
6. Internal energy shortcut
7. $C_V$, $C_p$, $\gamma$ table for both gas types
8. $v_\text{rms}$ formula
9. Adiabatic relations

### GATE
Write the four-process table from memory. Then explain in one sentence why temperature flatlines during a phase change. No formulas in the sentence.

---

## PHY 7 — 40 min | Fluids

### READ — two core principles and two specific traps

**Archimedes' Principle:**

Any object submerged in (or floating on) a fluid experiences an upward buoyant force equal to the weight of fluid it displaces.

$$F_b = \rho_\text{fluid} V_\text{displaced} g$$

$\rho_\text{fluid}$ = density of the fluid (kg/m³). $V_\text{displaced}$ = volume of fluid displaced by the object (m³).

How to use it: write Newton's 2nd law for the object, including $F_b$ as an upward force.

Example — object floating: $F_b = mg$ (buoyancy exactly equals weight).
Example — object sinking at constant velocity: $F_b + F_\text{drag} = mg$.

**Pascal's Principle:**

Pressure applied to a confined fluid is transmitted equally throughout. This is how hydraulic systems work.

$$P = \frac{F}{A}$$

For a hydraulic press: $P_1 = P_2 \implies \frac{F_1}{A_1} = \frac{F_2}{A_2}$

**The hydraulic trap — specifically flagged in your exam materials:**

In the spring problem from the exam screenshots: a weight sits on small piston (area $A_1$), a spring sits on large piston (area $A_2 = 18A_1$). You want to know how much sand to pour in to compress the spring by 5 cm.

You **cannot** set $P_1 = P_2$ at the tops of the two pistons if they are at different heights. Fluid pressure increases with depth: $P = \rho g h$.

You **must** set pressures equal at the **same horizontal reference level** (typically the bottom, where the two sides connect).

At that reference level, the pressure from the left column (under the sand) = pressure from the right column (under the spring):
$$\frac{mg_\text{sand}}{A_1} + \rho g h_\text{left} = \frac{F_\text{spring}}{A_2} + \rho g h_\text{right}$$

If the fluid levels are equal: $\rho g h$ cancels, and:
$$\frac{mg}{A_1} = \frac{kx}{A_2}$$
$$m = \frac{kx A_1}{g A_2} = \frac{3.0\times10^4 \times 0.05 \times A_1}{9.8 \times 18A_1} = \frac{1500}{176.4} \approx 8.5\ \text{kg}$$

**Bernoulli's Equation:**

For a fluid flowing along a streamline (derived from the Work-KE theorem):
$$P + \frac{1}{2}\rho v^2 + \rho g h = \text{constant}$$

Between two points:
$$P_1 + \frac{1}{2}\rho v_1^2 + \rho g h_1 = P_2 + \frac{1}{2}\rho v_2^2 + \rho g h_2$$

Intuition: where fluid speeds up, pressure drops. This is why airplane wings generate lift and why a shower curtain blows inward.

**Equation of Continuity:**
$$A_1 v_1 = A_2 v_2$$

Narrower pipe → faster flow. Wider pipe → slower flow. Volume flow rate is constant.

### CLOSE. WRITE COLD.
1. Archimedes formula + how to use it in Newton's 2nd law
2. Pascal's principle (the pressure equality formula)
3. Pascal's trap — one sentence: where do you set pressures equal, and what extra term appears?
4. Bernoulli's equation
5. Continuity equation

### GATE
In the Pascal's hydraulic problem: why can't you set $P_1 = P_2$ at the top of each piston? One sentence. No notes.

---

## STOP

Seven topics loaded. Kinematics you already had. That's the full exam covered.

Tonight: eat, sleep early. Tomorrow is the math exam and then a physics revision pass. Don't try to cram more tonight — your brain needs to consolidate what you just loaded.

---
