# Comparing `tmp/nucleus_driver-1.4.7.tar.gz` & `tmp/nucleus_driver-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nucleus_driver-1.4.7.tar", last modified: Fri Apr 14 09:59:03 2023, max compression
+gzip compressed data, was "nucleus_driver-1.5.0.tar", last modified: Fri Jun  9 06:15:00 2023, max compression
```

## Comparing `nucleus_driver-1.4.7.tar` & `nucleus_driver-1.5.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-14 09:59:03.559152 nucleus_driver-1.4.7/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1063 2023-03-27 14:20:11.000000 nucleus_driver-1.4.7/LICENSE.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)     9458 2023-04-14 09:59:03.559152 nucleus_driver-1.4.7/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     8987 2023-03-27 14:20:11.000000 nucleus_driver-1.4.7/README.md
--rw-rw-r--   0 martin    (1000) martin    (1000)      105 2023-03-27 14:20:11.000000 nucleus_driver-1.4.7/pyproject.toml
--rw-rw-r--   0 martin    (1000) martin    (1000)      737 2023-04-14 09:59:03.559152 nucleus_driver-1.4.7/setup.cfg
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-14 09:59:03.559152 nucleus_driver-1.4.7/src/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-14 09:59:03.559152 nucleus_driver-1.4.7/src/nucleus_driver/
--rw-rw-r--   0 martin    (1000) martin    (1000)       71 2023-03-27 14:20:11.000000 nucleus_driver-1.4.7/src/nucleus_driver/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2203 2023-03-27 14:20:11.000000 nucleus_driver-1.4.7/src/nucleus_driver/_assert.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    50233 2023-04-14 09:56:26.000000 nucleus_driver-1.4.7/src/nucleus_driver/_commands.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    16923 2023-04-14 09:56:26.000000 nucleus_driver-1.4.7/src/nucleus_driver/_connection.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    24616 2023-03-27 14:20:11.000000 nucleus_driver-1.4.7/src/nucleus_driver/_download.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    16554 2023-03-27 14:20:11.000000 nucleus_driver-1.4.7/src/nucleus_driver/_flash.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     9653 2023-04-14 09:56:26.000000 nucleus_driver-1.4.7/src/nucleus_driver/_logger.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      470 2023-03-27 14:20:11.000000 nucleus_driver-1.4.7/src/nucleus_driver/_messages.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    40241 2023-03-30 13:38:55.000000 nucleus_driver-1.4.7/src/nucleus_driver/_parser.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2523 2023-03-27 14:20:11.000000 nucleus_driver-1.4.7/src/nucleus_driver/_syslog.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    19018 2023-04-14 09:56:26.000000 nucleus_driver-1.4.7/src/nucleus_driver/app.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    11367 2023-04-14 09:56:26.000000 nucleus_driver-1.4.7/src/nucleus_driver/nucleus_driver.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-14 09:59:03.559152 nucleus_driver-1.4.7/src/nucleus_driver.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)     9458 2023-04-14 09:59:03.000000 nucleus_driver-1.4.7/src/nucleus_driver.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      673 2023-04-14 09:59:03.000000 nucleus_driver-1.4.7/src/nucleus_driver.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-04-14 09:59:03.000000 nucleus_driver-1.4.7/src/nucleus_driver.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       77 2023-04-14 09:59:03.000000 nucleus_driver-1.4.7/src/nucleus_driver.egg-info/entry_points.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       26 2023-04-14 09:59:03.000000 nucleus_driver-1.4.7/src/nucleus_driver.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       15 2023-04-14 09:59:03.000000 nucleus_driver-1.4.7/src/nucleus_driver.egg-info/top_level.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-09 06:15:00.310002 nucleus_driver-1.5.0/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1063 2023-03-27 14:20:11.000000 nucleus_driver-1.5.0/LICENSE.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)     9458 2023-06-09 06:15:00.310002 nucleus_driver-1.5.0/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     8987 2023-03-27 14:20:11.000000 nucleus_driver-1.5.0/README.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)      105 2023-03-27 14:20:11.000000 nucleus_driver-1.5.0/pyproject.toml
+-rw-rw-r--   0 martin    (1000) martin    (1000)      737 2023-06-09 06:15:00.310002 nucleus_driver-1.5.0/setup.cfg
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-09 06:15:00.306002 nucleus_driver-1.5.0/src/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-09 06:15:00.306002 nucleus_driver-1.5.0/src/nucleus_driver/
+-rw-rw-r--   0 martin    (1000) martin    (1000)       71 2023-03-27 14:20:11.000000 nucleus_driver-1.5.0/src/nucleus_driver/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2203 2023-03-27 14:20:11.000000 nucleus_driver-1.5.0/src/nucleus_driver/_assert.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    50233 2023-06-01 06:58:05.000000 nucleus_driver-1.5.0/src/nucleus_driver/_commands.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    16919 2023-06-08 13:16:41.000000 nucleus_driver-1.5.0/src/nucleus_driver/_connection.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    25406 2023-06-08 13:16:41.000000 nucleus_driver-1.5.0/src/nucleus_driver/_download.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    16554 2023-03-27 14:20:11.000000 nucleus_driver-1.5.0/src/nucleus_driver/_flash.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    10853 2023-06-08 13:16:41.000000 nucleus_driver-1.5.0/src/nucleus_driver/_logger.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      470 2023-03-27 14:20:11.000000 nucleus_driver-1.5.0/src/nucleus_driver/_messages.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    39751 2023-06-08 13:16:41.000000 nucleus_driver-1.5.0/src/nucleus_driver/_parser.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2523 2023-03-27 14:20:11.000000 nucleus_driver-1.5.0/src/nucleus_driver/_syslog.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    19018 2023-04-14 09:56:26.000000 nucleus_driver-1.5.0/src/nucleus_driver/app.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    11259 2023-06-08 13:16:41.000000 nucleus_driver-1.5.0/src/nucleus_driver/nucleus_driver.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-09 06:15:00.310002 nucleus_driver-1.5.0/src/nucleus_driver.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     9458 2023-06-09 06:15:00.000000 nucleus_driver-1.5.0/src/nucleus_driver.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      673 2023-06-09 06:15:00.000000 nucleus_driver-1.5.0/src/nucleus_driver.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-06-09 06:15:00.000000 nucleus_driver-1.5.0/src/nucleus_driver.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       77 2023-06-09 06:15:00.000000 nucleus_driver-1.5.0/src/nucleus_driver.egg-info/entry_points.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       26 2023-06-09 06:15:00.000000 nucleus_driver-1.5.0/src/nucleus_driver.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       15 2023-06-09 06:15:00.000000 nucleus_driver-1.5.0/src/nucleus_driver.egg-info/top_level.txt
```

### Comparing `nucleus_driver-1.4.7/LICENSE.txt` & `nucleus_driver-1.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.4.7/PKG-INFO` & `nucleus_driver-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nucleus_driver
-Version: 1.4.7
+Version: 1.5.0
 Summary: driver for the Nortek Nucleus
 Home-page: https://github.com/nortekgroup/nucleus_driver
 Author: Martin Bergene Johansen
 Author-email: martin.johansen@nortekgroup.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nucleus_driver-1.4.7/README.md` & `nucleus_driver-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.4.7/setup.cfg` & `nucleus_driver-1.5.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nucleus_driver
