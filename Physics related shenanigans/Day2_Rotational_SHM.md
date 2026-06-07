# Day 2 — Rotational Motion + Simple Harmonic Motion

---

## Rotational Motion

### The linear-angular parallel
Everything in linear motion has a rotational twin. If you know the linear version, you know the rotational version.

| Linear | Angular |
|--------|---------|
| position x | angle θ |
| velocity v | angular velocity ω |
| acceleration a | angular acceleration α |
| mass m | rotational inertia I |
| force F | torque τ |
| F = ma | τ = Iα |
| K = ½mv² | K = ½Iω² |

### Rotation ↔ linear conversions
Arc length
s = rθ

Tangential speed
v = rω

Tangential acceleration
a_t = rα

Centripetal acceleration
a_c = v²/r = ω²r

### Rotational inertia (I) — Rotational I
How hard something is to spin. Depends on how mass is distributed, not just total mass.

Discrete masses
I = Σ mᵢrᵢ²
Add up each mass × its distance from axis squared.

Parallel axis theorem
I = I_com + Mh²
h = distance from centre of mass to the new axis.
Use this when the axis is not through the centre of mass.

**Mass far from axis → higher I → harder to spin. Figure skater pulls arms in → smaller I → spins faster.**

### Torque — Rotational II
Torque
τ = rF sin(θ)
r = moment arm (distance from pivot to where force is applied)
θ = angle between r and F

Newton's second law for rotation
τ_net = Iα

Rotational kinetic energy
K = ½Iω²

**Exam trap: if an object is rolling, it has BOTH translational KE (½mv²) and rotational KE (½Iω²). Total K = ½mv² + ½Iω².**

---

## Simple Harmonic Motion

### What qualifies as SHM
Any system where restoring force is proportional to displacement and always pulls back toward centre.
F = −kx

### The three core equations
Displacement
x(t) = x_m cos(ωt + φ)
x_m = amplitude, φ = phase constant

Velocity
v(t) = −ωx_m sin(ωt + φ)
Max speed = ωx_m  (occurs at equilibrium, x = 0)

Acceleration
a(t) = −ω²x_m cos(ωt + φ)
Max acceleration = ω²x_m  (occurs at max displacement)
Also written as: a = −ω²x

Angular frequency
ω = √(k/m) = 2πf

**v, a are derivatives of x. If you forget a formula, differentiate the one above it.**

### Energy in SHM
Potential energy
U = ½kx²

Kinetic energy
K = ½mv²

Total mechanical energy
E = ½kx_m²   ← constant, depends only on amplitude

At max displacement (x = x_m): all PE, zero KE.
At equilibrium (x = 0): all KE, zero PE.
Total never changes (no friction).

### Pendulum periods
Simple pendulum (small angles only)
T = 2π√(L/g)
L = length to pivot

Physical pendulum
T = 2π√(I/mgL)
I = rotational inertia, L = distance from pivot to centre of mass

**Exam note: period does NOT depend on mass for a simple pendulum. Only L and g matter.**
