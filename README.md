# Gigabyte Z590 Vision D + i9 10900K + RX 6900 XT

![AboutThisMac](https://user-images.githubusercontent.com/23700365/135357946-539d1748-5f4a-4e8e-befb-b2119a552ab3.png)

**Latest working macOS**: 12.1
<br>
**Current OpenCore**: 0.7.6

## Complete hardware specs
- Intel i9 10900k @ stock
- Gigabyte Z590 Vision D
- WC NZXT X73
- AMD Radeon RX 6900 XT OC SE Nitro+ (PN 11308-03-20G)
- Fenvi M2 BCM94360NG - OOB
- 32GB RAM Corsair Dominator - 3400 MHz DDR4
- SSD NVME Gen4 - Seagate FireCuda 520 2Tb

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
- SMCProcessor.kext
- SMCSuperIO.kext
- USBMap.kext
- VirtualSMC.kext
- WhateverGreen.kext

## Geekbench Results:
- https://browser.geekbench.com/v5/cpu/10149829
- https://browser.geekbench.com/v5/compute/3451843
- https://browser.geekbench.com/v5/compute/3451844

## Thanks/Credits
- [Opencore Team](https://dortania.github.io/getting-started/)
- [BASE EFI - for 10th Intel Gen - Comet Lake](https://github.com/luchina-gabriel/BASE-EFI-INTEL-DESKTOP-10THGEN-COMET-LAKE)