-version = 1.4.7
+version = 1.5.0
 author = Martin Bergene Johansen
 author_email = martin.johansen@nortekgroup.com
 description = driver for the Nortek Nucleus
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/nortekgroup/nucleus_driver
 classifiers =
```

### Comparing `nucleus_driver-1.4.7/src/nucleus_driver/_assert.py` & `nucleus_driver-1.5.0/src/nucleus_driver/_assert.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.4.7/src/nucleus_driver/_commands.py` & `nucleus_driver-1.5.0/src/nucleus_driver/_commands.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.4.7/src/nucleus_driver/_connection.py` & `nucleus_driver-1.5.0/src/nucleus_driver/_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -266,15 +266,15 @@
         if self.get_connection_type() == 'serial':
             self._connected = _connect_serial()
 
         if self.get_connection_type() == 'tcp':
             self._connected = _connect_tcp()
 
         if not self.get_connection_status():
-            self.messages.write_warning('Failed to set current time on Nucleus device')
+            self.messages.write_warning('Failed to establish connection to device')
             return False
 
         if get_device_info:
             if not self.set_clockstring():
                 get_device_info = False
 
         if get_device_info:
```

### Comparing `nucleus_driver-1.4.7/src/nucleus_driver/_download.py` & `nucleus_driver-1.5.0/src/nucleus_driver/_download.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
         self._path = str(Path.cwd()) + '/download'
 
         self.dvl_download_statistics = dict()
         self.dvl_download_statistics['successful bytes'] = 0
         self.dvl_download_statistics['failed bytes'] = 0
 
