# Comparing `tmp/cbpi4-pt100x-0.1.8.tar.gz` & `tmp/cbpi4-pt100x-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbpi4-pt100x-0.1.8.tar", last modified: Wed Mar 29 04:57:17 2023, max compression
+gzip compressed data, was "cbpi4-pt100x-0.1.9.tar", last modified: Fri Jun  9 11:11:47 2023, max compression
```

## Comparing `cbpi4-pt100x-0.1.8.tar` & `cbpi4-pt100x-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-03-29 04:57:17.559811 cbpi4-pt100x-0.1.8/
--rw-rw-rw-   0        0        0    35149 2021-11-29 14:37:31.000000 cbpi4-pt100x-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     1084 2021-11-29 14:37:31.000000 cbpi4-pt100x-0.1.8/LICENSE-for-max31865
--rw-rw-rw-   0        0        0       72 2021-11-29 14:37:31.000000 cbpi4-pt100x-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     4061 2023-03-29 04:57:17.558807 cbpi4-pt100x-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     3695 2023-03-28 05:01:40.000000 cbpi4-pt100x-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-03-29 04:57:17.531809 cbpi4-pt100x-0.1.8/cbpi4-pt100x/
--rw-rw-rw-   0        0        0    11034 2023-03-28 05:01:23.000000 cbpi4-pt100x-0.1.8/cbpi4-pt100x/__init__.py
--rw-rw-rw-   0        0        0       29 2021-11-29 14:37:31.000000 cbpi4-pt100x-0.1.8/cbpi4-pt100x/config.yaml
--rw-rw-rw-   0        0        0     7730 2021-12-05 13:24:20.000000 cbpi4-pt100x-0.1.8/cbpi4-pt100x/max31865.py
-drwxrwxrwx   0        0        0        0 2023-03-29 04:57:17.555808 cbpi4-pt100x-0.1.8/cbpi4_pt100x.egg-info/
--rw-rw-rw-   0        0        0     4061 2023-03-29 04:57:16.000000 cbpi4-pt100x-0.1.8/cbpi4_pt100x.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-03-29 04:57:16.000000 cbpi4-pt100x-0.1.8/cbpi4_pt100x.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-29 04:57:16.000000 cbpi4-pt100x-0.1.8/cbpi4_pt100x.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-03-29 04:57:16.000000 cbpi4-pt100x-0.1.8/cbpi4_pt100x.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-29 04:57:17.560808 cbpi4-pt100x-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      868 2023-03-28 05:01:46.000000 cbpi4-pt100x-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:11:47.006441 cbpi4-pt100x-0.1.9/
+-rw-rw-rw-   0        0        0    35149 2021-11-29 14:37:31.000000 cbpi4-pt100x-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0     1084 2021-11-29 14:37:31.000000 cbpi4-pt100x-0.1.9/LICENSE-for-max31865
+-rw-rw-rw-   0        0        0       72 2021-11-29 14:37:31.000000 cbpi4-pt100x-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     5475 2023-06-09 11:11:47.004434 cbpi4-pt100x-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5109 2023-06-09 11:08:50.000000 cbpi4-pt100x-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 11:11:46.972436 cbpi4-pt100x-0.1.9/cbpi4-pt100x/
+-rw-rw-rw-   0        0        0    11032 2023-06-09 10:32:03.000000 cbpi4-pt100x-0.1.9/cbpi4-pt100x/__init__.py
+-rw-rw-rw-   0        0        0       29 2021-11-29 14:37:31.000000 cbpi4-pt100x-0.1.9/cbpi4-pt100x/config.yaml
+-rw-rw-rw-   0        0        0     7730 2021-12-05 13:24:20.000000 cbpi4-pt100x-0.1.9/cbpi4-pt100x/max31865.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:11:47.002458 cbpi4-pt100x-0.1.9/cbpi4_pt100x.egg-info/
+-rw-rw-rw-   0        0        0     5475 2023-06-09 11:11:46.000000 cbpi4-pt100x-0.1.9/cbpi4_pt100x.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2023-06-09 11:11:46.000000 cbpi4-pt100x-0.1.9/cbpi4_pt100x.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 11:11:46.000000 cbpi4-pt100x-0.1.9/cbpi4_pt100x.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-09 11:11:46.000000 cbpi4-pt100x-0.1.9/cbpi4_pt100x.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 11:11:47.006441 cbpi4-pt100x-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      868 2023-06-09 10:46:04.000000 cbpi4-pt100x-0.1.9/setup.py
```

### Comparing `cbpi4-pt100x-0.1.8/LICENSE` & `cbpi4-pt100x-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cbpi4-pt100x-0.1.8/LICENSE-for-max31865` & `cbpi4-pt100x-0.1.9/LICENSE-for-max31865`

 * *Files identical despite different names*

### Comparing `cbpi4-pt100x-0.1.8/PKG-INFO` & `cbpi4-pt100x-0.1.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbpi4-pt100x
-Version: 0.1.8
+Version: 0.1.9
 Summary: CraftBeerPi4 PT100/PT1000 Sensor Plugin
 Home-page: https://github.com/PiBrewing/cbpi4-pt100x
 Author: Alexander Vollkopf
 Author-email: avollkopf@web.de
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -17,33 +17,55 @@
 
 You can select the conversion mode and number of wires on your probe in software.  You will need to select a setting to get the probe working after an update.
 
 You will need to set the reference resistors on the craftbeerpi hardware page!  My max31865 chip uses a 4,3 kohm resistor for the PT1000. It might be 430 ohm for a PT100 board
 
 Using a max31865 board like: https://learn.adafruit.com/adafruit-max31865-rtd-pt100-amplifier/
 
