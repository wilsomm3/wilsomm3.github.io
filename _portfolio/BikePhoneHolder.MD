---
title: "Top-down Bike Phone Holder"
excerpt: "Mounts phone to bike handle bars for easy navigation."
header:
  teaser: /assets/img/PhoneSecure.jpg
---
![Phone is secure](/assets/img/Standalone.jpg)   

# Leveraging Topdown Modeling Principles

In designing this bike-mounted phone holder, I leveraged top-down modeling principles by building each component separately in one Fusion design. This allows the assembly to drive the design of each component, and no sketches were made in the top-level assembly. My initial component was a 32mm diameter, 72mm long cylinder that represented the handlebar segment of the bike I was designing for. My second component was the bike fixation that leveraged the diameter of the handlebar with an offset clearance of 1mm for its diameter. These two were rigidly fixed with an as-built joint. My third component, the phone fixation, was built with an interior post of 1mm clearance based on the inner diameter of the external post on the bike fixation component. These two components had an as-built cylindrical joint to help me visualize the rotation of the phone to portrait and landscape. The final component was the spring plug that filled the hole I built into the bike fixation to allow assembly of the parts with an internal spring. This plug leveraged the diameter of the hole and had a diameter 0.4 mm greater to ensure it would not be pulled through the hole. The bike fixation and spring plug also had a cylindrical joint for me to visualize how I would assemble the spring.

# CAD Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a4e96fd7743cbcb238?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

# Design Rationale

I wanted my phone holder to have a more binary decision between portrait and landscape mode than a lot of these types of devices have. Therefore, I implemented a slot-peg mechanism with 90 degree rotation between the phone fixation’s interior post and the bike fixation’s exterior post. A spring between the two keeps the phone fixation from flying out of the exterior post.

# Material Choice

I had an initial design concept prototype printed out of PLA that was successful, but on the second print, which was my first full iteration, many of the features did not form. This led me to switch to SLS powder-printing out of Nylon PA12.

|              | Failed Hook of Phone Fixation     | Failed Bike Fixation        |
| -------------|-----------------------------------|:-------------------------------:|
| Iteration 1  | ![Hook failed](/assets/img/PhoneFail.jpg) |![Mount failed](/assets/img/BikeFail.jpg)|


# Assembly Instructions

**Spring Component:**
1. A 4mm diameter, 20mm long spring must be attached to the hook on the underside of the phone fixation component.
2. Seat the phone fixation into the bike fixation aligning the pegs with the slots.
3. Pull the bottom loop of the spring through the hole under the bike fixation.
4. Attach the spring to the spring plug’s hook and seat the plug into the hole.


**Mounting:**
1. Seat the bike fixation on the handlebar.
2. Feed 2x M5 bolts (50mm length) through each hole in the bike fixation under the handle bar.
2. Tighten M5 nut and bolt with allen key and pliers.

# Gallery

The bike rider can easily switch the phone between landscape and portrait modes.
![Rotation](/assets/img/Rotation.gif)

The phone is secure while riding and has the perfect angle for viewing.
![It Works](/assets/img/InMotion.gif)
