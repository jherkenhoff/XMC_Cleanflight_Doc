# XMC Cleanflight

![Banner image](/img/banner.jpg)

This tutorial is going to walk you through installing [Cleanflight](http://cleanflight.com/) on the **Cerasus** flight controller from Infineon. You do not need programming skills to follow this tutorial.

For those unfamiliar with Cleanflight. It is an open source flight-controller firmware which is used on a broad range of commercial and open source flight-controllers. Since it is targeted towards 32 bit MCU's it provides a perfect base for the Cerasus. 

In addition to the firmware setup the build of the **Racecopter** drone hardware is shown. Note that the hardware is not coupled to the Cerasus sontroller, so you can choose to build your custom hardware.

* [Requirements](#requirements)
    * [Hardware used in this build](#used-in-this-build)
* [Cerasus Flight Controller](#cerasus-flight-controller)
    * [Firmware](#used-in-this-build)
        * [Download](#download)
        * [Build](#build)
        * [Flashing](#flashing)
    * [Configure](#configure)
* [Hardware build](#hardware-build)

<a name="requirements"></a>
# Requirements
To follow this guide, you need the following hardware and software:
* Infineon Cerasus V1.0 flight controller
* i-Bus receiver
* [XMC Link debugger](https://www.infineon.com/cms/en/product/evaluation-boards/kit_xmc_link_segger_v1/)
* Windows PC with [DAVE 4.x](https://infineoncommunity.com/dave-download_ID645) software installed
* General drone hardware (X4 Drone frame with Motors, Props, ESC and batteries etc.)

> **For Linux users:** I managed to get DAVE 4.4.2 running in Wine. You need to install the Segger J-Link tools used for flashing manually using the official [Segger Packages](https://www.segger.com/downloads/jlink/#J-LinkSoftwareAndDocumentationPack)

<a name="used-in-this-build"></a>
## Hardware used in this build:
* Custom carbon fiber X4 frame
* Racerstar [BR2205 2300KV](http://www.racerstar.com/Racerstar-Racing-Edition-2205-BR2205-2300KV-2-4S-Brushless-Motor-Red-CW-or-CCW-for-220-250-RC-Drone-FPV-Racing-p-33.html) brushless motor
* Racerstar Rev35A 4in1 ESC
* FS-i6 Transmitter
* Flysky FS-A8S i-Bus receiver
* Tattu 1550mAH 4S LiPo battery pack

You might as well use any other drone hardware as long as it fulfills the requirements listed in the Requirements section.

<a name="cerasus-flight-controller"></a>
# Cerasus Flight Controller

The *Cerasus* is a flight controller designed by Infineon. It is equipped with a microcontroller from Infineons XMC series (XMC4500 - 32 Bit ARM Cortex M4).

<a name="firmware"></a>
## Firmware
ZIP Runterladen, nicht klonen

<a name="download"></a>
### Download

<a name="build"></a>
### Build

<a name="flashing"></a>
### Flashing


<a name="configure"></a>
## Configure
Channel mapping
Motor direcion
Save nach Dump
Config file
ESC Calibration

<a name="hardware-build"></a>
# Hardware build

## Check Motor direction

## FLY
