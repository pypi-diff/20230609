# Comparing `tmp/googleapiutils2-0.9.4.tar.gz` & `tmp/googleapiutils2-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "googleapiutils2-0.9.4.tar", max compression
+gzip compressed data, was "googleapiutils2-0.9.5.tar", max compression
```

## Comparing `googleapiutils2-0.9.4.tar` & `googleapiutils2-0.9.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1069 2023-05-11 16:28:47.015700 googleapiutils2-0.9.4/LICENSE
--rw-r--r--   0        0        0     5214 2023-05-11 16:28:47.015936 googleapiutils2-0.9.4/README.md
--rw-r--r--   0        0        0      119 2023-06-02 03:26:51.461760 googleapiutils2-0.9.4/googleapiutils2/__init__.py
--rw-r--r--   0        0        0       25 2023-06-01 17:02:45.162747 googleapiutils2-0.9.4/googleapiutils2/drive/__init__.py
--rw-r--r--   0        0        0    21628 2023-06-08 02:25:59.112608 googleapiutils2-0.9.4/googleapiutils2/drive/drive.py
--rw-r--r--   0        0        0      314 2023-06-07 16:12:16.848980 googleapiutils2-0.9.4/googleapiutils2/drive/misc.py
--rw-r--r--   0        0        0       28 2022-12-30 01:32:12.341848 googleapiutils2-0.9.4/googleapiutils2/geocode/__init__.py
--rw-r--r--   0        0        0     1105 2023-06-02 03:24:36.559913 googleapiutils2-0.9.4/googleapiutils2/geocode/geocode.py
--rw-r--r--   0        0        0     1460 2023-06-01 21:02:51.625940 googleapiutils2-0.9.4/googleapiutils2/geocode/misc.py
--rw-r--r--   0        0        0      198 2023-06-01 17:02:24.139670 googleapiutils2-0.9.4/googleapiutils2/sheets/__init__.py
--rw-r--r--   0        0        0     9618 2023-06-02 19:09:36.958908 googleapiutils2-0.9.4/googleapiutils2/sheets/misc.py
--rw-r--r--   0        0        0    33736 2023-06-07 18:16:28.569445 googleapiutils2-0.9.4/googleapiutils2/sheets/sheets.py
--rw-r--r--   0        0        0     5219 2023-06-02 18:15:23.863635 googleapiutils2-0.9.4/googleapiutils2/sheets/sheets_value_range.py
--rw-r--r--   0        0        0     9430 2023-06-07 18:49:59.814378 googleapiutils2-0.9.4/googleapiutils2/utils.py
--rw-r--r--   0        0        0     1089 2023-06-08 02:47:17.467796 googleapiutils2-0.9.4/pyproject.toml
--rw-r--r--   0        0        0     6248 1970-01-01 00:00:00.000000 googleapiutils2-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-11 16:28:47.015700 googleapiutils2-0.9.5/LICENSE
+-rw-r--r--   0        0        0     5214 2023-05-11 16:28:47.015936 googleapiutils2-0.9.5/README.md
+-rw-r--r--   0        0        0      119 2023-06-02 03:26:51.461760 googleapiutils2-0.9.5/googleapiutils2/__init__.py
+-rw-r--r--   0        0        0       25 2023-06-01 17:02:45.162747 googleapiutils2-0.9.5/googleapiutils2/drive/__init__.py
+-rw-r--r--   0        0        0    22040 2023-06-09 19:21:45.977910 googleapiutils2-0.9.5/googleapiutils2/drive/drive.py
+-rw-r--r--   0        0        0      314 2023-06-07 16:12:16.848980 googleapiutils2-0.9.5/googleapiutils2/drive/misc.py
+-rw-r--r--   0        0        0       28 2022-12-30 01:32:12.341848 googleapiutils2-0.9.5/googleapiutils2/geocode/__init__.py
+-rw-r--r--   0        0        0     1105 2023-06-02 03:24:36.559913 googleapiutils2-0.9.5/googleapiutils2/geocode/geocode.py
+-rw-r--r--   0        0        0     1460 2023-06-01 21:02:51.625940 googleapiutils2-0.9.5/googleapiutils2/geocode/misc.py
+-rw-r--r--   0        0        0      198 2023-06-01 17:02:24.139670 googleapiutils2-0.9.5/googleapiutils2/sheets/__init__.py
+-rw-r--r--   0        0        0     9618 2023-06-02 19:09:36.958908 googleapiutils2-0.9.5/googleapiutils2/sheets/misc.py
+-rw-r--r--   0        0        0    33736 2023-06-07 18:16:28.569445 googleapiutils2-0.9.5/googleapiutils2/sheets/sheets.py
+-rw-r--r--   0        0        0     5219 2023-06-02 18:15:23.863635 googleapiutils2-0.9.5/googleapiutils2/sheets/sheets_value_range.py
+-rw-r--r--   0        0        0     9430 2023-06-07 18:49:59.814378 googleapiutils2-0.9.5/googleapiutils2/utils.py
+-rw-r--r--   0        0        0     1089 2023-06-09 19:22:10.168691 googleapiutils2-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0     6248 1970-01-01 00:00:00.000000 googleapiutils2-0.9.5/PKG-INFO
```

### Comparing `googleapiutils2-0.9.4/LICENSE` & `googleapiutils2-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.9.4/README.md` & `googleapiutils2-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.9.4/googleapiutils2/drive/drive.py` & `googleapiutils2-0.9.5/googleapiutils2/drive/drive.py`

 * *Files 2% similar despite different names*

```diff
@@ -346,23 +346,33 @@
             kwargs["body"]["parents"] = parents
         if mime_type is not None:
             kwargs["body"]["mimeType"] = mime_type.value
 
         file = self.files.create(**kwargs).execute()
         return file
 
