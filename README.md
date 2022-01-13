# Firmware For JGMaker Magic with MKS Robin Pro Board
![GitHub](https://img.shields.io/github/license/JGMaker3dofficial/artistd.svg)
## Official JGMaker ArtistD Firmware 
* Get the latest release of the Official Firmware: https://github.com/JGMaker3dofficial/artistd/releases/latest
## Official JGMaker Magic Firmware 
* Get the Official Firmware: https://github.com/JGMaker3dofficial/magic
## MKS Robin Pro Pinouts
[MKS Robin Pro Pinout](https://github.com/makerbase-mks/MKS-Robin-Pro/blob/master/hardware/MKS%20Robin%20Pro%20V1.0_001/MKS%20Robin%20Pro%20V1.0_001%20PIN.pdf)

## Setting up the new board

1.  Label all the wires as you remove them from the hotend connector.
2.  Fan connections only have a negative wire.
3.  The X-Endstop Ground wire is shared with the TH1- wire. If you reverse the TH1 - and + wires you will throw a thermal error when you trigger the X-Endstop connection.  Fix by reversing the TH1 wires.
4. 
### Mounting the board

1. Included in this project is a very basic mount 'MKS_Robin_Pro_Mount.stl'.  The board is mounted offset from the original alignment because the USB and Card slots cant align with this board.  There is enough offset to connect a usb cable and be able to slide the SD Card in and out of the slot.
2. Attach the board to the mount using (4) M3x8mm Screws with M3 nuts on the back.
3. Use 3 old board screws to secure the mount to the frame. The 4th hole under the new board will remain unattached, but doesnt affect the secureness of the mount.
### Hotend Pinout
                      Connector Clip Orientation -->
                      +--------+
                 X-S  |1*     6|  TH1+ (PC1)
      TH1-/X-G (PC1)  |2      7|  J1- (12/24v)
         HE0+ (PF10)  |3      8|  PB1- (FAN)
         HE0+ (PF10)  |4      9|  HE0- (PF10)
         HE0+ (PF10)  |5     10|  HE0- (PF10)
                      +--------+
             
### Bed Pinout

1. Connect both Red Wires together into PA0-.
2. Connect both Black Wires together into PA0+.
3. Connect the two remaining White wires to TB(PC0) for Bed Thermistor ( you will need to extend the length of these two wires so that the bed can freely move back and forth without pulling these wires tight).

## Current Status
This version of the firmware is based from the 2.0.7.2 Version of Marlin. 

## Getting the Upstream Marlin
There are some instructions here for setting your repository with the upstream Marlin Source. 
https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/configuring-a-remote-for-a-fork

$ git remote add upstream https://github.com/MarlinFirmware/Configurations.git

Thie will set an upstream remote that you can fetch and merge from. 

#Join the Community
[Checkout our Discord Server](https://discord.gg/H97VgdSwjF)