-        self.PACKET_LENGTH = 1024 * 10
+        self.PACKET_LENGTH = 1024 * 1024
 
     @staticmethod
     def _handle_crc(dvl_data: bytes):
 
         crc_fail_data = b''
 
         while True:
@@ -160,52 +160,58 @@
         download_parameters['sa'] = None
         download_parameters['end'] = None
         if not _get_download_parameters():
             return False, dict()
 
         return True, download_parameters
 
-    def download_data(self, fid, src, sa, length) -> (bool, bytes):
-
+    def download_data(self, fid, src, sa, length, timeout=3) -> (bool, bytes):
+        
         expected_data_length = len(str(length)) + 2 + length + 2 + 10 + 4  # length of _len number + length of \r\n + length of _len + length of \r\n + length of crc and \r\n + length of OK\r\n
 
         command = b'DOWNLOAD,FID=' + str(fid).encode() + b',SRC=' + str(src).encode() + b',SA=' + str(sa).encode() + b',LEN=' + str(length).encode() + b',CRC=1\r\n'
         self.connection.write(command)
-        data = self.connection.read(size=expected_data_length, timeout=3)
+        data = self.connection.read(size=expected_data_length, timeout=timeout)
         self.commands._check_reply(data=data, terminator=b'OK\r\n', command=command)
 
         if len(data) != expected_data_length:
-            self.messages.write_warning('received data from download reply is incorrect length')
+            self.messages.write_warning(f'received data from download reply is incorrect length: {len(data)} / {expected_data_length}')
+            self.connection.reset_buffers()
             return False, b''
 
         length_reply = data[:len(str(length)) + 2]
         data_reply = data[len(str(length)) + 2:-14]
         crc_reply = data[-14:-4]
         ok_reply = data[-4:]
 
         if length_reply[-2:] != b'\r\n':
-            self.messages.write_warning('unexpected format of the length reply from download command')
+            self.messages.write_warning(f"unexpected format of the length reply from download command. Reply should end with b'\r\n': {length_reply}")
+            self.connection.reset_buffers()
             return False, b''
 
         if data_reply[-2:] != b'\r\n':
-            self.messages.write_warning('unexpected format of the data reply from download command')
+            self.messages.write_warning(f"unexpected format of the data reply from download command. Reply should end with b'\r\n': {data_reply}")
+            self.connection.reset_buffers()
             return False, b''
 
         if crc_reply[-2:] != b'\r\n':
-            self.messages.write_warning('unexpected format of the crc reply from download command')
+            self.messages.write_warning(f"unexpected format of the crc reply from download command. Reply should end with b'\r\n': {crc_reply}")
+            self.connection.reset_buffers()
             return False, b''
 
         if ok_reply[-2:] != b'\r\n':
-            self.messages.write_warning('unexpected format of the ok reply from download command')
+            self.messages.write_warning(f"unexpected format of the ok reply from download command. Reply should end with b'\r\n': {ok_reply}")
+            self.connection.reset_buffers()
             return False, b''
 
         try:
             crc = int(crc_reply[:-2].decode(), 16)
         except ValueError:
