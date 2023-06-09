# Comparing `tmp/agh_vqis-2.0.4.tar.gz` & `tmp/agh_vqis-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agh_vqis-2.0.4.tar", last modified: Fri Mar  3 18:13:37 2023, max compression
+gzip compressed data, was "agh_vqis-2.0.5.tar", last modified: Fri Jun  9 16:35:32 2023, max compression
```

## Comparing `agh_vqis-2.0.4.tar` & `agh_vqis-2.0.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-03-03 18:13:37.880847 agh_vqis-2.0.4/
--rw-rw-rw-   0        0        0     2826 2023-01-28 21:45:19.000000 agh_vqis-2.0.4/LICENSE
--rw-rw-rw-   0        0        0     4967 2023-03-03 18:13:37.881845 agh_vqis-2.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3959 2023-03-03 18:07:18.000000 agh_vqis-2.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-03-03 18:13:37.703577 agh_vqis-2.0.4/agh_vqis.egg-info/
--rw-rw-rw-   0        0        0     4967 2023-03-03 18:13:37.000000 agh_vqis-2.0.4/agh_vqis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      712 2023-03-03 18:13:37.000000 agh_vqis-2.0.4/agh_vqis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-03 18:13:37.000000 agh_vqis-2.0.4/agh_vqis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      184 2023-03-03 18:13:37.000000 agh_vqis-2.0.4/agh_vqis.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-03-03 18:13:37.000000 agh_vqis-2.0.4/agh_vqis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       97 2023-01-28 21:02:34.000000 agh_vqis-2.0.4/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-03-03 18:13:37.647521 agh_vqis-2.0.4/python-cpbd/
-drwxrwxrwx   0        0        0        0 2023-03-03 18:13:37.728578 agh_vqis-2.0.4/python-cpbd/cpbd/
--rw-rw-rw-   0        0        0       49 2023-01-28 22:00:29.000000 agh_vqis-2.0.4/python-cpbd/cpbd/__init__.py
--rw-rw-rw-   0        0        0     7670 2023-01-28 22:00:29.000000 agh_vqis-2.0.4/python-cpbd/cpbd/compute.py
--rw-rw-rw-   0        0        0     1540 2023-01-28 22:00:29.000000 agh_vqis-2.0.4/python-cpbd/cpbd/octave.py
--rw-rw-rw-   0        0        0     1305 2023-03-03 18:13:37.893938 agh_vqis-2.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-03 18:13:37.649520 agh_vqis-2.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-03-03 18:13:37.862330 agh_vqis-2.0.4/src/agh_vqis/
--rw-rw-rw-   0        0        0   779962 2023-01-28 21:02:34.000000 agh_vqis-2.0.4/src/agh_vqis/12k_all_set.json
--rw-rw-rw-   0        0        0   412834 2023-01-28 21:02:34.000000 agh_vqis-2.0.4/src/agh_vqis/9k_all_set.json
--rw-rw-rw-   0        0        0      370 2023-03-03 18:12:50.000000 agh_vqis-2.0.4/src/agh_vqis/__init__.py
--rw-rw-rw-   0        0        0    25012 2023-03-03 18:09:41.000000 agh_vqis-2.0.4/src/agh_vqis/__main__.py
--rw-rw-rw-   0        0        0      202 2023-01-28 21:02:34.000000 agh_vqis-2.0.4/src/agh_vqis/_governor.py
--rw-rw-rw-   0        0        0     1349 2023-01-28 21:02:34.000000 agh_vqis-2.0.4/src/agh_vqis/_logger.py
--rw-rw-rw-   0        0        0    54984 2023-01-28 21:02:34.000000 agh_vqis-2.0.4/src/agh_vqis/agh_vqis_binary_macosx
--rw-rw-rw-   0        0        0    97508 2023-01-28 21:02:34.000000 agh_vqis-2.0.4/src/agh_vqis/agh_vqis_binary_macosx_mt
--rw-rw-rw-   0        0        0    66424 2023-01-28 21:02:34.000000 agh_vqis-2.0.4/src/agh_vqis/agh_vqis_binary_x86_mt
--rwxrwxrwx   0        0        0   127167 2023-01-28 21:02:34.000000 agh_vqis-2.0.4/src/agh_vqis/mitsuWin64_multithread.exe
--rwxrwxrwx   0        0        0     4104 2023-01-28 21:02:34.000000 agh_vqis-2.0.4/src/agh_vqis/mitsu_single_file.bat
--rw-rw-rw-   0        0        0     8169 2023-03-03 18:12:35.000000 agh_vqis-2.0.4/src/agh_vqis/mitsu_single_file.sh
--rw-rw-rw-   0        0        0     1519 2023-01-28 21:02:34.000000 agh_vqis-2.0.4/src/agh_vqis/ugc.py
-drwxrwxrwx   0        0        0        0 2023-03-03 18:13:37.876849 agh_vqis-2.0.4/src/agh_vqis/utils/
--rw-rw-rw-   0        0        0     7358 2023-02-24 14:46:31.000000 agh_vqis-2.0.4/src/agh_vqis/utils/utils.py
+drwxrwxr-x   0 filek7    (1000) filek7    (1000)        0 2023-06-09 16:35:32.038015 agh_vqis-2.0.5/
+-rw-rw-r--   0 filek7    (1000) filek7    (1000)     2802 2023-06-09 14:59:22.000000 agh_vqis-2.0.5/LICENSE
+-rw-rw-r--   0 filek7    (1000) filek7    (1000)     4859 2023-06-09 16:35:32.038015 agh_vqis-2.0.5/PKG-INFO
+-rw-rw-r--   0 filek7    (1000) filek7    (1000)     3875 2023-06-09 14:59:22.000000 agh_vqis-2.0.5/README.md
+drwxrwxr-x   0 filek7    (1000) filek7    (1000)        0 2023-06-09 16:35:32.034015 agh_vqis-2.0.5/agh_vqis.egg-info/
+-rw-rw-r--   0 filek7    (1000) filek7    (1000)     4859 2023-06-09 16:35:32.000000 agh_vqis-2.0.5/agh_vqis.egg-info/PKG-INFO
+-rw-rw-r--   0 filek7    (1000) filek7    (1000)      666 2023-06-09 16:35:32.000000 agh_vqis-2.0.5/agh_vqis.egg-info/SOURCES.txt
+-rw-rw-r--   0 filek7    (1000) filek7    (1000)        1 2023-06-09 16:35:32.000000 agh_vqis-2.0.5/agh_vqis.egg-info/dependency_links.txt
+-rw-rw-r--   0 filek7    (1000) filek7    (1000)      205 2023-06-09 16:35:32.000000 agh_vqis-2.0.5/agh_vqis.egg-info/requires.txt
+-rw-rw-r--   0 filek7    (1000) filek7    (1000)       14 2023-06-09 16:35:32.000000 agh_vqis-2.0.5/agh_vqis.egg-info/top_level.txt
+-rw-rw-r--   0 filek7    (1000) filek7    (1000)       94 2023-06-09 14:59:22.000000 agh_vqis-2.0.5/pyproject.toml
+drwxrwxr-x   0 filek7    (1000) filek7    (1000)        0 2023-06-09 16:35:32.034015 agh_vqis-2.0.5/python-cpbd/
+drwxrwxr-x   0 filek7    (1000) filek7    (1000)        0 2023-06-09 16:35:32.034015 agh_vqis-2.0.5/python-cpbd/cpbd/
+-rw-rw-r--   0 filek7    (1000) filek7    (1000)       46 2023-06-09 16:10:26.000000 agh_vqis-2.0.5/python-cpbd/cpbd/__init__.py
+-rw-rw-r--   0 filek7    (1000) filek7    (1000)     7459 2023-06-09 16:10:26.000000 agh_vqis-2.0.5/python-cpbd/cpbd/compute.py
+-rw-rw-r--   0 filek7    (1000) filek7    (1000)     1481 2023-06-09 16:10:26.000000 agh_vqis-2.0.5/python-cpbd/cpbd/octave.py
+-rw-rw-r--   0 filek7    (1000) filek7    (1000)     1279 2023-06-09 16:35:32.038015 agh_vqis-2.0.5/setup.cfg
+drwxrwxr-x   0 filek7    (1000) filek7    (1000)        0 2023-06-09 16:35:32.034015 agh_vqis-2.0.5/src/
+drwxrwxr-x   0 filek7    (1000) filek7    (1000)        0 2023-06-09 16:35:32.034015 agh_vqis-2.0.5/src/agh_vqis/
+-rw-rw-r--   0 filek7    (1000) filek7    (1000)      356 2023-06-09 16:00:36.000000 agh_vqis-2.0.5/src/agh_vqis/__init__.py
+-rw-rw-r--   0 filek7    (1000) filek7    (1000)    21441 2023-06-09 16:20:13.000000 agh_vqis-2.0.5/src/agh_vqis/__main__.py
+-rw-rw-r--   0 filek7    (1000) filek7    (1000)      202 2023-06-09 09:10:29.000000 agh_vqis-2.0.5/src/agh_vqis/_governor.py
+-rw-rw-r--   0 filek7    (1000) filek7    (1000)     1349 2023-06-09 09:10:29.000000 agh_vqis-2.0.5/src/agh_vqis/_logger.py
+drwxrwxr-x   0 filek7    (1000) filek7    (1000)        0 2023-06-09 16:35:32.034015 agh_vqis-2.0.5/src/agh_vqis/binaries/
+-rw-rw-r--   0 filek7    (1000) filek7    (1000)    97508 2023-06-09 09:10:29.000000 agh_vqis-2.0.5/src/agh_vqis/binaries/agh_vqis_binary_macosx_mt
+-rw-rw-r--   0 filek7    (1000) filek7    (1000)   127167 2023-06-09 09:10:29.000000 agh_vqis-2.0.5/src/agh_vqis/binaries/agh_vqis_binary_win64_mt.exe
+-rwxrwxr-x   0 filek7    (1000) filek7    (1000)    66424 2023-06-09 09:10:29.000000 agh_vqis-2.0.5/src/agh_vqis/binaries/agh_vqis_binary_x86_mt
+drwxrwxr-x   0 filek7    (1000) filek7    (1000)        0 2023-06-09 16:35:32.034015 agh_vqis-2.0.5/src/agh_vqis/models/
+drwxrwxr-x   0 filek7    (1000) filek7    (1000)        0 2023-06-09 16:35:32.034015 agh_vqis-2.0.5/src/agh_vqis/models/ugc/
+-rw-rw-r--   0 filek7    (1000) filek7    (1000)   779962 2023-06-09 09:10:29.000000 agh_vqis-2.0.5/src/agh_vqis/models/ugc/12k_all_set.json
+-rw-rw-r--   0 filek7    (1000) filek7    (1000)   412834 2023-06-09 09:10:29.000000 agh_vqis-2.0.5/src/agh_vqis/models/ugc/9k_all_set.json
+drwxrwxr-x   0 filek7    (1000) filek7    (1000)        0 2023-06-09 16:35:32.038015 agh_vqis-2.0.5/src/agh_vqis/utils/
+-rw-rw-r--   0 filek7    (1000) filek7    (1000)     4748 2023-06-09 15:48:27.000000 agh_vqis-2.0.5/src/agh_vqis/utils/helpers.py
+-rw-rw-r--   0 filek7    (1000) filek7    (1000)     6368 2023-06-09 12:38:14.000000 agh_vqis-2.0.5/src/agh_vqis/utils/ugc.py
```

### Comparing `agh_vqis-2.0.4/LICENSE` & `agh_vqis-2.0.5/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-NOTE:
-This evaluation license agreement is made between AGH University of Science and Technology in Krakow; 30 Mickiewicza Avenue 30-059 Krakow ("AGH") and You ("Licensee"). By installing, copying, or otherwise using the licensed software, you agree to be bound by the terms of this agreement. If you are accepting these terms on behalf of the Licensee, you represent and warrant that you have full authority to bind the Licensee to these terms.
-For inquiries about purchasing a full license, contact qoe@agh.edu.pl.
-
-
-EVALUATION LICENSE AGREEMENT
-
-1. SCOPE: This license agreement governs the terms and conditions of using the Python package for automatic image distortion detection ("agh-vqis" or "Software").
-
-2. EVALUATION LICENSE: AGH grants the Licensee a non-exclusive, non-transferable, non-sublicensable and revocable license to use the Software by reproducing it and running it on any number of devices, only for evaluation purposes, i.e. to allow the Licensee to become familiar with its functions before making a decision about purchasing a full license.
-
-3. DOCUMENTATION: If AGH makes any documentation available to the Licensee, the Licensee may use it for the same purposes, for which they may use the Software and make copies of it for the personnel using the Software.
-
-4. FREE OF CHARGE: Due to the nature of the license, it is granted free of charge.
-
-5. RESTRICTIONS: The Licensee may not use the Software nor its documentation for purposes not described in this agreement without separate authorization by AGH. The license does not authorize the Licensee to use the Software for production purposes, including in any commercial activity, nor to modify it, distribute it or otherwise make it available to third parties.
-
-6. THIRD PARTY COMPONENTS: To the extent that Software contains components to which a third party owns the copyright, such components are subject to license terms described in the documentation.
-
-7. PERIOD: The license is granted for an unlimited time. If the Licensee infringes intellectual property rights of AGH or breaches the obligations described in this Agreement, AGH may terminate the license with immediate effect.
-
-8. LIABILITY: Due to the nature of the license, AGH is not liable for any damages which may arise in connection with the use of the Software (e.g. due to its improper functioning, lack of expected functionality, other issues or legal defects). However, this exclusion does not apply to situations when damages arise due to intentional behaviour of AGH or when the mandatory provisions of the law do not allow to limit the liability.
-
-9. LAW AND VENUE: The License Agreement shall be governed by Polish law. Polish courts shall have jurisdiction with regard to any disputes arising from the License Agreement or in connection with it.
+NOTE:
+This evaluation license agreement is made between AGH University of Science and Technology in Krakow; 30 Mickiewicza Avenue 30-059 Krakow ("AGH") and You ("Licensee"). By installing, copying, or otherwise using the licensed software, you agree to be bound by the terms of this agreement. If you are accepting these terms on behalf of the Licensee, you represent and warrant that you have full authority to bind the Licensee to these terms.
+For inquiries about purchasing a full license, contact qoe@agh.edu.pl.
+
+
+EVALUATION LICENSE AGREEMENT
+
+1. SCOPE: This license agreement governs the terms and conditions of using the Python package for automatic image distortion detection ("agh-vqis" or "Software").
+
+2. EVALUATION LICENSE: AGH grants the Licensee a non-exclusive, non-transferable, non-sublicensable and revocable license to use the Software by reproducing it and running it on any number of devices, only for evaluation purposes, i.e. to allow the Licensee to become familiar with its functions before making a decision about purchasing a full license.
+
+3. DOCUMENTATION: If AGH makes any documentation available to the Licensee, the Licensee may use it for the same purposes, for which they may use the Software and make copies of it for the personnel using the Software.
+
+4. FREE OF CHARGE: Due to the nature of the license, it is granted free of charge.
+
+5. RESTRICTIONS: The Licensee may not use the Software nor its documentation for purposes not described in this agreement without separate authorization by AGH. The license does not authorize the Licensee to use the Software for production purposes, including in any commercial activity, nor to modify it, distribute it or otherwise make it available to third parties.
+
+6. THIRD PARTY COMPONENTS: To the extent that Software contains components to which a third party owns the copyright, such components are subject to license terms described in the documentation.
+
+7. PERIOD: The license is granted for an unlimited time. If the Licensee infringes intellectual property rights of AGH or breaches the obligations described in this Agreement, AGH may terminate the license with immediate effect.
+
+8. LIABILITY: Due to the nature of the license, AGH is not liable for any damages which may arise in connection with the use of the Software (e.g. due to its improper functioning, lack of expected functionality, other issues or legal defects). However, this exclusion does not apply to situations when damages arise due to intentional behaviour of AGH or when the mandatory provisions of the law do not allow to limit the liability.
+
+9. LAW AND VENUE: The License Agreement shall be governed by Polish law. Polish courts shall have jurisdiction with regard to any disputes arising from the License Agreement or in connection with it.
```

### Comparing `agh_vqis-2.0.4/PKG-INFO` & `agh_vqis-2.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,108 +1,108 @@
-Metadata-Version: 2.1
-Name: agh_vqis
-Version: 2.0.4
-Summary: A Python wrapper for 18 image quality indicators.
-Home-page: https://qoe.agh.edu.pl/indicators/
-Author: Jakub Nawała, Filip Korus
-Author-email: jakub.nawala@agh.edu.pl, fkorus@student.agh.edu.pl
-License: EVALUATION LICENSE AGREEMENT
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: Other/Proprietary License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Telecommunications Industry
-Classifier: Topic :: Multimedia :: Video
-Classifier: Topic :: Scientific/Engineering :: Image Processing
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# agh-vqis
-A Python package computing a set of image quality indicators (IQIs) for a given input video.
-
-Following IQIs are included in the package:
-
-- A set of 15 Video Quality Indicators (VQIs) developed by the team from AGH. See the following website for more information: https://qoe.agh.edu.pl/indicators/.
-- Our Python reimplementation of the Colourfulness IQI. See [this](http://infoscience.epfl.ch/record/33994/files/HaslerS03.pdf) paper for more information regarding this IQI.
-- Blur Amount IQI. See [package's Python Package Index web page](https://pypi.org/project/cpbd/) for more information.
-- UGC IQI (User-generated content).
-
-**Authors**: Jakub Nawała <[jakub.nawala@agh.edu.pl](mailto:jnawala@agh.edu.pl)>, Filip Korus <[fkorus@student.agh.edu.pl](mailto:fkorus@studnt.agh.edu.pl)>
-
-## Requirements
-- ffmpeg - version == 4.4.2 (4.x.x should also work)
-- Python - version >= 3.9
-
-## Installation
-```shell
-$ pip install agh_vqis
-```
-
-### Usage
-1. Single multimedia file:
-    ```python
-    from agh_vqis import process_single_mm_file
-    from pathlib import Path
-    
-    if __name__ == '__main__':
-        process_single_mm_file(Path('/path/to/single/movie.mp4'))
-    ```
-
-
-2. Folder with multimedia files:
-    ```python
-    from agh_vqis import process_folder_w_mm_files
-    from pathlib import Path
-    
-    if __name__ == '__main__':
-        process_folder_w_mm_files(Path('/path/to/multimedia/folder/'))
-   ```
-
-
-3. Options parameter - in either `process_single_mm_file` and `process_folder_w_mm_files` function options could be provided as an optional argument. It is being passed to function as a dictionary like below.
-    ```python
-     process_single_mm_file(Path('/path/to/single/movie.mp4'), options={
-         'contrast': False, # disable contrast indicator
-         'colourfulness': False, # disable colourfulness indicator
-         'exec': '/path/to/vqis/executable/file/',
-         'shell': '/bin/bash'
-     })
-    ```
-   
-
-4. How to disable/enable indicators to count? Every indicator is **enabled by default except `blue_amount`** due to long computing time. To disable one of following indicators `(blockiness, sa, letterbox, pillarbox, blockloss, blur, ta, blackout, freezing, exposure, contrast, interlace, noise, slice, flickering, colourfulness, ugc)` pass 
-   ```python
-   'indicator_name': False
-   ```
-   to options dictionary. Whereas to **enable** `blur_amount` indicator pass `True` value.
-
-
-5. Available optional parameters except indicators' flags:
-    - exec: Path to the binary file running 15 AGH VQIs. The default binaries (depending on system and CPU architecture) are provided in the package files and will run automatically. VQIS binary files could be downloaded from [here](https://qoe.agh.edu.pl/indicators/).
-    - shell: Alternative Bash interpreter (instead of the default `/bin/bash`). Provide here a path to the interpreter of your choice.
-
-
-6. agh-vqis package could be used from command line interface as well. For example:
-   ```shell
-   $ python3 -m agh_vqis /path/to/single/movie.mp4 # will run VQIS for single file
-   ```
-   or
-   ```shell
-   $ python3 -m agh_vqis /path/to/multimedia/folder/ # will run VQIS for folder
-   ```
-   Whereas this command will display help:
-   ```shell
-   $ python3 -m agh_vqis -h
-   ```
-7. Supported multimedia files: `mp4`, `y4m`, `mov`, `mkv`, `avi`, `ts`, `jpg`, `jpeg`, `png`, `gif`, `bmp`.
-
-### Output file
-First row of the output CSV file contains header with image quality indicators (IQIs) names, whereas each row below the header represents single video frame from the input video file. Each column provides a numerical result as returned by a given image quality indicator (IQI) when applied to the respective frame.
-
-### License
-The `agh-vqis` Python package is provided via the [Evaluation License Agreement](https://app.qoe.agh.edu.pl/public/agh-vqis/license.txt).
+Metadata-Version: 2.1
+Name: agh_vqis
+Version: 2.0.5
+Summary: A Python wrapper for 18 image quality indicators.
+Home-page: https://qoe.agh.edu.pl/indicators/
+Author: Jakub Nawała, Filip Korus
+Author-email: jakub.nawala@agh.edu.pl, fkorus@student.agh.edu.pl
+License: EVALUATION LICENSE AGREEMENT
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Telecommunications Industry
+Classifier: Topic :: Multimedia :: Video
+Classifier: Topic :: Scientific/Engineering :: Image Processing
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# agh-vqis
+A Python package computing a set of image quality indicators (IQIs) for a given input video.
+
+Following IQIs are included in the package:
+
+- A set of 15 Video Quality Indicators (VQIs) developed by the team from AGH. See the following website for more information: https://qoe.agh.edu.pl/indicators/.
+- Our Python reimplementation of the Colourfulness IQI. See [this](http://infoscience.epfl.ch/record/33994/files/HaslerS03.pdf) paper for more information regarding this IQI.
+- Blur Amount IQI. See [package's Python Package Index web page](https://pypi.org/project/cpbd/) for more information.
+- UGC IQI (User-generated content).
+
+**Authors**: Jakub Nawała <[jakub.nawala@agh.edu.pl](mailto:jnawala@agh.edu.pl)>, Filip Korus <[fkorus@student.agh.edu.pl](mailto:fkorus@studnt.agh.edu.pl)>
+
+## Requirements
+- ffmpeg - version == 4.4.2 (4.x.x should also work)
+- Python - version >= 3.9
+
+## Installation
+```shell
+$ pip install agh_vqis
+```
+
+### Usage
+1. Single multimedia file:
+    ```python
+    from agh_vqis import process_single_mm_file
+    from pathlib import Path
+    
+    if __name__ == '__main__':
+        process_single_mm_file(Path('/path/to/single/movie.mp4'))
+    ```
+
+
+2. Folder with multimedia files:
+    ```python
+    from agh_vqis import process_folder_w_mm_files
+    from pathlib import Path
+    
+    if __name__ == '__main__':
+        process_folder_w_mm_files(Path('/path/to/multimedia/folder/'))
+   ```
+
+
+3. Options parameter - in either `process_single_mm_file` and `process_folder_w_mm_files` function options could be provided as an optional argument. It is being passed to function as a dictionary like below.
+    ```python
+     process_single_mm_file(Path('/path/to/single/movie.mp4'), options={
+         'contrast': False, # disable contrast indicator
+         'colourfulness': False, # disable colourfulness indicator
+         'exec': '/path/to/vqis/executable/file/',
+         'shell': '/bin/bash'
+     })
+    ```
+   
+
+4. How to disable/enable indicators to count? Every indicator is **enabled by default except `blue_amount`** due to long computing time. To disable one of following indicators `(blockiness, sa, letterbox, pillarbox, blockloss, blur, ta, blackout, freezing, exposure, contrast, interlace, noise, slice, flickering, colourfulness, ugc)` pass 
+   ```python
+   'indicator_name': False
+   ```
+   to options dictionary. Whereas to **enable** `blur_amount` indicator pass `True` value.
+
+
+5. Available optional parameters except indicators' flags:
+    - exec: Path to the binary file running 15 AGH VQIs. The default binaries (depending on system and CPU architecture) are provided in the package files and will run automatically. VQIS binary files could be downloaded from [here](https://qoe.agh.edu.pl/indicators/).
+    - shell: Alternative Bash interpreter (instead of the default `/bin/bash`). Provide here a path to the interpreter of your choice.
+
+
+6. agh-vqis package could be used from command line interface as well. For example:
+   ```shell
+   $ python3 -m agh_vqis /path/to/single/movie.mp4 # will run VQIS for single file
+   ```
+   or
+   ```shell
+   $ python3 -m agh_vqis /path/to/multimedia/folder/ # will run VQIS for folder
+   ```
+   Whereas this command will display help:
+   ```shell
+   $ python3 -m agh_vqis -h
+   ```
+7. Supported multimedia files: `mp4`, `y4m`, `mov`, `mkv`, `avi`, `ts`, `jpg`, `jpeg`, `png`, `gif`, `bmp`.
+
+### Output file
+First row of the output CSV file contains header with image quality indicators (IQIs) names, whereas each row below the header represents single video frame from the input video file. Each column provides a numerical result as returned by a given image quality indicator (IQI) when applied to the respective frame.
+
+### License
+The `agh-vqis` Python package is provided via the [Evaluation License Agreement](https://app.qoe.agh.edu.pl/public/agh-vqis/license.txt).
```

### Comparing `agh_vqis-2.0.4/README.md` & `agh_vqis-2.0.5/README.md`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-# agh-vqis
-A Python package computing a set of image quality indicators (IQIs) for a given input video.
-
-Following IQIs are included in the package:
-
-- A set of 15 Video Quality Indicators (VQIs) developed by the team from AGH. See the following website for more information: https://qoe.agh.edu.pl/indicators/.
-- Our Python reimplementation of the Colourfulness IQI. See [this](http://infoscience.epfl.ch/record/33994/files/HaslerS03.pdf) paper for more information regarding this IQI.
-- Blur Amount IQI. See [package's Python Package Index web page](https://pypi.org/project/cpbd/) for more information.
-- UGC IQI (User-generated content).
-
-**Authors**: Jakub Nawała <[jakub.nawala@agh.edu.pl](mailto:jnawala@agh.edu.pl)>, Filip Korus <[fkorus@student.agh.edu.pl](mailto:fkorus@studnt.agh.edu.pl)>
-
-## Requirements
-- ffmpeg - version == 4.4.2 (4.x.x should also work)
-- Python - version >= 3.9
-
-## Installation
-```shell
-$ pip install agh_vqis
-```
-
-### Usage
-1. Single multimedia file:
-    ```python
-    from agh_vqis import process_single_mm_file
-    from pathlib import Path
-    
-    if __name__ == '__main__':
-        process_single_mm_file(Path('/path/to/single/movie.mp4'))
-    ```
-
-
-2. Folder with multimedia files:
-    ```python
-    from agh_vqis import process_folder_w_mm_files
-    from pathlib import Path
-    
-    if __name__ == '__main__':
-        process_folder_w_mm_files(Path('/path/to/multimedia/folder/'))
-   ```
-
-
-3. Options parameter - in either `process_single_mm_file` and `process_folder_w_mm_files` function options could be provided as an optional argument. It is being passed to function as a dictionary like below.
-    ```python
-     process_single_mm_file(Path('/path/to/single/movie.mp4'), options={
-         'contrast': False, # disable contrast indicator
-         'colourfulness': False, # disable colourfulness indicator
-         'exec': '/path/to/vqis/executable/file/',
-         'shell': '/bin/bash'
-     })
-    ```
-   
-
-4. How to disable/enable indicators to count? Every indicator is **enabled by default except `blue_amount`** due to long computing time. To disable one of following indicators `(blockiness, sa, letterbox, pillarbox, blockloss, blur, ta, blackout, freezing, exposure, contrast, interlace, noise, slice, flickering, colourfulness, ugc)` pass 
-   ```python
-   'indicator_name': False
-   ```
-   to options dictionary. Whereas to **enable** `blur_amount` indicator pass `True` value.
-
-
-5. Available optional parameters except indicators' flags:
-    - exec: Path to the binary file running 15 AGH VQIs. The default binaries (depending on system and CPU architecture) are provided in the package files and will run automatically. VQIS binary files could be downloaded from [here](https://qoe.agh.edu.pl/indicators/).
-    - shell: Alternative Bash interpreter (instead of the default `/bin/bash`). Provide here a path to the interpreter of your choice.
-
-
-6. agh-vqis package could be used from command line interface as well. For example:
-   ```shell
-   $ python3 -m agh_vqis /path/to/single/movie.mp4 # will run VQIS for single file
-   ```
-   or
-   ```shell
-   $ python3 -m agh_vqis /path/to/multimedia/folder/ # will run VQIS for folder
-   ```
-   Whereas this command will display help:
-   ```shell
-   $ python3 -m agh_vqis -h
-   ```
-7. Supported multimedia files: `mp4`, `y4m`, `mov`, `mkv`, `avi`, `ts`, `jpg`, `jpeg`, `png`, `gif`, `bmp`.
-
-### Output file
-First row of the output CSV file contains header with image quality indicators (IQIs) names, whereas each row below the header represents single video frame from the input video file. Each column provides a numerical result as returned by a given image quality indicator (IQI) when applied to the respective frame.
-
-### License
-The `agh-vqis` Python package is provided via the [Evaluation License Agreement](https://app.qoe.agh.edu.pl/public/agh-vqis/license.txt).
+# agh-vqis
+A Python package computing a set of image quality indicators (IQIs) for a given input video.
+
+Following IQIs are included in the package:
+
+- A set of 15 Video Quality Indicators (VQIs) developed by the team from AGH. See the following website for more information: https://qoe.agh.edu.pl/indicators/.
+- Our Python reimplementation of the Colourfulness IQI. See [this](http://infoscience.epfl.ch/record/33994/files/HaslerS03.pdf) paper for more information regarding this IQI.
+- Blur Amount IQI. See [package's Python Package Index web page](https://pypi.org/project/cpbd/) for more information.
+- UGC IQI (User-generated content).
+
+**Authors**: Jakub Nawała <[jakub.nawala@agh.edu.pl](mailto:jnawala@agh.edu.pl)>, Filip Korus <[fkorus@student.agh.edu.pl](mailto:fkorus@studnt.agh.edu.pl)>
+
+## Requirements
+- ffmpeg - version == 4.4.2 (4.x.x should also work)
+- Python - version >= 3.9
+
+## Installation
+```shell
+$ pip install agh_vqis
+```
+
+### Usage
+1. Single multimedia file:
+    ```python
+    from agh_vqis import process_single_mm_file
+    from pathlib import Path
+    
+    if __name__ == '__main__':
+        process_single_mm_file(Path('/path/to/single/movie.mp4'))
+    ```
+
+
+2. Folder with multimedia files:
+    ```python
+    from agh_vqis import process_folder_w_mm_files
+    from pathlib import Path
+    
+    if __name__ == '__main__':
+        process_folder_w_mm_files(Path('/path/to/multimedia/folder/'))
+   ```
+
+
+3. Options parameter - in either `process_single_mm_file` and `process_folder_w_mm_files` function options could be provided as an optional argument. It is being passed to function as a dictionary like below.
+    ```python
+     process_single_mm_file(Path('/path/to/single/movie.mp4'), options={
+         'contrast': False, # disable contrast indicator
+         'colourfulness': False, # disable colourfulness indicator
+         'exec': '/path/to/vqis/executable/file/',
+         'shell': '/bin/bash'
+     })
+    ```
+   
+
+4. How to disable/enable indicators to count? Every indicator is **enabled by default except `blue_amount`** due to long computing time. To disable one of following indicators `(blockiness, sa, letterbox, pillarbox, blockloss, blur, ta, blackout, freezing, exposure, contrast, interlace, noise, slice, flickering, colourfulness, ugc)` pass 
+   ```python
+   'indicator_name': False
+   ```
+   to options dictionary. Whereas to **enable** `blur_amount` indicator pass `True` value.
+
+
+5. Available optional parameters except indicators' flags:
+    - exec: Path to the binary file running 15 AGH VQIs. The default binaries (depending on system and CPU architecture) are provided in the package files and will run automatically. VQIS binary files could be downloaded from [here](https://qoe.agh.edu.pl/indicators/).
+    - shell: Alternative Bash interpreter (instead of the default `/bin/bash`). Provide here a path to the interpreter of your choice.
+
+
+6. agh-vqis package could be used from command line interface as well. For example:
+   ```shell
+   $ python3 -m agh_vqis /path/to/single/movie.mp4 # will run VQIS for single file
+   ```
+   or
+   ```shell
+   $ python3 -m agh_vqis /path/to/multimedia/folder/ # will run VQIS for folder
+   ```
+   Whereas this command will display help:
+   ```shell
+   $ python3 -m agh_vqis -h
+   ```
+7. Supported multimedia files: `mp4`, `y4m`, `mov`, `mkv`, `avi`, `ts`, `jpg`, `jpeg`, `png`, `gif`, `bmp`.
+
+### Output file
+First row of the output CSV file contains header with image quality indicators (IQIs) names, whereas each row below the header represents single video frame from the input video file. Each column provides a numerical result as returned by a given image quality indicator (IQI) when applied to the respective frame.
+
+### License
+The `agh-vqis` Python package is provided via the [Evaluation License Agreement](https://app.qoe.agh.edu.pl/public/agh-vqis/license.txt).
```

### Comparing `agh_vqis-2.0.4/agh_vqis.egg-info/PKG-INFO` & `agh_vqis-2.0.5/agh_vqis.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,108 +1,108 @@
-Metadata-Version: 2.1
-Name: agh-vqis
-Version: 2.0.4
-Summary: A Python wrapper for 18 image quality indicators.
-Home-page: https://qoe.agh.edu.pl/indicators/
-Author: Jakub Nawała, Filip Korus
-Author-email: jakub.nawala@agh.edu.pl, fkorus@student.agh.edu.pl
-License: EVALUATION LICENSE AGREEMENT
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: Other/Proprietary License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Telecommunications Industry
-Classifier: Topic :: Multimedia :: Video
-Classifier: Topic :: Scientific/Engineering :: Image Processing
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# agh-vqis
-A Python package computing a set of image quality indicators (IQIs) for a given input video.
-
-Following IQIs are included in the package:
-
-- A set of 15 Video Quality Indicators (VQIs) developed by the team from AGH. See the following website for more information: https://qoe.agh.edu.pl/indicators/.
-- Our Python reimplementation of the Colourfulness IQI. See [this](http://infoscience.epfl.ch/record/33994/files/HaslerS03.pdf) paper for more information regarding this IQI.
-- Blur Amount IQI. See [package's Python Package Index web page](https://pypi.org/project/cpbd/) for more information.
-- UGC IQI (User-generated content).
-
-**Authors**: Jakub Nawała <[jakub.nawala@agh.edu.pl](mailto:jnawala@agh.edu.pl)>, Filip Korus <[fkorus@student.agh.edu.pl](mailto:fkorus@studnt.agh.edu.pl)>
-
-## Requirements
-- ffmpeg - version == 4.4.2 (4.x.x should also work)
-- Python - version >= 3.9
-
-## Installation
-```shell
-$ pip install agh_vqis
-```
-
-### Usage
-1. Single multimedia file:
-    ```python
-    from agh_vqis import process_single_mm_file
-    from pathlib import Path
-    
-    if __name__ == '__main__':
-        process_single_mm_file(Path('/path/to/single/movie.mp4'))
-    ```
-
-
-2. Folder with multimedia files:
-    ```python
-    from agh_vqis import process_folder_w_mm_files
-    from pathlib import Path
-    
-    if __name__ == '__main__':
-        process_folder_w_mm_files(Path('/path/to/multimedia/folder/'))
-   ```
-
-
-3. Options parameter - in either `process_single_mm_file` and `process_folder_w_mm_files` function options could be provided as an optional argument. It is being passed to function as a dictionary like below.
-    ```python
-     process_single_mm_file(Path('/path/to/single/movie.mp4'), options={
-         'contrast': False, # disable contrast indicator
-         'colourfulness': False, # disable colourfulness indicator
-         'exec': '/path/to/vqis/executable/file/',
-         'shell': '/bin/bash'
-     })
-    ```
-   
-
-4. How to disable/enable indicators to count? Every indicator is **enabled by default except `blue_amount`** due to long computing time. To disable one of following indicators `(blockiness, sa, letterbox, pillarbox, blockloss, blur, ta, blackout, freezing, exposure, contrast, interlace, noise, slice, flickering, colourfulness, ugc)` pass 
-   ```python
-   'indicator_name': False
-   ```
-   to options dictionary. Whereas to **enable** `blur_amount` indicator pass `True` value.
-
-
-5. Available optional parameters except indicators' flags:
-    - exec: Path to the binary file running 15 AGH VQIs. The default binaries (depending on system and CPU architecture) are provided in the package files and will run automatically. VQIS binary files could be downloaded from [here](https://qoe.agh.edu.pl/indicators/).
-    - shell: Alternative Bash interpreter (instead of the default `/bin/bash`). Provide here a path to the interpreter of your choice.
-
-
-6. agh-vqis package could be used from command line interface as well. For example:
-   ```shell
-   $ python3 -m agh_vqis /path/to/single/movie.mp4 # will run VQIS for single file
-   ```
-   or
-   ```shell
-   $ python3 -m agh_vqis /path/to/multimedia/folder/ # will run VQIS for folder
-   ```
-   Whereas this command will display help:
-   ```shell
-   $ python3 -m agh_vqis -h
-   ```
-7. Supported multimedia files: `mp4`, `y4m`, `mov`, `mkv`, `avi`, `ts`, `jpg`, `jpeg`, `png`, `gif`, `bmp`.
-
-### Output file
-First row of the output CSV file contains header with image quality indicators (IQIs) names, whereas each row below the header represents single video frame from the input video file. Each column provides a numerical result as returned by a given image quality indicator (IQI) when applied to the respective frame.
-
-### License
-The `agh-vqis` Python package is provided via the [Evaluation License Agreement](https://app.qoe.agh.edu.pl/public/agh-vqis/license.txt).
+Metadata-Version: 2.1
+Name: agh-vqis
+Version: 2.0.5
+Summary: A Python wrapper for 18 image quality indicators.
+Home-page: https://qoe.agh.edu.pl/indicators/
+Author: Jakub Nawała, Filip Korus
+Author-email: jakub.nawala@agh.edu.pl, fkorus@student.agh.edu.pl
+License: EVALUATION LICENSE AGREEMENT
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Telecommunications Industry
+Classifier: Topic :: Multimedia :: Video
+Classifier: Topic :: Scientific/Engineering :: Image Processing
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# agh-vqis
+A Python package computing a set of image quality indicators (IQIs) for a given input video.
+
+Following IQIs are included in the package:
+
+- A set of 15 Video Quality Indicators (VQIs) developed by the team from AGH. See the following website for more information: https://qoe.agh.edu.pl/indicators/.
+- Our Python reimplementation of the Colourfulness IQI. See [this](http://infoscience.epfl.ch/record/33994/files/HaslerS03.pdf) paper for more information regarding this IQI.
+- Blur Amount IQI. See [package's Python Package Index web page](https://pypi.org/project/cpbd/) for more information.
+- UGC IQI (User-generated content).
+
+**Authors**: Jakub Nawała <[jakub.nawala@agh.edu.pl](mailto:jnawala@agh.edu.pl)>, Filip Korus <[fkorus@student.agh.edu.pl](mailto:fkorus@studnt.agh.edu.pl)>
+
+## Requirements
+- ffmpeg - version == 4.4.2 (4.x.x should also work)
+- Python - version >= 3.9
+
+## Installation
+```shell
+$ pip install agh_vqis
+```
+
+### Usage
+1. Single multimedia file:
+    ```python
+    from agh_vqis import process_single_mm_file
+    from pathlib import Path
+    
+    if __name__ == '__main__':
+        process_single_mm_file(Path('/path/to/single/movie.mp4'))
+    ```
+
+
+2. Folder with multimedia files:
+    ```python
+    from agh_vqis import process_folder_w_mm_files
+    from pathlib import Path
+    
+    if __name__ == '__main__':
+        process_folder_w_mm_files(Path('/path/to/multimedia/folder/'))
+   ```
+
+
+3. Options parameter - in either `process_single_mm_file` and `process_folder_w_mm_files` function options could be provided as an optional argument. It is being passed to function as a dictionary like below.
+    ```python
+     process_single_mm_file(Path('/path/to/single/movie.mp4'), options={
+         'contrast': False, # disable contrast indicator
+         'colourfulness': False, # disable colourfulness indicator
+         'exec': '/path/to/vqis/executable/file/',
+         'shell': '/bin/bash'
+     })
+    ```
+   
+
+4. How to disable/enable indicators to count? Every indicator is **enabled by default except `blue_amount`** due to long computing time. To disable one of following indicators `(blockiness, sa, letterbox, pillarbox, blockloss, blur, ta, blackout, freezing, exposure, contrast, interlace, noise, slice, flickering, colourfulness, ugc)` pass 
+   ```python
+   'indicator_name': False
+   ```
+   to options dictionary. Whereas to **enable** `blur_amount` indicator pass `True` value.
+
+
+5. Available optional parameters except indicators' flags:
+    - exec: Path to the binary file running 15 AGH VQIs. The default binaries (depending on system and CPU architecture) are provided in the package files and will run automatically. VQIS binary files could be downloaded from [here](https://qoe.agh.edu.pl/indicators/).
+    - shell: Alternative Bash interpreter (instead of the default `/bin/bash`). Provide here a path to the interpreter of your choice.
+
+
+6. agh-vqis package could be used from command line interface as well. For example:
+   ```shell
+   $ python3 -m agh_vqis /path/to/single/movie.mp4 # will run VQIS for single file
+   ```
+   or
+   ```shell
+   $ python3 -m agh_vqis /path/to/multimedia/folder/ # will run VQIS for folder
+   ```
+   Whereas this command will display help:
+   ```shell
+   $ python3 -m agh_vqis -h
+   ```
+7. Supported multimedia files: `mp4`, `y4m`, `mov`, `mkv`, `avi`, `ts`, `jpg`, `jpeg`, `png`, `gif`, `bmp`.
+
+### Output file
+First row of the output CSV file contains header with image quality indicators (IQIs) names, whereas each row below the header represents single video frame from the input video file. Each column provides a numerical result as returned by a given image quality indicator (IQI) when applied to the respective frame.
+
+### License
+The `agh-vqis` Python package is provided via the [Evaluation License Agreement](https://app.qoe.agh.edu.pl/public/agh-vqis/license.txt).
```

### Comparing `agh_vqis-2.0.4/agh_vqis.egg-info/SOURCES.txt` & `agh_vqis-2.0.5/agh_vqis.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -6,21 +6,18 @@
 agh_vqis.egg-info/SOURCES.txt
 agh_vqis.egg-info/dependency_links.txt
 agh_vqis.egg-info/requires.txt
 agh_vqis.egg-info/top_level.txt
 python-cpbd/cpbd/__init__.py
 python-cpbd/cpbd/compute.py
 python-cpbd/cpbd/octave.py
-src/agh_vqis/12k_all_set.json
-src/agh_vqis/9k_all_set.json
 src/agh_vqis/__init__.py
 src/agh_vqis/__main__.py
 src/agh_vqis/_governor.py
 src/agh_vqis/_logger.py
-src/agh_vqis/agh_vqis_binary_macosx
-src/agh_vqis/agh_vqis_binary_macosx_mt
-src/agh_vqis/agh_vqis_binary_x86_mt
-src/agh_vqis/mitsuWin64_multithread.exe
-src/agh_vqis/mitsu_single_file.bat
-src/agh_vqis/mitsu_single_file.sh
-src/agh_vqis/ugc.py
-src/agh_vqis/utils/utils.py
+src/agh_vqis/binaries/agh_vqis_binary_macosx_mt
+src/agh_vqis/binaries/agh_vqis_binary_win64_mt.exe
+src/agh_vqis/binaries/agh_vqis_binary_x86_mt
+src/agh_vqis/models/ugc/12k_all_set.json
+src/agh_vqis/models/ugc/9k_all_set.json
+src/agh_vqis/utils/helpers.py
+src/agh_vqis/utils/ugc.py
```

### Comparing `agh_vqis-2.0.4/python-cpbd/cpbd/compute.py` & `agh_vqis-2.0.5/python-cpbd/cpbd/compute.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,211 +1,211 @@
-# coding: utf-8
-
-from __future__ import (
-    absolute_import,
-    division,
-    print_function,
-    unicode_literals
-)
-
-from math import atan2, pi
-from sys import argv
-
-import numpy as np
-from imageio import imread
-from skimage.feature import canny
-
-from cpbd.octave import sobel
-
-
-# threshold to characterize blocks as edge/non-edge blocks
-THRESHOLD = 0.002
-
-# fitting parameter
-BETA = 3.6
-
-# block size
-BLOCK_HEIGHT, BLOCK_WIDTH = (64, 64)
-
-# just noticeable widths based on the perceptual experiments
-WIDTH_JNB = np.concatenate([5*np.ones(51), 3*np.ones(205)])
-
-
-def compute(image):
-    # type: (numpy.ndarray) -> float
-    """Compute the sharpness metric for the given data."""
-
-    # convert the image to double for further processing
-    image = image.astype(np.float64)
-
-    # edge detection using canny and sobel canny edge detection is done to
-    # classify the blocks as edge or non-edge blocks and sobel edge
-    # detection is done for the purpose of edge width measurement.
-    canny_edges = canny(image)
-    sobel_edges = sobel(image)
-
-    # edge width calculation
-    marziliano_widths = marziliano_method(sobel_edges, image)
-
-    # sharpness metric calculation
-    return _calculate_sharpness_metric(image, canny_edges, marziliano_widths)
-
-
-def marziliano_method(edges, image):
-    # type: (numpy.ndarray, numpy.ndarray) -> numpy.ndarray
-    """
-    Calculate the widths of the given edges.
-
-    :return: A matrix with the same dimensions as the given image with 0's at
-        non-edge locations and edge-widths at the edge locations.
-    """
-
-    # `edge_widths` consists of zero and non-zero values. A zero value
-    # indicates that there is no edge at that position and a non-zero value
-    # indicates that there is an edge at that position and the value itself
-    # gives the edge width.
-    edge_widths = np.zeros(image.shape)
-
-    # find the gradient for the image
-    gradient_y, gradient_x = np.gradient(image)
-
-    # dimensions of the image
-    img_height, img_width = image.shape
-
-    # holds the angle information of the edges
-    edge_angles = np.zeros(image.shape)
-
-    # calculate the angle of the edges
-    for row in range(img_height):
-        for col in range(img_width):
-            if gradient_x[row, col] != 0:
-                edge_angles[row, col] = atan2(gradient_y[row, col], gradient_x[row, col]) * (180 / pi)
-            elif gradient_x[row, col] == 0 and gradient_y[row, col] == 0:
-                edge_angles[row,col] = 0
-            elif gradient_x[row, col] == 0 and gradient_y[row, col] == pi/2:
-                edge_angles[row, col] = 90
-
-
-    if np.any(edge_angles):
-
-        # quantize the angle
-        quantized_angles = 45 * np.round(edge_angles / 45)
-
-        for row in range(1, img_height - 1):
-            for col in range(1, img_width - 1):
-                if edges[row, col] == 1:
-
-                    # gradient angle = 180 or -180
-                    if quantized_angles[row, col] == 180 or quantized_angles[row, col] == -180:
-                        for margin in range(100 + 1):
-                            inner_border = (col - 1) - margin
-                            outer_border = (col - 2) - margin
-
-                            # outside image or intensity increasing from left to right
-                            if outer_border < 0 or (image[row, outer_border] - image[row, inner_border]) <= 0:
-                                break
-
-                        width_left = margin + 1
-
-                        for margin in range(100 + 1):
-                            inner_border = (col + 1) + margin
-                            outer_border = (col + 2) + margin
-
-                            # outside image or intensity increasing from left to right
-                            if outer_border >= img_width or (image[row, outer_border] - image[row, inner_border]) >= 0:
-                                break
-
-                        width_right = margin + 1
-
-                        edge_widths[row, col] = width_left + width_right
-
-
-                    # gradient angle = 0
-                    if quantized_angles[row, col] == 0:
-                        for margin in range(100 + 1):
-                            inner_border = (col - 1) - margin
-                            outer_border = (col - 2) - margin
-
-                            # outside image or intensity decreasing from left to right
-                            if outer_border < 0 or (image[row, outer_border] - image[row, inner_border]) >= 0:
-                                break
-
-                        width_left = margin + 1
-
-                        for margin in range(100 + 1):
-                            inner_border = (col + 1) + margin
-                            outer_border = (col + 2) + margin
-
-                            # outside image or intensity decreasing from left to right
-                            if outer_border >= img_width or (image[row, outer_border] - image[row, inner_border]) <= 0:
-                                break
-
-                        width_right = margin + 1
-
-                        edge_widths[row, col] = width_right + width_left
-
-    return edge_widths
-
-
-def _calculate_sharpness_metric(image, edges, edge_widths):
-    # type: (numpy.array, numpy.array, numpy.array) -> numpy.float64
-
-    # get the size of image
-    img_height, img_width = image.shape
-
-    total_num_edges = 0
-    hist_pblur = np.zeros(101)
-
-    # maximum block indices
-    num_blocks_vertically = int(img_height / BLOCK_HEIGHT)
-    num_blocks_horizontally = int(img_width / BLOCK_WIDTH)
-
-    #  loop over the blocks
-    for i in range(num_blocks_vertically):
-        for j in range(num_blocks_horizontally):
-
-            # get the row and col indices for the block pixel positions
-            rows = slice(BLOCK_HEIGHT * i, BLOCK_HEIGHT * (i + 1))
-            cols = slice(BLOCK_WIDTH * j, BLOCK_WIDTH * (j + 1))
-
-            if is_edge_block(edges[rows, cols], THRESHOLD):
-                block_widths = edge_widths[rows, cols]
-                # rotate block to simulate column-major boolean indexing
-                block_widths = np.rot90(np.flipud(block_widths), 3)
-                block_widths = block_widths[block_widths != 0]
-
-                block_contrast = get_block_contrast(image[rows, cols])
-                block_jnb = WIDTH_JNB[block_contrast]
-
-                # calculate the probability of blur detection at the edges
-                # detected in the block
-                prob_blur_detection = 1 - np.exp(-abs(block_widths/block_jnb) ** BETA)
-
-                # update the statistics using the block information
-                for probability in prob_blur_detection:
-                    bucket = int(round(probability * 100))
-                    hist_pblur[bucket] += 1
-                    total_num_edges += 1
-
-    # normalize the pdf
-    if total_num_edges > 0:
-        hist_pblur = hist_pblur / total_num_edges
-
-    # calculate the sharpness metric
-    return np.sum(hist_pblur[:64])
-
-
-def is_edge_block(block, threshold):
-    # type: (numpy.ndarray, float) -> bool
-    """Decide whether the given block is an edge block."""
-    return np.count_nonzero(block) > (block.size * threshold)
-
-
-def get_block_contrast(block):
-    # type: (numpy.ndarray) -> int
-    return int(np.max(block) - np.min(block))
-
-
-if __name__ == '__main__':
-    input_image = imread(argv[1], pilmode = 'L')
-    sharpness = compute(input_image)
-    print('CPBD sharpness for %s: %f' % (argv[1], sharpness))
+# coding: utf-8
+
+from __future__ import (
+    absolute_import,
+    division,
+    print_function,
+    unicode_literals
+)
+
+from math import atan2, pi
+from sys import argv
+
+import numpy as np
+from imageio import imread
+from skimage.feature import canny
+
+from cpbd.octave import sobel
+
+
+# threshold to characterize blocks as edge/non-edge blocks
+THRESHOLD = 0.002
+
+# fitting parameter
+BETA = 3.6
+
+# block size
+BLOCK_HEIGHT, BLOCK_WIDTH = (64, 64)
+
+# just noticeable widths based on the perceptual experiments
+WIDTH_JNB = np.concatenate([5*np.ones(51), 3*np.ones(205)])
+
+
+def compute(image):
+    # type: (numpy.ndarray) -> float
+    """Compute the sharpness metric for the given data."""
+
+    # convert the image to double for further processing
+    image = image.astype(np.float64)
+
+    # edge detection using canny and sobel canny edge detection is done to
+    # classify the blocks as edge or non-edge blocks and sobel edge
+    # detection is done for the purpose of edge width measurement.
+    canny_edges = canny(image)
+    sobel_edges = sobel(image)
+
+    # edge width calculation
+    marziliano_widths = marziliano_method(sobel_edges, image)
+
+    # sharpness metric calculation
+    return _calculate_sharpness_metric(image, canny_edges, marziliano_widths)
+
+
+def marziliano_method(edges, image):
+    # type: (numpy.ndarray, numpy.ndarray) -> numpy.ndarray
+    """
+    Calculate the widths of the given edges.
+
+    :return: A matrix with the same dimensions as the given image with 0's at
+        non-edge locations and edge-widths at the edge locations.
+    """
+
+    # `edge_widths` consists of zero and non-zero values. A zero value
+    # indicates that there is no edge at that position and a non-zero value
+    # indicates that there is an edge at that position and the value itself
+    # gives the edge width.
+    edge_widths = np.zeros(image.shape)
+
+    # find the gradient for the image
+    gradient_y, gradient_x = np.gradient(image)
+
+    # dimensions of the image
+    img_height, img_width = image.shape
+
+    # holds the angle information of the edges
+    edge_angles = np.zeros(image.shape)
+
+    # calculate the angle of the edges
+    for row in range(img_height):
+        for col in range(img_width):
+            if gradient_x[row, col] != 0:
+                edge_angles[row, col] = atan2(gradient_y[row, col], gradient_x[row, col]) * (180 / pi)
+            elif gradient_x[row, col] == 0 and gradient_y[row, col] == 0:
+                edge_angles[row,col] = 0
+            elif gradient_x[row, col] == 0 and gradient_y[row, col] == pi/2:
+                edge_angles[row, col] = 90
+
+
+    if np.any(edge_angles):
+
+        # quantize the angle
+        quantized_angles = 45 * np.round(edge_angles / 45)
+
+        for row in range(1, img_height - 1):
+            for col in range(1, img_width - 1):
+                if edges[row, col] == 1:
+
+                    # gradient angle = 180 or -180
+                    if quantized_angles[row, col] == 180 or quantized_angles[row, col] == -180:
+                        for margin in range(100 + 1):
+                            inner_border = (col - 1) - margin
+                            outer_border = (col - 2) - margin
+
+                            # outside image or intensity increasing from left to right
+                            if outer_border < 0 or (image[row, outer_border] - image[row, inner_border]) <= 0:
+                                break
+
+                        width_left = margin + 1
+
+                        for margin in range(100 + 1):
+                            inner_border = (col + 1) + margin
+                            outer_border = (col + 2) + margin
+
+                            # outside image or intensity increasing from left to right
+                            if outer_border >= img_width or (image[row, outer_border] - image[row, inner_border]) >= 0:
+                                break
+
+                        width_right = margin + 1
+
+                        edge_widths[row, col] = width_left + width_right
+
+
+                    # gradient angle = 0
+                    if quantized_angles[row, col] == 0:
+                        for margin in range(100 + 1):
+                            inner_border = (col - 1) - margin
+                            outer_border = (col - 2) - margin
+
+                            # outside image or intensity decreasing from left to right
+                            if outer_border < 0 or (image[row, outer_border] - image[row, inner_border]) >= 0:
+                                break
+
+                        width_left = margin + 1
+
+                        for margin in range(100 + 1):
+                            inner_border = (col + 1) + margin
+                            outer_border = (col + 2) + margin
+
+                            # outside image or intensity decreasing from left to right
+                            if outer_border >= img_width or (image[row, outer_border] - image[row, inner_border]) <= 0:
+                                break
+
+                        width_right = margin + 1
+
+                        edge_widths[row, col] = width_right + width_left
+
+    return edge_widths
+
+
+def _calculate_sharpness_metric(image, edges, edge_widths):
+    # type: (numpy.array, numpy.array, numpy.array) -> numpy.float64
+
+    # get the size of image
+    img_height, img_width = image.shape
+
+    total_num_edges = 0
+    hist_pblur = np.zeros(101)
+
+    # maximum block indices
+    num_blocks_vertically = int(img_height / BLOCK_HEIGHT)
+    num_blocks_horizontally = int(img_width / BLOCK_WIDTH)
+
+    #  loop over the blocks
+    for i in range(num_blocks_vertically):
+        for j in range(num_blocks_horizontally):
+
+            # get the row and col indices for the block pixel positions
+            rows = slice(BLOCK_HEIGHT * i, BLOCK_HEIGHT * (i + 1))
+            cols = slice(BLOCK_WIDTH * j, BLOCK_WIDTH * (j + 1))
+
+            if is_edge_block(edges[rows, cols], THRESHOLD):
+                block_widths = edge_widths[rows, cols]
+                # rotate block to simulate column-major boolean indexing
+                block_widths = np.rot90(np.flipud(block_widths), 3)
+                block_widths = block_widths[block_widths != 0]
+
+                block_contrast = get_block_contrast(image[rows, cols])
+                block_jnb = WIDTH_JNB[block_contrast]
+
+                # calculate the probability of blur detection at the edges
+                # detected in the block
+                prob_blur_detection = 1 - np.exp(-abs(block_widths/block_jnb) ** BETA)
+
+                # update the statistics using the block information
+                for probability in prob_blur_detection:
+                    bucket = int(round(probability * 100))
+                    hist_pblur[bucket] += 1
+                    total_num_edges += 1
+
+    # normalize the pdf
+    if total_num_edges > 0:
+        hist_pblur = hist_pblur / total_num_edges
+
+    # calculate the sharpness metric
+    return np.sum(hist_pblur[:64])
+
+
+def is_edge_block(block, threshold):
+    # type: (numpy.ndarray, float) -> bool
+    """Decide whether the given block is an edge block."""
+    return np.count_nonzero(block) > (block.size * threshold)
+
+
+def get_block_contrast(block):
+    # type: (numpy.ndarray) -> int
+    return int(np.max(block) - np.min(block))
+
+
+if __name__ == '__main__':
+    input_image = imread(argv[1], pilmode = 'L')
+    sharpness = compute(input_image)
+    print('CPBD sharpness for %s: %f' % (argv[1], sharpness))
```

### Comparing `agh_vqis-2.0.4/python-cpbd/cpbd/octave.py` & `agh_vqis-2.0.5/python-cpbd/cpbd/octave.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-# coding: utf-8
-
-from __future__ import (
-    absolute_import,
-    division,
-    print_function,
-    unicode_literals,
-)
-
-import numpy as np
-from scipy.ndimage import convolve
-from skimage.filters.edges import HSOBEL_WEIGHTS
-
-
-def sobel(image):
-    # type: (numpy.ndarray) -> numpy.ndarray
-    """
-    Find edges using the Sobel approximation to the derivatives.
-
-    Inspired by the [Octave implementation](https://sourceforge.net/p/octave/image/ci/default/tree/inst/edge.m#l196).
-    """
-
-    h1 = np.array(HSOBEL_WEIGHTS)
-    h1 /= np.sum(abs(h1))  # normalize h1
-
-    strength2 = np.square(convolve(image, h1.T))
-
-    # Note: https://sourceforge.net/p/octave/image/ci/default/tree/inst/edge.m#l59
-    thresh2 = 2 * np.sqrt(np.mean(strength2))
-
-    strength2[strength2 <= thresh2] = 0
-    return _simple_thinning(strength2)
-
-
-def _simple_thinning(strength):
-    # type: (numpy.ndarray) -> numpy.ndarray
-    """
-    Perform a very simple thinning.
-
-    Inspired by the [Octave implementation](https://sourceforge.net/p/octave/image/ci/default/tree/inst/edge.m#l512).
-    """
-    num_rows, num_cols = strength.shape
-
-    zero_column = np.zeros((num_rows, 1))
-    zero_row = np.zeros((1, num_cols))
-
-    x = (
-        (strength > np.c_[zero_column, strength[:, :-1]]) &
-        (strength > np.c_[strength[:, 1:], zero_column])
-    )
-
-    y = (
-        (strength > np.r_[zero_row, strength[:-1, :]]) &
-        (strength > np.r_[strength[1:, :], zero_row])
-    )
-
-    return x | y
-
-
+# coding: utf-8
+
+from __future__ import (
+    absolute_import,
+    division,
+    print_function,
+    unicode_literals,
+)
+
+import numpy as np
+from scipy.ndimage import convolve
+from skimage.filters.edges import HSOBEL_WEIGHTS
+
+
+def sobel(image):
+    # type: (numpy.ndarray) -> numpy.ndarray
+    """
+    Find edges using the Sobel approximation to the derivatives.
+
+    Inspired by the [Octave implementation](https://sourceforge.net/p/octave/image/ci/default/tree/inst/edge.m#l196).
+    """
+
+    h1 = np.array(HSOBEL_WEIGHTS)
+    h1 /= np.sum(abs(h1))  # normalize h1
+
+    strength2 = np.square(convolve(image, h1.T))
+
+    # Note: https://sourceforge.net/p/octave/image/ci/default/tree/inst/edge.m#l59
+    thresh2 = 2 * np.sqrt(np.mean(strength2))
+
+    strength2[strength2 <= thresh2] = 0
+    return _simple_thinning(strength2)
+
+
+def _simple_thinning(strength):
+    # type: (numpy.ndarray) -> numpy.ndarray
+    """
+    Perform a very simple thinning.
+
+    Inspired by the [Octave implementation](https://sourceforge.net/p/octave/image/ci/default/tree/inst/edge.m#l512).
+    """
+    num_rows, num_cols = strength.shape
+
+    zero_column = np.zeros((num_rows, 1))
+    zero_row = np.zeros((1, num_cols))
+
+    x = (
+        (strength > np.c_[zero_column, strength[:, :-1]]) &
+        (strength > np.c_[strength[:, 1:], zero_column])
+    )
+
+    y = (
+        (strength > np.r_[zero_row, strength[:-1, :]]) &
+        (strength > np.r_[strength[1:, :], zero_row])
+    )
+
+    return x | y
+
+
```

### Comparing `agh_vqis-2.0.4/setup.cfg` & `agh_vqis-2.0.5/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,82 +1,80 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 2061 6768 5f76 7169 730d 0a76 6572   = agh_vqis..ver
-00000020: 7369 6f6e 203d 2032 2e30 2e34 0d0a 6175  sion = 2.0.4..au
-00000030: 7468 6f72 203d 204a 616b 7562 204e 6177  thor = Jakub Naw
-00000040: 61c5 8261 2c20 4669 6c69 7020 4b6f 7275  a..a, Filip Koru
-00000050: 730d 0a61 7574 686f 725f 656d 6169 6c20  s..author_email 
-00000060: 3d20 6a61 6b75 622e 6e61 7761 6c61 4061  = jakub.nawala@a
-00000070: 6768 2e65 6475 2e70 6c2c 2066 6b6f 7275  gh.edu.pl, fkoru
-00000080: 7340 7374 7564 656e 742e 6167 682e 6564  s@student.agh.ed
-00000090: 752e 706c 0d0a 6465 7363 7269 7074 696f  u.pl..descriptio
-000000a0: 6e20 3d20 4120 5079 7468 6f6e 2077 7261  n = A Python wra
-000000b0: 7070 6572 2066 6f72 2031 3820 696d 6167  pper for 18 imag
-000000c0: 6520 7175 616c 6974 7920 696e 6469 6361  e quality indica
-000000d0: 746f 7273 2e0d 0a6c 6f6e 675f 6465 7363  tors...long_desc
-000000e0: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
-000000f0: 5245 4144 4d45 2e6d 640d 0a6c 6f6e 675f  README.md..long_
-00000100: 6465 7363 7269 7074 696f 6e5f 636f 6e74  description_cont
-00000110: 656e 745f 7479 7065 203d 2074 6578 742f  ent_type = text/
-00000120: 6d61 726b 646f 776e 0d0a 7572 6c20 3d20  markdown..url = 
-00000130: 6874 7470 733a 2f2f 716f 652e 6167 682e  https://qoe.agh.
-00000140: 6564 752e 706c 2f69 6e64 6963 6174 6f72  edu.pl/indicator
-00000150: 732f 0d0a 6c69 6365 6e73 6520 3d20 4556  s/..license = EV
-00000160: 414c 5541 5449 4f4e 204c 4943 454e 5345  ALUATION LICENSE
-00000170: 2041 4752 4545 4d45 4e54 0d0a 6c69 6365   AGREEMENT..lice
-00000180: 6e73 655f 6669 6c65 7320 3d20 4c49 4345  nse_files = LICE
-00000190: 4e53 450d 0a63 6c61 7373 6966 6965 7273  NSE..classifiers
-000001a0: 203d 200d 0a09 5072 6f67 7261 6d6d 696e   = ...Programmin
-000001b0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000001c0: 7468 6f6e 203a 3a20 330d 0a09 5072 6f67  thon :: 3...Prog
-000001d0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-000001e0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-000001f0: 390d 0a09 5072 6f67 7261 6d6d 696e 6720  9...Programming 
-00000200: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000210: 6f6e 203a 3a20 332e 3130 0d0a 0950 726f  on :: 3.10...Pro
-00000220: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000230: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000240: 2e31 310d 0a09 4c69 6365 6e73 6520 3a3a  .11...License ::
-00000250: 204f 7468 6572 2f50 726f 7072 6965 7461   Other/Proprieta
-00000260: 7279 204c 6963 656e 7365 0d0a 094f 7065  ry License...Ope
-00000270: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
-00000280: 2050 4f53 4958 203a 3a20 4c69 6e75 780d   POSIX :: Linux.
-00000290: 0a09 4f70 6572 6174 696e 6720 5379 7374  ..Operating Syst
-000002a0: 656d 203a 3a20 4d69 6372 6f73 6f66 7420  em :: Microsoft 
-000002b0: 3a3a 2057 696e 646f 7773 0d0a 094f 7065  :: Windows...Ope
-000002c0: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
-000002d0: 204d 6163 4f53 0d0a 0949 6e74 656e 6465   MacOS...Intende
-000002e0: 6420 4175 6469 656e 6365 203a 3a20 5363  d Audience :: Sc
-000002f0: 6965 6e63 652f 5265 7365 6172 6368 0d0a  ience/Research..
-00000300: 0949 6e74 656e 6465 6420 4175 6469 656e  .Intended Audien
-00000310: 6365 203a 3a20 5465 6c65 636f 6d6d 756e  ce :: Telecommun
-00000320: 6963 6174 696f 6e73 2049 6e64 7573 7472  ications Industr
-00000330: 790d 0a09 546f 7069 6320 3a3a 204d 756c  y...Topic :: Mul
-00000340: 7469 6d65 6469 6120 3a3a 2056 6964 656f  timedia :: Video
-00000350: 0d0a 0954 6f70 6963 203a 3a20 5363 6965  ...Topic :: Scie
-00000360: 6e74 6966 6963 2f45 6e67 696e 6565 7269  ntific/Engineeri
-00000370: 6e67 203a 3a20 496d 6167 6520 5072 6f63  ng :: Image Proc
-00000380: 6573 7369 6e67 0d0a 0d0a 5b6f 7074 696f  essing....[optio
-00000390: 6e73 5d0d 0a70 6163 6b61 6765 5f64 6972  ns]..package_dir
-000003a0: 203d 2061 6768 5f76 7169 733d 7372 632f   = agh_vqis=src/
-000003b0: 6167 685f 7671 6973 2c63 7062 643d 7079  agh_vqis,cpbd=py
-000003c0: 7468 6f6e 2d63 7062 642f 6370 6264 0d0a  thon-cpbd/cpbd..
-000003d0: 7079 7468 6f6e 5f72 6571 7569 7265 7320  python_requires 
-000003e0: 3d20 3e3d 332e 390d 0a69 6e73 7461 6c6c  = >=3.9..install
-000003f0: 5f72 6571 7569 7265 7320 3d20 0d0a 096d  _requires = ...m
-00000400: 6174 706c 6f74 6c69 623e 3d33 2e35 2e31  atplotlib>=3.5.1
-00000410: 0d0a 096e 756d 7079 3e3d 312e 3232 2e33  ...numpy>=1.22.3
-00000420: 0d0a 0970 616e 6461 733e 3d31 2e34 2e32  ...pandas>=1.4.2
-00000430: 0d0a 0950 494d 533e 3d30 2e35 0d0a 0973  ...PIMS>=0.5...s
-00000440: 6369 6b69 742d 696d 6167 653e 3d30 2e31  cikit-image>=0.1
-00000450: 392e 320d 0a09 736c 6963 6572 6174 6f72  9.2...slicerator
-00000460: 3e3d 312e 312e 300d 0a09 7363 656e 6564  >=1.1.0...scened
-00000470: 6574 6563 743e 3d30 2e36 2e30 2e33 0d0a  etect>=0.6.0.3..
-00000480: 096f 7065 6e63 762d 7079 7468 6f6e 3e3d  .opencv-python>=
-00000490: 342e 362e 302e 3636 0d0a 0978 6762 6f6f  4.6.0.66...xgboo
-000004a0: 7374 3d3d 302e 3930 0d0a 0973 6369 6b69  st==0.90...sciki
-000004b0: 742d 6c65 6172 6e3d 3d31 2e30 2e32 0d0a  t-learn==1.0.2..
-000004c0: 0961 763e 3d38 2e30 2e33 0d0a 0d0a 5b6f  .av>=8.0.3....[o
-000004d0: 7074 696f 6e73 2e70 6163 6b61 6765 5f64  ptions.package_d
-000004e0: 6174 615d 0d0a 2a20 3d20 2a0d 0a0d 0a5b  ata]..* = *....[
-000004f0: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
-00000500: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
-00000510: 6520 3d20 300d 0a0d 0a                   e = 0....
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 6167 685f 7671 6973 0a76 6572 7369  = agh_vqis.versi
+00000020: 6f6e 203d 2032 2e30 2e35 0a61 7574 686f  on = 2.0.5.autho
+00000030: 7220 3d20 4a61 6b75 6220 4e61 7761 c582  r = Jakub Nawa..
+00000040: 612c 2046 696c 6970 204b 6f72 7573 0a61  a, Filip Korus.a
+00000050: 7574 686f 725f 656d 6169 6c20 3d20 6a61  uthor_email = ja
+00000060: 6b75 622e 6e61 7761 6c61 4061 6768 2e65  kub.nawala@agh.e
+00000070: 6475 2e70 6c2c 2066 6b6f 7275 7340 7374  du.pl, fkorus@st
+00000080: 7564 656e 742e 6167 682e 6564 752e 706c  udent.agh.edu.pl
+00000090: 0a64 6573 6372 6970 7469 6f6e 203d 2041  .description = A
+000000a0: 2050 7974 686f 6e20 7772 6170 7065 7220   Python wrapper 
+000000b0: 666f 7220 3138 2069 6d61 6765 2071 7561  for 18 image qua
+000000c0: 6c69 7479 2069 6e64 6963 6174 6f72 732e  lity indicators.
+000000d0: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
+000000e0: 6e20 3d20 6669 6c65 3a20 5245 4144 4d45  n = file: README
+000000f0: 2e6d 640a 6c6f 6e67 5f64 6573 6372 6970  .md.long_descrip
+00000100: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
+00000110: 6520 3d20 7465 7874 2f6d 6172 6b64 6f77  e = text/markdow
+00000120: 6e0a 7572 6c20 3d20 6874 7470 733a 2f2f  n.url = https://
+00000130: 716f 652e 6167 682e 6564 752e 706c 2f69  qoe.agh.edu.pl/i
+00000140: 6e64 6963 6174 6f72 732f 0a6c 6963 656e  ndicators/.licen
+00000150: 7365 203d 2045 5641 4c55 4154 494f 4e20  se = EVALUATION 
+00000160: 4c49 4345 4e53 4520 4147 5245 454d 454e  LICENSE AGREEMEN
+00000170: 540a 6c69 6365 6e73 655f 6669 6c65 7320  T.license_files 
+00000180: 3d20 4c49 4345 4e53 450a 636c 6173 7369  = LICENSE.classi
+00000190: 6669 6572 7320 3d20 0a09 5072 6f67 7261  fiers = ..Progra
+000001a0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+000001b0: 3a20 5079 7468 6f6e 203a 3a20 330a 0950  : Python :: 3..P
+000001c0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+000001d0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+000001e0: 2033 2e39 0a09 5072 6f67 7261 6d6d 696e   3.9..Programmin
+000001f0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000200: 7468 6f6e 203a 3a20 332e 3130 0a09 5072  thon :: 3.10..Pr
+00000210: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000220: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000230: 332e 3131 0a09 4c69 6365 6e73 6520 3a3a  3.11..License ::
+00000240: 204f 7468 6572 2f50 726f 7072 6965 7461   Other/Proprieta
+00000250: 7279 204c 6963 656e 7365 0a09 4f70 6572  ry License..Oper
+00000260: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
+00000270: 504f 5349 5820 3a3a 204c 696e 7578 0a09  POSIX :: Linux..
+00000280: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
+00000290: 203a 3a20 4d69 6372 6f73 6f66 7420 3a3a   :: Microsoft ::
+000002a0: 2057 696e 646f 7773 0a09 4f70 6572 6174   Windows..Operat
+000002b0: 696e 6720 5379 7374 656d 203a 3a20 4d61  ing System :: Ma
+000002c0: 634f 530a 0949 6e74 656e 6465 6420 4175  cOS..Intended Au
+000002d0: 6469 656e 6365 203a 3a20 5363 6965 6e63  dience :: Scienc
+000002e0: 652f 5265 7365 6172 6368 0a09 496e 7465  e/Research..Inte
+000002f0: 6e64 6564 2041 7564 6965 6e63 6520 3a3a  nded Audience ::
+00000300: 2054 656c 6563 6f6d 6d75 6e69 6361 7469   Telecommunicati
+00000310: 6f6e 7320 496e 6475 7374 7279 0a09 546f  ons Industry..To
+00000320: 7069 6320 3a3a 204d 756c 7469 6d65 6469  pic :: Multimedi
+00000330: 6120 3a3a 2056 6964 656f 0a09 546f 7069  a :: Video..Topi
+00000340: 6320 3a3a 2053 6369 656e 7469 6669 632f  c :: Scientific/
+00000350: 456e 6769 6e65 6572 696e 6720 3a3a 2049  Engineering :: I
+00000360: 6d61 6765 2050 726f 6365 7373 696e 670a  mage Processing.
+00000370: 0a5b 6f70 7469 6f6e 735d 0a70 6163 6b61  .[options].packa
+00000380: 6765 5f64 6972 203d 2061 6768 5f76 7169  ge_dir = agh_vqi
+00000390: 733d 7372 632f 6167 685f 7671 6973 2c63  s=src/agh_vqis,c
+000003a0: 7062 643d 7079 7468 6f6e 2d63 7062 642f  pbd=python-cpbd/
+000003b0: 6370 6264 0a70 7974 686f 6e5f 7265 7175  cpbd.python_requ
+000003c0: 6972 6573 203d 203e 3d33 2e39 0a69 6e73  ires = >=3.9.ins
+000003d0: 7461 6c6c 5f72 6571 7569 7265 7320 3d20  tall_requires = 
+000003e0: 0a09 6d61 7470 6c6f 746c 6962 3e3d 332e  ..matplotlib>=3.
+000003f0: 352e 310a 096e 756d 7079 3e3d 312e 3232  5.1..numpy>=1.22
+00000400: 2e33 0a09 7061 6e64 6173 3e3d 312e 342e  .3..pandas>=1.4.
+00000410: 320a 0950 494d 533e 3d30 2e35 0a09 7363  2..PIMS>=0.5..sc
+00000420: 696b 6974 2d69 6d61 6765 3e3d 302e 3139  ikit-image>=0.19
+00000430: 2e32 0a09 736c 6963 6572 6174 6f72 3e3d  .2..slicerator>=
+00000440: 312e 312e 300a 0973 6365 6e65 6465 7465  1.1.0..scenedete
+00000450: 6374 3e3d 302e 362e 302e 330a 096f 7065  ct>=0.6.0.3..ope
+00000460: 6e63 762d 7079 7468 6f6e 3e3d 342e 362e  ncv-python>=4.6.
+00000470: 302e 3636 0a09 7867 626f 6f73 743d 3d30  0.66..xgboost==0
+00000480: 2e39 300a 0973 6369 6b69 742d 6c65 6172  .90..scikit-lear
+00000490: 6e3d 3d31 2e30 2e32 0a09 6176 3e3d 382e  n==1.0.2..av>=8.
+000004a0: 302e 330a 0966 666d 7065 672d 7079 7468  0.3..ffmpeg-pyth
+000004b0: 6f6e 3e3d 302e 322e 300a 0a5b 6f70 7469  on>=0.2.0..[opti
+000004c0: 6f6e 732e 7061 636b 6167 655f 6461 7461  ons.package_data
+000004d0: 5d0a 2a20 3d20 2a0a 0a5b 6567 675f 696e  ].* = *..[egg_in
+000004e0: 666f 5d0a 7461 675f 6275 696c 6420 3d20  fo].tag_build = 
+000004f0: 0a74 6167 5f64 6174 6520 3d20 300a 0a    .tag_date = 0..
```

### Comparing `agh_vqis-2.0.4/src/agh_vqis/12k_all_set.json` & `agh_vqis-2.0.5/src/agh_vqis/models/ugc/12k_all_set.json`

 * *Files identical despite different names*

### Comparing `agh_vqis-2.0.4/src/agh_vqis/9k_all_set.json` & `agh_vqis-2.0.5/src/agh_vqis/models/ugc/9k_all_set.json`

 * *Files identical despite different names*

### Comparing `agh_vqis-2.0.4/src/agh_vqis/__main__.py` & `agh_vqis-2.0.5/src/agh_vqis/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,126 +1,71 @@
-# Author: Jakub Nawała <jnawala@agh.edu.pl>
+# Authors: Jakub Nawała <jnawala@agh.edu.pl>, Filip Korus <fkorus@student.agh.edu.pl>
 # Created: June 1, 2021
-import xml.dom
-from pathlib import Path
+import argparse
+import logging
+
 import numpy as np
-import pims
-from ._logger import setup_console_and_file_logger
-from subprocess import PIPE, STDOUT, Popen
-import re
-import shutil
 import pandas as pd
-from pims import PyAVVideoReader
-import argparse
-from enum import Enum
+import pims
 from cpbd.compute import compute
-import platform
-import sys
-import logging
-from .utils import utils
-from .ugc import ugc
+from pims import PyAVVideoReader
 
+from ._logger import setup_console_and_file_logger
+from .utils import ugc
+from .utils.helpers import *
 
 logger = setup_console_and_file_logger(__name__, log_file_name=f"{__name__}.log", level=logging.INFO)
-single_file_script_path = Path(
-    '/'.join(__file__.split('/')[:-1]) if platform.system() != 'Windows' else '\\'.join(__file__.split('\\')[:-1]),
-    f'mitsu_single_file.{"sh" if platform.system() != "Windows" else "bat"}'
-)
-
-
-class Results(Enum):
-    """
-    Makes it less error-prone to index a dictionary with objects storing IQIs results
-    """
-    BLUR_AMOUNT = 1
-    COLOURFULNESS = 2
-    UGC = 3
-    VQIS = 4
-
-
-def _get_mm_file_properties(path: Path):
-    """
-    Get properties of a multimedia (MM) file identified by *path*.
-
-    :param path: path to a video or image file from which to extract properties
-    :return: a 3-tuple: (i) MM file width, (ii) MM file height and (iii) the number of frames (0 for images)
-    """
-    # Try to read as a video file first
-    try:
-        video = PyAVVideoReader(str(path))
-    except (OSError, TypeError):
-        # Try to read as an image file instead
-        image = pims.open(str(path))
-        nb_frames = 0
-        img_w = image.frame_shape[0]  # 0th index -> no. of rows (=height), 1st index -> no. of columns (=width)
-        img_h = image.frame_shape[1]  # img = image
-        return img_w, img_h, nb_frames
-
-    logger.debug(f"The input video has the duration of {video.duration} seconds.")
 
-    nb_frames = len(video)
-    logger.debug(f"The input video has {nb_frames} frames.")
-    video_w = video.frame_shape[1]  # 0th index -> no. of rows (=height), 1st index -> no. of columns (=width)
-    video_h = video.frame_shape[0]
+allowed_mm_file_extensions = ['.jpg', '.jpeg', '.png', '.ts', '.mp4', '.y4m', '.mov', '.avi', '.mkv', '.gif', '.bmp']
 
-    return video_w, video_h, nb_frames
 
-
-def _run_agh_viqs(mm_file_path: Path, script_path: Path, binary_path: Path, selected_vqis=32767,
-                  bash_path=Path("/bin/bash")):
+def _run_agh_viqs(mm_file_path: Path, binary_path: Path, selected_vqis=32767):
     """
     Runs 15 VQ AGH's Video Quality Indicators (VQIs) on an input video or image (identified by *video_path*) and returns
     Pandas DataFrame with results.
 
     :param mm_file_path: path to a video or image file to process
-    :param script_path: path to a VQIs calculation automation script
     :param binary_path: path to a binary executable computing VQIs
     :param selected_vqis: a positive 16-bit integer stating which VQIs to run (all are run by default)
-    :param bash_path: a path to a BASH interpreter that should be used to run the AGH VQIs
     :return: Pandas DataFrame with VQIs results or -1 if an error occurred
     """
-    if bash_path is None:
-        bash_path = Path("/bin/bash")
+
     if binary_path is None:
-        binary_path = Path('\\'.join(__file__.split('\\')[:-1]),
-                           'mitsuWin64_multithread.exe') if platform.system() == 'Windows' else Path(
-            '/'.join(__file__.split('/')[:-1]),
-            'agh_vqis_binary_x86_mt' if platform.system() == 'Linux' else 'agh_vqis_binary_macosx_mt')
-    # sfs --- single file script
-    sfs_call_elems = [str(bash_path), str(script_path.resolve()), str(mm_file_path.resolve()),
-                      str(binary_path.resolve()), str(selected_vqis)]
-    try:
-        # completed_sfs_run = run(sfs_call, check=True, shell=True, stdout=PIPE, stderr=STDOUT)
-        sfs_popen = Popen(sfs_call_elems if platform.system() != 'Windows' else sfs_call_elems[1:], stdout=PIPE,
-                          stderr=STDOUT)
-        sfs_stdout, sfs_stderr = sfs_popen.communicate()  # wait for the VQIs to finish
-    except OSError as e:
-        logger.error(f"Calling the {str(script_path)} script failed with the following message: {e}")
-        return -1
-    if sfs_popen.returncode != 0:
-        logger.error(f"Calling the {str(script_path)} script failed with the following return code: "
-                     f"{sfs_popen.returncode}")
-        logger.error(f"{str(script_path)}\'s output: {sfs_stdout.decode('ascii')}")
+        executable_file = get_executable_filename()
+        binary_path = Path('/'.join(__file__.split('/')[:-1]) if platform.system() != 'Windows' else '\\'.join(__file__.split('\\')[:-1]), 'binaries/', executable_file)
+
+    if not os.access(binary_path.resolve(), os.X_OK):
+        logger.error(f'{str(binary_path.resolve())} file is not executable')
         return -1
-    logger.debug(f"The {script_path} script was successfully executed")
 
-    # Read the results from a proper CSV file and remove leftovers (ffmpeg log & the CSV file with results)
-    results_folder_name_match = re.search(r"VQIs-results-\d{4}-\d{2}-\d{2}",
-                                          sfs_stdout.decode("ascii"))
-    csv_filename_match = re.search(r"results-.+\.csv", sfs_stdout.decode("ascii"))
-    assert results_folder_name_match is not None
-    assert csv_filename_match is not None
-    folder_name = results_folder_name_match.group()
-    csv_filename = csv_filename_match.group().replace('"', '')
+    logger.debug('Creating working directory')
+    random_folder_name = generate_uuid()
+    mkdir(random_folder_name)
+    yuv_file_path = Path(random_folder_name, mm_file_path.stem + '.yuv')
+
+    logger.debug(f'Converting {str(mm_file_path.resolve())} to yuv format')
+    convert_to_yuv(mm_file_path, yuv_file_path)
+
+    video_width, video_height, _, FPS = get_mm_file_properties(mm_file_path)
+
+    logger.debug('Calling VQIs binary file')
+
+    sfs_call_elems = [str(binary_path.resolve()), str(yuv_file_path.resolve()), str(video_width), str(video_height), str(selected_vqis), str(FPS)]
+    system_call(sfs_call_elems, logger)
+
+    logger.debug(f'{sfs_call_elems[0]} binary file was successfully executed')
+
+    vqis_csv_path = Path(random_folder_name, mm_file_path.stem + '.csv')
+
+    mv_file(Path('./metricsResultsCSV.csv').resolve(), vqis_csv_path.resolve())
 
-    vqis_csv_path = Path(folder_name) / Path(csv_filename)
-    vqis_res_df = pd.read_csv(vqis_csv_path, sep=r"\s+")
+    vqis_res_df = pd.read_csv(vqis_csv_path, sep=r'\s+')
 
-    logger.debug("Removing leftovers")
-    shutil.rmtree(folder_name, ignore_errors=True)
+    logger.debug('Removing working directory')
+    rmdir(random_folder_name)
 
     return vqis_res_df
 
 
 def _colourfulness(frame: np.ndarray):
     """
     Runs Colourfulness image quality indicator (IQI) on a single video frame (see the *frame* parameter). Returns
@@ -237,24 +182,24 @@
         blur_amount = _blur_amount(frame)
         logger.debug(f"Blur Amount IQI for the {frame.frame_no}-th frame: {blur_amount:.5f}")
         blur_amount_s.loc[frame.frame_no] = blur_amount
     return blur_amount_s
 
 
 def _ugc(in_path: Path, results_vqis: pd.DataFrame):
-    FPS = utils.get_FPS(str(in_path))
+    _, _, FPS, _ = get_mm_file_properties(in_path)
 
     # Get a list of shots
-    scene_list_out = utils.find_scenes(str(in_path))
+    scene_list_out = ugc.find_scenes(str(in_path))
 
     if len(scene_list_out) == 0:
         return None
 
-    shots_data = utils.get_shots_data(scene_list_out, results_vqis)
-    shots_data = ugc(results_vqis, shots_data)
+    shots_data = ugc.get_shots_data(scene_list_out, results_vqis)
+    shots_data = ugc.ugc(results_vqis, shots_data)
 
     return [{
         'range_start': int(item['frames_range'].split(', ')[0]) - 1,
         'range_end': int(item['frames_range'].split(', ')[1]) - 1,
         'ugc': item['ugc']
     } for item in shots_data]
 
@@ -309,46 +254,14 @@
 
     res.columns = res.columns.str.replace(':', '')
     res.to_csv(out_filename, index=False)
     logger.info(f"All results stored in the {out_filename} file")
     return
 
 
-def _get_selected_vqis(options: dict) -> int:
-    vqis = {
-        'blockiness': 1,
-        'sa': 2,
-        'letterbox': 4,
-        'pillarbox': 8,
-        'blockloss': 16,
-        'blur': 32,
-        'ta': 64,
-        'blackout': 128,
-        'freezing': 256,
-        'exposure': 512,
-        'contrast': 1024,
-        'interlace': 2048,
-        'noise': 4096,
-        'slice': 8192,
-        'flickering': 16384
-    }
-
-    # selected_vqis = sum(vqis.values())
-    selected_vqis = 32767  # select all by default
-
-    for key, value in options.items():
-        if not value:
-            try:
-                selected_vqis -= vqis[key]  # remove vqis
-            except KeyError:
-                pass
-
-    return selected_vqis
-
-
 def parse_user_input(cli: bool = False, options: dict = {}):
     """
     Parses user input (as provided through the command line).
 
     :return: nothing yet
     """
     parser = argparse.ArgumentParser(description="Computes image quality indicators (IQIs) for the input image or for"
@@ -376,16 +289,14 @@
                                              " the 16-bit positive integer): Blockiness (1), SA (2), Letterbox (4),"
                                              " Pillarbox (8), Blockloss (16), Blur (32), TA (64), Blackout (128),"
                                              " Freezing (256), Exposure (512), Contrast (1024), Interlace (2048),"
                                              " Noise (4096), Slice (8192) and Flickering (16384)."
                                              " Please note that you can provide a value for the VQIS parameter"
                                              " in the form of a hexadecimal number."
                                              " For example, 0x7FFF means running all VQIs.")
-    parser.add_argument("-s", "--shell", help="asks to run an alternative Bash interpreter (instead of the default "
-                                              "/bin/bash). Provide here a path to the interpreter of your choice.")
     parser.add_argument("-e", "--exec", help="provide here the path to the binary file running 15 AGH VQIs. The "
                                              "default is to use the agh_vqis_binary_x86_mt binary contained in the "
                                              "repo.", type=Path)
     args = parser.parse_args()
     # Run 15 AGH VQIs if no VQIs were selected
     if cli and not args.vqis:
         logger.info("No IQIs were selected. Running 15 AGH VQIs only.")
@@ -397,79 +308,87 @@
     """
     Processes single multimedia file (image or video).
 
     :param in_path: path to an input file to process
     :param options: options for executable file
     :return: status, 0 if successful, 1 otherwise
     """
-    # Read properties of an input multimedia file
+
     if args is None:
         args = parse_user_input(cli, options)
 
-    in_mm_file_w, in_mm_file_h, nb_frames = _get_mm_file_properties(in_path)
+    if not in_path.exists():
+        logger.error(f'{str(in_path)} file does not exists')
+        return -1
+
+    mm_file_ext = in_path.suffix
+    if mm_file_ext not in allowed_mm_file_extensions:
+        logger.error(f'{mm_file_ext} file extension is not supported')
+        return -1
+
+    # Read properties of an input multimedia file
+    in_mm_file_w, in_mm_file_h, nb_frames, frame_rate = get_mm_file_properties(in_path)
     is_input_video = True  # a flag making further processing logic easier to comprehend
     if nb_frames == 0:
         is_input_video = False
 
     # Prepare a dictionary in which to store objects with IQIs results
     results = {}
 
     # Run Blur Amount IQI on the input video or image (if requested)
-    if ('blur_amount' in options and options['blur_amount']) or args.blur_amount:
-        logger.info(f"Running the Blur Amount IQI on the input ({str(in_path)})")
+    if (VQIs.blur_amount in options and options[VQIs.blur_amount]) or args.blur_amount:
+        logger.info(f"Running the Blur Amount IQI on the input ({str(in_path.resolve())})")
         blur_amount_s = get_blur_amount_iqi(in_path, is_video=is_input_video)
         blur_amount_s.name = "Blur_amount"
         results.update({Results.BLUR_AMOUNT: blur_amount_s})
 
     # Run Colorfulness indicator on the input video or image (if requested)
-    if args.colourfulness or (not cli and 'colourfulness' not in options) or (
-            not cli and 'colourfulness' in options and options['colourfulness']):
-        logger.info(f"Running the Colourfulness IQI on the input ({str(in_path)})")
+    if args.colourfulness or (not cli and VQIs.colourfulness not in options) or (
+            not cli and VQIs.colourfulness in options and options[VQIs.colourfulness]):
+        logger.info(f"Running the Colourfulness IQI on the input ({str(in_path.resolve())})")
         # s --- series
         colourfulness_s = get_colourfulness_iqi(in_path, is_video=is_input_video)
         colourfulness_s.name = "Colourfulness"
         results.update({Results.COLOURFULNESS: colourfulness_s})
 
     run_UGC = False
-    if is_input_video and (args.ugc or (not cli and 'ugc' not in options) or (
-            not cli and 'ugc' in options and options['ugc'])):
+    if is_input_video and (args.ugc or (not cli and VQIs.ugc not in options) or (
+            not cli and VQIs.ugc in options and options[VQIs.ugc])):
         run_UGC = True
-        options['TA'] = True  # UGC indicator requires TA
-        options['SA'] = True  # and SA IQIs
+        options[VQIs.TA] = True  # UGC indicator requires TA
+        options[VQIs.SA] = True  # and SA IQIs
 
     if cli and args.vqis:
         vqis_selected = int(args.vqis, base=0)  # parse optional hexadecimal input
 
     if not cli:
-        vqis_selected = _get_selected_vqis(options)
+        vqis_selected = get_selected_vqis(options)
 
     vqis_res_df = None
     # Run the mitsu_single_file.sh script on the input video or image (if requested)
     if not cli or args.vqis:
-        logger.info(f"Running requested AGH VQIs on the input ({str(in_path)})")
+        logger.info(f"Running requested AGH VQIs on the input ({str(in_path.resolve())})")
         agh_vqis_path = Path(options['exec']) if ('exec' in options and options['exec']) else args.exec
-        vqis_res_df = _run_agh_viqs(in_path, single_file_script_path, agh_vqis_path, vqis_selected,
-                                    bash_path=(Path(args.shell) if args.shell is not None else (
-                                        Path(options['shell']) if ('shell' in options and options['shell']) else None)))
+        vqis_res_df = _run_agh_viqs(in_path, agh_vqis_path, vqis_selected)
         if type(vqis_res_df) is not pd.DataFrame:  # Running the VQIs failed
             return -1
 
         if (len(vqis_res_df) != int(nb_frames)) and is_input_video:
             logger.warning(
-                f"For some reason the number of frames read by PIMS does not match the number of frames read "
-                f"by {str(single_file_script_path)}. You may want to check whether the results are valid.")
+                f"For some reason the number of frames read by ffmpeg-python does not match the number of frames read "
+                f"by binary file. You may want to check whether the results are valid.")
             logger.warning(f"This is the difference in the number of frames as indicated by the two methods: "
                            f"{np.abs(len(vqis_res_df) - int(nb_frames))}")
 
     if run_UGC:
-        logger.info(f"Running the UGC IQI on the input ({str(in_path)})")
+        logger.info(f"Running the UGC IQI on the input ({str(in_path.resolve())})")
         # s --- series
         # print(results)
 
-        ugc_s = get_ugc_iqi(in_path, nb_frames, vqis_res_df)
+        ugc_s = get_ugc_iqi(in_path, int(nb_frames), vqis_res_df)
         if ugc_s is None:
             logger.error(f"Error when running UGC IQI")
         else:
             ugc_s.name = "UGC"
             results.update({Results.UGC: ugc_s})
 
     if vqis_res_df is not None:
@@ -496,16 +415,15 @@
     for child in folder_path.iterdir():
         # Ignore subdirectories
         if child.is_dir():
             logger.info(f"Skipping a subdirectory ({str(child)})")
             continue
         # Ignore non-video and non-image files
         # TODO Add here any video or image extensions we want to support
-        if (child.suffix not in [".mp4", ".mov", ".avi", ".mkv", ".ts", ".y4m"]) and (
-                child.suffix not in [".png", ".jpg", ".jpeg", ".bmp", ".gif"]):
+        if (child.suffix not in allowed_mm_file_extensions):
             logger.info(f"Not a multimedia file ({str(child)}), skipping")
             continue
         # Process a single video file
         # TODO Consider adding functionality of keeping all results in a single CSV file (as done in the legacy BATCH
         #  file)
         mm_file_path = child  # mm = multimedia
         status = process_single_mm_file(mm_file_path, cli, options, args)
```

### Comparing `agh_vqis-2.0.4/src/agh_vqis/_logger.py` & `agh_vqis-2.0.5/src/agh_vqis/_logger.py`

 * *Files identical despite different names*

### Comparing `agh_vqis-2.0.4/src/agh_vqis/agh_vqis_binary_macosx_mt` & `agh_vqis-2.0.5/src/agh_vqis/binaries/agh_vqis_binary_macosx_mt`

 * *Files identical despite different names*

### Comparing `agh_vqis-2.0.4/src/agh_vqis/agh_vqis_binary_x86_mt` & `agh_vqis-2.0.5/src/agh_vqis/binaries/agh_vqis_binary_x86_mt`

 * *Files identical despite different names*

### Comparing `agh_vqis-2.0.4/src/agh_vqis/mitsuWin64_multithread.exe` & `agh_vqis-2.0.5/src/agh_vqis/binaries/agh_vqis_binary_win64_mt.exe`

 * *Files identical despite different names*

### Comparing `agh_vqis-2.0.4/src/agh_vqis/utils/utils.py` & `agh_vqis-2.0.5/src/agh_vqis/utils/ugc.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,75 +1,31 @@
 import sys
 import os
 import subprocess
 import csv
 import shutil
 import logging
 
+import pickle
+import xgboost as xgb
+import pandas as pd
+import numpy as np
+import platform
+from pathlib import Path
+
 # For content-aware scene detection:
 from scenedetect.detectors.content_detector import ContentDetector
 from scenedetect.scene_manager import SceneManager
 # For caching detection metrics and saving/loading to a stats file
 from scenedetect.stats_manager import StatsManager
 from scenedetect.video_manager import VideoManager
 
 # Disable scenedetect logging to prevent "VideoManager is deprecated and will be removed." message from showing
 logging.getLogger('pyscenedetect').disabled = True
 
-def get_resolution(video_path):
-    """
-    Gets the video resolution of a video using ffprobe
-    :param video_path: full path to the analysed video
-    :return: Tuple (width,height)
-    """
-    if not os.path.exists(video_path):
-        sys.stderr.write("ERROR: filename %r was not found!" % (video_path,))
-        return -1
-    out = subprocess.check_output(
-        ["ffprobe", video_path, "-v", "error", "-show_entries", "stream=width,height", "-of",  "default=noprint_wrappers=1"])
-    width = out.decode("utf-8").split('\n')[0].split('=')[1].split('\r')[0]
-    height = out.decode("utf-8").split('\n')[1].split('=')[1].split('\r')[0]
-    #print(width)
-    #print(height)
-    resolution = (width, height)
-    return resolution
-
-def get_FPS(video_path):
-    """
-    Calculates the FPS of the input video based on ffprobe.
-    Based on: https://askubuntu.com/questions/110264/how-to-find-frames-per-second-of-any-video-file
-    :param video_path: full path to the analysed video
-    :return: FPS value or -1 if not detected or file not found
-    """
-
-    if not os.path.exists(video_path):
-        sys.stderr.write("ERROR: filename %r was not found!" % (video_path,))
-        return -1
-    out = subprocess.check_output(
-        ["ffprobe", video_path, "-v", "0", "-select_streams", "v", "-print_format", "flat", "-show_entries",
-         "stream=r_frame_rate"])
-    rate = out.decode("utf-8").split('"')[1].split('/')
-    if len(rate) == 1:
-        return float(rate[0])
-    if len(rate) == 2:
-        return float(rate[0]) / float(rate[1])
-    return -1
-
-
-def my_system_call(call):
-    """
-    Executes the given string system call using subprocess package. Returns any errors risen by subprocess
-    to the console.
-    :param call: String system call
-    """
-    try:
-        subprocess.check_call(call, shell=True)
-    except subprocess.CalledProcessError as e:
-        print("ERROR: " + str(e.output))
-
 
 def find_scenes(video_path, threshold=30.0):
     """
     Detects scenes in the provided video file.
     :param video_path: full path to the analysed video
     :param threshold: threshold used by the pyscenedetect. Default 30.
     :return: List of detected scenes in the video
@@ -178,34 +134,51 @@
 
         ta_sum = 0
         sa_sum = 0
 
     return shots_data
 
 
-def make_dir(dir_name):
-    """
-    This function creates a directory
-    :param dir_name: Name of the directory to create
-    :return: Nothing
-    """
-    if not os.path.exists(dir_name):
-        os.makedirs(dir_name)
+def video_to_cuts(df, shots_data):
+    df = df.astype(float)
 
+    df['Frame:'] += 1
 
-def my_file_copy(src, dst):
-    """
-    This function copies a file from source to destination with exception handling
-    :param src: Source file
-    :param dst: Destination file
-    :return: Nothing
-    """
-    try:
-        shutil.copy(src, dst)
-    except shutil.Error as e:
-        print('Error: %s' % e)
-        print("Src: " + src + "Dst: " + dst)
-        exit()
-        exit()
-    except IOError as e:
-        print('Error: %s' % e.strerror)
-        print("Src: " + src + "Dst: " + dst)
+    data = []
+    cuts = pd.DataFrame()
+    for i in shots_data:
+        frame = i['frames_range'].replace(" ", "").split(",")
+        data.append(df.iloc[int(frame[0]):int(frame[1]),:].mean())
+
+    cuts = pd.DataFrame(data)
+    cuts = cuts[['Blockiness:', 'SA:', 'Blockloss:', 'Blur:', 'TA:',
+                    'Exposure(bri):', 'Contrast:', 'Noise:', 'Slice:', 'Flickering:']]
+    cuts.columns = ['Blockiness:', 'SA:', 'Blockloss:', 'Blur:', 'TA:',
+                    'Exposure(bri):', 'Contrast:', 'Noise:', 'Slice:', 'Flickering:']
+    return cuts, shots_data
+
+
+def ugc(df, shots_data):
+#  input path to files where shots data are in pickle format
+#  returns updated shots_data
+    cuts, shots_data = video_to_cuts(df, shots_data)
+
+    # 9k_all_set.json
+    # 12k_all_set.json
+    model_path = Path('/'.join(__file__.split('/')[:-1]) if platform.system() != 'Windows' else '\\'.join(__file__.split('\\')[:-1]), '../models/ugc/', '12k_all_set.json')
+
+    # model_path = Path('./model.bin')
+
+    xgb_cl = pickle.load(open(str(model_path), 'rb'))  # exception thrown
+    # pickle.dump(xgb_cl, open('model.bin', 'wb'))
+    # xgb_cl = xgb.XGBRFClassifier()
+    # xgb_cl.load_model(str(model_path))
+    for count, value in enumerate(shots_data):
+
+        X = cuts[count:count+1]
+        preds = xgb_cl.predict(X)
+
+        # print(X)
+        # print(preds[0])
+
+        value['ugc'] = 0 if int(preds[0]) == 1 else 1
+    return shots_data  # 0 => not UGC, 1 => UGC
```

