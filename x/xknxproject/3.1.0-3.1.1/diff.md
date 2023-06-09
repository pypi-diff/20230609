# Comparing `tmp/xknxproject-3.1.0.tar.gz` & `tmp/xknxproject-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xknxproject-3.1.0.tar", last modified: Mon May  8 19:58:19 2023, max compression
+gzip compressed data, was "xknxproject-3.1.1.tar", last modified: Fri Jun  9 21:16:56 2023, max compression
```

## Comparing `xknxproject-3.1.0.tar` & `xknxproject-3.1.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:58:19.546286 xknxproject-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-08 19:58:00.000000 xknxproject-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-08 19:58:00.000000 xknxproject-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    23615 2023-05-08 19:58:19.546286 xknxproject-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-08 19:58:00.000000 xknxproject-3.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-08 19:58:00.000000 xknxproject-3.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-08 19:58:19.546286 xknxproject-3.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:58:19.546286 xknxproject-3.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-08 19:58:00.000000 xknxproject-3.1.0/test/test_knxproj.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-08 19:58:00.000000 xknxproject-3.1.0/test/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:58:19.546286 xknxproject-3.1.0/xknxproject/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:58:19.546286 xknxproject-3.1.0/xknxproject/combination/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/combination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/combination/combination.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:58:19.546286 xknxproject-3.1.0/xknxproject/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:58:19.546286 xknxproject-3.1.0/xknxproject/loader/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/loader/application_program_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/loader/hardware_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/loader/knx_master_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10840 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/loader/project_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:58:19.546286 xknxproject-3.1.0/xknxproject/models/
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/models/knxproject.py
--rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/models/static.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/xknxproj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:58:19.546286 xknxproject-3.1.0/xknxproject/xml/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10201 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/xml/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:58:19.546286 xknxproject-3.1.0/xknxproject/zip/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/zip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-05-08 19:58:00.000000 xknxproject-3.1.0/xknxproject/zip/extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:58:19.546286 xknxproject-3.1.0/xknxproject.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23615 2023-05-08 19:58:18.000000 xknxproject-3.1.0/xknxproject.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-08 19:58:19.000000 xknxproject-3.1.0/xknxproject.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 19:58:18.000000 xknxproject-3.1.0/xknxproject.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-08 19:58:19.000000 xknxproject-3.1.0/xknxproject.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-08 19:58:19.000000 xknxproject-3.1.0/xknxproject.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:16:56.977818 xknxproject-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-09 21:16:39.000000 xknxproject-3.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-09 21:16:39.000000 xknxproject-3.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    23615 2023-06-09 21:16:56.981818 xknxproject-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-06-09 21:16:39.000000 xknxproject-3.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-06-09 21:16:39.000000 xknxproject-3.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-09 21:16:56.981818 xknxproject-3.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:16:56.977818 xknxproject-3.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-09 21:16:39.000000 xknxproject-3.1.1/test/test_knxproj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-09 21:16:39.000000 xknxproject-3.1.1/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:16:56.977818 xknxproject-3.1.1/xknxproject/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:16:56.977818 xknxproject-3.1.1/xknxproject/combination/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/combination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/combination/combination.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:16:56.977818 xknxproject-3.1.1/xknxproject/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:16:56.977818 xknxproject-3.1.1/xknxproject/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/loader/application_program_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/loader/hardware_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/loader/knx_master_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10840 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/loader/project_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:16:56.977818 xknxproject-3.1.1/xknxproject/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/models/knxproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/models/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/xknxproj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:16:56.977818 xknxproject-3.1.1/xknxproject/xml/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10458 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/xml/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:16:56.977818 xknxproject-3.1.1/xknxproject/zip/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/zip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-06-09 21:16:39.000000 xknxproject-3.1.1/xknxproject/zip/extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:16:56.977818 xknxproject-3.1.1/xknxproject.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23615 2023-06-09 21:16:56.000000 xknxproject-3.1.1/xknxproject.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-09 21:16:56.000000 xknxproject-3.1.1/xknxproject.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 21:16:56.000000 xknxproject-3.1.1/xknxproject.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-09 21:16:56.000000 xknxproject-3.1.1/xknxproject.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-09 21:16:56.000000 xknxproject-3.1.1/xknxproject.egg-info/top_level.txt
```

### Comparing `xknxproject-3.1.0/LICENSE` & `xknxproject-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xknxproject-3.1.0/PKG-INFO` & `xknxproject-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xknxproject
-Version: 3.1.0
+Version: 3.1.1
 Summary: A library to gather information from ETS project files used for KNX
 Author-email: Marvin Wichmann <me@marvin-wichmann.de>, Matthias Alphart <farmio@alphart.net>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

