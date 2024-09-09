---
icon: bell-exclamation
---

# Alarms

**The sources of alarms** in the Radiacode-10X series device are: current value of count rate value; current value of dose rate value; value of accumulated dose;

The **Alarm Status** is indicated by:

* red LED flashes;
* alarm icons on the status panel of the device display;
* unacknowledged alarms status line.

| ![](../.gitbook/assets/cr\_alarm\_1.png)         | Level 1 alarm on Count Rate. |
| ------------------------------------------------ | ---------------------------- |
| ![](../.gitbook/assets/cr\_alarm\_2.png)         | Level 2 alarm on Count Rate. |
| ![](../.gitbook/assets/cr\_alarm\_3.png)         | Count Rate over-range alarm. |
| ![](../.gitbook/assets/md\_alarm\_1.png)         | Level 1 Dose Rate alarm.     |
| ![](../.gitbook/assets/md\_alarm\_2.png)         | Level 2 Dose Rate alarm.     |
| ![](../.gitbook/assets/md\_alarm\_3.png)         | Dose Rate over-range alarm.  |
| ![](<../.gitbook/assets/dose\_alarm\_1 (1).png>) | Level 1 alarm on Dose.       |
| ![](../.gitbook/assets/dose\_alarm\_2.png)       | Level 2 alarm on Dose.       |
| ![](../.gitbook/assets/dose\_alarm\_3.png)       | Alarm 3 on Dose over scale   |

**Setting alarm thresholds**

Two  alarm thresholds for the dose rate level can be set using the menu. When the dose rate alarm threshold level is exceeded, a pulsating sign will be displayed in the status bar:

* "Alarm 1" – ![](<../.gitbook/assets/md\_alarm\_1 (2).png>);
* "Alarm 2" – ![](../.gitbook/assets/md\_alarm\_2.png);
* "Alarm 3 (off the scale)" – ![](../.gitbook/assets/md\_alarm\_3.png) .

Two alarm thresholds for the count rate alarm level can be set using the menu. When the count rate alarm threshold level is exceeded, a pulsating sign will be displayed in the status bar:

* "Alarm 1" – ![](<../.gitbook/assets/cr\_alarm\_1 (3).png>);
* "Alarm 2" – ![](../.gitbook/assets/cr\_alarm\_2.png) ;
* "Alarm 3 (off the scale)" – ![](../.gitbook/assets/cr\_alarm\_3.png) .

Two alarm thresholds for the accumulated dose level can be set using the menu. When the alarm threshold level is exceeded, a pulsating sign will be displayed in the status bar:

* "Alarm 1" – ![](<../.gitbook/assets/dose\_alarm\_1 (2).png>);
* "Alarm 2" – ![](../.gitbook/assets/dose\_alarm\_2.png);
* "Alarm 3 (off the scale)" – ![](../.gitbook/assets/dose\_alarm\_3.png).

There are three alarm thresholds for each of these sources in the Radiacode-10X series instrument: If the current count rate, dose rate, or dose value crosses any of the thresholds from bottom to top, an **Alarm event** occurs:

* first threshold - Alarm 1;
* second threshold - Alarm 2;
* upper limit of the scale - over scale;

The values of alarm thresholds of the first and second level, separately for each of the sources, are set in the device settings. They can be changed at your discretion. The value of the third threshold is the upper limit of the scale of each of the measured values. These thresholds cannot be changed through the menu. The instrument constantly checks the current values of count rate, dose rate, accumulated dose and compares them with the threshold values.

Exceeding any of the thresholds puts the instrument into the **Alarm state**.&#x20;

Each **Alarm Source** defines one of 4 states:

* Normal - value below the first threshold (no alarm);
* Alarm 1 - value higher than the first threshold but not higher than the second;
* Alarm 2 - value higher than the second threshold, but not higher than the third;
* Over scale - value above the third threshold, going beyond the scale.

Exceeding the upper threshold by count rate leads to unreliability of dose rate estimation. In this case the upper threshold for dose rate is also considered to be exceeded.

If any of the alarm thresholds for dose rate, count rate or accumulated dose is exceeded, the corresponding alarm will be activated. To stop the alarm for any level, you need to confirm by briefly pressing the round button that you have accepted the alarm. The instrument will continue to display exceeding the set level with a flashing icon of the appropriate type. To terminate an alarm based on the accumulated dose level, you must reset it to zero, or change the corresponding alarm threshold.

Each **Alarm Event** has corresponding Alarms associated with it:

* audible alarm;
* vibration signal;

Audio and vibration Alarms can be enabled/disabled in the Radiacode-10X series settings for each level of any of the **alarm sources** independently.

On an **Alarm Event**, Radiacode-10X series will play the Alarms allowed in the settings.

You can stop playing the alarm by briefly pressing the _round button_.

The next **Alarm Event** will be signaled again.

Light signals can be turned on/off in the settings Radiacode-10X series

If the device has been locked, if the alarm indication settings (sound and/or vibro) are enabled, a line of maximum recorded levels of unconfirmed alarms will be shown on the device display after the thresholds have been exceeded: !\[\[alarm\_screen.png]]

The following rules are adopted for indication of states and events of alarms on the display:

* If the swing buttons are locked, the status panel displays the message "Alarms:" and icons of maximum alarm levels reached from the moment the buttons are locked to the current moment of time - one icon for each source.&#x20;
* By long pressing the round button, the user can confirm viewing of the presented list of maximum alarm levels, after which the swing buttons will be unlocked and the normal instrument status panel will be displayed.
* If Alarm Events occurred while displaying the menu, upon exiting the menu, the display will show the list of maximum alarm levels mentioned above. The swing buttons will then be locked.
* If the swing buttons are unlocked and the display shows one of the measurement display modes, the status bar will show the current alarm level icons for each of the sources, alternating between them.
