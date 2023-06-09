# Comparing `tmp/hcsr04sensor-1.6.3.tar.gz` & `tmp/hcsr04sensor-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hcsr04sensor-1.6.3.tar", last modified: Sat Feb 19 01:02:25 2022, max compression
+gzip compressed data, was "hcsr04sensor-1.7.tar", last modified: Fri Jun  9 16:23:21 2023, max compression
```

## Comparing `hcsr04sensor-1.6.3.tar` & `hcsr04sensor-1.7.tar`

### file list

```diff
@@ -1,16 +1,21 @@
-drwxrwxr-x   0 al        (1000) al        (1000)        0 2022-02-19 01:02:25.000000 hcsr04sensor-1.6.3/
--rw-rw-r--   0 al        (1000) al        (1000)     5205 2022-02-19 00:59:38.000000 hcsr04sensor-1.6.3/README.md
--rw-rw-r--   0 al        (1000) al        (1000)     1039 2022-02-19 00:18:47.000000 hcsr04sensor-1.6.3/setup.py
--rw-rw-r--   0 al        (1000) al        (1000)     6980 2022-02-19 01:02:25.000000 hcsr04sensor-1.6.3/PKG-INFO
--rw-rw-r--   0 al        (1000) al        (1000)       18 2021-12-30 12:55:24.000000 hcsr04sensor-1.6.3/MANIFEST.in
--rw-rw-r--   0 al        (1000) al        (1000)       38 2022-02-19 01:02:25.000000 hcsr04sensor-1.6.3/setup.cfg
-drwxrwxr-x   0 al        (1000) al        (1000)        0 2022-02-19 01:02:25.000000 hcsr04sensor-1.6.3/hcsr04sensor.egg-info/
--rw-rw-r--   0 al        (1000) al        (1000)        1 2022-02-19 01:02:25.000000 hcsr04sensor-1.6.3/hcsr04sensor.egg-info/dependency_links.txt
--rw-rw-r--   0 al        (1000) al        (1000)     6980 2022-02-19 01:02:25.000000 hcsr04sensor-1.6.3/hcsr04sensor.egg-info/PKG-INFO
--rw-rw-r--   0 al        (1000) al        (1000)       13 2022-02-19 01:02:25.000000 hcsr04sensor-1.6.3/hcsr04sensor.egg-info/top_level.txt
--rw-rw-r--   0 al        (1000) al        (1000)      236 2022-02-19 01:02:25.000000 hcsr04sensor-1.6.3/hcsr04sensor.egg-info/SOURCES.txt
-drwxrwxr-x   0 al        (1000) al        (1000)        0 2022-02-19 01:02:25.000000 hcsr04sensor-1.6.3/hcsr04sensor/
--rw-rw-r--   0 al        (1000) al        (1000)        0 2021-12-30 12:55:24.000000 hcsr04sensor-1.6.3/hcsr04sensor/__init__.py
--rw-rw-r--   0 al        (1000) al        (1000)     8573 2021-12-30 12:55:24.000000 hcsr04sensor-1.6.3/hcsr04sensor/sensor.py
-drwxrwxr-x   0 al        (1000) al        (1000)        0 2022-02-19 01:02:25.000000 hcsr04sensor-1.6.3/bin/
--rwxrwxr-x   0 al        (1000) al        (1000)     2166 2021-12-30 12:55:24.000000 hcsr04sensor-1.6.3/bin/hcsr04.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-09 16:23:21.729392 hcsr04sensor-1.7/
+-rw-r--r--   0 al        (1000) users      (984)     1075 2023-02-19 17:00:08.000000 hcsr04sensor-1.7/LICENSE
+-rw-r--r--   0 al        (1000) users      (984)       18 2023-02-19 16:54:57.000000 hcsr04sensor-1.7/MANIFEST.in
+-rw-r--r--   0 al        (1000) users      (984)     5777 2023-06-09 16:23:21.729392 hcsr04sensor-1.7/PKG-INFO
+-rw-r--r--   0 al        (1000) users      (984)     4991 2023-06-09 16:22:18.000000 hcsr04sensor-1.7/README.md
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-09 16:23:21.726058 hcsr04sensor-1.7/bin/
+-rwxr-xr-x   0 al        (1000) users      (984)     2111 2023-06-09 16:22:18.000000 hcsr04sensor-1.7/bin/hcsr04.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-09 16:23:21.726058 hcsr04sensor-1.7/hcsr04sensor/
+-rw-r--r--   0 al        (1000) users      (984)        0 2023-02-19 16:54:57.000000 hcsr04sensor-1.7/hcsr04sensor/__init__.py
+-rw-r--r--   0 al        (1000) users      (984)     8562 2023-06-09 16:22:18.000000 hcsr04sensor-1.7/hcsr04sensor/sensor.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-09 16:23:21.729392 hcsr04sensor-1.7/hcsr04sensor.egg-info/
+-rw-r--r--   0 al        (1000) users      (984)     5777 2023-06-09 16:23:21.000000 hcsr04sensor-1.7/hcsr04sensor.egg-info/PKG-INFO
+-rw-r--r--   0 al        (1000) users      (984)      309 2023-06-09 16:23:21.000000 hcsr04sensor-1.7/hcsr04sensor.egg-info/SOURCES.txt
+-rw-r--r--   0 al        (1000) users      (984)        1 2023-06-09 16:23:21.000000 hcsr04sensor-1.7/hcsr04sensor.egg-info/dependency_links.txt
+-rw-r--r--   0 al        (1000) users      (984)       13 2023-06-09 16:23:21.000000 hcsr04sensor-1.7/hcsr04sensor.egg-info/top_level.txt
+-rw-r--r--   0 al        (1000) users      (984)       38 2023-06-09 16:23:21.729392 hcsr04sensor-1.7/setup.cfg
+-rw-r--r--   0 al        (1000) users      (984)      988 2023-06-09 16:22:18.000000 hcsr04sensor-1.7/setup.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-09 16:23:21.729392 hcsr04sensor-1.7/tests/
+-rw-r--r--   0 al        (1000) users      (984)     8692 2023-06-04 12:10:24.000000 hcsr04sensor-1.7/tests/test_sensor.py
+-rw-r--r--   0 al        (1000) users      (984)     1740 2023-06-09 16:22:18.000000 hcsr04sensor-1.7/tests/tests_hcsr04.py
+-rw-r--r--   0 al        (1000) users      (984)     9935 2023-06-09 16:22:18.000000 hcsr04sensor-1.7/tests/tests_sensor.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `hcsr04sensor-1.6.3/README.md` & `hcsr04sensor-1.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -80,16 +80,19 @@
 This module is not suitable for long distances.
 
 
 ## Usage
 
 See example scripts in https://github.com/alaudet/hcsr04sensor/tree/master/recipes
 
-Access to Raspberry Pi GPIO pins require elevated priviledges if using version 0.5.11 of RPi.GPIO.  Run example
-scripts with sudo.
+Access to Raspberry Pi GPIO pins requires the user account to be in the Linux gpio group.
+
+To add your user account name to the gpio group;
+
+    sudo usermod -aG gpio username
 
 ## Testing the Module
 
 Added a script that is installed to /usr/local/bin called hcsr04.py.
 This utility does not presently support BOARD pin values.  Use BCM pin values.
 
 usage: hcsr04.py [-h] -t TRIG -e ECHO [-sp SPEED] [-ss SAMPLES]
@@ -99,19 +102,13 @@
 If you don't want to use a sample of readings for error handling, warnings or pin cleanups I have included a static method in the Measurement class that will return a basic metric reading.  It returns the exact one-time reading that is provided  by the sensor and RPi.GPIO.  This allows you to handle all of these things to your own preference in your code.
 
 See the example basic_reading.py script in https://github.com/alaudet/hcsr04sensor/tree/master/recipes
 
 
 ## Contributing
 
-Contributions to hcsr04sensor are welcome.  Please open an issue in the issue
-tracker prior to a pull request.
-
-New features and bug fixes should be applied against the devel branch and not master. Contributions against the master branch will be rejected.
-
-Nose is currently used for testing.  All tests should pass before issuing
-the pull request.
+Read the contributing guidelines if you are interested in collaborating on this project.
 
 
 ## Donate
 
-[Your Donation is Appreciated](https://www.linuxnorth.org/donate/)
+[Your Donation is Appreciated](https://www.linuxnorth.org/donate/)
```

