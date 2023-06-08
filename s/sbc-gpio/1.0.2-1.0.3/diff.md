# Comparing `tmp/sbc_gpio-1.0.2.tar.gz` & `tmp/sbc_gpio-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbc_gpio-1.0.2.tar", last modified: Thu Jun  8 06:00:47 2023, max compression
+gzip compressed data, was "sbc_gpio-1.0.3.tar", last modified: Thu Jun  8 06:11:05 2023, max compression
```

## Comparing `sbc_gpio-1.0.2.tar` & `sbc_gpio-1.0.3.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-06-08 06:00:47.017150 sbc_gpio-1.0.2/
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     1095 2023-05-01 17:06:12.000000 sbc_gpio-1.0.2/LICENSE
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)      690 2023-06-08 06:00:47.017150 sbc_gpio-1.0.2/PKG-INFO
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)      984 2023-06-08 05:42:09.000000 sbc_gpio-1.0.2/pyproject.toml
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)       38 2023-06-08 06:00:47.017150 sbc_gpio-1.0.2/setup.cfg
-drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-06-08 06:00:47.010483 sbc_gpio-1.0.2/src/
-drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-06-08 06:00:47.013816 sbc_gpio-1.0.2/src/sbc_gpio/
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)       62 2023-06-08 03:34:57.000000 sbc_gpio-1.0.2/src/sbc_gpio/DIR.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)      105 2023-05-01 16:10:24.000000 sbc_gpio-1.0.2/src/sbc_gpio/EVENT.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)       77 2023-05-01 16:10:30.000000 sbc_gpio-1.0.2/src/sbc_gpio/PULL.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)    22859 2023-06-08 03:56:52.000000 sbc_gpio-1.0.2/src/sbc_gpio/__init__.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)    11583 2023-06-08 03:59:36.000000 sbc_gpio-1.0.2/src/sbc_gpio/__main__.py
-drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-06-08 06:00:47.013816 sbc_gpio-1.0.2/src/sbc_gpio/device_tests/
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     6497 2023-05-01 17:05:09.000000 sbc_gpio-1.0.2/src/sbc_gpio/device_tests/_test_base.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     3843 2023-04-24 05:33:29.000000 sbc_gpio-1.0.2/src/sbc_gpio/device_tests/bmx_spi.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     2390 2023-04-24 05:41:03.000000 sbc_gpio-1.0.2/src/sbc_gpio/device_tests/button_gpiod.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     4556 2023-04-21 05:07:35.000000 sbc_gpio-1.0.2/src/sbc_gpio/device_tests/dht_spi.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     3910 2023-04-21 05:05:08.000000 sbc_gpio-1.0.2/src/sbc_gpio/device_tests/i2c_display.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)    15093 2023-05-11 06:04:40.000000 sbc_gpio-1.0.2/src/sbc_gpio/device_tests/ir.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     3381 2023-04-21 05:27:04.000000 sbc_gpio-1.0.2/src/sbc_gpio/device_tests/led_gpiod.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     7952 2023-04-30 05:51:05.000000 sbc_gpio-1.0.2/src/sbc_gpio/device_tests/uart.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     6449 2023-06-08 05:39:56.000000 sbc_gpio-1.0.2/src/sbc_gpio/dynamic_dts.py
-drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-06-08 06:00:47.013816 sbc_gpio-1.0.2/src/sbc_gpio/gpio_libs/
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     2759 2023-06-06 02:23:36.000000 sbc_gpio-1.0.2/src/sbc_gpio/gpio_libs/_generic_gpio.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     6439 2023-05-11 06:05:12.000000 sbc_gpio-1.0.2/src/sbc_gpio/gpio_libs/gpiod.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     4391 2023-05-11 06:05:12.000000 sbc_gpio-1.0.2/src/sbc_gpio/gpio_libs/rpi_gpio.py
-drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-06-08 06:00:47.017150 sbc_gpio-1.0.2/src/sbc_gpio/platforms/
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     1589 2023-06-08 05:46:58.000000 sbc_gpio-1.0.2/src/sbc_gpio/platforms/_generic.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     1355 2023-06-08 03:52:31.000000 sbc_gpio-1.0.2/src/sbc_gpio/platforms/pi4b.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     5453 2023-06-08 03:49:47.000000 sbc_gpio-1.0.2/src/sbc_gpio/platforms/rock5b.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)      609 2023-06-08 05:41:51.000000 sbc_gpio-1.0.2/src/sbc_gpio/scripts.py
-drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-06-08 06:00:47.017150 sbc_gpio-1.0.2/src/sbc_gpio/tests/
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     9523 2023-05-11 06:05:12.000000 sbc_gpio-1.0.2/src/sbc_gpio/tests/devtester_test.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     1861 2023-06-08 04:00:27.000000 sbc_gpio-1.0.2/src/sbc_gpio/tests/sbc_test.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)      230 2023-06-06 21:23:52.000000 sbc_gpio-1.0.2/src/sbc_gpio/tests/test_dynamic_overlay.py
-drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-06-08 06:00:47.013816 sbc_gpio-1.0.2/src/sbc_gpio.egg-info/
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)      690 2023-06-08 06:00:47.000000 sbc_gpio-1.0.2/src/sbc_gpio.egg-info/PKG-INFO
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)      989 2023-06-08 06:00:47.000000 sbc_gpio-1.0.2/src/sbc_gpio.egg-info/SOURCES.txt
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)        1 2023-06-08 06:00:47.000000 sbc_gpio-1.0.2/src/sbc_gpio.egg-info/dependency_links.txt
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)       86 2023-06-08 06:00:47.000000 sbc_gpio-1.0.2/src/sbc_gpio.egg-info/entry_points.txt
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)        9 2023-06-08 06:00:47.000000 sbc_gpio-1.0.2/src/sbc_gpio.egg-info/top_level.txt
+drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-06-08 06:11:05.059244 sbc_gpio-1.0.3/
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     1095 2023-05-01 17:06:12.000000 sbc_gpio-1.0.3/LICENSE
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)      699 2023-06-08 06:11:05.059244 sbc_gpio-1.0.3/PKG-INFO
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)      994 2023-06-08 06:10:54.000000 sbc_gpio-1.0.3/pyproject.toml
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)       38 2023-06-08 06:11:05.059244 sbc_gpio-1.0.3/setup.cfg
+drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-06-08 06:11:05.052578 sbc_gpio-1.0.3/src/
+drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-06-08 06:11:05.055911 sbc_gpio-1.0.3/src/sbc_gpio/
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)       62 2023-06-08 03:34:57.000000 sbc_gpio-1.0.3/src/sbc_gpio/DIR.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)      105 2023-05-01 16:10:24.000000 sbc_gpio-1.0.3/src/sbc_gpio/EVENT.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)       77 2023-05-01 16:10:30.000000 sbc_gpio-1.0.3/src/sbc_gpio/PULL.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)    22859 2023-06-08 03:56:52.000000 sbc_gpio-1.0.3/src/sbc_gpio/__init__.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)    11583 2023-06-08 03:59:36.000000 sbc_gpio-1.0.3/src/sbc_gpio/__main__.py
+drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-06-08 06:11:05.059244 sbc_gpio-1.0.3/src/sbc_gpio/device_tests/
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     6497 2023-05-01 17:05:09.000000 sbc_gpio-1.0.3/src/sbc_gpio/device_tests/_test_base.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     3843 2023-04-24 05:33:29.000000 sbc_gpio-1.0.3/src/sbc_gpio/device_tests/bmx_spi.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     2390 2023-04-24 05:41:03.000000 sbc_gpio-1.0.3/src/sbc_gpio/device_tests/button_gpiod.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     4556 2023-04-21 05:07:35.000000 sbc_gpio-1.0.3/src/sbc_gpio/device_tests/dht_spi.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     3910 2023-04-21 05:05:08.000000 sbc_gpio-1.0.3/src/sbc_gpio/device_tests/i2c_display.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)    15093 2023-05-11 06:04:40.000000 sbc_gpio-1.0.3/src/sbc_gpio/device_tests/ir.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     3381 2023-04-21 05:27:04.000000 sbc_gpio-1.0.3/src/sbc_gpio/device_tests/led_gpiod.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     7952 2023-04-30 05:51:05.000000 sbc_gpio-1.0.3/src/sbc_gpio/device_tests/uart.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     6449 2023-06-08 05:39:56.000000 sbc_gpio-1.0.3/src/sbc_gpio/dynamic_dts.py
+drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-06-08 06:11:05.059244 sbc_gpio-1.0.3/src/sbc_gpio/gpio_libs/
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     2759 2023-06-06 02:23:36.000000 sbc_gpio-1.0.3/src/sbc_gpio/gpio_libs/_generic_gpio.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     6439 2023-05-11 06:05:12.000000 sbc_gpio-1.0.3/src/sbc_gpio/gpio_libs/gpiod.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     4391 2023-05-11 06:05:12.000000 sbc_gpio-1.0.3/src/sbc_gpio/gpio_libs/rpi_gpio.py
+drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-06-08 06:11:05.059244 sbc_gpio-1.0.3/src/sbc_gpio/platforms/
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     1589 2023-06-08 05:46:58.000000 sbc_gpio-1.0.3/src/sbc_gpio/platforms/_generic.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     1355 2023-06-08 03:52:31.000000 sbc_gpio-1.0.3/src/sbc_gpio/platforms/pi4b.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     5453 2023-06-08 03:49:47.000000 sbc_gpio-1.0.3/src/sbc_gpio/platforms/rock5b.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)      609 2023-06-08 05:41:51.000000 sbc_gpio-1.0.3/src/sbc_gpio/scripts.py
+drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-06-08 06:11:05.059244 sbc_gpio-1.0.3/src/sbc_gpio/tests/
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     9523 2023-05-11 06:05:12.000000 sbc_gpio-1.0.3/src/sbc_gpio/tests/devtester_test.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     1861 2023-06-08 04:00:27.000000 sbc_gpio-1.0.3/src/sbc_gpio/tests/sbc_test.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)      230 2023-06-06 21:23:52.000000 sbc_gpio-1.0.3/src/sbc_gpio/tests/test_dynamic_overlay.py
+drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-06-08 06:11:05.055911 sbc_gpio-1.0.3/src/sbc_gpio.egg-info/
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)      699 2023-06-08 06:11:05.000000 sbc_gpio-1.0.3/src/sbc_gpio.egg-info/PKG-INFO
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     1024 2023-06-08 06:11:05.000000 sbc_gpio-1.0.3/src/sbc_gpio.egg-info/SOURCES.txt
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)        1 2023-06-08 06:11:05.000000 sbc_gpio-1.0.3/src/sbc_gpio.egg-info/dependency_links.txt
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)       86 2023-06-08 06:11:05.000000 sbc_gpio-1.0.3/src/sbc_gpio.egg-info/entry_points.txt
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)       84 2023-06-08 06:11:05.000000 sbc_gpio-1.0.3/src/sbc_gpio.egg-info/requires.txt
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)        9 2023-06-08 06:11:05.000000 sbc_gpio-1.0.3/src/sbc_gpio.egg-info/top_level.txt
```

### Comparing `sbc_gpio-1.0.2/LICENSE` & `sbc_gpio-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sbc_gpio-1.0.2/PKG-INFO` & `sbc_gpio-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: sbc_gpio
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python Library for abstraction GPIO and for SBC testing
 Author-email: Thomas Dunteman <git@learningtopi.com>
 Project-URL: Homepage, https://www.learningtopi.com/python-modules-applications/sbc_gpio/
 Project-URL: Bug Tracker, https://github.com/LearningToPi/sbc_gpio/issues
 Project-URL: Source Code, https://github.com/LearningToPi/sbc_gpio
