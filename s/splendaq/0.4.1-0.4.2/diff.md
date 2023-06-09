# Comparing `tmp/splendaq-0.4.1.tar.gz` & `tmp/splendaq-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splendaq-0.4.1.tar", last modified: Tue Feb 28 21:10:06 2023, max compression
+gzip compressed data, was "splendaq-0.4.2.tar", last modified: Fri Jun  9 17:18:01 2023, max compression
```

## Comparing `splendaq-0.4.1.tar` & `splendaq-0.4.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 21:10:06.692944 splendaq-0.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 21:10:06.684944 splendaq-0.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 21:10:06.684944 splendaq-0.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-02-28 21:09:56.000000 splendaq-0.4.1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-02-28 21:09:56.000000 splendaq-0.4.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-02-28 21:09:56.000000 splendaq-0.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-02-28 21:09:56.000000 splendaq-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-02-28 21:09:56.000000 splendaq-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-02-28 21:10:06.692944 splendaq-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-02-28 21:09:56.000000 splendaq-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-28 21:09:56.000000 splendaq-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-02-28 21:10:06.692944 splendaq-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-28 21:09:56.000000 splendaq-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 21:10:06.684944 splendaq-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 21:10:06.688944 splendaq-0.4.1/src/splendaq/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-02-28 21:09:56.000000 splendaq-0.4.1/src/splendaq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-02-28 21:09:56.000000 splendaq-0.4.1/src/splendaq/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-28 21:10:06.000000 splendaq-0.4.1/src/splendaq/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 21:10:06.688944 splendaq-0.4.1/src/splendaq/daq/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-02-28 21:09:56.000000 splendaq-0.4.1/src/splendaq/daq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18310 2023-02-28 21:09:56.000000 splendaq-0.4.1/src/splendaq/daq/_log_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    23457 2023-02-28 21:09:56.000000 splendaq-0.4.1/src/splendaq/daq/_offline_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-02-28 21:09:56.000000 splendaq-0.4.1/src/splendaq/daq/_oscilloscope.py
--rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-02-28 21:09:56.000000 splendaq-0.4.1/src/splendaq/daq/_sequencer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 21:10:06.688944 splendaq-0.4.1/src/splendaq/io/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-28 21:09:56.000000 splendaq-0.4.1/src/splendaq/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-02-28 21:09:56.000000 splendaq-0.4.1/src/splendaq/io/_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 21:10:06.688944 splendaq-0.4.1/src/splendaq/io/_liconvert/
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-02-28 21:09:56.000000 splendaq-0.4.1/src/splendaq/io/_liconvert/COPYING.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)   716536 2023-02-28 21:09:56.000000 splendaq-0.4.1/src/splendaq/io/_liconvert/liconvert_linux
--rwxr-xr-x   0 runner    (1001) docker     (123)   629104 2023-02-28 21:09:56.000000 splendaq-0.4.1/src/splendaq/io/_liconvert/liconvert_macos
--rw-r--r--   0 runner    (1001) docker     (123)   689928 2023-02-28 21:09:56.000000 splendaq-0.4.1/src/splendaq/io/_liconvert/liconvert_windows.exe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 21:10:06.688944 splendaq-0.4.1/src/splendaq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-02-28 21:10:06.000000 splendaq-0.4.1/src/splendaq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-02-28 21:10:06.000000 splendaq-0.4.1/src/splendaq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 21:10:06.000000 splendaq-0.4.1/src/splendaq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-28 21:10:06.000000 splendaq-0.4.1/src/splendaq.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 21:10:06.000000 splendaq-0.4.1/src/splendaq.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-28 21:10:06.000000 splendaq-0.4.1/src/splendaq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-28 21:10:06.000000 splendaq-0.4.1/src/splendaq.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 21:10:06.684944 splendaq-0.4.1/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 21:10:06.692944 splendaq-0.4.1/tutorials/daq/
--rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-02-28 21:09:56.000000 splendaq-0.4.1/tutorials/daq/dc_oscilloscope.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-02-28 21:09:56.000000 splendaq-0.4.1/tutorials/daq/event_building.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-02-28 21:09:56.000000 splendaq-0.4.1/tutorials/daq/logging_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-02-28 21:09:56.000000 splendaq-0.4.1/tutorials/daq/running_the_sequencer.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-02-28 21:09:56.000000 splendaq-0.4.1/tutorials/daq/sequencer_settings.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 21:10:06.692944 splendaq-0.4.1/tutorials/io/
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-02-28 21:09:56.000000 splendaq-0.4.1/tutorials/io/read_files.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-02-28 21:09:56.000000 splendaq-0.4.1/tutorials/io/write_files.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:18:01.279411 splendaq-0.4.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:18:01.271411 splendaq-0.4.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:18:01.271411 splendaq-0.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-09 17:17:50.000000 splendaq-0.4.2/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-09 17:17:50.000000 splendaq-0.4.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-09 17:17:50.000000 splendaq-0.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-09 17:17:50.000000 splendaq-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-09 17:17:50.000000 splendaq-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-09 17:18:01.279411 splendaq-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-09 17:17:50.000000 splendaq-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 17:17:50.000000 splendaq-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-09 17:18:01.279411 splendaq-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-09 17:17:50.000000 splendaq-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:18:01.271411 splendaq-0.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:18:01.271411 splendaq-0.4.2/src/splendaq/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-09 17:17:50.000000 splendaq-0.4.2/src/splendaq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-09 17:17:50.000000 splendaq-0.4.2/src/splendaq/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-09 17:18:01.000000 splendaq-0.4.2/src/splendaq/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:18:01.275411 splendaq-0.4.2/src/splendaq/daq/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-09 17:17:50.000000 splendaq-0.4.2/src/splendaq/daq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18531 2023-06-09 17:17:50.000000 splendaq-0.4.2/src/splendaq/daq/_log_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23457 2023-06-09 17:17:50.000000 splendaq-0.4.2/src/splendaq/daq/_offline_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-06-09 17:17:50.000000 splendaq-0.4.2/src/splendaq/daq/_oscilloscope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-06-09 17:17:50.000000 splendaq-0.4.2/src/splendaq/daq/_sequencer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:18:01.275411 splendaq-0.4.2/src/splendaq/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-09 17:17:50.000000 splendaq-0.4.2/src/splendaq/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-06-09 17:17:50.000000 splendaq-0.4.2/src/splendaq/io/_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:18:01.275411 splendaq-0.4.2/src/splendaq/io/_liconvert/
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-09 17:17:50.000000 splendaq-0.4.2/src/splendaq/io/_liconvert/COPYING.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)   716536 2023-06-09 17:17:50.000000 splendaq-0.4.2/src/splendaq/io/_liconvert/liconvert_linux
+-rwxr-xr-x   0 runner    (1001) docker     (123)   629104 2023-06-09 17:17:50.000000 splendaq-0.4.2/src/splendaq/io/_liconvert/liconvert_macos
+-rw-r--r--   0 runner    (1001) docker     (123)   689928 2023-06-09 17:17:50.000000 splendaq-0.4.2/src/splendaq/io/_liconvert/liconvert_windows.exe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:18:01.275411 splendaq-0.4.2/src/splendaq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-09 17:18:01.000000 splendaq-0.4.2/src/splendaq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-09 17:18:01.000000 splendaq-0.4.2/src/splendaq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 17:18:01.000000 splendaq-0.4.2/src/splendaq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-09 17:18:01.000000 splendaq-0.4.2/src/splendaq.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 17:18:01.000000 splendaq-0.4.2/src/splendaq.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-09 17:18:01.000000 splendaq-0.4.2/src/splendaq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-09 17:18:01.000000 splendaq-0.4.2/src/splendaq.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:18:01.271411 splendaq-0.4.2/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:18:01.279411 splendaq-0.4.2/tutorials/daq/
+-rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-06-09 17:17:50.000000 splendaq-0.4.2/tutorials/daq/dc_oscilloscope.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-06-09 17:17:50.000000 splendaq-0.4.2/tutorials/daq/event_building.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-06-09 17:17:50.000000 splendaq-0.4.2/tutorials/daq/logging_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-06-09 17:17:50.000000 splendaq-0.4.2/tutorials/daq/running_the_sequencer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-09 17:17:50.000000 splendaq-0.4.2/tutorials/daq/sequencer_settings.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:18:01.279411 splendaq-0.4.2/tutorials/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-06-09 17:17:50.000000 splendaq-0.4.2/tutorials/io/read_files.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-06-09 17:17:50.000000 splendaq-0.4.2/tutorials/io/write_files.ipynb
```

### Comparing `splendaq-0.4.1/.github/workflows/python-package.yml` & `splendaq-0.4.2/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.1/.github/workflows/python-publish.yml` & `splendaq-0.4.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.1/.gitignore` & `splendaq-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.1/LICENSE` & `splendaq-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.1/PKG-INFO` & `splendaq-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splendaq
-Version: 0.4.1
+Version: 0.4.2
 Summary: Generalized offline data acquisition with a focus on the Moku
 Home-page: https://github.com/splendor-collab/splendaq
 Author: SPLENDOR Collaboration
 Maintainer: SPLENDOR Collaboration
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `splendaq-0.4.1/README.md` & `splendaq-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.1/setup.cfg` & `splendaq-0.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.1/src/splendaq/_cli.py` & `splendaq-0.4.2/src/splendaq/_cli.py`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.1/src/splendaq/daq/_log_data.py` & `splendaq-0.4.2/src/splendaq/daq/_log_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -450,16 +450,21 @@
 
         self.DL.set_samplerate(self._fs)
 
         filenames = []
         nfiles = np.int32(np.ceil(duration / self._max_dur_per_file))
 
         for ii in range(nfiles):
