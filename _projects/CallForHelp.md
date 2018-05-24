---
layout: project
title: Call for Help
date: 18 May 2018
tags: [SOS, Help]
screenshot:
  src: /ONECoreSite/assets/img/projects/SOS.png
  srcset:
    1920w: /ONECoreSite/assets/img/projects/SOS.png
    960w: /ONECoreSite/assets/img/projects/SOS.png
    480w: /ONECoreSite/assets/img/projects/SOS.png
caption: I have ideas but need help
description: >
    I have ideas but need help
---

# SOS

Sometimes I have ideas that would presumably help Neuroscience, but don't have the time, resources, or knowledge how to implement them. Maybe a plead posted here will push the projects to completion, somehow.

---
# Open Source Fiber Photometry
Fiber Photometry is an inexpensive way to image fluorescence proteins (e.g. GFP) in deep structures of the brain using a single optic probe. You can get LFP like recordings (some claim you can get fancy with your math and get spikes, but that is disputable and beyond me). A typical set up requires control of two LEDs and recording of one analog signal. Companies in the industry talk about how you need a lock in amplifier, but when you are in the digital world, this is two lines of code in MatLab (or Python). I can share the code with you.

It is certainly inexpensive, but I think it could be more so. And the Arduino like Teensy certainly must be up to the challenge. A bit more detail about the control of the set up: the two LEDs (405 nm and 470nm) are controlled (modulated) as sinusoids, from zero to five volts. It is important that we be able to control the min and max of the Amplitude (voltage). The relative phase of these signals does not mater. These are fed into the system, and the fluoresence protein will absorb these signals and output a third wavelength of light as a combination of the two inputs (and of course the contribution of the CA++, which happens much much slower). At any rate, what comes back to the system is an analog signal from 0-9V. Nyquist sampling rate (two time higher than the input signal) would be 2*511 = 1022Hz, a laughable requirement for the teensy. And getting the 0-9V down to the teensy 3.3 V would be a simple voltage divider. But how to output these analog signals is confusing to me.

More information can be found [here](https://forum.pjrc.com/threads/46824-Teensy-Fiber-Photometry-Neuroscience?p=156193#post156193).

Help.

---
# Arduino controlled Lesion Maker
Lesions are still used today to mark electrode location ("you claim you were recording from this brain region, prove it" -Reviewer).The lesion makers I see around here are ancient (beautiful relics, with vacuum tube components). From [here](https://drive.google.com/file/d/15kfHP8jOXf1dwQSMLRsNy6OHagUYhdAd/view) I can get an equation that sounds appropriate. I know (or can input into Arduino) the size of my electrode, and can play around with the time and current, but know from their notes that the current should be on the order of 5-35 uA. And this must be DC, constant current. Sparkfun has a really inexpensive constant current part called the PicoAmp. They talk about replacing one resistor to UP the current, I would like to put a larger resistor in to drive the current DOWN, to the 5-35 uA range. I built the system up, saw good initial testing, the proceeded to try and overlay a keyboard/LCD screen. The code got complex and then even going back to the original code, found that the testing was no longer exactly repeatable. I've never found the time to go back to this. It should be a thing though. I can share what I have thus far with anyone that would like to pursue it.

***

# ONE Core acknowledgement
Please acknowledge the ONE Core facility in your publications. An appropriate wording would be:

*"Engineering support was provided by the Optogenetics and Neural Engineering Core at the University of Colorado Anschutz Medical Campus, funded in part by the National Institute of Neurological Disorders and Stroke of the National Institutes of Health under award number P30NS048154."*