### Comparing `xknxproject-3.1.0/README.md` & `xknxproject-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `xknxproject-3.1.0/pyproject.toml` & `xknxproject-3.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xknxproject-3.1.0/test/test_knxproj.py` & `xknxproject-3.1.1/test/test_knxproj.py`

 * *Files identical despite different names*

### Comparing `xknxproject-3.1.0/test/test_util.py` & `xknxproject-3.1.1/test/test_util.py`

 * *Files identical despite different names*

### Comparing `xknxproject-3.1.0/xknxproject/combination/combination.py` & `xknxproject-3.1.1/xknxproject/combination/combination.py`

 * *Files identical despite different names*

### Comparing `xknxproject-3.1.0/xknxproject/loader/application_program_loader.py` & `xknxproject-3.1.1/xknxproject/loader/application_program_loader.py`

 * *Files identical despite different names*

### Comparing `xknxproject-3.1.0/xknxproject/loader/hardware_loader.py` & `xknxproject-3.1.1/xknxproject/loader/hardware_loader.py`

 * *Files identical despite different names*

### Comparing `xknxproject-3.1.0/xknxproject/loader/knx_master_loader.py` & `xknxproject-3.1.1/xknxproject/loader/knx_master_loader.py`

 * *Files identical despite different names*

### Comparing `xknxproject-3.1.0/xknxproject/loader/project_loader.py` & `xknxproject-3.1.1/xknxproject/loader/project_loader.py`

 * *Files identical despite different names*

### Comparing `xknxproject-3.1.0/xknxproject/models/__init__.py` & `xknxproject-3.1.1/xknxproject/models/__init__.py`

 * *Files identical despite different names*

### Comparing `xknxproject-3.1.0/xknxproject/models/knxproject.py` & `xknxproject-3.1.1/xknxproject/models/knxproject.py`

 * *Files identical despite different names*

### Comparing `xknxproject-3.1.0/xknxproject/models/models.py` & `xknxproject-3.1.1/xknxproject/models/models.py`

 * *Files identical despite different names*

### Comparing `xknxproject-3.1.0/xknxproject/models/static.py` & `xknxproject-3.1.1/xknxproject/models/static.py`

 * *Files identical despite different names*

### Comparing `xknxproject-3.1.0/xknxproject/util.py` & `xknxproject-3.1.1/xknxproject/util.py`

 * *Files identical despite different names*

### Comparing `xknxproject-3.1.0/xknxproject/xknxproj.py` & `xknxproject-3.1.1/xknxproject/xknxproj.py`

 * *Files identical despite different names*

### Comparing `xknxproject-3.1.0/xknxproject/xml/parser.py` & `xknxproject-3.1.1/xknxproject/xml/parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,39 +54,46 @@
         _ga_id_to_address = {ga.identifier: ga.address for ga in self.group_addresses}
 
         communication_objects: dict[str, CommunicationObject] = {}
         devices_dict: dict[str, Device] = {}
         for device in self.devices:
             device_com_objects: list[str] = []
             for com_object in device.com_object_instance_refs:
