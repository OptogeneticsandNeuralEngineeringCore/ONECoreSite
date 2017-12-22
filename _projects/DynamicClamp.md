---
layout: project
title: Dynamic Clamp
date: 21 Dec 2017
tags: [3D Print, FDM, Teensy]
screenshot:
  src: /ONECoreSite/assets/img/projects/DynamicClamp/20171128_151640.jpg
  srcset:
    1920w: /ONECoreSite/assets/img/projects/DynamicClamp/20171128_151640.jpg
    960w: /ONECoreSite/assets/img/projects/DynamicClamp/20171128_151640.jpg
    480w: /ONECoreSite/assets/img/projects/DynamicClamp/20171128_151640.jpg
caption: Control your patch clamping like never before on the cheap
description: >
    A very inexpensive Teensy is placed on a breadboard with several other circuits to create a Dynamic Clamp with sufficient resolution and timing for controlling your patch clamp recordings.
links:
  - title: Download All
    url: https://github.com/OptogeneticsandNeuralEngineeringCore/DynamicClamp/archive/master.zip
  - title: Source
    url: https://github.com/OptogeneticsandNeuralEngineeringCore/DynamicClamp
---

# Dynamic Clamp Introduction

Patch clamp is vital to neuroscience and allows for direct recording and stimulation of neurons or membrane channels. Typically voltage clamp or current clamp is used to hold one constant while varying the other. An underutilized technique known as Dynamic Clamp can allow for more precise control. This configuration of patch clamp records the action potential (voltage) of the cell in real time and returns a specific, non-predetermined membrane current. Historically, such real time calculations have required the addition of very expensive equipment. Luckily, today microcontrollers are advanced and inexpensive enough for this application. Additionally, there is a great drive for sharing of designs, allowing for rapid advancement of science.