-            self.messages.write_warning('Unable to convert received crc value to integer')
+            self.messages.write_warning(f'Unable to convert received crc value to integer. crc value: {crc_reply}')
+            self.connection.reset_buffers()
             return False, b''
 
         if crc32(data_reply[:-2]) == crc:
             return True, data_reply[:-2]
         else:
             return False, data_reply[:-2]
 
@@ -373,15 +379,18 @@
 
             return True
 
         def _download_data() -> (bool, bytes):
 
             failed_attempt = False
             for attempt in range(1, 11):
-                status, package = self.download_data(fid=download_parameters['fid'], src=1, sa=index, length=min(download_parameters['end'] - index, self.PACKET_LENGTH))
+                
+                timeout = min(2 + attempt, 10)  # First iteration is 3s, 3 last iterations are 10s
+
+                status, package = self.download_data(fid=download_parameters['fid'], src=1, sa=index, length=min(download_parameters['end'] - index, self.PACKET_LENGTH), timeout=timeout)
 
                 if status:
                     if failed_attempt:
                         self.messages.write_message('successfully received packet at index {}'.format(index))
                     break
                 else:
                     failed_attempt = True
@@ -513,15 +522,18 @@
 
             return True
 
         def _download_data() -> (bool, bytes):
 
             failed_attempt = False
             for attempt in range(1, 11):
-                status, package = self.download_data(fid=download_parameters['fid'], src=0, sa=index, length=min(download_parameters['end'] - index, self.PACKET_LENGTH))
+
+                timeout = min(2 + attempt, 10)  # First iteration is 3s, 3 last iterations are 10s
+
+                status, package = self.download_data(fid=download_parameters['fid'], src=0, sa=index, length=min(download_parameters['end'] - index, self.PACKET_LENGTH), timeout=timeout)
 
                 if status:
                     if failed_attempt:
                         self.messages.write_message('successfully received packet at index {}'.format(index))
                     break
                 else:
                     failed_attempt = True
```

### Comparing `nucleus_driver-1.4.7/src/nucleus_driver/_flash.py` & `nucleus_driver-1.5.0/src/nucleus_driver/_flash.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.4.7/src/nucleus_driver/_logger.py` & `nucleus_driver-1.5.0/src/nucleus_driver/_logger.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,25 +11,29 @@
     def __init__(self, **kwargs):
 
         self.messages = kwargs.get('messages')
         self.connection = kwargs.get('connection')
         self.commands = None
 
         self._logging = False
+        self._logging_folder = None
+        self._current_profile_logging = False
 
         self._writing_packet = False
         self._writing_ascii = False
         self._writing_condition = False
 
         self._path = str(Path.cwd()) + '/logs'
         self.packet_file = None
+        self.current_profile_file = None
         self.ascii_file = None
         self.condition_file = None
 
         self.packet_writer = None
+        self.current_profile_writer = None
         self.ascii_writer = None
         self.condition_writer = None
 
         self.cp_nc = None
 
     def _get_field_names_packet(self):
         """function to return the fieldnames for the UNS logging"""
@@ -81,28 +85,28 @@
                       'timeVelBeam1', 'timeVelBeam2', 'timeVelBeam3',
                       'velocityX', 'velocityY', 'velocityZ', 'fomX', 'fomY', 'fomZ',
                       'dtXYZ', 'timeVelXYZ']
 
         alti_fields = ['status.altimeterDistanceValid', 'status.altimeterQualityValid', 'status.pressureValid', 'status.temperatureValid',
                        'serialNumber', 'soundSpeed', 'temperature', 'pressure',
                        'altimeterDistance', 'altimeterQuality']