-                if com_object.links:
-                    com_object_key = f"{device.individual_address}/{com_object.ref_id}"
-                    group_address_links = [
-                        _ga_id_to_address[link] for link in com_object.links
-                    ]
-                    communication_objects[com_object_key] = CommunicationObject(
-                        name=com_object.name,  # type: ignore[typeddict-item]
-                        number=com_object.number,  # type: ignore[typeddict-item]
-                        text=com_object.text,  # type: ignore[typeddict-item]
-                        function_text=com_object.function_text,  # type: ignore[typeddict-item]
-                        description=com_object.description or "",
-                        device_address=device.individual_address,
-                        dpts=com_object.datapoint_types,
-                        object_size=com_object.object_size,  # type: ignore[typeddict-item]
-                        flags=Flags(
-                            read=com_object.read_flag,  # type: ignore[typeddict-item]
-                            write=com_object.write_flag,  # type: ignore[typeddict-item]
-                            communication=com_object.communication_flag,  # type: ignore[typeddict-item]
-                            update=com_object.update_flag,  # type: ignore[typeddict-item]
-                            read_on_init=com_object.read_on_init_flag,  # type: ignore[typeddict-item]
-                            transmit=com_object.transmit_flag,  # type: ignore[typeddict-item]
-                        ),
-                        group_address_links=group_address_links,
-                    )
-                    device_com_objects.append(com_object_key)
+                if not com_object.links:
+                    continue
+                group_address_links = [
+                    valid_link
+                    for link in com_object.links
+                    if (valid_link := _ga_id_to_address.get(link))
+                ]
+                if not group_address_links:
+                    # skip orphaned ComObjectInstanceRef pointing only to non-existent GroupAddress
+                    # see https://github.com/XKNX/knx-frontend/issues/71
+                    continue
+                com_object_key = f"{device.individual_address}/{com_object.ref_id}"
+                communication_objects[com_object_key] = CommunicationObject(
+                    name=com_object.name,  # type: ignore[typeddict-item]
+                    number=com_object.number,  # type: ignore[typeddict-item]
+                    text=com_object.text,  # type: ignore[typeddict-item]
+                    function_text=com_object.function_text,  # type: ignore[typeddict-item]
+                    description=com_object.description or "",
+                    device_address=device.individual_address,
+                    dpts=com_object.datapoint_types,
+                    object_size=com_object.object_size,  # type: ignore[typeddict-item]
+                    flags=Flags(
+                        read=com_object.read_flag,  # type: ignore[typeddict-item]
+                        write=com_object.write_flag,  # type: ignore[typeddict-item]
+                        communication=com_object.communication_flag,  # type: ignore[typeddict-item]
+                        update=com_object.update_flag,  # type: ignore[typeddict-item]
+                        read_on_init=com_object.read_on_init_flag,  # type: ignore[typeddict-item]
+                        transmit=com_object.transmit_flag,  # type: ignore[typeddict-item]
+                    ),
+                    group_address_links=group_address_links,
+                )
+                device_com_objects.append(com_object_key)
 
             devices_dict[device.individual_address] = Device(
                 name=device.product_name,
                 hardware_name=device.hardware_name,
                 description=device.description,
                 manufacturer_name=device.manufacturer_name,
                 individual_address=device.individual_address,
```

### Comparing `xknxproject-3.1.0/xknxproject/zip/extractor.py` & `xknxproject-3.1.1/xknxproject/zip/extractor.py`

 * *Files identical despite different names*

### Comparing `xknxproject-3.1.0/xknxproject.egg-info/PKG-INFO` & `xknxproject-3.1.1/xknxproject.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xknxproject
-Version: 3.1.0
+Version: 3.1.1
 Summary: A library to gather information from ETS project files used for KNX
 Author-email: Marvin Wichmann <me@marvin-wichmann.de>, Matthias Alphart <farmio@alphart.net>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

### Comparing `xknxproject-3.1.0/xknxproject.egg-info/SOURCES.txt` & `xknxproject-3.1.1/xknxproject.egg-info/SOURCES.txt`

 * *Files identical despite different names*

