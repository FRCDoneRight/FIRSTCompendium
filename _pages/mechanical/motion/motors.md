---
title: "Motors"
permalink: /motion/motors
sidebar:
  nav: mechanical_sidebar
---

DC motors are an integral part of competition robotics, and proper motor selection is essential to successful robot design.

To help select proper motors for mechanisms, a table with specifications of popular motors is below. This table contains mostly experimental data from VEX, which can be found [here](http://motors.vex.com/#testing). VEX Robotics motor curves were developed experimentally using a "down-up" dyno test, an industry-standard measurement system which helps to correct for rotational inertia. This data is more useful for comparison than nominal specifications due to its common method of measurement.


|Free Speed (RPM)|Free Current (A)| Maximum Power (W)|Stall Torque (Nm)|Stall Current(A)|Price ($)
--------------------|-------|-----|-----|------|-----|-----
CIM                 | 5330  | 2.7 | 337 | 2.41 | 131 | 27.99
Vex Mini CIM        | 5840  | 3.0 | 215 | 1.41 | 89  | 24.99
Vex BAG             | 13180 | 1.8 | 149 | 0.43 | 53  | 24.99
Vex/WCP 775pro      | 18730 | 0.7 | 347 | 0.71 | 134 | 17.99
AndyMark Redline*   |       |     |     |      |     | 18.00
AndyMark 9015       | 14270 | 3.7 | 134 | 0.36 | 71  | 14.00
AndyMark NeveRest** | 5480  | 0.4 | 25  | 0.17 | 10  | 18.00
AndyMark RS-775-125 | 5800  | 1.6 | 43  | 0.28 | 18  | 18.00
BaneBots RS-775 18V | 13050 | 2.7 | 246 | 0.72 | 97  | 17.50
BaneBots RS-550     | 19000 | 0.4 | 190 | 0.38 | 84  |  7.25

\* Specifications are nominal (not measured)

\*\* Price is $10 without encoder.

## Key Characteristics of DC Motors

Four key characteristics are used to define a motor's performance. When designing a mechanism, all tradeoffs must be considered for the particular application.

* **Free Speed** (RPM) – The maximum speed at which a motor will rotate when under no load
* **Free Current** (A) – The minimum current a motor will draw when under no load
* **Stall Torque** (Nm) – The amount of load placed on a motor that will cause it to stall (stop moving)
* **Stall Current** (A) – The amount of current drawn by a motor when it is stalled

Under no load, "free", a motor spins at its **free speed** and draws a **free current**. Conversely, **stall torque** and **stall current** represent a motor being worked to its maximum, or "stalled", to the point at which it can no longer move.

These characteristics represent the theoretical minimum and maximum conditions for a motor.

Motors generally should not be run at these edge conditions, so usage in mechanisms should be optimized somewhere in the middle. Holding a load at stall will quickly destroy a motor, especially those with small thermal mass (meaning small capacity to store or redirect heat). Very little work can be done at free speeds, since zero torque occurs at maximum speed.
