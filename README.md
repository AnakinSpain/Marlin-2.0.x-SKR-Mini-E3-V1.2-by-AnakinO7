# Marlin 3D Printer Firmware

COMPILING FIRMWARE

I used VSCode with the PlatformIO extension and Git GUI.
Chris Riley VSCode installation guide for Marlin 2.0.
You can find the firmware file in Marlin/.pio/build/STM32F103RC_btt_512K/firmware.bin
FLASHING FIRMWARE

Place the firmware.bin file onto your SD card, them insert it into your printer and turn it on. After a short 20-30 sec blank screen your printer should be ready.
If after ~50-60 sec there is still a blank screen, don't worry just turn off your printer. A long blank screen could mean that the firmware you just tried is bad in some way. You could try recompiling it to see if it works.
UPDATING/REFLASHING FIRMWARE

You don't need to redo all the changes every time you want to update to a newer version of marlin, you just need to copy your edited configuration files to the new marlin and compare them in VSC Source Control (Ctrl+Shift+G), and copy anything that is new or changed to your files.
Not all changes will be applied on a firmware update, for that you will need to reset your printer settings by going in the printer menu - Configuration - Restore defaults, or by sending an M502 to the printer. It will reset your settings to your firmware defaults.

