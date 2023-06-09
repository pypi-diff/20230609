# Comparing `tmp/pybash-0.3.2.tar.gz` & `tmp/pybash-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybash-0.3.2.tar", max compression
+gzip compressed data, was "pybash-0.3.3.tar", max compression
```

## Comparing `pybash-0.3.2.tar` & `pybash-0.3.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1060 2023-05-25 01:42:43.603008 pybash-0.3.2/LICENSE
--rw-r--r--   0        0        0     4055 2023-05-25 01:42:43.603008 pybash-0.3.2/README.md
--rw-r--r--   0        0        0        0 2023-05-25 01:42:43.603008 pybash-0.3.2/pybash/__init__.py
--rw-r--r--   0        0        0      684 2023-05-25 01:42:43.603008 pybash-0.3.2/pybash/__main__.py
--rw-r--r--   0        0        0      531 2023-05-25 01:42:43.603008 pybash-0.3.2/pybash/hook.py
--rw-r--r--   0        0        0    15560 2023-05-25 01:42:43.603008 pybash-0.3.2/pybash/transformer.py
--rw-r--r--   0        0        0      792 2023-05-25 01:42:43.603008 pybash-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     4599 1970-01-01 00:00:00.000000 pybash-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-06-09 02:00:03.224966 pybash-0.3.3/LICENSE
+-rw-r--r--   0        0        0     4055 2023-06-09 02:00:03.224966 pybash-0.3.3/README.md
+-rw-r--r--   0        0        0        0 2023-06-09 02:00:03.224966 pybash-0.3.3/pybash/__init__.py
+-rw-r--r--   0        0        0      684 2023-06-09 02:00:03.224966 pybash-0.3.3/pybash/__main__.py
+-rw-r--r--   0        0        0      531 2023-06-09 02:00:03.224966 pybash-0.3.3/pybash/hook.py
+-rw-r--r--   0        0        0    15694 2023-06-09 02:00:03.224966 pybash-0.3.3/pybash/transformer.py
+-rw-r--r--   0        0        0      792 2023-06-09 02:00:03.224966 pybash-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     4599 1970-01-01 00:00:00.000000 pybash-0.3.3/PKG-INFO
```

### Comparing `pybash-0.3.2/LICENSE` & `pybash-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pybash-0.3.2/README.md` & `pybash-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pybash-0.3.2/pybash/__main__.py` & `pybash-0.3.3/pybash/__main__.py`

 * *Files identical despite different names*

### Comparing `pybash-0.3.2/pybash/hook.py` & `pybash-0.3.3/pybash/hook.py`

 * *Files identical despite different names*

### Comparing `pybash-0.3.2/pybash/transformer.py` & `pybash-0.3.3/pybash/transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
         if not subs:
             return parsed_command
 
         for sub in subs:
             parsed_command = re.sub(pattern, '" + f\"\"\"{' + sub + '}\"\"\" + "', parsed_command, 1)
 
-        return parsed_command
+        return parsed_command.replace('"" + f"""', 'f"""').replace('""" + ""', '"""')
 
     @staticmethod
     def direct_interpolate(string: str) -> str:
         """Process {{ static interpolations }} and substitute.
             Static interpolations are denotated by a {{ }} with a variable or a function call inside.
             Substitution happens directly on the parsed command string. Therefore, certain characters
             cannot be interpolated as they get parsed out before substitution.
@@ -69,15 +69,16 @@
 
         # validate interpolation
         invalid_chars = [' ', '"', "'"]
         matches = re.findall(r'{{(.+?)}}', string)
         if matches and any(any(bad_char in match for bad_char in invalid_chars) for match in matches):
             raise InvalidInterpolation
 
-        return re.sub(r'{{(.+?)}}', r'" + \1 + "', string)
+        interpolated = re.sub(r'{{(.+?)}}', r'" + \1 + "', string)
+        return interpolated.replace('"" + ', '').replace(' + ""', '')
 
 
 class Shelled(Processor):
     # $ls .github/*
     command_char = ">"
 
     def transform(self) -> token_utils.Token:
```

### Comparing `pybash-0.3.2/pyproject.toml` & `pybash-0.3.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PyBash"
-version = "0.3.2"
+version = "0.3.3"
 description = ">execute bash commands from python easily"
 authors = ["Jay <jay.github0@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pybash"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `pybash-0.3.2/PKG-INFO` & `pybash-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybash
-Version: 0.3.2
+Version: 0.3.3
 Summary: >execute bash commands from python easily
 Author: Jay
 Author-email: jay.github0@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

