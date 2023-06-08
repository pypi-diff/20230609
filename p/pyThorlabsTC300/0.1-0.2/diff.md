# Comparing `tmp/pyThorlabsTC300-0.1.tar.gz` & `tmp/pyThorlabsTC300-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyThorlabsTC300-0.1.tar", last modified: Thu Jun  8 23:04:07 2023, max compression
+gzip compressed data, was "pyThorlabsTC300-0.2.tar", last modified: Thu Jun  8 23:07:40 2023, max compression
```

## Comparing `pyThorlabsTC300-0.1.tar` & `pyThorlabsTC300-0.2.tar`

### file list

```diff
@@ -1,19 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 23:04:07.749812 pyThorlabsTC300-0.1/
--rw-rw-rw-   0        0        0       68 2022-04-01 03:57:29.000000 pyThorlabsTC300-0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     7592 2023-06-08 23:04:07.748817 pyThorlabsTC300-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     7263 2022-10-06 04:44:02.000000 pyThorlabsTC300-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 23:04:07.692204 pyThorlabsTC300-0.1/pyThorlabsTC300/
--rw-rw-rw-   0        0        0    40834 2023-06-07 20:01:07.000000 pyThorlabsTC300-0.1/pyThorlabsTC300/TC300_COMMAND_LIB.py
--rw-rw-rw-   0        0        0    17045 2021-12-03 07:56:46.000000 pyThorlabsTC300-0.1/pyThorlabsTC300/TC300_COMMAND_LIB_EXAMPLE.py
--rw-rw-rw-   0        0        0      330 2022-10-03 21:45:25.000000 pyThorlabsTC300-0.1/pyThorlabsTC300/__init__.py
--rw-rw-rw-   0        0        0     9437 2023-06-08 04:34:41.000000 pyThorlabsTC300-0.1/pyThorlabsTC300/driver.py
--rw-rw-rw-   0        0        0    48530 2023-06-08 20:39:00.000000 pyThorlabsTC300-0.1/pyThorlabsTC300/main.py
-drwxrwxrwx   0        0        0        0 2023-06-08 23:04:07.702181 pyThorlabsTC300-0.1/pyThorlabsTC300.egg-info/
--rw-rw-rw-   0        0        0     7592 2023-06-08 23:04:07.000000 pyThorlabsTC300-0.1/pyThorlabsTC300.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      426 2023-06-08 23:04:07.000000 pyThorlabsTC300-0.1/pyThorlabsTC300.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 23:04:07.000000 pyThorlabsTC300-0.1/pyThorlabsTC300.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-06-08 23:04:07.000000 pyThorlabsTC300-0.1/pyThorlabsTC300.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-06-08 23:04:07.000000 pyThorlabsTC300-0.1/pyThorlabsTC300.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       16 2023-06-08 23:04:07.000000 pyThorlabsTC300-0.1/pyThorlabsTC300.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-08 23:04:07.749812 pyThorlabsTC300-0.1/setup.cfg
--rw-rw-rw-   0        0        0      982 2023-06-08 23:02:38.000000 pyThorlabsTC300-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 23:07:40.337226 pyThorlabsTC300-0.2/
+-rw-rw-rw-   0        0        0       97 2023-06-08 23:07:04.000000 pyThorlabsTC300-0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     7592 2023-06-08 23:07:40.336222 pyThorlabsTC300-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7263 2022-10-06 04:44:02.000000 pyThorlabsTC300-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 23:07:40.194221 pyThorlabsTC300-0.2/pyThorlabsTC300/
+-rw-rw-rw-   0        0        0   258560 2021-12-03 07:56:46.000000 pyThorlabsTC300-0.2/pyThorlabsTC300/TC300COMMANDLIB_win32.dll
+-rw-rw-rw-   0        0        0   312832 2021-12-03 07:56:46.000000 pyThorlabsTC300-0.2/pyThorlabsTC300/TC300COMMANDLIB_win64.dll
+-rw-rw-rw-   0        0        0    40834 2023-06-07 20:01:07.000000 pyThorlabsTC300-0.2/pyThorlabsTC300/TC300_COMMAND_LIB.py
+-rw-rw-rw-   0        0        0    17045 2021-12-03 07:56:46.000000 pyThorlabsTC300-0.2/pyThorlabsTC300/TC300_COMMAND_LIB_EXAMPLE.py
+-rw-rw-rw-   0        0        0      330 2022-10-03 21:45:25.000000 pyThorlabsTC300-0.2/pyThorlabsTC300/__init__.py
+-rw-rw-rw-   0        0        0      405 2023-06-08 20:59:24.000000 pyThorlabsTC300-0.2/pyThorlabsTC300/config.json
+-rw-rw-rw-   0        0        0     9437 2023-06-08 04:34:41.000000 pyThorlabsTC300-0.2/pyThorlabsTC300/driver.py
+drwxrwxrwx   0        0        0        0 2023-06-08 23:07:40.264529 pyThorlabsTC300-0.2/pyThorlabsTC300/graphics/
+-rw-rw-rw-   0        0        0     7799 2021-08-31 16:42:47.000000 pyThorlabsTC300-0.2/pyThorlabsTC300/graphics/pause.png
+-rw-rw-rw-   0        0        0     9320 2021-08-31 16:41:38.000000 pyThorlabsTC300-0.2/pyThorlabsTC300/graphics/play.png
+-rw-rw-rw-   0        0        0     3439 2021-08-29 03:28:31.000000 pyThorlabsTC300-0.2/pyThorlabsTC300/graphics/refresh.png
+-rw-rw-rw-   0        0        0     7522 2021-08-31 16:43:00.000000 pyThorlabsTC300-0.2/pyThorlabsTC300/graphics/stop.png
+-rw-rw-rw-   0        0        0    48530 2023-06-08 20:39:00.000000 pyThorlabsTC300-0.2/pyThorlabsTC300/main.py
+drwxrwxrwx   0        0        0        0 2023-06-08 23:07:40.242555 pyThorlabsTC300-0.2/pyThorlabsTC300.egg-info/
+-rw-rw-rw-   0        0        0     7592 2023-06-08 23:07:40.000000 pyThorlabsTC300-0.2/pyThorlabsTC300.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      678 2023-06-08 23:07:40.000000 pyThorlabsTC300-0.2/pyThorlabsTC300.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 23:07:40.000000 pyThorlabsTC300-0.2/pyThorlabsTC300.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-06-08 23:07:40.000000 pyThorlabsTC300-0.2/pyThorlabsTC300.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-08 23:04:07.000000 pyThorlabsTC300-0.2/pyThorlabsTC300.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       16 2023-06-08 23:07:40.000000 pyThorlabsTC300-0.2/pyThorlabsTC300.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 23:07:40.338221 pyThorlabsTC300-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      982 2023-06-08 23:07:16.000000 pyThorlabsTC300-0.2/setup.py
```

### Comparing `pyThorlabsTC300-0.1/PKG-INFO` & `pyThorlabsTC300-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyThorlabsTC300
-Version: 0.1
+Version: 0.2
 Summary: A python library/GUI to access and control the TC300 Temperature Controller of Thorlabs.
 Home-page: https://github.com/MicheleCotrufo/
 Author: Michele Cotrufo
 Author-email: michele.cotrufo@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `pyThorlabsTC300-0.1/README.md` & `pyThorlabsTC300-0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyThorlabsTC300-0.1/pyThorlabsTC300/TC300_COMMAND_LIB.py` & `pyThorlabsTC300-0.2/pyThorlabsTC300/TC300_COMMAND_LIB.py`

 * *Files identical despite different names*

