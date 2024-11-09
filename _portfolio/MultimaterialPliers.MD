---
title: "Multimaterial Pliers"
excerpt: "Functional pliers 3D printed out of a combo of TPU and PLA."
header:
  teaser: /assets/img/Holding.jpg
---
![Iteration1](/assets/img/Holding.jpg)   

# Purpose

The aim of this project is to design and develop a microfluidic device, using resin 3D printing technology, that can separate particles based on their size. The method used for separation is pinch flow fractionation (PFF).


# About Multimaterial Parts


Experiment-specific dimensions:
- Larger particle diameter: 550 microns
- Smaller particle diameter: 165 microns
- Channel depth: 1000 microns
- Inlet 1 and 2 width: 1500 microns
- Pinched segment width: 800 microns
- Outlet channels width: 1000 microns

![Dimension Diagram](/assets/img/Diagram.png)   

# Instructions after mold is 3D printed
1. Post cure the resin-printed mold for 1 minute to keep warping to a minimum
2. Coat the inside with parylene (more information on this below)
3. Fill with PDMS
![Pouring PDMS](/assets/img/IMG_7710.jpg)  
4. Vacuum the air bubbles out of the PDMS
5. Let the PDMS set
6. Remove from mold and add glass slide

SLA resin printing has a lot of benefits that are essential to 3D manufacturing microfluidic devices, the most notable of which is the small resolution that the ultraviolet laser can cure, or harden, the resin with. In the image below, this would result in a line width on the scale of micrometers. In other words, I could print really small features that would create microchannels in the final PDMS device. However, the biggest drawback of SLA resin printing is that the laser’s scanning pattern inherently leaves some resin uncured in liquid form within the final part. This happens because the cross-sections of the laser lines are parabolas as shown in the image below, and with a bunch of parabolas stacked next to each other, there will be empty space where resin does not get cured. The uncured resin will leak from inside the part to the surface over time, which would prevent the PDMS material from hardening in the mold. Therefore, I coated the 3D resin-printed mold in a very thin layer of parylene, a hydrophobic polymer, that keeps the uncured resin from leaking to the surface. After this coating is applied, the mold can be used to make many more microfluidic devices.

![Parabolic Laser Cross Section](/assets/img/DragonScale.png)
(From Additive Manufacturing 3rd Edition.)


# CAD Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a4c3ec97dd392138ce?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

# Iterations

|             | 6%, 8%, 10% Infill     | Failed Dovetail Joints        |
| ------------|------------------------|:-----------------------------:|
| Iteration 1 | /assets/img/Infill.jpg |/assets/img/Failed Dovetail.jpg|

|             | Standard Holding       | Standard Closed       | Extra Squeezing           | Expanded Jaw Capacity   |
| ------------|------------------------|-----------------------|---------------------------|:-----------------------:|
| Iteration 2 |/assets/img/Holding.jpg |/assets/img/Closed.jpg |/assets/img/ExtraClosed.jpg|/assets/img/ExtraOpen.jpg|



# Application of PFF
Pinch flow fractionation is an effective technique for separating particles by size. A few hypothetical applications are given below:
- DNA mutation diagnoses when DNA segments have been cleaved and are smaller than others
- Testing blood by separating it into red blood cells, white blood cells, and platelets
- Identifying environmental pollutants in water

(From AI generated Google search)

In all of these applications, the greatest benefit of using microfluidic devices compared to other testing devices is the reduced sample volume needed. For example, instead of taking pints of blood, a patient can give a sample as small as 5 mL, and the device would function. This significantly reduces cost as well.


