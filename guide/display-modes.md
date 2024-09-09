---
icon: tv-retro
---

# Display Modes

The Radiacode-10X series dosimeter has a single mode of operation - continuous data collection, accumulation and analysis.

|                                                     |                                                                                                                                                                                                                                                                                                                                                                        |                                         |
| --------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------- |
| !\[\[RC101\_is\_off\_f.png]]                        | <p>- Press and hold the round button until the instrument turns on (at least 3 seconds);<br><br>- When turned on, the instrument will be in the Monitor and display the dose rate;<br>- With the appropriate settings, the sound power on will be played at this time.<br>- At appropriate settings at this moment the backlight of the display will be turned on.</p> | !\[\[estimation\_sound\_on\_f.png]]     |
| ![](../.gitbook/assets/estimation\_unlocked\_f.png) | <p>Press and hold the round button to move to the menu;<br><br>- The name of the current menu item will be displayed at the top. (In this case it is "Monitor" [[Display Modes]]);<br>- The icons of the main menu items will be placed vertically;<br>- The active item will be highlighted with a negative icon</p>                                                  | !\[\[menu\_monitor\_selected\_f 1.png]] |

At any moment one of several ways of displaying the radiation situation assessment is available:

!\[\[dose\_rate\_sym.png]] \[\[#Monitor]] – estimation of dose rate and count rate; !\[\[dose\_sym.png]] \[\[#Dose]] – dose assessment; !\[\[lookup\_sym.png]] \[\[#Search]]– operational search; !\[\[spectrum\_sym.png]] \[\[#Spectrum]] –  energy spectrum of photon radiation.

During operation, the instrument also detects the exceeding of all Alarms levels. Informs the user of radiation hazards or changes in the environment.

#### Monitor

This mode is intended to represent dose rate or count rate. When the instrument is turned on, it starts working in this particular display mode. All incoming data are accumulated and analyzed. If a change in the radiation situation is detected, the instrument starts a new interval of data accumulation. If there are no signs of changes in the radiation situation, the averaging continues in order to increase the reliability of the estimation. Statistical error in the Monitor mode is maintained at the level not more than 15% for the confidence interval 2δ at sufficient radiation intensity.

In the **Monitor** display mode, the screen shows:

* status panel - from the top;
* parameters of dose rate or count rate estimation - at the bottom. !\[\[presentation\_dose\_rate\_all\_signs\_f 1.png]] The upper part of the screen, from left to right, contains basic information about the status of the instrument:

!\[\[status\_monitor\_all\_signs 1.png|250]]

* current time: hours, minutes;
* detector temperature;
* sign of exceeding the thresholds for dose rate, dose rate, count rate;
* audio indication status;
* presence of Bluetooth or USB connection;
* swing button lock sign;
* battery status.

At the bottom of the screen from left to right:

* graphical representation of the dose rate or count rate estimate;
* value of the dose rate or count rate estimate;
* value of random error in %;
* dose rate measurement units - Sv/h, R/h, or count rate - CPS, CPM.

With the help of the menu the choice between the measurement units is available:

* Sv/h or R/h - when displaying dose rate;
* CPS or CPM - when displaying the count rate.

The type of radiation intensity estimation: Dose rate or count rate can be selected in the menu, or can be switched operatively with the instrument buttons.

> \[!todo] Quick control in this mode is available via the buttons:
>
> * a short press on the top button of the swing to switch between the types of photon radiation intensity display:&#x20;
> * dose rate or count rate;
> * long pressing on the upper button of the swing turns on and off the sound indication;
> * short pressing on the lower button of the swing switches on the sound indication of registered quanta (clicks).

#### Dose

The mode is intended for presentation of accumulated dose.

In the Dose display mode the screen shows:

* status panel - from the top;
* parameters of accumulated dose estimation.

!\[\[presentation\_dose\_f.png]] The upper part of the screen, from left to right, contains basic information about the status of the instrument:

!\[\[status\_dose\_all\_signs 1.png|250]]

* time since the beginning of dose accumulation: days, hours, minutes;
* detector temperature;
* sign of exceeding the thresholds for dose rate, dose rate, count rate;
* audio indication status;
* presence of Bluetooth or USB connection;
* swing button lock sign;
* battery status.

At the bottom of the screen from left to right:

* graphical representation of the cumulative dose estimate.
* cumulative dose assessment value;
* dose measurement units - Sv, R;

Using the menu you can choose between the measurement units:

* Sv or P - when displaying dose rate.

> \[!todo] Quick control in this mode is available via the buttons:
>
> * long pressing the lower button resets the value of the accumulated dose;
> * long pressing on the upper button of the swing turns on and off the sound indication.

**Setting alarm thresholds**

#### Search

The mode is designed to represent the count rate in the form of a search graph. It is applicable for operative search of the source or zone with increased radiation level.

In the Search display mode the screen shows:

* status bar - on top;
* search graph of count rate - at the bottom.

!\[\[presentation\_scan\_f 1.png]]

The upper part of the screen, from left to right, contains basic information about the status of the instrument:

!\[\[status\_scan\_all\_signs 1.png|250]]

* averaging time, price of one bar on the chart in seconds - 1/2, 1, 2, 4 seconds;
* current count rate value;
* count rate units - CPS or CPM;
* sign of exceeding thresholds on dose rate, dose rate, count rate level;
* audio indication status;
* Bluetooth or USB connection;
* swing buttons lock sign;
* battery status.

At the bottom of the screen from left to right:

* graphical representation of the current count rate.
* search graph of the count rate;

> \[!todo] Quick control in this mode is available via buttons:
>
> * a short press on the upper swing button increases the averaging time;
> * a short press on the lower swing button decreases the averaging time;
> * long press on the lower swing button clears the screen and starts a new search session;
> * long pressing the upper swing button turns the sound indication on and off.

#### Spectrum

The mode is intended for representation of the general view of the photon (gamma and X-ray) radiation energy spectrum.

In the **Spectrum** display mode the screen shows: state panel - from top; energy spectrum of photon (gamma and X-ray) radiation.

The upper part of the screen, from left to right, contains basic information about the instrument status:

!\[\[status\_spectrum 1.png|250]]

* scale of the amplitude scale of the photon radiation energy spectrum - linear or logarithmic;
* time since the beginning of spectrum accumulation: hours, minutes, seconds;
* sign of exceeding thresholds by dose rate, dose rate, count rate;
* audio indication status;
* Bluetooth or USB connection;
* swing buttons lock sign;
* \[battery]\(Before use) status.

At the bottom of the screen from left to right: !\[\[presentation\_spectrum\_log\_1MeV\_scale\_Cs137\_f 1.png]]

* graphical representation of dose rate estimation.
* histogram of the photon radiation energy spectrum;

Labels are placed under the energy scale of the histogram:

* dots - every 100keV;
* dashes every 500keV;
* arrows - every 1000keV.

> \[!todo] Quick control of the spectrum view is available via the buttons:
>
> * a short press on the upper swing button switches the spectrum amplitude scale between linear and logarithmic;
> * a short press on the lower button of the swing cycles the scale of the energy scale 1MeV -> 2MeV -> 3MeV -> 1MeV.... ;
> * long press on the lower button of the swing clears the screen and starts a new session of spectrum accumulation;
> * long pressing the upper button of the swing turns on and off the sound indication.

Each horizontal bar shows a graphical representation of a value (dose rate, dose, count rate) on a logarithmic scale.

The ranges of the bars differ by a factor of 10. For example, for dose rate (µSv/h) the ranges will look as follows:

!\[\[indicator\_levels\_sym.png]]
