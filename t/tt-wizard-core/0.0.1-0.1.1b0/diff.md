# Comparing `tmp/tt_wizard_core-0.0.1.tar.gz` & `tmp/tt_wizard_core-0.1.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tt_wizard_core-0.0.1.tar", last modified: Fri Jun  2 16:06:24 2023, max compression
+gzip compressed data, was "tt_wizard_core-0.1.1b0.tar", last modified: Fri Jun  9 10:44:20 2023, max compression
```

## Comparing `tt_wizard_core-0.0.1.tar` & `tt_wizard_core-0.1.1b0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 bumblebee  (1000) bumblebee  (1000)        0 2023-06-02 16:06:24.432621 tt_wizard_core-0.0.1/
--rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)     1416 2023-06-02 15:56:33.000000 tt_wizard_core-0.0.1/Example.py
--rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)    35149 2023-06-02 07:39:27.000000 tt_wizard_core-0.0.1/LICENSE.txt
--rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)       84 2023-06-02 11:53:29.000000 tt_wizard_core-0.0.1/MANIFEST.in
--rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)     3874 2023-06-02 16:06:24.431621 tt_wizard_core-0.0.1/PKG-INFO
--rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)     2935 2023-06-02 15:56:29.000000 tt_wizard_core-0.0.1/README.md
--rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)       38 2023-06-02 16:06:24.432621 tt_wizard_core-0.0.1/setup.cfg
--rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)     1419 2023-06-02 16:05:37.000000 tt_wizard_core-0.0.1/setup.py
-drwxr-xr-x   0 bumblebee  (1000) bumblebee  (1000)        0 2023-06-02 16:06:24.429621 tt_wizard_core-0.0.1/src/
-drwxr-xr-x   0 bumblebee  (1000) bumblebee  (1000)        0 2023-06-02 16:06:24.431621 tt_wizard_core-0.0.1/src/tt_wizard_core.egg-info/
--rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)     3874 2023-06-02 16:06:24.000000 tt_wizard_core-0.0.1/src/tt_wizard_core.egg-info/PKG-INFO
--rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)      284 2023-06-02 16:06:24.000000 tt_wizard_core-0.0.1/src/tt_wizard_core.egg-info/SOURCES.txt
--rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)        1 2023-06-02 16:06:24.000000 tt_wizard_core-0.0.1/src/tt_wizard_core.egg-info/dependency_links.txt
--rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)       17 2023-06-02 16:06:24.000000 tt_wizard_core-0.0.1/src/tt_wizard_core.egg-info/requires.txt
--rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)       15 2023-06-02 16:06:24.000000 tt_wizard_core-0.0.1/src/tt_wizard_core.egg-info/top_level.txt
--rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)     3206 2023-06-02 14:46:44.000000 tt_wizard_core-0.0.1/src/tt_wizard_core.py
+drwxr-xr-x   0 bumblebee  (1000) bumblebee  (1000)        0 2023-06-09 10:44:20.483319 tt_wizard_core-0.1.1b0/
+-rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)     1853 2023-06-09 10:36:29.000000 tt_wizard_core-0.1.1b0/Example.py
+-rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)    35129 2023-06-02 16:17:46.000000 tt_wizard_core-0.1.1b0/LICENSE
+-rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)       84 2023-06-02 11:53:29.000000 tt_wizard_core-0.1.1b0/MANIFEST.in
+-rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)     4513 2023-06-09 10:44:20.483319 tt_wizard_core-0.1.1b0/PKG-INFO
+-rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)     3521 2023-06-09 10:42:12.000000 tt_wizard_core-0.1.1b0/README.md
+-rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)       38 2023-06-09 10:44:20.483319 tt_wizard_core-0.1.1b0/setup.cfg
+-rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)     1479 2023-06-09 10:39:31.000000 tt_wizard_core-0.1.1b0/setup.py
+drwxr-xr-x   0 bumblebee  (1000) bumblebee  (1000)        0 2023-06-09 10:44:20.481319 tt_wizard_core-0.1.1b0/src/
+drwxr-xr-x   0 bumblebee  (1000) bumblebee  (1000)        0 2023-06-09 10:44:20.482319 tt_wizard_core-0.1.1b0/src/tt_wizard_core.egg-info/
+-rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)     4513 2023-06-09 10:44:20.000000 tt_wizard_core-0.1.1b0/src/tt_wizard_core.egg-info/PKG-INFO
+-rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)      280 2023-06-09 10:44:20.000000 tt_wizard_core-0.1.1b0/src/tt_wizard_core.egg-info/SOURCES.txt
+-rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)        1 2023-06-09 10:44:20.000000 tt_wizard_core-0.1.1b0/src/tt_wizard_core.egg-info/dependency_links.txt
+-rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)       17 2023-06-09 10:44:20.000000 tt_wizard_core-0.1.1b0/src/tt_wizard_core.egg-info/requires.txt
+-rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)       15 2023-06-09 10:44:20.000000 tt_wizard_core-0.1.1b0/src/tt_wizard_core.egg-info/top_level.txt
+-rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)     7342 2023-06-09 10:09:31.000000 tt_wizard_core-0.1.1b0/src/tt_wizard_core.py
```

### Comparing `tt_wizard_core-0.0.1/LICENSE.txt` & `tt_wizard_core-0.1.1b0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-                    GNU GENERAL PUBLIC LICENSE
+GNU GENERAL PUBLIC LICENSE
                        Version 3, 29 June 2007
 
  Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
  Everyone is permitted to copy and distribute verbatim copies
  of this license document, but changing it is not allowed.
 
                             Preamble
