---
layout: project
title: Some Notes on DC Power Sources
date: 16 May 2018
tags: [DC Current, Electrical]
screenshot:
  src: /ONECoreSite/assets/img/projects/DC.png
  srcset:
    1920w: /ONECoreSite/assets/img/projects/DC.png
    960w: /ONECoreSite/assets/img/projects/DC.png
    480w: /ONECoreSite/assets/img/projects/DC.png
caption: Power your research!
description: >
    Power your research!
---
# Specifying a DC power source
This seems to come up a lot, so I thought I would draft up a quick how to specify a DC power source, or at least the main points. The first thing to consider when specifying a DC power source is obviously that you get one that plugs into the wall. If in the US, it should be a US plug that can accept the 120V, 60Hz AC power. Then:

* DC voltage. What you are trying to power should give you an indication here. For example: Arduino Uno does well with 7-12V in the power jack or 5V through the USB. LED's need to be above what is called the forward voltage.
* Current. The current listed on the power supply is the maximum current it can supply. If you go over this current, you could damage the plug or whatever you are powering.
* Polarity. Which pole (positive or ground) is in the center can change with the plug you buy. Any plug should list which one is which with a picture showing what is connected to the outside (the 'c') and what is connected to the inside (the center dot). But it's always a good idea to check with a Digital Multimeter.
![Polarity](/ONECoreSite/assets/img/projects/DCPolarity.png "Polarity")
This plug has the outside as negative and the inside as positive.
* Size. Most DC barrel plugs are 5.5mm sleeve and a 2.1mm pin, but this can vary wildly.

If you are not sure of what to get, there are [Universal AC/DC adapters](https://www.amazon.com/Universal-CUGLB-Switching-Selectable-Electronics/dp/B074FT2LXD/ref=sr_1_16?ie=UTF8&qid=1526138805&sr=8-16&keywords=variable+dc+power+supply) that come with US/EU and other plugs. You can set the voltage by turning a knob, the maximum current is not something you can change, but you can change the polarity by reversing how you plug in the barrel (which also comes in different sizes).
Also note that I have had great success with inexpensive variable DC power supplies such as the [Yescom 110V Input 30V 5A Output Precision Variable Digital DC Power Supply with Alligator Test Lead Set](https://www.amazon.com/Yescom-Precision-Variable-Digital-Alligator/dp/B00QJS8RW0/ref=sr_1_10?ie=UTF8&qid=1526138805&sr=8-10&keywords=variable+dc+power+supply) which also allows for setting the maximum current output rather than the voltage (handy for [CLARITY](/ONECoreSite/_projects/CLARITYL-ETC))

***

# ONE Core acknowledgement
Please acknowledge the ONE Core facility in your publications. An appropriate wording would be:

*"Engineering support was provided by the Optogenetics and Neural Engineering Core at the University of Colorado Anschutz Medical Campus, funded in part by the National Institute of Neurological Disorders and Stroke of the National Institutes of Health under award number P30NS048154."*
