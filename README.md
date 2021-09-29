# Hackintosh: Gigabyte Z590 Vision D + i9 10900K + RX 6900 XT

Intel 10900k, Z590 Vision D, RX 6900XT Nitro+

**Latest working macOS**: 11.6

**Current OpenCore**: 0.7.3

Complete hardware specs:
- Intel 10900k @ stock
- Gigabyte Z590 Vision D
- WC NZXT X73
- AMD Radeon RX 6900 XT OC SE Nitro+
- Fenvi M2 BCM94360NG - OOB
- 32GB RAM - 3400 MHz DDR4
- SSD NVME Gen4 - Seagate FireCuda 520 2Tb

**SMBIOS**: iMacPro1,1

The system dual boots Windows 10

## Get it running
0. Make sure to update your BIOS, disable VT-d, disable CSM support and enable XHCI Hand-off (for Airdrop/Continuity/Sidecar)
1. Generate a new serial number, motherboard id, ROM (that's your mobo's mac address without dots) and SMUUID (make sure serial number is **invalid** in order to iMessage/Facetime to work) ([how?](https://dortania.github.io/OpenCore-Install-Guide/config.plist/comet-lake.html#platforminfo) + [this tool](https://mackie100projects.altervista.org/download-opencore-configurator/))
2. Boot the new macOS partition

## What works
- macOS Big Sur, macOS Catalina and macOS Monterey
- WiFi and Bluetooth + Airdrop + Sidecar + Continuity
- Audio
- HDMI/DP (OOB thanks to 6900 XT)
- All USB ports
- 2x 2.5Gbit Ethernet
- Everything iCloud related (Drive, iMessage, Facetime, unlock with Apple Watch, etc)
- Temperature monitoring for everything except GPU (no GPU temp support in VirtualSMC for navi and big navi cards)
- DRM content (Netflix, ATV+, Airplay 2 mirroring etc)
- Shutdown/Reboot/Update to newer macOS builds over time

## What doesn't work
- Sleep? Never got the chance to test it, my hackintosh is up 24/7

## Kexts used:
- Lilu.kext
- NVMeFix.kext
- RestrictEvents.kext
- SMCProcessor.kext
- SMCSuperIO.kext
- USBMap.kext
- VirtualSMC.kext
- WhateverGreen.kext

## Drivers used:
- OpenCanopy.efi (required by OpenCore)
- OpenRuntime.efi (required by OpenCore)
- HFSPlus (optional, make HFS drives discoverable in OpenCore bootloader if you want to use Mojave or older macOS versions)

## Geekbench Results:
https://browser.geekbench.com/v5/cpu/10149829
<br>
https://browser.geekbench.com/v5/compute/3451843
<br>
https://browser.geekbench.com/v5/compute/3451844

## Thanks/Credits
- [Opencore Team](https://dortania.github.io/getting-started/)
