# Comparing `tmp/yinstruments-1.2.2.tar.gz` & `tmp/yinstruments-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yinstruments-1.2.2.tar", last modified: Mon Nov 21 16:15:34 2022, max compression
+gzip compressed data, was "yinstruments-1.3.0.tar", last modified: Fri Jun  9 19:52:27 2023, max compression
```

## Comparing `yinstruments-1.2.2.tar` & `yinstruments-1.3.0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxr-x   0 jgoeders  (1002) jgoeders  (1002)        0 2022-11-21 16:15:34.120825 yinstruments-1.2.2/
--rw-rw-r--   0 jgoeders  (1002) jgoeders  (1002)      323 2022-11-21 16:15:34.120825 yinstruments-1.2.2/PKG-INFO
--rw-rw-r--   0 jgoeders  (1002) jgoeders  (1002)       38 2022-11-21 16:15:34.120825 yinstruments-1.2.2/setup.cfg
--rw-rw-r--   0 jgoeders  (1002) jgoeders  (1002)      392 2022-11-21 16:15:25.000000 yinstruments-1.2.2/setup.py
-drwxrwxr-x   0 jgoeders  (1002) jgoeders  (1002)        0 2022-11-21 16:15:34.120825 yinstruments-1.2.2/yinstruments/
--rw-rw-r--   0 jgoeders  (1002) jgoeders  (1002)     3481 2022-11-09 22:34:36.000000 yinstruments-1.2.2/yinstruments/async_reader.py
--rwxrwxr-x   0 jgoeders  (1002) jgoeders  (1002)     3626 2022-11-21 16:07:19.000000 yinstruments-1.2.2/yinstruments/netbooter.py
--rw-rw-r--   0 jgoeders  (1002) jgoeders  (1002)     6157 2022-11-07 19:07:39.000000 yinstruments-1.2.2/yinstruments/powersupply.py
--rw-rw-r--   0 jgoeders  (1002) jgoeders  (1002)     4122 2022-11-09 22:37:07.000000 yinstruments-1.2.2/yinstruments/usb_finder.py
--rw-rw-r--   0 jgoeders  (1002) jgoeders  (1002)     3626 2022-11-17 16:23:47.000000 yinstruments-1.2.2/yinstruments/usb_power.py
-drwxrwxr-x   0 jgoeders  (1002) jgoeders  (1002)        0 2022-11-21 16:15:34.120825 yinstruments-1.2.2/yinstruments.egg-info/
--rw-rw-r--   0 jgoeders  (1002) jgoeders  (1002)      323 2022-11-21 16:15:34.000000 yinstruments-1.2.2/yinstruments.egg-info/PKG-INFO
--rw-rw-r--   0 jgoeders  (1002) jgoeders  (1002)      323 2022-11-21 16:15:34.000000 yinstruments-1.2.2/yinstruments.egg-info/SOURCES.txt
--rw-rw-r--   0 jgoeders  (1002) jgoeders  (1002)        1 2022-11-21 16:15:34.000000 yinstruments-1.2.2/yinstruments.egg-info/dependency_links.txt
--rw-rw-r--   0 jgoeders  (1002) jgoeders  (1002)       14 2022-11-21 16:15:34.000000 yinstruments-1.2.2/yinstruments.egg-info/requires.txt
--rw-rw-r--   0 jgoeders  (1002) jgoeders  (1002)       13 2022-11-21 16:15:34.000000 yinstruments-1.2.2/yinstruments.egg-info/top_level.txt
+drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-06-09 19:52:27.097223 yinstruments-1.3.0/
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      312 2023-06-09 19:52:27.087223 yinstruments-1.3.0/PKG-INFO
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       38 2023-06-09 19:52:27.097223 yinstruments-1.3.0/setup.cfg
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      432 2023-06-09 19:50:33.000000 yinstruments-1.3.0/setup.py
+drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-06-09 19:52:27.087223 yinstruments-1.3.0/yinstruments/
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     3633 2023-06-06 14:51:33.000000 yinstruments-1.3.0/yinstruments/async_reader.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     5828 2023-06-09 19:36:07.000000 yinstruments-1.3.0/yinstruments/powersupply.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     4131 2023-06-09 19:32:01.000000 yinstruments-1.3.0/yinstruments/usb_finder.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     3564 2023-06-09 19:39:39.000000 yinstruments-1.3.0/yinstruments/usb_power.py
+drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-06-09 19:52:27.087223 yinstruments-1.3.0/yinstruments.egg-info/
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      312 2023-06-09 19:52:27.000000 yinstruments-1.3.0/yinstruments.egg-info/PKG-INFO
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      297 2023-06-09 19:52:27.000000 yinstruments-1.3.0/yinstruments.egg-info/SOURCES.txt
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)        1 2023-06-09 19:52:27.000000 yinstruments-1.3.0/yinstruments.egg-info/dependency_links.txt
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       45 2023-06-09 19:52:27.000000 yinstruments-1.3.0/yinstruments.egg-info/requires.txt
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       13 2023-06-09 19:52:27.000000 yinstruments-1.3.0/yinstruments.egg-info/top_level.txt
```

### Comparing `yinstruments-1.2.2/yinstruments/async_reader.py` & `yinstruments-1.3.0/yinstruments/async_reader.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,26 +21,29 @@
         # If there is already a line in the list from a previous read, then return it.
         if self.lines:
             return self.lines.pop(0)
 
         # Otherwise get some new data and split it into lines, and return the first line.
         try:
             new_text = self._get_data()
