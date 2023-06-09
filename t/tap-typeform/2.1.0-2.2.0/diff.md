# Comparing `tmp/tap-typeform-2.1.0.tar.gz` & `tmp/tap-typeform-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tap-typeform-2.1.0.tar", last modified: Wed Apr 26 05:22:26 2023, max compression
+gzip compressed data, was "dist/tap-typeform-2.2.0.tar", last modified: Wed May 31 15:24:22 2023, max compression
```

## Comparing `tap-typeform-2.1.0.tar` & `tap-typeform-2.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 05:22:26.000000 tap-typeform-2.1.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       52 2022-11-02 08:28:59.000000 tap-typeform-2.1.0/MANIFEST.in
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 05:22:26.000000 tap-typeform-2.1.0/tap_typeform/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6601 2022-11-02 08:28:59.000000 tap-typeform-2.1.0/tap_typeform/client.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 05:22:26.000000 tap-typeform-2.1.0/tap_typeform/schemas/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5375 2022-11-02 08:28:59.000000 tap-typeform-2.1.0/tap_typeform/schemas/questions.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      584 2022-11-02 08:28:59.000000 tap-typeform-2.1.0/tap_typeform/schemas/answers.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      777 2022-11-02 08:28:59.000000 tap-typeform-2.1.0/tap_typeform/schemas/unsubmitted_landings.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1068 2022-11-02 08:28:59.000000 tap-typeform-2.1.0/tap_typeform/schemas/forms.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      793 2022-11-02 08:28:59.000000 tap-typeform-2.1.0/tap_typeform/schemas/submitted_landings.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14553 2023-04-26 05:15:57.000000 tap-typeform-2.1.0/tap_typeform/streams.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1889 2022-11-02 08:28:59.000000 tap-typeform-2.1.0/tap_typeform/schema.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1601 2023-04-26 05:15:57.000000 tap-typeform-2.1.0/tap_typeform/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3087 2023-04-26 05:15:57.000000 tap-typeform-2.1.0/tap_typeform/sync.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1021 2022-11-02 08:28:59.000000 tap-typeform-2.1.0/tap_typeform/discover.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 05:22:26.000000 tap-typeform-2.1.0/tap_typeform.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       96 2023-04-26 05:22:26.000000 tap-typeform-2.1.0/tap_typeform.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-26 05:22:26.000000 tap-typeform-2.1.0/tap_typeform.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       62 2023-04-26 05:22:26.000000 tap-typeform-2.1.0/tap_typeform.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      312 2023-04-26 05:22:26.000000 tap-typeform-2.1.0/tap_typeform.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      601 2023-04-26 05:22:26.000000 tap-typeform-2.1.0/tap_typeform.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       13 2023-04-26 05:22:26.000000 tap-typeform-2.1.0/tap_typeform.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      100 2023-04-26 05:22:26.000000 tap-typeform-2.1.0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      312 2023-04-26 05:22:26.000000 tap-typeform-2.1.0/PKG-INFO
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      837 2023-04-26 05:15:57.000000 tap-typeform-2.1.0/setup.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32393 2022-11-02 08:28:59.000000 tap-typeform-2.1.0/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3117 2022-11-02 08:28:59.000000 tap-typeform-2.1.0/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 15:24:22.000000 tap-typeform-2.2.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       52 2022-11-02 08:28:59.000000 tap-typeform-2.2.0/MANIFEST.in
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 15:24:22.000000 tap-typeform-2.2.0/tap_typeform/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6601 2023-05-31 15:24:01.000000 tap-typeform-2.2.0/tap_typeform/client.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 15:24:22.000000 tap-typeform-2.2.0/tap_typeform/schemas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5375 2023-05-31 15:24:01.000000 tap-typeform-2.2.0/tap_typeform/schemas/questions.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      584 2023-05-31 15:24:01.000000 tap-typeform-2.2.0/tap_typeform/schemas/answers.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      777 2023-05-31 15:24:01.000000 tap-typeform-2.2.0/tap_typeform/schemas/unsubmitted_landings.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1068 2023-05-31 15:24:01.000000 tap-typeform-2.2.0/tap_typeform/schemas/forms.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      907 2023-05-31 15:24:05.000000 tap-typeform-2.2.0/tap_typeform/schemas/submitted_landings.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14597 2023-05-31 15:24:05.000000 tap-typeform-2.2.0/tap_typeform/streams.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1889 2023-05-31 15:24:01.000000 tap-typeform-2.2.0/tap_typeform/schema.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1601 2023-05-31 15:24:01.000000 tap-typeform-2.2.0/tap_typeform/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3087 2023-05-31 15:24:01.000000 tap-typeform-2.2.0/tap_typeform/sync.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1021 2023-05-31 15:24:01.000000 tap-typeform-2.2.0/tap_typeform/discover.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 15:24:22.000000 tap-typeform-2.2.0/tap_typeform.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       96 2023-05-31 15:24:22.000000 tap-typeform-2.2.0/tap_typeform.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-31 15:24:22.000000 tap-typeform-2.2.0/tap_typeform.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       62 2023-05-31 15:24:22.000000 tap-typeform-2.2.0/tap_typeform.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      312 2023-05-31 15:24:22.000000 tap-typeform-2.2.0/tap_typeform.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      601 2023-05-31 15:24:22.000000 tap-typeform-2.2.0/tap_typeform.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       13 2023-05-31 15:24:22.000000 tap-typeform-2.2.0/tap_typeform.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      100 2023-05-31 15:24:22.000000 tap-typeform-2.2.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      312 2023-05-31 15:24:22.000000 tap-typeform-2.2.0/PKG-INFO
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      837 2023-05-31 15:24:05.000000 tap-typeform-2.2.0/setup.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32393 2022-11-02 08:28:59.000000 tap-typeform-2.2.0/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3117 2023-05-31 15:24:01.000000 tap-typeform-2.2.0/README.md
```

### Comparing `tap-typeform-2.1.0/tap_typeform/client.py` & `tap-typeform-2.2.0/tap_typeform/client.py`

 * *Files identical despite different names*

### Comparing `tap-typeform-2.1.0/tap_typeform/schemas/questions.json` & `tap-typeform-2.2.0/tap_typeform/schemas/questions.json`

 * *Files identical despite different names*

### Comparing `tap-typeform-2.1.0/tap_typeform/schemas/answers.json` & `tap-typeform-2.2.0/tap_typeform/schemas/answers.json`

 * *Files identical despite different names*

### Comparing `tap-typeform-2.1.0/tap_typeform/schemas/unsubmitted_landings.json` & `tap-typeform-2.2.0/tap_typeform/schemas/unsubmitted_landings.json`

 * *Files identical despite different names*

### Comparing `tap-typeform-2.1.0/tap_typeform/schemas/forms.json` & `tap-typeform-2.2.0/tap_typeform/schemas/forms.json`

 * *Files identical despite different names*

### Comparing `tap-typeform-2.1.0/tap_typeform/schemas/submitted_landings.json` & `tap-typeform-2.2.0/tap_typeform/schemas/submitted_landings.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.986111111111111%*

 * *Differences: {"'properties'": "{'tags': OrderedDict([('type', ['null', 'array']), ('items', "*

 * *                 "OrderedDict([('type', ['null', 'string'])]))])}"}*

