---
layout: page
title: Changelog
permalink: /changelog/
---


**All fixes/ new features/ changed behaviours are listed from the most important to the least important**


**Currently version numbers are the same for Topas4Server and WinTopas4 (simultaneous release)**

## Abbreviations
* (C)-Client (WinTopas4): applies only to client application
* (S)-Server (Topas4 Server): applies only to server application
* (FN)-Fixed new: describes correct behavior after bug fix
* (FO)-Fixed old: describes wrong behavior before bug fix
* (PA)-Public API: applies to public API
* beta : auto-updates active only for PCs in Light Conversion local area network



## 1.7.0 (2017-09-06) (beta)

### Changed behaviors

1. (C) Change shutter button style and size, move 'Interactions' and 'Messages' buttons
1. (C) Remove button 'Shift curve by current difference' in motor curve view 
1. (C) First result of reset operation is ignored in 'Testing workbench'



## 1.6.9 (2017-09-01) 

### Fixes

1. (S)(FO) Server setting wavelength for other device on the same PC doesn't use loopback address >> no authentication




## 1.6.8 (2017-08-31) 

### Fixes

1. (S)(FO) Reset latch difference is calculated from second movement to switch

### Changed behaviors

1. (S) Direct communication with motor board using WinUSB enabled for boards with six-motor extension boards
1. (C) Various new access keys, 'Save current position' changed to Alt+P 
1. (C) NumPad keys can be used to focus motors too




## 1.6.7 (2017-08-24) 

### Fixes

1. (S)(FO) Wrong motor diagnostics status is returned for section if it contains hidden motors




## 1.6.6 (2017-08-23) 

### New Features

1. (C) User can import separation images from zipped configuration




## 1.6.5 (2017-08-21) 

### Fixes

1. (C)(FO) Affix can't be changed by entering new value, only using button 'To 0'



## 1.6.4 (2017-08-18) 

### New Features

1. Backlash compensation 
1. (C) Function to set motor affix to such value that current position is 0 units




## 1.6.3 (2017-08-16) 

### Fixes

1. (C)(FO) DIY installer creator timeouts after 5 minutes, which is too soon


### New features

1. (C) WinTopas4 can be launched with NoAutoLaunch argument (--NoAutoLaunch) to prevent self-hosts launch. 'Manage devices' tool can be used to launch device later on.



## 1.6.2 (2017-08-11) 

### Fixes

1. (C)(FO) Application might get stuck in zombie state on startup with no visible window



## 1.6.1 (2017-08-11)

### No changes



## 1.6.0 (2017-08-11) 

### Changed behaviors

1. (S) Communication with motor board using WinUSB directly (TopasAPI.dll no longer used) beta, enabled inside LC only
1. (C) Motor Diagnostics tool has nicer UI




## 1.5.2 (2017-08-09) 

### Fixes

1. (C)(FO) Application crashes if user tries to modify motor curve and this curve does not cover currently set wavelength



## 1.5.1 (2017-08-08) (beta)

### New features

1. (C) User can change serial number of device and motor board before launching device from zipped configuration



## 1.5.0 (2017-07-25) (beta)

### New features

1. Each device has a model included in configuration (Topas-Prime, Orpheus-F, etc)




## 1.4.2 (2017-07-17)

### New features

1. (S) 'Saved motor positions' service is in public API




## 1.4.1 (2017-07-13)

### New features

1. (C) Motor properties window can be opened directly from 'Testing workbench' (mouse right click)

### Changed behaviors

1. (C) Self-hosted servers can be managed with advanced user access level



## 1.4.0 (2017-07-12)

### New features

1. Add basic Pharos control from WinTopas4 via Topas4Server if connection is configured 
1. (C) Add new hotkey for shutter: Ctrl+NumPad0

### Changed behaviors

1. (C) Motor board drivers are installed by default




## 1.3.4 (2017-06-29)


### New features

1. Add 'Restart server' button to Motor Testing Workbench



## 1.3.3 (2017-06-27) (beta)


### Changed behaviors

