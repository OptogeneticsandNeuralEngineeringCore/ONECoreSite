---
layout: project
title: CLARITY L-ETC
date: 18 June 2017
tags: [CLARITY]
screenshot:
  src: /ONECoreSite/assets/img/projects/CLARITYExploded.png
  srcset:
    1920w: /ONECoreSite/assets/img/projects/CLARITYExploded.png
    960w: /ONECoreSite/assets/img/projects/CLARITYExploded.png
    480w: /ONECoreSite/assets/img/projects/CLARITYExploded.png
caption: Clear your tissues reliably, safely, and inexpensively.
description: >
    CLARITY as developed by Chung et al., 2013, is a method to affix a biological tissue sample in a hydrogel polymer and rapidly clear tissue of light scattering molecules, allowing for deep imaging. The Linear Electrophoretic Tissue Clearing (L-ETC) described herein allows for secure tissue containment, more consistent and efficient tissue cooling, fast lipid removal, easier chamber fabrication, and very low initial costs.
links:
  - title: Download All
    url: https://github.com/OptogeneticsandNeuralEngineeringCore/ETC-CLARITY-Chamber/archive/master.zip
  - title: Source
    url: https://github.com/OptogeneticsandNeuralEngineeringCore/ETC-CLARITY-Chamber
---
# Introduction

The L-ETC, is an inexpensive and reliable CLARITY ETC chamber that can be easily assembled by a novice user. It provides several key advantages over previous ETC chamber fabrication methods including secure tissue containment, more consistent and efficient tissue cooling, fast lipid removal, easier chamber fabrication, and very low initial costs. The L-ETC chamber aligns the Electric Field with Clearing Solution flow and is the main focus of this proposal. The L-ETC system as a whole (pump, refrigerator, and power supply) will also be discussed in terms of settings.

The L-ETC chamber is easily fabricated from ‘off the shelf’ parts, and are therefore subject to industry standards, thereby minimizing the risk of leaks. The tissue to be cleared is securely contained in a fine mesh cylindrical tissue strainer. The tissue strainer is fit into off the shelf plumbing components between platinum mesh plate electrodes, creating the L-ETC. The detergent buffer clearing solution (as described in (Structural and molecular interrogation of intact biological systems, Deisseroth 2013)[https://www.nature.com/nature/journal/v497/n7449/full/nature12107.html]) is pumped through the L-ETC, forcing the solution over and through the tissue, expelling generated bubbles from around the tissue. A DC power supply applies an electrical field over the tissue and a refrigerator removes the heat from the solution generated at the platinum-solution interface. The L-ETC applies a uniform electric field, allowing for rapid tissue clearing. The temperature and pressure of the solution can be monitored at the inlet or outlet near the tissue. If necessary, the use of a simple refrigerator allows for stable, uniform cooling without the need for non-uniform ice baths or expensive cooling equipment.

The L-ETC system has shown success with mouse brains and spinal cords and rat lungs. Half mouse brains (n=20) have been successfully cleared in 2-3 days with the L-ETC and whole mouse brains (n=4) have also been cleared in 3-5 days. Smaller, 128 μm slices of mouse brain can be cleared in under a day (n=3). Rat lung slices (5 mm) were cleared in 2 days.

***

# Files

A pdf describing this project in detail can be found [here](https://github.com/OptogeneticsandNeuralEngineeringCore/ETC-CLARITY-Chamber/raw/master/Linear%20CLARITY%20Electrophoretic%20Tissue%20Clearing%20Chamber.pdf). Instructions on how to assemble and key parameters are discussed. Note that you can build your own chamber, have the ONE Core build your own, or you can bring your tissue to the ONE Core for clearing. Please [contact us](mailto:neuralengineering@ucdenver.edu) for more information. Assistance with deep tissue imaging can be found at the [Advanced Light Microscopy Core Site](https://lightmicroscopy.ucdenver.edu/microscopes.php).

***

# Part List

![Linear CLARITY ETC](/ONECoreSite/assets/img/projects/CLARITYExploded.png "L-ETC (or el ETC)")

$$/
Item	Description	PN 	Supplier	Qty need	Qty in package	Price per Package	Total $	Total Cost Per Chamber
1	Solution Inlet	-	-	-	-	-	-	-
2	Thermometer	6182K51	McMaster	1	1	17.91	17.91	17.91
3	3/8" ID Barbed Tube Plug	2974K401	McMaster	4	10	8	8	3.2
4	3/8" ID Clear PVC Tube  	5231K355	McMaster	12"	300	11.25	11.25	-
5	1 1/4" Hex Threaded Nipple	46825K51	McMaster	1	1	1.94	1.94	1.94
6	1" PVC Pipe (spacers)	48925K93	McMaster	.178"	60"	5.27	5.27	0.02
7	1" PVC Pipe (spacers)	48925K93	McMaster	.681"	-	-	-	0.06
8	Sample Holder	21008-949	VWR	2	50	72.3	72.3	2.892
9	1" PVC Pipe (spacers)	48925K93	McMaster	.927"	-	-	-	0.08
10	1 1/4" Coupling	46885k185	McMaster	2	1	6.12	12.24	12.24
11	Platinum 2" x 3" with 4" stem	PLATINUM	The Amateur Chemist	 1/5	1	25	25	5
12	1 1/4" to 3/4" Reducer Hex Nipple 	46885K305	McMaster	2	1	2.91	5.82	5.82
13	3/8" Tube to 3/4" Female Threaded Pipe	5372K222	McMaster	2	5	7.89	7.89	3.156
14	3/8" Cross Connectors	5463K97	McMaster	2	5	8.51	8.51	3.404
15	Pressure Gage	Not Nec	-	-	-	-	-	-
16	Solution Outlet	-	-	-	-	-	-	-
17	Positive Wire (NP)	Lab	-	-	-	-	-	-
18	Negative Wire (NP)	Lab	-	-	-	-	-	-
19	High Strength Sealant (NP)	7475A67	McMaster	1	1	9.41	9.41	9.41
20	Dorm Refridgerator (NP)	Lab	-	-	-	-	-	-
21	Pump (NP) (~.4 L/min)	Lab	-	-	-	-	-	-
22	Power Supply (NP) (28V 0.05A)	Lab	-	-	-	-	-	-
23	TaegaSeal PTFE Tape	4591K12	McMaster	1	1	2.31	2.31	2.31
	Totals	-    -     -     -     -     -      -     -     --    -     -     -     -     -      -     -     - 176.13	65.13
$$

Many of the 3D files shown are from [McMaster](http://www.mcmaster.com/).

***

Please see the files linked above for more information about this project.

***

# ONE Core acknowledgement
Please acknowledge the ONE Core facility in your publications. An appropriate wording would be:

*"Engineering support was provided by the Optogenetics and Neural Engineering Core at the University of Colorado Anschutz Medical Campus, funded in part by the National Institute of Neurological Disorders and Stroke of the National Institutes of Health under award number P30NS048154."*
