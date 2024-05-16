
<img src="http://directoutput.github.com/DirectOutput/DirectOutputR3_Small.png" alt="DirectOutput framework R3 for virtual pinball cabinets"/>

DirectOutput framework R3 for virtual pinball cabinets
======================____=============================

DirectOutput is a framework to control the toys which are installed in a virtual pinball cabinet.

Please read the documentation at http://directoutput.github.io/DirectOutput/

Updated PinballX Plugin to version 1.5:

- Added extra logging for instances when the LED matrix does not display anything. This could occur if the table does not match a ROM set up in DOF, or if the table lacks a 'PF Back PBX MX' setup in DOF, among other scenarios.
- Implemented ROM matching. It will first verify if the table has a ROM listed in the XML file and then check for a match. This improves accuracy for tables with multiple ROMs, such as ACDC. When using Database Manager, the ROM will be automatically populated from the VPT and VPX files. A Dice Coefficient fuzzy search has been integrated into the plugin for enhanced matching.
- If no matching table is found, it will default to the "PinballX MX" table within the DOF configuration, which displays the PinballX animation. This setting can be modified in the DOF config tool to display your chosen effect.

Prerequisite:

- Update your DOF with the config file from January 15, 2022, to enable this functionality.
