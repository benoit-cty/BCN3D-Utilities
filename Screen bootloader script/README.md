## Screen Bootloader script

This script is needed as the 4D systems displays come preloaded with a factory firmware.
As we store all the files in the microSD card and not in the flash memory, we need to tell the display to get the files from the microSD card.
This is done through this script.

### Run the script for multiple screen

1. Connect all the displays you have via usb using the FTDI converter board.
2. Find out the COM ports assigned to them by running ``mode`` on cmd.
3. Open the file ``ScreenBootloaderScript.bat`` and replace the COM ports numbers where the X are
4. Fire up a command line prompt and go to the ``/BCN3D-Utilities/Screen bootloader script/``
5. Run the ``.bat`` script
6. After a few seconds, all the displays should display a black background and a gren flashing text saying "Drive not mounted"
7. DONE 

## Another, maybe easiest way for one screen
1. Connect all the displays you have via usb using a 5V FTDI converter board.
2. Install the 4D Workshop 4 IDE https://www.4dsystems.com.au/product/4D_Workshop_4_IDE
3. Launch the application named "Program Loader" in the Windows start menu.
4. Then select the FTDI COM port in the IHM.
5. Load the temp4D.4XE of this repository. Make sure the temp4D.cfg file is in the same directory
6. Click on OK
7. DONE
