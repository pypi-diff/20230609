# Comparing `tmp/captif_cpx_config-0.4.tar.gz` & `tmp/captif_cpx_config-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "captif_cpx_config-0.4.tar", max compression
+gzip compressed data, was "captif_cpx_config-0.5.tar", max compression
```

## Comparing `captif_cpx_config-0.4.tar` & `captif_cpx_config-0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1084 2023-06-08 04:28:05.170526 captif_cpx_config-0.4/LICENSE
--rw-r--r--   0        0        0       19 2023-06-08 04:28:05.170526 captif_cpx_config-0.4/README.md
--rw-r--r--   0        0        0       44 2023-06-08 04:28:05.170526 captif_cpx_config-0.4/captif_cpx_config/__init__.py
--rw-r--r--   0        0        0     4168 2023-06-08 04:28:05.170526 captif_cpx_config-0.4/captif_cpx_config/metadata.py
--rw-r--r--   0        0        0      521 2023-06-08 04:28:05.170526 captif_cpx_config-0.4/pyproject.toml
--rw-r--r--   0        0        0      519 1970-01-01 00:00:00.000000 captif_cpx_config-0.4/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-06-09 00:45:40.220634 captif_cpx_config-0.5/LICENSE
+-rw-r--r--   0        0        0       19 2023-06-09 00:45:40.220634 captif_cpx_config-0.5/README.md
+-rw-r--r--   0        0        0       44 2023-06-09 00:45:40.220634 captif_cpx_config-0.5/captif_cpx_config/__init__.py
+-rw-r--r--   0        0        0     4112 2023-06-09 00:45:40.220634 captif_cpx_config-0.5/captif_cpx_config/metadata.py
+-rw-r--r--   0        0        0      521 2023-06-09 00:45:40.220634 captif_cpx_config-0.5/pyproject.toml
+-rw-r--r--   0        0        0      519 1970-01-01 00:00:00.000000 captif_cpx_config-0.5/PKG-INFO
```

### Comparing `captif_cpx_config-0.4/LICENSE` & `captif_cpx_config-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `captif_cpx_config-0.4/captif_cpx_config/metadata.py` & `captif_cpx_config-0.5/captif_cpx_config/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,39 +25,68 @@
     )
 
 
 class AccelerometerDetails(BaseModel):
     accelerometer_position: Literal["chassis", "axle"] = Field(
         description="accelerometer position ('chassis' or 'axle')",
     )
-    accelerometer_serial_number: str = Field(
-        description="accelerometer serial number",
-    ),
+    accelerometer_serial_number: str = (
+        Field(
+            description="accelerometer serial number",
+        ),
+    )
     accelerometer_sensitivity_mv_g: condecimal(decimal_places=2) = Field(
         description="accelerometer sensitivity in mV/g",
     )
     wav_file_channel_number: int = Field(
         description=(
             "channel number in the wav file corresponding to the "
             "accelerometer. The channels number uses zero-based indexing."
         ),
     )
 
 
-
 class DeviceCorrections(BaseModel):
     frequency_hz: list[condecimal(decimal_places=1)] = Field(
         description="list third-octave band centre frequencies in Hz",
     )
     correction_db: list[condecimal(decimal_places=2)] = Field(
         description="list of device corrections in dB",
     )
 
 
-class MeasurementDetails(BaseModel):
+class WheelBayDetails(BaseModel):
+    wheel_bay_name: Literal["left", "right"] = Field(
+        description="wheel bay name ('left' or 'right')",
+    )
+    wheel_bay_configuration_details: str = Field(
+        description="description of the wheel bay configuration",
+    )
+    wheel_bay_calibration_date: date_ = Field(
+        description="wheel bay / device correction calibration date"
+    )
+    tyre: str = Field(
+        description="tyre name/type (e.g. 'P1', 'H1', etc.)",
+    )
+    tyre_purchase_date: date_ = Field(
+        description="tyre purchase date",
+    )
+    hardness: condecimal(decimal_places=1) = Field(
+        description="tyre hardness in Shore A",
+    )
+    hardness_date: date_ = Field(
+        description="tyre hardness measurement date",
+    )
+
+    microphone_details: list["MicrophoneDetails"]
+    accelerometer_details: list["AccelerometerDetails"] = []
+    device_corrections: "DeviceCorrections"
+
+
+class Metadata(BaseModel):
     date: date_ = Field(
         description="date of measurement",
     )
     location: str = Field(
         description="location of measurement",
     )
     purpose: str = Field(
@@ -84,46 +113,15 @@
             "to convert the data back into volts."
         ),
     )
     notes: str = Field(
         description="any additional notes",
     )
 
-
-class WheelBayDetails(BaseModel):
-    wheel_bay_name: Literal["left", "right"] = Field(
-        description="wheel bay name ('left' or 'right')",
-    )
-    wheel_bay_configuration_details: str = Field(
-        description="description of the wheel bay configuration",
-    )
-    wheel_bay_calibration_date: date_ = Field(
-        description="wheel bay / device correction calibration date"
-    )
-    tyre: str = Field(
-        description="tyre name/type (e.g. 'P1', 'H1', etc.)",
-    )
-    tyre_purchase_date: date_ = Field(
-        description="tyre purchase date",
-    )
-    hardness: condecimal(decimal_places=1) = Field(
-        description="tyre hardness in Shore A",
-    )
-    hardness_date: date_ = Field(
-        description="tyre hardness measurement date",
-    )
-
-    microphone_details: list["MicrophoneDetails"]
-    accelerometer_details: list["AccelerometerDetails"] = []
-    device_corrections: "DeviceCorrections"
-
-
-class Metadata(BaseModel):
-    measurement_details: "MeasurementDetails"
-    wheel_bay_details: list["WheelBayDetails"]
+    wheel_bay_details: list["WheelBayDetails"] = []
 
     def write(self, path: str):
         with open(path, "w") as f:
             f.write(self.json(indent=4))
 
     @staticmethod
     def read(path: str):
```

### Comparing `captif_cpx_config-0.4/pyproject.toml` & `captif_cpx_config-0.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "captif-cpx-config"
-version = "0.4"
+version = "0.5"
 description = ""
 authors = ["John Bull <john.bull@nzta.govt.nz>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "captif_cpx_config"}]
 
 [tool.poetry.dependencies]
```

### Comparing `captif_cpx_config-0.4/PKG-INFO` & `captif_cpx_config-0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: captif-cpx-config
-Version: 0.4
+Version: 0.5
 Summary: 
 License: MIT
 Author: John Bull
 Author-email: john.bull@nzta.govt.nz
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

