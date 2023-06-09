# Comparing `tmp/cabinet-2023.5.31.3.tar.gz` & `tmp/cabinet-2023.6.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cabinet-2023.5.31.3.tar", last modified: Wed May 31 16:38:06 2023, max compression
+gzip compressed data, was "cabinet-2023.6.8.1.tar", last modified: Fri Jun  9 04:30:15 2023, max compression
```

## Comparing `cabinet-2023.5.31.3.tar` & `cabinet-2023.6.8.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-31 16:38:06.220978 cabinet-2023.5.31.3/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    11357 2023-03-06 03:35:41.000000 cabinet-2023.5.31.3/LICENSE
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     6580 2023-05-31 16:38:06.220978 cabinet-2023.5.31.3/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     6228 2023-05-31 04:52:07.000000 cabinet-2023.5.31.3/README.md
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       98 2023-03-06 04:41:10.000000 cabinet-2023.5.31.3/pyproject.toml
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      750 2023-05-31 16:38:06.220978 cabinet-2023.5.31.3/setup.cfg
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-31 16:38:06.220978 cabinet-2023.5.31.3/src/
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-31 16:38:06.220978 cabinet-2023.5.31.3/src/cabinet/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       80 2023-05-31 16:37:40.000000 cabinet-2023.5.31.3/src/cabinet/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       69 2023-05-31 04:50:50.000000 cabinet-2023.5.31.3/src/cabinet/__main__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    26102 2023-05-31 05:11:01.000000 cabinet-2023.5.31.3/src/cabinet/cabinet.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     3687 2023-04-16 16:59:23.000000 cabinet-2023.5.31.3/src/cabinet/mail.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-31 16:38:06.220978 cabinet-2023.5.31.3/src/cabinet.egg-info/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     6580 2023-05-31 16:38:06.000000 cabinet-2023.5.31.3/src/cabinet.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      333 2023-05-31 16:38:06.000000 cabinet-2023.5.31.3/src/cabinet.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-05-31 16:38:06.000000 cabinet-2023.5.31.3/src/cabinet.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2023-05-31 16:38:06.000000 cabinet-2023.5.31.3/src/cabinet.egg-info/entry_points.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2023-05-31 16:38:06.000000 cabinet-2023.5.31.3/src/cabinet.egg-info/top_level.txt
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-31 16:38:06.220978 cabinet-2023.5.31.3/test/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     5868 2023-05-31 04:52:07.000000 cabinet-2023.5.31.3/test/test___init__.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-09 04:30:15.960220 cabinet-2023.6.8.1/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    11357 2023-03-06 03:35:41.000000 cabinet-2023.6.8.1/LICENSE
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     6579 2023-06-09 04:30:15.960220 cabinet-2023.6.8.1/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     6228 2023-05-31 04:52:07.000000 cabinet-2023.6.8.1/README.md
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       98 2023-03-06 04:41:10.000000 cabinet-2023.6.8.1/pyproject.toml
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      750 2023-06-09 04:30:15.960220 cabinet-2023.6.8.1/setup.cfg
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-09 04:30:15.960220 cabinet-2023.6.8.1/src/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-09 04:30:15.960220 cabinet-2023.6.8.1/src/cabinet/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       80 2023-06-09 04:30:03.000000 cabinet-2023.6.8.1/src/cabinet/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       69 2023-05-31 04:50:50.000000 cabinet-2023.6.8.1/src/cabinet/__main__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    26147 2023-06-09 04:29:47.000000 cabinet-2023.6.8.1/src/cabinet/cabinet.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     3687 2023-04-16 16:59:23.000000 cabinet-2023.6.8.1/src/cabinet/mail.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-09 04:30:15.960220 cabinet-2023.6.8.1/src/cabinet.egg-info/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     6579 2023-06-09 04:30:15.000000 cabinet-2023.6.8.1/src/cabinet.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      333 2023-06-09 04:30:15.000000 cabinet-2023.6.8.1/src/cabinet.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-06-09 04:30:15.000000 cabinet-2023.6.8.1/src/cabinet.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2023-06-09 04:30:15.000000 cabinet-2023.6.8.1/src/cabinet.egg-info/entry_points.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2023-06-09 04:30:15.000000 cabinet-2023.6.8.1/src/cabinet.egg-info/top_level.txt
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-09 04:30:15.960220 cabinet-2023.6.8.1/test/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     5868 2023-05-31 04:52:07.000000 cabinet-2023.6.8.1/test/test___init__.py
```

### Comparing `cabinet-2023.5.31.3/LICENSE` & `cabinet-2023.6.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cabinet-2023.5.31.3/PKG-INFO` & `cabinet-2023.6.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cabinet
-Version: 2023.5.31.3
+Version: 2023.6.8.1
 Summary: Easily manage data storage and logging across repos
 Home-page: https://github.com/tylerjwoodfin/cabinet
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `cabinet-2023.5.31.3/README.md` & `cabinet-2023.6.8.1/README.md`

 * *Files identical despite different names*

### Comparing `cabinet-2023.5.31.3/src/cabinet/cabinet.py` & `cabinet-2023.6.8.1/src/cabinet/cabinet.py`

 * *Files 1% similar despite different names*

```diff
@@ -346,28 +346,30 @@
 
             - FileNotFoundError: If the file does not exist and create_if_not_exist is True.
 
         Returns:
             None
         """
 
+        path_edit = self.get("path", "edit")
+
         # edit settings.json if no file_path
         if file_path is None:
             message = (
                 "Enter the path of the file you want to edit "
                 f"(default: {self.path_cabinet}/settings.json):\n"
             )
 
             path = self.path_settings_file or input(
                 message) or f"{self.path_cabinet}/settings.json"
             self.edit_file(path)
             return
 
         # allows for shortcuts by setting paths in settings.json -> path -> edit
-        if file_path in self.get("path", "edit"):
+        if path_edit and file_path in path_edit:
             item = self.get("path", "edit", file_path)
             if not isinstance(item, dict) or "value" not in item.keys():
                 self.log(f"Could not use shortcut for {file_path} \
                     in getItem(path -> edit); should be a JSON object with value", level="warn")
             else:
                 file_path = item["value"]
```

### Comparing `cabinet-2023.5.31.3/src/cabinet/mail.py` & `cabinet-2023.6.8.1/src/cabinet/mail.py`

 * *Files identical despite different names*

### Comparing `cabinet-2023.5.31.3/src/cabinet.egg-info/PKG-INFO` & `cabinet-2023.6.8.1/src/cabinet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cabinet
-Version: 2023.5.31.3
+Version: 2023.6.8.1
 Summary: Easily manage data storage and logging across repos
 Home-page: https://github.com/tylerjwoodfin/cabinet
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `cabinet-2023.5.31.3/test/test___init__.py` & `cabinet-2023.6.8.1/test/test___init__.py`

 * *Files identical despite different names*

