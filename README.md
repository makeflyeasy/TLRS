
# TLRS #
## 我是谁？##
我是一名来自makeflyeasy的电子工程师，Ardupilot的支持者，无人机狂热爱好者。

## 遇到的问题 ##

我经常在固定翼上使用数传，检测飞机的姿态信息，我在使用3DR radio遇到了2个难以解决的问题。

* 3DR radio基于Sik开源固件，主流支持Si1000，目前很难购买。
* 3DR radio实际飞行测试距离，通常只有几百米。

## 诞生一个想法 ##

我想做一个数传，实现下面的功能：

* 基于Sik固件开发，方便在Mission Planner地面站软件配置参数
* 主控STM32F103系列，射频模块Si4463，采用常规芯片，方便采购，性价比高
* 支持915/868 MHz，不使用2.4G，主要是固定翼山区飞行，信号绕射能力太差
* 主要支持Mavlink 完整数据包，支持PPM/SBUS16个RC通道
* 软硬件都开源，未来能够合并到AP_Periph，让更多的无人机爱好者受益

能够做的事情：

* 设计原理图和PCB文件，交付打样生产
* 元器件采购、焊接、硬件调试
* 编写一个透传测试程序，检测基本功能和接口

主要挑战：

* 我对Sik并不熟悉，可能需要很长的时间才能完成移植开发
* Sik固件稳定测试需要很长的时间

希望：

* 目前把数传名字命名为TLRS，"T"代表Together，希望汇聚开源的力量，共同完成这个挑战！

* 如果有擅长Sik固件开发无人机爱好者，欢迎加入，我可以免费提供硬件开发平台，方便软件开发和测试


## 最后感谢

我因为没找到一款LRS可以满足我的固定翼需求，才决定开始这个项目。我非常感谢其他开源LRS项目提供的思考灵感，列在下面表达感谢！

SiK radios：https://github.com/ArduPilot/SiK

OpenLRS：https://github.com/openLRSng/openLRSng

ExpressLRS：https://github.com/ExpressLRS/ExpressLRS

mLRS：https://github.com/olliw42/mLRS

#TLRS#
## who I am? ##
I'm an electrical engineer from makeflyeasy, an Ardupilot supporter, and a drone fanatic.

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


## Final thanks

I decided to start this project because I couldn't find an LRS that would meet my fixed wing needs. I am very grateful for the thought inspiration provided by other open source LRS projects, listed below to express my gratitude!

SiK radios: https://github.com/ArduPilot/SiK

OpenLRS: https://github.com/openLRSng/openLRSng

ExpressLRS: https://github.com/ExpressLRS/ExpressLRS

mLRS: https://github.com/olliw42/mLRS