-
+        '''
         cp_fields = ['serialNumber', 'soundVelocity', 'temperature', 'pressure',
                      'cellSize', 'blanking', 'numberOfCells', 'ambiguityVelocity']
 
         if self.cp_nc is not None:
             for index in range(self.cp_nc * 3):
                 cp_fields.append('velocityData_{}'.format(index))
 
             for index in range(self.cp_nc * 3):
                 cp_fields.append('amplitudeData_{}'.format(index))
 
             for index in range(self.cp_nc * 3):
                 cp_fields.append('correlationData_{}'.format(index))
-
+        '''
         fc_fields = ['status.pointsUsedInEstimation',
                      'hardIron.x', 'hardIron.y', 'hardIron.z',
                      'sAxis_0', 'sAxis_1', 'sAxis_2',
                      'sAxis_3', 'sAxis_4', 'sAxis_5',
                      'sAxis_6', 'sAxis_7', 'sAxis_8',
                      'newPoint.x', 'newPoint.y', 'newPoint.z',
                      'fomFieldCalibration', 'coverage']
@@ -115,15 +119,15 @@
                        is_valid_field,  # TODO: This is a temporary fix where this value needs to be in the log file, but nothing is logged to this column
                        ahrs_fields,
                        ins_fields,
                        imu_fields,
                        mag_fields,
                        dvl_fields,
                        alti_fields,
-                       cp_fields,
+                       #cp_fields,
                        fc_fields,
                        string_fields]
 
         field_names = list()
         for fields in data_fields:
             for field in fields:
                 if field not in field_names:
@@ -145,64 +149,86 @@
 
         return field_names
 
     def get_logging_status(self):
 
         return self._logging
 
-    def get_cp_nc(self):
+    def get_current_profile_logging_status(self):
 
-        reply = self.commands.get_cur_prof(profile_range=True, cs=True, bd=True, ds=True)
+        return self._current_profile_logging
+    
+    def set_path(self, path: str):
 
-        if len(reply) != 2:
-            self.messages.write_warning('Unable to obtain current profile configuration')
+        self._path = path.rstrip('/')
 
-        else:
-            try:
-                cp_data = reply[0].split(b',')
-                cp_range = float(cp_data[0].decode())
-                cp_cs = float(cp_data[1].decode())
-                cp_bd = float(cp_data[2].decode())
-                cp_ds = cp_data[3].rstrip(b'\r\n').decode()
-
-                if cp_ds == '"OFF"':
-                    self.cp_nc = 0
-
-                else:
-                    nc = ceil((cp_range - cp_bd) / cp_cs)
-                    if nc > 0:
-                        self.cp_nc = nc
-                    else:
-                        self.cp_nc = None
+    def open_current_profile_writer(self, number_of_cells: int) -> bool:
+        
+        def _get_field_names():
 
-            except Exception as e:
-                self.messages.write_warning('Error occured when trying to extract current profile data: {}'.format(e))
+            header_fields = ['sizeHeader', 'id', 'family', 'sizeData', 'size', 'dataCheckSum', 'headerCheckSum']
 
-    def set_path(self, path: str):
+            common_fields = ['version', 'offsetOfData', 'flags.posixTime', 'timeStamp', 'microSeconds']
 
-        self._path = path.rstrip('/')
+            driver_fields = ['timestampPython']
+
+            cp_fields = ['serialNumber', 'soundVelocity', 'temperature', 'pressure',
+                        'cellSize', 'blanking', 'numberOfCells', 'ambiguityVelocity']
+
+            for index in range(number_of_cells * 3):
+                cp_fields.append('velocityData_{}'.format(index))
+
+            for index in range(number_of_cells * 3):
+                cp_fields.append('amplitudeData_{}'.format(index))
+
+            for index in range(number_of_cells * 3):
+                cp_fields.append('correlationData_{}'.format(index))
+
+            data_fields = [header_fields,
+                           common_fields,
+                           driver_fields,
+                           cp_fields]
+
+            field_names = list()
+            for fields in data_fields:
+                for field in fields:
+                    if field not in field_names:
+                        field_names.append(field)
+
+            return field_names
+
+        if self._logging_folder is None:
+            return False
+        
+        self.current_profile_file = open(self._logging_folder + '/current_profile_log.csv', 'w', newline='')
+
+        self.current_profile_writer = csv.DictWriter(self.current_profile_file, fieldnames=_get_field_names())
+        
+        self.current_profile_writer.writeheader()
+
+        self._current_profile_logging = True
+
+        return True
 
     def start(self, _converting=False) -> str:
 
         folder = self._path + '/' + datetime.now().strftime('%y%m%d_%H%M%S')
