---
layout: project
title: Nutcracker Project
description: Nutcracker design problem
image: /assets/images/Nutcracker-diagram.jpeg
---

1. Problem Statement and Objective

The objective of this project is to design a simple lever-based nutcracker capable of cracking a macadamia nut by hand. Macadamia nuts require significantly larger cracking forces than most other nuts, so the device must provide sufficient mechanical advantage to amplify the force applied by the user.

The goal is to determine a feasible geometry for a nutcracker such that a human user can apply a reasonable hand force while generating the required compressive force on the nut. Additionally, the design will be modified to consider the use of a linear actuator instead of hand grip strength as the input force.

2. Constraints and Input Parameters

Several inputs and constraints are required for the design.

Macadamia nut cracking force

Research shows that the average load required to crack a macadamia nut is approximately:

F_crack = 220kg

Converting to force:

F_crack = 220(9.81) = 2160 N = 485 lbf

Human grip strength

Typical maximum grip strength for adults ranges between:

F_hand = 300 ~ 500 N

For a conservative design, a hand force of:

F_hand = 300 N is assumed.

Nut size

Macadamia nuts typically have diameters around:

d_nut = 16 ~ 22 mm

The jaw opening of the nutcracker must therefore accommodate this size.

Design requirements
	•	Generate at least 2160 N (485 lbf) compressive force on the nut
	•	Be operable with a reasonable hand force
	•	Use simple lever mechanics
	•	Allow placement of a nut approximately 20 mm in diameter

3. Approach and Calculations

The nutcracker is modeled as a simple lever system with a pivot near the jaws.

Lever geometry

Let

L_h = distance from pivot to where the hand force is applied
L_j = distance from pivot to the nut contact point

The mechanical advantage (MA) of the lever is:

MA = L_h / L_j

Force balance about the pivot gives:

F_hand * L_h = F_nut * L_j

or

F_nut = F_hand * L_h / L_j

Required mechanical advantage

To crack the nut:

MA = F_crack / F_hand

MA = 2160/300 = 7.2

Therefore the nutcracker must have at least 7.2× mechanical advantage.

Proposed geometry

A feasible design uses:

Pivot → hand distance
L_h = 120mm

Pivot → nut distance
L_j = 15mm

Mechanical advantage:

MA = 120/15 = 8

Output force on the nut:

F_nut = 300 * 8 = 2400 N

Since

2400 N > 2160 N

the design should successfully crack a macadamia nut.


4. 
<img src="/assets/images/Nutcracker-diagram.jpeg" width="500">

5. Usability Discussion

The nutcracker design is practical because it significantly amplifies the force applied by the user. With a mechanical advantage of approximately 8, a moderate hand force of around 300 N can generate the large force required to crack a macadamia nut.

The long handles improve ergonomics and allow the user to apply force comfortably. Additionally, a small jaw distance from the pivot increases mechanical advantage, which is necessary due to the extreme hardness of macadamia shells.

However, placing the nut too close to the pivot can make insertion slightly more difficult and may require careful positioning to ensure the nut does not slip. Textured or curved jaws could improve stability.