-    def delete(self, file_id: str, **kwargs: Any):
+    def delete(self, file_id: str, trash: bool = True, **kwargs: Any):
         """Delete a file from Google Drive.
-        For more information, see: https://developers.google.com/drive/api/v3/reference/files/delete
+        If `trash` is True, the file will be moved to the trash. Otherwise, it will be deleted permanently.
+
+        For more information on deleting files, see: https://developers.google.com/drive/api/v3/reference/files/delete
 
         Args:
             file_id (str): The ID of the file to delete.
+            trash (bool, optional): Whether to trash the file instead of deleting it. Defaults to True.
         """
         file_id = parse_file_id(file_id)
-        return self.files.delete(fileId=file_id, **kwargs).execute()
+
+        if trash:
+            return self.files.update(
+                fileId=file_id,
+                body={"trashed": True},
+            )
+        else:
+            return self.files.delete(fileId=file_id, **kwargs).execute()
 
     def _upload(
         self,
         uploader: Callable[[GoogleMimeTypes], Any],
         name: str,
         filepath: FilePath,
         mime_type: GoogleMimeTypes | None = None,
```

### Comparing `googleapiutils2-0.9.4/googleapiutils2/geocode/geocode.py` & `googleapiutils2-0.9.5/googleapiutils2/geocode/geocode.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.9.4/googleapiutils2/geocode/misc.py` & `googleapiutils2-0.9.5/googleapiutils2/geocode/misc.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.9.4/googleapiutils2/sheets/misc.py` & `googleapiutils2-0.9.5/googleapiutils2/sheets/misc.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.9.4/googleapiutils2/sheets/sheets.py` & `googleapiutils2-0.9.5/googleapiutils2/sheets/sheets.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.9.4/googleapiutils2/sheets/sheets_value_range.py` & `googleapiutils2-0.9.5/googleapiutils2/sheets/sheets_value_range.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.9.4/googleapiutils2/utils.py` & `googleapiutils2-0.9.5/googleapiutils2/utils.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.9.4/pyproject.toml` & `googleapiutils2-0.9.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "googleapiutils2"
-version = "0.9.4"
+version = "0.9.5"
 description = "Wrapper for Google's Python API."
 authors = ["Mike Babb <mike7400@gmail.com>"]
 
 readme = "README.md"
 keywords = ["google", "googleapi", "googleapiutils2"]
 license = "MIT"
 repository = "https://github.com/mkbabb/googleapiutils2"
```

### Comparing `googleapiutils2-0.9.4/PKG-INFO` & `googleapiutils2-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: googleapiutils2
-Version: 0.9.4
+Version: 0.9.5
 Summary: Wrapper for Google's Python API.
 Home-page: https://github.com/mkbabb/googleapiutils2
 License: MIT
 Keywords: google,googleapi,googleapiutils2
 Author: Mike Babb
 Author-email: mike7400@gmail.com
 Requires-Python: >=3.10,<4.0
```