-Keywords: sbc,gpio
+Keywords: sbc,gpio,overlays
 Classifier: Topic :: System :: Logging
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sbc_gpio-1.0.2/pyproject.toml` & `sbc_gpio-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [project]
 name = "sbc_gpio"
-version = "1.0.2"
+version = "1.0.3"
 description = "Python Library for abstraction GPIO and for SBC testing"
 authors = [{name = "Thomas Dunteman", email= "git@learningtopi.com"}]
-keywords = ["sbc", "gpio"]
+keywords = ["sbc", "gpio", "overlays"]
 readme = "README.md"
 requires-python =">=3.8"
 classifiers = [
     "Topic :: System :: Logging",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3"
 ]
-dependencies = []
+dependencies = ["gpiod", "bmx280-spi", "dht11-spi", "Jinja2", "lirc",
+            "logging-handler", "pyserial", "RPLCD", "smbus2", "spidev"]
 
 [project.urls]
 "Homepage" = "https://www.learningtopi.com/python-modules-applications/sbc_gpio/"
 "Bug Tracker" = "https://github.com/LearningToPi/sbc_gpio/issues"
 "Source Code" = "https://github.com/LearningToPi/sbc_gpio"
 
 [build-system]
-requires = ["setuptools>=61", "gpiod", "bmx280-spi", "dht11-spi", "Jinja2", "lirc",
-            "logging-handler", "pyserial", "RPLCD", "smbus2", "spidev"]
+requires = ["setuptools>=61"]
 build-backend = "setuptools.build_meta"
 
 [project.scripts]
 "update_dynamic_overlay.py"="sbc_gpio.scripts:update_dynamic_overlay"
