---
layout: project
title: Arduino TTL Pulse Generator and Controller
date: 18 June 2017
tags: [3D Print, FDM, Arduino]
screenshot:
  src: /ONECoreWebSite/assets/img/projects/TTL Gen.jpg
  srcset:
    1920w: /ONECoreWebSite/assets/img/projects/TTL Gen.jpg
    960w: /ONECoreWebSite/assets/img/projects/TTL Gen.jpg
    480w: /ONECoreWebSite/assets/img/projects/TTL Gen.jpg
caption: Design and Control your experiments with a TTL Generator and Controller
description: >
    An Arduino based system to generate, listen for, and (coming soon) record TTL Pulses
links:
  - title: Download All
    url: https://github.com/OptogeneticsandNeuralEngineeringCore/Arduino-TTL-Pulse-Generator-and-Controller/archive/master.zip
  - title: Source
    url: https://github.com/OptogeneticsandNeuralEngineeringCore/Arduino-TTL-Pulse-Generator-and-Controller
---
# Arduino TTL Pulse Generator and Controller

Design and Control your experiments with a TTL Generator and Controller

An inexpensive Arduino controlled, four channel, simultaneous TTL pulse generator and controller with BNC connectors and optional 3D printed housing is detailed. TTL pulse modulation requires programing in the Arduino language, but 2 examples are given such **that no prior programing experience** is necessary. The first example shows how to set up four independent TTL outputs. The second example expands on this and allows for input into the generator for a closed loop system, controlled by TTL.

***

# Files

