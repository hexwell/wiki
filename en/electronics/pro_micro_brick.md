# How to unbrick an Arduino Pro Micro

Arduino Pro Micros can get bricked from time to time. To unbrick:

-   Open blank sketch on Arduino IDE
-   Connect RST and GND pins. The device should reboot and appear to the OS under a different port
-   Select the new port in Arduino IDE
-   If it fails to upload launch the upload again and quickly reset the Arduino before the upload starts. If your having problems with this try to reset the board and quickly upload instead.
-   After a second the board should appear to the OS on it\'s original port. Try to upload the sketch there. If it upload your board is unbricked.
