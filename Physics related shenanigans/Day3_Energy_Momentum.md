# Day 3 — Energy + Momentum

---

## Energy

### Work-kinetic energy theorem
W_net = ΔK = K_f − K_i
Net work done on an object = change in its kinetic energy. Always. No exceptions.

Work done by a constant force
W = F · d · cos(θ)
θ = angle between force and displacement direction.
If force is perpendicular to motion → W = 0.

### Potential energy
Gravitational PE
U_g = mgh
h = height above your chosen reference point (you pick h = 0).

Spring PE
U_s = ½kx²
x = compression or extension from natural length.

### Conservation of mechanical energy
No friction
ΔK + ΔU = 0
K_i + U_i = K_f + U_f
Total mechanical energy stays constant.

With friction
K_i + U_i = K_f + U_f + f_k · d
f_k · d = thermal energy lost to friction (always positive — energy out, not in).

**Decision rule: no friction mentioned → use conservation directly. Friction mentioned → add the f_k·d term to the right side.**

### Finding force from a PE graph
F(x) = −dU/dx
Force = negative slope of the PE curve.
Equilibrium → slope = 0 (flat point on PE curve).
Turning point → K = 0, all energy is PE.

### Power
Average power
P_avg = W / t

Instantaneous power
P = F · v

---

## Momentum

### Linear momentum
p = mv
Direction matters — momentum is a vector.

Newton's second law (real form)
F_net = dp/dt
If F_net = 0 → p is constant → momentum conserved.

### Impulse
J = Δp = F_avg · Δt
A large force for a short time gives the same impulse as a small force for a long time.
J = area under a force-time graph.

### Collision types
Elastic collision
Momentum conserved AND kinetic energy conserved.
p_i = p_f   AND   K_i = K_f

Inelastic collision
Momentum conserved, kinetic energy NOT conserved.
p_i = p_f   BUT   K_f < K_i
Energy lost goes to heat, sound, deformation.

**Momentum is ALWAYS conserved in a collision (if no external forces). KE is only conserved in elastic.**

### Elastic collision shortcuts (target at rest, v₂ᵢ = 0)
Velocity of object 1 after
v₁f = ((m₁ − m₂) / (m₁ + m₂)) · v₁ᵢ

Velocity of object 2 after
v₂f = (2m₁ / (m₁ + m₂)) · v₁ᵢ

Equal masses (m₁ = m₂)
v₁f = 0, v₂f = v₁ᵢ
First object stops dead. Second takes all the speed. Classic pool ball result.

**These shortcuts only apply when the target starts at rest.**
