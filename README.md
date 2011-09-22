AVR MICRO USB
==========


This project is a small USB key based on Atmel ATtiny45-like microcontrollers.

License
-------

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 2 of the License, or
(at your option) any later version.

Contents
--------

    COPYING     text version of the GPL
    README      this file
    firmware/   source directory for firmware files
    hardware/   source directory for the hardware design files

Firmware
--------

Building requires an avr-gcc toolchain, in the firmware/ directory, to build
run:

    make main.hex

Flashing the firmware on the device requires avrdude and a compatible hardware
programmer. Default configuration is stored at the beginning of the Makefile.
To program with the default configuration, run:

    make flash

Fuses can be configured running:

    make fuses

Hardware
--------

All hardware files (schematic, layout and libraries) are in CadSoft Eagle
format.
