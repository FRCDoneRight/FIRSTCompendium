---
title: "Bearings and Bushings"
permalink: /motion/bearings
sidebar:
  nav: mechanical_sidebar
---

Bearings and bushing are designed to constrain relative motion and reduce friction between rotating parts. There are a very wide variety of bearings available; those most commonly used in FRC designs are discussed below.

### Radial Ball Bearings

Radial ball bearing are the most common type of bearing used in products. Normally, radial bearings are constructed with ball grooves in both the inner and outer races, containing a number of ball bearings. These bearings generally need to be lubricated with grease, however in FRC we normally use sealed bearings, which are pre-lubricated. Radial ball bearing are designed for radial loads, and some smaller axial loads.

Because nearly all COTS gearboxes and wheels are designed around 1/2" hex or round shaft, the use of the deep groove inch size “R” bearings is an obvious choice. They are available with flanges (FR, typically used) and without (R) flanges. The most common used R8 size (1/2 inch ID, 1 1/8 inch OD) bearing, which are rated for 1000 pounds radial load, and about 250 pound axial load. The most typically used FRC bearings are listed below, with IDs from common vendors.

#### Typical Bearings Used (R Inches Series)

Outer Diameter | Inner Diameter | Identifier | VexPro ID | Andymark ID
---------------|----------------|------------|-----------|------------
0.875"         | 0.375" hexagon | FR6ZZ-Hex  | N/A       | N/A
0.875"         | 0.375" round   | FR6ZZ      | 217-2733  | am-0028
1.125"         | 0.375" hexagon | FR6ZZL-Hex | 217-2735  | am-0692
1.125"         | 0.500" hexagon | FR8ZZ-HEX  | 217-3875  | am-2986
1.125"         | 0.500" round   | FR8ZZ      | 217-2731  | am-0030

##### Thunderhex

ThunderHex stock works in all applications where 1/2" or 3/8" shaft will work, and also includes rounded corners. These rounded corners allow the shaft to pilot inside a 13.75 mm round (ThunderHex) Bearing instead of a standard 1/2" Hex Bearing, eliminating some difficult manufacturing tolerances and results in a smoother end result. A similar effect can be achieved with hex stock and a lathe.

##### Seal Types

Open bearings dissipate heat more efficiently than shielded and sealed bearings.

Shielded bearings block out dust and other contaminants, but do not dissipate heat as efficiently as open bearings. These are the most common in FRC conditions.

Sealed bearings block out dust and other contaminants better than open and shielded bearings, but retain the most heat.

#### Needle Roller Bearings

A needle roller bearing uses small cylindrical rollers rather than balls. Needle bearings can only be used for round shafts, but offer high radial load capacity in a smaller outside diameter package than with standard roller bearings. The small OD size can be advantageous when space is at a premium, such as supporting an inner shaft on a coaxial swerve drive.

#### Thrust Bearings

In locations where an axial load is applied, a thrust bearing is used to reduce friction. Depending on the load, there are thrust bearings with needle or ball bearings. For smaller loads a simple "washer style" type of bearing (similar to a bushing) made with bronze, Oilite, Teflon, or another plastic is sufficient.

#### Tapered Ball & Roller Bearings

Tapered bearings are designed for both axial and radial loads. These bearings are used on automobile wheels, and also used in the old cup and cone style bicycle wheels. The axial preload on the bearing needs to be adjustable. These are not commonly used in robotics due to the high cost and installation complexity of these bearings. For combined axial and radial loads, FRC teams typically instead use a combination of a radial bearing and a thrust bearing.

### Bushings

Bushing are similar to bearings, but lack any roller elements. They are typically used in lower-speed applications and generally have slightly higher friction. Bushings are widely available in bronze, Oilite, PFTE (Teflon), Nylon, and other plastics.

## Addendum

#### Precision (ABEC-rated) Bearings

Precision bearings are uncommon for general FRC usage, but provide a high tolerance and similar characteristics for a specific bearing (i.e. two bearings from the same rating must be very similar). Most bearings from common FRC suppliers are "standard" - meaning that they have undefined and very large possible tolerances. Precision bearings are rated using a scale from largest to smallest tolerances: ABEC 1, 3, 5, 7, 9, etc, where higher ABEC classes provide better precision, efficiency, and other requirements.

There are a number of factors covered by the ABEC grades. Arguably, the most important is the eccentricity (roundness) of the track in the inner ring, which determines run-out. The figures given below show the maximum eccentricity allowable.

Rating  | Max. Eccentricity (in) | Max. Eccentricity (mm)
--------|------------------------|----------------
ABEC 1  | 0.000295"              | 0.0075 mm
ABEC 3  | 0.000197"              | 0.0050 mm
ABEC 5  | 0.000138"              | 0.0035 mm
ABEC 7  | 0.000098"              | 0.0025 mm
ABEC 9  | 0.000047"              | 0.0012 mm
ABEC 11 | 0.0000235"             | 0.0006 mm
ABEC 13 | 0.00001175"            | 0.0003 mm
