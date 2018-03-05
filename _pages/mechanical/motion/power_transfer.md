---
title: "Power Transfer"
permalink: /motion/power_transfer
sidebar:
  nav: mechanical_sidebar
toc: true
last_modified_at: 2018-03-05T16:03:57-05:00
---


For many mechanisms, it is convenient to locate the motor off of the mechanism proper. There are various methods to transfer power between two locations on a robot.

## Belt Drive

There are about 20 different belt standards available for use for power transmission. The most standardized belt drive used in FRC is the Gates 5mm HTD synchronous belt (timing belt).

Synchronous belts combine the torque tranmission ability of gear and chain drives with the easier direction and pliancy of flexible flat and v-belts, without stretch or slip.

There are two standard widths of HTD belt, 9mm and 15mm. The belt part number is normally order by width and length (i.e 1500-5M-09) for a 1500mm length (300 tooth) belt with a 9mm width. The 9mm width is rated for 600 pounds strength, and the 15mm width is rated for 1100 pounds, so either are more than adequate for robotics usage for all but the most high force applications.

HTD belts use a specific matched pulley profile. These are readily available for ordering, and can also be 3-D printed as well. Try to avoid the use of pulleys smaller than 24 Teeth as they will reduce belt life.

There are online belt calculators to aid with the design process and to help determine the appropriate center-distance and belt length needed for two given pulley sizes. For the simple case of two same sized pulleys add the full pitch diameter (as there are two "half pulleys") and double the center distance to find the closest stock belt. Adjust the center distance as needed to match the nearest stock belt size.

## Chain Drive

Chain and sprocket drives are familiar to all, and are very similar to those used on bicycles. Sprockets and chains are widely available, and are used by many FRC teams.

Sprockets are typically available in teeth counts between 10 and 60. They come with several different mounting options and additional available hubs; to allow attachment in just about any situation. There are different sprockets for the two common chain types.

There are two common sizes of chain used in robotics #25 and #35. #35 chain is over twice as heavy but considerably stronger than #25. Unless specially needed for strength, use the lighter #25 chain.

Chain|Pitch (Inches)|Roller Size (Inches)|Width (inches)|Weight (lbs. / ft)|Tensile Strength (lbs)
--|--
ANSI #25|1/4|0.130|1/8 |0.104|780
ANSI #35|3/8|0.200|3/16|0.250|1760

Roller chain is ordinarily completed using a master link (also known as a connecting link), which typically has one pin held by a horseshoe clip rather than friction fit, allowing it to be inserted or removed with simple tools. Chain with a removable link or pin is also known as cottered chain, which allows the length of the chain to be adjusted. Half links (also known as offsets) are available and are used to increase the length of the chain by a single roller rather than two.

With the rise in popularity of the Dark Souls chain breaker, master links have virtually disappeared in competition robotics. Instead of using a master link, Dark Souls-style chain breakers, such as those sold by Vex, push out the friction-fit pin in the chain itself, and allow it to be reattached at the desired length.

In use, chain will stretch in length. The design should either have an adjustable center distance, or a chain tensioner built into the design. There are a number of sprocket center distance and chain length calculators available on the internet to aid the design process.

## Polycord

Polycord (urethane round belting) is a hollow core flexible tube that can be cut to length and the ends joined either with a connector or welded together with a heat. Heat welding is often much more durable, and the equipment to do so is a wise investment for any team.

The belt is simply driven by round pulleys that can either be machined out of plastic or 3D printed.

Polycord is ideal for lower torque requirements such as intake roller systems. Polycord belting comes in a variety of sizes, with 3/16, 1/4, and 5/16 being most typically used. It is normally finished a bit short, and stretched over the pulleys to keep it taut and prevent slippage.

## Spur Gears
For short distances, spur gears can be used to transfer power. The largest commonly available gear is an 84 Tooth (14.5 degree pressure angle, 20DP) from Vex. Without intermediate shafting, it would limit the center distance range to 4.2 inches or less. See the [Gearing section]({{ '/motion/gears' | relative_url }}) for more spur gear information.
