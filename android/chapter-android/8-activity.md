# 8 Activity

The “Activity” tab is designed to determine the absolute and specific activity of the Cs-137 isotope in various loose and watery materials (primarily in food) and the absolute activity of Cs-137 point sources. This isotope is one of the main pollutants after nuclear accidents and tests.

Measurement parameters

The upper part of the tab displays the parameters that shall be specified before starting the measurement:

|                |             |
| -------------- | ----------- |
| Parameter name | Description |

|             |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Geometry    | <p>The parameter is selected from the list and determines the geometry of the sample in which the activity of Cs-137 is evaluated.<br>If the sample dimensions are small (less than 5 mm), then the geometry should be selected “Point source 5 cm”. In this case, during the measurement, the sample is located at a distance of 5 cm from the “+” symbol on the back cover of the device and from the side of this symbol.<br><br>If the sample is large enough (does not fit the description of the point source above), then one of the containers in the list should be selected. Containers are not included in the device delivery set and should be purchased separately.</p> |
| Product     | Name of the sample material, selected from the list. The parameter if not entered if geometry is selected “Point source 5 cm”.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| Weight      | Numerical value of the sample weight in grams with an accuracy of 0.1 g. The parameter is omitted if "Point source 5cm" geometry is selected.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| Spectrum    | Displays the spectrum name of the sample taken from the spectrum library, or “Current”if a new spectrum is being accumulated during the measurement process.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| Backgroun d | Name of the background spectrum from the spectra library                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |

Measurement results

The results are displayed below the measurement parameters and grouped into: Activity/Specific, MDA/Specific and MPC.

|                                                                               |                                                                                                                                                                                                                                                                                                                                           |
| ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Result name                                                                   | Description                                                                                                                                                                                                                                                                                                                               |
| Activity Absolute activity of the sample minus the background, in becquerels. |                                                                                                                                                                                                                                                                                                                                           |
| Specific activity                                                             | Specific activity of the sample, based on the injected mass, in becquerels per kilogram. The parameter is not calculated if geometry is selected “Point source 5 cm”.                                                                                                                                                                     |
| %                                                                             | Estimation of the random error of the current values ?of absolute and specific activity. The error decreases with increasing the measurement time. At error values g?reater than 30%, the measured activity values ?are considered unreliable and are displayed in gray. If it is impossible to estimate the error, dashes are displayed. |
| MDA                                                                           | Estimate of the minimum detectable activity, in becquerels. Calculated from the background spectrum and the sample spectrum, taking into account their random errors.                                                                                                                                                                     |
| Specific MDA                                                                  | Estimate of the minimum detectable specific activity calculated based on the MDA and the sample mass, in becquerels per kilogram. The parameter is not calculated if geometry is selected “Point source 5 cm”.                                                                                                                            |
| MPC                                                                           | Exceeding the MPC level, in times. MPC is maximum permissible concentration, tabular values a?re taken for Russia. The parameter is not calculated if geometry is selected “Point source 5 cm”.                                                                                                                                           |

At the bottom of the “Activity” tab there is an area for displaying the histogram of the spectrum section, according to which the above estimates are calculated. In the center of the histogram, there is a region of the spectrum where the presence of a Cs-137 peak with an energy of 662 keV is assumed. The region with energies of 662 ±100 keV is displayed in brighter colors. The criterion for the availability of cesium in the sample is the bell-shaped peak on the spectrum, which stands out above the background level, with a maximum in the middle of the graph. If such peak is not visible, then the measured values ?may be unreliable.

Start/stop button (combined) serves to start/stop the measurement. When starting a measurement, you can either continue the current measurement (if any) or start a new one. During the measurement, the current data is saved once a minute, the measurement will automatically continue after reconnecting the device and after restarting the application.

“Diskette” button serves to save the obtained spectrum to the spectra library. “i” button serves to display extended information about the measurement. "Gear" button opens the activity measurement settings dialog:

Activity measuring units: Becquerel - defined as the activity of a source in which an average of one radioactive decay occurs per second. 1 \[Bc] = 1 decay/sec.\
Curie is an outdated measure of activity. It is defined as the activity of 1 gram of radium-226 together with daughter radionuclides. 1 \[Ci] = 37,000,000,000 Bq.

Use MPC standards for the country: select the country for which the MPC standards apply. When you select a country, the list of products available for measuring their activity also changes.

Offer to save the spectrum when stopping the activity measurement: If the activity measurement is performed in several steps, this option can be disabled so that the application does not offer to save the accumulated spectrum each time the measurement is stopped.

Measurement procedure

Use the following methods to assess the sample activity:

Measurement of sample activity in a container Point source activity measurement

8.1 Measurement of sample activity in a container Measurement procedure

IMPORTANT: To determine the activity of loose and watery materials, it is necessary to give them a standard shape by placing them in a special container (containers are not included in the device delivery set and are purchased separately). At the moment, the program calculates activity, when using multiple containers:

0.5 l Marinelli container 60 ml container 100 ml container

0.5 l Marinelli author 0.2 l Marinelli author\
You can download the files for 3D printing of the author's containers here.

To measure the mass of the container and sample a balance with an accuracy of at least 1 g will also be required.

1. Charge the device to at least 50% capacity and using the “Spectrum” mode generate a background spectrum set. When obtaining the spectrum, the device shall always be in the same place where the activity measurement will be carried out. To improve the measurement accuracy, it is recommended to obtain spectra for at least 8 hours, and if possible - a day or more. Save the acquired spectrum to the spectra library with the name “Background Date/Location” or similar.
2. Open the “Activity” tab of the application and in the dropdown list of the “Geometry:” line select the container used.
3. In the dropdown list of the “Product:” line select the product type.
4. In the “Weight:” line enter the weight (net) of the sample. For this:

* ·  measure the weight of the empty container with the lid;