### Comparing `hcsr04sensor-1.6.3/setup.py` & `hcsr04sensor-1.7/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from setuptools import setup
 
-version = "1.6.3"
+version = "1.7"
 
 setup(
     name="hcsr04sensor",
     version=version,
     description="Module to access the HCSR04 sensor on a Raspberry Pi",
-    long_description_content_type='text/markdown',
+    long_description_content_type="text/markdown",
     long_description=open("./README.md", "r").read(),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: End Users/Desktop",
         "Natural Language :: English",
         "Operating System :: POSIX :: Linux",
-        "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.9",
         "Topic :: Home Automation",
         "License :: OSI Approved :: MIT License",
     ],
     author="Al Audet",
     author_email="alaudet@linuxnorth.org",
```

### Comparing `hcsr04sensor-1.6.3/PKG-INFO` & `hcsr04sensor-1.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,138 +1,135 @@
 Metadata-Version: 2.1
 Name: hcsr04sensor
-Version: 1.6.3
+Version: 1.7
 Summary: Module to access the HCSR04 sensor on a Raspberry Pi
 Home-page: https://www.linuxnorth.org/hcsr04sensor/
+Download-URL: https://github.com/alaudet/hcsr04sensor/releases
 Author: Al Audet
 Author-email: alaudet@linuxnorth.org
 License: MIT License
