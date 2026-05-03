---
layout: project
title: Nutcracker 2
description: Nutcracker Design 2
image: /assets/images/Nutcracker-diagram.jpeg
---
### a. Location of Maximum Elastic Deflection

For this update, I modeled one nutcracker handle as a cantilever beam. The handle is assumed to be fixed near the pivot/jaw region and loaded by the actuator force at the far end of the handle. Only the transverse component of the actuator force is considered.

Assumptions:

- Handle length: `L = 120 mm = 0.12 m`

- Actuator force needed: about `300 N`

- Handle modeled as a cantilever beam

- Maximum deflection occurs at the free end of the handle where the actuator force is applied

For a cantilever beam with a point load at the end:

\[

\delta_{max} = \frac{PL^3}{3EI}

\]

The maximum elastic deflection occurs at the end of the handle because that point is farthest from the fixed pivot region and experiences the largest bending displacement.

---

### b. Beam Design for Less Than 2% Deflection

The deflection limit is:

\[

\delta_{allowable} = 0.02L

\]

\[

\delta_{allowable} = 0.02(120 mm) = 2.4 mm

\]

I selected **6061-T6 aluminum** for the handle because it is lightweight, stiff, and commonly used for mechanical components. 6061-T6 aluminum has an elastic modulus of approximately `68.9 GPa` and yield strength around `276 MPa`. 

Using:

\[

I_{required} = \frac{PL^3}{3E\delta}

\]

\[

I_{required} = \frac{(300)(0.12)^3}{3(68.9 \times 10^9)(0.0024)}

\]

\[

I_{required} \approx 1.05 \times 10^{-9} m^4

\]

A feasible rectangular cross-section is:

- Width: `15 mm`

- Height: `10 mm`

For a rectangular beam:

\[

I = \frac{bh^3}{12}

\]

\[

I = \frac{(15)(10^3)}{12} = 1250 mm^4

\]

\[

I = 1.25 \times 10^{-9} m^4

\]

Since:

\[

1.25 \times 10^{-9} > 1.05 \times 10^{-9}

\]

this cross-section satisfies the deflection requirement.

The predicted deflection is:

\[

\delta_{max} = \frac{PL^3}{3EI}

\]

\[

\delta_{max} \approx 2.01 mm

\]

Since:

\[

2.01 mm < 2.4 mm

\]

the design meets the requirement.

The maximum bending stress is:

\[

\sigma_{max} = \frac{Mc}{I}

\]

\[

\sigma_{max} = \frac{(300)(0.12)(0.005)}{1.25 \times 10^{-9}}

\]

\[

\sigma_{max} \approx 144 MPa

\]

This is below the yield strength of 6061-T6 aluminum, so the handle should remain elastic.

---

### c. Final Beam Design

Final handle design:

- Material: 6061-T6 aluminum

- Handle length: `120 mm`

- Cross-section: rectangular beam

- Width: `15 mm`

- Height: `10 mm`

- Maximum deflection: `2.01 mm`

- Allowable deflection: `2.4 mm`

- Result: design meets the stiffness requirement

This design is mass-efficient because the handle uses a relatively small rectangular cross-section while still keeping the deflection below 2% of the handle length. A taller cross-section is useful because bending stiffness increases with height cubed, making it more efficient than simply making the handle wider.