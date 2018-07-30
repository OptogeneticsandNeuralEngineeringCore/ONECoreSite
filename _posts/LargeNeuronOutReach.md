---
layout: project
title: Large Neuron Outreach
date: 3 June 2018
tags: [Outreach]
screenshot:
  src: /ONECoreSite/assets/img/projects/lata.png
  srcset:
    1920w: /ONECoreSite/assets/img/projects/lata.png
    960w: /ONECoreSite/assets/img/projects/lata.png
    480w: /ONECoreSite/assets/img/projects/lata.png
caption: An interactive display with lots of hidden teaching opportunities
description: >
  The main focus is to show information flow (and summation) through a single neuron, but there's flashing lights, giant (smashable) buttons, and bubbles!!! Kids love bubbles!!! Encourage everyone, all ages, all levels of education to learn something about these 80 billion little cells that somehow makes a human brain.
links:
  - title: Download All
    url: https://github.com/OptogeneticsandNeuralEngineeringCore/ETC-CLARITY-Chamber/archive/lata.zip
  - title: Source
    url: https://github.com/OptogeneticsandNeuralEngineeringCore/ETC-CLARITY-lata
---
# Large Neuron Outreach

It is a simple and fun project for students, teachers, and research assistances to undertake and teaches simple engineering along the way.  Play with microcontrollers (Arduino), do some simple soldering, hack a bubble machine.

Two big (smashable) buttons sit at the input of two dendrites. Smash one (stimulate) and 'information' is propegated to the cell body as shown by 'moving' lights. Kind of cool. Smash the other and it does the same. OK. Smash BOTH within 2.5 seconds, and they both send lights down, but now the neuron sums, and decides to send out an action potential down the axon (more moving lights). But there are glial cells which speed it up. At the axon end, the neuron need to send out neurotransmitter, which is of course BUBBLES!!!

The neuron itself can be made from tubing, a simple painting, or paper mache.

An Arduino controls the whole shebang. It two two inputs (buttons), outputs two wires to each LED strip, and outputs to a transistor controlling the bubble machine (the power of the bubble machine is too high for the Arduino).

***

# Part List

| Part                                                                         | Supplier | Cost  | Comment                                        |
|------------------------------------------------------------------------------|----------|-------|------------------------------------------------|
| [Arduino Metro](https://www.adafruit.com/product/50)                         | Adafruit | 17.5  | This is Adafruits flavor of the Arduino Uno    |
| [Neopixel Digital RGB Strip](https://www.adafruit.com/product/1376?length=3) | Adafruit | 50.85 | Get 3 meters                                   |
| [TIP120](https://www.adafruit.com/product/976)                               | Adafruit | 2.5   |                                                |
| [Power supply](https://www.adafruit.com/product/1448)                        | Adafruit | 15    | Get 2. Set it to 6V (center positive) for the Arduino and 9 V for the bubble machine |
| [Big Dome Pushbutton](https://www.sparkfun.com/products/9181)                | Sparkfun | 10    | Other colors available                         |
| 22 Gage single core wire                                                     | ??       | ??    | Amazon has some                                |
| [Female DC Power adapter](https://www.adafruit.com/product/368) | Adafruit | 2 | |

***

# Files

The Arduino file can be found [here](https://github.com/OptogeneticsandNeuralEngineeringCore/Outreach/raw/master/LargeNeuron.ino). Simply download it, download the latest [Arduino IDE](https://www.arduino.cc/en/Main/Software?), and open the file. Install the libraries through the manager (click Sketch, Include Library, Manage Libraries). Search for and install the SPI and LPD8806 libraries. Then click Tools, Board, and Arduino Uno. Click Tools, Serial Port, and then select the port number of the Arduino (hint, see what number appears when you connect and disconnect the Arduino). Then click on the verify and upload buttons at the bottom.

***

# Build



***

# ONE Core acknowledgement
Please acknowledge the ONE Core facility in your publications. An appropriate wording would be:

*"Engineering support was provided by the Optogenetics and Neural Engineering Core at the University of Colorado Anschutz Medical Campus, funded in part by the National Institute of Neurological Disorders and Stroke of the National Institutes of Health under award number P30NS048154."*