-Download-URL: https://github.com/alaudet/hcsr04sensor/releases
-Description: # HC-SR04 Ultrasonic Sensor on Raspberry Pi
-        
-        [Hcsr04sensor Web Page](https://www.linuxnorth.org/hcsr04sensor)
-        
-        Calculate distance and depth measurements with an HCSR04 Ultrasonic Sound Sensor and a Raspberry Pi. Instructions assume that you are using Raspbian Linux.
-        
-        This module also works with the JSN-SR04T waterproof sound sensor.
-        
-        ![wiring](https://www.linuxnorth.org/raspi-sump/images/raspi-sump-wiring.jpg)
-        
-        ## Python3 Install
-        
-        Install dependencies;
-        
-            sudo apt install python3-pip python3-rpi.gpio
-        
-        The above installs RPi.GPIO 0.7.0.  If using Raspberry Pi OS (Bullseye) you may prefer to install RPi.GPIO 0.7.1 with Pip. Either one should work.
-        
-         To get the latest install it with Pip as follows;
-        
-            sudo apt remove python3-rpi.gpio  <--0.7.0
-            sudo pip3 install RPi.GPIO <--0.7.1
-        
-        Install the hcsr04sensor module
-        
-            sudo pip3 install hcsr04sensor
-        
-        ## Description
-        
-        The module does the following;
-        
-        * Returns an error corrected distance by using the median reading of a sorted
-          sample. NOTE - The default sample size is 11 readings.
-        
-          You can specify a
-          different sample size by passing sample_size=x  to raw_distance (where x is your desired
-          number of readings).  This is useful if you need to lower the sample size to take
-          quicker readings.  Beware that the probability of getting erroneous readings
-          increases as sample size is reduced.  For my purposes a sample of 11 readings gives a consistent
-          value that I can trust and takes approximately 3 seconds to run with a 0.1
-          second wait time between individual samples.
-        
-          It is also possible to speed up the readings by passing a lower value to
-          sample_wait in raw_distance.
-        
-          The lower the value the quicker the invidual
-          samples will be taken.  A default of 0.1 is a safe wait time but this can be
-          reduced further.  CPU usage increases as faster readings are taken as well as
-          the chance for errors.
-        
-          This module uses BCM pin values.  See the Raspberry Pi pin layout documentation for your model.
-        
-        * Uses BCM pin values by default.  BOARD pin values are supported.
-        
-        * Adjusts the reading based on temperature by adjusting the speed of sound.
-        
-        * Allows measuring distance and depth in metric and imperial units.  See;
-        
-            pydoc hcsr04sensor.sensor
-        
-        * Raises an exception if a faulty cable or sensor prevents an echo pulse from being received.
-        
-        * Calculate the volume of different types of containers.  See recipes for examples.
-        
-        ## Accuracy of Readings
-        
-        If you need highly accurate readings then this module would not be suitable for your project.  In that case you should probably use an Arduino instead of a Raspberry Pi.
-        
-        Linux is not a Real Time OS so you can expect to get a small variance on each reading, usually within a half cm of the actual value.  I say "usually" because every once in a while you can get a reading that is way out of range.  This is due to the OS executing other tasks before getting your distance reading.  It is why I use a sample of readings.  I can always trust that the median of my sample of 11 readings is good.
-        
-        Highly accurate readings are not required for some applications. For example I use this module in an application I wrote for a sump pump monitor.  I am not worried about millimeter accuracy for that application.  1 cm variance on a meter deep pit is close enough to alert me to problems.
-        
-        Another example would be to calculate the water volume of a drinking water well (standing cylinder shape).
-        It would not matter if you are a gallon off on a 1000 gallon reading.
-        
-        
-        ## Distance Limitations
-        
-        The HCSR04 sensor is suited for short distance readings.  The specification manual says it is suitable up to 13 feet.  I have tested it to go further than that, but anything over 12 feet starts having periodic strange readings.
-        This module is not suitable for long distances.
-        
-        
-        ## Usage
-        
-        See example scripts in https://github.com/alaudet/hcsr04sensor/tree/master/recipes
-        
-        Access to Raspberry Pi GPIO pins require elevated priviledges if using version 0.5.11 of RPi.GPIO.  Run example
-        scripts with sudo.
-        
-        ## Testing the Module
-        
-        Added a script that is installed to /usr/local/bin called hcsr04.py.
-        This utility does not presently support BOARD pin values.  Use BCM pin values.
-        
-        usage: hcsr04.py [-h] -t TRIG -e ECHO [-sp SPEED] [-ss SAMPLES]
-        
-        ## Take a Basic Reading
-        
-        If you don't want to use a sample of readings for error handling, warnings or pin cleanups I have included a static method in the Measurement class that will return a basic metric reading.  It returns the exact one-time reading that is provided  by the sensor and RPi.GPIO.  This allows you to handle all of these things to your own preference in your code.
-        
-        See the example basic_reading.py script in https://github.com/alaudet/hcsr04sensor/tree/master/recipes
-        
-        
-        ## Contributing
-        
-        Contributions to hcsr04sensor are welcome.  Please open an issue in the issue
-        tracker prior to a pull request.
-        
-        New features and bug fixes should be applied against the devel branch and not master. Contributions against the master branch will be rejected.
-        
-        Nose is currently used for testing.  All tests should pass before issuing
-        the pull request.
-        
-        
-        ## Donate
-        
-        [Your Donation is Appreciated](https://www.linuxnorth.org/donate/)
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Home Automation
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# HC-SR04 Ultrasonic Sensor on Raspberry Pi
+
+[Hcsr04sensor Web Page](https://www.linuxnorth.org/hcsr04sensor)
+
+Calculate distance and depth measurements with an HCSR04 Ultrasonic Sound Sensor and a Raspberry Pi. Instructions assume that you are using Raspbian Linux.
+
+This module also works with the JSN-SR04T waterproof sound sensor.
+
+![wiring](https://www.linuxnorth.org/raspi-sump/images/raspi-sump-wiring.jpg)
+
+## Python3 Install
+
+Install dependencies;
+
+    sudo apt install python3-pip python3-rpi.gpio
+
+The above installs RPi.GPIO 0.7.0.  If using Raspberry Pi OS (Bullseye) you may prefer to install RPi.GPIO 0.7.1 with Pip. Either one should work.
+
+ To get the latest install it with Pip as follows;
+
+    sudo apt remove python3-rpi.gpio  <--0.7.0
+    sudo pip3 install RPi.GPIO <--0.7.1
+
+Install the hcsr04sensor module
+
+    sudo pip3 install hcsr04sensor
+
+## Description
+
+The module does the following;
+
+* Returns an error corrected distance by using the median reading of a sorted
+  sample. NOTE - The default sample size is 11 readings.
+
+  You can specify a
+  different sample size by passing sample_size=x  to raw_distance (where x is your desired
+  number of readings).  This is useful if you need to lower the sample size to take
+  quicker readings.  Beware that the probability of getting erroneous readings
+  increases as sample size is reduced.  For my purposes a sample of 11 readings gives a consistent
+  value that I can trust and takes approximately 3 seconds to run with a 0.1
+  second wait time between individual samples.
+
+  It is also possible to speed up the readings by passing a lower value to
+  sample_wait in raw_distance.
+
+  The lower the value the quicker the invidual
+  samples will be taken.  A default of 0.1 is a safe wait time but this can be
+  reduced further.  CPU usage increases as faster readings are taken as well as
+  the chance for errors.
+
+  This module uses BCM pin values.  See the Raspberry Pi pin layout documentation for your model.
+
+* Uses BCM pin values by default.  BOARD pin values are supported.
+
+* Adjusts the reading based on temperature by adjusting the speed of sound.
+
+* Allows measuring distance and depth in metric and imperial units.  See;
+
+    pydoc hcsr04sensor.sensor
+
+* Raises an exception if a faulty cable or sensor prevents an echo pulse from being received.
+
+* Calculate the volume of different types of containers.  See recipes for examples.
+
+## Accuracy of Readings
+
+If you need highly accurate readings then this module would not be suitable for your project.  In that case you should probably use an Arduino instead of a Raspberry Pi.
+
+Linux is not a Real Time OS so you can expect to get a small variance on each reading, usually within a half cm of the actual value.  I say "usually" because every once in a while you can get a reading that is way out of range.  This is due to the OS executing other tasks before getting your distance reading.  It is why I use a sample of readings.  I can always trust that the median of my sample of 11 readings is good.
+
+Highly accurate readings are not required for some applications. For example I use this module in an application I wrote for a sump pump monitor.  I am not worried about millimeter accuracy for that application.  1 cm variance on a meter deep pit is close enough to alert me to problems.
+
+Another example would be to calculate the water volume of a drinking water well (standing cylinder shape).
+It would not matter if you are a gallon off on a 1000 gallon reading.
+
+
+## Distance Limitations
+
+The HCSR04 sensor is suited for short distance readings.  The specification manual says it is suitable up to 13 feet.  I have tested it to go further than that, but anything over 12 feet starts having periodic strange readings.
+This module is not suitable for long distances.
+
+
+## Usage
+
+See example scripts in https://github.com/alaudet/hcsr04sensor/tree/master/recipes
+
+Access to Raspberry Pi GPIO pins requires the user account to be in the Linux gpio group.
+
+To add your user account name to the gpio group;
+
+    sudo usermod -aG gpio username
+
+## Testing the Module
+
+Added a script that is installed to /usr/local/bin called hcsr04.py.
+This utility does not presently support BOARD pin values.  Use BCM pin values.
+
+usage: hcsr04.py [-h] -t TRIG -e ECHO [-sp SPEED] [-ss SAMPLES]
+
+## Take a Basic Reading
+
+If you don't want to use a sample of readings for error handling, warnings or pin cleanups I have included a static method in the Measurement class that will return a basic metric reading.  It returns the exact one-time reading that is provided  by the sensor and RPi.GPIO.  This allows you to handle all of these things to your own preference in your code.
+
+See the example basic_reading.py script in https://github.com/alaudet/hcsr04sensor/tree/master/recipes
+
+
+## Contributing
+
+Read the contributing guidelines if you are interested in collaborating on this project.
+
+
+## Donate
+
+[Your Donation is Appreciated](https://www.linuxnorth.org/donate/)
```

### Comparing `hcsr04sensor-1.6.3/hcsr04sensor.egg-info/PKG-INFO` & `hcsr04sensor-1.7/hcsr04sensor.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,138 +1,135 @@
 Metadata-Version: 2.1
 Name: hcsr04sensor
-Version: 1.6.3
+Version: 1.7
 Summary: Module to access the HCSR04 sensor on a Raspberry Pi
 Home-page: https://www.linuxnorth.org/hcsr04sensor/
+Download-URL: https://github.com/alaudet/hcsr04sensor/releases
 Author: Al Audet
 Author-email: alaudet@linuxnorth.org
 License: MIT License
-Download-URL: https://github.com/alaudet/hcsr04sensor/releases
-Description: # HC-SR04 Ultrasonic Sensor on Raspberry Pi
-        
-        [Hcsr04sensor Web Page](https://www.linuxnorth.org/hcsr04sensor)
-        
-        Calculate distance and depth measurements with an HCSR04 Ultrasonic Sound Sensor and a Raspberry Pi. Instructions assume that you are using Raspbian Linux.
-        
-        This module also works with the JSN-SR04T waterproof sound sensor.
-        
-        ![wiring](https://www.linuxnorth.org/raspi-sump/images/raspi-sump-wiring.jpg)
-        
-        ## Python3 Install
-        
-        Install dependencies;
-        
-            sudo apt install python3-pip python3-rpi.gpio
-        
-        The above installs RPi.GPIO 0.7.0.  If using Raspberry Pi OS (Bullseye) you may prefer to install RPi.GPIO 0.7.1 with Pip. Either one should work.
-        
-         To get the latest install it with Pip as follows;
-        
-            sudo apt remove python3-rpi.gpio  <--0.7.0
-            sudo pip3 install RPi.GPIO <--0.7.1
-        
-        Install the hcsr04sensor module
-        
-            sudo pip3 install hcsr04sensor
-        
-        ## Description
-        
-        The module does the following;
-        
-        * Returns an error corrected distance by using the median reading of a sorted
-          sample. NOTE - The default sample size is 11 readings.
-        
-          You can specify a
-          different sample size by passing sample_size=x  to raw_distance (where x is your desired
-          number of readings).  This is useful if you need to lower the sample size to take
-          quicker readings.  Beware that the probability of getting erroneous readings
-          increases as sample size is reduced.  For my purposes a sample of 11 readings gives a consistent
-          value that I can trust and takes approximately 3 seconds to run with a 0.1
-          second wait time between individual samples.
-        
-          It is also possible to speed up the readings by passing a lower value to
-          sample_wait in raw_distance.
-        
-          The lower the value the quicker the invidual
-          samples will be taken.  A default of 0.1 is a safe wait time but this can be
-          reduced further.  CPU usage increases as faster readings are taken as well as
-          the chance for errors.
-        
-          This module uses BCM pin values.  See the Raspberry Pi pin layout documentation for your model.
-        
-        * Uses BCM pin values by default.  BOARD pin values are supported.
-        
-        * Adjusts the reading based on temperature by adjusting the speed of sound.
-        
-        * Allows measuring distance and depth in metric and imperial units.  See;
-        
-            pydoc hcsr04sensor.sensor
-        
-        * Raises an exception if a faulty cable or sensor prevents an echo pulse from being received.
-        
-        * Calculate the volume of different types of containers.  See recipes for examples.
-        
-        ## Accuracy of Readings
-        
-        If you need highly accurate readings then this module would not be suitable for your project.  In that case you should probably use an Arduino instead of a Raspberry Pi.
-        
-        Linux is not a Real Time OS so you can expect to get a small variance on each reading, usually within a half cm of the actual value.  I say "usually" because every once in a while you can get a reading that is way out of range.  This is due to the OS executing other tasks before getting your distance reading.  It is why I use a sample of readings.  I can always trust that the median of my sample of 11 readings is good.
-        
-        Highly accurate readings are not required for some applications. For example I use this module in an application I wrote for a sump pump monitor.  I am not worried about millimeter accuracy for that application.  1 cm variance on a meter deep pit is close enough to alert me to problems.
-        
-        Another example would be to calculate the water volume of a drinking water well (standing cylinder shape).
-        It would not matter if you are a gallon off on a 1000 gallon reading.
-        
-        
-        ## Distance Limitations
-        
-        The HCSR04 sensor is suited for short distance readings.  The specification manual says it is suitable up to 13 feet.  I have tested it to go further than that, but anything over 12 feet starts having periodic strange readings.
-        This module is not suitable for long distances.
-        
-        
-        ## Usage
-        
-        See example scripts in https://github.com/alaudet/hcsr04sensor/tree/master/recipes
-        
-        Access to Raspberry Pi GPIO pins require elevated priviledges if using version 0.5.11 of RPi.GPIO.  Run example
-        scripts with sudo.
-        
-        ## Testing the Module
-        
-        Added a script that is installed to /usr/local/bin called hcsr04.py.
-        This utility does not presently support BOARD pin values.  Use BCM pin values.
-        
-        usage: hcsr04.py [-h] -t TRIG -e ECHO [-sp SPEED] [-ss SAMPLES]
-        
-        ## Take a Basic Reading
-        
-        If you don't want to use a sample of readings for error handling, warnings or pin cleanups I have included a static method in the Measurement class that will return a basic metric reading.  It returns the exact one-time reading that is provided  by the sensor and RPi.GPIO.  This allows you to handle all of these things to your own preference in your code.
-        
-        See the example basic_reading.py script in https://github.com/alaudet/hcsr04sensor/tree/master/recipes
-        
-        
-        ## Contributing
-        
-        Contributions to hcsr04sensor are welcome.  Please open an issue in the issue
-        tracker prior to a pull request.
-        
-        New features and bug fixes should be applied against the devel branch and not master. Contributions against the master branch will be rejected.
-        
-        Nose is currently used for testing.  All tests should pass before issuing
-        the pull request.
-        
-        
-        ## Donate
-        
-        [Your Donation is Appreciated](https://www.linuxnorth.org/donate/)
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Home Automation
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# HC-SR04 Ultrasonic Sensor on Raspberry Pi
+
+[Hcsr04sensor Web Page](https://www.linuxnorth.org/hcsr04sensor)
+
+Calculate distance and depth measurements with an HCSR04 Ultrasonic Sound Sensor and a Raspberry Pi. Instructions assume that you are using Raspbian Linux.
+
+This module also works with the JSN-SR04T waterproof sound sensor.
+
+![wiring](https://www.linuxnorth.org/raspi-sump/images/raspi-sump-wiring.jpg)
+
+## Python3 Install
+
+Install dependencies;
+
+    sudo apt install python3-pip python3-rpi.gpio
+
+The above installs RPi.GPIO 0.7.0.  If using Raspberry Pi OS (Bullseye) you may prefer to install RPi.GPIO 0.7.1 with Pip. Either one should work.
+
+ To get the latest install it with Pip as follows;
+
+    sudo apt remove python3-rpi.gpio  <--0.7.0
+    sudo pip3 install RPi.GPIO <--0.7.1
+
+Install the hcsr04sensor module
+
+    sudo pip3 install hcsr04sensor
+
+## Description
+
+The module does the following;
+
+* Returns an error corrected distance by using the median reading of a sorted
+  sample. NOTE - The default sample size is 11 readings.
+
+  You can specify a
+  different sample size by passing sample_size=x  to raw_distance (where x is your desired
+  number of readings).  This is useful if you need to lower the sample size to take
+  quicker readings.  Beware that the probability of getting erroneous readings
+  increases as sample size is reduced.  For my purposes a sample of 11 readings gives a consistent
+  value that I can trust and takes approximately 3 seconds to run with a 0.1
+  second wait time between individual samples.
+
+  It is also possible to speed up the readings by passing a lower value to
+  sample_wait in raw_distance.
+
+  The lower the value the quicker the invidual
+  samples will be taken.  A default of 0.1 is a safe wait time but this can be
+  reduced further.  CPU usage increases as faster readings are taken as well as
+  the chance for errors.
+
+  This module uses BCM pin values.  See the Raspberry Pi pin layout documentation for your model.
+
+* Uses BCM pin values by default.  BOARD pin values are supported.
+
+* Adjusts the reading based on temperature by adjusting the speed of sound.
+
+* Allows measuring distance and depth in metric and imperial units.  See;
+
+    pydoc hcsr04sensor.sensor
+
+* Raises an exception if a faulty cable or sensor prevents an echo pulse from being received.
+
+* Calculate the volume of different types of containers.  See recipes for examples.
+
+## Accuracy of Readings
+
+If you need highly accurate readings then this module would not be suitable for your project.  In that case you should probably use an Arduino instead of a Raspberry Pi.
+
+Linux is not a Real Time OS so you can expect to get a small variance on each reading, usually within a half cm of the actual value.  I say "usually" because every once in a while you can get a reading that is way out of range.  This is due to the OS executing other tasks before getting your distance reading.  It is why I use a sample of readings.  I can always trust that the median of my sample of 11 readings is good.
+
+Highly accurate readings are not required for some applications. For example I use this module in an application I wrote for a sump pump monitor.  I am not worried about millimeter accuracy for that application.  1 cm variance on a meter deep pit is close enough to alert me to problems.
+
+Another example would be to calculate the water volume of a drinking water well (standing cylinder shape).
+It would not matter if you are a gallon off on a 1000 gallon reading.
+
+
+## Distance Limitations
+
+The HCSR04 sensor is suited for short distance readings.  The specification manual says it is suitable up to 13 feet.  I have tested it to go further than that, but anything over 12 feet starts having periodic strange readings.
+This module is not suitable for long distances.
+
+
+## Usage
+
+See example scripts in https://github.com/alaudet/hcsr04sensor/tree/master/recipes
+
+Access to Raspberry Pi GPIO pins requires the user account to be in the Linux gpio group.
+
+To add your user account name to the gpio group;
+
+    sudo usermod -aG gpio username
+
+## Testing the Module
+
+Added a script that is installed to /usr/local/bin called hcsr04.py.
+This utility does not presently support BOARD pin values.  Use BCM pin values.
+
+usage: hcsr04.py [-h] -t TRIG -e ECHO [-sp SPEED] [-ss SAMPLES]
+
+## Take a Basic Reading
+
+If you don't want to use a sample of readings for error handling, warnings or pin cleanups I have included a static method in the Measurement class that will return a basic metric reading.  It returns the exact one-time reading that is provided  by the sensor and RPi.GPIO.  This allows you to handle all of these things to your own preference in your code.
+
+See the example basic_reading.py script in https://github.com/alaudet/hcsr04sensor/tree/master/recipes
+
+
+## Contributing
+
+Read the contributing guidelines if you are interested in collaborating on this project.
+
+
+## Donate
+
+[Your Donation is Appreciated](https://www.linuxnorth.org/donate/)
```

### Comparing `hcsr04sensor-1.6.3/hcsr04sensor/sensor.py` & `hcsr04sensor-1.7/hcsr04sensor/sensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""Measure the distance or depth with an HCSR04 Ultrasonic sound 
+"""Measure the distance or depth with an HCSR04 Ultrasonic sound
 sensor and a Raspberry Pi.  Imperial and Metric measurements are available"""
 
 # Al Audet
 # MIT License
 from __future__ import division
 
 import time
 import math
 import warnings
 import RPi.GPIO as GPIO
 
 
 class Measurement(object):
-    """Create a measurement using a HC-SR04 Ultrasonic Sensor connected to 
+    """Create a measurement using a HC-SR04 Ultrasonic Sensor connected to
     the GPIO pins of a Raspberry Pi.
 
     Metric values are used by default. For imperial values use
     unit='imperial'
     temperature=<Desired temperature in Fahrenheit>
     """
 
@@ -27,32 +27,32 @@
         self.echo_pin = echo_pin
         self.temperature = temperature
         self.unit = unit
         self.gpio_mode = gpio_mode
         self.pi = math.pi
 
     def raw_distance(self, sample_size=11, sample_wait=0.1):
-        """Return an error corrected unrounded distance, in cm, of an object 
+        """Return an error corrected unrounded distance, in cm, of an object
         adjusted for temperature in Celcius.  The distance calculated
         is the median value of a sample of `sample_size` readings.
 
 
         Speed of readings is a result of two variables.  The sample_size
         per reading and the sample_wait (interval between individual samples).
 
-        Example: To use a sample size of 5 instead of 11 will increase the 
+        Example: To use a sample size of 5 instead of 11 will increase the
         speed of your reading but could increase variance in readings;
 
         value = sensor.Measurement(trig_pin, echo_pin)
         r = value.raw_distance(sample_size=5)
 
         Adjusting the interval between individual samples can also
         increase the speed of the reading.  Increasing the speed will also
         increase CPU usage.  Setting it too low will cause errors.  A default
-        of sample_wait=0.1 is a good balance between speed and minimizing 
+        of sample_wait=0.1 is a good balance between speed and minimizing
         CPU usage.  It is also a safe setting that should not cause errors.
 
         e.g.
 
         r = value.raw_distance(sample_wait=0.03)
         """
 
@@ -153,18 +153,18 @@
         s_min_a = height / 2  # semi minor axis
         if depth > height or depth < 0:
             raise ValueError("Depth must be less than the height and not less than 0")
         volume = (
             length
             * (s_maj_a / s_min_a)
             * (
-                (self.pi * (s_min_a ** 2)) / 2
+                (self.pi * (s_min_a**2)) / 2
                 + (depth - s_min_a)
-                * math.sqrt((s_min_a ** 2) - ((depth - s_min_a) ** 2))
-                + (s_min_a ** 2) * math.asin(depth / s_min_a - 1)
+                * math.sqrt((s_min_a**2) - ((depth - s_min_a) ** 2))
+                + (s_min_a**2) * math.asin(depth / s_min_a - 1)
             )
         )
 
         if self.unit == "metric":
             return volume / 1000
         else:
             return volume / 231
```

### Comparing `hcsr04sensor-1.6.3/bin/hcsr04.py` & `hcsr04sensor-1.7/bin/hcsr04.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,35 +47,36 @@
         help="Reading Sample Size (Optional - must be an \
                                 integer, default is 11)",
         required=False,
         default=11,
     )
 
     args = parser.parse_args()
+
     trig = args.trig
     echo = args.echo
     speed = args.speed
     samples = args.samples
+
     return trig, echo, speed, samples
 
 
 def main():
     """Main function to run the sensor with passed arguments"""
 
     trig, echo, speed, samples = get_args()
-    print("trig pin = gpio {}".format(trig))
-    print("echo pin = gpio {}".format(echo))
-    print("speed = {}".format(speed))
-    print("samples = {}".format(samples))
-    print("")
 
+    print(f"trig pin = gpio {trig}")
+    print(f"echo pin = gpio {echo}")
+    print(f"speed = {speed}")
+    print(f"samples = {samples}")
+    print("")
     value = sensor.Measurement(trig, echo)
     raw_distance = value.raw_distance(sample_size=samples, sample_wait=speed)
-
-    imperial_distance = value.distance_imperial(raw_distance)
-    metric_distance = value.distance_metric(raw_distance)
-    print("The imperial distance is {} inches.".format(round(imperial_distance, 1)))
-    print("The metric distance is {} centimetres.".format(round(metric_distance, 1)))
+    imperial_distance = value.distance(raw_distance) * 0.394
+    metric_distance = value.distance(raw_distance)
+    print(f"The imperial distance is {round(imperial_distance, 1)} inches.")
+    print(f"The metric distance is {round(metric_distance, 1)} centimetres.")
 
 
 if __name__ == "__main__":
     main()
```