1. Update links to web pages




## 1.3.2 (2017-06-27) (beta)


### New features

1. Add motor modules diagnostics tool ('Misc' tab, 'Diagnostics') (new unmanaged Topas3 dlls v3.3.0.52)




## 1.3.1 (2017-06-26)

### Fixes

1. (C)(FO) Tabbing navigation does not work in 'Smooth Scanner' view

### New features

1. (C) Add step scanner tool (Misc tab)



## 1.3.0 (2017-06-20)

### Changed behaviors

1. (S)(PA) Motor reset (homing) functions are exposed via public API
1. (C) Named motor positions can be modified with advanced user access level




## 1.2.11 (2017-06-15)

### Fixes

1. (C)(FN)  'Start Wavelength' in 'Create/Modify interaction' has reasonable fall-back value in case it is can be negative (i.e. using DFP)




## 1.2.10 (2017-06-12) 

### Fixes

1. (S)(FO) Device location code might cause crash when restarting server


## 1.2.9 (2017-06-07) (beta)

### Fixes

1. (C) Various 'Create/ modify interaction' wavelength range calculation improvements 




## 1.2.8 (2017-06-05)

### Changed behaviors

1. (C) Add separation configuration check for overlapping ranges




## 1.2.7 (2017-05-31)

### New features

1. (C)  Add two new demo configurations (Topas-Prime+NirUVis and Orpheus-HP)

### Changed behaviors

1. Optical devices are always kept ordered by index


## 1.2.6 (2017-05-31)

### Changed behaviors

1. (S)  Up to two successive motor board status read failures are ignored
1. (C)  Application exits point insertion mode in motor curve view when it loses visibility
1. (C)  Optical configuration checker checks for small steps that are not small enough (<=0.1 nm, but > 0.001 nm)




## 1.2.5 (2017-05-26)

### Changed behaviors

1. (S)  All motor positions are saved within five seconds after setting new target position (i.e. moving motor)
1. (C) 'Reset in progress' warning is bigger and flashing



## 1.2.4 (2017-05-25)

### Changed behaviors

1. (C) Red warning 'undefined' is no longer shown for motors with named positions which are in none of them




## 1.2.3 (2017-05-22)

### Fixes

1. (S)(FO) Server application enters infinite relaunch loop if Windows are localized and firewall permissions are missing




## 1.2.2 (2017-05-22)

### Fixes

1. (S)(FO) Wrong motor reset position difference calculation (second pass used instead of first)

### Changed behaviors

1. (C) Minor UI tweaks




## 1.2.1 (2017-05-19)

### Fixes

1. (S)(FO) Likely fixed: application might crash when restarting (System.NullReferenceException at System.Threading.Overlapped.get_iocbHelper)
1. (S)(FN) Remove unused websocket module initialization which might cause real one to become unavailable (crash before 1.2.0)
1. (C)(FO) Application crashes if user tries to add neutral position without selecting motor first
1. (C)(FO) Application crashes if user tries to open wavelength fixer tool for interaction with no calibration points that apply for fixing




## 1.2.0 (2017-05-16)

### Fixes

1. (FO) Wrong minimal motor position calculation in case negative factor is used
1. (S)(FO) When named motor position is renamed, separation configuration does not update accordingly


### New features

1. (C) After Topas3 > Topas4 conversion user can start device as demo (without using actual hardware)

### Changed behaviors

1. (C) Topas3 to Topas4 converter tries to guess named motor positions names for wavelength separators and some other motors with discrete positions
1. (C) Other minor tweaks in Topas3 to Topas4 converter
1. Add EULA to installers
2. (C) Separation configuration sanity checker for multiple entries which differ only by interaction is disabled



## 1.1.3 (2017-05-11)

### Fixes 

1. (C)(FN) When trying to delete/inactivate self hosted server from WinTopas4 check whether it has actually exited.



## 1.1.2 (2017-05-11)

### New features

1. (C) New tool to manage SelfHosted servers from WinTopas4 (Tools>Self Hosts>Manage devices).

### Changed behaviors