### Comparing `pyThorlabsTC300-0.1/pyThorlabsTC300/TC300_COMMAND_LIB_EXAMPLE.py` & `pyThorlabsTC300-0.2/pyThorlabsTC300/TC300_COMMAND_LIB_EXAMPLE.py`

 * *Files identical despite different names*

### Comparing `pyThorlabsTC300-0.1/pyThorlabsTC300/driver.py` & `pyThorlabsTC300-0.2/pyThorlabsTC300/driver.py`

 * *Files identical despite different names*

### Comparing `pyThorlabsTC300-0.1/pyThorlabsTC300/main.py` & `pyThorlabsTC300-0.2/pyThorlabsTC300/main.py`

 * *Files identical despite different names*

### Comparing `pyThorlabsTC300-0.1/pyThorlabsTC300.egg-info/PKG-INFO` & `pyThorlabsTC300-0.2/pyThorlabsTC300.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyThorlabsTC300
-Version: 0.1
+Version: 0.2
 Summary: A python library/GUI to access and control the TC300 Temperature Controller of Thorlabs.
 Home-page: https://github.com/MicheleCotrufo/
 Author: Michele Cotrufo
 Author-email: michele.cotrufo@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `pyThorlabsTC300-0.1/setup.py` & `pyThorlabsTC300-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open(path.join(this_directory, 'README.md'),encoding ='unicode_escape') as f:
     long_description = f.read()
 
 with open("requirements_strict.txt") as f:
     required_packages = f.read().splitlines()
 
 setuptools.setup(name='pyThorlabsTC300',
-      version='0.1',
+      version='0.2',
       description='A python library/GUI to access and control the TC300 Temperature Controller of Thorlabs.',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/MicheleCotrufo/',
       author='Michele Cotrufo',
       author_email='michele.cotrufo@gmail.com',
       license='MIT',
```

