---
title: "Multimaterial Pliers"
excerpt: "Functional pliers 3D printed out of a combo of TPU and PLA."
header:
  teaser: /assets/img/Holding.jpg
---
![Iteration1](/assets/img/Holding.jpg)   


# About Multimaterial Parts




# CAD Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a4c3ec97dd392138ce?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>


# Specifications

The jaw length is approximately 30 mm long: 10 mm straight part and 20 mm part angled at 8 degrees. The handles are 7 cm apart and 9.5 cm long. The joint is 30mm x 30mm.


# Print Settings
### Rigid

The plier handles and pinchers shown in white were printed in PLA on the Voron 300 with a 0.6 nozzle. The settings were all set to default, except the infill was gyroid pattern at 10%.

### Elastic

The joint shown in black was printed in TPU 95A on the Voron 300 with a 0.6 nozzle. The solid layers on the top and bottom were set to 0. The infill was set to 10% with the rectilinear pattern angled 45 degrees. All other settings were set to default.


# Iterations
### Iteration 1

Infill testing: I printed the TPU joint component in three models with infill percentages of 6%, 8%, and 10%. The joint was designed to be a diamond shape, rather than a square, in this iteration. This made it harder to pick the correct infill angle because 45 degrees did not. The next iteration

Dovetail fit testing: I could not determine the best infill percentage from this iteration because the handle pieces fit too loosely with the joint. The dovetail angles were 70 degrees, the lower dimension was 1.5mm, the upper was 4mm, and the offset clearance between the joint and the PLA pieces was 0.2 mm. This led to more square-like dovetail joints that did not retain the pieces to the joint during pinching.

Functionality: none

### Iteration 2

Infill testing: All were springy enough, but 10% felt the best. The others did not take much force to close them, so even having my hands on the handles was enough to make them close. On the other hand, 10% required more intentionality to overcome the force, which better matched the feeling of normal pliers.

Dovetail fit testing: The lower dimension stayed 1.5mm, but the upper was increased to 5mm, the angle was decreased to 50 degrees, and the offset clearance was reduced to 0.1mm.

Functionality: This iteration of the pliers opened and closed as required, but I wanted to optimize it. The ergonomics of the handle were not ideal since I had to stretch my hand too far to comfortably squeeze the handle. Also, the jaw capacity was only 4mm and met at a small point. Finally, if I squeezed it tightly, the half-dovetail joints between the pinchers and the joint would come loose as shown in the red circle below.

### Iteration 3

Infill testing: none. I reused the joint from iteration 2.

Dovetail fit testing: none. I reused the clearance and geometry from iteration 2 on the PLA pieces.

Functionality: I made the handles parallel to each other, rather than angling outward, to increase ergonomics. I added an angle away from the midline to the end of the pinchers, which increased the jaw capacity to 9 mm and the surface area at which the pinchers met. I also completed the joints that were coming loose in iteration 2.




|               | 6%, 8%, 10% Infill                | Failed Dovetail Joints                     |
| --------------|-----------------------------------|:------------------------------------------:|
| Iteration 1   | ![Infill](/assets/img/Infill.jpg) |![Dovetail](/assets/img/FailedDovetail.jpg)|

|             | Standard Holding         | Standard Closed         | Extra Squeezing             | Expanded Jaw Capacity     |
| ------------|--------------------------|-------------------------|-----------------------------|:-------------------------:|
| Iteration 2 |![Hold](/assets/img/Holding.jpg) |![Close](/assets/img/Closed.jpg) |![Squeeze](/assets/img/ExtraClosed.jpg)|![Open](/assets/img/ExtraOpen.jpg)|

