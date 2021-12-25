# Marlin Sovol Firmware

## To use this repository

This repository provides custom configurations for Marlin 2.0 for your Sovol SV01.

Select the branch for your printer:
- 2.0.9.3-sv01 : For Sovol SV01 without modifications
- 2.0.9.3-sv01-bltouch : For Sovol SV01 with BLTouch
- 2.0.9.3-sv01-bltouch-e3dv6 : For Sovol SV01 with BLTouch and an E3Dv6 hotend
- 2.0.9.3-sv01-silentboard : For Sovol SV01 with Silent Board
- 2.0.9.3-sv01-silentboard-bltouch : For Sovol SV01 with Silent Board and BLTouch
- 2.0.9.3-sv01-silentboard-bltouch-e3dv6 : For Sovol SV01 with Silent Board, BLTouch and E3Dv6 hotend
- 2.0.9.3-sv03-silentboard-bltouch : For stock Sovol SV03

There are no code changes in this repository. It just creates Configuration.h and Configuration_adv.h files for the printers mentioned above.

## Features that require support in Slicer or Octoprint

- Action Commands. RECOMMENDED. Install Ocotprint plugins "Action Command Notification Support" and "Action Command Prompt Support". This will allow you to start, pauze and stop queued prints in Octoprint from your LCD.
- ArcWelder support. RECOMMENDED. This feature enables your printer to print arcs, so they do not have to be passed in through many small gcode commands. This will reduce printing artefacts. For Cura, install the "Arc Welder" Cura plugin and enable "Arc Welder" and "G90 Influences Extruder" in Special Modes. Alternatively, you can install the OctoPrint plugin "ArcWelder".
- M73 progress. RECOMMENDED. Install the Octoprint Plugin "M73 Progress Plugin". This will display print progress on your LCD when printing from OctoPrint.

## Building Marlin 2.0

To build Marlin 2.0 you'll need [Arduino IDE 1.8.8 or newer](https://www.arduino.cc/en/main/software) or [PlatformIO](http://docs.platformio.org/en/latest/ide.html#platformio-ide). Detailed build and install instructions are posted at:

  - [Installing Marlin (Arduino)](http://marlinfw.org/docs/basics/install_arduino.html)
  - [Installing Marlin (VSCode)](http://marlinfw.org/docs/basics/install_platformio_vscode.html).

## Marlin Support

The Issue Queue is reserved for Bug Reports and Feature Requests. To get help with configuration and troubleshooting, please use the following resources:

- [Marlin Documentation](http://marlinfw.org) - Official Marlin documentation
- [Marlin Discord](https://discord.gg/n5NJ59y) - Discuss issues with Marlin users and developers
- Facebook Group ["Marlin Firmware"](https://www.facebook.com/groups/1049718498464482/)
- RepRap.org [Marlin Forum](http://forums.reprap.org/list.php?415)
- Facebook Group ["Marlin Firmware for 3D Printers"](https://www.facebook.com/groups/3Dtechtalk/)
- [Marlin Configuration](https://www.youtube.com/results?search_query=marlin+configuration) on YouTube

## Contributors

Marlin is constantly improving thanks to a huge number of contributors from all over the world bringing their specialties and talents. Huge thanks are due to [all the contributors](https://github.com/MarlinFirmware/Marlin/graphs/contributors) who regularly patch up bugs, help direct traffic, and basically keep Marlin from falling apart. Marlin's continued existence would not be possible without them.

## License

Marlin is published under the [GPL license](/LICENSE) because we believe in open development. The GPL comes with both rights and obligations. Whether you use Marlin firmware as the driver for your open or closed-source product, you must keep Marlin open, and you must provide your compatible Marlin source code to end users upon request. The most straightforward way to comply with the Marlin license is to make a fork of Marlin on Github, perform your modifications, and direct users to your modified fork.

While we can't prevent the use of this code in products (3D printers, CNC, etc.) that are closed source or crippled by a patent, we would prefer that you choose another firmware or, better yet, make your own.
