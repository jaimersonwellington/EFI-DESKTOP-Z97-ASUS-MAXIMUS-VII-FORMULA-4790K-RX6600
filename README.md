# Asus Maximus VII Formula + Intel i7 4790K + ASUS Radeon RX 6600 Dual V3 8 GB + BCM4352HBM

![about-12 3 1](https://github.com/jaimersonwellington/EFI-DESKTOP-Z97-ASUS-MAXIMUS-VII-FORMULA-4790K-RX6600/blob/main/Screenshots/Screenshot%202026-03-14%20at%2017.44.29.png)

**Latest working macOS**: 26.3.1 SMBIOS MacPro7,1
<br>
**Current OpenCore**: 1.0.7

## Complete hardware specs
- Intel i7 4790K
- Asus Maximus VII Formula @ BIOS 3503
- RX 6600 ASUS Radeon RX 6600 Dual V3 8 GB (Asus - PN: 90YV0GP3-M0NA00)
- 4x 8Gb DDR3 1866Mhz with XMP Enabled
- Wifi/BT BCM4352HBM

## What works
- macOS Sonoma, macOS Sequoia and macOS Tahoe
- Audio
- HDMI/DP (in dGPU) (in iGPU, Sonoma and Sequoia)
- All USB ports
- Wifi/BT (in order) (boot-args -amfipassbeta)
	- IOSkywalkFamily.Kext - MinK 23.0.0 MaxK 25.99.99
	- IO80211FamilyLegacy.kext - MinK 23.0.0 MaxK 25.99.99
	- IO80211FamilyLegacy.kext/Contents/PlugIns/AirPortBrcmNIC.kext - MinK 23.0.0 MaxK 25.99.99
	- AMFIPass.kext - MinK 23.0.0
	- AirportBrcmFixup.kext - MinK 12.0.0
	- AirportBrcmFixup.kext/Contents/PlugIns/AirPortBrcmNIC_Injector.kext - MinK 20.0.0 
	- BlueToolFixup.kext - MinK 21.0.0
	- BrcmFirmwareData.kext
	- BrcmPatchRAM3.kext
- DRM content (Netflix, ATV+, Airplay 2 mirroring etc)
- Shutdown/Reboot/Sleep/Update

## Kexts used (in order):
- Lilu.kext
- VirtualSMC.kext
- WhateverGreen.kext
- AppleALC.kext
- SMCProcessor.kext
- SSMCSuperIO.kext
- CPUFriend.kext
- CPUFriendDataProvider.kext
- IntelMausi.kext
- HoRNDIS.kext
- USBMap.kext
- IOSkywalkFamily.kext
- IO80211FamilyLegacy.kext
- IO80211FamilyLegacy.kext/Contents/PlugIns/AirPortBrcmNIC.kext
- AMFIPass.kext
- AirportBrcmFixup.kext
- AirportBrcmFixup.kext/Contents/PlugIns/AirPortBrcmNIC_Injector.kext
- BlueToolFixup.kext
- BrcmFirmwareData.kext
- BrcmPatchRAM3.kext
- RestrictEvents.kext
- FeatureUnlock.kext

## Geekbench Results:
- https://browser.geekbench.com/v6/cpu/17070439
- https://browser.geekbench.com/v6/compute/6010338
- https://browser.geekbench.com/v6/compute/6010296

## Thanks/Credits
- [Opencore Team](https://dortania.github.io/getting-started/)
- [Gabriel Luchina](https://github.com/luchina-gabriel/RP-CORE)