+        self._logging_folder = folder
 
         Path(folder).mkdir(parents=True, exist_ok=True)
 
         if not _converting:
             self.messages.write_message('Logging started. Path: {}'.format(folder))
         else:
             self.messages.write_message('Converting started. Path: {}'.format(folder))
 
         self.packet_file = open(folder + '/nucleus_log.csv', 'w', newline='')
         self.condition_file = open(folder + '/condition_log.csv', 'w', newline='')
         self.ascii_file = open(folder + '/ascii_log.csv', 'w', newline='')
 
-        #if self.connection.get_connection_status():
-        #    self.connection.get_info()
-
         if self.connection.get_all is not None and _converting is False:
             with open(folder + '/get_all.txt', 'w') as file:
                 file.writelines(self.connection.get_all)
 
         self.packet_writer = csv.DictWriter(self.packet_file, fieldnames=self._get_field_names_packet())
         self.condition_writer = csv.DictWriter(self.condition_file, fieldnames=self._get_field_names_condition())
         self.ascii_writer = csv.DictWriter(self.ascii_file, fieldnames=self._get_field_names_ascii())
@@ -214,24 +240,29 @@
         self._logging = True
 
         return folder
 
     def stop(self):
 
         self._logging = False
+        self._logging_folder = None
+        self._current_profile_logging = False
 
         # give the writers up to 0.1 sec to complete writing
-        for i in range(10):
+        for _ in range(10):
 
             if not self._writing_packet and not self._writing_ascii and not self._writing_condition:
                 break
 
             time.sleep(0.01)
 
         if isinstance(self.packet_file, io.TextIOWrapper):
             self.packet_file.close()
 
+        if isinstance(self.current_profile_file, io.TextIOWrapper):
+            self.current_profile_file.close()
+
         if isinstance(self.condition_file, io.TextIOWrapper):
             self.condition_file.close()
 
         if isinstance(self.ascii_file, io.TextIOWrapper):
             self.ascii_file.close()
```

### Comparing `nucleus_driver-1.4.7/src/nucleus_driver/_parser.py` & `nucleus_driver-1.5.0/src/nucleus_driver/_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -114,16 +114,22 @@
 
             self.packet_queue.put_nowait(packet)
 
         if self.logger._logging is True:
 
             self.logger._writing_packet = True
 
+            if packet['id'] == self.ID_CURRENT_PROFILE and not self.logger.get_current_profile_logging_status():
+                self.logger.open_current_profile_writer(number_of_cells=int(packet['numberOfCells']))
+
             try:
-                self.logger.packet_writer.writerow(packet)
+                if packet['id'] == self.ID_CURRENT_PROFILE:
+                    self.logger.current_profile_writer.writerow(packet)
+                else:
+                    self.logger.packet_writer.writerow(packet)
             except ValueError as exception:
                 self.messages.write_warning('Failed to write package to csv file: {}'.format(exception))
 
             self.logger._writing_packet = False
 
     def read_packet(self, timeout=None):
 
@@ -159,15 +165,15 @@
             ascii_packet = {'timestamp_python': datetime.now().timestamp(),
                             'message': ascii_message}
 
             self.logger._writing_ascii = True
 
             try:
                 self.logger.ascii_writer.writerow(ascii_packet)
-            except ValueError as exception:
+            except Exception as exception:
                 self.messages.write_warning('Failed to write ascii message to csv file: {}'.format(exception))
 
             self.logger._writing_ascii = False
 
     def read_ascii(self, timeout=None):
 
         packet = None
@@ -310,58 +316,46 @@
 
             if len(binary_packet) >= header_data['sizeHeader'] + header_data['sizeData']:
                 status = True
 
             return status
 
         def get_header_data():
