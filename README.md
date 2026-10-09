# Debug-Boards

This repository contains the hardware designs for our integrated debug probe, debug adapter, flex debug cables and RF calibration board.

## 📦 Contents

This repository includes designs for:

*   **Flex debug cable**: Flexible flat cable that connects a debugger to the low-profile debug connector on the target board.
*   **Debug Adapter**: SWD debug adapter board that breaks the target debug connector out to a standard debug host, with its own target power supply.
*   **Integrated Debugger**: Integrated debug probe for flashing and debugging target hardware over SWD, with a UART bridge and switchable target power. It is hardware compatible with the [Black Magic Debug](https://black-magic.org/) firmware.
*   **RF VNA calibrator**: Calibration board for vector network analyzer (VNA) RF measurements.

Each subdirectory is a standalone KiCad project with its schematics and PCB layout, and a `production` folder with the manufacturing files (gerbers, BOM, pick-and-place positions) of the released revisions.

The projects use the symbol, footprint and 3D model libraries from [Hardware-Resources](https://github.com/PicoballoonLabs/Hardware-Resources).

## 🔌 Integrated Debugger firmware

No firmware is distributed in this repository. The Integrated Debugger runs the upstream [Black Magic Debug](https://github.com/blackmagic-debug/blackmagic) firmware (GPLv3), which can be installed and updated with [bmputil](https://github.com/blackmagic-debug/bmputil).

## 📄 Licence

The hardware designs in this repository are released under the MIT Licence, see [LICENSE](LICENSE).
