# Day 4 — Thermodynamics + Kinetic Theory

---

## Thermodynamics

### First law
ΔE_int = Q − W
Q = heat absorbed BY the gas (positive in, negative out)
W = work done BY the gas (positive out, negative in)
ΔE_int = change in internal energy

Energy is never created or destroyed — only moved as heat or work.

### Special process cases — make a table, know all four
| Process | Condition | Simplification |
|---------|-----------|----------------|
| Adiabatic | Q = 0 | ΔE_int = −W  (gas cools when it expands) |
| Isochoric | W = 0 | ΔE_int = Q  (all heat → internal energy) |
| Isobaric | p = constant | W = pΔV |
| Cyclical | closed loop | ΔE_int = 0, so Q = W |
| Free expansion | Q = 0, W = 0 | ΔE_int = 0, T unchanged |

**Exam trap: free expansion looks like adiabatic but W = 0 too. Temperature does NOT change.**

### Temperature scales
Kelvin ↔ Celsius
T_K = T_C + 273.15

**Always convert to Kelvin before using any gas law. Never plug in Celsius.**

### Heat equations
Heat with temperature change
Q = mcΔT
c = specific heat capacity of the material

Phase change (melting / boiling)
Q = Lm
L = latent heat. Temperature stays flat during the entire phase change.

**If a question gives you a heating curve, the flat sections are phase changes. Q = Lm there. The sloped sections are Q = mcΔT.**

---

## Kinetic Theory

### Ideal gas law
Using moles
pV = nRT
R = 8.31 J/mol·K

Using molecules
pV = NkT
k = 1.38 × 10⁻²³ J/K (Boltzmann constant)

Use moles form when given mass/molar mass. Use molecules form when given number of particles.

### Work done by gas
General
W = ∫ p dV  (area under p-V graph)

Isothermal (constant T)
W = nRT ln(V_f / V_i)

Isobaric (constant p)
W = p(V_f − V_i)

Isochoric (constant V)
W = 0

### Internal energy and specific heats
Internal energy (monoatomic ideal gas)
E_int = (3/2)nRT

Heat capacity at constant volume
C_V = (3/2)R  →  monoatomic
C_V = (5/2)R  →  diatomic

Heat capacity at constant pressure
C_p = C_V + R

Average KE per molecule
K_avg = (3/2)kT
Temperature IS average kinetic energy. Hotter = faster molecules.

### RMS speed
v_rms = √(3RT / M)
M = molar mass in kg/mol. Lighter gas → faster molecules at same temperature.

### Adiabatic process (Q = 0)
Pressure-volume relation
p_i · V_i^γ = p_f · V_f^γ

Temperature-volume relation
T_i · V_i^(γ−1) = T_f · V_f^(γ−1)

Gamma
γ = C_p / C_V
≈ 1.67 for monoatomic
≈ 1.40 for diatomic

**Use adiabatic relations only when Q = 0 AND the process is quasi-static (not free expansion).**
