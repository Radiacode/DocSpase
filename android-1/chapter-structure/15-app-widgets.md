# 15 App widgets

If you don't know what a widget is and how to put it on your smartphone's desktop, look on the

Internet for help.

Application RadiaCode app provides several widgets:

Indicators widget

This widget can only be resized horizontally. The right side with the battery, temperature and Bluetooth signal strength is only displayed if there is enough space for it. The red square in the lower left corner means that the track is being recorded.

The indicator widget is updated approximately every two seconds.

Device screen widget

This is a screenshot of the device screen, which is updated every two seconds. When an alarm occurs, the widget can be updated more frequently. You cannot change the size of the device screen widget.

Spectrum widget

This widget displays the spectrum graph in the form that corresponds to the settings of the "Spectrum" tab in the app itself. The spectrum widget is updated at the interval specified for automatic spectrum updates in the application, but, unlike the application, the spectrum widget is always updated automatically. The size of the spectrum widget can be changed without restriction.

Remarks

Touching the widget launches the app RadiaCode.

When you exit the RadiaCode app normally, it notifies the open widgets that the device is disconnected from the smartphone, and the widgets display a corresponding inscription. If you exit abnormally, for example, when "swiping" an application in the screen of running smartphone applications, the RadiaCode app may not receive any notifications from the system. In this case, widgets will display the latest information received from the application, although the application is no longer in smartphone memory.

The RadiaCode widgets are updated quite often, which, by default, is not provided by the system. So far, no negative effects of frequent widget updates have been detected.

Spectrum, spectrogram and track libraries

16 Spectrum, spectrogram and track libraries\
The spectra, spectrograms and tracks storages are called libraries and are stored in the application

database. We will call a spectrum, spectrogram and track by the word "object".

To open a library, tap the symbol on the control bar (toolbar) of the "Spectrum", "View" or "Spectrogram" tab. The track library is opened by the icon on the map toolbar.

A list of saved objects is displayed. For each object, its name, which was specified when saving, the recording start date, the serial number of the device and other information corresponding to the type of object are displayed. For tracks that were created by a device with firmware that does not support energy compensation, a yellow icon is displayed in the lower right corner. For 8-bit spectra created by a device with firmware version less than 4.00, an orange marker with the number 8 is displayed in the lower right corner. For each saved spectrum, its graph in the logarithmic scale, name and accumulation time are displayed.

It is possible to create folders for more convenient organization of the library. You can manage folders through the options menu, which is accessed by tapping the three-dot icon in the top right corner of the screen. The options menu also contains:

· Search: An input line appears where you can enter part of the object name. Only object names containing the entered substring will remain on the screen. The search is performed within the displayed folder, i.e. this function essentially works as a filter. To find a object located in a folder, you need to switch the display to "Simple list without folders" mode through the same options menu before searching.

· Import object: The system file selector opens. For more information, see "Export and Import". Tapping a line opens a dropdown menu:

· Open object: Load an object for viewing (the track opens on the map). If the object is a spectrogram and is currently being recorded, it continues in the background. To return to the

Spectrum, spectrogram and track libraries 82

graph of the spectrogram being recorded, tap the button on the "Spectrogram" tab and select

"Close spectrogram".

* ·  Share object: Export the object data and "share" this file, i.e. save it in smartphone memory,