```

### Comparing `tt_wizard_core-0.0.1/PKG-INFO` & `tt_wizard_core-0.1.1b0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: tt_wizard_core
-Version: 0.0.1
-Summary: Core of TT_WIZARD
-Home-page: https://github.com/BumblebeeMan
+Version: 0.1.1b0
+Summary: Tool to download and manage gme-files. Core of TT_WIZARD.
+Home-page: https://github.com/BumblebeeMan/tt_wizard_core
 Author: BumblebeeMan (Dennis Schweer)
 Author-email: dennis@bumblebeeman.engineer
 Keywords: TipToi,TipTio,tip,toi,tio
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -16,73 +16,86 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Multimedia :: Sound/Audio
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+License-File: LICENSE
 
 ﻿# Welcome to TT_WIZARD_CORE!
 
-This projects provides an operating system independent backend to download and manage *.gme-files / audio files for the TipToi® pen sold by Ravensburger®. By removing the hassle to deal with file versioning and download servers, it especially enables the creation of tools on plattforms that are currently not officially supported by the manufacturer itself (like Linux). **TT_WIZARD_CORE** only uses the official servers (i.e. hosted by the manufacturer) to download any media files! 
+This projects provides an operating system independent backend to download and manage *.gme-files / audio files for the TipToi pen sold by Ravensburger. By removing the hassle to deal with file versioning and download servers, it especially enables the creation of tools for operating systems that are currently not officially supported by the manufacturer itself (like Linux). **TT_WIZARD_CORE** only uses the official servers (i.e. hosted by the manufacturer) to download any media files! 
 
 ## Following operations are currently supported:
-- Searching the names of all currently published TipToi® media for a keyword (e.g. "puzzle" to get all puzzles listed).
+- Searching the names of all currently published TipToi media for a keyword (e.g. "puzzle" to get all puzzles listed).
 - Picking and downloading selected media from the search results above.
-- Checking whether an allready downloaded media file needs an update or not. (Attention: Files without recent updates may be flagged to require an update, even though no newer versions are available. This is a known issue.) 
+- Checking whether an already downloaded media file needs an update or not. (Attention: Files without recent updates may be flagged to require an update, even though no newer versions are available. This is a known issue.) 
+- Auto update of media files that are already loaded to the TipToi pen
 
 ## Planned features