-
-            header = {'sizeHeader': None,
-                      'id': None,
-                      'family': None,
-                      'sizeData': None,
-                      'size': None,
-                      'dataCheckSum': None,
-                      'headerCheckSum': None}
+            
+            header = None
 
             try:
                 header = {'sizeHeader': unpack('<B', binary_packet[1:2])[0],
                           'id': unpack('<B', binary_packet[2:3])[0],
                           'family': unpack('<B', binary_packet[3:4])[0],
                           'sizeData': unpack('<H', binary_packet[4:6])[0],
                           'size': unpack('<B', binary_packet[1:2])[0] + unpack('<H', binary_packet[4:6])[0],
                           'dataCheckSum': unpack('<H', binary_packet[6:8])[0],
                           'headerCheckSum': unpack('<H', binary_packet[8:10])[0]}
 
             except struct_error:
-                self.messages.write_warning('Failed to unpack header data')
-                self.messages.write_warning(data)
+                self.messages.write_warning(f'Failed to unpack header data: {binary_packet}')
 
             return header
 
         def get_common_data():
 
-            common = {'version': None,
-                      'offsetOfData': None,
-                      'flags.posixTime': None,
-                      'timeStamp': None,
-                      'microSeconds': None}
+            common = None
 
             try:
                 status = unpack('<B', data[2:3])[0]
 
                 common = {'version': unpack('<B', data[0:1])[0],
                           'offsetOfData': unpack('<B', data[1:2])[0],
                           'flags.posixTime': _get_status(status_bits=status, bit=0),
                           'timeStamp': unpack('<I', data[4:8])[0],
                           'microSeconds': unpack('<I', data[8:12])[0]}
 
             except struct_error:
-                self.messages.write_warning('Failed to unpack common data')
-                self.messages.write_warning(data)
+                self.messages.write_warning(f'Failed to unpack common data: {data}')
 
             return common
 
         def get_sensor_data():
 
             sensor = None
 
@@ -556,31 +550,28 @@
                                   'blanking': unpack('<f', data[40:44])[0],
                                   'numberOfCells': unpack('<H', data[44:46])[0],
                                   'ambiguityVelocity': unpack('<H', data[46:48])[0]}
 
                         velocity_data_format = '<' + ''.ljust(3 * sensor['numberOfCells'], 'H')
                         velocity_data_offset = common_data['offsetOfData']
                         velocity_data_size = 2 * 3 * sensor['numberOfCells']
-                        # sensor['velocityData'] = unpack(velocity_data_format, data[velocity_data_offset: velocity_data_offset + velocity_data_size])[:velocity_data_size]
                         velocity_data = unpack(velocity_data_format, data[velocity_data_offset: velocity_data_offset + velocity_data_size])[:velocity_data_size]
                         for index, velocity_cell in enumerate(velocity_data):
                             sensor['velocityData_{}'.format(index)] = velocity_cell
 
                         amplitude_data_format = '<' + ''.ljust(3 * sensor['numberOfCells'], 'B')
                         amplitude_data_offset = common_data['offsetOfData'] + 6 * sensor['numberOfCells']
                         amplitude_data_size = 1 * 3 * sensor['numberOfCells']
-                        # sensor['amplitudeData'] = unpack(amplitude_data_format, data[amplitude_data_offset: amplitude_data_offset + amplitude_data_size])[:amplitude_data_size]
                         amplitude_data = unpack(amplitude_data_format, data[amplitude_data_offset: amplitude_data_offset + amplitude_data_size])[:amplitude_data_size]
                         for index, amplitude_cell in enumerate(amplitude_data):
                             sensor['amplitudeData_{}'.format(index)] = amplitude_cell
 
                         correlation_data_format = '<' + ''.ljust(3 * sensor['numberOfCells'], 'B')
                         correlation_data_offset = common_data['offsetOfData'] + 9 * sensor['numberOfCells']
                         correlation_data_size = 1 * 3 * sensor['numberOfCells']