+            if (ii + 1) * self._max_dur_per_file > duration:
+                this_file_duration = duration % self._max_dur_per_file
+            else:
+                this_file_duration = self._max_dur_per_file
+
             logfile = self.DL.start_logging(
-                duration=duration,
+                duration=this_file_duration,
                 comments=comments,
                 file_name_prefix=file_name_prefix,
             )
             # Track progress percentage of the data logging session
             is_logging = True
             while is_logging:
                 # Wait for the logging session to progress by sleeping 0.5sec
```

### Comparing `splendaq-0.4.1/src/splendaq/daq/_offline_trigger.py` & `splendaq-0.4.2/src/splendaq/daq/_offline_trigger.py`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.1/src/splendaq/daq/_oscilloscope.py` & `splendaq-0.4.2/src/splendaq/daq/_oscilloscope.py`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.1/src/splendaq/daq/_sequencer.py` & `splendaq-0.4.2/src/splendaq/daq/_sequencer.py`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.1/src/splendaq/io/_io.py` & `splendaq-0.4.2/src/splendaq/io/_io.py`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.1/src/splendaq/io/_liconvert/COPYING.txt` & `splendaq-0.4.2/src/splendaq/io/_liconvert/COPYING.txt`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.1/src/splendaq/io/_liconvert/liconvert_linux` & `splendaq-0.4.2/src/splendaq/io/_liconvert/liconvert_linux`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.1/src/splendaq/io/_liconvert/liconvert_macos` & `splendaq-0.4.2/src/splendaq/io/_liconvert/liconvert_macos`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.1/src/splendaq/io/_liconvert/liconvert_windows.exe` & `splendaq-0.4.2/src/splendaq/io/_liconvert/liconvert_windows.exe`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.1/src/splendaq.egg-info/PKG-INFO` & `splendaq-0.4.2/src/splendaq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splendaq
-Version: 0.4.1
+Version: 0.4.2
 Summary: Generalized offline data acquisition with a focus on the Moku
 Home-page: https://github.com/splendor-collab/splendaq
 Author: SPLENDOR Collaboration
 Maintainer: SPLENDOR Collaboration
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `splendaq-0.4.1/src/splendaq.egg-info/SOURCES.txt` & `splendaq-0.4.2/src/splendaq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.1/tutorials/daq/dc_oscilloscope.ipynb` & `splendaq-0.4.2/tutorials/daq/dc_oscilloscope.ipynb`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.1/tutorials/daq/event_building.ipynb` & `splendaq-0.4.2/tutorials/daq/event_building.ipynb`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.1/tutorials/daq/logging_data.ipynb` & `splendaq-0.4.2/tutorials/daq/logging_data.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993489583333334%*

 * *Differences: {"'cells'": '{7: {\'source\': ["convert_li_to_h5(\'created_file.li\', my_os=\'mac\')"]}}'}*

```diff
@@ -84,15 +84,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "c4053b26-01a5-4170-97fc-47c3ebbd118a",
             "metadata": {},
             "outputs": [],
             "source": [
-                "convert_li_to_h5('created_file.li', my_os='macos')"
+                "convert_li_to_h5('created_file.li', my_os='mac')"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "585b3c5c-4cf9-4c5d-ba88-80849ac753e4",
             "metadata": {},
             "source": [
```

### Comparing `splendaq-0.4.1/tutorials/daq/running_the_sequencer.ipynb` & `splendaq-0.4.2/tutorials/daq/running_the_sequencer.ipynb`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.1/tutorials/daq/sequencer_settings.yaml` & `splendaq-0.4.2/tutorials/daq/sequencer_settings.yaml`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.1/tutorials/io/read_files.ipynb` & `splendaq-0.4.2/tutorials/io/read_files.ipynb`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.1/tutorials/io/write_files.ipynb` & `splendaq-0.4.2/tutorials/io/write_files.ipynb`

 * *Files identical despite different names*