-- Auto update of media files that are allready loaded to the TipToi® pen
+- Auto detect of pen mount point
 
-## Installation
+## Installation of released version
 
 Use pip to install:
 
 ```python
 pip install tt_wizard_core
 ```
  
 ## Usage
 
 ```python
+#!/usr/bin/env python
+
+# if installed using pip
 from tt_wizard_core import tt_wizard_core
 
 # if not installed using pip and using source code
-# from src.tt_wizard_core import tt_wizard_core
+#from src.tt_wizard_core import tt_wizard_core
 
 print("Welcome to an example of TT_WIZARD_CORE!")
 
 # Create an tt_wizard_core object and provide it with the path to your pen,
 # otherwise the current directory is used.
 # A list of all available media files is downloaded automatically.
 print("What is the path to your TipToi pen?")
 penPath = str(input())
 ttwiz = tt_wizard_core(penPath)
-if len(penPath) < 1:
-    penPath = ""
-    ttwiz = tt_wizard_core()
+#if len(penPath) < 1:
+#    penPath = ""
+#    ttwiz = tt_wizard_core()
 
-# Provide a string to search in the list of available media . 
+# Provide a string to search in the list of available media. 
 print("Please enter keyword to search avaiable media for: ")
 keyword = str(input())
 
 # Search for string and receive a python list of media titles that partially match.
 print("Found following media:")
 searchResult = ttwiz.searchEntry(keyword)
 num = 0
 for item in searchResult:
     print(str(num) + ": " + item)
     num = num + 1
 
 # Decide on which one to download and download media to folder specified in first step.
 print("Which one do you like to download?")
 chosenNum = int(input())
-ttwiz.downloadMedium(searchResult[chosenNum]) #searchResult[chosenNum] is "<<fileName>>.gme"
+titleAsList = [searchResult[chosenNum]]
+ttwiz.downloadMedia(titleAsList) #searchResult[chosenNum] is "<<fileName>>.gme"
+
+# Do you want to download all available files?
+#allMediaFilesList = ttwiz.getAllAvailableTitles()
+#ttwiz.downloadMedia(allMediaFilesList)
+
+# Pass the file name to retrieve information on whether an update is suggested or not.
+#print("Update? " + str(ttwiz.checkForUpdate(searchResult[chosenNum], penPath))) # when >>penPath<< is different from the one configured in the constructor
+print("Update? " + str(ttwiz.checkForUpdate(searchResult[chosenNum])))
 
-# Pass the path and file name to retrieve information on whether an update is suggested or not.
-print("Update? " + str(ttwiz.checkForUpdate(penPath, searchResult[chosenNum])))
+# Perform automatic update on already downloaded media files.
+print("Files updated: " + str(ttwiz.performAutoUpdate(dryRun=True)))
 ```
 
 # Disclaimer and Trademark Notice
 
-NOTE: This package is not verified by, affiliated with, or supported by Ravensburger® AG. TipToi® and Ravensburger® are registered trademarks or trademarks of Ravensburger® AG, in the Germany and/or other countries. These and all other trademarks referenced in this Software or Documentation are the property of their respective owners.
+NOTE: This package is not verified by, affiliated with, or supported by Ravensburger® AG. TipToi® and Ravensburger® are registered trademarks or trademarks of Ravensburger® AG, in the Germany and/or other countries. These and all other trademarks referenced in this Software or Documentation are the property of their respective owners. The trademarkes are mentioned for reference only.
```

### Comparing `tt_wizard_core-0.0.1/README.md` & `tt_wizard_core-0.1.1b0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,64 +1,77 @@
 ﻿# Welcome to TT_WIZARD_CORE!
 
