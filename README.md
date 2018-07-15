# XMC Cleanflight

![Banner image](/img/banner.jpg)

This tutorial is going to walk you through installing [Cleanflight](http://cleanflight.com/) on the **Cerasus** flight controller from Infineon.
It assumes you are new to Ubuntu and ROS and is meant to be a dummies guide to installing and configuring a Multiple ROS Master System. Note there are newer versions of ROS available as well as Ubuntu which you can choose to install on your own.

For those unfamiliar with Cleanflight. It is an open source flight-controller firmware which is used on a broad range of commercial and open source flight-controllers. Since it is targeted towards 32 bit MCU's it provides a perfect base for the Cerasus. 

In addition to the firmware setup the build of the **Racecopter** drone hardware is shown. You might as well use any other drone hardware as long as it fulfills

## Getting startet

### Requirements
To follow this guide, you need the following hardware and software:
* Infineon Cerasus V1.0 Flight Controller
* i-Bus Receiver
* [XMC Link debugger](https://www.infineon.com/cms/en/product/evaluation-boards/kit_xmc_link_segger_v1/)
* Windows PC with [DAVE 4.x](https://infineoncommunity.com/dave-download_ID645) Software installed
* General drone hardware (Frame with Motors, Props, ESC and batteries etc.)

> **For Linux users:** I managed to get DAVE 4.4.2 running in Wine. You need to install the Segger J-Link tools used for flashing manually using the official Segger [Packages](https://www.segger.com/downloads/jlink/#J-LinkSoftwareAndDocumentationPack)

#### Hardware used in this build:
* Custom carbon fiber X4 frame
* Racerstar [BR2205 2300KV](http://www.racerstar.com/Racerstar-Racing-Edition-2205-BR2205-2300KV-2-4S-Brushless-Motor-Red-CW-or-CCW-for-220-250-RC-Drone-FPV-Racing-p-33.html) brushless motor
* Racerstar Rev35A 4in1 ESC
* FS-i6 Transmitter
* Flysky FS-A8S i-Bus receiver
* Tattu 1550mAH 4S LiPo battery pack


## Hardware build


## Flashing FC Firmware
ZIP Runterladen, nicht klonen


## Configure FC
Channel mapping
Motor direcion
Save nach Dump
Config file
ESC Calibration
