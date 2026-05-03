---
layout: project
title: Nutcracker 2
description: Nutcracker Design 2
---
## Problem Update

Initially, the nutcracker handles were assumed to be rigid. In this analysis, the handles are modeled as beams that deform under load.

Only the transverse (vertical) components of the forces from the actuator and the nut are considered.

---

## a. Location of Maximum Elastic Deflection

The handle is modeled as a cantilever beam.

Assumptions:

- Handle length: L = 120 mm  

- Force applied at end: P ≈ 300 N  

- Fixed at the pivot  

- Load applied at the free end  

For a cantilever beam with a point load at the end, the maximum deflection occurs at the free end.

Therefore, the location of maximum elastic deflection is at the end of the handle, where the actuator force is applied.

---

## b. Beam Design for Less Than 2% Deflection

### Deflection constraint

delta_allowable = 0.02 L  

delta_allowable = 0.02 (120 mm) = 2.4 mm  

---

### Material selection

Material: 6061-T6 Aluminum  

- Elastic modulus: E ≈ 69 GPa  

- Yield strength: ≈ 276 MPa  

This material is chosen because it is lightweight and provides good stiffness.

---

### Required stiffness

For a cantilever beam:

delta = (P * L^3) / (3 * E * I)

Rearranging:

I_required ≈ 1.05 × 10^-9 m^4  

---

### Selected cross-section

Rectangular beam:

- Width b = 15 mm  

- Height h = 10 mm  

Moment of inertia:

I = (b * h^3) / 12  

I ≈ 1.25 × 10^-9 m^4  

Since:

1.25 × 10^-9 > 1.05 × 10^-9  

✔ The design satisfies the stiffness requirement

---

### Deflection check

delta_max ≈ 2.01 mm  

Since:

2.01 mm < 2.4 mm  

✔ Deflection is within the allowable limit

---

### Stress check

sigma_max ≈ 144 MPa  

Since:

144 MPa < 276 MPa  

✔ The beam remains in the elastic region

---

## c. Final Beam Design

- Material: 6061-T6 Aluminum  

- Length: 120 mm  

- Cross-section: 15 mm × 10 mm  

- Maximum deflection: 2.01 mm  

- Allowable deflection: 2.4 mm  

This design is mass-efficient because increasing the height of the beam significantly improves stiffness (proportional to h³), allowing a small cross-section to meet the deflection requirement.

<img src="/workspaces/sp26-portfolio-ericlee4992/assets/images/New-nutcracker.png">

---