-                        # sensor['correlationData'] = unpack(correlation_data_format, data[correlation_data_offset: correlation_data_offset + correlation_data_size])[:correlation_data_size]
                         correlation_data = unpack(correlation_data_format, data[correlation_data_offset: correlation_data_offset + correlation_data_size])[:correlation_data_size]
                         for index, correlation_cell in enumerate(correlation_data):
                             sensor['correlationData_{}'.format(index)] = correlation_cell
 
                     if header_data['id'] == self.ID_FIELD_CALIBRATION:
                         status = unpack('<I', data[12:16])[0]
 
@@ -618,18 +609,19 @@
 
             return sensor
 
         if not check_header_size():
             self.messages.write_exception('Packet is smaller than specified header length. Extraction aborted')
             return header_checksum, data_checksum, packet
 
-
-
         header_data = get_header_data()
 
+        if header_data is None:
+            return header_checksum, data_checksum, packet
+
         if self.checksum(binary_packet[:header_data['sizeHeader'] - 2]) == header_data['headerCheckSum']:
             header_checksum = True
         else:
             self.messages.write_exception('Header did not pass checksum. Extraction aborted')
             return header_checksum, data_checksum, packet
 
         packet.update(header_data)
@@ -644,14 +636,18 @@
             self.messages.write_exception('Packet did not pass checksum. Extraction aborted')
             return header_checksum, data_checksum, packet
 
         data = binary_packet[header_data['sizeHeader']:header_data['sizeHeader'] + header_data['sizeData']]
 
         if header_data['id'] != self.ID_ASCII:
             common_data = get_common_data()
+
+            if common_data is None:
+                return header_checksum, False, packet
+
             packet.update(common_data)
 
         packet['timestampPython'] = datetime.now().timestamp()
 
         sensor_data = get_sensor_data()
 
         if sensor_data is None:
```

### Comparing `nucleus_driver-1.4.7/src/nucleus_driver/_syslog.py` & `nucleus_driver-1.5.0/src/nucleus_driver/_syslog.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.4.7/src/nucleus_driver/app.py` & `nucleus_driver-1.5.0/src/nucleus_driver/app.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.4.7/src/nucleus_driver/nucleus_driver.py` & `nucleus_driver-1.5.0/src/nucleus_driver/nucleus_driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,14 @@
             return b''
 
         if not self.parser.thread_running:
             self.parser.start()
 
         time.sleep(0.1)
 
-        response = self.logger.get_cp_nc()
         response = self.commands._start()
 
         return response
 
     def start_measurement_and_logging(self):
         
         if not self.connection.get_connection_status():
@@ -160,15 +159,14 @@
             return b''
 
         if not self.parser.thread_running:
             self.parser.start()
 
         time.sleep(0.1)
 
-        self.logger.get_cp_nc()
         self.connection.get_info()
 
         response = self.commands._start()
 
         if b'OK\r\n' not in response:
             self.messages.write_warning('Failed to start Nucleus')
             return response
@@ -197,18 +195,16 @@
         if not self.connection.get_connection_status():
             self.messages.write_warning('Nucleus not connected')
             return b''
 
         if not self.parser.thread_running:
             self.parser.start()
 
-
         time.sleep(0.1)
 
-        self.logger.get_cp_nc()
         self.connection.get_info()
 
         response = self.commands._fieldcal()
 
         if b'OK\r\n' not in response:
             self.messages.write_warning('Failed to start Nucleus')
             return response
```

### Comparing `nucleus_driver-1.4.7/src/nucleus_driver.egg-info/PKG-INFO` & `nucleus_driver-1.5.0/src/nucleus_driver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nucleus-driver
-Version: 1.4.7
+Version: 1.5.0
 Summary: driver for the Nortek Nucleus
 Home-page: https://github.com/nortekgroup/nucleus_driver
 Author: Martin Bergene Johansen
 Author-email: martin.johansen@nortekgroup.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nucleus_driver-1.4.7/src/nucleus_driver.egg-info/SOURCES.txt` & `nucleus_driver-1.5.0/src/nucleus_driver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

