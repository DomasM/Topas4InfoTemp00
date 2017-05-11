---
layout: page
title: Migrate from WinTopas3
permalink: /Migrate-From-WinTopas3/
---


## Why upgrade to WinTopas4?

**Access most often used functions quicker and easier!**
<img src="https://www.dropbox.com/s/k700nsnhbi6glwx/01.png?dl=1" alt="" usemap="#map1494520202657">
<map id="map1494520202657" name="map1494520202657"><area shape="rect" coords="93.015625,894.015625,777.015625,996.015625" title="" alt="" href="http://domasm.github.io/Topas4Info/How-Tos/#Vid001" target="_blank"></map>

**Control multiple devices from the same window**
![02](https://www.dropbox.com/s/obmyvi5hsar11gk/02.png?dl=1)

**You can even control Topas/Orpheus from your smartphone**
![03](https://www.dropbox.com/s/l0t48t7dhe9ixr7/03.png?dl=1)


**Better support for interaction with overlapping wavelength range**
<img src="https://www.dropbox.com/s/30pyuxsdojva235/04.png?dl=1" alt="" usemap="#map1494523577671">
<map id="map1494523577671" name="map1494523577671"><area shape="rect" coords="1071.000081046875,981.0000200117188,1924.6667470468751,1172.6666860117189" title="" alt="" href="http://domasm.github.io/Topas4Info/How-Tos/#Vid002" target="_blank"><area shape="rect" coords="1243.000081046875,603.0000200117188,1954.6667470468751,738.6666860117189" title="" alt="" href="http://domasm.github.io/Topas4Info/How-Tos/#Vid006" target="_blank"></map>


**Easier and faster calibration modification**
![05](https://www.dropbox.com/s/3qeoh3d1s5exuha/05.png?dl=1)

**Smooth wavelength scanner: scan selected wavelength range to achieve quasi-broadband spectrum**
<video  controls="controls">
<source src="https://www.dropbox.com/s/2dfh3g3cn7zvqs1/HowToUserSmoothScanner.mp4?dl=1" type="video/mp4" />
</video>

**And many other reasons:**

1. WinTopas4 looks great on high resolution, high dpi screens
1. All upcoming features will be available only in WinTopas4 
1. ...?



## Instructions

### System requirements

1. Windows 7 or newer
2. Topas control board with USB connection (LPT board is not supported)

**Time required ~ 2 minutes**


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
1. Enjoy! All motor settings and calibration curves have been imported!


### Case B. Installation on another PC
1. Get .ini and .crv files for the device that you want to use from the PC where WinTopas3 is currently running. 
1. Install WinTopas4.  Check 'Topas3 motor board drivers' in the first dialog page.
1. Connect Topas USB cable to the new PC.
1. Follow the steps 3-9 as in Case A. You'll have to browse to the .ini files yourself in step 5 instead of selecting them from combo box.

## Q&A

**1. I have multiple .crv files for the same stage (e.g. Mixer2). I see that interactions have been imported only from the one of them!**

You can easily import additional curves from .crv files after conversion. See video ['Import interactions from WinTopas3 .crv files'](http://domasm.github.io/Topas4Info/How-Tos/#Vid006)

**2. Can I quickly return to WinTopas3 if something goes wrong?**

Close Topas4 applications (especially servers, the green ones) and start WinTopas3. Reset all motors in WinTopas3. Any changes you made in WinTopas4 won't propagate to WinTopas3 (and vice versa).

**3.After conversion some of the motors after have named positions. Can I change their names?**




