---
layout: project
title: Microscope Camera
date: 3 March 2018
tags: [Raspberry Pi, Raspbian, Microscope]
screenshot:
  src: /ONECoreSite/assets/img/projects/MC/20180312_110331.png
  srcset:
    1920w: /ONECoreSite/assets/img/projects/MC/20180312_110331.png
    960w: /ONECoreSite/assets/img/projects/MC/20180312_110331.png
    480w: /ONECoreSite/assets/img/projects/MC/20180312_110331.png
caption: A super inexpensive and powerful system to get pictures and videos
description: >
    This is an inexpensive stand alone system based on the Raspberry Pi and associated camera. It allows for you to remotely take high resolution pictures and video based on your input, time delays, or even motion. 3D components are given that allow you to focus the camera into the eyepiece of any microscope.
links:
  - title: Download All
    url: https://github.com/OptogeneticsandNeuralEngineeringCore/MicroscopeCamera/archive/master.zip
  - title: Source
    url: https://github.com/OptogeneticsandNeuralEngineeringCore/MicroscopeCamera
---

# Microscope Camera

This is a super cool project. With this project, you can learn to build a very inexpensive stand alone computer (Raspberry Pi, FTW!). It acts as a stand alone system for any of your scientific (or otherwise) endeavors; after set up, it allows you to capture pictures and videos (8 MP!) from ANYWHERE with internet access. Tell your boss you were in over the weekend (I did! She fell for it!) and have pictorial evidence to back it up. You can monitor your experimental set up from ANYWHERE with internet access. Simply go to the specified website and tell the system how and when to capture the pictures or videos, and then download thm. You can tell the system to capture pictures and videos based on your input, some time series, or even *motion* (right?). The system will act as a server, and will hold the pictures for you to access whenever you (or your boss) feels like returning to 'work'. Check out the latest functionality [here](https://elinux.org/RPi-Cam-Web-Interface).

And beyond this: Have you ever tried to take a picture from an eyepiece of a microscope? What a pain! Just when you get it all aligned, the dang camera (phone) will 'auto-focus' to some other random point! Well, we include some files that will allow you to inexpensively 3D print some parts out that will attach to any eyepiece of a microscope. Throw in some other parts (everyone has inexpensive clicking pens, so the design is based around that), and boom, you have a system that can now easily focus on your project.

The system is made up of the computer (Raspberry Pi), a 5 MP Raspberry Pi camera, a microSD card, an inexpensive touchscreen (optional), an inexpensive wireless mouse and keyboard (optional), 3D printed housing (optional, I guess), and 3D printed parts to attach to a microscope eyepiece (again, optional). The references shown at the bottom of the page can show you how to set up the operating system and software (all open source and free), but you can save yourself some major headaches (!) by using the image given. You can also use an IR camera for night vision.

***

# Files

| File | Description | File Type  |
| --- | --- | --- |
| [MicroscopeCamera.img](https://drive.google.com/open?id=1669Rly20GG5IpvITtk1oS-zLRX3fnquC) | Raspbian with all the drivers and software to get you going. Caution, it's 7 GB | img |
| [Housing Bottom.ipt](https://github.com/OptogeneticsandNeuralEngineeringCore/MicroscopeCamera/raw/master/Housing%20Bottom.ipt) | Housing Bottom | ipt (3D editable) |
| [Housing Bottom.stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MicroscopeCamera/raw/master/Housing%20Bottom.stl) | Housing Bottom | stl (3D printable) |
| [Housing Top.ipt](https://github.com/OptogeneticsandNeuralEngineeringCore/MicroscopeCamera/raw/master/Housing%20Top.ipt) | Housing Top | ipt (3D editable) |
| [Housing Top.stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MicroscopeCamera/raw/master/Housing%20Top.stl) | Housing Top | stl (3D printable) |
| [Microscope Eyepiece Holder Back.ipt](https://github.com/OptogeneticsandNeuralEngineeringCore/MicroscopeCamera/raw/master/Microscope%20Eyepiece%20Holder%20Back.ipt) | Eyepiece back | ipt (3D editable) |
| [Microscope Eyepiece Holder Back.stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MicroscopeCamera/raw/master/Microscope%20Eyepiece%20Holder%20Back.stl) | Eyepiece back | stl (3D printable) |
| [Microscope Eyepiece Holder Cup.ipt](https://github.com/OptogeneticsandNeuralEngineeringCore/MicroscopeCamera/raw/master/Microscope%20Eyepiece%20Holder%20Cup.ipt) | Eyepiece front | ipt (3D editable) |
| [Microscope Eyepiece Holder Cup.stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MicroscopeCamera/raw/master/Microscope%20Eyepiece%20Holder%20Cup.stl) | Eyepiece front | stl (3D printable) |
| [Microscope Eyepiece Holder Ball.ipt](https://github.com/OptogeneticsandNeuralEngineeringCore/MicroscopeCamera/raw/master/Microscope%20Eyepiece%20Holder%20Ball.ipt) | Eyepiece center | ipt (3D editable) |
| [Microscope Eyepiece Holder Ball.stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MicroscopeCamera/raw/master/Microscope%20Eyepiece%20Holder%20Ball.stl) | Eyepiece center | stl (3D printable) |
| [Microscope Eyepiece El L.ipt](https://github.com/OptogeneticsandNeuralEngineeringCore/MicroscopeCamera/raw/master/Microscope%20Eyepiece%20Holder%20El%20L.ipt) | L Bracket | ipt (3D editable) |
| [Microscope Eyepiece El L.stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MicroscopeCamera/raw/master/Microscope%20Eyepiece%20Holder%20El%20L.stl) | L Bracket | stl (3D printable) |
| [Microscope Eyepiece Holder Eyepiece Holder Grips.ipt](https://github.com/OptogeneticsandNeuralEngineeringCore/MicroscopeCamera/raw/master/Microscope%20Eyepiece%20Holder%20Grips.ipt) | Eyepiece (all three) | ipt (3D editable) |
| [Microscope Eyepiece Holder Eyepiece Holder Grips.stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MicroscopeCamera/raw/master/Microscope%20Eyepiece%20Holder%20Grips.stl) | Eyepiece (all three) | stl (3D printable) |
| [Microscope Stylist Holder.ipt](https://github.com/OptogeneticsandNeuralEngineeringCore/MicroscopeCamera/raw/master/Stylis%20holder.ipt) | Stylist Holder | ipt (3D editable) |
| [Microscope Stylist Holder.stl](https://github.com/OptogeneticsandNeuralEngineeringCore/MicroscopeCamera/raw/master/Stylis%20holder.stl) | Stylist Holder | stl (3D printable) |

To view the stl files in your web browser, go [here](https://github.com/OptogeneticsandNeuralEngineeringCore/MicroscopeCamera).

# Printing profile
Parts have been successfully printed with either PLA or nGen (preferred) with standard Cura settings (normal detail), 20-50% infill. No supports are required. Parts should probably be rotated in your slicing software.

Don't have an FDM printer? You can upload these to 3DHubs. Or support the [ONE Core](mailto:neuralengineering@ucdenver.edu) and order though us!!!!

***

# Other components

| Part | Estimated Cost | Comment  |
| --- | --- | --- |
| [Raspberry Pi 3](https://www.sparkfun.com/products/13825) | $40 | Maybe the cheaper Raspberry Pi Zero could work?? |
| [Raspberry Pi Power](https://www.sparkfun.com/products/13831) | $7 | !Make sure the power supply can have enough current |
| [Raspberry Pi Cam](https://www.sparkfun.com/products/14028) | $30 | Or does your project require night vision? |
| [Raspberry Pi Ribbon Cable](https://www.adafruit.com/product/1731) | $3 | The camera comes with a cable, but this is super handy |
| [microSD Card](https://www.amazon.com/Samsung-MicroSDXC-Adapter-MB-ME64GA-AM/dp/B06XX29S9Q/ref=sr_1_3?ie=UTF8&qid=1520862662&sr=8-3&keywords=microsd) | $20? | This project allows you to spec your own. Get one +8GB (but at 8 GB, you will probably only have room for one picture). Make sure you can connect it to your main computer via SD or USB. |
| Four M2 nuts | $1/100 | McMaster: 90592A004 (sorry, their links never work well) |
| Eight M2 Phillips 10mm screws | $4/100 | McMaster: 92005A033 You will need 11. Four in the Eyepiece holder need be only 5 mm long, so get those if you want pretty, or just use these and let them hang out |
| [Touch Screen](https://www.amazon.com/dp/B072813CS7/ref=dp_prsubs_2) | $30 | Comes with several other components pictured. Optional, but not as cool, and you'd have to SSH into the Pi with some program like PuTTY (not covered here) |
| [Fan](https://www.amazon.com/Vktech-Brushless-Cooling-0-1-0-3A-50x15mm/dp/B00EL938E6/ref=pd_lpo_vtph_147_bs_t_1?_encoding=UTF8&psc=1&refRID=F3WWZAZ9J4PKY1ABSYMV) | $9/6 | Any 5VDC fan could work. But honestly, you probably don't need one. I added one to be extra safe, but the system doesn't really get all that warm |
| [Keyboard/Mouse](https://www.amazon.com/Rii-Wireless-Touchpad-Keyboard-Android/dp/B00JO80LUI/ref=sr_1_5?ie=UTF8&qid=1520875418&sr=8-5&keywords=rii+wireless&dpID=51irg9urQPL&preST=_SX300_QL70_&dpSrc=srch) | $14 | You can plug in (any-ish) keyboard and mouse to the Raspberry Pi. This one is wireless and both a keyboard and mouse, but long terminal commands can be cumbersome |
| [Retractable Pen](https://www.amazon.com/BIC-Retractable-Medium-Point-12-Count/dp/B00006IE7Y/ref=sr_1_4?ie=UTF8&qid=1520863790&sr=8-4&keywords=pen%2Bclick&th=1) | $5/12 | Oh, come on, you have one laying around your office. Or swipe one from that annoying office neighbor whom is always clicking the darn thing |

So for $165, you can get all the bells and whistles, have lots of [extra parts](https://gizmodo.com/5422121/how-to-build-a-pencil-crossbow/). All software is free.

***

# Assembly

Instructions on how to assemble the 3D printed components can be found [here](https://github.com/OptogeneticsandNeuralEngineeringCore/MicroscopeCamera/raw/master/Microscope%20Camera%20Assembly%20Instructions.pdf). This includes the housing to house the Raspberry Pi and touchscreen (it'll even hold the stylist, you stylish person you). The 3D printed eyepiece parts are assembled with a simple click pen (you know, like [this](/ONECoreSite/assets/img/projects/MC/20180312_110335.jpg)). The outer part of the pen acts as the necessary shafts, and the springs of the pen help quickly disassemble. Some of the screws can help you make small adjustments (better focusing), but are not really that necessary (the 3D parts friction fit onto the pen, so you can just push the camera where you want).

***

# Operating System and Software

You can find the latest Operating System, currently Raspbian Jessie [here](https://www.raspberrypi.org/blog/raspbian-jessie-is-here/). It's a flavor of Linux. It has a look and feel of any OS you are used to. It is open and free. Plus it comes with some cool games, office programs, and the super powerful Linux terminal, which, I advise you use (don't worry, the instructions to do so are below and so so simple). Of course, you can start here (with a fresh and new OS), expand the OS on the microSD card, download the drivers for the touchscreen, and download the software for the Web Cam interface...but it's not exactly straightforward.

I therefore recommend that you simply download the OS image in the link above. It will work as is, and I'll go over how to update it (security, new features, and whatnot that might come after I document this).

The microSD card should be 8 GB or more (if storing videos, consider at least 128 GB). There are lots of documentation showing what cards work with the Raspberry Pi, so I won't go into that, but consider getting a high 'Class' one. It should be blank.

(If not, you can clear it and restore it by following the instructions [here](https://www.howtogeek.com/170794/ask-htg-how-can-i-reclaim-the-full-capacity-of-an-sd-card/). If that link doesn't work: on a Windows machine: put in the MicroSD card, hit the window key, type `cmd`, hit enter. Type `disk part`, hit enter. Click OK, type `list disk`, hit enter. (!)Understand which disk listed is the MicroSD card. ¡If you mess this up, you can erase your entire computer(!!!!!!!!!). Type `select disk #` (where the number is the MicroSD card (¡!)). Hit enter. Type `clean`, hit enter. Type `create partition primary`, hit enter. Type `list volume`. Understand what volume the microSD card is. Type `select volume #` (where # is the number of the microSD). Type `assign *` (where * is a letter you choose to assign the drive, R is good (for raspberry)), hit enter.)

Now with a clean, large microSD card, the MicroscopeCamera image downloaded, and the system generally assembled, let's burn the image to the the microSD card. There are lots of image burning software, I recommend [Win32DiskIamger](https://sourceforge.net/projects/win32diskimager/). Download that and open it. Click on the folder icon and find the MicroscopeCamera.img file. (!!!!!)Ensure that you select the drive that is the microSC card (R). Click Write and OK and go get a coffee. Figure out how to send me one.

When done, safely eject. Put the microSD card in the Raspberry. Turn the system on by plugging in the power cord. The touchscreen may show an error (it's minor, but pain to get rid of, so whatever). Then the beautiful Raspberry Pi images will flash, and within 10 seconds, you have a functioning system! Feel free to play around, there's lots of cools stuff here!

Care was taken to shrink the OS and software. We fit it in as small a package as we could, and it should fit any microSD larger than itself. But currently, the Operating System it doesn't see the entire microSD, so let's tell it what's up. Bring up the *all powerful* terminal by holding ctrl alt and hit t. Type `sudo raspi-config`, hit enter. Push the down arrow until Advanced Options is highlighted, hit enter. Expand Filesystem should be highlighted, hit enter. Hit enter.

If you used my image, the drivers for the touchscreen are already there and rocking out. But every individual touchscreen is different, so calibrate it. Click on the 'start' (Red Raspberry image) in the top right of the screen, select preferences, and select Calibrate Touchscreen. Follow the instructions.

We need interwebz. Connect to your wireless (or wired, if you are so inclined). If connecting to a University wireless system, the process can be difficult. See [here](https://optogeneticsandneuralengineeringcore.github.io/ONECoreSite/projects/Connecting%20Linux%20to%20Campus%20WiFi/) for my instruction for UCDenver for some help. (Basically, if you connect to a guest network, the system probably won't automatically redirect you to a log in page, so you have to figure out how to type that in to an address bar. If you have to log in, the process is more involved, the link should help point you in the right direction).

Sweet, now let's figure out the IP address of the system. In the terminal (ctrl alt t) type `ifconfig`, hit enter. If you are on wireless, your IP address is listed under wlan0, inet6 address. If on wired, your IP address is listed under lo inet6 address. Now, any computer *on the same internet* you can go to this IP address and access the video stream. That is, using any modern internet browser, type in the IP address you found above, and you can access the camera on the raspberry!

Updating is good. Hold control and alt and hit t. This will bring up the *all powerful* terminal. Type `sudo apt-get upgrade`, hit enter. Go get a coffee. Figure out how to send me one. When done, type `sudo apt-get update`, hit enter. For the ultimate update (yo, this...might break things, but it'll update yer system real good like). So, if you do this and it doesn't work, start over and don't do this, LoL. But it'll probably be fine, probably, LoLz) type `sudo apt-get dist-upgrade`, hit enter. Update the interface with `cd RPI_Cam`, hit tab, hit enter. Type `./update.sh`, hit enter.

Of course you can access the camera though the system itself. Click the button next to raspberry pi icon (Blue Web Browser image) and type in the IP found above. This will bring you to the Web Cam interface. I won't go into much detail on how to use that, because [they](https://elinux.org/RPi-Cam-Web-Interface) will probably update more often than I, so just follow and support them.

Now, how awesome is this? For very little money, you have a fully functional stand alone computer/server. It intelligently will take pictures and videos. Random notes to noobs: always shut down the system (!) by clicking on the top left raspberry and shut down (or `sudo shutdown -now` in the terminal). If you run into errors, google them.

Helpful note: The terminal doesn't allow for typical copy/paste; use ctrl shift c and ctrl shift v.

This is really just an easy way to access already available projects. Support them. Expand on them. What can you do with this? Let [me](mailto:later) know.

***

# References

This project is a combination of other people's projects. The main components are from:
https://elinux.org/RPi-Cam-Web-Interface
https://www.waveshare.com/wiki/5inch_HDMI_LCD
https://www.howtogeek.com/170794/ask-htg-how-can-i-reclaim-the-full-capacity-of-an-sd-card/
https://www.raspberrypi.org/forums/viewtopic.php?t=84999
http://www.cs.upc.edu/lclsi/Manuales/wireless/files/wpa_supplicant.conf
https://github.com/Drewsif/PiShrink
https://github.com/qrti/shrink

***

# ONE Core acknowledgement
Please acknowledge the ONE Core facility in your publications. An appropriate wording would be:

*"Engineering support was provided by the Optogenetics and Neural Engineering Core at the University of Colorado Anschutz Medical Campus, funded in part by the National Institute of Neurological Disorders and Stroke of the National Institutes of Health under award number P30NS048154."*
