# Comparing `tmp/ppk2-api-0.9.1.tar.gz` & `tmp/ppk2-api-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ppk2-api-0.9.1.tar", last modified: Fri Mar 17 12:29:02 2023, max compression
+gzip compressed data, was "ppk2-api-0.9.2.tar", last modified: Fri Jun  9 13:35:36 2023, max compression
```

## Comparing `ppk2-api-0.9.1.tar` & `ppk2-api-0.9.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 nejc      (1000) nejc      (1000)        0 2023-03-17 12:29:02.989695 ppk2-api-0.9.1/
--rw-r--r--   0 nejc      (1000) nejc      (1000)    18092 2021-01-05 13:27:46.000000 ppk2-api-0.9.1/LICENSE.md
--rw-rw-r--   0 nejc      (1000) nejc      (1000)      372 2023-03-17 12:29:02.989695 ppk2-api-0.9.1/PKG-INFO
--rw-rw-r--   0 nejc      (1000) nejc      (1000)     3650 2021-10-05 08:49:32.000000 ppk2-api-0.9.1/README.md
--rw-rw-r--   0 nejc      (1000) nejc      (1000)       38 2023-03-17 12:29:02.989695 ppk2-api-0.9.1/setup.cfg
--rw-r--r--   0 nejc      (1000) nejc      (1000)     1071 2023-03-17 12:28:03.000000 ppk2-api-0.9.1/setup.py
-drwxrwxr-x   0 nejc      (1000) nejc      (1000)        0 2023-03-17 12:29:02.985695 ppk2-api-0.9.1/src/
--rw-r--r--   0 nejc      (1000) nejc      (1000)     7274 2021-10-05 09:15:26.000000 ppk2-api-0.9.1/src/power_profiler.py
-drwxrwxr-x   0 nejc      (1000) nejc      (1000)        0 2023-03-17 12:29:02.989695 ppk2-api-0.9.1/src/ppk2_api/
--rw-r--r--   0 nejc      (1000) nejc      (1000)        0 2021-05-07 08:48:48.000000 ppk2-api-0.9.1/src/ppk2_api/__init__.py
--rw-rw-r--   0 nejc      (1000) nejc      (1000)    17733 2023-03-17 12:25:04.000000 ppk2-api-0.9.1/src/ppk2_api/ppk2_api.py
-drwxrwxr-x   0 nejc      (1000) nejc      (1000)        0 2023-03-17 12:29:02.989695 ppk2-api-0.9.1/src/ppk2_api.egg-info/
--rw-r--r--   0 nejc      (1000) nejc      (1000)      372 2023-03-17 12:29:02.000000 ppk2-api-0.9.1/src/ppk2_api.egg-info/PKG-INFO
--rw-r--r--   0 nejc      (1000) nejc      (1000)      280 2023-03-17 12:29:02.000000 ppk2-api-0.9.1/src/ppk2_api.egg-info/SOURCES.txt
--rw-r--r--   0 nejc      (1000) nejc      (1000)        1 2023-03-17 12:29:02.000000 ppk2-api-0.9.1/src/ppk2_api.egg-info/dependency_links.txt
--rw-r--r--   0 nejc      (1000) nejc      (1000)        9 2023-03-17 12:29:02.000000 ppk2-api-0.9.1/src/ppk2_api.egg-info/requires.txt
--rw-r--r--   0 nejc      (1000) nejc      (1000)       24 2023-03-17 12:29:02.000000 ppk2-api-0.9.1/src/ppk2_api.egg-info/top_level.txt
+drwxrwxr-x   0 nejc      (1000) nejc      (1000)        0 2023-06-09 13:35:36.010501 ppk2-api-0.9.2/
+-rw-r--r--   0 nejc      (1000) nejc      (1000)    18092 2021-01-05 13:27:46.000000 ppk2-api-0.9.2/LICENSE.md
+-rw-rw-r--   0 nejc      (1000) nejc      (1000)      372 2023-06-09 13:35:36.010501 ppk2-api-0.9.2/PKG-INFO
+-rw-rw-r--   0 nejc      (1000) nejc      (1000)     3650 2021-10-05 08:49:32.000000 ppk2-api-0.9.2/README.md
+-rw-rw-r--   0 nejc      (1000) nejc      (1000)       38 2023-06-09 13:35:36.010501 ppk2-api-0.9.2/setup.cfg
+-rw-rw-r--   0 nejc      (1000) nejc      (1000)     1071 2023-06-09 13:32:38.000000 ppk2-api-0.9.2/setup.py
+drwxrwxr-x   0 nejc      (1000) nejc      (1000)        0 2023-06-09 13:35:36.010501 ppk2-api-0.9.2/src/
+-rw-r--r--   0 nejc      (1000) nejc      (1000)     7274 2021-10-05 09:15:26.000000 ppk2-api-0.9.2/src/power_profiler.py
+drwxrwxr-x   0 nejc      (1000) nejc      (1000)        0 2023-06-09 13:35:36.010501 ppk2-api-0.9.2/src/ppk2_api/
+-rw-r--r--   0 nejc      (1000) nejc      (1000)        0 2021-05-07 08:48:48.000000 ppk2-api-0.9.2/src/ppk2_api/__init__.py
+-rw-rw-r--   0 nejc      (1000) nejc      (1000)    18744 2023-06-09 13:33:05.000000 ppk2-api-0.9.2/src/ppk2_api/ppk2_api.py
+drwxrwxr-x   0 nejc      (1000) nejc      (1000)        0 2023-06-09 13:35:36.010501 ppk2-api-0.9.2/src/ppk2_api.egg-info/
+-rw-r--r--   0 nejc      (1000) nejc      (1000)      372 2023-06-09 13:35:36.000000 ppk2-api-0.9.2/src/ppk2_api.egg-info/PKG-INFO
+-rw-r--r--   0 nejc      (1000) nejc      (1000)      280 2023-06-09 13:35:36.000000 ppk2-api-0.9.2/src/ppk2_api.egg-info/SOURCES.txt
+-rw-r--r--   0 nejc      (1000) nejc      (1000)        1 2023-06-09 13:35:36.000000 ppk2-api-0.9.2/src/ppk2_api.egg-info/dependency_links.txt
+-rw-r--r--   0 nejc      (1000) nejc      (1000)        9 2023-06-09 13:35:36.000000 ppk2-api-0.9.2/src/ppk2_api.egg-info/requires.txt
+-rw-r--r--   0 nejc      (1000) nejc      (1000)       24 2023-06-09 13:35:36.000000 ppk2-api-0.9.2/src/ppk2_api.egg-info/top_level.txt
```

### Comparing `ppk2-api-0.9.1/LICENSE.md` & `ppk2-api-0.9.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ppk2-api-0.9.1/README.md` & `ppk2-api-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `ppk2-api-0.9.1/setup.py` & `ppk2-api-0.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         join(dirname(__file__), *names), encoding=kwargs.get("encoding", "utf8")
     ) as fh:
         return fh.read()
 
 
 setup(
     name="ppk2-api",
-    version="0.9.1",
+    version="0.9.2",
     description="API for Nordic Semiconductor's Power Profiler Kit II (PPK 2).",
     url="https://github.com/IRNAS/ppk2-api-python",
     packages=find_packages("src"),
     package_dir={"": "src"},
     py_modules=[splitext(basename(path))[0] for path in glob("src/*.py")],
     install_requires=[
         "pyserial",
```

