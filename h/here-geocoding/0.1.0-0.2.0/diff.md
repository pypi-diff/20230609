# Comparing `tmp/here_geocoding-0.1.0.tar.gz` & `tmp/here_geocoding-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "here_geocoding-0.1.0.tar", last modified: Fri Jun  9 08:28:43 2023, max compression
+gzip compressed data, was "here_geocoding-0.2.0.tar", last modified: Fri Jun  9 08:49:56 2023, max compression
```

## Comparing `here_geocoding-0.1.0.tar` & `here_geocoding-0.2.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 08:28:43.321715 here_geocoding-0.1.0/
--rw-rw-rw-   0        0        0      176 2023-06-09 07:40:11.000000 here_geocoding-0.1.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3739 2023-06-09 07:40:11.000000 here_geocoding-0.1.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-06-09 07:40:11.000000 here_geocoding-0.1.0/HISTORY.rst
--rw-rw-rw-   0        0        0     1099 2023-06-09 07:40:11.000000 here_geocoding-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      273 2023-06-09 07:40:11.000000 here_geocoding-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4083 2023-06-09 08:28:43.322635 here_geocoding-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2890 2023-06-09 08:10:51.000000 here_geocoding-0.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-09 08:28:43.276647 here_geocoding-0.1.0/docs/
--rw-rw-rw-   0        0        0      635 2023-06-09 07:40:11.000000 here_geocoding-0.1.0/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-06-09 07:40:11.000000 here_geocoding-0.1.0/docs/authors.rst
--rw-rw-rw-   0        0        0     5049 2023-06-09 07:40:11.000000 here_geocoding-0.1.0/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-06-09 07:40:11.000000 here_geocoding-0.1.0/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-06-09 07:40:11.000000 here_geocoding-0.1.0/docs/history.rst
--rw-rw-rw-   0        0        0      331 2023-06-09 07:40:11.000000 here_geocoding-0.1.0/docs/index.rst
--rw-rw-rw-   0        0        0     1225 2023-06-09 07:40:11.000000 here_geocoding-0.1.0/docs/installation.rst
--rwxrwxrwx   0        0        0      812 2023-06-09 07:40:11.000000 here_geocoding-0.1.0/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-06-09 07:40:11.000000 here_geocoding-0.1.0/docs/readme.rst
--rw-rw-rw-   0        0        0       90 2023-06-09 07:40:11.000000 here_geocoding-0.1.0/docs/usage.rst
-drwxrwxrwx   0        0        0        0 2023-06-09 08:28:43.284566 here_geocoding-0.1.0/here_geocoding/
--rw-rw-rw-   0        0        0      180 2023-06-09 07:44:37.000000 here_geocoding-0.1.0/here_geocoding/__init__.py
--rw-rw-rw-   0        0        0      436 2023-06-09 07:40:11.000000 here_geocoding-0.1.0/here_geocoding/cli.py
--rw-rw-rw-   0        0        0     3480 2023-06-09 07:48:31.000000 here_geocoding-0.1.0/here_geocoding/here_geocoding.py
-drwxrwxrwx   0        0        0        0 2023-06-09 08:28:43.309012 here_geocoding-0.1.0/here_geocoding.egg-info/
--rw-rw-rw-   0        0        0     4083 2023-06-09 08:28:42.000000 here_geocoding-0.1.0/here_geocoding.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      695 2023-06-09 08:28:43.000000 here_geocoding-0.1.0/here_geocoding.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 08:28:42.000000 here_geocoding-0.1.0/here_geocoding.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-06-09 08:28:42.000000 here_geocoding-0.1.0/here_geocoding.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-06-09 08:28:42.000000 here_geocoding-0.1.0/here_geocoding.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       46 2023-06-09 08:28:42.000000 here_geocoding-0.1.0/here_geocoding.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-09 08:28:42.000000 here_geocoding-0.1.0/here_geocoding.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      409 2023-06-09 08:28:43.326140 here_geocoding-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1845 2023-06-09 08:20:11.000000 here_geocoding-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 08:28:43.320483 here_geocoding-0.1.0/tests/
--rw-rw-rw-   0        0        0       45 2023-06-09 07:40:11.000000 here_geocoding-0.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0    14059 2023-06-09 07:15:05.000000 here_geocoding-0.1.0/tests/address-sample.xlsx
--rw-rw-rw-   0        0        0     1141 2023-06-09 07:48:43.000000 here_geocoding-0.1.0/tests/examples.py
--rw-rw-rw-   0        0        0      934 2023-06-09 07:40:11.000000 here_geocoding-0.1.0/tests/test_here_geocoding.py
+drwxrwxrwx   0        0        0        0 2023-06-09 08:49:56.632655 here_geocoding-0.2.0/
+-rw-rw-rw-   0        0        0      176 2023-06-09 07:40:11.000000 here_geocoding-0.2.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3739 2023-06-09 07:40:11.000000 here_geocoding-0.2.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-06-09 07:40:11.000000 here_geocoding-0.2.0/HISTORY.rst
+-rw-rw-rw-   0        0        0     1099 2023-06-09 07:40:11.000000 here_geocoding-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-06-09 07:40:11.000000 here_geocoding-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4083 2023-06-09 08:49:56.632838 here_geocoding-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2890 2023-06-09 08:10:51.000000 here_geocoding-0.2.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-09 08:49:56.508283 here_geocoding-0.2.0/docs/
+-rw-rw-rw-   0        0        0      635 2023-06-09 07:40:11.000000 here_geocoding-0.2.0/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2023-06-09 07:40:11.000000 here_geocoding-0.2.0/docs/authors.rst
+-rw-rw-rw-   0        0        0     5049 2023-06-09 07:40:11.000000 here_geocoding-0.2.0/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-06-09 07:40:11.000000 here_geocoding-0.2.0/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-06-09 07:40:11.000000 here_geocoding-0.2.0/docs/history.rst
+-rw-rw-rw-   0        0        0      331 2023-06-09 07:40:11.000000 here_geocoding-0.2.0/docs/index.rst
+-rw-rw-rw-   0        0        0     1225 2023-06-09 07:40:11.000000 here_geocoding-0.2.0/docs/installation.rst
+-rwxrwxrwx   0        0        0      812 2023-06-09 07:40:11.000000 here_geocoding-0.2.0/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2023-06-09 07:40:11.000000 here_geocoding-0.2.0/docs/readme.rst
+-rw-rw-rw-   0        0        0       90 2023-06-09 07:40:11.000000 here_geocoding-0.2.0/docs/usage.rst
+drwxrwxrwx   0        0        0        0 2023-06-09 08:49:56.548282 here_geocoding-0.2.0/here_geocoding/
+-rw-rw-rw-   0        0        0      180 2023-06-09 07:44:37.000000 here_geocoding-0.2.0/here_geocoding/__init__.py
+-rw-rw-rw-   0        0        0      436 2023-06-09 07:40:11.000000 here_geocoding-0.2.0/here_geocoding/cli.py
+-rw-rw-rw-   0        0        0     3480 2023-06-09 07:48:31.000000 here_geocoding-0.2.0/here_geocoding/here_geocoding.py
+drwxrwxrwx   0        0        0        0 2023-06-09 08:49:56.598396 here_geocoding-0.2.0/here_geocoding.egg-info/
+-rw-rw-rw-   0        0        0     4083 2023-06-09 08:49:56.000000 here_geocoding-0.2.0/here_geocoding.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      695 2023-06-09 08:49:56.000000 here_geocoding-0.2.0/here_geocoding.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 08:49:56.000000 here_geocoding-0.2.0/here_geocoding.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-06-09 08:49:56.000000 here_geocoding-0.2.0/here_geocoding.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-09 08:49:56.000000 here_geocoding-0.2.0/here_geocoding.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       55 2023-06-09 08:49:56.000000 here_geocoding-0.2.0/here_geocoding.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-09 08:49:56.000000 here_geocoding-0.2.0/here_geocoding.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      409 2023-06-09 08:49:56.634871 here_geocoding-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1857 2023-06-09 08:48:49.000000 here_geocoding-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 08:49:56.627635 here_geocoding-0.2.0/tests/
+-rw-rw-rw-   0        0        0       45 2023-06-09 07:40:11.000000 here_geocoding-0.2.0/tests/__init__.py
+-rw-rw-rw-   0        0        0    14059 2023-06-09 07:15:05.000000 here_geocoding-0.2.0/tests/address-sample.xlsx
+-rw-rw-rw-   0        0        0     1141 2023-06-09 07:48:43.000000 here_geocoding-0.2.0/tests/examples.py
+-rw-rw-rw-   0        0        0      934 2023-06-09 07:40:11.000000 here_geocoding-0.2.0/tests/test_here_geocoding.py
```

### Comparing `here_geocoding-0.1.0/CONTRIBUTING.rst` & `here_geocoding-0.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `here_geocoding-0.1.0/LICENSE` & `here_geocoding-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `here_geocoding-0.1.0/PKG-INFO` & `here_geocoding-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: here_geocoding
-Version: 0.1.0
+Version: 0.2.0
 Summary: The "here-geocoding" package is a Python library designed to streamline the process of converting addresses stored in an Excel (xlsx) file into latitude and longitude coordinates. It provides a convenient solution for geocoding large sets of addresses using the HERE geocoding service.
 Home-page: https://github.com/Mariosmsk/here_geocoding
 Author: Marios S. Kyriakou
 Author-email: mariosmsk@gmail.com
 License: MIT license
 Keywords: here_geocoding
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `here_geocoding-0.1.0/README.rst` & `here_geocoding-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `here_geocoding-0.1.0/docs/Makefile` & `here_geocoding-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `here_geocoding-0.1.0/docs/conf.py` & `here_geocoding-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `here_geocoding-0.1.0/docs/installation.rst` & `here_geocoding-0.2.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `here_geocoding-0.1.0/docs/make.bat` & `here_geocoding-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `here_geocoding-0.1.0/here_geocoding/here_geocoding.py` & `here_geocoding-0.2.0/here_geocoding/here_geocoding.py`

 * *Files identical despite different names*

### Comparing `here_geocoding-0.1.0/here_geocoding.egg-info/PKG-INFO` & `here_geocoding-0.2.0/here_geocoding.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: here-geocoding
-Version: 0.1.0
+Version: 0.2.0
 Summary: The "here-geocoding" package is a Python library designed to streamline the process of converting addresses stored in an Excel (xlsx) file into latitude and longitude coordinates. It provides a convenient solution for geocoding large sets of addresses using the HERE geocoding service.
 Home-page: https://github.com/Mariosmsk/here_geocoding
 Author: Marios S. Kyriakou
 Author-email: mariosmsk@gmail.com
 License: MIT license
 Keywords: here_geocoding
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `here_geocoding-0.1.0/here_geocoding.egg-info/SOURCES.txt` & `here_geocoding-0.2.0/here_geocoding.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `here_geocoding-0.1.0/setup.py` & `here_geocoding-0.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
-requirements = ['requests', 'pyproj', 'pandas', 'here_location_services']
+requirements = ['requests', 'pyproj', 'pandas', 'here_location_services', 'openpyxl']
 
 test_requirements = []
 
 setup(
     author="Marios S. Kyriakou",
     author_email='mariosmsk@gmail.com',
     python_requires='>=3.6',
@@ -44,10 +44,10 @@
     include_package_data=True,
     keywords='here_geocoding',
     name='here_geocoding',
     packages=find_packages(include=['here_geocoding', 'here_geocoding.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/Mariosmsk/here_geocoding',
-    version='0.1.0',
+    version='0.2.0',
     zip_safe=False,
 )
```

### Comparing `here_geocoding-0.1.0/tests/address-sample.xlsx` & `here_geocoding-0.2.0/tests/address-sample.xlsx`

 * *Files identical despite different names*

### Comparing `here_geocoding-0.1.0/tests/examples.py` & `here_geocoding-0.2.0/tests/examples.py`

 * *Files identical despite different names*

### Comparing `here_geocoding-0.1.0/tests/test_here_geocoding.py` & `here_geocoding-0.2.0/tests/test_here_geocoding.py`

 * *Files identical despite different names*

