# 5 Search

The "Search" mode is designed to analyze the operational ("raw") data of the device and search for a source of radiation or heterogeneity of radiation fields. The data is displayed in several graphical representations for two measurement channels – count rate and/or dose rate.

The operational data is raw gamma radiation data that is sent to the application from the device in real time every 500 ms. The application stores this data for the last 10 minutes. The values of the operational data vary widely and are characterized by a high random measurement error. With an increase in the level of recorded radiation, this error decreases.

The button, when held or pressed, allows you to select display options:

· The count rate in the form of an arrow indicator and a graph · Dose rate in the form of an arrow indicator and a graph\
· The count rate and dose rate in the form of arrow indicators

Graphs always display operational data in the form in which they come from the device, without any processing. The data displayed on the arrow indicator is averaged: the arithmetic mean is calculated over a time interval that can be specified in the settings.

Analog arrow indicator

The indicator is a fixed linear scale with divisions from 0 to 100 and an arrow. The scale is colored according to the alarm thresholds set in the dosimeter (see Device settings). To get readings corresponding to the position of the arrow, you need to multiply the value on the scale by the coefficient active in the list to the right of the indicator.

In the center of the arrow indicator is a numeric value that reflects the current value of the data. The units of measurement are located under the indicator. The name of the measured value is displayed in the upper left corner. There is a bright circle marker at the end of the arrow for greater contrast.

There are two dynamically changing zones along the circumference on the surface of the indicator scale. The blue statistics area displays the maximum and minimum range of values registered since the application was launched or since the statistics were reset.

The cyan zone on top of the blue one displays the oscillation range of the arrow, the boundaries of which dynamically indicate the activity zone and the direction of the arrow displacement.

Graph

The graph shows the operational data coming from the device. It is similar to the graphs on the "Charts" tab, with the following features:

* ·  Time scales – from 1 to 10 minutes.
