# Comparing `tmp/FindSystemFontsFilename-0.0.4.tar.gz` & `tmp/FindSystemFontsFilename-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FindSystemFontsFilename-0.0.4.tar", last modified: Tue Jun  6 00:57:55 2023, max compression
+gzip compressed data, was "FindSystemFontsFilename-0.1.0.tar", last modified: Fri Jun  9 00:54:20 2023, max compression
```

## Comparing `FindSystemFontsFilename-0.0.4.tar` & `FindSystemFontsFilename-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 00:57:55.919253 FindSystemFontsFilename-0.0.4/
-drwxrwxrwx   0        0        0        0 2023-06-06 00:57:55.910468 FindSystemFontsFilename-0.0.4/FindSystemFontsFilename.egg-info/
--rw-rw-rw-   0        0        0     1984 2023-06-06 00:57:55.000000 FindSystemFontsFilename-0.0.4/FindSystemFontsFilename.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      554 2023-06-06 00:57:55.000000 FindSystemFontsFilename-0.0.4/FindSystemFontsFilename.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 00:57:55.000000 FindSystemFontsFilename-0.0.4/FindSystemFontsFilename.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 00:57:55.000000 FindSystemFontsFilename-0.0.4/FindSystemFontsFilename.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-06-06 00:57:55.000000 FindSystemFontsFilename-0.0.4/FindSystemFontsFilename.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1086 2023-04-28 01:55:06.000000 FindSystemFontsFilename-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     1984 2023-06-06 00:57:55.919253 FindSystemFontsFilename-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1092 2023-04-29 02:43:05.000000 FindSystemFontsFilename-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 00:57:55.917299 FindSystemFontsFilename-0.0.4/find_system_fonts_filename/
--rw-rw-rw-   0        0        0      140 2023-06-06 00:45:05.000000 FindSystemFontsFilename-0.0.4/find_system_fonts_filename/__init__.py
--rw-rw-rw-   0        0        0      190 2023-04-28 16:03:29.000000 FindSystemFontsFilename-0.0.4/find_system_fonts_filename/exceptions.py
--rw-rw-rw-   0        0        0      652 2023-04-29 01:59:59.000000 FindSystemFontsFilename-0.0.4/find_system_fonts_filename/fonts_filename.py
--rw-rw-rw-   0        0        0     4931 2023-06-06 00:44:37.000000 FindSystemFontsFilename-0.0.4/find_system_fonts_filename/linux_fonts.py
--rw-rw-rw-   0        0        0     5326 2023-06-06 00:55:47.000000 FindSystemFontsFilename-0.0.4/find_system_fonts_filename/mac_fonts.py
--rw-rw-rw-   0        0        0      280 2023-04-28 01:38:49.000000 FindSystemFontsFilename-0.0.4/find_system_fonts_filename/system_fonts.py
--rw-rw-rw-   0        0        0    20240 2023-06-06 00:44:41.000000 FindSystemFontsFilename-0.0.4/find_system_fonts_filename/windows_fonts.py
--rw-rw-rw-   0        0        0       42 2023-06-06 00:57:55.920240 FindSystemFontsFilename-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1698 2023-04-29 02:21:21.000000 FindSystemFontsFilename-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 00:54:20.218856 FindSystemFontsFilename-0.1.0/
+drwxrwxrwx   0        0        0        0 2023-06-09 00:54:20.206857 FindSystemFontsFilename-0.1.0/FindSystemFontsFilename.egg-info/
+-rw-rw-rw-   0        0        0     2277 2023-06-09 00:54:20.000000 FindSystemFontsFilename-0.1.0/FindSystemFontsFilename.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      598 2023-06-09 00:54:20.000000 FindSystemFontsFilename-0.1.0/FindSystemFontsFilename.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 00:54:20.000000 FindSystemFontsFilename-0.1.0/FindSystemFontsFilename.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 00:54:20.000000 FindSystemFontsFilename-0.1.0/FindSystemFontsFilename.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-06-09 00:54:20.000000 FindSystemFontsFilename-0.1.0/FindSystemFontsFilename.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1086 2023-04-28 01:55:06.000000 FindSystemFontsFilename-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2277 2023-06-09 00:54:20.217857 FindSystemFontsFilename-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1385 2023-06-09 00:53:39.000000 FindSystemFontsFilename-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 00:54:20.216857 FindSystemFontsFilename-0.1.0/find_system_fonts_filename/
+-rw-rw-rw-   0        0        0      164 2023-06-09 00:53:39.000000 FindSystemFontsFilename-0.1.0/find_system_fonts_filename/__init__.py
+-rw-rw-rw-   0        0        0     4209 2023-06-09 00:53:39.000000 FindSystemFontsFilename-0.1.0/find_system_fonts_filename/android_fonts.py
+-rw-rw-rw-   0        0        0      308 2023-06-09 00:53:39.000000 FindSystemFontsFilename-0.1.0/find_system_fonts_filename/exceptions.py
+-rw-rw-rw-   0        0        0     1027 2023-06-09 00:53:39.000000 FindSystemFontsFilename-0.1.0/find_system_fonts_filename/fonts_filename.py
+-rw-rw-rw-   0        0        0     4931 2023-06-06 00:44:37.000000 FindSystemFontsFilename-0.1.0/find_system_fonts_filename/linux_fonts.py
+-rw-rw-rw-   0        0        0     5326 2023-06-06 00:55:47.000000 FindSystemFontsFilename-0.1.0/find_system_fonts_filename/mac_fonts.py
+-rw-rw-rw-   0        0        0      280 2023-04-28 01:38:49.000000 FindSystemFontsFilename-0.1.0/find_system_fonts_filename/system_fonts.py
+-rw-rw-rw-   0        0        0    20240 2023-06-06 00:44:41.000000 FindSystemFontsFilename-0.1.0/find_system_fonts_filename/windows_fonts.py
+-rw-rw-rw-   0        0        0       42 2023-06-09 00:54:20.218856 FindSystemFontsFilename-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1698 2023-04-29 02:21:21.000000 FindSystemFontsFilename-0.1.0/setup.py
```

### Comparing `FindSystemFontsFilename-0.0.4/FindSystemFontsFilename.egg-info/PKG-INFO` & `FindSystemFontsFilename-0.1.0/FindSystemFontsFilename.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FindSystemFontsFilename
-Version: 0.0.4
+Version: 0.1.0
 Summary: Find the system fonts filename.
 Home-page: https://github.com/moi15moi/FindSystemFontsFilename/
 Author: moi15moi
 Author-email: moi15moismokerlolilol@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/moi15moi/FindSystemFontsFilename/
 Project-URL: Tracker, https://github.com/moi15moi/FindSystemFontsFilename/issues/
