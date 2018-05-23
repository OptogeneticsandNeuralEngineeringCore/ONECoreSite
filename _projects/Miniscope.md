---
layout: project
title: MiniScope
date: 12 March 2018
tags: [MiniScope, 3D printing, FDM, SLA]
screenshot:
  src: /ONECoreSite/assets/img/projects/MiniScope/Hand.jpg
  srcset:
    1920w: /ONECoreSite/assets/img/projects/MiniScope/Hand.jpg
    960w: /ONECoreSite/assets/img/projects/MiniScope/Hand.jpg
    480w: /ONECoreSite/assets/img/projects/MiniScope/Hand.jpg
caption: Some hopeful improvements to the MiniScope Project
description: >
    Here are some improvements to the MiniScope Project, allowing for single cell resolution of awake behaving animals.
links:
  - title: Download All
    url: https://github.com/OptogeneticsandNeuralEngineeringCore/MicroscopeCamera/archive/later.zip
  - title: Source
    url: https://github.com/OptogeneticsandNeuralEngineeringCore/later
---

# MiniScope

Here are some project ideas to help advance the *amazing* [MiniScope project](http://miniscope.org/index.php/Main_Page). Single cell resolution on behaving animal on the cheap? Yes plz.

***

# DAQ housing

![DAQ](/ONECoreSite/assets/img/projects/MiniScope/DAQ.jpg "DAQ Housing")

The original DAQ housing, at the time of writing, has errors in the STL (I couldn't get it into my slicing Software). Here is a quick update to the housing that emphasizes minimal print volume and writes the DAQ inputs and outputs within the housing. It prints well with nGen, 40% infill, no supports necessary. Assemble with pan head M3 screws, 20 mm long (McMaster 92005A128), no nuts or glue is necessary. The current DAQ PCB only has one through hole for seating. This is...odd, but this design conforms.

There is a new design for allowing for a BNC Connector so that you can trigger the camera with a [TTL](/ONECoreSite/projects/Arduino%20TTL%20Pulse%20Generator%20and%20Controller). More below.

| File | Description | File Type  |
| --- | --- | --- |
| [Redid DAQ Enclosure Bottom.ipt](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/Redid%20DAQ%20Enclosure%20Bottom.ipt) | DAQ Enclosure Bottom | ipt |
| [Redid DAQ Enclosure Bottom.stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/Redid%20DAQ%20Enclosure%20Bottom.stl) | DAQ Enclosure Bottom | [stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/blob/master/Redid%20DAQ%20Enclosure%20Bottom.stl) |
| [Redid DAQ Enclosure Top.ipt](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/Redid%20DAQ%20Enclosure%20Top.ipt) | DAQ Enclosure Top | ipt |
| [Redid DAQ Enclosure Top.stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/Redid%20DAQ%20Enclosure%20Top.stl) | DAQ Enclosure Top | [stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/blob/master/Redid%20DAQ%20Enclosure%20Top.stl) |
| [Redid DAQ Enclosure Bottom TTL.ipt](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/Redid%20DAQ%20Enclosure%20Bottom%20TTL.ipt) | DAQ Enclosure Bottom TTL | ipt |
| [Redid DAQ Enclosure Bottom TTL.stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/Redid%20DAQ%20Enclosure%20Bottom%20TTL.stl) | DAQ Enclosure Bottom TTL | [stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/blob/master/Redid%20DAQ%20Enclosure%20Bottom%20TTL.stl) |
| [Redid DAQ Enclosure Top TTL.ipt](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/Redid%20DAQ%20Enclosure%20Top%20TTL.ipt) | DAQ Enclosure Top TTL | ipt |
| [Redid DAQ Enclosure Top TTL.stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/Redid%20DAQ%20Enclosure%20Top%20TTL.stl) | DAQ Enclosure Top TTL | [stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/blob/master/Redid%20DAQ%20Enclosure%20Top%20TTL.stl) |

Don't have an FDM printer? Support the [ONE Core](mailto:neuralengineering@ucdenver.edu) and order though us!!!! Or use an inexpensive outside 3D printing shop. [Rosenberg Industries](mailto:j.rosenberg@rosenbergindustries.com) is aware of ONE Core projects and requirements  and has proven success with ONE Core projects.

***

# Trigger Input
"In the 3.2 version of the DAQ PCB the "trigger in" port isn't one of the 2 ports that come assembled with an SMA connector. Here, http://imgur.com/a/hgzua, is a picture of where the connections of this port are located. You can solder one of these coax cables, https://www.digikey.com/products/en?keywords=0897611670, to the 2 pads and then run it out of the DAQ Box." -Daniel Aharoni June 15th, 2017, MiniScope forum

I have made an update to the DAQ housing to reliably hold a BNC Connector (TE Connectivity PN 5227726-1, Mouser [571-5227726-1](https://www.mouser.com/ProductDetail/571-5227726-1)). To assemble, cut and strip some 22 gauge single core wire. Take the BNC connector and bend out the ground pin a bit. Hook the ground wire through the hole and pinch it tight with pliers. Insert the signal wire in the center and pinch close with pliers.

![BNC Solder](/ONECoreSite/assets/img/projects/MiniScope/BNC Solder.png "BNC Solder")

Hit it with *a lot* of heat and then some solder. Isolate the connections with some shrink wrap.

![BNC Shrink](/ONECoreSite/assets/img/projects/MiniScope/BNC Shrink.png "BNC Shrink")

Then, be sure to feed the assembly through the housing and the nut *before you solder the wires to the PCBA*. Else, you have to unsolder it to get it to assemble, not that I would know...

![TTL Over](/ONECoreSite/assets/img/projects/MiniScope/TTL Over.png "TTL Over")
![TTL Assembled](/ONECoreSite/assets/img/projects/MiniScope/TTL Assembled.png "TTL Assembled")

***

# Miniscope Holders

![Stereotaxic Holder](/ONECoreSite/assets/img/projects/MiniScope/2Axis.jpg "Stereotaxic")

How do you hold the MiniScope during implantation? There are holders out there for current commercial imaging microscopes, but they are expensive (!). Hold your Miniscope with these inexpensive FDM 3D printed holders! They assemble with M3 Screws and nuts, and do not require any glue or otherwise to assemble. Two flavors are given: one that simply attaches to a basic 6mm stereotaxic rod at 90 degrees, and another that attaches to a ball on the end of a 6 mm rod (place into your stereotaxic equipment), allowing you some rotation around two axis (McMaster PN 6402K12). Some researchers needed a cup  to increase the diameter of the rod to fit into their stereotaxic equipment, so that is there as well. You can keep wires out of the way by fitting them into the holes on top of the parts. I like nGen, 40% infill (maybe more on the ball system), no supports necessary.

Note: in order for the system to accept the ball, still be flexible, the parts are kind of thin. I've found it helpful to print it out, then hit it quick with a heat gun before I insert the ball. I then let it cool. I hit it with the heat gun again, and pinch it snug around the ball with my fingers. Thermoplastics and all.

| File | Description | File Type  |
| --- | --- | --- |
| [Stereotaxic Miniscope Holder](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/StereotaxicNeuroprobeamajigerMiniscope.ipt) | Hold the Miniscope at 90* | ipt |
| [Stereotaxic Miniscope Holder](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/StereotaxicNeuroprobeamajigerMiniscope.stl) | Hold the Miniscope at 90* | [stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/blob/master/StereotaxicNeuroprobeamajigerMiniscope.stl) |
| [Stereotaxic Miniscope Holder with Angle](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/NeuroprobeholdermajigerV11MiniscopeAngle.ipt) | Hold the Miniscope at a variety of angles | ipt |
| [Stereotaxic Miniscope Holder with Angle](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/NeuroprobeholdermajigerV11MiniscopeAngle.stl) | Hold the Miniscope at a variety of angles | [stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/blob/master/NeuroprobeholdermajigerV11MiniscopeAngle.stl) |
| [Stereotaxic Miniscope Holder with Angle 3D Design](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/NeuroprobeholdermajigerV11MiniscopeAngle43DScope.ipt) | Hold the Miniscope at a variety of angles | ipt |
| [Stereotaxic Miniscope Holder with Angle 3D Design](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/NeuroprobeholdermajigerV11MiniscopeAngle43DScope.stl) | Hold the Miniscope at a variety of angles | [stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/blob/master/NeuroprobeholdermajigerV11MiniscopeAngle43DScope.stl) |

More stereotaxic probes can be found [here](/ONECoreSite/projects/Neuroprobeamajiger).

Don't have an FDM printer? Support the [ONE Core](mailto:neuralengineering@ucdenver.edu) and order though us!!!! Or use an inexpensive outside 3D printing shop. [Rosenberg Industries](mailto:j.rosenberg@rosenbergindustries.com) is aware of ONE Core projects and requirements  and has proven success with ONE Core projects.

***

# 3D Printed Head Mount MiniScope

![Head Mount](/ONECoreSite/assets/img/projects/MiniScope/Hand.jpg "Head Mount")

I redesigned the Head Mount system to allow for 3D printing. Unless you are super crazy good (like, world class), FDM printing will not be the way to go. microSLA or Polyjet would be the way to go. I have successfully printed these with a Projet1200 (set to Green resin settings) using Deep Black Resin from FunToDo. Of course, this voids the warranty of the Projet, but the resin is over 10X less expensive, and you get to understand and play with the properties of the resin. Want to find out how to do this and how to fix the resin vats? Shoot me an [email](mailto:neuralengineering@ucdenver.edu). This resin reportedly has less autoflourescence than Delrin.

All components fit with the original PCB, LED, and filters and use the same screws. The walls are thicker, because this plastic doesn't seem to block light as well, but the entire assembly is only .1 grams more. It includes tick marks so you can know the height you have set the camera at. It has a smaller footprint, and therefore does not fit on the previous MS_Holders.

Don't have a microSLA printer? Support the [ONE Core](mailto:neuralengineering@ucdenver.edu) and order though us!!!! Or use an inexpensive outside 3D printing shop. [Rosenberg Industries](mailto:j.rosenberg@rosenbergindustries.com) is aware of ONE Core projects and requirements  and has proven success with ONE Core projects.

![Head Mount Blurry](/ONECoreSite/assets/img/projects/MiniScope/MiniScopeBlurry.jpg "Head Mount")

| File | Description | File Type  |
| --- | --- | --- |
| [Cover](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/Cover.ipt) | Miniscope Head Mount Cover | ipt |
| [Cover](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/Cover.stl) | Miniscope Head Mount Cover | [stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/blob/master/Cover.stl) |
| [Faceplatev11](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/Faceplatev11.ipt) | Miniscope Head Mount Faceplate | ipt |
| [Faceplatev11](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/Faceplatev11.stl) | Miniscope Head Mount Faceplate | [stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/blob/master/Faceplatev11.stl) |
| [MS_BasePlatev11](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/MS_BasePlatev11.ipt) | Miniscope Head Mount MS_BasePlate | ipt |
| [MS_BasePlatev11](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/MS_BasePlatev11.stl) | Miniscope Head Mount MS_BasePlate | [stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/blob/master/MS_BasePlatev11.stl) |
[MS_BasePlatewGrinHole](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/MS_BasePlatev11wGrinHole.ipt) | Miniscope Head Mount MS_BasePlatewGrinHole | ipt |
| [MS_BasePlatewGrinHole](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/MS_BasePlatev11wGrinHole.stl) | Miniscope Head Mount MS_BasePlatewGrinHole | [stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/blob/master/MS_BasePlatev11wGrinHole.stl) |
| [MS_FocusSliderv11](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/MS_FocusSliderv11.ipt) | Miniscope Head Mount MS_FocusSlider | ipt |
| [MS_FocusSliderv11](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/MS_FocusSliderv11.stl) | Miniscope Head Mount MS_FocusSlider | [stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/blob/master/MS_FocusSliderv11.stl) |
| [MS_Holderv11](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/MS_Holderv11.ipt) | Miniscope Head Mount MS_Holder | ipt |
| [MS_Holderv11](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/MS_Holderv11.stl) | Miniscope Head Mount MS_Holder | [stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/blob/master/MS_Holderv11.stl) |
| [Protector](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/Protector.ipt) | Miniscope Head Mount Protector | ipt |
| [Protector](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/Protector.stl) | Miniscope Head Mount Protector | [stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/blob/master/Protector.stl) |
| [Trainer](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/Trainer.ipt) | Miniscope Head Mount Trainer | ipt |
| [Trainer](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/Trainer.stl) | Miniscope Head Mount Trainer | [stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/blob/master/Trainer.stl) |

New components:
The baseplate with Grin Hole has hole on the side. With this you could use one of the 0-80 set screws to have the Miniscope hold into the Grin Lens. This may be required for use with future, longer grin lenses.

The Protector can be placed on top of the PCBA for extra protection. This additional weight may not be great for mice, but may be required for larger, more aggressive animals (prairie voles). It can be assembled with the given screws. Consider throwing a dab of hot glue on top to hold the coaxial cable better.

I've also included a 'trainer' scope that has the overall shape of the system, but doesn't require the other components. Glue some weight (washers) up on top to replicate that of the PCB, glue or press fit in the magnets, and boom, now you can train the animal without risk of damage of the actual system.

Assembly and Ramblings:
The cooner coaxial cable is crazy expensive. Alpha Wire [9438 WH033](https://www.digikey.com/product-detail/en/alpha-wire/9438-WH033/A9438W-10-ND/6003378) works just as well at a fraction of the price. Or, if you are using a larger animal, save yourself some head ache and go with a [larger cable](https://www.digikey.com/product-detail/en/alpha-wire/9434-WH033/A9434W-10-ND/6003374). The [Jonard Tools ST-450](https://www.digikey.com/product-detail/en/jonard-tools/ST-450/K545-ND/1990301) works well to strip these.

Because these parts are 3D printed, you will not have to clean the machined burrs out. But, because these are 3D printed, there may be some slight sagging of the very small holes. It is a good idea to clean them out prior to using any of the screws. Use a McMaster 2546A23 tap to hold onto [#61-80 wire gauge drill bits](https://www.amazon.com/gp/product/B000TY190C/ref=oh_aui_search_detailpage?ie=UTF8&psc=1) to clean up the holes.

***

# ONE Core acknowledgement
Please acknowledge the ONE Core facility in your publications. An appropriate wording would be:

*"Engineering support was provided by the Optogenetics and Neural Engineering Core at the University of Colorado Anschutz Medical Campus, funded in part by the National Institute of Neurological Disorders and Stroke of the National Institutes of Health under award number P30NS048154."*