```diff
@@ -53,14 +53,26 @@
         "submitted_at": {
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
+        "tags": {
+            "items": {
+                "type": [
+                    "null",
+                    "string"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
+            ]
+        },
         "token": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "user_agent": {
```

### Comparing `tap-typeform-2.1.0/tap_typeform/streams.py` & `tap-typeform-2.2.0/tap_typeform/streams.py`

 * *Files 0% similar despite different names*

```diff
@@ -272,14 +272,15 @@
     child_data_key = 'answers'
 
     def add_fields_at_1st_level(self, record, additional_data={}):
         """
         Add additional data and nested fields to top level
         """
         record.update({
+                "tags": record.get("tags"),
                 "_sdc_form_id": additional_data["_sdc_form_id"],
                 "user_agent": record["metadata"]["user_agent"],
                 "platform": record["metadata"]["platform"],
                 "referer": record["metadata"]["referer"],
                 "network_id": record["metadata"]["network_id"],
                 "browser": record["metadata"]["browser"],
                 "hidden": json.dumps(record["hidden"]) if "hidden" in record else ""
```

### Comparing `tap-typeform-2.1.0/tap_typeform/schema.py` & `tap-typeform-2.2.0/tap_typeform/schema.py`

 * *Files identical despite different names*

### Comparing `tap-typeform-2.1.0/tap_typeform/__init__.py` & `tap-typeform-2.2.0/tap_typeform/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-typeform-2.1.0/tap_typeform/sync.py` & `tap-typeform-2.2.0/tap_typeform/sync.py`

 * *Files identical despite different names*

### Comparing `tap-typeform-2.1.0/tap_typeform/discover.py` & `tap-typeform-2.2.0/tap_typeform/discover.py`

 * *Files identical despite different names*

### Comparing `tap-typeform-2.1.0/tap_typeform.egg-info/SOURCES.txt` & `tap-typeform-2.2.0/tap_typeform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tap-typeform-2.1.0/setup.py` & `tap-typeform-2.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(
     name="tap-typeform",
-    version="2.1.0",
+    version="2.2.0",
     description="Singer.io tap for extracting data from the TypeForm Responses API",
     author="bytcode.io",
     url="http://singer.io",
     classifiers=["Programming Language :: Python :: 3 :: Only"],
     install_requires=[
         "singer-python==5.10.0",
         "pendulum",
```

### Comparing `tap-typeform-2.1.0/LICENSE` & `tap-typeform-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-typeform-2.1.0/README.md` & `tap-typeform-2.2.0/README.md`

 * *Files identical despite different names*