-This projects provides an operating system independent backend to download and manage *.gme-files / audio files for the TipToi® pen sold by Ravensburger®. By removing the hassle to deal with file versioning and download servers, it especially enables the creation of tools on plattforms that are currently not officially supported by the manufacturer itself (like Linux). **TT_WIZARD_CORE** only uses the official servers (i.e. hosted by the manufacturer) to download any media files! 
+This projects provides an operating system independent backend to download and manage *.gme-files / audio files for the TipToi pen sold by Ravensburger. By removing the hassle to deal with file versioning and download servers, it especially enables the creation of tools for operating systems that are currently not officially supported by the manufacturer itself (like Linux). **TT_WIZARD_CORE** only uses the official servers (i.e. hosted by the manufacturer) to download any media files! 
 
 ## Following operations are currently supported:
-- Searching the names of all currently published TipToi® media for a keyword (e.g. "puzzle" to get all puzzles listed).
+- Searching the names of all currently published TipToi media for a keyword (e.g. "puzzle" to get all puzzles listed).
 - Picking and downloading selected media from the search results above.
-- Checking whether an allready downloaded media file needs an update or not. (Attention: Files without recent updates may be flagged to require an update, even though no newer versions are available. This is a known issue.) 
+- Checking whether an already downloaded media file needs an update or not. (Attention: Files without recent updates may be flagged to require an update, even though no newer versions are available. This is a known issue.) 
+- Auto update of media files that are already loaded to the TipToi pen
 
 ## Planned features
-- Auto update of media files that are allready loaded to the TipToi® pen
+- Auto detect of pen mount point
 
-## Installation
+## Installation of released version
 
 Use pip to install:
 
 ```python
 pip install tt_wizard_core
 ```
  
 ## Usage
 
 ```python
+#!/usr/bin/env python
+
+# if installed using pip
 from tt_wizard_core import tt_wizard_core
 
 # if not installed using pip and using source code
-# from src.tt_wizard_core import tt_wizard_core
+#from src.tt_wizard_core import tt_wizard_core
 
 print("Welcome to an example of TT_WIZARD_CORE!")
 
 # Create an tt_wizard_core object and provide it with the path to your pen,
 # otherwise the current directory is used.
 # A list of all available media files is downloaded automatically.
 print("What is the path to your TipToi pen?")
 penPath = str(input())
 ttwiz = tt_wizard_core(penPath)
-if len(penPath) < 1:
-    penPath = ""
-    ttwiz = tt_wizard_core()
+#if len(penPath) < 1:
+#    penPath = ""
+#    ttwiz = tt_wizard_core()
 
-# Provide a string to search in the list of available media . 
+# Provide a string to search in the list of available media. 
 print("Please enter keyword to search avaiable media for: ")
 keyword = str(input())
 
 # Search for string and receive a python list of media titles that partially match.
 print("Found following media:")
 searchResult = ttwiz.searchEntry(keyword)
 num = 0
 for item in searchResult:
     print(str(num) + ": " + item)
     num = num + 1
 
 # Decide on which one to download and download media to folder specified in first step.
 print("Which one do you like to download?")
 chosenNum = int(input())
-ttwiz.downloadMedium(searchResult[chosenNum]) #searchResult[chosenNum] is "<<fileName>>.gme"
+titleAsList = [searchResult[chosenNum]]
+ttwiz.downloadMedia(titleAsList) #searchResult[chosenNum] is "<<fileName>>.gme"
+
+# Do you want to download all available files?
+#allMediaFilesList = ttwiz.getAllAvailableTitles()
+#ttwiz.downloadMedia(allMediaFilesList)
+
+# Pass the file name to retrieve information on whether an update is suggested or not.
+#print("Update? " + str(ttwiz.checkForUpdate(searchResult[chosenNum], penPath))) # when >>penPath<< is different from the one configured in the constructor
+print("Update? " + str(ttwiz.checkForUpdate(searchResult[chosenNum])))
 
-# Pass the path and file name to retrieve information on whether an update is suggested or not.
-print("Update? " + str(ttwiz.checkForUpdate(penPath, searchResult[chosenNum])))
+# Perform automatic update on already downloaded media files.
+print("Files updated: " + str(ttwiz.performAutoUpdate(dryRun=True)))
 ```
 
 # Disclaimer and Trademark Notice
 
