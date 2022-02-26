# TLRS #
## who I am? ##
I'm an electrical engineer from [makeflyeasy](http://en.makeflyeasy.com/) , an Ardupilot supporter, and a drone fanatic.

## Problems encountered ##

I often use telemetry on the fixed wing to detect the attitude information of the aircraft, and I encountered 2 difficult problems when using the 3DR radio.

* 3DR radio is based on Sik open source firmware, and the mainstream supports Si1000, which is difficult to buy at present.
* The actual flight test distance of 3DR radio is usually only a few hundred meters.

## Birth an idea ##

I want to do a telemetry to achieve the following functions:

* Based on Sik firmware development, it is convenient to configure parameters in the Mission Planner ground station software
* Main control STM32F103 series, RF module Si4463, using conventional chips, easy to purchase, cost-effective
* Support 915/868 MHz, do not use 2.4G, mainly for fixed-wing mountain flight, the signal diffraction ability is too poor
* Mainly support Mavlink complete data package, support PPM/SBUS 16 RC channels
* Both software and hardware are open source and can be merged into AP_Periph in the future to benefit more drone enthusiasts

What can be done:

* Design schematics and PCB files, deliver proofing for production
* Component procurement, welding, hardware debugging
* Write a transparent transmission test program to detect basic functions and interfaces

Main challenges:

* I am not familiar with Sik, it may take a long time to complete the port development
*Sik firmware stability test takes a long time

hope:

* Currently named TLRS, "T" stands for Together, I hope to gather the power of open source to complete this challenge together!

* If there are drone enthusiasts who are good at Sik firmware development, welcome to join, I can provide a hardware development platform for free to facilitate software development and testing


## Special thanks to！

I decided to start this project because I couldn't find an LRS that would meet my fixed wing needs. I am very grateful for the thought inspiration provided by other open source LRS projects, listed below to express my gratitude!

* SiK radios: https://github.com/ArduPilot/SiK

* OpenLRS: https://github.com/openLRSng/openLRSng

* ExpressLRS: https://github.com/ExpressLRS/ExpressLRS

* mLRS: https://github.com/olliw42/mLRS

## Contact information
* TLRS:https://github.com/makeflyeasy/TLRS

* Discussion address:https://discuss.ardupilot.org/t/tlrs-lets-make-a-long-distance-telemetry-system-together/82365

* Contact email: makeflyeasy@qq.com