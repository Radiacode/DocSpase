# 10 Map and tracks

Application RadiaCode equipped with functions of displaying the emission situation on a map in real

time, as well as functions of recording routes (“tracks”) and their subsequent download for view.

To access the map, select the “Map” item in the main menu, which is called by tapping the icon top left. To record tracks, the app needs access to the location of the device. Also, the location function of the phone/tablet must be enabled.

Opens the settings related to the map.

|   |                                                                                                                                                                                                                                                                                                                                                                |
| - | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|   | Opens track library.                                                                                                                                                                                                                                                                                                                                           |
|   | Displays a point in the center of the map that corresponds to your current location. A long tap on this icon additionally sets some average map scale.                                                                                                                                                                                                         |
|   | Starts or continues recording a track.                                                                                                                                                                                                                                                                                                                         |
|   | <p>Indicates that marker colors are determined from dose rate values. When clicked, switches to the mode of marker coloring by count rate, and the icon on the button is replaced by this:<br><br>This icon indicates that marker colors are determined by count rate values, and clicking on it switches to the mode of marker coloring by dose rate.</p>     |
|   | <p>Opens a dropdown menu:<br>· Mark: Enter marker flagging mode. In this mode, tapping a marker flags it for later<br><br>deletion. The flagged markers are white and surrounded by a pink circle.<br>· Delete selected...: After confirmation, delete the flagged markers from the track. Markers<br><br>are permanently deleted and cannot be recovered.</p> |
|   | Automatically colors markers on the map in accordance with the minimum and maximum dose rate/count rate values. A long tap additionally automatically sets the minimum and maximum values of the displayed markers.                                                                                                                                            |
|   | Expands/hides the color bar graph.                                                                                                                                                                                                                                                                                                                             |

Tracks

When you record a track, each current location is marked with a circle on the map. The color of the circle corresponds to the emission level or count rate measured at this point, taking into account the color settings on the color scale.

The colors of the markers are determined by the dose rate values or, starting with application version 1.30.00, by the count rate values. The display mode is selected using the corresponding button on the toolbar. Tracks recorded with older versions of the software do not contain count rate information, so marker colors will appear the same in both modes. Tracks recorded by a device whose firmware did not yet support energy compensation essentially contain dose rate values that are directly proportional to the count rate.

To start recording a track, tap the icon at the top left of the screen. You will be prompted to enter a track title. After that, recording will start, and the name of the track will be displayed at the top of the screen under the buttons:

New points appear on the map, and, accordingly, are remembered in the track only when the location changes. In the application settings, you can set the minimum position accuracy. It should be borne in mind that the correctness of determining the location depends on many factors - the

quality of the phone's GPS module, the interference situation, etc. In the absence of information from the GPS sensor, the smartphone can determine the location using other sources - cell towers and Wi-Fi networks.

When first displayed on the map in the dose rate mode, the marker is colored according to the current value of the dose rate transmitted by the device, and surrounded by a thick gray line. The operational value of the dose rate transmitted by the device lags behind the current calendar moment in time. The lag time depends on the rate of change in the radiation situation: with small changes in dose rate values, the lag can be tens of seconds; with sharp changes, the lag is reduced. As data arrives from the device, operational markers corresponding to the calendar time of the received values ?are repainted in accordance with the accepted value and acquire the status of permanent ones, the thick stroke disappears. You can turn off the thick outline of operational markers in the map settings. Hot markers are not stored in the database.

Track recording continues until it is explicitly stopped and as long as the application is in communication with the device. When the device is reconnected, track recording resumes automatically.

It should be borne in mind that in the track recording mode, the smartphone consumes a lot of energy and its battery will drain faster. If you do not need to, do not set too small a value for the positioning accuracy in the application settings.

If you tap any circle (marker), information corresponding to this point will be displayed - date/time, measured emission level, count rate, and positioning accuracy:

Touching the information window opens a drop-down menu - with its help you can attach a picture to the point, remove the point from the track, or simply close the information window.

Color scale

