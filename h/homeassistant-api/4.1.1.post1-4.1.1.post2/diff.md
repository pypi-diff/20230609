# Comparing `tmp/homeassistant_api-4.1.1.post1.tar.gz` & `tmp/homeassistant_api-4.1.1.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homeassistant_api-4.1.1.post1.tar", max compression
+gzip compressed data, was "homeassistant_api-4.1.1.post2.tar", max compression
```

## Comparing `homeassistant_api-4.1.1.post1.tar` & `homeassistant_api-4.1.1.post2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    32473 2023-04-14 18:04:37.583228 homeassistant_api-4.1.1.post1/LICENSE
--rw-r--r--   0        0        0     2069 2023-04-14 18:04:37.583228 homeassistant_api-4.1.1.post1/README.md
--rw-r--r--   0        0        0     1139 2023-04-14 18:04:37.587225 homeassistant_api-4.1.1.post1/homeassistant_api/__init__.py
--rw-r--r--   0        0        0     1313 2023-04-14 18:04:37.587225 homeassistant_api-4.1.1.post1/homeassistant_api/client.py
--rw-r--r--   0        0        0     2841 2023-04-14 18:04:37.587225 homeassistant_api-4.1.1.post1/homeassistant_api/errors.py
--rw-r--r--   0        0        0      474 2023-04-14 18:04:37.587225 homeassistant_api-4.1.1.post1/homeassistant_api/models/__init__.py
--rw-r--r--   0        0        0      594 2023-04-14 18:04:37.587225 homeassistant_api-4.1.1.post1/homeassistant_api/models/base.py
--rw-r--r--   0        0        0     4241 2023-04-14 18:04:37.587225 homeassistant_api-4.1.1.post1/homeassistant_api/models/domains.py
--rw-r--r--   0        0        0     4293 2023-04-14 18:04:37.587225 homeassistant_api-4.1.1.post1/homeassistant_api/models/entity.py
--rw-r--r--   0        0        0     1387 2023-04-14 18:04:37.587225 homeassistant_api-4.1.1.post1/homeassistant_api/models/events.py
--rw-r--r--   0        0        0      720 2023-04-14 18:04:37.587225 homeassistant_api-4.1.1.post1/homeassistant_api/models/history.py
--rw-r--r--   0        0        0      983 2023-04-14 18:04:37.587225 homeassistant_api-4.1.1.post1/homeassistant_api/models/logbook.py
--rw-r--r--   0        0        0     1322 2023-04-14 18:04:37.587225 homeassistant_api-4.1.1.post1/homeassistant_api/models/states.py
--rw-r--r--   0        0        0     5391 2023-04-14 18:04:37.587225 homeassistant_api-4.1.1.post1/homeassistant_api/processing.py
--rw-r--r--   0        0        0        0 2023-04-14 18:04:37.587225 homeassistant_api-4.1.1.post1/homeassistant_api/py.typed
--rw-r--r--   0        0        0    12645 2023-04-14 18:04:37.587225 homeassistant_api-4.1.1.post1/homeassistant_api/rawasyncclient.py
--rw-r--r--   0        0        0     5570 2023-04-14 18:04:37.587225 homeassistant_api-4.1.1.post1/homeassistant_api/rawbaseclient.py
--rw-r--r--   0        0        0    12191 2023-04-14 18:04:37.587225 homeassistant_api-4.1.1.post1/homeassistant_api/rawclient.py
--rw-r--r--   0        0        0     2267 2023-04-14 18:04:37.587225 homeassistant_api-4.1.1.post1/pyproject.toml
--rw-r--r--   0        0        0     3200 1970-01-01 00:00:00.000000 homeassistant_api-4.1.1.post1/PKG-INFO
+-rw-r--r--   0        0        0    32473 2023-06-09 19:40:05.689024 homeassistant_api-4.1.1.post2/LICENSE
+-rw-r--r--   0        0        0     2069 2023-06-09 19:40:05.689024 homeassistant_api-4.1.1.post2/README.md
+-rw-r--r--   0        0        0     1139 2023-06-09 19:40:05.689024 homeassistant_api-4.1.1.post2/homeassistant_api/__init__.py
+-rw-r--r--   0        0        0     1313 2023-06-09 19:40:05.693024 homeassistant_api-4.1.1.post2/homeassistant_api/client.py
+-rw-r--r--   0        0        0     2841 2023-06-09 19:40:05.693024 homeassistant_api-4.1.1.post2/homeassistant_api/errors.py
+-rw-r--r--   0        0        0      474 2023-06-09 19:40:05.693024 homeassistant_api-4.1.1.post2/homeassistant_api/models/__init__.py
+-rw-r--r--   0        0        0      594 2023-06-09 19:40:05.693024 homeassistant_api-4.1.1.post2/homeassistant_api/models/base.py
+-rw-r--r--   0        0        0     4241 2023-06-09 19:40:05.693024 homeassistant_api-4.1.1.post2/homeassistant_api/models/domains.py
+-rw-r--r--   0        0        0     4293 2023-06-09 19:40:05.693024 homeassistant_api-4.1.1.post2/homeassistant_api/models/entity.py
+-rw-r--r--   0        0        0     1387 2023-06-09 19:40:05.693024 homeassistant_api-4.1.1.post2/homeassistant_api/models/events.py
+-rw-r--r--   0        0        0      720 2023-06-09 19:40:05.693024 homeassistant_api-4.1.1.post2/homeassistant_api/models/history.py
+-rw-r--r--   0        0        0      983 2023-06-09 19:40:05.693024 homeassistant_api-4.1.1.post2/homeassistant_api/models/logbook.py
+-rw-r--r--   0        0        0     1322 2023-06-09 19:40:05.693024 homeassistant_api-4.1.1.post2/homeassistant_api/models/states.py
+-rw-r--r--   0        0        0     5447 2023-06-09 19:40:05.693024 homeassistant_api-4.1.1.post2/homeassistant_api/processing.py
+-rw-r--r--   0        0        0        0 2023-06-09 19:40:05.693024 homeassistant_api-4.1.1.post2/homeassistant_api/py.typed
+-rw-r--r--   0        0        0    12645 2023-06-09 19:40:05.693024 homeassistant_api-4.1.1.post2/homeassistant_api/rawasyncclient.py
+-rw-r--r--   0        0        0     5570 2023-06-09 19:40:05.693024 homeassistant_api-4.1.1.post2/homeassistant_api/rawbaseclient.py
+-rw-r--r--   0        0        0    12191 2023-06-09 19:40:05.693024 homeassistant_api-4.1.1.post2/homeassistant_api/rawclient.py
+-rw-r--r--   0        0        0     2268 2023-06-09 19:40:05.693024 homeassistant_api-4.1.1.post2/pyproject.toml
+-rw-r--r--   0        0        0     3200 1970-01-01 00:00:00.000000 homeassistant_api-4.1.1.post2/PKG-INFO
```

### Comparing `homeassistant_api-4.1.1.post1/LICENSE` & `homeassistant_api-4.1.1.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.1.1.post1/README.md` & `homeassistant_api-4.1.1.post2/README.md`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.1.1.post1/homeassistant_api/__init__.py` & `homeassistant_api-4.1.1.post2/homeassistant_api/__init__.py`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.1.1.post1/homeassistant_api/client.py` & `homeassistant_api-4.1.1.post2/homeassistant_api/client.py`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.1.1.post1/homeassistant_api/errors.py` & `homeassistant_api-4.1.1.post2/homeassistant_api/errors.py`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.1.1.post1/homeassistant_api/models/base.py` & `homeassistant_api-4.1.1.post2/homeassistant_api/models/base.py`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.1.1.post1/homeassistant_api/models/domains.py` & `homeassistant_api-4.1.1.post2/homeassistant_api/models/domains.py`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.1.1.post1/homeassistant_api/models/entity.py` & `homeassistant_api-4.1.1.post2/homeassistant_api/models/entity.py`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.1.1.post1/homeassistant_api/models/events.py` & `homeassistant_api-4.1.1.post2/homeassistant_api/models/events.py`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.1.1.post1/homeassistant_api/models/history.py` & `homeassistant_api-4.1.1.post2/homeassistant_api/models/history.py`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.1.1.post1/homeassistant_api/models/logbook.py` & `homeassistant_api-4.1.1.post2/homeassistant_api/models/logbook.py`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.1.1.post1/homeassistant_api/models/states.py` & `homeassistant_api-4.1.1.post2/homeassistant_api/models/states.py`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.1.1.post1/homeassistant_api/processing.py` & `homeassistant_api-4.1.1.post2/homeassistant_api/processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,18 +55,19 @@
 
     def process_content(self, *, async_: bool = False) -> Any:
         """
         Looks up processors by their Content-Type header and then
         calls the processor with the response.
         """
 
-        mimetype = self._response.headers.get(  # type: ignore [arg-type]
+        mimetype_header = self._response.headers.get(  # type: ignore [arg-type]
             "content-type",
             "text/plain",
         )
+        mimetype = mimetype_header.split(";")[0]
         for processor in self._processors.get(mimetype, ()):
             if not async_ ^ inspect.iscoroutinefunction(processor):
                 logger.debug("Using processor %r on %r", processor, self._response)
                 return processor(self._response)
         raise ProcessorNotFoundError(
             f"No response processor found for mimetype {mimetype!r}."
         )
```

