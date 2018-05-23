---
layout: project
title: Dissecting Microscope Illumination
date: 11 May 2018
tags: [LED, Illumination]
screenshot:
  src: /ONECoreSite/assets/img/projects/Curtain1.png
  srcset:
    1920w: /ONECoreSite/assets/img/projects/MicroscopeLED/LED.jpg
    960w: /ONECoreSite/assets/img/projects/MicroscopeLED/LED.jpg
    480w: /ONECoreSite/assets/img/projects/MicroscopeLED/LED.jpg
caption: Illuminate your research!
description: >
    Illuminate your research!
---
# Intro

Viewing objects under a dissecting microscope requires a lot of optical power. Current-off-the-shelf products (including the old goose neck systems) are inefficient, often not true white, and are expensive. Here is an inexpensive (!), closer-to-true white light source that can fit on most dissecting microscopes.

This is a remix from a design shared by Thingiverse user bmv234, [Universal LED Ring Light Mount](https://www.thingiverse.com/thing:2548178). The design given here emphasizes minimal printing time and material, ease of function and assembly (no trying to 3D print screws), and increasing optical power. The dirt cheap LED sources are LED rings that kids use to 'soup up their cars' whatever that means, but hey, cheap tools. A inexpensive switch allows for on/off functionality with a simple (capacitance) touch, and dimming with prolonged touch. An inexpensive wall plug provides the DC current needed (think about how to specify a DC Power source [here](/ONECoreSite/projects/DCPowerSources)). Some 3D printed components are given, which hold the LED rings and protect the 'scope from scratching.

Need MOAR light? These are crazy bright, but OK. There are two designs given: one system with one LED ring. Another with two LED rings, one offset from the other, but the light is still well dispersed and centered. Need EVEN MOAR LIGHT? That's just crazy and you are on your own.

*Note: These are really bright. I recommend that you do not look directly at them. Point them at the wall when you first turn them on*

---
# Parts

Here is a list of the parts:

| Part | Supplier | Estimated Cost | Note |
| --- | --- | --- | --- |
| [1pair Bright White 100mm Angel Eyes 33 SMD LED Ring Car Light](https://www.aliexpress.com/item/B86-Hot-2Pcs-Bright-White-100mm-Angel-Eyes-33-SMD-LED-Ring-Car-Light/32777360207.html?spm=a2g0s.9042311.0.0.lUEUOp) | Aliexpress | 3.15 | There are two in the package |
| [Touch LED Dimmer Touch Switch Brightness with DC Female Male Plug for Single Color LED Strip Lamp DC 12V-24V 3A Black/White](https://www.aliexpress.com/item/DC-12V-24V-4A-LED-Strip-Connector-Touch-Dimmer-Brightness-Control-Switch-1-Keys-Dimmer-Light/32818464433.html?spm=2114.search0104.3.9.1d60d994OsDSy1&ws_ab_test=searchweb0_0,searchweb201602_2_10152_10151_10065_10344_10068_10130_5722815_10324_10342_10547_10325_10343_10546_10340_5722915_10548_10341_10545_5722615_10696_10084_10083_10618_10307_5722715_5711215_10059_308_100031_10103_10624_10623_10622_5711315_5722515_10621_10620,searchweb201603_2,ppcSwitch_4&algo_expid=8873c616-9647-467c-9751-c647bf9f3eca-1&algo_pvid=8873c616-9647-467c-9751-c647bf9f3eca&priceBeautifyAB=0) | Aliexpress | 1.89 | NA |
| [Black 12V 2V US DC power Aaptor 5.5*2.1mm 5.5 2.5mm 1m cable EVD DVD LED light and Monitoring equipment power charger](https://www.aliexpress.com/item/Black-12V-2A-US-dc-power-adaptor-5-5-2-1mm-5-5-2-5mm-1m/32799447713.html) | Aliexpress | 3.57 | See above for DC power supply discussion |
| M3 Screw | McMaster Part: 92005A128 | 3.16 | You get 100 of these, you'll need 3. But I try to use this size in lots of my designs, so look around for other ways to use these here! |
| M3 Nut | McMaster Part: 90592A085	 | 0.88 (really?) | You get 100 of these, you'll need 3. But I try to use this size in lots of my designs, so look around for other ways to use these here! |
| 3D printed parts | ONE Core??? | Not sure, [contact us!](mailto:neuralengineering@ucdenver.edu) | NA |

Here is a list of 3D Printed Components. All were printed successfully with nGen, 20% infill, no supports, except the 2LED system. First choose if you are going to use one or two LED rings. Then estimate if you have a relatively large or smaller microscope to choose short or long soft tips. They are small parts and you could probably just print them all and see. You will need three soft tips per unit.

| Name | Design | File Type | Use |
| --- | --- | --- | --- |
| [Minimal LED holder](https://github.com/OptogeneticsandNeuralEngineeringCore/MicroscopeLED/raw/master/Minimal%20LED%20holder.ipt) | 1 LED | .ipt | Holds the LED |
| [Minimal LED holder](https://github.com/OptogeneticsandNeuralEngineeringCore/MicroscopeLED/raw/master/Minimal%20LED%20holder.stl) | 1 LED | [.stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MicroscopeLED/blob/master/Minimal%20LED%20holder.stl) | Holds the LED |
| [SoftTipLong](https://github.com/OptogeneticsandNeuralEngineeringCore/MicroscopeLED/raw/master/SoftTipLong.ipt) | Both | .ipt | Protects a small microscope |
| [SoftTipLong](https://github.com/OptogeneticsandNeuralEngineeringCore/MicroscopeLED/raw/master/SoftTipLong.stl) | Both | [.stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MicroscopeLED/blob/master/SoftTipLong.stl) | Protects a small microscope |
| [SoftTipShort](https://github.com/OptogeneticsandNeuralEngineeringCore/MicroscopeLED/raw/master/SoftTipShort.ipt) | Both | .ipt | Protects a larger microscope |
| [SoftTipShort](https://github.com/OptogeneticsandNeuralEngineeringCore/MicroscopeLED/raw/master/SoftTipShort.stl) | Both | [.stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MicroscopeLED/blob/master/SoftTipShort.stl) | Protects a larger microscope |
| [Minimal LED holder 2 LEDsys](https://github.com/OptogeneticsandNeuralEngineeringCore/MicroscopeLED/raw/master/Minimal%20LED%20holder%202%20LEDsys.ipt) | 2 LED | .ipt | Holds the LEDs |
| [Minimal LED holder 2 LEDsys](https://github.com/OptogeneticsandNeuralEngineeringCore/MicroscopeLED/raw/master/Minimal%20LED%20holder%202%20LEDsys.stl) | 2 LED | [stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MicroscopeLED/blob/master/Minimal%20LED%20holder%202%20LEDsys.stl) | Holds the LEDs |

Tools include: Soldering station, hot glue gun, Phillips screwdriver, wire strippers, shrink wrap, heat gun

---
# Assembly

1. If you bought the right size DC plug, simply plug the DC power supply to the Dimmer Switch. If you're like me and you don't listen to your [own advise](/ONECoreSite/projects/DCPowerSources), you bought a power supply with the wrong size barrel jack (thanks, Jack!). No biggie, simply cut and splice the wires together:
   1. Cut and strip the wires
   2. Insert heat shrink over the wire
   3. Check the orientation of the dimmer (!). The circle end should go to power supply and the flat line should face the LEDs, as shown in the pic
   4. Twist the wires together. Put the jackets together, and angle the wires away from each other at ~45*, so it forms a 'Y'. Then twist together. Solder together.
   ![Twisted](/ONECoreSite/assets/img/projects/MicroscopeLED/Twisted.png "Twisted")
   5. Heat shrink each wire individually
   ![ShrinkIndivi](/ONECoreSite/assets/img/projects/MicroscopeLED/ShrinkIndivi.jpg "ShrinkIndivi")
   6. Place the two wires together and bend them to one direction so the entire assembly appears as one line. Shrink wrap
   ![ShrinkTogeth](/ONECoreSite/assets/img/projects/MicroscopeLED/ShrinkTogeth.jpg "ShrinkTogeth")   

 2. The LEDs come with bare wire. So the easiest thing to do is cut the plug off of the dimmer switch. This also allows you to add additional wire for a longer cable. Get good, solid, isolated connections using the ideas in 1 above.

 3. Clear the holes in the LED holder such that M3 screws can slide through easily. Grab three M3 nuts and throw them into the LED holder. Then insert screw the screws in. No glue is required. Then screw on the soft tips. Test sizing on the microscope.
 ![SoftTip](/ONECoreSite/assets/img/projects/MicroscopeLED/SoftTip.png "SoftTip")

 4. Attach the LED ring to the LED holder with a liberal amount of hot glue (why is it I can rock a soldering iron no problem, but can't hot glue without burning myself???). Then attach the set up to the microscope.

 **Note, it's probably a good idea to put a 1000uF capacitor between the positive and the negative terminals just before the LED ring to prevent large spikes of current (during on/off) from damaging the LEDs, but I haven't yet seen issue.**

 The two LED system requires a bit more thought. I originally thought I would just push more voltage into the system, to see if I could get more light or blow up the system. But really, it didn't seem to do much other than throw more heat. I then thought I'd hook up two rings in series, but that didn't seem to work either, probably because of forward voltage or some other EE non-sense. So I tried them in parallel, and that works great. Note that each ring draws about 0.15 Amps of current. Hooking two up in parallel draws about 0.3 Amps, well below the max power specified by the DC power supply, so no worries there.

 1. Assembly of the two LED system is similar to the one LED system, but with two LEDs in parallel. To do that, simply have all the red wires together and all the black wires together. It's a good idea to strip more jacket off so you can twist together three wires.
 ![2LED](/ONECoreSite/assets/img/projects/MicroscopeLED/2LED.jpg "2LED")
---
# Keep going!
Need to take pictures or videos of what is happening under the 'scope? Hate holding up your phone to try and get a pic? Check out [this project](/ONECoreSite/projects/MicroscopeCamera)!

***

# ONE Core acknowledgement
Please acknowledge the ONE Core facility in your publications. An appropriate wording would be:

*"Engineering support was provided by the Optogenetics and Neural Engineering Core at the University of Colorado Anschutz Medical Campus, funded in part by the National Institute of Neurological Disorders and Stroke of the National Institutes of Health under award number P30NS048154."*
