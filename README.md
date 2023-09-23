# A-GPS-Locked-Frequency-Counter-Frequency-Standard-by-WA2FZW

This project is a GPS locked combination frequency counter/frequency standard.

It's designed to work with the QRP Labs QLG1 GPS Kit. It runs on an Arduino
Nano and uses a 4x20 LCD display. An Si5351 module is used as the frequency
standard.

Included is the software for the "GPS_Counter" program, a document that
describes how to build and operate it and the Gerber files for the printed
circuit board.

A second program, "Where_MI" can be run on the same hardware and provides
traditional GPS functionality.

Version 2.9 fixes a bug that was causing the time to be over a second behind
the actual time. The time is still a couple hundred milliseconds behind due
to the delay between when the QRP Labs GPS module sends the 1PPS pulse and
when it sends the time data message, but I can't do anything about that!

Version 3.0 fixes a bug that was causing the gate time button to not work
correctly and added code to make the gate LED work (somehow it was left
out in Version 2.9).

IMPORTANT: There is a serious unresolved issue! The code will not work
correctly on an Arduino Nano using the "New" bootloader. I'm still
working on this.

I also added the ZIP file for the PCF8574 library as the actual library
location (https://github.com/RobTillaart/Arduino/tree/master/libraries/PCF8574)
doesn't seem to have the button to download a ZIP file.

Where_MI Version 2.1 Uploaded Sept 23, 2023

    The computations for the grid square were all
    screwed up! It worked at my home location but
    not some others. I re-did the computations and
    tested the logic for a half dozen locations
    around the world. Seems to be fixed now.

Enjoy!

John - WA2FZW
