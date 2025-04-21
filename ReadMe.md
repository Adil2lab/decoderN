##               vJoy installation##
Please READ instructions in [vJoy site](http://vjoystick.sourceforge.net/site/index.php)

[Do not hesitate to contact me](mailto://shaul_ei@users.sourceforge.net)

---------------------------------------------------------
# Release notes for 16-Jul-2018 #

**v2.1.9 Build 1 - Windows 10 Compatibility Issues fixed**

Created and signed by **jshafer817** 

For additional info go to: [vJoy on GitHub](https://github.com/jshafer817/vJoy)

---------------------------------------------------------
# Release notes for 27-May-2018 #

**v2.1.8 Build 39 - Windows 10 (1803) bug fix **

**Problem**: 
When moving to Windows 10 release 1803 some users found that vJoy driver stopped functioning. This was manifested in cases where vJoy devices were configured with zero buttons.

**Fix**: This version of vJoy include configuration apps that do not cause such a problem.

**Recovery**: Before installing this version of vJoy make sure the previous configuration (if causes problems) is removed: Run vJoyConfig -r then install this version of vJoy.

**Status:**
Fixed

---------------------------------------------------------
# Release notes for 19-Apr-2017 #

**v2.1.8 Build 38 - FFB Spring Effect **

**Bug description:**
Spring effect was not properly detected by system due to erroneous commenting out of the spring entries in the INF file

**Status:**
Fixed

---------------------------------------------------------
# Release notes for 21-Mar-2017 #

**v2.1.8 Build 37 - Efficiency Improvement**


---------------------------------------------------------
# Release notes for 10-Mar-2017 #

**Bug description:**
Under heavy load vJoy sends arbitrary and momentary data to causing a glitch in the device position.

**Status:**
Fixed



---------------------------------------------------------
# Release notes for 01-Jan-2017 #
vGen interface DLL was added to installation

---------------------------------------------------------
# Release notes for 29-Nov-2016 #

## Version 2.1.8  ##

- Enhancement: New interface function GetOwnerPid(). 
 This function returns the ID of the process owning a specified vJoy device. You can use this function to:
     * Make sure that your process is indeed the owner of a device.
     * Get the process that prevents you from acquiring the device and issue an intelligent message to the user.
     * Facilitate killing zomby processes that still own a device.

- Enhancement: vJoyList - a utility that lists all vJoy devices and specifies the owner of each device. vJoyList is part of the installation.

- Enhancement: Smoother initialization of a vJoy device. A device is initialized when created, configured or requested to from the API. It retains its position when acquired to prevent a glitch.

-  Bug Fix: Initializing discrete POVs to non-default values was incorrectly done.
It is now possible: Discrete POV registry values are now:
     * 0x80: North/Forwards
     * 0x81: East/Right
     * 0x82: South/Backwards
     * 0x83: West/Left
     * 0x8F: Neutral Point



---------------------------------------------------------
# Release notes for 26-Sep-2016 #

## Version 2.1.7  ##

This release accumulates small improvements and bug fixes:

- Fixes bugs in the API - should improve feeder stability

- Improved Reset behaviour

Known Problem:
Reset/Initialize of discrete POVs from the registry is not functional

---------------------------------------------------------
# Release notes for 03-Feb-2016 #

## Version 2.1.6 Build 20 ##

This is a **minor** release that:

- Fixes bugs in the Kernel - should improve driver stability

- Fix bug in the **C# wrapper** DLL (Thank you Thierry) - Button 128 was interpreted as button 63.

- Fix bug in uninstaller - removing vJoy sometimes left Ghost devices on the system.

- Fix bug in installer - In rare cases, the installed would indicate failed after a successful installation

---------------------------------------------------------
# Release notes for 22-Jan-2016 #

## Version 2.1.6 Build 6 ##

This is a **minor** release that fixes minor problems and also:

- Improved JoyMonitor included

- Better file versioning.

- Tested for Windows 10 (Fixing a few bugs)

- Solves some of the cases where the installer just waits forever

- Installation on Vista may now require rebooting

- Installer supports flag VERYSILENT

**Note**: If you are happy with the currently installed  vJoy - no need to install this minor release

---------------------------------------------------------
# Release notes for 08-Oct-2015 #

## Version 2.1.6 ##

**Here are the key features for the first release:**


- Based on vJoy version 2.0.5.

- Extensive support for Force Feedback (FFB).

- Backward compatible with vJoy 2.0.x.

- Configurable Initial Positions

- Enable/Disable driver from vJoyConf

- Customized installation

- Tested on Windows 7, Windows 8, Windows 8.1 and Windows 10 

**In the near future:**


- SDK

- Documentation: New how-to-write-a-feeder manual

- Update site

**For the next build:**


- Bug fixes

- vJoyConfig (command-line update)