### Comparing `homeassistant_api-4.1.1.post1/homeassistant_api/rawasyncclient.py` & `homeassistant_api-4.1.1.post2/homeassistant_api/rawasyncclient.py`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.1.1.post1/homeassistant_api/rawbaseclient.py` & `homeassistant_api-4.1.1.post2/homeassistant_api/rawbaseclient.py`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.1.1.post1/homeassistant_api/rawclient.py` & `homeassistant_api-4.1.1.post2/homeassistant_api/rawclient.py`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.1.1.post1/pyproject.toml` & `homeassistant_api-4.1.1.post2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 documentation = "https://homeassistantapi.readthedocs.io"
 homepage = "https://github.com/GrandMoff100/HomeAssistantAPI"
 license = "GPL-3.0-or-later"
 name = "HomeAssistant-API"
 readme = "README.md"
 include = ["homeassistant_api/py.typed"]
 repository = "https://github.com/GrandMoff100/HomeAssistantAPI"
-version = "4.1.1.post1"
+version = "4.1.1.post2"
 packages = [{ include = "homeassistant_api" }]
 
 [tool.poetry.dependencies]
 aiohttp = "^3.8.1"
 aiohttp-client-cache = "^0.6.1"
 pydantic = "<=1.9.0"
 python = "^3.7,<4.0.0"
@@ -91,8 +91,8 @@
 [tool.isort]
 profile = "black"
 
 [tool.mypy]
 disable_error_code = [
     "no-untyped-def",
     "name-defined",
-]
+]
```

### Comparing `homeassistant_api-4.1.1.post1/PKG-INFO` & `homeassistant_api-4.1.1.post2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeassistant-api
-Version: 4.1.1.post1
+Version: 4.1.1.post2
 Summary: Python Wrapper for Homeassistant's REST API
 Home-page: https://github.com/GrandMoff100/HomeAssistantAPI
 License: GPL-3.0-or-later
 Author: GrandMoff100
 Author-email: minecraftcrusher100@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: homeassistant-api Version: 4.1.1.post1 Summary:
+Metadata-Version: 2.1 Name: homeassistant-api Version: 4.1.1.post2 Summary:
 Python Wrapper for Homeassistant's REST API Home-page: https://github.com/
 GrandMoff100/HomeAssistantAPI License: GPL-3.0-or-later Author: GrandMoff100
 Author-email: minecraftcrusher100@gmail.com Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later
 (GPLv3+) Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

