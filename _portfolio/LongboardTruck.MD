---
title: "Generative Design Longboard Truck"
excerpt: "Motorized longboard truck designed with AI assistance."
header:
  teaser: /assets/img/Alum_Rendering2.png
---
![Printed Truck](/assets/img/PrintedTruck.jpg)

## Introduction

Generative design uses AI technology to create a model that connects what the designer designates as preserve geometry while avoiding what they have designated as obstacle geometry. These calculations also take into consideration the predicted load cases that the design will experience during its intended use. As a result, the design generally builds more material in highly loaded areas while minimizing material in other places. Through this process, generative design creates the opportunity for natural geometries that traditional design practices cannot match. These geometries naturally pair with the powder bed fusion manufacturing process. Not only can powder bed fusion produce some of the highest mechanical strengths out of all the additive manufacturing methods, but it also produces resolutions as low as 110 microns. 

## Application

The aerospace industry is pushing for more fuel-efficient aircraft featuring optimized internal storage spaces, and generative design is helping engineers conceptualize new aircraft forms to meet these standards. Some potential inputs to an aerospace generative study are emissions, materials, aerodynamic geometries, and the forces of takeoff and landing. The study would then output ideal shape options, such as the blended-wing-body, that could replace the traditional tube-and-wing form. The use of AI is creating an expanded path for aerospace engineers to explore and analyze potentially ground-breaking changes to the industry.

From [Siemens](https://blogs.sw.siemens.com/thought-leadership/2022/10/10/applying-generative-design-to-aerospace/)

## Utility

Generative design has the potential to supply lots of design options for an engineer to choose from with diminished effort compared to traditional design techniques. It is especially useful in minimizing the number of components in an assembly while still remaining durable and easy to assemble post-manufacturing. In this project, I found that its ability to generate designs made out of different materials (aluminum and nylon) was especially useful. In my future career, I could see myself using generative design to determine whether a certain material will be strong enough to endure the anticipated loads as compared to other materials.

## Drawbacks

From this project, I learned that the load cases the designer chooses to apply are a large determining factor for the generative design’s outcomes. This can be a drawback for designers who do not have a great understanding of the forces the final outcome will undergo. From my experience with the longboard truck, theoretical force calculations are often not accurate compared to real-life simulations. I believe the most successful designs would have accurately simulated forces applied, which would take lots of prior research. For example, our class discussed how we cannot be sure what the forces of the longboard’s impact with a curb would be due to the wheels’ ability to store some of the kinetic energy. A solution to this would be attaching a gauge to the board and riding it ourselves at top speeds into a curb, but for safety reasons, we were obviously not willing to do this. Instead, I used general calculations and estimations to apply forces in my load cases. Still, I often had to lower the forces I implemented in my load cases in order to get the generative model to converge with a safety factor of 2. I found that these conditions were not conducive to generating a variety of outcomes to choose from, which is one of the largest benefits of using generative design techniques. While load cases are quite essential to ensure the final outcome is durable, they have the potential to highly restrict and diminish the value of the generative models, which is the main drawback I saw.

# My Longboard Truck

## Preserve Geometries

1. The pivot point 
-   I used this as the structural constraint in my design.
2. 8.2mm diameter sleeve to accept the threaded connecting rod.
-   Forces: weight of the rider and curb impact
3. Motor mounting plate
-   Forces: weight of the motor, motor torque, and belt tension
4. Through-hole between bushings
-   I chose not to apply any forces to this body as the TPU bushings on either side should absorb any loads it experiences.

## Load Cases

1. Regular Riding
-   This load case simulates a rider standing in the center of the board, not turning, and going approximately 30 km/hr.
2. Curb Impact
-   This load case simulates a rider standing in the center of the board, not turning, and going top speed of 55 km/hr when the board has a head-on collision with a curb.
3. Full-Weight Turn
-   This load case simulates the rider moving at a normal speed when they shift their entire weight to one side of the board in order to turn. This could also simulate the rider landing on one wheel during a trick, but since this is a motorized longboard, I believe full-weight turning would be a more realistic scenario.

## Printed Version

My first aluminum iteration that was SLS printed out of Nylon 12 was successful in fitting over the kingpin with the bushings installed as well as allowing room for the wheels to turn. These functionalities are demonstrated in the GIF below.
![It Half Works](/assets/img/Turning.gif)

Unfortunately, I was not able to shift the motor the necessary 4mm while the belt between the pulleys was put into tension as shown in the image below. 
![Pulley Out of Tension](/assets/img/LoosePulley.jpg)

This was due to extra material that the generative design built up around the motor mounting plate, which caused interference. The red arrows in the image below point these spots out.
![Interference](/assets/img/Interference.jpg)

The outer sleeve for the connecting rod also broke during part cleaning, but we can assume this would not have happened if it was actually printed out of aluminum, instead of nylon.

## Updated Design

I added extra obstacle geometries around the motor mount to ensure it has room to shift 4mm during assembly of the belt. I also added thickness to the outer sleeve to keep it from breaking in future prints. This turned out to make my models much thinner than before, which leads me to believe I could add the full forces I mentioned having to lower while still generating a converged model. Below are renderings and CAD models of the updated generative models.

|          | Aluminum         | Nylon 12       |
| ---------|--------------------------------------------|:------------------------------------------:|
| Front    | ![Front_Alum](/assets/img/Alum_Rendering1.png) |    |
| Back     |![Front_Alum](/assets/img/Alum_Rendering2.png)  |    |


# Aluminum CAD Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a448e821439a5afdfe?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

# Nylon CAD Model