An open sourced (GNU General Public License (version 3, 29 June 2007) Dynamic Clamp system has been generously developed by Niraj Desai, et Al. The system (its function, its properties, and its place in contemporary neuroscience) is described in detail in this paper: *Niraj S. Desai, Richard Gray, and Daniel Johnston. A dynamic clamp on every rig. eNeuro (DOI:10.1523/ENEURO.0250-17.2017).* The website [Dynamic Clamp](http://www.dynamicclamp.com) includes detailed instructions on how to assemble and use the system. This system is inexpensive and simple enough for the average patch clamper with no previous experience in electronics or coding to be up and dynamically clamping in short order.

The Optogenetics and Neural Engineering (ONE) Core has advanced this dynamic clamp system. We have designed 3D printed enclosures to hold the assembly in an isolated and rigid manner. The circuit can be rearranged to fit onto a smaller breadboard, and can be soldered for ultimate rigidity.  We have created a spreadsheet to ease calculations during calibration.

****

# Versions

The current system as described by Dr. Desai is simply assembled in a solderless breadboard. This is a great way to begin electronics (and test the system), but it is very easy to create shorts or open circuits. The inexpensive resistors suggested are rather flimsy, and the wires in/out of the system (heavy BNC connectors) can easily be pulled out from the system. The ONE Core shows how to fabricate the system with two revisions. Each system can fit into a 3D printed enclosure (below) for solid connections in a transportable system.

* Easy: Build the system on a solderless breadboard, *similar* to the instructions on the original web site. By moving where circuits are connected on the breadboard (while maintaining the circuit configuration), a 'half size' breadboard can be used. Therefore a much smaller footprint is needed. The 3D printed enclosure will hold the breadboard, the Teensy, and rigidly BNC connectors. This isolates the circuits, well holds them, and gives rigid connections for the in/out through BNC connectors.
* Better: Build the system on a solder-able breadboard. The layout of the circuits will be the same as the easy method, but everything can be well attached through soldering. Don't know how to solder? It's super fun and easy to learn! [Sparkfun](https://learn.sparkfun.com/tutorials/how-to-solder-through-hole-soldering) has a great tutorial on soldering. This system will give you a much more rigid system. The 3D printed enclosure holds the breadboard, Teensy, and BNC connectors.
* Better-er (not best, there's always room for improvement): In the easy and better systems, the Teensy is not connected to the breadboard. In fact, the Teensy is, well, tiny, and therefore the design does not have through holes to attach to enclosures. Therefore, these designs require the Teensy be hot glued down to the enclosure. A better solution would be to attach the Teensy to the breadboard which has through holes. This solution is not much more difficult than the 'better' solution, but does require at least one more additional thought. This enclosure holds the breadboard, with the Teensy attached, and the BNC Connectors. This system is the smallest and most rigid.

Easy | Better | Better-er
:---: | :---: | :---:
![Easy Pic 1](/ONECoreSite/assets/img/projects/DynamicClamp/20171101_142630.jpg "Pic 1 Easy") | ![Better Pic 1](/ONECoreSite/assets/img/projects/DynamicClamp/20171101_153911.jpg "Pic 1 Better") | ![Better-er Pic 1](/ONECoreSite/assets/img/projects/DynamicClamp/20171125_123122.jpg "Pic 1 Better-er")

***

# Fabrication

* Easy: The large (solderless) breadboard listed in original paper can be replaced with a (solderless) breadboard half the size (Sparkfun  [PRT-12002](https://www.sparkfun.com/products/12002)). There is a large opportunity for shorts when the legs of components (ex: resistors) are long, so it is wise to bend and cut the legs appropriately. Some resistors must cross over the top (from the bottom to the top of the breadboard) and are therefore long. If you'd like, you can electrically isolate these with shrink wrap. Of main note, this design saves space by compacting how circuits are laid out and reducing the need to cross over the breadboard (by duplicating the -9V rail). The Fritzing file readily shows all connections, and parts are named as they are in the original paper (and have the values given for the default design in the original paper). The Fritzing file is great, but you cannot resize parts, so it can be complicated. I hope that several pictures also help with assembly. The Teensy floats next to the breadboard in this design. It is a good idea to hot glue it down to the base of the 3D printed enclosure.

Fritzing file screen shot: Fritzing is a program that will show all connections, but you cannot resize or move the parts, so a screen shot may not be best.
![Easy Fritzing](/ONECoreSite/assets/img/projects/DynamicClamp/FritzingDCCompact.png "Fritzing Pic Easy")
Bend and cut all the wires such that it is unlikely to create a short. The rails from top to bottom are GND, -9V, -9V, and +9V. Rows 26-30 on the breadboard are kind of wasteful, they only connect a wire to a wire, which makes it easy for testing.
![Easy Pic 1](/ONECoreSite/assets/img/projects/DynamicClamp/20171101_142630.jpg "Pic 1 Easy")
![Easy Pic 2](/ONECoreSite/assets/img/projects/DynamicClamp/20171101_142633.jpg "Pic 2 Easy")
![Easy Pic 3](/ONECoreSite/assets/img/projects/DynamicClamp/20171101_142636.jpg "Pic 3 Easy")
![Easy Pic 4](/ONECoreSite/assets/img/projects/DynamicClamp/20171101_142639.jpg "Pic 4 Easy")

***

* Better: This design is the same as the easy, but with a solderable breadboard (Sparkfun [Prt-12070](https://www.sparkfun.com/products/12070)). The Fritzing is the same file as the Easy version, but pictures are given to show how it looks. The Teensy floats next to the breadboard in this design. It is a good idea to hot glue it down to the base of the 3D printed enclosure.

This design is much more robust. The resistors that cross over the microcircuits are coated in shrink wrap for isolation.
![Better Pic 1](/ONECoreSite/assets/img/projects/DynamicClamp/20171101_153911.jpg "Pic 1 Better")
Here it is in the 3D housing (more later). The Teensy floats, so be sure to hot glue it down.
![Better Pic 2](/ONECoreSite/assets/img/projects/DynamicClamp/20171102_103458.jpg "Pic 2 Better")

***

* Better-er: In this design, the space previously wasted on the left of the breadboard is utilized to hold the Teensy firmly. This is great because it can be difficult to plug in the USB cord. Note that the Teensy is turned 90° relative to the breadboard. Therefore it is very important (!) to only connect four pins to the breadboard. Otherwise you will be connecting the pins of the Teensy together! Pins 5, 20, 26, and 39 can be soldered to the bread breadboard with straight breakaway headers (Sparkfun [PRT-00116](https://www.sparkfun.com/products/116)).

The space wasted on the right of the breadboard can hold the teensy.
![Better-er Pic 1](/ONECoreSite/assets/img/projects/DynamicClamp/20171125_123122.jpg "Pic 1 Better-er")
All resistors and wires that cross over the top of the microcircuits have moved to the underside of the breadboard. Additionally, all input/outputs to the BNCs have moved to the bottom.
![Better-er Pic 2](/ONECoreSite/assets/img/projects/DynamicClamp/20171125_122958.jpg "Pic 2 Better-er")
Here's the Fritzing screenshot
![Better-er Pic 3](/ONECoreSite/assets/img/projects/DynamicClamp/FritzingDCCompactRobust.png "Pic 3 Better-er")
To get the Teensy onto the breadboard, first cut (4) breakaway headers into single pins. Put these in the appropriate holes of the breadboard and place the Teensy on top. Solder the pins to Teensy, but not the breadboard. You can then solder all other connections to the breadboard. Then solder the breadboard to the pins on the Teensy.
![Better-er Pic 4](/ONECoreSite/assets/img/projects/DynamicClamp/20171127_144805.jpg "Pic 4 Better-er")

***

* BNC Connections

First size and cut the wires for all connections (all Grounds connect, so leave extra length on the grounds so they can all wrap together). Then solder the wires to the BNC Connector (Mouser [PN 571-5227726-1](https://www.mouser.com/productdetail/571-5227726-1)) with ground on the outside, and 'data/hot' center. You can put shrink wrap over only the center wire for isolation of this solder connection. Then feed through the 3D enclosure, feed through the washer and the nut, and tighten down. Then solder down every 'data/hot'. Then connect all grounds together in a big ball. Solder them all together and cover with shrink wrap.

![BNC 1](/ONECoreSite/assets/img/projects/DynamicClamp/20171128_151746.jpg "BNC 1")
![BNC 2](/ONECoreSite/assets/img/projects/DynamicClamp/20171128_151730.jpg "BNC 2")

***

# Calibration

The original design allows this Dynamic Clamp to be used with a variety of patch clamp and DAQ systems. Each of these systems may use a different gains, and therefore different resistor values may be required in the circuits. These inexpensive resistors have tolerances that may be up to 5% of the stated value. It is therefore important to calibrate the system per the instructions in the original documentation. Although it is very wise to fully understand the equations used in the original design, it is easy to make mathematical errors. Therefore, the ONE Core has created a  [spreadsheet](https://github.com/OptogeneticsandNeuralEngineeringCore/DynamicClamp/raw/master/Calibration%20Of%20Dynamic%20Clamp%20UnitNumberXyZ.xlsx) to ease the calibration process.

To use the Calibration Input and Calibration Output tabs, simply fill out ONLY the columns highlighted in blue. The rest will automatically calculate. This will give you the intercepts and slopes required for calibration, as well as a measure of 'goodness' (R squared value) of both of these. Note that although each resistor is 5% tolerance, the combination of multiple resistors may output overall tolerances higher than 5%. This is OK, the linearity (R squared) is more important).

There is also a tab called Connections that may be used as a hook up guide (it shows how to connect the Dynamic Clamp System into the overall system, as given in the paper).

***

# Files

Here are the files discussed in one place. Calibration, Fritzing, and 3D files.

For the 3D files (printable stl and editable ipt): Parts printed successfully with FDM printer (Lulzbot FTW) PLA or nGen (preferred) with standard Cura settings (normal or high detail), 20% infill. No supports are required. In general, the Easy and Better designs have the Teensy floating next to the breadboards, so the enclosure is longer than the Better-er design. You can view and interact with some 3D files [here.](/ONECoreSite/blog/DynamicClamp3Dstlview)

*Update* Some researchers wanted more BNC connections, so the Better-er design was updated to allow for 8 connections (mega!).

| Name | File Type | Design (if applicable) | Use |
| --- | --- | --- |
| [Calibration File](https://github.com/OptogeneticsandNeuralEngineeringCore/DynamicClamp/raw/master/Calibration%20Of%20Dynamic%20Clamp%20UnitNumberXyZ.xlsx) | .xlsx | NA | Aids in calibration calculations |
| [Fritzing Compact](https://github.com/OptogeneticsandNeuralEngineeringCore/DynamicClamp/raw/master/Compact.fzz) | .fzz | Easy and Better | See the connections |
| [Fritzing Compact Robust](https://github.com/OptogeneticsandNeuralEngineeringCore/DynamicClamp/raw/master/CompactRobust.fzz) | .fzz | Better-er | See the connections |
| [DynamicClampBottom.ipt](https://github.com/OptogeneticsandNeuralEngineeringCore/DynamicClamp/raw/master/DynamicClampBottom.ipt) |.ipt | Easy and Better | Design file bottom |
| [DynamicClampTop.ipt](https://github.com/OptogeneticsandNeuralEngineeringCore/DynamicClamp/raw/master/DynamicClampMegaTop.ipt) |.ipt |  Easy and Better | Design file top |
| [DynamicClampBottom.stl](https://github.com/OptogeneticsandNeuralEngineeringCore/DynamicClamp/raw/master/DynamicClampBottom.stl) |.stl | Easy and Better | Print file bottom |
| [DynamicClampTop.stl](https://github.com/OptogeneticsandNeuralEngineeringCore/DynamicClamp/raw/master/DynamicClampTop.stl) |.stl | Easy and Better | Print file top |
| [DynamicClampBottomCompact.ipt](https://github.com/OptogeneticsandNeuralEngineeringCore/DynamicClamp/raw/master/DynamicClampBottomCompact.ipt) |.ipt | Better-er | Design file bottom |
| [DynamicClampTopCompact.ipt](https://github.com/OptogeneticsandNeuralEngineeringCore/DynamicClamp/raw/master/DynamicClampTopCompact.ipt) |.ipt | Better-er | Design file top |
| [DynamicClampBottomCompact.stl](https://github.com/OptogeneticsandNeuralEngineeringCore/DynamicClamp/raw/master/DynamicClampBottomCompact.stl) |.stl | Better-er | Print file bottom |
| [DynamicClampTopCompact.stl](https://github.com/OptogeneticsandNeuralEngineeringCore/DynamicClamp/raw/master/DynamicClampTopCompact.stl) |.stl | Better-er | Print file top |
| ---New Update--- | ---Mega--- | ---Now with more BNC--- | ---BNC!!--- |
| [DynamicClampBottomMegaTopCompact.ipt](https://github.com/OptogeneticsandNeuralEngineeringCore/DynamicClamp/raw/master/DynamicClampTopMegaCompact.ipt) |.ipt | Better-er | Design file top mega |
| [DynamicClampBottomMegaBottomCompact.ipt](https://github.com/OptogeneticsandNeuralEngineeringCore/DynamicClamp/raw/master/DynamicClampBottomMegaCompact.ipt) |.ipt | Better-er | Design file bottom mega |
| [DynamicClampBottomMegaTopCompact.stl](https://github.com/OptogeneticsandNeuralEngineeringCore/DynamicClamp/raw/master/DynamicClampTopMegaCompact.stl) |.stl | Better-er | Print file top mega |
| [DynamicClampBottomMegaBottomCompact.stl](https://github.com/OptogeneticsandNeuralEngineeringCore/DynamicClamp/raw/master/DynamicClampBottomMegaCompact.stl) |.stl | Better-er | Print file bottom mega |

***

# Additional parts

The designs shared here require several additional/alternative components from what is listed in the original paper.

| Description | Supplier | Part Number  |
| --- | --- | --- |
| 3D Enclosure | ONE Core! **[Support us!](mailto:neuralengineering@ucdenver.edu)** | Easy/Better/Better-er 3D files above |
| Hot glue | ?? | (If you build the Easy or Better design) |
| M3 Screw 4 mm long | McMaster | 92005A112 (sorry, no link, McMaster doesn't play well with links)	|
| BNC Connector | Mouser | [PN 571-5227726-1](https://www.mouser.com/productdetail/571-5227726-1) |
| Breakaway Headers | Sparkfun | [PRT-00116](https://www.sparkfun.com/products/116) |
| Solderable Breadboard | Sparkfun  | [Prt-12070](https://www.sparkfun.com/products/12070) |

***

# ONE Core acknowledgement
Please acknowledge the ONE Core facility in your publications. An appropriate wording would be:

*"Engineering support was provided by the Optogenetics and Neural Engineering Core at the University of Colorado Anschutz Medical Campus, funded in part by the National Institute of Neurological Disorders and Stroke of the National Institutes of Health under award number P30NS048154."*