-        except serial.serialutil.SerialException as e:
-            raise ReaderError(e)
-        except UnicodeEncodeError as e:
-            raise ReaderError(e)
+        except serial.serialutil.SerialException as exc:
+            raise ReaderError(exc) from exc
+        except UnicodeEncodeError as exc:
+            raise ReaderError(exc) from exc
 
         if not new_text:
             return None
 
         # Clean up string
         new_text = new_text.replace("\r", "")
         new_text = new_text.replace("\0", "")
 
+        if not new_text:
+            return None
+
         lines = new_text.splitlines(keepends=True)
 
         lines[0] = self.partial_line + lines[0]
 
         # Save last line
         if lines[-1][-1] != "\n":
             self.partial_line = lines.pop()
@@ -58,14 +61,15 @@
 
         new_text = self._get_data()
         if new_text:
             self.text += new_text
         return self.text
 
     def clear_accumulate(self):
+        """Clear the accumulated text that is return in 'get_accumulate'"""
         self.text = ""
 
     @abstractmethod
     def _get_data(self):
         pass
```

### Comparing `yinstruments-1.2.2/yinstruments/powersupply.py` & `yinstruments-1.3.0/yinstruments/powersupply.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import vxi11
-import config
 
 
 class PowerSupply:
     # GET_MEAS = "MEAS:{measurement}? (@{channel})"
     # MAX_TRIES = 10
 
     def __init__(self, ip_address):
@@ -124,16 +123,12 @@
 
     #     # print("Data List: ", data_list)
     #     # print("Type: ", type(data_list))
     #     return data_list
 
 
 if __name__ == "__main__":
-    instr = PowerSupply(config.IP_POWERSUPPLY)
+    ip = "192.168.0.100"
+    instr = PowerSupply(ip)
 
-    # Turn on Zedboard
-    # instr.set_channel_voltage(config.POWER_SUPPLY_CHANNEL_ZEDBOARD, config.ZEDBOARD_VOLTAGE)
-    instr.disable_channel(config.POWER_SUPPLY_CHANNEL_ZEDBOARD)
-    # instr.enable_channel(config.POWER_SUPPLY_CHANNEL_ZEDBOARD)
-
-    # instr.set_channel_voltage(config.POWER_SUPPLY_CHANNEL_SRAM, 1.0)
-    # instr.enable_channel(config.POWER_SUPPLY_CHANNEL_SRAM)
+    instr.disable_channel(1)
+    # instr.enable_channel(1)
```

### Comparing `yinstruments-1.2.2/yinstruments/usb_finder.py` & `yinstruments-1.3.0/yinstruments/usb_finder.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     """This will find the correct /dev/ttyACMX file for a given physical USB port and interface."""
 
     match_str = match_str = "/devices/.*?/.*?/usb\d+/.*/(.*?)/tty/ttyACM\d+$"
     return _find_dev_file(usb_phys_port, "ACM", match_str, interface)
 
 
 def _find_dev_file(usb_phys_port, ttyType, match_str, interface):
-
     """This function will search through all /dev devices and find the one that maps to the given
     usb_phys_port, ttyType, regex match string and interface.
 
     This function works by running "udevadm info -q path -n /dev/ttyUSB0" for each serial port,
     and looking for the output that matches the location.  For example, if it is located at
     1-10.1, the output of interface 1 will be
     /devices/pci0000:00/0000:00:14.0/usb1/1-10/1-10.1/1-10.1:1.1/ttyUSB3/tty/ttyUSB3
@@ -62,16 +61,17 @@
                     )
                 match_found = f
                 # print(p.stdout.decode())
             if not m:
                 print(p.stdout.decode(), "did not match regex.")
                 assert False
     if match_found is None:
-        raise USBFindError("Could not find serial device at USB location "
-            + usb_phys_port + ":1." + str(interface))
+        raise USBFindError(
+            "Could not find serial device at USB location " + usb_phys_port + ":1." + str(interface)
+        )
 
     return match_found
 
 
 def find_dev_file_usb_bus(usb_phys_port):
     """
     For a given usb physical port, this function finds the USB bus device file.
```

### Comparing `yinstruments-1.2.2/yinstruments/usb_power.py` & `yinstruments-1.3.0/yinstruments/usb_power.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import subprocess
 import time
-
+import sys
 import argparse
 
 import pyhubctl
 
-from utils import error, print_color, TermColors
-
 # TODO: At one point uhubctl failed with the following error:
 # uhubctl: symbol lookup error: uhubctl: undefined symbol: libusb_free_container_id_descriptor
 # I restarted the NUC and it worked, but I don't know what went wrong.
 # That error was invisible to the other scripts...
 
 
 class USBPortPower:
@@ -40,15 +38,14 @@
         """Turn on port.  Can raise subprocess.CalledProcessError"""
         self.phc.run(
             pyhubctl.Configuration(action="on", location=self.usb_location, ports=self.usb_port)
         )
 
 
 def usbPowerCycle(usb_phys_port):
-
     usb_location = ".".join(usb_phys_port.split(".")[:-1])
     usb_port = usb_phys_port.split(".")[-1]
     print(" ".join(["uhubctl", "-a", "off", "-l", usb_location, "-p", usb_port]))
     proc_off = subprocess.run(
         ["uhubctl", "-a", "off", "-l", usb_location, "-p", usb_port],
         stdout=subprocess.DEVNULL,
         stderr=subprocess.DEVNULL,
@@ -110,15 +107,15 @@
     )
 
     args = parser.parse_args()
 
     result = usbPowerCycle(args.usb_physical_port)
 
     if True:
-        print_color(TermColors.GREEN, "Success")
+        print("Success")
     else:
-        error("USB power cycle failed")
+        sys.exit("USB power cycle failed")
 
 
 if __name__ == "__main__":
     main()
     # usbPowerCycle("1-1.1")
```