The color scale is a quick way to color the track points so that they clearly reflect the changing emission situation. By moving the scale sliders, you can set the minimum dose rate or count rate value, which corresponds to the violet color, and the maximum value, which corresponds to the red one:

This example shows that the entire range of measured values is approximately 40...77 μR/h. The purple slider is set to 40.5 μR/h, so all points with the same and lower dose rate level will be purple. The red slider is set to 77.2 μR/h, and all points with the same or higher level will be red. All points between 40 and 77 μR/h will have intermediate colors, from violet to red. In the map settings, you can select a palette of colors to display markers.

In the map settings, you can turn on the function of automatic coloring of markers in accordance with the current maximum and maximum measured value.

Attaching images to track points

In addition to the entire track, it is possible to attach images to individual track points. Attached images are displayed with a camera symbol:

There are two ways to attach a picture to a point on a track:\
· Take a photo with the camera. The picture will be attached to the very last point of the track.

· Tap a point on the map. A drop-down menu will open, allowing you to attach a picture to the point. Tapping the camera icon opens a drop-down menu for image manipulation.\
See also:\
Map settings

Track library Pseudo tracks

10.1 Map settings\
To open the map settings, tap at the top left of the screen. Maps API:

It is possible to choose the software platform that provides the maps and their rendering. The default is Google Maps. As an alternative map API you can choose the OpenStreetMap platform (https://www.openstreetmap.org/). OpenStreetMap is an open source project with the ability for users to add their own objects to the map.

Google Maps provides an opportunity to choose between the type of map - scheme, satellite photo or hybrid version and works only in online mode, ie, when displayed sections of the map are downloaded by the application from the Google server.

OpenStreetMap displays the map only as a diagram. You can choose between the online mode, when the map is downloaded as raster images-tiles from the servers of OpenStreetMap partner companies, and the offline mode, when preloaded files with vector maps are used for display (see below for details). OpenStreetMap draws markers much faster than Google Maps, so for very large tracks it is more convenient to use it.

Google Maps and OpenStreetMap settings are slightly different. The different settings are listed at the end of the page.

Store location in the database:\
Never: The coordinates of your smartphone's current location are not recorded in the database

(log).

Only when recording a track: The coordinates of your smartphone's current location are only entered into the database during track recording. This allows you to partially recover a track from the base log as a pseudo track.

Always: If enabled, the location is entered into the database along with the rest of the information. In the future, you can open on the map pseudo track and see the change in the radiation situation associated with the selected location. You should not enable this option unnecessarily, because location determination makes the smartphone consume a lot of power.

Coordinates are stored in the database only if location detection in the smartphone is enabled by the user. Android apps do not have the ability to turn location detection on and off on their own.

Location:

Location resolution and distance between markers on the map: If the location of the smartphone changes by more than the specified number of meters from the previous one, then in track a new point is recorded. Do not set too low values, since at the same time, the GPS module of the smartphone will work more intensively, while the number of track points will increase rapidly and the rendering of the track on the map will be slower.

Ignore a location if its measurement accuracy is worse than: If the accuracy of the position measurement is worse (greater than) the specified value, the application will ignore the system message about the position change. For example, if you specify to ignore locations with a measurement accuracy worse than 20 meters, and the system reports that the location has changed, but the measurement accuracy is ± 22 meters, then this location change will be ignored.

Ignore location if the distance to the previous point is less than: If the distance between the previous point and the current point is less than the specified value, the application will ignore the system message about the location change. The combination of the last two options allows you to eliminate situations where the system reports small changes in geolocation coordinates measured with poor accuracy.

In a group “Markers” you can choose how the circle markers will be displayed on the map:

* Minimum and maximum dose rate valuefor the marker defines the range of values ?o?f the measured dose rate level displayed on the map. Points with a dose rate level outside the specified range are not displayed.
* Automatically shift the minimum and maximum values: if the marker added to the track has a dose rate value that exceeds the boundaries of the levels displayed on the map ("Minimum and maximum dose rate value for the marker"), then change the corresponding boundary so that the marker is visible. For example, if the maximum limit is set to 120 μR/h, and the dose rate of the next marker is 140 μR/h, the maximum displayed value will become 140 μR/h.
* Display markers where the dose rate value is out of bounds defined by color scale: If this option is disabled, then only those points with the dose rate level between the values ?defined by the sliders will be displayed on the map. Points with values ?below the purple slider (for example, less than 40.5 μR/h) and above red (77.2 μR/h) will not be displayed.
* Connect markers with a line: Draw a dashed line connecting the markers. This helps to display the intended trajectory of movement if the markers are far apart, but slows down rendering.
* Automatically set marker colors by min./max. dose rate values: Set (including during the track recording process) colors so that purple corresponds to the minimum dose rate in the track, and red - to the maximum value. The triangles on the color bar will be set to their respective positions. If you move one of the triangles, then this option is disabled. It should also be borne in mind that the automatic coloring of markers with a significant number of points slows down the application.
* Enable the auto-coloring option when loading a new track: If auto-coloring was disabled, for example, due to manual manipulations with the color scale, then auto-coloring will be automatically enabled when loading another track or starting recording a new one.
* Disable live data marker stroke: Do not stroke live markers (for which the dose rate value has not yet been transmitted by the device) with a thick gray line.
* Marker size: you can select the diameter of the circles.
* Markers stroke: Marker circles are outlined with a semi-transparent gray line, which allows you to visually perceive them as a set of circles, and not as a solid line if the markers partially overlap. At small map scales, the stroke masks the colors of the circles, so you can turn off the stroke or choose to turn it off automatically at small scales. The track is rendered slightly faster when the stroke is off.
* Decimation of markers: One can choose an additional criterion, taking into account which the markers are decimated when they are added to the map in order to speed up the rendering of large tracks. When adding a new marker, the application compares its parameters with the parameters of the previously added marker. The next marker is NOT added if the following conditions are simultaneously met: 1). The distance between this marker and the previous one is less than specified in the selected criterion (1/4 of the marker radius, 1/2 of the radius, or whole radius). 2). The difference in the dose rate of this marker and the previous one does not exceed 10% of the value of the dose rate of the previous marker.