1. (C) Topas3 configuration converter preserves motor positions
1. (C) Topas3 configuration converter adds 127.0.0.1 to IP address white list (there is no need to authenticate after conversion)
1. (C) SelfHostedServers\Master directory is hidden



## 1.1.1 (2017-05-09)

### Fixes 

1. (FN) If connection to motor control board fails and client PC is not authenticated 'Start authentication' button is not shown

### New features

1. (S) Press F11 in server application to open Configuration\Settings folder

### Changed behaviors

1. (S) New help generator for REST services (faster startup)



## 1.1.0 (2017-05-08)

### New features

1. WinTopas4, including self hosted servers, can be updated offline by installing newest version on top



## 1.0.3 (2017-05-02)

### Fixes 

1. (S)(FO) Shutter might actually be open while control board thinks it's closed if close command is issued shortly after open command.



## 1.0.2 (2017-05-02)

### Fixes

1. (C)(FO) Respacer tool will add duplicate point under certain conditions



## 1.0.1 (2017-05-02)

### Fixes

1. (C)(FO) Position for motor curve with additive calibration is saved with no regard that it is additive when modifying motor curve in Calibration>Optical tab
1. (C)(FO) Motor curve with additive calibration is moved to wrong position when modifying interaction in Create/modify interaction tool
1. (C)(FO) Copy-pasting interaction input points does not handle decimal separator well

### New features

1. (C) Wavelength correction tool (move calibration points in all motor curves horizontally/add new point). Automated version with spectrometer in spectraLight since 2.5.0
1. (C) Respacer tool for interaction motor curves
1. (C) Arrow buttons to move named motor positions up/down in the list



## 0.9.2 (2017-04-27)

### Fixes

1. (C)(FO) Application crashes if incorrect password is provided



## 0.9.1 (2017-04-26)

No changes


## 0.9.0 (2017-04-26)

### New Feautures

1. (C) User can finish interaction modification by deleting all old points in motor curves

### Changed behaviors

1. Auto updater moved from Dropbox to Azure+GitHub.io to avoid Great Firewall of China 



## 0.8.8 (2017-04-25)

### Fixes

1. (FO) .pdb file for executable in not found by CLR, exceptions stack traces contains no line numbers (except for .dlls) 
1. (S)(FO) Under certain conditions shutter can't be opened ('due safety reasons') after setting wavelength
1. (C)(FO) Non-explicit IDL to SIG conversion creates invalid wavelength mapping curve



## 0.8.7 (2017-04-21)

### Fixes

1. (S)(FO) Timeout for motor reset is too short for slow motors with long travel range
1. (C)(FO) Feedback text box does not accept return key and does not wrap text
1. (C)(FO) It's possible to delete multiple points in motor curve and interaction views when only single point is selected
1. (C)(FO) Interaction output range sometimes is not updated in device view and interaction view 

### Changed behaviors

1. (C) Smooth scanner tool updates scan range every time new interaction is selected


## 0.8.6 (2017-04-19)

### Fixes

1. (C)(FO) Calibration editor crashes a lot if curve type is OtherDevice instead of motor



## 0.8.5 (2017-04-14) (beta), (2017-04-18)

### New features

1. (C) New tool to quickly stop motor on required position (right click on motor control and select 'Find position') 



## 0.8.4 (2017-04-14) (beta)

### Fixes

1. (C)(FO) Create/modify interaction tool crashes due invalid TwoWay binding



## 0.8.3 (2017-04-13) (beta)

### Fixes

1. (FN) user_id generator for application insights uses stable hashing algorithm
2. (S)(FN) Git index lock (might happen due crash or when creating installer) is handled by deleting index.lock file



## 0.8.2 (2017-04-12) (beta)

### Fixes

1. Various fixes/format changes in sent telemetry data

### New features

1. (C) User can send feedback straight from WinTopas4 application (if server seems reachable)



## 0.8.1 (2017-04-11) (beta)

### Fixes