-NOTE: This package is not verified by, affiliated with, or supported by Ravensburger® AG. TipToi® and Ravensburger® are registered trademarks or trademarks of Ravensburger® AG, in the Germany and/or other countries. These and all other trademarks referenced in this Software or Documentation are the property of their respective owners.
+NOTE: This package is not verified by, affiliated with, or supported by Ravensburger® AG. TipToi® and Ravensburger® are registered trademarks or trademarks of Ravensburger® AG, in the Germany and/or other countries. These and all other trademarks referenced in this Software or Documentation are the property of their respective owners. The trademarkes are mentioned for reference only.
```

### Comparing `tt_wizard_core-0.0.1/setup.py` & `tt_wizard_core-0.1.1b0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as file:
     long_description = file.read()
 
 setup(
     name = 'tt_wizard_core',
-    version = '0.0.1',
-    description = 'Core of TT_WIZARD',
+    version = '0.1.1-beta',
+    description = 'Tool to download and manage gme-files. Core of TT_WIZARD.',
     long_description = long_description,
     long_description_content_type='text/markdown',
 
     py_modules = ["tt_wizard_core"],
     package_dir = {'': 'src'},
 
     author="BumblebeeMan (Dennis Schweer)", 
     author_email="dennis@bumblebeeman.engineer",     
-    url="https://github.com/BumblebeeMan",
+    url="https://github.com/BumblebeeMan/tt_wizard_core",
 
     install_requires=["requests >= 2.30.0"],
 
     python_requires=">=3.7",
 
     keywords=["TipToi", "TipTio", "tip", "toi", "tio"],
```

### Comparing `tt_wizard_core-0.0.1/src/tt_wizard_core.egg-info/PKG-INFO` & `tt_wizard_core-0.1.1b0/src/tt_wizard_core.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: tt-wizard-core
-Version: 0.0.1
-Summary: Core of TT_WIZARD
-Home-page: https://github.com/BumblebeeMan
+Version: 0.1.1b0
+Summary: Tool to download and manage gme-files. Core of TT_WIZARD.
+Home-page: https://github.com/BumblebeeMan/tt_wizard_core
 Author: BumblebeeMan (Dennis Schweer)
 Author-email: dennis@bumblebeeman.engineer
 Keywords: TipToi,TipTio,tip,toi,tio
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -16,73 +16,86 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Multimedia :: Sound/Audio
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+License-File: LICENSE
 
 ﻿# Welcome to TT_WIZARD_CORE!
 
-This projects provides an operating system independent backend to download and manage *.gme-files / audio files for the TipToi® pen sold by Ravensburger®. By removing the hassle to deal with file versioning and download servers, it especially enables the creation of tools on plattforms that are currently not officially supported by the manufacturer itself (like Linux). **TT_WIZARD_CORE** only uses the official servers (i.e. hosted by the manufacturer) to download any media files! 
+This projects provides an operating system independent backend to download and manage *.gme-files / audio files for the TipToi pen sold by Ravensburger. By removing the hassle to deal with file versioning and download servers, it especially enables the creation of tools for operating systems that are currently not officially supported by the manufacturer itself (like Linux). **TT_WIZARD_CORE** only uses the official servers (i.e. hosted by the manufacturer) to download any media files! 
 
 ## Following operations are currently supported:
-- Searching the names of all currently published TipToi® media for a keyword (e.g. "puzzle" to get all puzzles listed).
+- Searching the names of all currently published TipToi media for a keyword (e.g. "puzzle" to get all puzzles listed).
 - Picking and downloading selected media from the search results above.
-- Checking whether an allready downloaded media file needs an update or not. (Attention: Files without recent updates may be flagged to require an update, even though no newer versions are available. This is a known issue.) 
+- Checking whether an already downloaded media file needs an update or not. (Attention: Files without recent updates may be flagged to require an update, even though no newer versions are available. This is a known issue.) 
+- Auto update of media files that are already loaded to the TipToi pen
 
 ## Planned features
-- Auto update of media files that are allready loaded to the TipToi® pen
+- Auto detect of pen mount point
 
-## Installation
+## Installation of released version
 
 Use pip to install:
 
 ```python
 pip install tt_wizard_core
 ```
  
 ## Usage
 
 ```python
+#!/usr/bin/env python
+
+# if installed using pip
 from tt_wizard_core import tt_wizard_core
 
 # if not installed using pip and using source code
-# from src.tt_wizard_core import tt_wizard_core
+#from src.tt_wizard_core import tt_wizard_core
 
 print("Welcome to an example of TT_WIZARD_CORE!")
 
 # Create an tt_wizard_core object and provide it with the path to your pen,
 # otherwise the current directory is used.
 # A list of all available media files is downloaded automatically.
 print("What is the path to your TipToi pen?")
 penPath = str(input())
 ttwiz = tt_wizard_core(penPath)
-if len(penPath) < 1:
-    penPath = ""
-    ttwiz = tt_wizard_core()
+#if len(penPath) < 1:
+#    penPath = ""
+#    ttwiz = tt_wizard_core()
 
-# Provide a string to search in the list of available media . 
+# Provide a string to search in the list of available media. 
 print("Please enter keyword to search avaiable media for: ")
 keyword = str(input())
 
 # Search for string and receive a python list of media titles that partially match.
 print("Found following media:")
 searchResult = ttwiz.searchEntry(keyword)
 num = 0
 for item in searchResult:
     print(str(num) + ": " + item)
     num = num + 1
 
 # Decide on which one to download and download media to folder specified in first step.
 print("Which one do you like to download?")
 chosenNum = int(input())
-ttwiz.downloadMedium(searchResult[chosenNum]) #searchResult[chosenNum] is "<<fileName>>.gme"
+titleAsList = [searchResult[chosenNum]]
+ttwiz.downloadMedia(titleAsList) #searchResult[chosenNum] is "<<fileName>>.gme"
+
+# Do you want to download all available files?
+#allMediaFilesList = ttwiz.getAllAvailableTitles()
+#ttwiz.downloadMedia(allMediaFilesList)
+
+# Pass the file name to retrieve information on whether an update is suggested or not.
+#print("Update? " + str(ttwiz.checkForUpdate(searchResult[chosenNum], penPath))) # when >>penPath<< is different from the one configured in the constructor
+print("Update? " + str(ttwiz.checkForUpdate(searchResult[chosenNum])))
 
-# Pass the path and file name to retrieve information on whether an update is suggested or not.
-print("Update? " + str(ttwiz.checkForUpdate(penPath, searchResult[chosenNum])))
+# Perform automatic update on already downloaded media files.
+print("Files updated: " + str(ttwiz.performAutoUpdate(dryRun=True)))
 ```
 
 # Disclaimer and Trademark Notice
 
-NOTE: This package is not verified by, affiliated with, or supported by Ravensburger® AG. TipToi® and Ravensburger® are registered trademarks or trademarks of Ravensburger® AG, in the Germany and/or other countries. These and all other trademarks referenced in this Software or Documentation are the property of their respective owners.
+NOTE: This package is not verified by, affiliated with, or supported by Ravensburger® AG. TipToi® and Ravensburger® are registered trademarks or trademarks of Ravensburger® AG, in the Germany and/or other countries. These and all other trademarks referenced in this Software or Documentation are the property of their respective owners. The trademarkes are mentioned for reference only.
```

