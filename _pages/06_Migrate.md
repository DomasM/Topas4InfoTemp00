---
layout: page
permalink: /Migrate-From-WinTopas3/
---

##Instructions

### System requirements

1. Windows 7 or newer
2. Topas control board with USB connection (LPT board is not supported)

**Time requried ~ 2 minutes**


### Case A. Installation on the same PC as WinTopas3 is currently running
**Installation is non-intrusive, meaning that WinTopas3 will be able to function as earlier when WinTopas4 application is closed.**

1. [Install WinTopas4 using default settings](https://www.dropbox.com/s/54ccgxua9gch6mt/WinTopas4-setup.exe?dl=1)
1. Close WinTopas3 application if running
1. Launch WinTopas4 using icon on desktop 
1. Click 'Tools>Access Level' and enter the password for advanced user or engineer
1. Click 'Tools>Topas3>Convert Topas3 configuration'
1. Select path to the WinTopas3 configuration .ini file from the combo box, click 'Convert', click 'Launch server'.
1. Click yes when Windows UAC prompts for administrator rights. Allow all applications through firewall.
1. If you have multiple devices connected to the same PC, repeat steps 6-7 for each ini file. **Make sure to use different Topas3 API slot for each device (enter value before launching server).**
1. If you want to return to WinTopas3 usage, close server application (green icon) and start WinTopas3. Reset all motors in WinTopas3. Any changes you made in WinTopas4 won't propagate to W3 (and vice versa).


### Case B. Installation on another PC
1. Get .ini and .crv files for the device that you want to use from the PC where WinTopas3 is currently running. 
1. Install WinTopas4.  Check 'Topas3 motor board drivers' in the first dialog page.
1. Connect Topas USB cable to the new PC.
1. Follow the steps 3-9 as in Case A. You'll have to browse to the .ini files yourself in step 5 instead of selecting them from combo box. 