| File | Description | File Type  |
| --- | --- | --- |
| [Arduino Simple 4 Channel TTL Pulse Generator.pdf](https://github.com/OptogeneticsandNeuralEngineeringCore/Arduino-TTL-Pulse-Generator-and-Controller/raw/master/Arduino%20Simple%204%20Channel%20TTL%20Pulse%20Generator.pdf) | The Main File for design and fabrication. Start here | pdf |
| [Arduino simple 4 channel ttl top.ipt](https://github.com/OptogeneticsandNeuralEngineeringCore/Arduino-TTL-Pulse-Generator-and-Controller/blob/master/Arduino%20simple%204%20channel%20ttl%20top.ipt) | Design file for enclosure top | ipt |
| [Arduino simple 4 channel ttl top.stl](https://github.com/OptogeneticsandNeuralEngineeringCore/Arduino-TTL-Pulse-Generator-and-Controller/blob/master/Arduino%20simple%204%20channel%20ttl%20top.stl) | Printable file for enclosure top | stl |
| [Arduino simple 4 channel ttl bottom.ipt](https://github.com/OptogeneticsandNeuralEngineeringCore/Arduino-TTL-Pulse-Generator-and-Controller/blob/master/Arduino%20simple%204%20channel%20ttl%20bottom.ipt) | Design file for enclosure bottom | ipt |
| [Arduino simple 4 channel ttl bottom.stl](https://github.com/OptogeneticsandNeuralEngineeringCore/Arduino-TTL-Pulse-Generator-and-Controller/blob/master/Arduino%20simple%204%20channel%20ttl%20bottom.stl) | Printable file for enclosure bottom | stl |
| [Arduino_Simple_TTL.ino](https://github.com/OptogeneticsandNeuralEngineeringCore/Arduino-TTL-Pulse-Generator-and-Controller/blob/master/Arduino_Simple_TTL.ino) | Arduino file for TTL Generation | ino |
| [Arduino_Simple_Closed_Loop.ino](https://github.com/OptogeneticsandNeuralEngineeringCore/Arduino-TTL-Pulse-Generator-and-Controller/blob/master/Arduino_Simple_Closed_Loop_Mega.ino) | Arduino file for TTL Control (TTL's triggered on input (button or IR Breakbeam) |ino |
| [Screenshots of Downloading and Programing the Arduino.ppt](https://github.com/OptogeneticsandNeuralEngineeringCore/Arduino-TTL-Pulse-Generator-and-Controller/blob/master/Screenshots%20of%20Downloading%20and%20Programing%20the%20Arduino.pptx) | Help in downloading and Programing with Arduino | pptx |
| !!! | If more than 4 channels are required: | !!! |
| [Arduino Simple 8 Channel MEGA TTL Pulse Generator.pdf](https://github.com/OptogeneticsandNeuralEngineeringCore/Arduino-TTL-Pulse-Generator-and-Controller/blob/master/Arduino%20Simple%208%20Channel%20MEGA%20TTL%20Pulse%20Generator.pdf) | If more inputs/outputs are required, try the 8 channel system | .pdf |
| [Arduino simple 8 channel ttl top.ipt](https://github.com/OptogeneticsandNeuralEngineeringCore/Arduino-TTL-Pulse-Generator-and-Controller/blob/master/Arduino%20simple%208%20channel%20ttl%20top%20Mega.ipt) | Design file for enclosure top | ipt |
| [Arduino simple 8 channel ttl top.stl](https://github.com/OptogeneticsandNeuralEngineeringCore/Arduino-TTL-Pulse-Generator-and-Controller/blob/master/Arduino%20simple%208%20channel%20ttl%20top%20Mega.stl) | Printable file for enclosure top | stl |
| [Arduino simple 8 channel ttl bottom.ipt](https://github.com/OptogeneticsandNeuralEngineeringCore/Arduino-TTL-Pulse-Generator-and-Controller/blob/master/Arduino%20simple%208%20channel%20ttl%20bottom%20Mega.ipt) | Design file for enclosure bottom | ipt |
| [Arduino simple 8 channel ttl bottom.stl](https://github.com/OptogeneticsandNeuralEngineeringCore/Arduino-TTL-Pulse-Generator-and-Controller/blob/master/Arduino%20simple%208%20channel%20ttl%20top%20Mega.stl) | Printable file for enclosure bottom | stl |
| [Arduino_Simple_Closed_Loop_Mega.ino](https://github.com/OptogeneticsandNeuralEngineeringCore/Arduino-TTL-Pulse-Generator-and-Controller/blob/master/Arduino_Simple_Closed_Loop_Mega.ino) | Arduino code for 8 channel system | ino |

***

# Introduction
Research labs often conduct experiments that require precise timing characteristics, synchronized across several signals. Pulse Width Modulation (PWM) is a digital on/off signal that carries information in the relative timing characteristics of the signal. Transistor Transistor Logic (TTL) is a form of PWM where the on state is 5 VDC and the off state is at 0 VDC. TTL is frequently employed to precisely control lab equipment such as lasers. Generation of the TTL signal often comes from expensive lab equipment and is carried through BNC cables from the generator to the equipment. The TTL signal is simple, but must be precisely controlled for correct on/off state and timing considerations. More information on TTL can be found here. Modern microcontrollers can easily accomplish the signal generation of more expensive equipment, for most applications. Arduino is a simple, inexpensive microcontroller that natively outputs TTL signals. The intent of this paper is to outline a method to fabricate an inexpensive TTL signal generator and controller.
Arduino outputs PWM digital signals. When the Arduino is powered correctly, this signal is conveniently at 5VDC, and is therefore TTL. Although the chosen board (the Arduino Uno R3) outputs six channels, only four are employed in this design for ease. If six signals are required, it would be easy to expand on this design. If more than 6 channels are required, it may be possible to connect several Arduinos together, but there may be some delay to consider.
This document will outline the equipment, fabrication, and software required. The equipment is intended to be inexpensive. A model for an optional housing for the Arduino and four BNC connections is offered and maybe 3D printed. Fabrication of the final assembly is simple but does require the use of a soldering iron. The software is free. The Arduino programing language is similar to C+, but it is intended that no previous programing is required to generate TTL signals with this set up. Two example programs are given that are intended to be explained in such a way that signal generation can be designed simply by modifying the code in key places. One example shows how to generate four simultaneous signals, each with a unique pulse pattern that is repeated Ad infinitum. The other example shows how to use this set up to control a closed loop experiment. The examples can also be used as an introduction to coding and covers if, for, and while statements.

***

# View .stl Files

If interact-able views of the 3D parts do not load, try reloading the page. If that doesn't work, view them on the GitHub pages (links above) or update your browser.

Four channel ttl top
<script src="https://embed.github.com/view/3d/OptogeneticsandNeuralEngineeringCore/Arduino-TTL-Pulse-Generator-and-Controller/master/Arduino simple 4 channel ttl top.stl"></script>

Four channel ttl bottom
<script src="https://embed.github.com/view/3d/OptogeneticsandNeuralEngineeringCore/Arduino-TTL-Pulse-Generator-and-Controller/master/Arduino simple 4 channel ttl bottom.stl"></script>

Eight channel ttl top
<script src="https://embed.github.com/view/3d/OptogeneticsandNeuralEngineeringCore/Arduino-TTL-Pulse-Generator-and-Controller/master/Arduino simple 8 channel ttl top Mega.stl"></script>

Eight channel ttl bottom
<script src="https://embed.github.com/view/3d/OptogeneticsandNeuralEngineeringCore/Arduino-TTL-Pulse-Generator-and-Controller/master/Arduino simple 8 channel ttl bottom Mega.stl"></script>

***

# ONE Core acknowledgement
Please acknowledge the ONE Core facility in your publications. An appropriate wording would be:

*"Engineering support was provided by the Optogenetics and Neural Engineering Core at the University of Colorado Anschutz Medical Campus, funded in part by the National Institute of Neurological Disorders and Stroke of the National Institutes of Health under award number P30NS048154."*