Decimation of markers affects only their display on the map. This setting does not affect the process of recording a track; non-displayed markers are not deleted from the track.

* Marker palette: you can select the palette of colors that are used to draw the markers.
* Map Auto-Centering: If in the process of recording a track you move the map to the side (for example, to view some other part of the map), then after the specified time the map will display in the center the position corresponding to the current location.
* Ignore a point if the accuracy of determining its location is worse than: When calculating the track length, ignore the points for which the positioning accuracy is worse than the specified one. This makes the calculation of the track length more accurate.
* Track length calculation: When calculating the track length, do not take into account points for which the accuracy of location determination is worse than specified. This allows for more accurate calculation of the track length.
* Display location accuracy: Display in the upper left corner of the map information about the accuracy with which the last location was determined. This function works only if track recording is on. If the location was recorded in the track, then the color of the text in the window will be black, otherwise it will be red (the conditions for recording coordinates are not met).
* Display track length: Display track length information in the upper left corner of the map.
* Display movement speed: Show speed in the upper left corner of the map. This information is provided by the system, the application does not calculate speed and displays it as is. Speed information may be unreliable due to, for example, low accuracy of location determination.
* Show movement direction: Show direction of travel in the upper left corner of the map. This information is provided by the system. By default, direction is designated by one or two letters: N - north, SE - southeast, etc. If you select "Detailed direction (3 letters)" below, the direction will be encoded by one, two or three letters: N - north, SE - southeast, WNW - west-northwest, etc.
* Keep smartphone screen on when map is active: The smartphone screen will not turn off if a map is displayed on the screen.

Some of the settings related to location are found in the application settings,. You can import a track with the button . The system file picker opens.

Export settings (“Share”)

Application RadiaCode can export a track in several formats:

* ·  in its own rctrk format, which is a text format and can be imported back into an application on another smartphone.
