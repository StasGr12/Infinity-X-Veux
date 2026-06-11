# Infinity X Veux
Unofficial build of Infinity X for veux

## Flashing Instuctions
Before installing please remember that:

**YOU are choosing to make these modifications and**

**I am not responsible for bricked devices or dead SD cards**
### Prequirements:
- Unlocked Bootloader
### Instructions:
 1. Download and install:
   - [ADB & FASTBOOT](https://developer.android.com/tools/releases/platform-tools?hl=en)
   - [Google USB Drivers](https://developer.android.com/studio/run/win-usb?hl=en)
 2. Reboot the PC
 3. Download the ROM ZIP and vendor_boot.img from [releases](https://github.com/StasGr12/Infinity-X-Veux/releases) and move them to the directory with ADB & FASTBOOT
 4. Flash the vendor_boot.img and reboot to recovery:
    - Enter the directory with ADB & FASTBOOT from CMD using cd command
    - Hold power button and volume down until the screen shows FASTBOOT
    - Plug your phone to your PC via USB and run fastboot devices in the CMD
      - If it shows a device your good to go
    - Flash the vendor_boot.img
      - Run this commands in CMD:
      - fastboot flash vendor_boot_a vendor_boot.img
      - fastboot flash vendor_boot_b vendor_boot.img
    - Reboot to recovery
      - Run this command in CMD:
      - fastboot reboot recovery
 5. Install the ROM
    - When in recovery press the Factory Reset button then press format data twice
    - Press apply update button and Apply from ADB
    - Run this command in CMD:
    - adb sideload "ROM NAME".zip
    - Make sure that you replace "ROM NAME" with the real name of ROM zip file
    - Press the reboot to system button
 6. Enjoy!
