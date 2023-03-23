## Support Monterey support Monterey support Bigsur support Bigsur

## Introduction

- Lenovo ThinkPad T480s Hackintosh EFI, based on OC, contains the basic driver, after modifying the three codes, it can be used out of the box.
- Applicable version: macOS Bigsur, macOS Monterey
- With OC boot interface theme, support WIN10 MACOS dual system security (but it is not recommended to use PD virtual machine)
- SIP is normally open/Users/baotailang/T480S-BIGSUR-EFI/README.md

## The most superior experience program

1. Replace the hard drive with Samsung SSD 970 EVO 1TB:
2. Change the network card to Fenvi BCM94352Z
3. Replace the monitor 2.5K Dolby screen, resolution 256/Users/baotailang/T480S-BIGSUR-EFI/README.md0*1440, color bit 8BIT (the original screen is only 1080p 6bit, there will be serious ribbon problems)

### SMBIOS MacBookPro15,2
- Support the new features of Monterey screen branching

### EFI self-test hardware configuration

Lenovo ThinkPad T480s

- Intel i5-8250U
- 24GB RAM (8+16)
- Samsung SSD 970 EVO 1TB
- Fenvi BCM94352Z
- 2K 8BIT screen

### Hardware usage status

* [x] Integrated graphics UHD620 3G video memory
* [x] Wired network
* [x] Wireless network (airdrop screen, airdrop)
* [x] Bluetooth
* [x] Battery status
* [x] hidpi (1440*810 perfect)
* [x] Sound
* [x] SD card read
* [x] Touchpad (multi-touch gestures are fully open)
* [x] Fn+F1-F12 PtrSc (FN shortcut keys are perfect, PtrSc support needs to set keyboard shortcuts, the default is CTRL+COMMAND+3 changed to F13)
* [x] little red dot
* [x] Thunderbolt 3 (No test, it should work well.)
* [x] Sleep/wake up/shutdown/restart (power LED, lid closing/opening are all in normal state)
* [x] Personal file safe 
* [x] All USB ports (multiple USBs will not have power supply problems)
* [x] The fan status is normal (add fan control drive/Users/baotailang/T480S-BIGSUR-EFI/README.mdr to refuse to heat)
* [] ~~Start Conversion Assistant~~ (It is recommended to use parallels desktop virtual machine to run WINDOWS)
* [] ~~ Discrete graphics card mx150~~ (No solution and no solution, only integrated graphics can be used)
* [] ~~Fingerprint Reader~~ (No solution and no solution, only password input)

## Instructions

- Copy EFI to the EFI partition Edit EFI/OC/config.plist to modify the SystemSerialNumber, SystemUUID, MLB three codes
- Change the shortcut key setting [Save the screen picture as a file] to PrtSc Note: You can see the shortcut prompt as F13

## Required tools

- one-key-hidpi: One-key open macOS HiDPI
- ThinkpadAssistant: Turn on THINKPAD to drive FN multi-function keys
- YogaSMCNC: Can control the fan speed, whether it is automatic or custom speed
- Hackintool: After opening, select the power tab and click the repair button (important, be sure to operate for a long time standby to prevent writing to the hard disk, otherwise it will not wake up)
 
## System Guide for Different System Versions

- Bigsur and Monterey uses the release version Bigsur&Monterey https://github.com/bdragonh/T480S-BIGSUR-EFI/releases
- Catalina system use release version Catalina https://github.com/bdragonh/T480S-EFI/releases/tag/Catalina

## Support Bigsur upgrade to Monterey OTA upgrade process

- Open the EFI partition and replace the EFI version to the Bigsur&Monterey version. Notice! No need to restart the system after changing!
- Search MACOS MONTEREY in APP STORT, just download and install it.

##Support for new installation of bigsur and Monterey
- Obtain an equipped USB flash disk according to the tutorial https://support.apple.com/zh-cn/HT201372
- Use the OpenCORE configurator to open the EFI partition of USB flash drive and copy the bigsur & Monterey version of EFI into it

##Known problems
- Bigsur is perfect
- There is a bug in the interval delivery of Monterey. You can't deliver files to other MacOS PCs, but you can accept files (this bug has been fed back to the developer for repair)
- If your t480s uses the original network card. You need to replace the network card or join the driver module of Intel network card and Bluetooth to connect and use Bluetooth normally

## Thanks

- MSzturc/ThinkpadAssistant https://github.com/MSzturc/ThinkpadAssistant
- daliansky/OC-little https://github.com/daliansky/OC-little
- acidanthera https://github.com/acidanthera
- All lovers of black apples in GITHUB
