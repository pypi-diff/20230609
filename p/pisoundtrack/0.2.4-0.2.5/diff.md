# Comparing `tmp/pisoundtrack-0.2.4.tar.gz` & `tmp/pisoundtrack-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pisoundtrack-0.2.4.tar", last modified: Thu Jun  1 14:32:30 2023, max compression
+gzip compressed data, was "pisoundtrack-0.2.5.tar", last modified: Fri Jun  9 07:01:02 2023, max compression
```

## Comparing `pisoundtrack-0.2.4.tar` & `pisoundtrack-0.2.5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:30.834955 pisoundtrack-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-01 14:32:19.000000 pisoundtrack-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-01 14:32:30.834955 pisoundtrack-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-01 14:32:19.000000 pisoundtrack-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:30.830953 pisoundtrack-0.2.4/pisoundtrack/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-01 14:32:19.000000 pisoundtrack-0.2.4/pisoundtrack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-01 14:32:19.000000 pisoundtrack-0.2.4/pisoundtrack/config-template.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-06-01 14:32:19.000000 pisoundtrack-0.2.4/pisoundtrack/soundtrack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:30.830953 pisoundtrack-0.2.4/pisoundtrack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-01 14:32:30.000000 pisoundtrack-0.2.4/pisoundtrack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-01 14:32:30.000000 pisoundtrack-0.2.4/pisoundtrack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:32:30.000000 pisoundtrack-0.2.4/pisoundtrack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-01 14:32:30.000000 pisoundtrack-0.2.4/pisoundtrack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-01 14:32:30.000000 pisoundtrack-0.2.4/pisoundtrack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:32:30.834955 pisoundtrack-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-01 14:32:19.000000 pisoundtrack-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:01:02.105104 pisoundtrack-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-09 07:00:44.000000 pisoundtrack-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-09 07:01:02.105104 pisoundtrack-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-09 07:00:44.000000 pisoundtrack-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:01:02.101104 pisoundtrack-0.2.5/pisoundtrack/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-09 07:00:44.000000 pisoundtrack-0.2.5/pisoundtrack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-09 07:00:44.000000 pisoundtrack-0.2.5/pisoundtrack/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-09 07:00:44.000000 pisoundtrack-0.2.5/pisoundtrack/config-template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-06-09 07:00:44.000000 pisoundtrack-0.2.5/pisoundtrack/soundtrack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:01:02.105104 pisoundtrack-0.2.5/pisoundtrack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-09 07:01:01.000000 pisoundtrack-0.2.5/pisoundtrack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-09 07:01:02.000000 pisoundtrack-0.2.5/pisoundtrack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 07:01:01.000000 pisoundtrack-0.2.5/pisoundtrack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-09 07:01:01.000000 pisoundtrack-0.2.5/pisoundtrack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-09 07:01:01.000000 pisoundtrack-0.2.5/pisoundtrack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 07:01:02.105104 pisoundtrack-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-09 07:00:44.000000 pisoundtrack-0.2.5/setup.py
```

### Comparing `pisoundtrack-0.2.4/LICENSE` & `pisoundtrack-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pisoundtrack-0.2.4/PKG-INFO` & `pisoundtrack-0.2.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 Metadata-Version: 2.1
 Name: pisoundtrack
-Version: 0.2.4
+Version: 0.2.5
 Summary: Raspberry Pi Sound tracking and influx output
 Home-page: https://github.com/Phornee/pisoundtrack
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
+Description: # pisoundtrack
+        Track sounds from mic and outputs it to influx
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Home Automation
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# pisoundtrack
-Track sounds from mic and outputs it to influx
-
-
```

### Comparing `pisoundtrack-0.2.4/pisoundtrack/soundtrack.py` & `pisoundtrack-0.2.5/pisoundtrack/soundtrack.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,116 +1,126 @@
-""" """
+""" Decibels calculator utitlty class """
 import os
-from datetime import datetime
 from pathlib import Path
 import math
+import logging
 
 import numpy
 import pyaudio
 
 from influxdb_wrapper import influxdb_factory
-from log_mgr import Logger
 from config_yml import Config
 
 SHORT_NORMALIZE = (1.0 / 32768.0)
 INPUT_BLOCK_TIME = 0.10
 SILENCE_SAMPLE_LEVEL = 251
 MIN_AUDIBLE_LEVEL = 0.00727  # 20 uPascals
 
 
 class Soundtrack():
-    def __init__(self, dry_run: bool = False):
-        self.logger = Logger(self.class_name(), 'soundtrack', dry_run=dry_run)
+    """ Samples the sound using a microphone, calculates Decibels, and output them to an influx db.
+    """
+    def __init__(self):
+        self.logger = logging.getLogger()
         self.logger.info("Initializing Soundtrack...")
         template_config_path = os.path.join(Path(__file__).parent.resolve(), './config-template.yml')
 
         self.config = Config(package_name=self.class_name(),
                              template_path=template_config_path,
                              config_file_name="config.yml")
 
         influx_conn_type = self.config['influxdbconn'].get('type', 'influx')
         self.conn = influxdb_factory(influx_conn_type)
-        self.conn.openConn(self.config['influxdbconn'])
+        self.conn.open_conn(self.config['influxdbconn'])
 
     @classmethod
     def class_name(cls):
+        """ class name """
         return "soundtrack"
 
