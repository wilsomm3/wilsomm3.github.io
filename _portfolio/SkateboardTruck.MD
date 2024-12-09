---
title: "Generative Design Skateboard Truck"
excerpt: "Mounts phone to bike handle bars for easy navigation."
header:
  teaser: /assets/img/PhoneSecure.jpg
---
![Phone is secure](/assets/img/Standalone.jpg)   

# Generative Design

Generative design uses AI technology to create a model that connects what the designer designates as preserve geometry while avoiding what they have designated as obstacle geometry. These calculations also take into consideration the predicted load cases that the design will experience during its intended use. As a result, the design generally builds more material in highly loaded areas while minimizing material in other places. Through this process, generative design creates the opportunity for natural geometries that traditional design practices cannot match. These geometries naturally pair with the powder bed fusion manufacturing process. Not only can powder bed fusion produce some of the highest mechanical strengths out of all the additive manufacturing methods, but it also produces resolutions as low as 110 microns. 

## Application

The aerospace industry is pushing for more fuel-efficient aircraft featuring optimized internal storage spaces, and generative design is helping engineers conceptualize new aircraft forms to meet these standards. Some potential inputs to an aerospace generative study are emissions, materials, aerodynamic geometries, and the forces of takeoff and landing. The study would then output ideal shape options, such as the blended-wing-body, that could replace the traditional tube-and-wing form. The use of AI is creating an expanded path for aerospace engineers to explore and analyze potentially ground-breaking changes to the industry.

From [Siemens] (https://blogs.sw.siemens.com/thought-leadership/2022/10/10/applying-generative-design-to-aerospace/)

## Utility

Generative design has the potential to supply lots of design options for an engineer to choose from with diminished effort compared to traditional design techniques. It is especially useful in minimizing the number of components in an assembly while still remaining durable and easy to assemble post-manufacturing. In this project, I found that its ability to generate designs made out of different materials (aluminum and nylon) was especially useful. In my future career, I could see myself using generative design to determine whether a certain material will be strong enough to endure the anticipated loads as compared to other materials.

## Drawbacks

From this project, I learned that the load cases the designer chooses to apply are a large determining factor for the generative design’s outcomes. This can be a drawback for designers who do not have a great understanding of the forces the final outcome will undergo. From my experience with the longboard truck, theoretical force calculations are often not accurate compared to real-life simulations. I believe the most successful designs would have accurately simulated forces applied, which would take lots of prior research. For example, our class discussed how we cannot be sure what the forces of the longboard’s impact with a curb would be due to the wheels’ ability to store some of the kinetic energy. A solution to this would be attaching a gauge to the board and riding it ourselves at top speeds into a curb, but for safety reasons, we were obviously not willing to do this. Instead, I used general calculations and estimations to apply forces in my load cases. Still, I often had to lower the forces I implemented in my load cases in order to get the generative model to converge with a safety factor of 2. I found that these conditions were not conducive to generating a variety of outcomes to choose from, which is one of the largest benefits of using generative design techniques. While load cases are quite essential to ensure the final outcome is durable, they have the potential to highly restrict and diminish the value of the generative models, which is the main drawback I saw.


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
