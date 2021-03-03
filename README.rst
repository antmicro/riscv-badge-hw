==========================
RISC-V Electronic Badge HW
==========================

Copyright (c) 2017-2021 `Antmicro <https://www.antmicro.com>`_

.. image:: Images/badge.jpg

Overview:
=========

This repository contains all the hardware design files required to build the RISC-V Electronic Badge development kit. The Badge allows for displaying text and graphics
on an e-Paper screen. The actual content to be displayed can be written to the EEPROM memory using an NFC programmer. The Badge contains a PCB module with a RISC-V based microcontroller
(SiFive's FE310) that reads the content of the EEPROM memory and transfers it to the e-Paper.

Key features:
=============

* 32-bit RISC-V based SiFive FE310 microcontroller placed on a tiny PCB module that can be re-used with a custom baseboard
* EG020BS011 2" e-Paper display
* NFC/RFID tag with 64Kbit EEPROM
* debug USB-JTAG/UART interface (FT4232H) allows the board to be used as an evaluation board
* battery powered (2x CR2032) / 5V over microUSB
* SiLabs EFR32-based ARTIK-030-AV1R IoT module with Bluetooth support (optional)

The device consists of two boards:

1. Badge board equipped with an e-Paper display and all the interfaces and peripherals (`FE310_Badge <FE310_Badge>`_ directory)
2. FE310 Module built around SiFive's FE310 RISC-V chip (`FE310_Module <FE310_Module>`_ directory)

The PCB projects were created in Altium Designer 14.1.

Software support:
=================

The software supporting this hardware platform can be found in a separate repository `here <https://github.com/antmicro/riscv-badge-application>`_.

Acknowledgements:
=================

This project was made possible thanks to the joint effort of Antmicro, SiFive and the RISC-V Foundation on the occasion of the 7th RISC-V Workshop.
If you have any questions, please write to contact@antmicro.com.

License
=======

`Apache-2.0 <LICENSE>`_
