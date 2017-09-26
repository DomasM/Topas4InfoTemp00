---
layout: page
title: Calibration How-Tos
permalink: /How-Tos/Calibration/
nolink: true
---



### <a name="Vid001"></a>Modify calibration
<button class="btn" data-clipboard-text="{{site.fullUrl}}{{page.url}}#Vid001">
    Copy address to this how-to
</button>
<video  controls="controls">
<source src="https://lightconupdater.blob.core.windows.net/topas4infopage/Videos/ModifyCalibration.mp4" type="video/mp4" />
</video>

Advanced user or service access level required.
**All calibration modification hotkeys can be found by pressing question button mark next to motor name**
1.	Go to 'Calibration' >> 'Optical'.
2.	Locate the interaction you want to modify.
3.	Choose motor you want to modify, select point from the graph or from the table below.
4.	Press keyboard button 'M', software will set the point you selected.
5.	Adjust the motor by pressing buttons 'Up', 'Down', 'Left' or 'Right' (also 'Page Up' and 'Page Down' for coarse adjustment).
6.	Press 'Enter' to save changes for that motor position. 
7.	Repeat steps 3-6 for other motors for the same calibration point.
Alternatively you can adjust all motors for the point you modify and save all changes at once by following this:
1.	First of all choose a motor and a point you want to start from.
2.	Press keyboard button 'M', software will set the point you selected.
3.	Using keyboard shortcuts 'Alt+[number]' (from 1 to 9 and 0), activate motor you want to adjust. 'Alt+1' will activate 1st motor from the list, 'Alt+5' - 5th and so on. 'Alt+0' will activate 10th motor and there is no keyboard shortcut to select the motors above 10.
4.	Adjust each motor, required to optimize calibration point, move between motors as many times as you need.
5.	Press 'Alt+Enter' to save all adjusted motor positions for the point you are modifying and move to the next point.
6.	Repeat steps 3-5 until all points are recalibrated. No additional save procedure is required, as system already updates tuning curve once you save modified point by pressing 'Enter' or 'Alt+Enter'.


### <a name="Vid002"></a>Correct interaction wavelengths to match actual output
<button class="btn" data-clipboard-text="{{site.fullUrl}}{{page.url}}#Vid002">
    Copy address to this how-to
</button>
<video  controls="controls">
<source src="https://lightconupdater.blob.core.windows.net/topas4infopage/Videos/CorrectWlsManual.mp4" type="video/mp4" />
</video>


Advanced or service user level required together with the spectrometer to measure actual OPA output wavelength.
1.	Go to 'Calibration' >> 'Optical'.
1.	Choose interaction, usually for Signal - 'SIG'.
1.	Below the graph near the pump wavelength window locate button 'Correct wavelengths' and press it.
1.	Measure actual output wavelength at the selected point using spectrometer.
1.	Put measured value in the 'Measured wavelength'.
1.	Press 'Change and next' (or use shortcut 'Alt+Enter') to move to the next point.
1.	Repeat steps 4-6 for all points in the tuning curve.


### <a name="Vid003"></a>Respace tuning curve points
<button class="btn" data-clipboard-text="{{site.fullUrl}}{{page.url}}#Vid003">
    Copy address to this how-to
</button>
<video  controls="controls">
<source src="https://lightconupdater.blob.core.windows.net/topas4infopage/Videos/RespaceWls.mp4" type="video/mp4" />
</video>

Advanced user or service access level required. This procedure is usually performed after Signal wavelengths correction.
1.	Go to 'Calibration' >> 'Optical'.
2.	Choose interaction, usually for Signal - 'SIG'.
3.	Below the graph near the pump wavelength window locate button 'Respace points' and press it.
4.	Choose start and end wavelength points together with the step size, press 'Respace' (consult support team for proper tuning curve spacing).
Depending on the corrections it might be necessary to re-optimize individual points from the calibration curve depending on the system performance. You can respace different parts of the same tuning curve with different step size.

### <a name="Vid008"></a>Extend calibration range of interaction
<button class="btn" data-clipboard-text="{{site.fullUrl}}{{page.url}}#Vid008">
    Copy address to this how-to
</button>
<video  controls="controls">
<source src="https://lightconupdater.blob.core.windows.net/topas4infopage/Videos/HowToExtendInteractionCalibrationRange.mp4" type="video/mp4" />
</video>

Advanced user or service access level required.
1.	Go to 'Calibration' >> 'Create interaction'.
2.	Enter name of interaction you want to modify in field 'Full interaction'. There is no need to select motors.
3.	Enter new start wavelength  (end wavelength will be the same).
4. Calibrate new points as usually.
5. Once you reach already-calibrated wavelengths you can click 'Finish' button.


### <a name="Vid004"></a>Recalculate Idler wavelengths after pump wavelength modification
<button class="btn" data-clipboard-text="{{site.fullUrl}}{{page.url}}#Vid004">
    Copy address to this how-to
</button>
<video  controls="controls">
<source src="https://lightconupdater.blob.core.windows.net/topas4infopage/Videos/RecalculateIdler.mp4" type="video/mp4" />
</video>

Advanced user or service access level required.




### <a name="Vid005"></a>Rename named motor position
<button class="btn" data-clipboard-text="{{site.fullUrl}}{{page.url}}#Vid005">
    Copy address to this how-to
</button>
<video  controls="controls">
<source src="https://lightconupdater.blob.core.windows.net/topas4infopage/Videos/HowToRenameNamedMotorPosition.mp4" type="video/mp4" />
</video>

Advanced user or service access level required.
1.	Go to 'Motors'.
2.	Choose motor from the list on the left.
3.	Go to 'Named positions'.
4.	Double mouse click 'Name' (and 'Shortname'), change the name and press 'Apply'.


### <a name="Vid006"></a>Change motor value for named motor position
<button class="btn" data-clipboard-text="{{site.fullUrl}}{{page.url}}#Vid006">
    Copy address to this how-to
</button>
<video  controls="controls">
<source src="https://lightconupdater.blob.core.windows.net/topas4infopage/Videos/ChangeMotorValueForNamedPosition.mp4" type="video/mp4" />
</video>

Advanced user or service access level required.
1.	Go to 'Motors'.
2.	Choose motor from the list on the left.
3.	Go to 'Named positions'.
4.	Double mouse click 'Position (steps)', change the value and press 'Apply'.





### <a name="Vid007"></a>Add/modify neutral motor position
<button class="btn" data-clipboard-text="{{site.fullUrl}}{{page.url}}#Vid007">
    Copy address to this how-to
</button>
<video  controls="controls">
<source src="https://lightconupdater.blob.core.windows.net/topas4infopage/Videos/ModifyAddNeutralPosition.mp4" type="video/mp4" />
</video>

Advanced user or service access level required.