### Comparing `ppk2-api-0.9.1/src/power_profiler.py` & `ppk2-api-0.9.2/src/power_profiler.py`

 * *Files identical despite different names*

### Comparing `ppk2-api-0.9.1/src/ppk2_api/ppk2_api.py` & `ppk2-api-0.9.2/src/ppk2_api/ppk2_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -185,34 +185,31 @@
 
     def _generate_mask(self, bits, pos):
         pos = pos
         mask = ((2**bits-1) << pos)
         mask = self._twos_comp(mask)
         return {"mask": mask, "pos": pos}
 
-    def _get_masked_value(self, value, meas):
+    def _get_masked_value(self, value, meas, is_bits=False):
         masked_value = (value & meas["mask"]) >> meas["pos"]
-        if meas["pos"] == 24:
-            if masked_value == 255:
-                masked_value = -1
         return masked_value
 
     def _handle_raw_data(self, adc_value):
         """Convert raw value to analog value"""
         try:
             current_measurement_range = min(self._get_masked_value(
                 adc_value, self.MEAS_RANGE), 4)  # 5 is the number of parameters
             adc_result = self._get_masked_value(adc_value, self.MEAS_ADC) * 4
             bits = self._get_masked_value(adc_value, self.MEAS_LOGIC)
             analog_value = self.get_adc_result(
                 current_measurement_range, adc_result) * 10**6
