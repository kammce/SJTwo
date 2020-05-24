# SJTwo

Open source development board for the LPC4078 microcontroller with buttons,
leds, sensors and display, used for educational purposes

## Source Files

I've made the DipTrace source files available so that you can download them,
inspect them, modify them, do whatever you want with them. They can be found in
the `diptrace/` directory. The root of the directory has the current Rev F
version of the board. All older versions can be found in the `diptrace/archives`
folder.

There is also a Segger JTAG Mini to SJTwo adapter in there as well, if you don't
want to connect header pins.

Also included are the `archives` datasheets, 3D models for the Diptrace 3D
renderer, old BOMs and the old gerbers.

Logos, images, datasheets, drawings and 3D models are owned by their respective
owners.

Forgive me for DipTrace as the files cannot be exported or converted to any
other platform, thus locking people into that ecosystem. I'd recommend EasyEDA
as an a free alternative. Fantastic web application that gets better everyday.
And if have the cash to pay for Altium, I'd recommend that.

## Ordering PCBs and BOM

Please go to this link on kitspace.org (adding link soon) to order a PCB and the
BOM.

## Developing software for the board
Go to [SJSU-Dev2](https://github.com/kammce/SJSU-Dev2/) to download the software
development kit for this board. The development platform also enables the
development of other boards and microcontrollers as well.

### Factory Testing board

A `.hex` file can be generated for the board by building the
[factory test demo](https://github.com/kammce/SJSU-Dev2/tree/master/demos/sjtwo/factory_test).

This binary can be loaded onto each chip before it is soldered onto the board.
And once the board is finished, power can be supplied to the board, and the 4
LEDs above the buttons will turn on when the test is finished. Should only take
a few seconds to complete. Serial output detailing the process can also be seen
via a serial terminal like Putty or minicom over a USB micro cable.
