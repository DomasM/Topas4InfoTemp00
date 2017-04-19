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
* beta : auto-updates active only for PCs in Light Conversion local area network


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

1. (C) Add buttons "delete current configuration" to optical and separation configurations

### Changed behaviors

1. (C) Change calibration motor curve offset control to indicator, add two new buttons : "Set offset" and "Shift curve to make offset zero". "Add current offset" button renamed to "Shift curve by current diff".
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
1. (C)(FO) "Calibration>Optical" adds current motor position instead of target when modifying motor curve
1. (C)(FO) "Tools>Create Installer with current configuration" fails with multiple self-hosted servers due too short timeout
1. (S)(FN) Before starting server with configured TCP ports, server checks if they aren't used by other applications and informs user if so instead of crashing
1. (S)(FN) When calculating motor positions for wavelength, neutral positions are used only from optical devices that are actually used to set requested wavelength
1. (FO) Device location might not work if PC isn't connected to LAN
1. (C)(FO) When connecting to new device in client application, named motor positions and forbidden ranges might not be synced
1. (C)(FO) Motor curves, if they have points with "None" interpolation, are incorrectly converted  when using SIG<>IDL conversion with explicit IDL motor curves
1. (C)(FN) "Calibration>Create/modify interaction" informs user if end wavelength<=start wavelength

### New features

1. (C) Import anything from zipped configuration. User can inform any part of optical configuration (whole optical configuration, optical device, interaction, motor curve), separation configuration (...), or motor property from zipped server configuration
1. (C) Start a new self hosted server from zipped configuration (optionally as demo, i.e. without actual hardware)
1. Forbidden motor ranges: each motor has a list of forbidden positions ranges.
If shutter is open when motor is entering forbidden range it will be closed by server and reopened after motor leaves forbidden range. Shutter can't be opened while motor is in forbidden range.
1. On hardware failure, inform user to power-cycle device, reconnect USB and restart server application (pop-up in Client)
1. Hidden motors : if motor socket is installed in Topas3 board, but there is no motor connected, you can completely hide it from clients
1. (C) "Update is available" message in title bar
1. (C) Rectangle around motor control

### Changed behavior

1. (C) All self-hosted servers in \Resources\SelfHostedServer are launched on start. Prepend '_' to folder name to ignore server (P17189 >> _P17189).
1. (C) Motor controls can be used with mouse in interactive mode ("Calibration>Optical")
1. (C) Calibration and Motors tabs are not visible in User Access Level
1. Shutter has three states: open, closed and temporarily closed. Shutter in temporarily closed state can't be opened by user, but will be opened by server after reason why it was closed is no longer valid: e.g. motor leaves forbidden range, wavelength setting is finished
1. (C) Order of named motor positions is kept unchanged after modifying position/name/short name
1. (C) To close device tab, Shift key has to be held while clicking x button
1. (S) Can't open shutter during motor reset
1. (C) Bigger Interactions and Messages buttons