1. (C)(FN) Web page for mobile clients is hosted using port RestPort+2 instead of port 80 to avoid clashes with others applications (Skype etc)
2. (S)(FN) Output metrics collector for Application Insights does not try to make sense of device state if motors are not available



## 0.8.0 (2017-04-10) (beta)

### New features

1. Application Insights

### Fixes

1. (C)(FO) CMP-SIG template in Create/modify interaction tab uses SIG as mapping wavelength mapping function
2. (C)(FO) Saved motors positions list in single device tab does not show vertical scrollbar if there isn't enough space


## 0.7.4 (2017-03-28)

### New features

1. (C) Add buttons 'delete current configuration' to optical and separation configurations

### Changed behaviors

1. (C) Change calibration motor curve offset control to indicator, add two new buttons : 'Set offset' and 'Shift curve to make offset zero'. 'Add current offset' button renamed to 'Shift curve by current diff'.
1. (C) Calibration motor curve points are always auto-ordered by wavelength, user can't reorder



## 0.7.3 (2017-03-27)

### New features

1. Add link to [Topas4 info page](https://domasm.github.io/Topas4Info/) in three different locations

### Changed behaviors

1. Beautified local (per device) API help pages, add more info to some methods



## 0.4.12 (2017-02-13) ---> 0.7.2 (2017-03-13)

### Fixes

1. (S)(FO) Decrease power on still does not work at all
1. (S)(FO) Shutter is opened when it shouldn't be:
* Open shutter
* Trigger interlock (shutter will be closed)
* Defeat interlock
* Set wavelength
* Shutter will be opened
1. (C)(FO) 'Calibration>Optical' adds current motor position instead of target when modifying motor curve
1. (C)(FO) 'Tools>Create Installer with current configuration' fails with multiple self-hosted servers due too short timeout
1. (S)(FN) Before starting server with configured TCP ports, server checks if they aren't used by other applications and informs user if so instead of crashing
1. (S)(FN) When calculating motor positions for wavelength, neutral positions are used only from optical devices that are actually used to set requested wavelength
1. (FO) Device location might not work if PC isn't connected to LAN
1. (C)(FO) When connecting to new device in client application, named motor positions and forbidden ranges might not be synced
1. (C)(FO) Motor curves, if they have points with 'None' interpolation, are incorrectly converted  when using SIG<>IDL conversion with explicit IDL motor curves
1. (C)(FN) 'Calibration>Create/modify interaction' informs user if end wavelength<=start wavelength

### New features

1. (C) Import anything from zipped configuration. User can inform any part of optical configuration (whole optical configuration, optical device, interaction, motor curve), separation configuration (...), or motor property from zipped server configuration
1. (C) Start a new self hosted server from zipped configuration (optionally as demo, i.e. without actual hardware)
1. Forbidden motor ranges: each motor has a list of forbidden positions ranges.
If shutter is open when motor is entering forbidden range it will be closed by server and reopened after motor leaves forbidden range. Shutter can't be opened while motor is in forbidden range.
1. On hardware failure, inform user to power-cycle device, reconnect USB and restart server application (pop-up in Client)
1. Hidden motors : if motor socket is installed in Topas3 board, but there is no motor connected, you can completely hide it from clients
1. (C) 'Update is available' message in title bar
1. (C) Rectangle around motor control

### Changed behavior

1. (C) All self-hosted servers in \Resources\SelfHostedServer are launched on start. Prepend '_' to folder name to ignore server (P17189 >> _P17189).
1. (C) Motor controls can be used with mouse in interactive mode ('Calibration>Optical')
1. (C) Calibration and Motors tabs are not visible in User Access Level
1. Shutter has three states: open, closed and temporarily closed. Shutter in temporarily closed state can't be opened by user, but will be opened by server after reason why it was closed is no longer valid: e.g. motor leaves forbidden range, wavelength setting is finished
1. (C) Order of named motor positions is kept unchanged after modifying position/name/short name
1. (C) To close device tab, Shift key has to be held while clicking x button
1. (S) Can't open shutter during motor reset
1. (C) Bigger Interactions and Messages buttons