-### Software installation:
+## Software installation:
 
 - sudo pip3 install cbpi4-pt100x
 - or install from repo: sudo pip3 install https://github.com/PiBrewing/cbpi4-pt100x/archive/main.zip
 
 
-### Hardware Installation:
+## Hardware Installation:
 
 - on your pi use the following GPIO pins:
 - csPin = 8  *this one can be any GPIO you want, if using multiple probes you change this on each one, but keep the other 3 pins the same*
 - misoPin = 9
 - mosiPin = 10
 - clkPin = 11
 
+The code for the request to the max chip is from https://github.com/steve71/MAX31865 so all credit really goes there... i slightly modified the code from the craftbeerpi v3 plugin(https://github.com/thegreathoe/cbpi-pt100-sensor) to allow also the usage of tha PT1000 and added some other parameters.
 
+## Sensor Configuration
 
-The code for the request to the max chip is from https://github.com/steve71/MAX31865 so all credit really goes there... i slightly modified the code from the craftbeerpi v3 plugin(https://github.com/thegreathoe/cbpi-pt100-sensor) to allow also the usage of tha PT1000 and added some other parameters.
+The sensor must be configured on the hardware page. The following parameters must be set and will affect your readings:
+
+- csPin: The BCM number of the GPIO you max board cs pin is connected to.
+- ResSens: Reistance in ohm of your sensor. Select 1000 for PT1000 or 100 for PT100.
+- RefRest: Resistance in ohm of your reference resistor on your max board. Typically 4300 for a PT100 board and 430 for a PT100 board. The value is typically listed on the resistor of your board (Please have a look [here](https://www.hobby-hour.com/electronics/smdcalc.php?fbclid=IwAR1frc48ImXjxPMLqCeVPX2SZEEDDhXrLxRsUWpZ_e1XeJnrN20qRXZOEo4) for smd resistance codings.)
+- offset: Defines a temperature offset for your temp probe.
+- ignore_above: Ignores Temp readings above this value (0: deactivated)
+- ignore_below: Ignores Temp readings below this value (0: deactivated)
+- ignore_delta: If you experience issues with 'jumping' temp readings, you can define a threshold (only positive values are allowed) for the difference between two readings. If the difference between two subsequent readings is higher than the threshold, the value will be ignored. If the next reading is also higher (lower), this value is used / logged. (0: deactivated)
+- alpha: calculates the average between 2 subsequent values. Must be between 0 and 1. (1: deactivated). 0.5 yields for instance in the average of two subsequent readings.
+- ConfigText: You need to set this parameter to the configuration of your maxboard / sensor.
+- Interval: defines the frequency of sensor readings in seconds.
+- Kettle/Fermenter: You can select a Kettle OR Fermenter if you want to activate reduced sensor logging during inactivity of the Kettle / Fermenter
+- Reducedlogging: Defines the logging interval for reduced logging in seconds (e.g. 300 would result in logging every 5 Minutes when the Kettle / Fermenter logic is not acitve) (0: no sensor logging during inactivity)
+
+
+Please note that the max board delivers readings above 900C if no sensor is connected to the board.
+
+![Sensor Configuration](https://github.com/PiBrewing/cbpi4-pt100x/blob/main/Hardware_Configuration.png?raw=true)
 
 ### Changelog:
+
+- 09.06.23: (0.1.9) Updated descriptions for Sensor parameters on Hardware page. Updated README.
 - 28.03.23: (0.1.8) No logging options in case of Kettle or Fermenter inactivity (set reducedlogging to 0)
 - 25.03.23: (0.1.4) Reduced logging options in case of Kettle or Fermenter inactivity
 - 10.05.22: (0.1.3) updated readme (removed cbpi add)
 - 10.05.22: (0.1.2) Removed cbpi dependency
 - 08.12.21: (0.1.1) Removed resampling as it caused issues with respect to long term stability (sensor unresponsivness)
 - 01.12.21: (0.1.0) Improved handling of resampling in case of issues (test)	
 - 01.11.21: (0.0.11) Experimental update under development branch: Read another sample if delta between two values is too high
@@ -53,16 +75,9 @@
 - 09.04.21: (0.0.7) Fix in offset handling in case value is not None but empty
 - 15.03.21: (0.0.6) Change to supprt cbpi >= 4.0.0.31
 - 20.02.21: (0.0.4) Change to support cbpi >= 4.0.0.24. Added sensor log fucntionality
 - 14.02.21: (0.0.3) Updated function to retrieve temperature unit. Units will be changed automatically for sensor when settigs saved properly. No need to update the sensor 
 - 09.02.21: (0.0.2) Added offset parameter and changed the GPIO.setmode. Currnetly, warnings are displayed during startup of CBPi. However, they cause typically no issues
 - 05.02.21: (0.0.1) Adpated code to run under cbpi4
 
-### Old versions:
-
-- CBPi3
-- 7/20/20:: Added PT1000 functionality. This can be selected in the setup of the sensor. Added also parameters such as offset, low and high vaule filter that are comparable to the OneWireSensor plugins. PT1000 (2-wire) is for instance used in the Speidel Braumeister 20 / 50 and can be read out directly with this plugin. There is no need to change the sensor or the thermowell for these devices.
-- 8/2/17:: Pascal has been working on a pretty nice update which allows you to select the number of wires used on your probe in software... you still need to sever traces or solder jumpers on the board!  He has also been added as a contributer
-- 7/2/17:: Verified with Pascal Fouchy that it is working on multiple sensors at once, and i have added the ability to change the reference resistor value from the craftbeerpi hardware page
-
```

### Comparing `cbpi4-pt100x-0.1.8/README.md` & `cbpi4-pt100x-0.1.9/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -4,33 +4,55 @@
 
 You can select the conversion mode and number of wires on your probe in software.  You will need to select a setting to get the probe working after an update.
 
 You will need to set the reference resistors on the craftbeerpi hardware page!  My max31865 chip uses a 4,3 kohm resistor for the PT1000. It might be 430 ohm for a PT100 board
 
 Using a max31865 board like: https://learn.adafruit.com/adafruit-max31865-rtd-pt100-amplifier/
 
-### Software installation:
+## Software installation:
 
 - sudo pip3 install cbpi4-pt100x
 - or install from repo: sudo pip3 install https://github.com/PiBrewing/cbpi4-pt100x/archive/main.zip
 
 
-### Hardware Installation:
+## Hardware Installation:
 
 - on your pi use the following GPIO pins:
 - csPin = 8  *this one can be any GPIO you want, if using multiple probes you change this on each one, but keep the other 3 pins the same*
 - misoPin = 9
 - mosiPin = 10
 - clkPin = 11
 
+The code for the request to the max chip is from https://github.com/steve71/MAX31865 so all credit really goes there... i slightly modified the code from the craftbeerpi v3 plugin(https://github.com/thegreathoe/cbpi-pt100-sensor) to allow also the usage of tha PT1000 and added some other parameters.
 
+## Sensor Configuration
 
-The code for the request to the max chip is from https://github.com/steve71/MAX31865 so all credit really goes there... i slightly modified the code from the craftbeerpi v3 plugin(https://github.com/thegreathoe/cbpi-pt100-sensor) to allow also the usage of tha PT1000 and added some other parameters.
+The sensor must be configured on the hardware page. The following parameters must be set and will affect your readings:
+
+- csPin: The BCM number of the GPIO you max board cs pin is connected to.
+- ResSens: Reistance in ohm of your sensor. Select 1000 for PT1000 or 100 for PT100.
+- RefRest: Resistance in ohm of your reference resistor on your max board. Typically 4300 for a PT100 board and 430 for a PT100 board. The value is typically listed on the resistor of your board (Please have a look [here](https://www.hobby-hour.com/electronics/smdcalc.php?fbclid=IwAR1frc48ImXjxPMLqCeVPX2SZEEDDhXrLxRsUWpZ_e1XeJnrN20qRXZOEo4) for smd resistance codings.)
+- offset: Defines a temperature offset for your temp probe.
+- ignore_above: Ignores Temp readings above this value (0: deactivated)
+- ignore_below: Ignores Temp readings below this value (0: deactivated)
+- ignore_delta: If you experience issues with 'jumping' temp readings, you can define a threshold (only positive values are allowed) for the difference between two readings. If the difference between two subsequent readings is higher than the threshold, the value will be ignored. If the next reading is also higher (lower), this value is used / logged. (0: deactivated)
+- alpha: calculates the average between 2 subsequent values. Must be between 0 and 1. (1: deactivated). 0.5 yields for instance in the average of two subsequent readings.
+- ConfigText: You need to set this parameter to the configuration of your maxboard / sensor.
+- Interval: defines the frequency of sensor readings in seconds.
+- Kettle/Fermenter: You can select a Kettle OR Fermenter if you want to activate reduced sensor logging during inactivity of the Kettle / Fermenter
+- Reducedlogging: Defines the logging interval for reduced logging in seconds (e.g. 300 would result in logging every 5 Minutes when the Kettle / Fermenter logic is not acitve) (0: no sensor logging during inactivity)
+
+
+Please note that the max board delivers readings above 900C if no sensor is connected to the board.
+
+![Sensor Configuration](https://github.com/PiBrewing/cbpi4-pt100x/blob/main/Hardware_Configuration.png?raw=true)
 
 ### Changelog:
+
+- 09.06.23: (0.1.9) Updated descriptions for Sensor parameters on Hardware page. Updated README.
 - 28.03.23: (0.1.8) No logging options in case of Kettle or Fermenter inactivity (set reducedlogging to 0)
 - 25.03.23: (0.1.4) Reduced logging options in case of Kettle or Fermenter inactivity
 - 10.05.22: (0.1.3) updated readme (removed cbpi add)
 - 10.05.22: (0.1.2) Removed cbpi dependency
 - 08.12.21: (0.1.1) Removed resampling as it caused issues with respect to long term stability (sensor unresponsivness)
 - 01.12.21: (0.1.0) Improved handling of resampling in case of issues (test)	
 - 01.11.21: (0.0.11) Experimental update under development branch: Read another sample if delta between two values is too high
@@ -40,14 +62,7 @@
 - 09.04.21: (0.0.7) Fix in offset handling in case value is not None but empty
 - 15.03.21: (0.0.6) Change to supprt cbpi >= 4.0.0.31
 - 20.02.21: (0.0.4) Change to support cbpi >= 4.0.0.24. Added sensor log fucntionality
 - 14.02.21: (0.0.3) Updated function to retrieve temperature unit. Units will be changed automatically for sensor when settigs saved properly. No need to update the sensor 
 - 09.02.21: (0.0.2) Added offset parameter and changed the GPIO.setmode. Currnetly, warnings are displayed during startup of CBPi. However, they cause typically no issues
 - 05.02.21: (0.0.1) Adpated code to run under cbpi4
 
-### Old versions:
-
-- CBPi3
-- 7/20/20:: Added PT1000 functionality. This can be selected in the setup of the sensor. Added also parameters such as offset, low and high vaule filter that are comparable to the OneWireSensor plugins. PT1000 (2-wire) is for instance used in the Speidel Braumeister 20 / 50 and can be read out directly with this plugin. There is no need to change the sensor or the thermowell for these devices.
-- 8/2/17:: Pascal has been working on a pretty nice update which allows you to select the number of wires used on your probe in software... you still need to sever traces or solder jumpers on the board!  He has also been added as a contributer
-- 7/2/17:: Verified with Pascal Fouchy that it is working on multiple sensors at once, and i have added the ability to change the reference resistor value from the craftbeerpi hardware page
-
```

### Comparing `cbpi4-pt100x-0.1.8/cbpi4-pt100x/__init__.py` & `cbpi4-pt100x-0.1.9/cbpi4-pt100x/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 from cbpi.api.dataclasses import NotificationAction, NotificationType
 
 logger = logging.getLogger(__name__)
 
 
 @parameters([Property.Select(label="csPin", options=[0, 1, 2, 3, 4, 5, 6, 7, 8, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27], description="GPIO Pin connected to the CS Pin of the MAX31865 - For MISO, MOSI, CLK no choice by default it's PIN 9, 10, 11"),
     Property.Select(label="ResSens", options = [100,1000],description = "Select 100 for PT100 or 1000 for PT1000"),
-    Property.Number(label="RefRest", configurable = True, default_value = 4300, description = "Reference Resistor of the MAX31865 board (it's written on the resistor: 430 or 4300,....)"),
+    Property.Number(label="RefRest", configurable = True, default_value = 4300, description = "Reference Resistor of the MAX31865 board (430 (PT100) or 4300 ohm (PT1000) depending on your board)"),
     Property.Number(label="offset",configurable = True, default_value = 0, description="Offset for the PT Sensor (Default is 0)"),
     Property.Number(label="ignore_below",configurable = True, default_value = 0, description="Readings below this value will be ignored"),
     Property.Number(label="ignore_above",configurable = True,default_value = 100, description="Readings above this value will be ignored"),
-    Property.Number(label="ignore_delta",configurable = True,default_value = 1, description="Ignore reading if delta between two readings is above this value. Must be positive and 0 deaxctivates filter"),
+    Property.Number(label="ignore_delta",configurable = True,default_value = 1, description="Ignore reading if delta between two readings is above this value. Must be positive (0: inactive)"),
     Property.Number(label="alpha",configurable = True,default_value = 1, description="Calculate Average between 2 values. Must be between 0 and 1. 1 deactivates averaging"),
     Property.Select(label="ConfigText", options=["[0xB2] - 3 Wires Manual","[0xD2] - 3 Wires Auto","[0xA2] - 2 or 4 Wires Manual","[0xC2] - 2 or 4 Wires Auto"], description="Choose beetween 2, 3 or 4 wire PT100 & the Conversion mode at 60 Hz beetween Manual or Continuous Auto"),
     Property.Select(label="Interval", options=[1,5,10,30,60], description="Interval in Seconds"),
     Property.Kettle(label="Kettle", description="Reduced logging if Kettle is inactive (only Kettle or Fermenter to be selected)"),
     Property.Fermenter(label="Fermenter", description="Reduced logging in seconds if Fermenter is inactive (only Kettle or Fermenter to be selected)"),
     Property.Number(label="ReducedLogging", configurable=True, description="Reduced logging frequency in seconds if selected Kettle or Fermenter is inactive (default: 60 sec | disabled: 0)")])
```

### Comparing `cbpi4-pt100x-0.1.8/cbpi4-pt100x/max31865.py` & `cbpi4-pt100x-0.1.9/cbpi4-pt100x/max31865.py`

 * *Files identical despite different names*

### Comparing `cbpi4-pt100x-0.1.8/cbpi4_pt100x.egg-info/PKG-INFO` & `cbpi4-pt100x-0.1.9/cbpi4_pt100x.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbpi4-pt100x
-Version: 0.1.8
+Version: 0.1.9
 Summary: CraftBeerPi4 PT100/PT1000 Sensor Plugin
 Home-page: https://github.com/PiBrewing/cbpi4-pt100x
 Author: Alexander Vollkopf
 Author-email: avollkopf@web.de
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -17,33 +17,55 @@
 
 You can select the conversion mode and number of wires on your probe in software.  You will need to select a setting to get the probe working after an update.
 
 You will need to set the reference resistors on the craftbeerpi hardware page!  My max31865 chip uses a 4,3 kohm resistor for the PT1000. It might be 430 ohm for a PT100 board
 
 Using a max31865 board like: https://learn.adafruit.com/adafruit-max31865-rtd-pt100-amplifier/
 
-### Software installation:
+## Software installation:
 
 - sudo pip3 install cbpi4-pt100x
 - or install from repo: sudo pip3 install https://github.com/PiBrewing/cbpi4-pt100x/archive/main.zip
 
 
-### Hardware Installation:
+## Hardware Installation:
 
 - on your pi use the following GPIO pins:
 - csPin = 8  *this one can be any GPIO you want, if using multiple probes you change this on each one, but keep the other 3 pins the same*
 - misoPin = 9
 - mosiPin = 10
 - clkPin = 11
 
+The code for the request to the max chip is from https://github.com/steve71/MAX31865 so all credit really goes there... i slightly modified the code from the craftbeerpi v3 plugin(https://github.com/thegreathoe/cbpi-pt100-sensor) to allow also the usage of tha PT1000 and added some other parameters.
 
+## Sensor Configuration
 
-The code for the request to the max chip is from https://github.com/steve71/MAX31865 so all credit really goes there... i slightly modified the code from the craftbeerpi v3 plugin(https://github.com/thegreathoe/cbpi-pt100-sensor) to allow also the usage of tha PT1000 and added some other parameters.
+The sensor must be configured on the hardware page. The following parameters must be set and will affect your readings:
+
+- csPin: The BCM number of the GPIO you max board cs pin is connected to.
+- ResSens: Reistance in ohm of your sensor. Select 1000 for PT1000 or 100 for PT100.
+- RefRest: Resistance in ohm of your reference resistor on your max board. Typically 4300 for a PT100 board and 430 for a PT100 board. The value is typically listed on the resistor of your board (Please have a look [here](https://www.hobby-hour.com/electronics/smdcalc.php?fbclid=IwAR1frc48ImXjxPMLqCeVPX2SZEEDDhXrLxRsUWpZ_e1XeJnrN20qRXZOEo4) for smd resistance codings.)
+- offset: Defines a temperature offset for your temp probe.
+- ignore_above: Ignores Temp readings above this value (0: deactivated)
+- ignore_below: Ignores Temp readings below this value (0: deactivated)
+- ignore_delta: If you experience issues with 'jumping' temp readings, you can define a threshold (only positive values are allowed) for the difference between two readings. If the difference between two subsequent readings is higher than the threshold, the value will be ignored. If the next reading is also higher (lower), this value is used / logged. (0: deactivated)
+- alpha: calculates the average between 2 subsequent values. Must be between 0 and 1. (1: deactivated). 0.5 yields for instance in the average of two subsequent readings.
+- ConfigText: You need to set this parameter to the configuration of your maxboard / sensor.
+- Interval: defines the frequency of sensor readings in seconds.
+- Kettle/Fermenter: You can select a Kettle OR Fermenter if you want to activate reduced sensor logging during inactivity of the Kettle / Fermenter
+- Reducedlogging: Defines the logging interval for reduced logging in seconds (e.g. 300 would result in logging every 5 Minutes when the Kettle / Fermenter logic is not acitve) (0: no sensor logging during inactivity)
+
+
+Please note that the max board delivers readings above 900C if no sensor is connected to the board.
+
+![Sensor Configuration](https://github.com/PiBrewing/cbpi4-pt100x/blob/main/Hardware_Configuration.png?raw=true)
 
 ### Changelog:
+
+- 09.06.23: (0.1.9) Updated descriptions for Sensor parameters on Hardware page. Updated README.
 - 28.03.23: (0.1.8) No logging options in case of Kettle or Fermenter inactivity (set reducedlogging to 0)
 - 25.03.23: (0.1.4) Reduced logging options in case of Kettle or Fermenter inactivity
 - 10.05.22: (0.1.3) updated readme (removed cbpi add)
 - 10.05.22: (0.1.2) Removed cbpi dependency
 - 08.12.21: (0.1.1) Removed resampling as it caused issues with respect to long term stability (sensor unresponsivness)
 - 01.12.21: (0.1.0) Improved handling of resampling in case of issues (test)	
 - 01.11.21: (0.0.11) Experimental update under development branch: Read another sample if delta between two values is too high
@@ -53,16 +75,9 @@
 - 09.04.21: (0.0.7) Fix in offset handling in case value is not None but empty
 - 15.03.21: (0.0.6) Change to supprt cbpi >= 4.0.0.31
 - 20.02.21: (0.0.4) Change to support cbpi >= 4.0.0.24. Added sensor log fucntionality
 - 14.02.21: (0.0.3) Updated function to retrieve temperature unit. Units will be changed automatically for sensor when settigs saved properly. No need to update the sensor 
 - 09.02.21: (0.0.2) Added offset parameter and changed the GPIO.setmode. Currnetly, warnings are displayed during startup of CBPi. However, they cause typically no issues
 - 05.02.21: (0.0.1) Adpated code to run under cbpi4
 
-### Old versions:
-
-- CBPi3
-- 7/20/20:: Added PT1000 functionality. This can be selected in the setup of the sensor. Added also parameters such as offset, low and high vaule filter that are comparable to the OneWireSensor plugins. PT1000 (2-wire) is for instance used in the Speidel Braumeister 20 / 50 and can be read out directly with this plugin. There is no need to change the sensor or the thermowell for these devices.
-- 8/2/17:: Pascal has been working on a pretty nice update which allows you to select the number of wires used on your probe in software... you still need to sever traces or solder jumpers on the board!  He has also been added as a contributer
-- 7/2/17:: Verified with Pascal Fouchy that it is working on multiple sensors at once, and i have added the ability to change the reference resistor value from the craftbeerpi hardware page
-
```

### Comparing `cbpi4-pt100x-0.1.8/setup.py` & `cbpi4-pt100x-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='cbpi4-pt100x',
-      version='0.1.8',
+      version='0.1.9',
       description='CraftBeerPi4 PT100/PT1000 Sensor Plugin',
       author='Alexander Vollkopf',
       author_email='avollkopf@web.de',
       url='https://github.com/PiBrewing/cbpi4-pt100x',
       include_package_data=True,
       package_data={
         # If any package contains *.txt or *.rst files, include them:
```

