---
title: "Gears"
permalink: /motion/gears
sidebar:
  nav: mechanical_sidebar
---

See also: [Gearboxes]({{ '/motion/gearboxes' | relative_url }})

## Gear Basics

Gears are used to transmit power. By varying the ratio between two gears (in terms of teeth) you can vary output speed and torque.

A ratio of 2:1 can be created through the use of any two gears in that ratio (40 tooth:20 tooth, 32 tooth: 16 tooth, etc). If the larger gear is the input gear, the output gear will spin about twice as fast, with roughly half as much torque. Small variences here are a result of lost power (inperfect efficiency) to friction and other forces. If the smaller gear is the input gear, the gears will create a 1:2 reduction and cause speed to be halved and torque to be doubled.

#### Gearing Efficiency

Each stage of gearing will result in some inefficiency in the power transmission.

Type           | Normal Ratios | Efficiency
---------------|---------------|-----------
Spur	         | 1:1 to 6:1    | 94% to 98%
Straight Bevel | 1.1 to 5:1    | 93% to 97%
Worm 	         | 5:1 to 75:1   | 50% to 90%


## Spur Gears

Spur Gears are the most commonly used gears in robotics. The individual teeth have a straight cut involute profile.

US System gears are specified in diametral pitch (teeth per inch of diameter), and pressure angle. Mating (or meshing) gears must have the same diametral pitch and pressure angle.

Metal gears are typically available in a DPs of 3 to 32, and pressure angles of 14.5 degrees & 20 degrees. Plastic and brass gears typically run with a DP of 16 to 64 and a pressure angle of 20 degrees. Typical COTS gears used in FRC, such as those sold by AndyMark and Vex, have a DP of 20 and a pressure angle of 14.5⁰.

#### Definitions

The pitch diameter is the location where the teeth mate. This is NOT the same as the outside diameter of the gear.

Pitch diameter = number of teeth / diameteral pitch

The outside diameter (OD) of the gear is calculated as follows:

Outer diameter = (Number of teeth + 2) / diameteral pitch

#### Metric Gears

Metric Gears are specified by module, which is simply the pitch diameter/number of teeth. They all use a 20° pressure angle. The only common metric gears in FRC is used in some of the automotive window & throttle motors. Module 1.25 gearing is the most similar to the 20dp gearing while module 1.0 gearing is equivlent to a 25.4dp.

## Bevel & Miter Gears

Bevel gears are useful to change the direction of mechanical power, typically by 90 degrees. This allows unique packaging, and is especially useful in mechanisms like swerve drives and turrets. Bevel gears can also provide a speed reduction or increase depending on tooth count.

Bevel gears are normally bought as a set. The teeth are cut in each set so that both angles meet at a central point, creating a cone-like profile. In use, bevel gears apply force away from each other so a thrust bearing should be used when possible to support the gears`.

Miter gears are simply bevel gears with the same tooth count (1:1 ratio).

## Worm Gearing

Worm gears are another method of transmitting power at a right angle, and can provide a very compact speed reduction (up to 75:1). As with bevel gears, these are always purchased as a set. The worm is normally of steel construction, and the worm gear is normally a softer metal such as brass to control wear.

Worm gears are useful over bevel gears in some applications due to the very compact reduction and because the worm gear can’t back-drive the worme.

Worm gear efficiency is a function of the lead angle of the worm. Lead angles of 45⁰ provide the maximum efficiency.

## Ancillary Gearing
There are other forms of gearing available including multi-angled herringbone gears, slanted helical gears and curved gearing such as hypoid and cycloid gearing. These are typically more expensive, more difficult to source, and challenging to design with.
