---
title: "Motors"
permalink: /motion/motors
sidebar:
  nav: mechanical_sidebar
toc: true
last_modified_at: 2018-03-03T15:10:36-05:00
---

DC motors are an integral part of competition robotics, and proper motor selection is essential to successful robot design. FIRST competitions have limits on which motors may be used and how many (FRC Rule R29). Consult the game manual each year to insure the motors and specific part numbers are permitted.

To help select proper motors for mechanisms, a table with specifications of popular motors is below. This table contains mostly experimental data from VEX, which can be found [here](http://motors.vex.com/#testing). VEX Robotics motor curves were developed experimentally using a "down-up" dyno test, an industry-standard measurement system which helps to correct for rotational inertia. This data is more useful for comparison than nominal specifications due to its common method of measurement.


Motor|Free Speed (RPM)|Free Current (A)| Maximum Power (W)|Stall Torque (Nm)|Stall Current(A)|Price ($)
--------------------|-------|-----|-----|------|-----|-----
[CIM](#cim)                           | 5330  | 2.7 | 337 | 2.41 | 131 | 27.99
[Mini CIM (Vex)](#mini_cim)           | 5840  | 3.0 | 215 | 1.41 | 89  | 24.99
[BAG (Vex)](#bag)                     | 13180 | 1.8 | 149 | 0.43 | 53  | 24.99
[775pro (Vex/WCP)](#775pro)           | 18730 | 0.7 | 347 | 0.71 | 134 | 17.99
[Redline* (AndyMark)](#redline)       | 18730 | 0.7 | 347 | 0.71 | 134 | 18.00
[9015 (AndyMark)](#9015)              | 14270 | 3.7 | 134 | 0.36 | 71  | 14.00
[NeveRest** (AndyMark)](#neverest)    | 5480  | 0.4 | 25  | 0.17 | 10  | 18.00
[RS-775-125 (AndyMark)](#rs775_125)   | 5800  | 1.6 | 43  | 0.28 | 18  | 18.00
[RS-775-5*** (AndyMark)](#rs775_5)    | 5700  | 1.5 | 36  | 0.25 | 22  | 18.00
[Snow Blower (Andymark)](#snow_blower)| 100   | 5   | 20  | 8    | 24  | 39.00
[RS-775 18V (BaneBots)](#rs775_bb)    | 13050 | 2.7 | 246 | 0.72 | 97  | 17.50
[RS-550 (BaneBots)](#rs550_bb)        | 19000 | 0.4 | 190 | 0.38 | 84  |  7.25

\* Interchangable with the Vex/WCP 775pro. Information used here from 775pro testing.

\*\* Price is $10 without encoder.

\*\*\* Specifications are nominal (not measured)

## Key Characteristics of DC Motors

Four key characteristics are used to define a motor's performance. When designing a mechanism, all tradeoffs must be considered for the particular application.

* **Free Speed** (RPM) – The maximum speed at which a motor will rotate when under no load
* **Free Current** (A) – The minimum current a motor will draw when under no load
* **Stall Torque** (Nm) – The amount of load placed on a motor that will cause it to stall (stop moving)
* **Stall Current** (A) – The amount of current drawn by a motor when it is stalled

Under no load, "free", a motor spins at its **free speed** and draws a **free current**. Conversely, **stall torque** and **stall current** represent a motor being worked to its maximum, or "stalled", to the point at which it can no longer move.

These characteristics represent the theoretical minimum and maximum conditions for a motor.

Motors generally should not be run at these edge conditions, so usage in mechanisms should be optimized somewhere in the middle. Holding a load at stall will quickly destroy a motor, especially those with small thermal mass (meaning small capacity to store or redirect heat). Very little work can be done at free speeds, since zero torque occurs at maximum speed.

## Direct Comparison

For comparison purposes, it is useful to consider torque when 80% operating speed is reduced to 200 rpm output speed. Typical DC motor efficiency is highest near this range.

### CIM Motor (CCL)
{: #cim }

Motor|Free Speed (RPM)|Free Current (A)| Maximum Power (W)|Stall Torque (Nm)|Stall Current(A)
--|--
CIM | 5330  | 2.7 | 337 | 2.41 | 131

Geometry|
-----|----
Mounting|	2x 10-32 UNF tapped holes on 2" bolt circle
Output Shaft|	8 mm Shaft w/ 2mm Keyway
Weight|	2.8 Pounds

Largest DC motor permitted under current rules. In past years, these motors were limited to 6 per robot, though this restriction has been lifted. These are almost always used for the drive train power.

Its 80% speed is 4248 rpm (28.8 amps). With a 21.24 gear ratio its output would be 90.6 inch-pounds. at 200 rpm.

### Mini CIM Motor (Vex)
{: #mini_cim }

Motor|Free Speed (RPM)|Free Current (A)| Maximum Power (W)|Stall Torque (Nm)|Stall Current(A)
--|--
Mini CIM        | 5840  | 3.0 | 215 | 1.41 | 89

Geometry|
-----|----
Mounting|	2x 10-32 UNF tapped holes on 2" bolt circle
Output Shaft| 8 mm Shaft w/ 2mm Keyway
Weight	|2.16 Pounds
Second largest DC motor permitted under current rules.

Its 80% speed is 4272 rpm (20.2 amps). With a 23.36 gear ratio its output would be 57.9 inch-pounds at 200 rpm.

### BAG Motor (Vex)
{: #bag }

Motor|Free Speed (RPM)|Free Current (A)| Maximum Power (W)|Stall Torque (Nm)|Stall Current(A)
--|--
BAG (Vex)             | 13180 | 1.8 | 149 | 0.43 | 53  | 24.99

Geometry|
-----|----
Mounting|	2x M4 tapped holes on 25mm bolt circle
Output Shaft|	4 mm Shaft
Weight|	0.71 Pounds

Comparable to the Banebot RS550, nice small motor for intake systems and other low current and low torque needs.

Its 80% speed is 10544 rpm (12.04 amps). With a 57.72 gear ratio its output would be 36.9 inch-pounds at 200 rpm.

### 775 Pro Motor (Vex, West Coast Products)
{: #775pro }

Motor|Free Speed (RPM)|Free Current (A)| Maximum Power (W)|Stall Torque (Nm)|Stall Current(A)
--|--
775pro (Vex/WCP)      | 18730 | 0.7 | 347 | 0.71 | 134

Geometry|
--|--
Mounting| 2x M4 tapped holes on 29mm bolt circle
Output Shaft| 5 mm Shaft
Weight| 0.8 Pounds

Relatively new high speed and high torque motor. This is interchangable with the Andymark Redline.

Its 80% speed is 14984 rpm (26.9 amps). With a 74.92 gear ratio its output would be 94.1 inch-pounds at 200 rpm.

### Redline (Andymark)
{: #redline }

Motor|Free Speed (RPM)|Free Current (A)| Maximum Power (W)|Stall Torque (Nm)|Stall Current(A)
--|--
775pro (Vex/WCP) | 18730 | 0.7 | 347 | 0.71 | 134

Geometry|
--|--
Mounting| 2x M4 tapped holes on 29mm bolt circle
Output Shaft| 5 mm Shaft
Weight| 0.8 lbs

New high speed and high torque motor. This is interchangable with the Vex/WCP 775pro. Motor information taken from Vex's 775pro data.

Its 80% speed is 14984 rpm (26.9 amps). With a 74.92 gear ratio its output would be 94.1 inch-pounds at 200 rpm.

### 9015 Motor (AndyMark)
{: #rs775_125 }

### NeveRest Motor (AndyMark
{: #neverest }

Motor|Free Speed (RPM)|Free Current (A)| Maximum Power (W)|Stall Torque (Nm)|Stall Current(A)
--|--
NeveRest** (AndyMark) | 5480  | 0.4 | 25  | 0.17 | 10


Geometry|
--|--
Mounting|			3x M2-0.4 x 22mm deep
Output shaft| 12 tooth pinion gear for NeveRest Gearboxes
Weight| 0.550 lbs

Its 80% speed is 5280 RPM. 20:1 reduction gearbox yields a stall torque of 197 oz-in and free speed of 275-315 RPM. 40:1 yields a 350 oz-in stall torque and free speed of 160 rpm. 60:1 yields a stall torque of 593 oz-in and free speed of 105 RPM.

### RS775-125 (AndyMark)
{: #rs775_125 }

Motor|Free Speed (RPM)|Free Current (A)| Maximum Power (W)|Stall Torque (Nm)|Stall Current(A)
--|--
RS-775-125 (AndyMark)  | 5800  | 1.6 | 43  | 0.28 | 18  |

Geometry|
--|--
Mounting| 2x M3 tapped holes on 25mm bolt circle
Output Shaft| 11 tooth pinion gear for PG27 gearboxes
Weight| 0.78 Pounds

Primarily sold with the PG27 planetary gearbox, the raw shaft is 0.125 inches without the pinion.

Its 80% speed is 4560 rpm (5.6 amps). With a 22.8 gear ratio its output would be 1.13 Nm at 200 rpm.

### RS775-5 (AndyMark)
{: #rs775_5 }

Motor|Free Speed (RPM)|Free Current (A)| Maximum Power (W)|Stall Torque (Nm)|Stall Current(A)
--|--
RS775-5 (AndyMark)|5,700|1.5 Amps|?|0.25|22

Geometry|
--|--
Mounting|	2x M3 tapped holes on 25mm bolt circle
Output Shaft|	17 tooth pinion gear for PG188 & PG71 gearboxes
Weight|	0.81 Pounds

Primarily offered with the PG188 and PG71 gearboxes. The raw shaft is 5 mm without the pinion gear.

Its 80% speed is 4560 rpm (5.6 amps). With a 22.8 gear ratio its output would be 1.10 Nm at 200 rpm.

### Snow Blower (AndyMark)
{: #snow_blower }

Motor|Free Speed (RPM)|Free Current (A)| Maximum Power (W)|Stall Torque (Nm)|Stall Current(A)
--|--
Snow Blower (Andymark)| 100   | 5   | 20  | 8    | 24

Geometry|
--|--
Mounting| 3 x 10-32
Output Shaft| 10 mm DD Hub
Weight| 1.1 Pounds

The Snow Blower motor contains a built-in worm-gear transmission, and is ideal for very slow turning outputs.

It 80% speed is 80 rpm (8.8 amps). With a 0.40 gear ratio its output would be 0.621 Nm at 200 rpm.

### RS-775 18V (Banebots)
{: #rs775_bb }
##### (M7-RS775-18)

Motor|Free Speed (RPM)|Free Current (A)| Maximum Power (W)|Stall Torque (Nm)|Stall Current(A)
--|--
RS-775 18V (BaneBots)   | 13050 | 2.7 | 246 | 0.72 | 97

Geometry|
--|--
Mounting|	2x M4 tapped holes on 25mm bolt circle
Output Shaft|	5 mm Shaft
Weight|	0.74 Pounds

Its 80% speed is 10440 rpm (28 amps). With a 52.2 gear ratio its output would be 108.7 inch-pounds at 200 rpm.

### RS-550 (BaneBots)
{: #rs550_bb }
##### (M5-RS550)

Motor|Free Speed (RPM)|Free Current (A)| Maximum Power (W)|Stall Torque (Nm)|Stall Current(A)
--|--
RS-550 (BaneBots)        | 19000 | 0.4 | 190 | 0.38 | 84  |  7.25

Geometry|
--|--
Mounting|	2x M4 tapped holes on 25mm bolt circle
Output Shaft|	0.125 inch Shaft
Weight|	0.74 Pounds

Its 80% speed is 15440 rpm (28 amps). With a 77.2 gear ratio its output would be 66.4 inch-pounds at 200 rpm.


### Ancillary Motors
All automotive throttle control, window, door, windshield wiper, and seat motors are normally legal. Integrating these into standard robot gearboxes or shafts can be challenging. However there an enormous number of potential solutions in this huge range of options.
