---
title: "Microfluidic Pinch Flow Fractionation Device"
excerpt: "Separates particles by size."
header:
  teaser: /assets/img/IMG_7778.jpg
---
![Completed PFF Device](/assets/img/IMG_7778.jpg)   

# Purpose

The aim of this project is to design and develop a microfluidic device, using resin 3D printing technology, that can separate particles based on their size. The method used for separation is pinch flow fractionation (PFF).


# Conducive Geometries for PFF

There should be two inlets: inlet 1 through which a liquid with the different-sized particles is fed and inlet 2 through which a liquid without any particles is fed. The size of these inlet channels should be wide enough not to induce any controlled flow profiles. Inlet 2 should have a flow rate that is about 6x as fast as the flow rate from inlet 1. The two channels will meet at a relatively short “pinched” segment, which should have a smaller width than any of the other channel segments. Its width should be as close to the diameter of the largest particles without causing any clogs. Inlet 2’s higher flow rate will push the particles from inlet 1 to one wall of the pinched segment aligning the particles in a single file flow. As the particles exit the pinched segment, the flow rate of the liquid should have a stronger effect on the smaller particles per the laws of physics, increasing the angle at which they leave the segment. There will be three outlet channels with wide enough widths that do not induce any controlled flow profiles and leave room for the particles to deviate out of the pinched segment. The first is at a positive 90-degree angle away from the pinched segment to collect the smaller particles. The second is at a 180-degree angle, or straight, to collect the larger particles. The third is a collector of liquid without any particles in it. The depth of all of these channels should be large enough to not clog based on the size of the largest particles you are trying to separate.

Experiment-specific dimensions:
- Larger particle diameter: 550 microns
- Smaller particle diameter: 165 microns
- Channel depth: 1000 microns
- Inlet 1 and 2 width: 1500 microns
- Pinched segment width: 800 microns
- Outlet channels width: 1000 microns

![Dimension Diagram](/assets/img/diagram.jpg)   

# Instructions after mold is 3D printed
1. Post cure the resin-printed mold for 1 minute to keep warping to a minimum
2. Coat the inside with parylene (more information on this below)
3. Fill with PDMS
![Pouring PDMS](/assets/img/IMG_7710.jpg)  
4. Vacuum the air bubbles out of the PDMS
5. Let the PDMS set
6. Remove from mold and add glass slide

SLA resin printing has a lot of benefits that are essential to 3D manufacturing microfluidic devices, the most notable of which is the small resolution that the ultraviolet laser can cure, or harden, the resin with. In the image below, this would result in a line width on the scale of micrometers. In other words, I could print really small features that would create microchannels in the final PDMS device. However, the biggest drawback of SLA resin printing for this application is that the laser’s scanning pattern inherently leaves some resin uncured in liquid form within the final part. This happens because the cross-sections of the laser lines are parabolas as shown in the image, and with a bunch of parabolas stacked next to each other, there will be empty space where resin does not get cured. The uncured resin will leak from inside the part to the surface over time, which would prevent the PDMS material from hardening in the mold. Therefore, I coated the 3D resin-printed mold in a very thin layer of parylene, a hydrophobic polymer, that keeps the uncured resin from leaking to the surface. After this coating is applied, the mold can be used to make many more microfluidic devices.


# CAD Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a4cecb590d706cc6f2?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>


# Application of PFF
Pinch flow fractionation is an effective technique for separating particles by size. A few hypothetical applications are given below:
- DNA mutation diagnoses when DNA segments have been cleaved and are smaller than others
- Testing blood by separating it into red blood cells, white blood cells, and platelets
- Identifying environmental pollutants in water

In all of these applications, the greatest benefit of using microfluidic devices compared to other testing devices is the reduced sample volume needed. For example, instead of taking pints of blood a patient can give a sample as small as 5 mL, and the device would function. This significantly reduces cost as well.

An additional button on the side of the enclosure changes the motor between clockwise and counterclockwise. When the button is not pressed, the motor will move clockwise, dispensing the liquid. When the button is pressed, the motor will operate counterclockwise. This allows the syringe pump to be reset to its original position without manually turning the lead screw or flexible coupler with your fingers. This button is red and located on the far right of our enclosure. 

A potentiometer controls the flow rate of the syringe pump. The flow rate is displayed in the serial monitor of the Arduino IDE and updates as the potentiometer turns. It is controlled by a dial extruded through the lid of the enclosure. The flow rate increases as the user turns the dial to the left.

