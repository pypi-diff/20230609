# Comparing `tmp/appstream-python-0.6.1.tar.gz` & `tmp/appstream-python-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appstream-python-0.6.1.tar", last modified: Mon Apr 24 13:23:40 2023, max compression
+gzip compressed data, was "appstream-python-0.6.2.tar", last modified: Fri Jun  9 08:43:58 2023, max compression
```

## Comparing `appstream-python-0.6.1.tar` & `appstream-python-0.6.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:40.035801 appstream-python-0.6.1/
--rw-r--r--   0 root         (0) root         (0)     1318 2023-04-24 13:22:10.000000 appstream-python-0.6.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       71 2023-04-24 13:22:10.000000 appstream-python-0.6.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1286 2023-04-24 13:23:40.035801 appstream-python-0.6.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      112 2023-04-24 13:22:10.000000 appstream-python-0.6.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:40.035801 appstream-python-0.6.1/appstream_python/
--rw-r--r--   0 root         (0) root         (0)     2777 2023-04-24 13:22:10.000000 appstream-python-0.6.1/appstream_python/Collection.py
--rw-r--r--   0 root         (0) root         (0)    35641 2023-04-24 13:22:10.000000 appstream-python-0.6.1/appstream_python/Component.py
--rw-r--r--   0 root         (0) root         (0)     2186 2023-04-24 13:22:10.000000 appstream-python-0.6.1/appstream_python/StandardConstants.py
--rw-r--r--   0 root         (0) root         (0)      164 2023-04-24 13:22:10.000000 appstream-python-0.6.1/appstream_python/__init__.py
--rw-r--r--   0 root         (0) root         (0)      326 2023-04-24 13:22:10.000000 appstream-python-0.6.1/appstream_python/_helper.py
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-24 13:22:10.000000 appstream-python-0.6.1/appstream_python/version.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:40.035801 appstream-python-0.6.1/appstream_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1286 2023-04-24 13:23:40.000000 appstream-python-0.6.1/appstream_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      512 2023-04-24 13:23:40.000000 appstream-python-0.6.1/appstream_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 13:23:40.000000 appstream-python-0.6.1/appstream_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-24 13:23:40.000000 appstream-python-0.6.1/appstream_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-04-24 13:23:40.000000 appstream-python-0.6.1/appstream_python.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1366 2023-04-24 13:22:10.000000 appstream-python-0.6.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 13:23:40.035801 appstream-python-0.6.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:40.035801 appstream-python-0.6.1/tests/
--rw-r--r--   0 root         (0) root         (0)     1114 2023-04-24 13:22:10.000000 appstream-python-0.6.1/tests/test_appstream_data.py
--rw-r--r--   0 root         (0) root         (0)     1147 2023-04-24 13:22:10.000000 appstream-python-0.6.1/tests/test_description.py
--rw-r--r--   0 root         (0) root         (0)     2982 2023-04-24 13:22:10.000000 appstream-python-0.6.1/tests/test_display_length.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 08:43:58.030553 appstream-python-0.6.2/
+-rw-r--r--   0 root         (0) root         (0)     1318 2023-06-09 08:43:21.000000 appstream-python-0.6.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       71 2023-06-09 08:43:21.000000 appstream-python-0.6.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1286 2023-06-09 08:43:58.030553 appstream-python-0.6.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      112 2023-06-09 08:43:21.000000 appstream-python-0.6.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 08:43:58.030553 appstream-python-0.6.2/appstream_python/
+-rw-r--r--   0 root         (0) root         (0)     2777 2023-06-09 08:43:21.000000 appstream-python-0.6.2/appstream_python/Collection.py
+-rw-r--r--   0 root         (0) root         (0)    35746 2023-06-09 08:43:21.000000 appstream-python-0.6.2/appstream_python/Component.py
+-rw-r--r--   0 root         (0) root         (0)     2186 2023-06-09 08:43:21.000000 appstream-python-0.6.2/appstream_python/StandardConstants.py
+-rw-r--r--   0 root         (0) root         (0)      164 2023-06-09 08:43:21.000000 appstream-python-0.6.2/appstream_python/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      326 2023-06-09 08:43:21.000000 appstream-python-0.6.2/appstream_python/_helper.py
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-09 08:43:21.000000 appstream-python-0.6.2/appstream_python/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 08:43:58.030553 appstream-python-0.6.2/appstream_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1286 2023-06-09 08:43:58.000000 appstream-python-0.6.2/appstream_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      512 2023-06-09 08:43:58.000000 appstream-python-0.6.2/appstream_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 08:43:58.000000 appstream-python-0.6.2/appstream_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-09 08:43:58.000000 appstream-python-0.6.2/appstream_python.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-06-09 08:43:58.000000 appstream-python-0.6.2/appstream_python.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1366 2023-06-09 08:43:21.000000 appstream-python-0.6.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 08:43:58.030553 appstream-python-0.6.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 08:43:58.030553 appstream-python-0.6.2/tests/
+-rw-r--r--   0 root         (0) root         (0)     1114 2023-06-09 08:43:21.000000 appstream-python-0.6.2/tests/test_appstream_data.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2023-06-09 08:43:21.000000 appstream-python-0.6.2/tests/test_description.py
+-rw-r--r--   0 root         (0) root         (0)     2982 2023-06-09 08:43:21.000000 appstream-python-0.6.2/tests/test_display_length.py
```

### Comparing `appstream-python-0.6.1/LICENSE` & `appstream-python-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `appstream-python-0.6.1/PKG-INFO` & `appstream-python-0.6.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appstream-python
-Version: 0.6.1
+Version: 0.6.2
 Summary: A library for dealing with Freedesktop Appstream data
 Author-email: JakobDev <jakobdev@gmx.de>
 License: BSD-2-Clause
 Project-URL: Documentation, https://appstream-python.readthedocs.io
 Project-URL: Issues, https://codeberg.org/JakobDev/appstream-python/issues
 Project-URL: Source, https://codeberg.org/JakobDev/appstream-python
 Project-URL: Donation, https://ko-fi.com/jakobdev
```

