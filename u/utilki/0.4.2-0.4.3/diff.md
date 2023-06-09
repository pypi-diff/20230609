# Comparing `tmp/utilki-0.4.2.tar.gz` & `tmp/utilki-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utilki-0.4.2.tar", max compression
+gzip compressed data, was "utilki-0.4.3.tar", max compression
```

## Comparing `utilki-0.4.2.tar` & `utilki-0.4.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1064 2023-06-09 12:49:02.071124 utilki-0.4.2/README.md
--rw-r--r--   0        0        0      525 2023-06-09 12:49:02.071124 utilki-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      269 2023-06-09 12:49:02.071124 utilki-0.4.2/utilki/__init__.py
--rw-r--r--   0        0        0     2184 2023-06-09 12:49:02.071124 utilki-0.4.2/utilki/cli.py
--rw-r--r--   0        0        0     5273 2023-06-09 12:49:02.071124 utilki-0.4.2/utilki/log_utils.py
--rw-r--r--   0        0        0     6381 2023-06-09 12:49:02.071124 utilki-0.4.2/utilki/task_mixin.py
--rw-r--r--   0        0        0     1659 1970-01-01 00:00:00.000000 utilki-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-09 15:57:24.421282 utilki-0.4.3/README.md
+-rw-r--r--   0        0        0      525 2023-06-09 15:57:24.421282 utilki-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0      269 2023-06-09 15:57:24.421282 utilki-0.4.3/utilki/__init__.py
+-rw-r--r--   0        0        0     2184 2023-06-09 15:57:24.421282 utilki-0.4.3/utilki/cli.py
+-rw-r--r--   0        0        0     5273 2023-06-09 15:57:24.421282 utilki-0.4.3/utilki/log_utils.py
+-rw-r--r--   0        0        0     6437 2023-06-09 15:57:24.421282 utilki-0.4.3/utilki/task_mixin.py
+-rw-r--r--   0        0        0     1659 1970-01-01 00:00:00.000000 utilki-0.4.3/PKG-INFO
```

### Comparing `utilki-0.4.2/README.md` & `utilki-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `utilki-0.4.2/pyproject.toml` & `utilki-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "utilki"
-version = "0.4.2"
+version = "0.4.3"
 description = "A collection of useful utilities"
 readme = "README.md"
 authors = ["Khaidar Bikmaev <khaidar@bikmaev.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.7"
 click = "^8.1.3"
```

### Comparing `utilki-0.4.2/utilki/cli.py` & `utilki-0.4.3/utilki/cli.py`

 * *Files identical despite different names*

### Comparing `utilki-0.4.2/utilki/log_utils.py` & `utilki-0.4.3/utilki/log_utils.py`

 * *Files identical despite different names*

### Comparing `utilki-0.4.2/utilki/task_mixin.py` & `utilki-0.4.3/utilki/task_mixin.py`

 * *Files 7% similar despite different names*

```diff
@@ -125,47 +125,47 @@
 def parse_options(value, type_):
     if value in ["None", "none", None, "null", "NULL", ""]:
         return None
     else:
         return type_(value)
 
 
-def parse_list(list_str: str, type_) -> List[Any]:
+def parse_list(list_str: str, type_, name_) -> List[Any]:
     if list_str.startswith("[") and list_str.endswith("]"):
         return json.loads(list_str)
     # TODO: make this a separate tuple parsing function
     # elif list_str.startswith("(") and list_str.endswith(")"):
     #     list_str.replace("(", "[")
     #     list_str.replace(")", "]")
     #     return json.loads(list_str)
     elif "," in list_str:
         return list(map(type_, list_str.split(",")))
     else:
-        raise ValueError("Invalid list format")
+        raise ValueError(f"Invalid list format {name_}: {list_str}")
 
 
 def get_date(param: str):
     n = [int(n) for n in param.split("-")]
     if len(n) == 3:
         return datetime(n[0], n[1], n[2])
     elif len(n) == 6:
         return datetime(n[0], n[1], n[2], n[3], n[4], n[5])
     else:
         raise ValueError("Invalid datetime format")
 
 
 def parse_variations(type_, value, name_):
     if type_ == List[int]:
-        return parse_list(value, int)
+        return parse_list(value, int, name_)
     elif type_ == List[str]:
-        return parse_list(value, str)
+        return parse_list(value, str, name_)
     elif type_ == List[float]:
-        return parse_list(value, float)
+        return parse_list(value, float, name_)
     elif type_ == List[bool]:
-        return parse_list(value, parse_bool)
+        return parse_list(value, parse_bool, name_)
     elif type_ == Union[int, None]:
         return parse_options(value, int)
     elif type_ == Union[str, None]:
         return parse_options(value, str)
     elif type_ == Union[float, None]:
         return parse_options(value, float)
     elif type_ == Union[bool, None]:
```

### Comparing `utilki-0.4.2/PKG-INFO` & `utilki-0.4.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilki
-Version: 0.4.2
+Version: 0.4.3
 Summary: A collection of useful utilities
 Author: Khaidar Bikmaev
 Author-email: khaidar@bikmaev.com
 Requires-Python: >=3.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