@@ -23,27 +23,30 @@
 # FindSystemFontsFilename
 This tool allows you to get the font filename on your system. It will collect TrueType (.ttf), OpenType (.otf) and TrueType Collection (.ttf) font format.
 
 It uses some APIs to find the font filename:
 - Windows: [DirectWrite API](https://learn.microsoft.com/en-us/windows/win32/directwrite/direct-write-portal)
 - macOS: [Core Text API](https://developer.apple.com/documentation/coretext)
 - Linux: [Fontconfig API](https://www.freedesktop.org/wiki/Software/fontconfig/)
+- Android: [NDK Font API](https://developer.android.com/ndk/reference/group/font)
 
 ## Installation
 ```
 pip install FindSystemFontsFilename
 ```
 
 ## How to use it
 ```python
-from find_system_fonts_filename import get_system_fonts_filename, FontConfigNotFound, OSNotSupported
+from find_system_fonts_filename import AndroidLibraryNotFound, get_system_fonts_filename, FontConfigNotFound, OSNotSupported
 
 try:
     fonts_filename = get_system_fonts_filename()
-except (FontConfigNotFound, OSNotSupported):
+except (AndroidLibraryNotFound, FontConfigNotFound, OSNotSupported):
     # Deal with the exception
-    # OSNotSupported can only happen in Windows and macOS
+    # OSNotSupported can only happen in Windows, macOS and Android
     #   - Windows Vista SP2 and more are supported
     #   - macOS 10.6 and more are supported
+    #   - Android SDK/API 29 and more are supported
     # FontConfigNotFound can only happen on Linux when Fontconfig could't be found.
+    # AndroidLibraryNotFound can only happen on Android when the android library could't be found.
     pass
 ```
```

### Comparing `FindSystemFontsFilename-0.0.4/FindSystemFontsFilename.egg-info/SOURCES.txt` & `FindSystemFontsFilename-0.1.0/FindSystemFontsFilename.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -3,13 +3,14 @@
 setup.py
 FindSystemFontsFilename.egg-info/PKG-INFO
 FindSystemFontsFilename.egg-info/SOURCES.txt
 FindSystemFontsFilename.egg-info/dependency_links.txt
 FindSystemFontsFilename.egg-info/requires.txt
 FindSystemFontsFilename.egg-info/top_level.txt
 find_system_fonts_filename/__init__.py
+find_system_fonts_filename/android_fonts.py
 find_system_fonts_filename/exceptions.py
 find_system_fonts_filename/fonts_filename.py
 find_system_fonts_filename/linux_fonts.py
 find_system_fonts_filename/mac_fonts.py
 find_system_fonts_filename/system_fonts.py
 find_system_fonts_filename/windows_fonts.py
```

### Comparing `FindSystemFontsFilename-0.0.4/LICENSE` & `FindSystemFontsFilename-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FindSystemFontsFilename-0.0.4/PKG-INFO` & `FindSystemFontsFilename-0.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FindSystemFontsFilename
-Version: 0.0.4
+Version: 0.1.0
 Summary: Find the system fonts filename.
 Home-page: https://github.com/moi15moi/FindSystemFontsFilename/
 Author: moi15moi
 Author-email: moi15moismokerlolilol@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/moi15moi/FindSystemFontsFilename/
 Project-URL: Tracker, https://github.com/moi15moi/FindSystemFontsFilename/issues/
@@ -23,27 +23,30 @@
 # FindSystemFontsFilename
 This tool allows you to get the font filename on your system. It will collect TrueType (.ttf), OpenType (.otf) and TrueType Collection (.ttf) font format.
 
 It uses some APIs to find the font filename:
 - Windows: [DirectWrite API](https://learn.microsoft.com/en-us/windows/win32/directwrite/direct-write-portal)
 - macOS: [Core Text API](https://developer.apple.com/documentation/coretext)
 - Linux: [Fontconfig API](https://www.freedesktop.org/wiki/Software/fontconfig/)
+- Android: [NDK Font API](https://developer.android.com/ndk/reference/group/font)
 
 ## Installation
 ```
 pip install FindSystemFontsFilename
 ```
 
 ## How to use it
 ```python
-from find_system_fonts_filename import get_system_fonts_filename, FontConfigNotFound, OSNotSupported
+from find_system_fonts_filename import AndroidLibraryNotFound, get_system_fonts_filename, FontConfigNotFound, OSNotSupported
 
 try:
     fonts_filename = get_system_fonts_filename()
-except (FontConfigNotFound, OSNotSupported):
+except (AndroidLibraryNotFound, FontConfigNotFound, OSNotSupported):
     # Deal with the exception
-    # OSNotSupported can only happen in Windows and macOS
+    # OSNotSupported can only happen in Windows, macOS and Android
     #   - Windows Vista SP2 and more are supported
     #   - macOS 10.6 and more are supported
+    #   - Android SDK/API 29 and more are supported
     # FontConfigNotFound can only happen on Linux when Fontconfig could't be found.
+    # AndroidLibraryNotFound can only happen on Android when the android library could't be found.
     pass
 ```
```

### Comparing `FindSystemFontsFilename-0.0.4/README.md` & `FindSystemFontsFilename-0.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 # FindSystemFontsFilename
 This tool allows you to get the font filename on your system. It will collect TrueType (.ttf), OpenType (.otf) and TrueType Collection (.ttf) font format.
 
 It uses some APIs to find the font filename:
 - Windows: [DirectWrite API](https://learn.microsoft.com/en-us/windows/win32/directwrite/direct-write-portal)
 - macOS: [Core Text API](https://developer.apple.com/documentation/coretext)
 - Linux: [Fontconfig API](https://www.freedesktop.org/wiki/Software/fontconfig/)
+- Android: [NDK Font API](https://developer.android.com/ndk/reference/group/font)
 
 ## Installation
 ```
 pip install FindSystemFontsFilename
 ```
 
 ## How to use it
 ```python
-from find_system_fonts_filename import get_system_fonts_filename, FontConfigNotFound, OSNotSupported
+from find_system_fonts_filename import AndroidLibraryNotFound, get_system_fonts_filename, FontConfigNotFound, OSNotSupported
 
 try:
     fonts_filename = get_system_fonts_filename()
-except (FontConfigNotFound, OSNotSupported):
+except (AndroidLibraryNotFound, FontConfigNotFound, OSNotSupported):
     # Deal with the exception
-    # OSNotSupported can only happen in Windows and macOS
+    # OSNotSupported can only happen in Windows, macOS and Android
     #   - Windows Vista SP2 and more are supported
     #   - macOS 10.6 and more are supported
+    #   - Android SDK/API 29 and more are supported
     # FontConfigNotFound can only happen on Linux when Fontconfig could't be found.
+    # AndroidLibraryNotFound can only happen on Android when the android library could't be found.
     pass
 ```
```

### Comparing `FindSystemFontsFilename-0.0.4/find_system_fonts_filename/linux_fonts.py` & `FindSystemFontsFilename-0.1.0/find_system_fonts_filename/linux_fonts.py`

 * *Files identical despite different names*

### Comparing `FindSystemFontsFilename-0.0.4/find_system_fonts_filename/mac_fonts.py` & `FindSystemFontsFilename-0.1.0/find_system_fonts_filename/mac_fonts.py`

 * *Files identical despite different names*

### Comparing `FindSystemFontsFilename-0.0.4/find_system_fonts_filename/windows_fonts.py` & `FindSystemFontsFilename-0.1.0/find_system_fonts_filename/windows_fonts.py`

 * *Files identical despite different names*

### Comparing `FindSystemFontsFilename-0.0.4/setup.py` & `FindSystemFontsFilename-0.1.0/setup.py`

 * *Files identical despite different names*

