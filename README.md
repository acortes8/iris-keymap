Keymap, hex, and all other associated files to flash the keebio iris rev5 keyboard with my preferred keymap, along with additions to implement RGB-lighting on layers, and to turn on Via support.

Two approaches when installing onto your keyboard.

1.) Use QMK Toolbox to flash the already provided hex file onto your iris. 
You have to flash both halves of the iris, it is fine to leave the halves connected while doing this.
Open QMK Toolbox, and then reset the iris using the button located under the PCB to have it show up on QMK Toolbox. Select Clear EEPROM, to wipe the the onboard memory. Select the provided hex file in QMK Toolkit, and then select Flash.
Once finished, unplug that half of the keyboard and repeat the process with the other half.
Keyboard should now have the new hex files flashed onto them and working.
To view the keymappings or change them to your preference, you can use the browser tool Via. 

2.) Use QMK MSYS to compile the provided files yourself and create a new hex file to flash instead. Doing this you can make any changes you want to the provided files like the keymap.c, config.h, or others. See QMK's tutorial on QMK MSYS for a guide.
