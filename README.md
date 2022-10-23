# GBS-control
GBS-control, https://github.com/ramapcsx2/gbs-control, is an alternative firmware for Tvia Trueview5725 based upscalers / video converter boards such as the "GBS8200".

This repository contains the boards I designed to improve my own GBS-8200 with GBS-control using ESP12/ESP-M2 modules.

# Disclaimer
This is a hobbyist project, it comes with no warranty and no support.

This board is not endorsed by firmware author, please don't bother him with issues you might have because of it.

I publish my work under the CC-BY-NC-SA license.

If you find it useful and want to reward my hard work : I am always looking for Amiga/Amstrad CPC hardware to repair and hack, please contact me.

# BOM
- 1x ESP12 or ESP-M2 module
- 1x PLCC-44 through-hole socket
- 1x 10uF 0805 capacitor
- 2x 100nF 0805 capacitors (the one on EN might be omitted)
- 4x 10K 0805 resistors (the ones on GPIO0 and GPIO0 might be omitted)

# Making it
The socket must be prepared before soldering : remove the 4 small stands inside the socket and file plastic from its top up to the contacts so the socket can plug on top of the PLCC chip without popping out. Be careful to remove plastic debris, and check its orientation before soldering under the PCB.

Check for shorts at least between power traces before applying power !

The programming port does not need to be soldered since it needs to be programmed just once : you can just hold it in place during the few seconds required for programming with an USB to serial adapter. When you want to program it, remember to short GPIO0 to ground before applying power. 

# Using it
Plug the board on the PLCC controller.

There is no need to populate P8 since it is shorted by the board. It also takes the 3.3V from the PLCC chip so no additional power connection is required.

See GBS-control wiki for software setup.

