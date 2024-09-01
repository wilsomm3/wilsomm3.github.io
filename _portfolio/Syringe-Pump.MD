---
title: "DIY Syringe Pump"
excerpt: "Delivers precise and accurate volumes of fluids in laboratory and medical settings."
header:
  teaser: /assets/img/syringe-pump.jpg
---
![Completed Syringe Pump](/assets/img/syringe-pump.jpg)   

# Features

* **Massive Print Area: 1140 x 1200 x 1100 mm.** With a build envelop just shy of 4 feet in all dimensions, the LF3DP is capable of printing furniture and other large objects.
* **High Volumetric Output Extruder: 1 kg/hr - 450 C.** This printer come standard with a MDPH2 extruder by Massive Dimension, which can extrude at a rate of 1 kg/hr. Unlike typical filament extruders, the MDPH2 uses a screw to convey and liquify plastic pellets before the molten material is pushed out of a large nozzle (1 to 5 mm extrusion diameter). Please note: This printer can also be configured for other high flow rate extruders, such as the Typhoon and Pulsar by Dyze Design.
* **Affordable Pellet Feedstock** Pellets are the cheapest form of feedstock for any plastic-based manufacturing process. Save 50-75% of material costs by using pellets instead of spools of filament. Concentrated colorant can be added to the virgin material to achieve any color in the rainbow without requiring large amounts of storage. Recyled material can also be used for sustainable material printing.

# Off-the-shelf Parts Used

| Part Name                                | Quantity      |
| ---------------------------------------- |:-------------:|
| 250mm lead screw (2mm pitch/8mm lead)    | 1             |
| 1/4 inch 8mm flexible coupler            | 1             |
| 200mm linear rod (8mm diameter)          | 2             |
| LM8UU linear bearing for 8mm diameter rod| 2             |
| 2040 aluminum extrusion 1 inch length    | 1             |
| Nema 17 stepper motor                    | 1             |
| MeanWell AC-DC quad output power supply  | 1             |
| Arduino Uno                              | 1             |
| A4988 stepper driver                     | 1             |
| Small breadboard                         | 1             |
| Panel mount latching push buttons        | 2             |
| Limit switch                             | 1             |
| RGB common cathode LED                   | 1             |
| Potentiometer                            | 1             |
| 10mL syringe                             | 1             |


# 3D Printed Parts Used

| Part Name                      | Quantity      |
| ------------------------------ |:-------------:|
| Motor Mounting Plate           | 1             |
| End Supports with Syringe Slots| 2             |
| Carriage with Syringe Slot     | 1             |
| Enclosure Lid                  | 1             |
| Enclosure Base                 | 1             |


# CAD Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a4806a535b816c4399?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

# Arduino Code
Our Arduino code [[1](https://app.arduino.cc/sketches/10db4069-85a7-4e58-bffd-baaf771bee5d?view-mode=preview)] completes precise calculations to find the necessary stepper motor speed to dispense fluid at a given flow rate determined by the potentiometer. It also converts manual operations of the push buttons attached to the enclosure into instructions for the stepper motor to follow. The code outputs signs to the user of the internal operation of the motor via the LED light.

*1. Syringe pump Arduino code for Team Kazoo*

# Pump Operation Instructions
  Our syringe pump is motor-driven. A latching button mounted on the side of the enclosure is utilized to initiate and stop the pump's movement. It is the black button to the right of the LED light. The pump is also controlled by the limit switch attached to the carriage once the syringe is entirely dispensed, but that will occur automatically. The LED to the right of the black latching button indicates if the pump is running, paused, or out of the liquid. Green means it is running, yellow means it is broken, and red means the syringe is out of fluid.  
  An additional button on the side of the enclosure changes the motor between clockwise and counterclockwise. When the button is not pressed, the motor will move clockwise, dispensing the liquid. When the button is pressed, the motor will operate counterclockwise. This allows the syringe pump to be reset to its original position without manually turning the lead screw or flexible coupler with your fingers. This button is red and located on the far right of our enclosure. 
  A potentiometer controls the flow rate of the syringe pump. The flow rate is displayed in the serial monitor of the Arduino IDE and updates as the potentiometer turns. It is controlled by a dial extruded through the lid of the enclosure. The flow rate increases as the user turns the dial to the left.


