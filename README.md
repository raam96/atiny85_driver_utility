# ATtiny85 USB Connectivity with Digikey Bootloader

Welcome to the ATtiny85 USB Connectivity project! This guide will walk you through the process of setting up your ATtiny85 module with the Digikey Bootloader for seamless USB connectivity.

## Purchase

Before purchasing the ATtiny85 module, ensure that it comes pre-flashed with the DigiStump Bootloader. If not, sellers might provide a blank chip, requiring an ICSP programmer to flash the bootloader. You can find the necessary files in the "Digistump_Bootloader" folder.

Assuming you have a Digikey bootloader flashed chip, let's get started!

### Driver Installation

1. Download the [ghostronics_Atiny_85 utility.zip](https://drive.google.com/drive/folders/1PtO-p04wGJjrjjJ2HX2sP6jJz13yPMmA?usp=sharing).
2. Extract the zip file using the password: `ghostronics`.
3. Inside the extracted folder "ghostronics_atiny_utility," navigate to the "Digistump_driver" folder.
4. Run "DPinst64.exe" for 64-bit OS or "DPinst.exe" for other OS, based on your system specifications.
5. Connect the device and check Device Manager under "Keyboards" to ensure proper recognition. Restart your PC if needed.

### Arduino Installation

1. Open your Arduino software.
2. Go to "File > Preferences" or press "CTRL" + ",".
3. In Preferences, find the space for "Additional Boards Manager URLs" and paste: `http://digistump.com/package_digistump_index.json`.
4. Press OK, go to "Tools > Board > Boards Manager."
5. Wait for the download to complete, then search for "Digistump" in the Boards Manager.
6. Find and install "Digistump AVR Boards."
7. Go to "Tools > Boards" and select "Digispark (default 16.5 MHz)."
8. Open the "Test_example.ino" file in the downloaded folder and compile it.

Note: Keep the device disconnected. After hitting the upload button, Arduino will prompt you to plug in the device within 60 seconds for programming. The onboard LED should flash with a 100ms delay if successful.

Happy tinkering!
