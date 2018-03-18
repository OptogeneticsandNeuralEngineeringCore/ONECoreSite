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
    Here are some hopeful improvements to the MiniScope Project, allowing for single cell resolution of awake behaving animals.
links:
  - title: Download All
    url: https://github.com/OptogeneticsandNeuralEngineeringCore/MicroscopeCamera/archive/later.zip
  - title: Source
    url: https://github.com/OptogeneticsandNeuralEngineeringCore/later
---

# Introduction

Here are some project ideas to help advance the *amazing* [MiniScope project](http://miniscope.org/index.php/Main_Page). Single cell resolution on behaving animal on the cheap? Yes plz. More to come.

***

# DAQ housing

![DAQ](/ONECoreSite/assets/img/projects/MiniScope/DAQ.jpg "DAQ Housing")

The original DAQ housing, at the time of writing, has errors in the STL (I couldn't get it into my slicing Software). Here is a quick update to the housing that emphasizes minimal print volume and writes the DAQ inputs and outputs within the housing. It prints well with clear nGen, 40% infill, no supports necessary. You may need to rotate in your slicing software. Assemble with pan head M3 screws, 20 mm long. The current DAQ PCB only has one through hole for seating. This is...odd, but this design conforms.

| File | Description | File Type  |
| --- | --- | --- |
| [Redid DAQ Enclosure Bottom.ipt](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/Redid%20DAQ%20Enclosure%20Bottom.ipt) | DAQ Enclosure Bottom | ipt |
| [Redid DAQ Enclosure Bottom.stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/Redid%20DAQ%20Enclosure%20Bottom.stl) | DAQ Enclosure Bottom | [stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/blob/master/Redid%20DAQ%20Enclosure%20Bottom.stl) |
| [Redid DAQ Enclosure Top.ipt](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/Redid%20DAQ%20Enclosure%20Top.ipt) | DAQ Enclosure Top | ipt |
| [Redid DAQ Enclosure Top.stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/Redid%20DAQ%20Enclosure%20Top.stl) | DAQ Enclosure Top | [stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/blob/master/Redid%20DAQ%20Enclosure%20Top.stl) |


Don't have an FDM printer? You can upload these to 3DHubs. Or support the [ONE Core](mailto:neuralengineering@ucdenver.edu) and order though us!!!!

***

# Miniscope Holders

![Stereotaxic Holder](/ONECoreSite/assets/img/projects/MiniScope/2Axis.jpg "Stereotaxic")

How do you hold the MiniScope during implantation? There are holders out there for current commercial imaging microscopes, but they are expensive (!). Hold your Miniscope with these inexpensive FDM 3D printed holders! They assemble with M3 Screws and nuts, and do not require any glue or otherwise to assemble. Two flavors are given: one that simply attaches to a basic 6mm stereotaxic rod at 90 degrees, and another that attaches to a ball on the end of a 6 mm rod (place into your stereotaxic equipment), allowing you some rotation around two axis (McMaster PN 6402K12). Some researchers needed a cup think to increase the diameter of the rod to fit into their stereotaxic equipment, so that is there as well. You can keep wires out of the way by fitting them into the holes on top of the parts. I like nGen, 40% infill (maybe more on the ball system), no supports necessary.

Note: in order for the system to accept the ball, still be flexible, the parts are kind of thin. I've found it helpful to print it out, then hit it quick with a heat gun before I insert the ball. I then let it cool. I hit it with the heat gun again, and pinch it snug around the ball with my fingers. Thermoplastics and all.

| File | Description | File Type  |
| --- | --- | --- |
| [Stereotaxic Miniscope Holder](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/StereotaxicNeuroprobeamajigerMiniscope.ipt) | Hold the Miniscope at 90* | ipt |
| [Stereotaxic Miniscope Holder](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/StereotaxicNeuroprobeamajigerMiniscope.stl) | Hold the Miniscope at 90* | [stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/blob/master/StereotaxicNeuroprobeamajigerMiniscope.stl) |
| [Stereotaxic Miniscope Holder with Angle](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/NeuroprobeholdermajigerV11MiniscopeAngle.ipt) | Hold the Miniscope at a variety of angles | ipt |
| [Stereotaxic Miniscope Holder with Angle](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/NeuroprobeholdermajigerV11MiniscopeAngle.stl) | Hold the Miniscope at a variety of angles | [stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/blob/master/NeuroprobeholdermajigerV11MiniscopeAngle.stl) |

More stereotaxic probes can be found [here](/ONECoreSite/projects/Neuroprobeamajiger).

***

# 3D Printed Head Mount MiniScope

![Head Mount](/ONECoreSite/assets/img/projects/MiniScope/Hand.jpg "Head Mount")

I redesigned the Head Mount system to allow for 3D printing. Unless you are super crazy good (like, world class), FDM printing will not be the way to go. microSLA or Polyjet would be the way to go. I have successfully printed these with a Projet1200 (set to Green resin settings) using Deep Black Resin from FunToDo. Of course, this voids the warrenty of the Projet, but the resin is over 10X less expensive, and you get to understand and play with the properties of the resin. Want to find out how to do this and how to fix the resin vats? Shoot me an email. This resin reportedly has less autoflourescence than Delrin.

All components fit with the original PCB, LED, and filters and use the same screws. The walls are thicker, because this plastic doesn't seem to block light as well, but the entire assembly is only .1 grams more. It has a smaller footprint, and therefore does not fit on the previous MS_Holders. It includes tick marks so you can know the height you have set the camera at. I've also included a 'trainer' scope that has the overall shape of the system, but doesn't require the other components. Glue some weight up on top to replicate that of the PCB (washers), glue or press fit in the magnets, and boom, now you can train the animal without risk of damage of the actual system.

Don't have these printers? Check out 3DHubs for a local printer or support the [ONE Core](mailto:neuralengineering@ucdenver.edu) and order though us!!!!

![Head Mount Blurry](/ONECoreSite/assets/img/projects/MiniScope/MiniScopeBlurry.jpg "Head Mount")

| File | Description | File Type  |
| --- | --- | --- |
| [Cover](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/Cover.ipt) | Miniscope Head Mount Cover | ipt |
| [Cover](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/Cover.stl) | Miniscope Head Mount Cover | [stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/blob/master/Cover.stl) |
| [Faceplatev11](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/Faceplatev11.ipt) | Miniscope Head Mount Faceplate | ipt |
| [Faceplatev11](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/Faceplatev11.stl) | Miniscope Head Mount Faceplate | [stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/blob/master/Faceplatev11.stl) |
| [MS_BasePlatev11](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/MS_BasePlatev11.ipt) | Miniscope Head Mount MS_BasePlate | ipt |
| [MS_BasePlatev11](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/MS_BasePlatev11.stl) | Miniscope Head Mount MS_BasePlate | [stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/blob/master/MS_BasePlatev11.stl) |
| [MS_FocusSliderv11](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/MS_FocusSliderv11.ipt) | Miniscope Head Mount MS_FocusSlider | ipt |
| [MS_FocusSliderv11](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/MS_FocusSliderv11.stl) | Miniscope Head Mount MS_FocusSlider | [stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/blob/master/MS_FocusSliderv11.stl) |
| [MS_Holderv11](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/MS_Holderv11.ipt) | Miniscope Head Mount MS_Holder | ipt |
| [MS_Holderv11](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/MS_Holderv11.stl) | Miniscope Head Mount MS_Holder | [stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/blob/master/MS_Holderv11.stl) |
| [Trainer](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/Trainer.ipt) | Miniscope Head Mount Trainer | ipt |
| [Trainer](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/raw/master/Trainer.stl) | Miniscope Head Mount Trainer | [stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MiniScope/blob/master/Trainer.stl) |



***

# ONE Core acknowledgement
Please acknowledge the ONE Core facility in your publications. An appropriate wording would be:

*"Engineering support was provided by the Optogenetics and Neural Engineering Core at the University of Colorado Anschutz Medical Campus, funded in part by the National Institute of Neurological Disorders and Stroke of the National Institutes of Health under award number P30NS048154."*
