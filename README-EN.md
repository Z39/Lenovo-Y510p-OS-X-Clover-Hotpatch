# Lenovo IdeaPad Y510P NoteBook for macOS Big Sur 11.0 &macOS Catalina 10.15& macOS Mojave 10.14& High Sierra 10.13

Hackintosh your Y510P Notebook

[English](README-EN.md) | [中文](README.md)

* | Computer:Lenovo IdeaPad Y510P Laptop
* | CPU :Intel Core i5-4200M @ 2.50G/Intel Core i7-4700MQ @ 2.40G (Haswell )
* | Chipset : Lenovo (Intel HM86 Chipset)
* | Graphics :HD4600 (using Intel GPU only) 
* | Audio:ALC282 @ Intel Lynx Point High Definition Audio
* | Ethernet:Atheros QCA8171 Gigabit Ethernet
* | WiFi:Broadcom BCM94352HMB 802.11AC(after replacing the original card)   
* | Bluetooth:BCM20702 (4.0)(after replacing the original card)             
* | BIOS Version:3.08                 
![Screen](Screen.JPG)  
![Screen](Screen1.JPG)  
## Features

* Support macOS Big Sur 11.0 & macOS Catalina 10.15& macOS Mojave 10.14& High Sierra 10.13
* ACPI fixes use hotpatch; related files are located in `/CLOVER/ACPI/patched`.## Releases

## Releases
The latest version can be downloaded on the[release page](https://github.com/Z39/Y510p-OS-X-Clover-Hotpatch/releases) 

## What Works
- [x] Graphics with full acceleration QE/CI (using Intel GPU only) + HDMI Video
- [x] Audio using AppleALC or VoodooHDA.kext(if you use VoodooHDA,pls remember let your Laptop sleep once and then wake it,HDMI sound output will work properly)
- [x]  Ethernet (LAN)
- [x]  WiFi / Bluetooth (after replacing the Intel card (incompatible) with a compatible one like Broadcom BCM4352 for example
- [x]  Sleep (also sleep on Lid Close)
- [x]  Brightness,Support use FN+Arrows﻿
- [x]  Battery
- [x]  Keyboard / Touchpad
- [x]  CPU Power Management
- [x]  Web-Cam
- [x]  All USB ports
- [x]  App Store/iCloud/iMessage/Facetime
- [x]  TRIM
- [x]  SIP (0ff)



## Problems
* VGA Port:This will not work at all. A workaround when projecting to VGA display is to buy and use (male)HDMI-to-(fem﻿ale)VGA adapter. 
* Restart:There is a problem related to graphics occurs when﻿ display goes off then on, like when system sleeps ﻿and wake or when changing display r﻿esolutio﻿n for example, which results in n﻿o display on restart﻿. These ev﻿ents requires re-initialization for the graphic driver but it seems the driver re-initialize incorrectly. As a result, the graphics related memory hold wrong data for some graphic registers which indirectly affects the restart functionality. Once the system is restarted in any of these scenarios, the POST (where Lenovo logo should appear) has no display and so is Clover and beyond if an OS is selected and booted using keyboard blindly. However, this is a graphic driver issue and has nothing to do with power or reboot function itself.
* Nvidia GPU (built-in): This will have to be disabled as OS X does not support Optimus technology.
* Audio:There is a problem of pop when boot the notebook
* Truddy:There is a problem of truddy when boot the notebook if your notebook's bios be set to uefi only.

## Links

- Clover EFI bootloader [Link](https://github.com/Dids/clover-builder/releases)

- FakeSMC [Link](https://bitbucket.org/RehabMan/os-x-fakesmc-kozlek/downloads/)

- VoodooPS2Controller [Link](https://bitbucket.org/RehabMan/os-x-acpi-battery-driver/)

- ACPIBatteryManager [Link](https://bitbucket.org/RehabMan/os-x-acpi-battery-driver/)

- BrcmPatchRAM [Link](https://bitbucket.org/RehabMan/os-x-brcmpatchram/downloads/)

- Lilu [Link](https://github.com/acidanthera/Lilu)

- AirportBrcmFixup [Link](https://github.com/acidanthera/AirportBrcmFixup)

- WhateverGreen [Link](https://github.com/acidanthera/WhateverGreen)

- AppleALC [Link](https://github.com/acidanthera/AppleALC)

- AtherosE2200Ethernet [Link](https://github.com/Mieze/AtherosE2200Ethernet)

- Enable macOS HiDPI [Link](https://github.com/xzhih/one-key-hidpi)

## Credits

- Thanks to RehabMan、intruder16、panybbib、ahmed_ais