### Comparing `appstream-python-0.6.1/appstream_python/Collection.py` & `appstream-python-0.6.2/appstream_python/Collection.py`

 * *Files identical despite different names*

### Comparing `appstream-python-0.6.1/appstream_python/Component.py` & `appstream-python-0.6.2/appstream_python/Component.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,16 +120,19 @@
 
     def load_tag(self, tag: etree.Element) -> None:
         "Loads an Tag. Only for internal use."
         if tag.get("{http://www.w3.org/XML/1998/namespace}lang") is None:
             current_text = ""
             for i in tag.getchildren():
                 if i.get(_XML_LANG) is None:
-                    current_text = i.text.strip()
-                    self._translated_data[current_text] = {}
+                    try:
+                        current_text = i.text.strip()
+                        self._translated_data[current_text] = {}
+                    except AttributeError:
+                        pass
                 else:
                     if current_text in self._translated_data:
                         self._translated_data[current_text][i.get(_XML_LANG)] = i.text.strip()
         else:
             if tag.get("{http://www.w3.org/XML/1998/namespace}lang") not in self._translated_lists:
                 self._translated_lists[tag.get("{http://www.w3.org/XML/1998/namespace}lang")] = []
             for i in tag.getchildren():
```

### Comparing `appstream-python-0.6.1/appstream_python/StandardConstants.py` & `appstream-python-0.6.2/appstream_python/StandardConstants.py`

 * *Files identical despite different names*

### Comparing `appstream-python-0.6.1/appstream_python.egg-info/PKG-INFO` & `appstream-python-0.6.2/appstream_python.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appstream-python
-Version: 0.6.1
+Version: 0.6.2
 Summary: A library for dealing with Freedesktop Appstream data
 Author-email: JakobDev <jakobdev@gmx.de>
 License: BSD-2-Clause
 Project-URL: Documentation, https://appstream-python.readthedocs.io
 Project-URL: Issues, https://codeberg.org/JakobDev/appstream-python/issues
 Project-URL: Source, https://codeberg.org/JakobDev/appstream-python
 Project-URL: Donation, https://ko-fi.com/jakobdev
```

### Comparing `appstream-python-0.6.1/appstream_python.egg-info/SOURCES.txt` & `appstream-python-0.6.2/appstream_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `appstream-python-0.6.1/pyproject.toml` & `appstream-python-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `appstream-python-0.6.1/tests/test_appstream_data.py` & `appstream-python-0.6.2/tests/test_appstream_data.py`

 * *Files identical despite different names*

### Comparing `appstream-python-0.6.1/tests/test_description.py` & `appstream-python-0.6.2/tests/test_description.py`

 * *Files identical despite different names*

### Comparing `appstream-python-0.6.1/tests/test_display_length.py` & `appstream-python-0.6.2/tests/test_display_length.py`

 * *Files identical despite different names*

