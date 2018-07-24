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

Top                                      |  Bottom
-----------------------------------------|-----------------------------------------
<img src="/img/fc-top.jpg" width="480">  | <img src="/img/fc-bot.jpg" width="480">

The Cerasus can be configured using the [Cleanflight Configurator](https://github.com/cleanflight/cleanflight-configurator) via USB. (Details in the [Configure](#configure) section)
You do not need to hook up a battery to configure and play around with the flight-controller, since it can be powered from USB. But don't be afraid to hook up your USB cable when its powered from battery: A diode in the supply rail protects your USB Port from overvoltage..

The Cerasus flight-controller outputs four PWM signals for "communication" with the ESC. The numbering in the picture above (PWM 1 - PWM 4) represents the corresponding motor number. The individual pins are labeled on the PCB.

There are two connectors labeled *RC* on the PCB. Since my receiver came with a 4-Pin plug, I used the 4-Pin connector on the bottom side of the PCB.

<a name="firmware"></a>
## Firmware

<a name="download"></a>
### Download
The Firmware for the Cerasus flight controller is located in [this repository](https://github.com/WielandD/XMC_Cleanflight).
An error accours when opening the project in Dave, when you downloaded the repository using `git clone`. As a workaround you can just download the repository by pressing the `Download Zip` button in github.

<img src="/img/zip.png" width="480">

Unzip the contents to a destination of your choice..

<a name="build"></a>
### Build
Launch the Dave IDE and choose a workspace folder. (For example a folder named *Workspace* in your home directory. Do not use the just downloaded repository as your workspace.)
Choose `File > Import` from the top menu bar. Then choos `Infineon >> Dave Project` and click on *next*.

<img src="/img/import1.png"  width="480">

Browse to the folder you unzipped the contents of the git-repo into.
The entry *XMC_Cleanflight* should apear in the project list. 

<img src="/img/import2.png" width="480">

After the project has finished loading you need to activate the correct build configuration. Rightclick on the *XMC_Cleanflight* entry in the left sidepanel and select `Build Configurations > Set Active > Cerasus` from the context menu.

<img src="/img/buildconfig.png" width="500">

Now its time to build the firmware. Click on `Project > Build All` in the top bar to start the building process.
If everything went well, the console on the bottom of the screen should print *Build Finished*.

<a name="flashing"></a>
### Flashing

`[YourDaveWorkspace] > XMC_Cleanflight > Cerasus > XMC_Cleanflight.hex`
`J-Flash Lite`

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
