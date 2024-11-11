---
title: "Multimaterial Pliers"
excerpt: "Functional pliers 3D printed out of a combo of TPU and PLA."
header:
  teaser: /assets/img/Final.jpg
---
![Iteration1](/assets/img/Final.jpg)   


# Background

Print-in-place parts can be functional straight off the print bed with no assembly required. Sometimes it is more convenient to design simple parts that can be assembled together in a functional model after each piece is printed. However, new advances in design techniques and printer settings have allowed engineers to 3D print functional joints and moveable pieces with one model, saving time on production. Some examples of print-in-place parts range from silly models like octopi with legs that have lots of joints to make them wiggle or useful like robotic fingers for anthropomorphic manipulators or dental prostheses. The key applications for printing-in-place are in parts that function with movement by designing hinges, flexures, and other joints to be printed within the model. If these parts are printed with one material, the layers around the joints need to be precisely separated, which is difficult in plastic filament deposition. Printing with 2 or more materials, AKA multimaterial, in one part increases the opportunity for variety in the parts. In my multimaterial pliers, the combination of an elastic joint with rigid plastic handles allows for opening and closing functionality. Common material combinations for multimaterial print-in-place parts are PLA-TPU and ABS-TPU.


# CAD Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a4c3ec97dd392138ce?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>


# Specifications

The jaw length is approximately 30mm long: 10mm straight section and 20mm section angled at 8 degrees. The handles are 7cm apart and 9.5cm long. The joint is 30mm x 30mm.


# Print Settings
### Rigid

The plier handles and pinchers shown in white were printed in PLA on the Voron 300 with a 0.6 nozzle. The settings were all set to default, except the infill was gyroid pattern at 10%.

### Elastic

The joint shown in black was printed in TPU 95A on the Voron 300 with a 0.6 nozzle. The solid layers on the top and bottom were set to 0. The infill was set to 10% with the rectilinear pattern angled 45 degrees. All other settings were set to default.


# Iterations

see picture gallery below for references

### Iteration 1

Infill testing: I printed the TPU joint component in three models with infill percentages of 6%, 8%, and 10% (1). The joint was designed to be a diamond shape, rather than a square, in this iteration. This made it harder to pick the correct infill angle because 45 degrees did not line up perfectly with the edges.

Dovetail fit testing: I could not determine the best infill percentage from this iteration because the handle pieces fit too loosely with the joint. The dovetail angles were 70 degrees, the lower dimension was 1.5mm, the upper was 4mm, and the offset clearance between the joint and the PLA pieces was 0.2 mm. This led to more square-like dovetail joints that did not retain the pieces to the joint during pinching (2).

Functionality: none

### Iteration 2

Infill testing: The joint was changed to be a 30x30mm square. All were springy enough, but 10% felt the best. The others did not take much force to close them, so even having my hands on the handles was enough to make them close. On the other hand, 10% required more intentionality to overcome the force, which better matched the feeling of normal pliers.

Dovetail fit testing: The lower dimension stayed 1.5mm, but the upper was increased to 5mm, the angle was decreased to 50 degrees, and the offset clearance was reduced to 0.1mm.

Functionality: This iteration of the pliers opened and closed as required, but I wanted to optimize it. The ergonomics of the handle were not ideal since I had to stretch my hand too far to comfortably squeeze the handle. Also, the jaw capacity was only 4mm and met at a small point. Finally, if I squeezed it tightly, the half-dovetail joints between the pinchers and the joint would come loose as shown in the red circle below (3).

### Iteration 3

Infill testing: none. I reused the joint from iteration 2.

Dovetail fit testing: none. I reused the clearance and geometry from iteration 2 on the PLA pieces.

Functionality: I made the handles parallel to each other, rather than angling outward, to increase ergonomics. I added an angle away from the midline to the end of the pinchers, which increased the jaw capacity to 9 mm and the surface area at which the pinchers met. I also completed the joints that were coming loose in iteration 2.


|                | 6%, 8%, 10% Infill (1)         | Failed Dovetail Joints (2)         |
| ---------------|-----------------------------------|:------------------------------------------:|
| Iteration 1    | ![Infill](/assets/img/Infill.jpg) |![Dovetail](/assets/img/FailedDovetail.jpg)|

|                | Standard Holding         | Standard Closed         | Extra Squeezing (3)     |
| ---------------|--------------------------|-------------------------|:-----------------------:|
| Iteration 2    |![Hold](/assets/img/Holding.jpg) |![Close](/assets/img/Closed.jpg) |![Squeeze](/assets/img/ExtraClosed.jpg)|

|                | Standard Holding        | Standard Closed         |
| ---------------|-----------------------------------|:------------------------------------------:|
| Iteration 3    | ![Final Holding](/assets/img/FinalHolding.jpg) |![Final Closed](/assets/img/FinalClosed.jpg)|


# GIF
![It Works(/assets/img/Pliers.gif)
