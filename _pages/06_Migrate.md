---
layout: page
title: Migrate from WinTopas3
permalink: /Migrate-From-WinTopas3/
---




## Why upgrade to WinTopas4?

**Access most often used functions quicker and easier!**
<img src="https://lightconupdater.blob.core.windows.net/topas4infopage/Images/Migrate-From-WinTopas3/01.png" alt="" usemap="#map1494520202657">
<map id="map1494520202657" name="map1494520202657"><area shape="rect" coords="93.015625,894.015625,777.015625,996.015625" title="" alt="" href="http://domasm.github.io/Topas4Info/How-Tos/#Vid001" target="_blank"></map>

**Control multiple devices from the same window**
![02](https://lightconupdater.blob.core.windows.net/topas4infopage/Images/Migrate-From-WinTopas3/02.png)

**You can even control Topas/Orpheus from your smartphone**


<div style="display:flex; flex-direction: row; justify-content: left; align-items: left">
     <a href='https://play.google.com/store/apps/details?id=com.LightConversion.WinTopas4&utm_source=topas4info&pcampaignid=MKT-Other-global-all-co-prtnr-py-PartBadge-Mar2515-1'><img height="82" alt='Get it on Google Play' src='https://lightconupdater.blob.core.windows.net/topas4infopage/Images/Migrate-From-WinTopas3/google-play-badge.png'/></a>

<a href="https://itunes.apple.com/us/app/evernote/id281796108?mt=8" style="display:inline-block;overflow:hidden;background:url(https://linkmaker.itunes.apple.com/assets/shared/badges/en-us/appstore-lrg.svg) no-repeat;width:270px;height:80px;background-size:contain;"></a>
</div>


**Better support for interactions with overlapping wavelength ranges**



<img src="https://lightconupdater.blob.core.windows.net/topas4infopage/Images/Migrate-From-WinTopas3/04.png" alt="" usemap="#map1494523577671">
<map id="map1494523577671" name="map1494523577671"><area shape="rect" coords="1071.000081046875,981.0000200117188,1924.6667470468751,1172.6666860117189" title="" alt="" href="http://domasm.github.io/Topas4Info/How-Tos/#Vid002" target="_blank"><area shape="rect" coords="1243.000081046875,603.0000200117188,1954.6667470468751,738.6666860117189" title="" alt="" href="http://domasm.github.io/Topas4Info/How-Tos/#Vid006" target="_blank"></map>


**Easier and faster calibration modification**
![05](https://lightconupdater.blob.core.windows.net/topas4infopage/Images/Migrate-From-WinTopas3/05.png)

**Smooth wavelength scanner: scan selected wavelength range to achieve quasi-broadband spectrum**
<video  controls="controls">
<source src="https://lightconupdater.blob.core.windows.net/topas4infopage/Videos/SmoothScannerQuickDemo.mp4" type="video/mp4" />
</video>

**And many other reasons:**

1. WinTopas4 looks great on high resolution, high dpi screens
1. Non-intrusive automatic software updates
1. Forbidden motor position ranges increase user safety and lower risk of accidental device damage (need to be configured after migration)
1. Smart integrated device configuration backups every 15 minutes
1. Extensive calibration sanity checks help to avoid common mistakes when creating/modifying interactions
1. All upcoming features will be available only in WinTopas4 



## Instructions

### System requirements

1. Windows 7 or newer
1. Administrator rights (for installation and first launch only)
1. Topas control board with USB connection (LPT board is not supported)
1. Topas/Orpheus device manufactured or serviced in 2011 or later ([contact Light Conversion for earlier devices](mailto:support@lightcon.com), as there might be conversion problems)


**Time required ~ 2 minutes**


### Case A. Installation on the same PC as WinTopas3 is currently running
**Installation is non-intrusive, meaning that WinTopas3 will be able to function as earlier when WinTopas4 application is closed.**
 


1. [Install WinTopas4 using default settings](https://lightconupdater.blob.core.windows.net/installers/WinTopas4-setup.exe)
1. Close WinTopas3 application if running
1. Launch WinTopas4 using icon on desktop 
1. Click 'Tools>Access Level' and enter the password for advanced user or engineer
1. Click 'Tools>Topas3>Convert Topas3 configuration'
1. Select path to the WinTopas3 configuration .ini file from the combo box, click 'Convert', click 'Launch server'.
1. Click yes when Windows UAC prompts for administrator rights. Allow all applications through firewall.
1. If you have multiple devices connected to the same PC, repeat steps 6-7 for each ini file. **Make sure to use different Topas3 API slot for each device (enter value before launching server).**
1. Enjoy! All motor settings and calibration curves have been imported!

**Video for case A:**

<video  controls="controls">
<source src="https://lightconupdater.blob.core.windows.net/topas4infopage/Videos/HowToConvertFromTopas3.mp4" type="video/mp4" />
</video>


### Case B. Installation on another PC
1. [Install WinTopas4 using default settings](https://lightconupdater.blob.core.windows.net/installers/WinTopas4-setup.exe)
1. Get .ini and .crv files for the device that you want to use from the PC where WinTopas3 is currently running. 
1. Connect Topas USB cable to the new PC.
1. Follow the steps 3-9 as in Case A. You'll have to browse to the .ini files yourself in step 5 instead of selecting them from combo box.

## Q&A

**1. I have multiple .crv files for the same stage (e.g. Mixer2). I see that interactions have been imported only from the one of them!**

You can easily import additional curves from .crv files after conversion. See video below.

<video  controls="controls">
<source src="https://lightconupdater.blob.core.windows.net/topas4infopage/Videos/HowToImportCalibrationFromWinTopas3CRVFiles.mp4" type="video/mp4" />
</video>

**2. Can I quickly return to WinTopas3 if something goes wrong?**

Close Topas4 applications (especially servers, the green ones) and start WinTopas3. Reset all motors in WinTopas3. Any changes you made in WinTopas4 won't propagate to WinTopas3 (and vice versa).

**3. It looks like some interactions have lost calibration curves for some motors (e.g. SIG used to have 5 motor curves, and now only has 3). Is this is a bug?**

If you inspect interaction under 'Calibration>Optical' you might think that not all motor curves have been imported. Instead, they have been imported and converted to separation configuration ('Calibration>Separation'). You do not need to take any further steps, motors will move to correct positions when setting wavelength.


**4. I see orange\red exclamation marks near 'Calibration' tab. What do they mean?**

WinTopas4 performs sanity checks on calibration. Orange exclamation marks are used to denote possible mistakes and give suggestions. Red exclamation marks are used to denote 100% configuration mistakes. Hover over exclamation mark or click on it to read detailed descriptions what's wrong and learn how to fix the issues.


**5. After conversion some of the motors have named positions like 'P 1678'. What does that mean? Can I change their names?**

WinTopas3 to WinTopas4 converter tries to extract discrete motor positions from staircase-like calibration curves and give them meaningful names. This is not always possible, so some motors end up with the named positions like 'P 1678', which is simply motor position in steps when this position is set. See video ['Rename named motor positon'](http://domasm.github.io/Topas4Info/How-Tos/Calibration#Vid005) to learn how to give more meaningful names. Separation configuration will be updated automatically.

**6. Are interaction comments from WinTopas3 gone?**

Yes.

**7. So where is WinTopas4 installer?**

See the first step of the instructions above.