```

### Comparing `sbc_gpio-1.0.2/src/sbc_gpio/__init__.py` & `sbc_gpio-1.0.3/src/sbc_gpio/__init__.py`

 * *Files identical despite different names*

### Comparing `sbc_gpio-1.0.2/src/sbc_gpio/__main__.py` & `sbc_gpio-1.0.3/src/sbc_gpio/__main__.py`

 * *Files identical despite different names*

### Comparing `sbc_gpio-1.0.2/src/sbc_gpio/device_tests/_test_base.py` & `sbc_gpio-1.0.3/src/sbc_gpio/device_tests/_test_base.py`

 * *Files identical despite different names*

### Comparing `sbc_gpio-1.0.2/src/sbc_gpio/device_tests/bmx_spi.py` & `sbc_gpio-1.0.3/src/sbc_gpio/device_tests/bmx_spi.py`

 * *Files identical despite different names*

### Comparing `sbc_gpio-1.0.2/src/sbc_gpio/device_tests/button_gpiod.py` & `sbc_gpio-1.0.3/src/sbc_gpio/device_tests/button_gpiod.py`

 * *Files identical despite different names*

### Comparing `sbc_gpio-1.0.2/src/sbc_gpio/device_tests/dht_spi.py` & `sbc_gpio-1.0.3/src/sbc_gpio/device_tests/dht_spi.py`

 * *Files identical despite different names*

### Comparing `sbc_gpio-1.0.2/src/sbc_gpio/device_tests/i2c_display.py` & `sbc_gpio-1.0.3/src/sbc_gpio/device_tests/i2c_display.py`

 * *Files identical despite different names*

### Comparing `sbc_gpio-1.0.2/src/sbc_gpio/device_tests/ir.py` & `sbc_gpio-1.0.3/src/sbc_gpio/device_tests/ir.py`

 * *Files identical despite different names*

### Comparing `sbc_gpio-1.0.2/src/sbc_gpio/device_tests/led_gpiod.py` & `sbc_gpio-1.0.3/src/sbc_gpio/device_tests/led_gpiod.py`

 * *Files identical despite different names*

### Comparing `sbc_gpio-1.0.2/src/sbc_gpio/device_tests/uart.py` & `sbc_gpio-1.0.3/src/sbc_gpio/device_tests/uart.py`

 * *Files identical despite different names*

### Comparing `sbc_gpio-1.0.2/src/sbc_gpio/dynamic_dts.py` & `sbc_gpio-1.0.3/src/sbc_gpio/dynamic_dts.py`

 * *Files identical despite different names*

### Comparing `sbc_gpio-1.0.2/src/sbc_gpio/gpio_libs/_generic_gpio.py` & `sbc_gpio-1.0.3/src/sbc_gpio/gpio_libs/_generic_gpio.py`

 * *Files identical despite different names*

### Comparing `sbc_gpio-1.0.2/src/sbc_gpio/gpio_libs/gpiod.py` & `sbc_gpio-1.0.3/src/sbc_gpio/gpio_libs/gpiod.py`

 * *Files identical despite different names*

### Comparing `sbc_gpio-1.0.2/src/sbc_gpio/gpio_libs/rpi_gpio.py` & `sbc_gpio-1.0.3/src/sbc_gpio/gpio_libs/rpi_gpio.py`

 * *Files identical despite different names*

### Comparing `sbc_gpio-1.0.2/src/sbc_gpio/platforms/_generic.py` & `sbc_gpio-1.0.3/src/sbc_gpio/platforms/_generic.py`

 * *Files identical despite different names*

### Comparing `sbc_gpio-1.0.2/src/sbc_gpio/platforms/pi4b.py` & `sbc_gpio-1.0.3/src/sbc_gpio/platforms/pi4b.py`

 * *Files identical despite different names*

### Comparing `sbc_gpio-1.0.2/src/sbc_gpio/platforms/rock5b.py` & `sbc_gpio-1.0.3/src/sbc_gpio/platforms/rock5b.py`

 * *Files identical despite different names*

### Comparing `sbc_gpio-1.0.2/src/sbc_gpio/scripts.py` & `sbc_gpio-1.0.3/src/sbc_gpio/scripts.py`

 * *Files identical despite different names*

### Comparing `sbc_gpio-1.0.2/src/sbc_gpio/tests/devtester_test.py` & `sbc_gpio-1.0.3/src/sbc_gpio/tests/devtester_test.py`

 * *Files identical despite different names*

### Comparing `sbc_gpio-1.0.2/src/sbc_gpio/tests/sbc_test.py` & `sbc_gpio-1.0.3/src/sbc_gpio/tests/sbc_test.py`

 * *Files identical despite different names*

### Comparing `sbc_gpio-1.0.2/src/sbc_gpio.egg-info/PKG-INFO` & `sbc_gpio-1.0.3/src/sbc_gpio.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: sbc-gpio
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python Library for abstraction GPIO and for SBC testing
 Author-email: Thomas Dunteman <git@learningtopi.com>
 Project-URL: Homepage, https://www.learningtopi.com/python-modules-applications/sbc_gpio/
 Project-URL: Bug Tracker, https://github.com/LearningToPi/sbc_gpio/issues
 Project-URL: Source Code, https://github.com/LearningToPi/sbc_gpio
-Keywords: sbc,gpio
+Keywords: sbc,gpio,overlays
 Classifier: Topic :: System :: Logging
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sbc_gpio-1.0.2/src/sbc_gpio.egg-info/SOURCES.txt` & `sbc_gpio-1.0.3/src/sbc_gpio.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 src/sbc_gpio/__main__.py
 src/sbc_gpio/dynamic_dts.py
 src/sbc_gpio/scripts.py
 src/sbc_gpio.egg-info/PKG-INFO
 src/sbc_gpio.egg-info/SOURCES.txt
 src/sbc_gpio.egg-info/dependency_links.txt
 src/sbc_gpio.egg-info/entry_points.txt
+src/sbc_gpio.egg-info/requires.txt
 src/sbc_gpio.egg-info/top_level.txt
 src/sbc_gpio/device_tests/_test_base.py
 src/sbc_gpio/device_tests/bmx_spi.py
 src/sbc_gpio/device_tests/button_gpiod.py
 src/sbc_gpio/device_tests/dht_spi.py
 src/sbc_gpio/device_tests/i2c_display.py
 src/sbc_gpio/device_tests/ir.py
```

