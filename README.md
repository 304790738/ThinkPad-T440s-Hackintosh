# MacOS ThinkPad T440s
Hackintosh MacOS , the branch number is the version of MacOS,

 e.g :

branch  ---> MacOS version

10.15.2 ---> 10.15.2

## Pre-Installation

### 1. Warning: check you BIOS version !!!

**You should update(downgrade) BIOS to v2.36 version or MOD BIOS to remove Whitelist!**

### 2. BIOS settings

- `Security -> Security` Chip: **Disabled**
- `Memory Protection -> Execution Prevention`: **Enabled**
- `Virtualization -> Intel Virtualization Technology`: **Disabled**
- `Internal Device Access -> Bottom Cover Tamper Detection`: must be **Disabled**
- `Anti-Theft -> Current Setting`: **Disabled**;
- `Anti-Theft -> Computrace -> Current Setting`: **Disabled**
- `Secure Boot -> Secure Boot`: **Disabled**
- `UEFI/Legacy Boot`: **Both**
- `UEFI/Legacy Priority`: **UEFI First**
- `CSM Support`: **Yes**

### 3. Know your hardware

|Compenent|Reference|
|---|---|
|CPU|Intel Core i7-4600U|
|RAM|DDR3L 12GB Bus 1600MHz|
|GFX|Intel HD Graphics 4400|
|Sound|Intel HD Audio (Realtek ALC292)|
|Display|14" FHD IPS LCD|
|WIFI|Intel Wireless N7260|
|SD Card reader|Realtek PCI Express Card Reader|
|Camera|Integrated Camera (USB Internal port)|

#### What will work:
- Intel HD 4400 Graphics QE/CI
- USB Ports
- Intel Ethernet
- Audio (All Inputs & Outputs)
- Sleep and Wake
- Touch Screen
- Mini DisplayPort and Mini DisplayPort Audio
- VGA / D-Sub Port
- CPU and IGPU Power Management
- Battery Status
- Brightness
- Function Keys (Fn)
- ClickPad and TrackPad
- Integrated Camera

#### What will not work:
- Wireless (shoud be replace)

#### WIFI :
ThinPad T440s M.2 WIFI port is A+E keyed
- BCM94360CS2 (Recommend)
- DW1560 (BCM94352Z)
- DW1830

The USB WIFI 
- COMFAST CF-811AC 650
## Installation

....

## Post-Installation

### 1. Tools needed

- Clover Installer (https://sourceforge.net/projects/cloverefiboot/)
- Clover Configurator (https://mackie100projects.altervista.org/download-clover-configurator/)
...
- OpenCore (soon)

### 2. Kexts used
- VirtualSMC.kext
- SMCProcessor.kext
- SMCBatteryManager.kext
- SMCSuperIO.kext
- Lilu.kext
- AppleALC.kext
- VoodooPS2Controller.kext
- WhateverGreen.kext
- USBPorts.kext
- EFICheckDisabler.kext
- IntelMausiEthernet.kext
- USBInjectAll.kext

### 3. Patched
- Copy patch to /ACPI/patched/
