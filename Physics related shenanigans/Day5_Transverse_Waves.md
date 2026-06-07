# Day 5 — Transverse Waves

---

## What is a transverse wave?
Disturbance is perpendicular to the direction of travel.
Rope shaken side to side → wave travels forward, rope moves up and down.
A wave moves energy, not matter.

---

## The wave equation — know every part
y(x, t) = y_m sin(kx − ωt)

| Symbol | Name | What it means |
|--------|------|---------------|
| y_m | Amplitude | Max displacement from equilibrium |
| k | Wave number | How many radians per metre of wave |
| ω | Angular frequency | How many radians per second of oscillation |
| kx − ωt | Phase | Determines position on the wave cycle at any (x, t) |

**Given any wave equation, you should be able to read off y_m, k, and ω instantly.**

---

## All the quantities you need to extract
Wave number
k = 2π / λ   →   λ = 2π / k

Angular frequency
ω = 2π / T = 2πf   →   T = 2π / ω   →   f = ω / 2π

Wave speed — three equivalent forms
v = λ / T = ω / k = fλ

**Fastest way to find speed from the equation: v = ω / k. No extra steps.**

---

## Transverse velocity of a particle
This is NOT the wave speed. It's how fast a single point on the medium moves up and down.

Transverse velocity
u_p = dy/dt = −ωy_m cos(kx − ωt)

Maximum transverse speed
u_p,max = ωy_m

**Exam question type: given y(x,t) = 0.1 sin(4x − 5t), find max transverse speed.**
→ y_m = 0.1, ω = 5
→ u_p,max = 5 × 0.1 = 0.5 m/s

---

## Speed of a wave on a string
v = √(T / μ)
T = tension in the string (Newtons)
μ = linear mass density = mass / length (kg/m)

**μ = m / L. If given mass in grams, convert to kg first.**

Example: L = 10 m, mass = 20 g = 0.02 kg
μ = 0.02 / 10 = 0.002 kg/m

---

## Worked example — the lecture slide type
Given: y(x, t) = 0.1 sin(4x − 5t)

Read off directly:
y_m = 0.1 m
k = 4 rad/m
ω = 5 rad/s

Then calculate:
λ = 2π / k = 2π / 4 = π/2 m
T = 2π / ω = 2π / 5 s
f = ω / 2π = 5 / 2π Hz
v = ω / k = 5 / 4 = 1.25 m/s
u_p,max = ωy_m = 5 × 0.1 = 0.5 m/s

**Drill this until extracting all 6 quantities from one equation takes under a minute.**

---

## Wave interference — quick reference
Two waves, same frequency, phase difference φ:

General amplitude
A = 2y_m cos(φ / 2)

Fully constructive (φ = 0)
Amplitude = 2y_m   (waves perfectly in phase)

Fully destructive (φ = π)
Amplitude = 0   (waves cancel completely)

Anything between 0 and π → partial interference.

---

## Standing waves
Right-travelling wave + left-travelling wave of same frequency = standing wave.

Standing wave equation
y = (2y_m sin(kx)) cos(ωt)

Nodes — points of zero movement
sin(kx) = 0

Antinodes — points of maximum movement
sin(kx) = ±1

**The wave pattern doesn't move — it just pulses in place. Nodes never move. Antinodes have maximum amplitude.**