-            return analog_value
+            return analog_value, bits
         except Exception as e:
             print("Measurement outside of range!")
-            return None
+            return None, None
 
     @staticmethod
     def list_devices():
         import serial.tools.list_ports
         ports = serial.tools.list_ports.comports()
         if os.name == 'nt':
             devices = [port.device for port in ports if port.description.startswith("nRF Connect USB CDC ACM")]
@@ -323,47 +320,74 @@
         self.prev_range = current_range
         return adc
 
     def _digital_to_analog(self, adc_value):
         """Convert discrete value to analog value"""
         return int.from_bytes(adc_value, byteorder="little", signed=False)  # convert reading to analog value
 
+    def digital_channels(self, bits):
+        """
+        Convert raw digital data to digital channels.
+
+        Returns a 2d matrix with 8 rows (one for each channel). Each row contains HIGH and LOW values for the selected channel.
+        """
+
+        # Prepare 2d matrix with 8 rows (one for each channel)
+        digital_channels = [[], [], [], [], [], [], [], []]
+        for sample in bits:
+            digital_channels[0].append((sample & 1) >> 0)
+            digital_channels[1].append((sample & 2) >> 1)
+            digital_channels[2].append((sample & 4) >> 2)
+            digital_channels[3].append((sample & 8) >> 3)
+            digital_channels[4].append((sample & 16) >> 4)
+            digital_channels[5].append((sample & 32) >> 5)
+            digital_channels[6].append((sample & 64) >> 6)
+            digital_channels[7].append((sample & 128) >> 7)
+        return digital_channels
+
     def get_samples(self, buf):
         """
         Returns list of samples read in one sampling period.
         The number of sampled values depends on the delay between serial reads.
         Manipulation of samples is left to the user.
         See example for more info.
         """
 
         sample_size = 4  # one analog value is 4 bytes in size
         offset = self.remainder["len"]
         samples = []
+        raw_digital_output = []
 
         first_reading = (
             self.remainder["sequence"] + buf[0:sample_size-offset])[:4]
         adc_val = self._digital_to_analog(first_reading)
-        measurement = self._handle_raw_data(adc_val)
+        measurement, bits = self._handle_raw_data(adc_val)
         if measurement is not None:
             samples.append(measurement)
+        if bits is not None:
+            raw_digital_output.append(bits)
 
         offset = sample_size - offset
 
         while offset <= len(buf) - sample_size:
             next_val = buf[offset:offset + sample_size]
             offset += sample_size
             adc_val = self._digital_to_analog(next_val)
-            measurement = self._handle_raw_data(adc_val)
+            measurement, bits = self._handle_raw_data(adc_val)
             if measurement is not None:
                 samples.append(measurement)
+            if bits is not None:
+                raw_digital_output.append(bits)
 
         self.remainder["sequence"] = buf[offset:len(buf)]
         self.remainder["len"] = len(buf)-offset
 
-        return samples  # return list of samples, handle those lists in PPK2 API wrapper
+        # return list of samples and raw digital outputs
+        # handle those lists in PPK2 API wrapper
+        return samples, raw_digital_output  
 
 
 class PPK_Fetch(threading.Thread):
     '''
     Background process for polling the data in multi-threaded variant
     '''
     def __init__(self, ppk2, quit_evt, buffer_len_s=10, buffer_chunk_s=0.5):
@@ -397,15 +421,14 @@
             while len(local_buffer) >= self._buffer_chunk:
                 # FIXME: check if lock might be needed when discarding old data
                 self._buffer_q.put(local_buffer[:self._buffer_chunk])
                 while self._buffer_q.qsize()>self._buffer_max_len/self._buffer_chunk:
                     self._buffer_q.get()
                 local_buffer = local_buffer[self._buffer_chunk:]
                 self._last_timestamp = tm_now
-                # print(len(d), len(local_buffer), self._buffer_q.qsize())
 
             # calculate stats
             s += len(d)
             dt = tm_now - t
             if dt >= 0.1:
                 if self.print_stats:
                     print(f"Samples: {s}, delta time: {dt}")
```

