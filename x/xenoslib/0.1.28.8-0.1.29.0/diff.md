# Comparing `tmp/xenoslib-0.1.28.8.tar.gz` & `tmp/xenoslib-0.1.29.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xenoslib-0.1.28.8.tar", last modified: Fri Jun  9 05:40:36 2023, max compression
+gzip compressed data, was "xenoslib-0.1.29.0.tar", last modified: Fri Jun  9 05:47:21 2023, max compression
```

## Comparing `xenoslib-0.1.28.8.tar` & `xenoslib-0.1.29.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:40:36.542197 xenoslib-0.1.28.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-09 05:40:22.000000 xenoslib-0.1.28.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-09 05:40:36.542197 xenoslib-0.1.28.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-09 05:40:22.000000 xenoslib-0.1.28.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 05:40:36.542197 xenoslib-0.1.28.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-09 05:40:22.000000 xenoslib-0.1.28.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:40:36.542197 xenoslib-0.1.28.8/xenoslib/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-09 05:40:22.000000 xenoslib-0.1.28.8/xenoslib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-09 05:40:22.000000 xenoslib-0.1.28.8/xenoslib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-09 05:40:22.000000 xenoslib-0.1.28.8/xenoslib/about.py
--rw-r--r--   0 runner    (1001) docker     (123)    11629 2023-06-09 05:40:22.000000 xenoslib-0.1.28.8/xenoslib/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-09 05:40:22.000000 xenoslib-0.1.28.8/xenoslib/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-06-09 05:40:22.000000 xenoslib-0.1.28.8/xenoslib/extend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-09 05:40:22.000000 xenoslib-0.1.28.8/xenoslib/linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-09 05:40:22.000000 xenoslib-0.1.28.8/xenoslib/mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-06-09 05:40:22.000000 xenoslib-0.1.28.8/xenoslib/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-06-09 05:40:22.000000 xenoslib-0.1.28.8/xenoslib/onedrive.py
--rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-06-09 05:40:22.000000 xenoslib-0.1.28.8/xenoslib/win_trayicon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-09 05:40:22.000000 xenoslib-0.1.28.8/xenoslib/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:40:36.542197 xenoslib-0.1.28.8/xenoslib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-09 05:40:36.000000 xenoslib-0.1.28.8/xenoslib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-09 05:40:36.000000 xenoslib-0.1.28.8/xenoslib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 05:40:36.000000 xenoslib-0.1.28.8/xenoslib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-09 05:40:36.000000 xenoslib-0.1.28.8/xenoslib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-09 05:40:36.000000 xenoslib-0.1.28.8/xenoslib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:47:21.372109 xenoslib-0.1.29.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-09 05:47:06.000000 xenoslib-0.1.29.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-09 05:47:21.372109 xenoslib-0.1.29.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-09 05:47:06.000000 xenoslib-0.1.29.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 05:47:21.372109 xenoslib-0.1.29.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-09 05:47:06.000000 xenoslib-0.1.29.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:47:21.372109 xenoslib-0.1.29.0/xenoslib/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-09 05:47:06.000000 xenoslib-0.1.29.0/xenoslib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-09 05:47:06.000000 xenoslib-0.1.29.0/xenoslib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-09 05:47:06.000000 xenoslib-0.1.29.0/xenoslib/about.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-06-09 05:47:06.000000 xenoslib-0.1.29.0/xenoslib/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-09 05:47:06.000000 xenoslib-0.1.29.0/xenoslib/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-06-09 05:47:06.000000 xenoslib-0.1.29.0/xenoslib/extend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-09 05:47:06.000000 xenoslib-0.1.29.0/xenoslib/linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-09 05:47:06.000000 xenoslib-0.1.29.0/xenoslib/mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-06-09 05:47:06.000000 xenoslib-0.1.29.0/xenoslib/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-06-09 05:47:06.000000 xenoslib-0.1.29.0/xenoslib/onedrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-06-09 05:47:06.000000 xenoslib-0.1.29.0/xenoslib/win_trayicon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-09 05:47:06.000000 xenoslib-0.1.29.0/xenoslib/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:47:21.372109 xenoslib-0.1.29.0/xenoslib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-09 05:47:21.000000 xenoslib-0.1.29.0/xenoslib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-09 05:47:21.000000 xenoslib-0.1.29.0/xenoslib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 05:47:21.000000 xenoslib-0.1.29.0/xenoslib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-09 05:47:21.000000 xenoslib-0.1.29.0/xenoslib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-09 05:47:21.000000 xenoslib-0.1.29.0/xenoslib.egg-info/top_level.txt
```

### Comparing `xenoslib-0.1.28.8/LICENSE` & `xenoslib-0.1.29.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.8/README.md` & `xenoslib-0.1.29.0/README.md`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.8/setup.py` & `xenoslib-0.1.29.0/setup.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.8/xenoslib/base.py` & `xenoslib-0.1.29.0/xenoslib/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -319,14 +319,40 @@
         module.__dict__[obj_name] = obj
         print(f"Monkey patched <{obj_name}> in <{module.__name__}>", file=sys.stderr)
     for k, v in module.__dict__.items():
         if inspect.ismodule(v) and v.__package__ == package:
             monkey_patch(v, obj_name, obj, package)
 
 
+def get_dict_val(dictionary, *args):
+    """
+    Usage:
+    my_dict = {"name": "John", "age": 30, "city": "New York"}
+    result = filter_dict_by_keys(environ, "CLIENT_SECRET", "age")
+    print(result)  # Output: {'name': 'John', 'age': 30}
+    """
+    return {key: value for key, value in dictionary.items() if key in args}
+
+
+def get_attr_val(obj, *args):
+    """
+    Usage:
+    class Person:
+        def __init__(self, name, age, city):
+            self.name = name
+            self.age = age
+            self.city = city
+
+    person = Person("John", 30, "New York")
+    attributes = get_attr_val(person, "name", "age")
+    print(attributes)  # Output: {'name': 'John', 'age': 30}
+    """
+    return {attr: getattr(obj, attr) for attr in args}
+
+
 if __name__ == "__main__":
     data = {"a": 1, "b": {"c": 2, "d": [3, 4, {"e": 5}]}, "f": (6, 7, {"g": 8})}
     n = NestedData(data)
 
     from pprint import pprint
 
     pprint(list(n.search("b")))
```

### Comparing `xenoslib-0.1.28.8/xenoslib/dev.py` & `xenoslib-0.1.29.0/xenoslib/dev.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.8/xenoslib/extend.py` & `xenoslib-0.1.29.0/xenoslib/extend.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.8/xenoslib/linux.py` & `xenoslib-0.1.29.0/xenoslib/linux.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.8/xenoslib/mail.py` & `xenoslib-0.1.29.0/xenoslib/mail.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.8/xenoslib/mock.py` & `xenoslib-0.1.29.0/xenoslib/mock.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.8/xenoslib/onedrive.py` & `xenoslib-0.1.29.0/xenoslib/onedrive.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.8/xenoslib/win_trayicon.py` & `xenoslib-0.1.29.0/xenoslib/win_trayicon.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.8/xenoslib/windows.py` & `xenoslib-0.1.29.0/xenoslib/windows.py`

 * *Files identical despite different names*