-    def get_rms(self, block):
-        # RMS amplitude is defined as the square root of the
-        # mean over time of the square of the amplitude.
-
+    def get_rms(self, block) -> float:
+        """ Calculates RMS for a block of samples
+            RMS amplitude is defined as the square root of the
+            mean over time of the square of the amplitude.
+        Args:
+            block (bytes): Raw samples
+        Returns:
+            _type_: _description_
+        """
         # SHORT_NORMALIZE = (1.0 / 32768.0)
         SHORT_NORMALIZE = (1.0 / 26000.0)
 
         # iterate over the block.
         sum_squares = 0.0
         for sample in block:
             norm_sample = sample * SHORT_NORMALIZE
             sum_squares += norm_sample * norm_sample
 
         return math.sqrt(sum_squares / block.size)
 
-    def sensorRead(self):
-        """
-        Read sensors information
-        """
-        have_readings = False
-
-        print("Initializing Pyaudio....")
+    def open_device(self, device_name):
+        """ Open an input device stream """
         self.logger.info("Initializing Pyaudio...")
         pyaud = pyaudio.PyAudio()
 
-        device_name = u'WordForum USB: Audio'
-
-        print("Getting devices...")
+        self.logger.info("Getting devices...")
         info = pyaud.get_host_api_info_by_index(0)
         num_devices = info.get('deviceCount')
         input_device = -1
         for i in range(0, num_devices):
             device_info = pyaud.get_device_info_by_host_api_device_index(0, i)
-            print(f"Evaluating device {device_info.get('name')}...")
+            self.logger.debug("Evaluating device %s...", device_info.get('name'))
             if device_info.get('name').startswith(device_name):
                 if (device_info.get('maxInputChannels')) > 0:
                     sampling_rate = int(device_info.get('defaultSampleRate'))
-                    print(f"Input Device id {i} - {device_info.get('name')}")
-                    print(f"Sampling Rate - {sampling_rate}")
+                    self.logger.debug("Input Device id %i - %s", i , device_info.get('name'))
+                    self.logger.debug("Sampling Rate - %s", sampling_rate)
                     input_device = i
                     break
-                else:
-                    self.logger.error(f"Device {device_name} has no input channels.")
+                self.logger.error("Device %s has no input channels.", device_name)
 
         if input_device == -1:
-            self.logger.error(f"Input Device {device_name} not found.")
-            return -1
+            self.logger.error("Input Device %s not found.", device_name)
+            return None, 0
 
         input_frames_per_block = int(sampling_rate * INPUT_BLOCK_TIME)
 
         stream = pyaud.open(format=pyaudio.paInt16, channels=1, rate=sampling_rate, input_device_index=input_device,
                             input=True, frames_per_buffer=input_frames_per_block)
+        return stream, input_frames_per_block
+
+    def microphone_listen(self):
+        """
+        Read sensors information
+        """
+        device_name = 'WordForum USB: Audio'
+        stream, input_frames_per_block= self.open_device(device_name)
+
+        if not stream:
+            return
 
         while True:
             num_seconds = 0
             max_read = 0
             while num_seconds < 60:
                 raw = stream.read(input_frames_per_block, exception_on_overflow=False)
                 samples = numpy.frombuffer(raw, dtype=numpy.int16)
                 rms = self.get_rms(samples)
                 if rms > max_read:
                     max_read = rms
-                print("{:.2f}".format(rms))
+                self.logger.debug("%0.2f", rms)
                 num_seconds += 1
 
             # Decibel conversion
             if MIN_AUDIBLE_LEVEL > max_read:
                 decibels = 0.0
             else:
                 decibels = 20 * math.log10(max_read/MIN_AUDIBLE_LEVEL)
 
-            self.logger.info(f"Decibels = {decibels}")
+            self.logger.info("Decibels = %i", decibels)
             points = [
                 {
                     "tags": {
                         "soundid": self.config['id']
                     },
                     "fields": {
                         "max": float(max_read),
@@ -120,20 +130,11 @@
                     }
                 }
             ]
 
             try:
                 self.conn.insert("sound", points)
             except Exception as ex:
-                self.logger.error(f"RuntimeError: {ex}")
+                self.logger.error("RuntimeError: %s", ex)
                 url = self.config['influxdbconn']['url']
                 token = self.config['influxdbconn']['token']
-                self.logger.error(f"influxDBURL={url} | influxDBToken={token}")
-
-if __name__ == "__main__":
-    sensors_instance = Soundtrack()
-    sensors_instance.sensorRead()
-
-
-
-
-
+                self.logger.error("influxDBURL=%s | influxDBToken=%s", url, token)
```

### Comparing `pisoundtrack-0.2.4/pisoundtrack.egg-info/PKG-INFO` & `pisoundtrack-0.2.5/pisoundtrack.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 Metadata-Version: 2.1
 Name: pisoundtrack
-Version: 0.2.4
+Version: 0.2.5
 Summary: Raspberry Pi Sound tracking and influx output
 Home-page: https://github.com/Phornee/pisoundtrack
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
+Description: # pisoundtrack
+        Track sounds from mic and outputs it to influx
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Home Automation
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# pisoundtrack
-Track sounds from mic and outputs it to influx
-
-
```

### Comparing `pisoundtrack-0.2.4/setup.py` & `pisoundtrack-0.2.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pisoundtrack",
-    version="0.2.4",
+    version="0.2.5",
     author="Ismael Raya",
     author_email="phornee@gmail.com",
     description="Raspberry Pi Sound tracking and influx output",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Phornee/pisoundtrack",
     packages=setuptools.find_packages(),
@@ -21,12 +21,13 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: POSIX :: Linux",
         "Topic :: Home Automation"
     ],
     install_requires=[
         'config_yml>=0.3.1',
         'log_mgr>=0.0.2',
-        'influxdb>=5.3.1',
-        'numpy>=1.21.5'
+        'influxdb_wrapper>=0.0.5',
+        'numpy>=1.21.5',
+        'pyaudio==0.2.11'
     ],
     python_requires='>=3.6',
 )
```

