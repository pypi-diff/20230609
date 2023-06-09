# Comparing `tmp/kepconfig-1.2.0.tar.gz` & `tmp/kepconfig-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kepconfig-1.2.0.tar", last modified: Fri Apr 21 18:38:17 2023, max compression
+gzip compressed data, was "kepconfig-1.2.1.tar", last modified: Fri Apr 28 20:00:58 2023, max compression
```

## Comparing `kepconfig-1.2.0.tar` & `kepconfig-1.2.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 18:38:17.024515 kepconfig-1.2.0/
--rw-rw-rw-   0        0        0     1127 2021-03-15 20:50:21.000000 kepconfig-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     6530 2023-04-21 18:38:17.022519 kepconfig-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     5624 2023-04-21 17:39:00.000000 kepconfig-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 18:38:16.926799 kepconfig-1.2.0/kepconfig/
--rw-rw-rw-   0        0        0      901 2023-04-21 18:37:58.000000 kepconfig-1.2.0/kepconfig/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 18:38:16.953955 kepconfig-1.2.0/kepconfig/admin/
--rw-rw-rw-   0        0        0      495 2023-03-31 19:09:46.000000 kepconfig-1.2.0/kepconfig/admin/__init__.py
--rw-rw-rw-   0        0        0     6776 2023-04-21 17:03:24.000000 kepconfig-1.2.0/kepconfig/admin/lls.py
--rw-rw-rw-   0        0        0     5316 2023-04-21 17:29:29.000000 kepconfig-1.2.0/kepconfig/admin/ua_server.py
--rw-rw-rw-   0        0        0     6507 2023-04-21 17:29:29.000000 kepconfig-1.2.0/kepconfig/admin/user_groups.py
--rw-rw-rw-   0        0        0     6139 2023-04-21 17:29:29.000000 kepconfig-1.2.0/kepconfig/admin/users.py
--rw-rw-rw-   0        0        0    20553 2023-04-20 20:32:21.000000 kepconfig-1.2.0/kepconfig/connection.py
-drwxrwxrwx   0        0        0        0 2023-04-21 18:38:16.968973 kepconfig-1.2.0/kepconfig/connectivity/
--rw-rw-rw-   0        0        0      759 2023-03-31 19:09:38.000000 kepconfig-1.2.0/kepconfig/connectivity/__init__.py
--rw-rw-rw-   0        0        0     7831 2023-04-21 17:29:29.000000 kepconfig-1.2.0/kepconfig/connectivity/channel.py
--rw-rw-rw-   0        0        0    11083 2023-04-21 17:29:29.000000 kepconfig-1.2.0/kepconfig/connectivity/device.py
-drwxrwxrwx   0        0        0        0 2023-04-21 18:38:16.983473 kepconfig-1.2.0/kepconfig/connectivity/egd/
--rw-rw-rw-   0        0        0      517 2023-03-31 19:17:27.000000 kepconfig-1.2.0/kepconfig/connectivity/egd/__init__.py
--rw-rw-rw-   0        0        0     8753 2023-04-21 17:29:29.000000 kepconfig-1.2.0/kepconfig/connectivity/egd/exchange.py
--rw-rw-rw-   0        0        0     6513 2023-04-21 17:29:29.000000 kepconfig-1.2.0/kepconfig/connectivity/egd/name.py
--rw-rw-rw-   0        0        0     7170 2023-04-21 17:29:29.000000 kepconfig-1.2.0/kepconfig/connectivity/egd/range.py
--rw-rw-rw-   0        0        0    22720 2023-04-21 17:29:29.000000 kepconfig-1.2.0/kepconfig/connectivity/tag.py
-drwxrwxrwx   0        0        0        0 2023-04-21 18:38:16.990479 kepconfig-1.2.0/kepconfig/connectivity/udd/
--rw-rw-rw-   0        0        0      445 2023-03-31 19:14:13.000000 kepconfig-1.2.0/kepconfig/connectivity/udd/__init__.py
--rw-rw-rw-   0        0        0     5930 2023-04-21 17:29:29.000000 kepconfig-1.2.0/kepconfig/connectivity/udd/profile.py
-drwxrwxrwx   0        0        0        0 2023-04-21 18:38:17.007513 kepconfig-1.2.0/kepconfig/datalogger/
--rw-rw-rw-   0        0        0      491 2023-04-14 21:02:13.000000 kepconfig-1.2.0/kepconfig/datalogger/__init__.py
--rw-rw-rw-   0        0        0     7654 2023-04-21 17:29:29.000000 kepconfig-1.2.0/kepconfig/datalogger/log_group.py
--rw-rw-rw-   0        0        0     6280 2023-04-21 17:29:29.000000 kepconfig-1.2.0/kepconfig/datalogger/log_items.py
--rw-rw-rw-   0        0        0     4366 2023-04-20 20:53:12.000000 kepconfig-1.2.0/kepconfig/datalogger/mapping.py
--rw-rw-rw-   0        0        0     6528 2023-04-21 17:29:29.000000 kepconfig-1.2.0/kepconfig/datalogger/triggers.py
--rw-rw-rw-   0        0        0     2455 2023-04-04 12:54:50.000000 kepconfig-1.2.0/kepconfig/error.py
-drwxrwxrwx   0        0        0        0 2023-04-21 18:38:17.018510 kepconfig-1.2.0/kepconfig/iot_gateway/
--rw-rw-rw-   0        0        0      634 2023-03-31 19:17:31.000000 kepconfig-1.2.0/kepconfig/iot_gateway/__init__.py
--rw-rw-rw-   0        0        0     8713 2023-04-21 17:29:29.000000 kepconfig-1.2.0/kepconfig/iot_gateway/agent.py
--rw-rw-rw-   0        0        0     6854 2023-04-21 17:29:29.000000 kepconfig-1.2.0/kepconfig/iot_gateway/iot_items.py
--rw-rw-rw-   0        0        0     1893 2023-04-03 19:20:56.000000 kepconfig-1.2.0/kepconfig/structures.py
--rw-rw-rw-   0        0        0     1480 2023-04-04 12:27:33.000000 kepconfig-1.2.0/kepconfig/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 18:38:16.938805 kepconfig-1.2.0/kepconfig.egg-info/
--rw-rw-rw-   0        0        0     6530 2023-04-21 18:38:16.000000 kepconfig-1.2.0/kepconfig.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1041 2023-04-21 18:38:16.000000 kepconfig-1.2.0/kepconfig.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 18:38:16.000000 kepconfig-1.2.0/kepconfig.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-21 18:38:16.000000 kepconfig-1.2.0/kepconfig.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       91 2022-10-21 00:45:52.000000 kepconfig-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-21 18:38:17.025515 kepconfig-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     2417 2023-03-29 20:07:04.000000 kepconfig-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 20:00:58.282288 kepconfig-1.2.1/
+-rw-rw-rw-   0        0        0     1127 2021-03-15 20:50:21.000000 kepconfig-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     6655 2023-04-28 20:00:58.281288 kepconfig-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5749 2023-04-28 19:59:59.000000 kepconfig-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 20:00:58.225754 kepconfig-1.2.1/kepconfig/
+-rw-rw-rw-   0        0        0      913 2023-04-28 20:00:38.000000 kepconfig-1.2.1/kepconfig/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 20:00:58.242784 kepconfig-1.2.1/kepconfig/admin/
+-rw-rw-rw-   0        0        0      495 2023-03-31 19:09:46.000000 kepconfig-1.2.1/kepconfig/admin/__init__.py
+-rw-rw-rw-   0        0        0     6776 2023-04-21 17:03:24.000000 kepconfig-1.2.1/kepconfig/admin/lls.py
+-rw-rw-rw-   0        0        0     5375 2023-04-28 19:59:59.000000 kepconfig-1.2.1/kepconfig/admin/ua_server.py
+-rw-rw-rw-   0        0        0     6566 2023-04-28 19:59:59.000000 kepconfig-1.2.1/kepconfig/admin/user_groups.py
+-rw-rw-rw-   0        0        0     6198 2023-04-28 19:59:59.000000 kepconfig-1.2.1/kepconfig/admin/users.py
+-rw-rw-rw-   0        0        0    20744 2023-04-28 19:59:59.000000 kepconfig-1.2.1/kepconfig/connection.py
+drwxrwxrwx   0        0        0        0 2023-04-28 20:00:58.250775 kepconfig-1.2.1/kepconfig/connectivity/
+-rw-rw-rw-   0        0        0      759 2023-03-31 19:09:38.000000 kepconfig-1.2.1/kepconfig/connectivity/__init__.py
+-rw-rw-rw-   0        0        0     7887 2023-04-28 19:59:59.000000 kepconfig-1.2.1/kepconfig/connectivity/channel.py
+-rw-rw-rw-   0        0        0    11095 2023-04-28 19:59:59.000000 kepconfig-1.2.1/kepconfig/connectivity/device.py
+drwxrwxrwx   0        0        0        0 2023-04-28 20:00:58.259285 kepconfig-1.2.1/kepconfig/connectivity/egd/
+-rw-rw-rw-   0        0        0      517 2023-03-31 19:17:27.000000 kepconfig-1.2.1/kepconfig/connectivity/egd/__init__.py
+-rw-rw-rw-   0        0        0     8815 2023-04-28 19:59:59.000000 kepconfig-1.2.1/kepconfig/connectivity/egd/exchange.py
+-rw-rw-rw-   0        0        0     6556 2023-04-28 19:59:59.000000 kepconfig-1.2.1/kepconfig/connectivity/egd/name.py
+-rw-rw-rw-   0        0        0     7229 2023-04-28 19:59:59.000000 kepconfig-1.2.1/kepconfig/connectivity/egd/range.py
+-rw-rw-rw-   0        0        0    22692 2023-04-28 19:59:59.000000 kepconfig-1.2.1/kepconfig/connectivity/tag.py
+drwxrwxrwx   0        0        0        0 2023-04-28 20:00:58.263283 kepconfig-1.2.1/kepconfig/connectivity/udd/
+-rw-rw-rw-   0        0        0      445 2023-03-31 19:14:13.000000 kepconfig-1.2.1/kepconfig/connectivity/udd/__init__.py
+-rw-rw-rw-   0        0        0     5930 2023-04-21 17:29:29.000000 kepconfig-1.2.1/kepconfig/connectivity/udd/profile.py
+drwxrwxrwx   0        0        0        0 2023-04-28 20:00:58.273288 kepconfig-1.2.1/kepconfig/datalogger/
+-rw-rw-rw-   0        0        0      491 2023-04-14 21:02:13.000000 kepconfig-1.2.1/kepconfig/datalogger/__init__.py
+-rw-rw-rw-   0        0        0     7712 2023-04-28 19:59:59.000000 kepconfig-1.2.1/kepconfig/datalogger/log_group.py
+-rw-rw-rw-   0        0        0     6338 2023-04-28 19:59:59.000000 kepconfig-1.2.1/kepconfig/datalogger/log_items.py
+-rw-rw-rw-   0        0        0     4424 2023-04-28 19:59:59.000000 kepconfig-1.2.1/kepconfig/datalogger/mapping.py
+-rw-rw-rw-   0        0        0     6586 2023-04-28 19:59:59.000000 kepconfig-1.2.1/kepconfig/datalogger/triggers.py
+-rw-rw-rw-   0        0        0     2455 2023-04-04 12:54:50.000000 kepconfig-1.2.1/kepconfig/error.py
+drwxrwxrwx   0        0        0        0 2023-04-28 20:00:58.279289 kepconfig-1.2.1/kepconfig/iot_gateway/
+-rw-rw-rw-   0        0        0      634 2023-03-31 19:17:31.000000 kepconfig-1.2.1/kepconfig/iot_gateway/__init__.py
+-rw-rw-rw-   0        0        0     8773 2023-04-28 19:59:59.000000 kepconfig-1.2.1/kepconfig/iot_gateway/agent.py
+-rw-rw-rw-   0        0        0     6913 2023-04-28 19:59:59.000000 kepconfig-1.2.1/kepconfig/iot_gateway/iot_items.py
+-rw-rw-rw-   0        0        0     1893 2023-04-03 19:20:56.000000 kepconfig-1.2.1/kepconfig/structures.py
+-rw-rw-rw-   0        0        0     1992 2023-04-28 19:59:59.000000 kepconfig-1.2.1/kepconfig/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 20:00:58.232753 kepconfig-1.2.1/kepconfig.egg-info/
+-rw-rw-rw-   0        0        0     6655 2023-04-28 20:00:58.000000 kepconfig-1.2.1/kepconfig.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1041 2023-04-28 20:00:58.000000 kepconfig-1.2.1/kepconfig.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 20:00:58.000000 kepconfig-1.2.1/kepconfig.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-28 20:00:58.000000 kepconfig-1.2.1/kepconfig.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       91 2022-10-21 00:45:52.000000 kepconfig-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-28 20:00:58.282288 kepconfig-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     2417 2023-03-29 20:07:04.000000 kepconfig-1.2.1/setup.py
```

### Comparing `kepconfig-1.2.0/LICENSE` & `kepconfig-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kepconfig-1.2.0/PKG-INFO` & `kepconfig-1.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kepconfig
-Version: 1.2.0
+Version: 1.2.1
 Summary: SDK package for Kepware Configuration API
 Home-page: https://github.com/PTCInc/Kepware-ConfigAPI-SDK-Python
 Author: PTC Inc
 License: MIT License
 Keywords: Kepware,OPC,Configuration,Thingworx
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -23,14 +23,16 @@
 
 # Kepware Configuration API SDK for Python
 
 [![Released Version](https://img.shields.io/pypi/v/kepconfig)](https://pypi.org/project/kepconfig) [![Supported Versions](https://img.shields.io/pypi/pyversions/kepconfig)](https://pypi.org/project/kepconfig) ![PyPI - Downloads](https://img.shields.io/pypi/dm/kepconfig) ![PyPI - License](https://img.shields.io/pypi/l/kepconfig)
 
 This is a package to help create Python applications to conduct operations with the Kepware Configuration API. This package is designed to work with all versions of Kepware that support the Configuration API including Thingworx Kepware Server (TKS), Thingworx Kepware Edge (TKE) and KEPServerEX (KEP).
 
+**API reference documentation is available on [Github Pages](https://ptcinc.github.io/Kepware-ConfigAPI-SDK-Python)**
+
 ## Prerequisites
 
 Package supported and tested on Python 3.9 or later. Older versions support earlier Python 3 environments but have less functionality. All HTTP communication is handled by the [urllib](https://docs.python.org/3/library/urllib.html#module-urllib) Python standard library.
 
 ## Features
 
 - Supports both HTTP and HTTPS connections with certificate validation options
@@ -94,15 +96,15 @@
 ## Key Concepts
 
 NOTE: Detailed examples can also be found in the [examples](./examples/) folder.
 
 ### Create server connection
 
 ```python
-import kepconfig.connection
+from kepconfig import connection
 
 server = connection.server(host = '127.0.0.1', port = 57412, user = 'Administrator', pw = '')
 
 # For HTTPS connections:
 server = connection.server(host = '127.0.0.1', port = 57512, user = 'Administrator', pw = '', https=True)
 
 ```
@@ -140,15 +142,15 @@
     },
     {
             "common.ALLTYPES_NAME": "Temp2",
             "servermain.TAG_ADDRESS": "R1"
     }
 ]
 tag_path = '{}.{}.{}'.format(ch_name, dev_name, tag_group_path)
-result = tag.add_tag(server, tag_path, tag_info))
+result = tag.add_tag(server, tag_path, tag_info)
 
 ```
 
 ## Need More Information
 
 **Visit:**
```

### Comparing `kepconfig-1.2.0/README.md` & `kepconfig-1.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Kepware Configuration API SDK for Python
 
 [![Released Version](https://img.shields.io/pypi/v/kepconfig)](https://pypi.org/project/kepconfig) [![Supported Versions](https://img.shields.io/pypi/pyversions/kepconfig)](https://pypi.org/project/kepconfig) ![PyPI - Downloads](https://img.shields.io/pypi/dm/kepconfig) ![PyPI - License](https://img.shields.io/pypi/l/kepconfig)
 
 This is a package to help create Python applications to conduct operations with the Kepware Configuration API. This package is designed to work with all versions of Kepware that support the Configuration API including Thingworx Kepware Server (TKS), Thingworx Kepware Edge (TKE) and KEPServerEX (KEP).
 
+**API reference documentation is available on [Github Pages](https://ptcinc.github.io/Kepware-ConfigAPI-SDK-Python)**
+
 ## Prerequisites
 
 Package supported and tested on Python 3.9 or later. Older versions support earlier Python 3 environments but have less functionality. All HTTP communication is handled by the [urllib](https://docs.python.org/3/library/urllib.html#module-urllib) Python standard library.
 
 ## Features
 
 - Supports both HTTP and HTTPS connections with certificate validation options
@@ -71,15 +73,15 @@
 ## Key Concepts
 
 NOTE: Detailed examples can also be found in the [examples](./examples/) folder.
 
 ### Create server connection
 
 ```python
-import kepconfig.connection
+from kepconfig import connection
 
 server = connection.server(host = '127.0.0.1', port = 57412, user = 'Administrator', pw = '')
 
 # For HTTPS connections:
 server = connection.server(host = '127.0.0.1', port = 57512, user = 'Administrator', pw = '', https=True)
 
 ```
@@ -117,15 +119,15 @@
     },
     {
             "common.ALLTYPES_NAME": "Temp2",
             "servermain.TAG_ADDRESS": "R1"
     }
 ]
 tag_path = '{}.{}.{}'.format(ch_name, dev_name, tag_group_path)
-result = tag.add_tag(server, tag_path, tag_info))
+result = tag.add_tag(server, tag_path, tag_info)
 
 ```
 
 ## Need More Information
 
 **Visit:**
```

### Comparing `kepconfig-1.2.0/kepconfig/__init__.py` & `kepconfig-1.2.1/kepconfig/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # -------------------------------------------------------------------------
 # Copyright (c) PTC Inc. and/or all its affiliates. All rights reserved.
 # See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
-r"""
+# **Kepware Configuration (kepconfig) API Library**
+# --
 
-**Kepware Configuration (kepconfig) API Library**
---
+# This is a package to help create Python applications to conduct operations with the Kepware Configuration API. 
+# This package is designed to work with all versions of Kepware that support the Configuration API including 
+# Thingworx Kepware Server (TKS), Thingworx Kepware Edge (TKE) and KEPServerEX (KEP).
 
-This is a package to help create Python applications to conduct operations with the Kepware Configuration API. 
-This package is designed to work with all versions of Kepware that support the Configuration API including 
-Thingworx Kepware Server (TKS), Thingworx Kepware Edge (TKE) and KEPServerEX (KEP).
+# Copyright (c) PTC Inc. and/or all its affiliates. All rights reserved.
+# See License.txt in the project root for
+# license information.
 
-Copyright (c) PTC Inc. and/or all its affiliates. All rights reserved.
-See License.txt in the project root for
-license information.
+r"""
+.. include:: ../README.md
 
 """
-__version__ = "1.2.0"
+__version__ = "1.2.1"
 from . import connection, error
-from .utils import path_split
```

### Comparing `kepconfig-1.2.0/kepconfig/admin/lls.py` & `kepconfig-1.2.1/kepconfig/admin/lls.py`

 * *Files identical despite different names*

### Comparing `kepconfig-1.2.0/kepconfig/admin/ua_server.py` & `kepconfig-1.2.1/kepconfig/admin/ua_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,30 @@
 
 r"""`ua_server` exposes an API to allow modifications (add, delete, modify) to 
 OPC UA Server endpoints within the Kepware Administration through the Kepware Configuration API
 """
 from typing import Union
 from ..error import KepHTTPError, KepError
 from ..connection import server
+from ..utils import _url_parse_object
 
 
 UA_ROOT = '/admin/ua_endpoints'
 
 def _create_url(endpoint = None):
     '''Creates url object for the "server_users" branch of Kepware's project tree. Used 
     to build a part of Kepware Configuration API URL structure
 
     Returns the user specific url when a value is passed as the user name.
     '''
     
     if endpoint == None:
         return UA_ROOT
     else:
-        return '{}/{}'.format(UA_ROOT,endpoint)
+        return '{}/{}'.format(UA_ROOT, _url_parse_object(endpoint))
 
 def add_endpoint(server: server, DATA: Union[dict, list]) -> Union[bool, list]:
     '''Add an `"endpoint"` or multiple `"endpoint"` objects to Kepware UA Server by passing a 
     list of endpoints to be added all at once.
 
     :param server: instance of the `server` class
     :param DATA: Dict or List of Dicts of the UA Endpoints to add
```

### Comparing `kepconfig-1.2.0/kepconfig/admin/user_groups.py` & `kepconfig-1.2.1/kepconfig/admin/user_groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 r"""`user_groups` exposes an API to allow modifications (add, delete, modify) to 
 user groups within the Kepware Administration User Manager through the Kepware Configuration API
 """
 from typing import Union
 from ..error import KepHTTPError, KepError
 from ..connection import server
+from ..utils import _url_parse_object
 
 
 USERGROUPS_ROOT = '/admin/server_usergroups'
 ENABLE_PROPERTY = 'libadminsettings.USERMANAGER_GROUP_ENABLED'
 
 def _create_url(user_group = None):
     '''Creates url object for the "server_usergroups" branch of Kepware's project tree. Used 
@@ -21,15 +22,15 @@
 
     Returns the user group specific url when a value is passed as the user_group name.
     '''
     
     if user_group == None:
         return USERGROUPS_ROOT
     else:
-        return '{}/{}'.format(USERGROUPS_ROOT,user_group)
+        return '{}/{}'.format(USERGROUPS_ROOT, _url_parse_object(user_group))
 
 def add_user_group(server: server, DATA: Union[dict, list]) -> Union[bool, list]:
     '''Add a `"user group"` or multiple `"user group"` objects to Kepware User Manager by passing a 
     list of user groups to be added all at once.
 
     :param server: instance of the `server` class
     :param DATA: Dict or List of Dicts of the user groups to add
```

### Comparing `kepconfig-1.2.0/kepconfig/admin/users.py` & `kepconfig-1.2.1/kepconfig/admin/users.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 r"""`users` exposes an API to allow modifications (add, delete, modify) to 
 users within the Kepware Administration User Management through the Kepware Configuration API
 """
 from typing import Union
 from ..error import KepError, KepHTTPError
 from ..connection import server
+from ..utils import _url_parse_object
 
 
 USERS_ROOT = '/admin/server_users'
 ENABLE_PROPERTY = 'libadminsettings.USERMANAGER_USER_ENABLED'
 
 def _create_url(user = None):
     '''Creates url object for the "server_users" branch of Kepware's project tree. Used 
@@ -21,15 +22,15 @@
 
     Returns the user specific url when a value is passed as the user name.
     '''
     
     if user == None:
         return USERS_ROOT
     else:
-        return '{}/{}'.format(USERS_ROOT,user)
+        return '{}/{}'.format(USERS_ROOT, _url_parse_object(user))
 
 def add_user(server: server, DATA: Union[dict, list]) -> Union[bool, list]:
     '''Add a `"user"` or multiple `"user"` objects to Kepware User Manager by passing a 
     list of users to be added all at once.
 
     :param server: instance of the `server` class
     :param DATA: Dict or List of Dicts of the users to add
```

### Comparing `kepconfig-1.2.0/kepconfig/connection.py` & `kepconfig-1.2.1/kepconfig/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -427,15 +427,17 @@
         except error.URLError as err:
             # print('URLError: {} URL: {}'.format(err.reason, request_obj.get_full_url()), file=sys.stderr)
             raise KepURLError(msg=err.reason, url=request_obj.get_full_url())
 
     # Fucntion used to ensure special characters are handled in the URL
     # Ex: Space will be turned to %20
     def __url_validate(self, url):
-        parsed_url = parse.urlparse(url)
+        # Configuration API does not use fragments in URL so ignore to allow # as a character
+        # Objects in Kepware can include # as part of the object names
+        parsed_url = parse.urlparse(url, allow_fragments= False)
         # Added % for scenarios where special characters have already been escaped with %
         updated_path = parse.quote(parsed_url.path, safe = '/%')
 
         # If host is "localhost", force using the IPv4 loopback adapter IP address in all calls
         # This is done to remove retries that will happen when the host resolution uses IPv6 intially
         # Kepware currently doesn't support IPv6 and is not listening on this interface
         if parsed_url.hostname.lower() == 'localhost':
```

### Comparing `kepconfig-1.2.0/kepconfig/connectivity/__init__.py` & `kepconfig-1.2.1/kepconfig/connectivity/__init__.py`

 * *Files identical despite different names*

### Comparing `kepconfig-1.2.0/kepconfig/connectivity/channel.py` & `kepconfig-1.2.1/kepconfig/connectivity/channel.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 channel objects within the Kepware Configuration API
 """
 
  
 import inspect
 from ..connection import server
 from ..error import KepHTTPError, KepError
+from ..utils import _url_parse_object
 from typing import Union
 from . import device
 
 CHANNEL_ROOT = '/project/channels'
 
 def _create_url(channel = None):
     '''Creates url object for the "channel" branch of Kepware's project tree. Used 
@@ -24,15 +25,15 @@
 
     Returns the channel specific url when a value is passed as the channel name.
     '''
     
     if channel == None:
         return CHANNEL_ROOT
     else:
-        return '{}/{}'.format(CHANNEL_ROOT,channel)
+        return '{}/{}'.format(CHANNEL_ROOT,_url_parse_object(channel))
 
 def add_channel(server: server, DATA: Union[dict, list]) -> Union[bool, list]:
     '''Add a `"channel"` or multiple `"channel"` objects to Kepware. Can be used to pass children of a channel object 
     such as devices and tags/tag groups. This allows you to create a channel, it's devices and tags 
     all in one function, if desired.
 
     Additionally it can be used to pass a list of channels and it's children to be added all at once.
@@ -80,15 +81,15 @@
 def modify_channel(server: server, DATA: dict, *, channel: str = None, force: bool = False) -> bool:
     '''Modify a channel object and it's properties in Kepware. If a `"channel"` is not provided as an input,
     you need to identify the channel in the *'common.ALLTYPES_NAME'* property field in `"DATA"`. It will 
     assume that is the channel that is to be modified.
 
     :param server: instance of the `server` class
     :param DATA: Dict of the `channel` properties to be modified
-    :param channel: *(optional)* - name of channel to modify. Only needed if not existing in `"DATA"`
+    :param channel: *(optional)* name of channel to modify. Only needed if not existing in `"DATA"`
     :param force: *(optional)* if True, will force the configuration update to the Kepware server
     
     :return: True - If a "HTTP 200 - OK" is received from Kepware server
 
     :raises KepHTTPError: If urllib provides an HTTPError
     :raises KepURLError: If urllib provides an URLError
     '''
```

### Comparing `kepconfig-1.2.0/kepconfig/connectivity/device.py` & `kepconfig-1.2.1/kepconfig/connectivity/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 r"""`device` exposes an API to allow modifications (add, delete, modify) to 
 device objects within the Kepware Configuration API
 """
 
 from ..connection import KepServiceResponse, server
 from ..error import KepHTTPError, KepError
+from ..utils import _url_parse_object, path_split
 from typing import Union
-import kepconfig
 from . import channel, tag
 import inspect
 
 DEVICE_ROOT = '/devices'
 ATG_URL = '/services/TagGeneration'
 
 def _create_url(device = None):
@@ -24,15 +24,15 @@
     to build a part of Kepware Configuration API URL structure
     
     Returns the device specific url when a value is passed as the device name.
     '''
     if device == None:
         return DEVICE_ROOT
     else:
-        return '{}/{}'.format(DEVICE_ROOT,device)
+        return '{}/{}'.format(DEVICE_ROOT,_url_parse_object(device))
 
 def add_device(server: server, channel_name: str, DATA: Union[dict, list]) -> Union[bool, list]:
     '''Add a `"device"` or multiple `"device"` objects to a channel in Kepware. Can be used to pass children of a device object 
     such as tags and tag groups. This allows you to create a device and tags 
     all in one function, if desired.
 
     Additionally it can be used to pass a list of devices and it's children to be added all at once.
@@ -70,15 +70,15 @@
 
     :return: True - If a "HTTP 200 - OK" is received from Kepware server
 
     :raises KepHTTPError: If urllib provides an HTTPError
     :raises KepURLError: If urllib provides an URLError
     '''
 
-    path_obj = kepconfig.path_split(device_path)
+    path_obj = path_split(device_path)
     try:
         r = server._config_del(server.url + channel._create_url(path_obj['channel']) + _create_url(path_obj['device']))
         if r.code == 200: return True 
         else: raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
     except KeyError as err:
         err_msg = 'Error: No {} identified in {} | Function: {}'.format(err,'device_path', inspect.currentframe().f_code.co_name)
         raise KepError(err_msg)
@@ -96,15 +96,15 @@
 
     :raises KepHTTPError: If urllib provides an HTTPError
     :raises KepURLError: If urllib provides an URLError
     '''
 
     device_data = server._force_update_check(force, DATA)
 
-    path_obj = kepconfig.path_split(device_path)
+    path_obj = path_split(device_path)
     try:
         r = server._config_update(server.url + channel._create_url(path_obj['channel']) + _create_url(path_obj['device']), device_data)
         if r.code == 200: return True 
         else: raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
     except KeyError as err:
             err_msg = 'Error: No {} identified in {} | Function: {}'.format(err,'device_path', inspect.currentframe().f_code.co_name)
             raise KepError(err_msg)
@@ -118,15 +118,15 @@
 
     :return: Dict of data for the device requested
 
     :raises KepHTTPError: If urllib provides an HTTPError
     :raises KepURLError: If urllib provides an URLError
     '''
 
-    path_obj = kepconfig.path_split(device_path)
+    path_obj = path_split(device_path)
     try:
         r = server._config_get(server.url + channel._create_url(path_obj['channel']) + _create_url(path_obj['device']))
         return r.payload
     except KeyError as err:
         err_msg = 'Error: No {} identified in {} | Function: {}'.format(err,'device_path', inspect.currentframe().f_code.co_name)
         raise KepError(err_msg)
     # except Exception as err:
@@ -160,15 +160,15 @@
 
     :return: `KepServiceResponse` instance with job information
     
     :raises KepHTTPError: If urllib provides an HTTPError (If not HTTP code 202 [Accepted] or 429 [Too Busy] returned)
     :raises KepURLError: If urllib provides an URLError
     '''
     
-    path_obj = kepconfig.path_split(device_path)
+    path_obj = path_split(device_path)
     try:
         url = server.url +channel._create_url(path_obj['channel']) + _create_url(path_obj['device']) + ATG_URL
         job = server._kep_service_execute(url, None, job_ttl)
         return job
     except KeyError as err:
         err_msg = 'Error: No {} identified in {} | Function: {}'.format(err,'device_path', inspect.currentframe().f_code.co_name)
         raise KepError(err_msg)
```

### Comparing `kepconfig-1.2.0/kepconfig/connectivity/egd/__init__.py` & `kepconfig-1.2.1/kepconfig/connectivity/egd/__init__.py`

 * *Files identical despite different names*

### Comparing `kepconfig-1.2.0/kepconfig/connectivity/egd/exchange.py` & `kepconfig-1.2.1/kepconfig/connectivity/egd/exchange.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 # --------------------------------------------------------------------------
 
 
 r"""`exchange` exposes an API to allow modifications (add, delete, modify) to 
 exchange objects for EGD devices within the Kepware Configuration API
 """
 
-from ... import path_split
 from ...connection import server
 from ...error import KepHTTPError, KepError
+from ...utils import _url_parse_object, path_split
 from typing import Union
 from .. import egd as EGD, channel, device
 
 CONSUMER_ROOT = '/consumer_exchange_groups/consumer exchanges/consumer_exchanges'
 PRODUCER_ROOT = '/producer_exchange_groups/producer exchanges/producer_exchanges'
 
 def _create_url(device_path, ex_type, exchange_name = None):
@@ -30,17 +30,17 @@
     if exchange_name == None:
         if ex_type.upper() == EGD.CONSUMER_EXCHANGE:
             return device_root + CONSUMER_ROOT
         else:
             return device_root + PRODUCER_ROOT
     else:
         if ex_type.upper() == EGD.CONSUMER_EXCHANGE:
-            return '{}{}/{}'.format(device_root,CONSUMER_ROOT,exchange_name)
+            return '{}{}/{}'.format(device_root,CONSUMER_ROOT,_url_parse_object(exchange_name))
         else:
-            return '{}{}/{}'.format(device_root,PRODUCER_ROOT,exchange_name)
+            return '{}{}/{}'.format(device_root,PRODUCER_ROOT,_url_parse_object(exchange_name))
 
 def add_exchange(server: server, device_path: str, ex_type: str, DATA: Union[dict, list]) -> Union[bool, list]:
     '''Add a `"exchange"` or multiple `"exchange"` objects to Kepware. Can be used to pass children of a exchange object 
     such as ranges. This allows you to create a exchange and ranges for the exchange all in one function, if desired.
 
     Additionally it can be used to pass a list of exchanges and it's children to be added all at once.
```

### Comparing `kepconfig-1.2.0/kepconfig/connectivity/egd/name.py` & `kepconfig-1.2.1/kepconfig/connectivity/egd/name.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # --------------------------------------------------------------------------
 
 
 r"""`names` exposes an API to allow modifications (add, delete, modify) to 
 name resolution objects for EGD devices within the Kepware Configuration API
 """
 
-from ... import path_split
+from ...utils import _url_parse_object, path_split
 from ...connection import server
 from ...error import KepHTTPError, KepError
 from typing import Union
 from .. import channel, device
 
 NAMES_ROOT = '/name_resolution_groups/Name Resolutions/name_resolutions'
 
@@ -25,15 +25,15 @@
     '''
     path_obj = path_split(device_path)
     device_root = channel._create_url(path_obj['channel']) + device._create_url(path_obj['device'])
 
     if name == None:
         return '{}/{}'.format(device_root, NAMES_ROOT)
     else:
-        return '{}/{}/{}'.format(device_root, NAMES_ROOT, name)
+        return '{}/{}/{}'.format(device_root, NAMES_ROOT, _url_parse_object(name))
 
 def add_name_resolution(server: server, device_path: str, DATA: Union[dict, list]) -> Union[bool, list]:
     '''Add a `"name resolution"` or multiple `"name resolution"` objects to Kepware. This allows you to 
     create a name resolution or multiple name resolutions all in one function, if desired.
 
     :param server: instance of the `server` class
     :param device_path: path to EGD device. Standard Kepware address decimal
```

### Comparing `kepconfig-1.2.0/kepconfig/connectivity/egd/range.py` & `kepconfig-1.2.1/kepconfig/connectivity/egd/range.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,29 +9,30 @@
 range objects in exchanges for EGD devices within the Kepware Configuration API
 """
 
 from typing import Union
 from .. import egd as EGD
 from ...connection import server
 from ...error import KepError, KepHTTPError
+from ...utils import _url_parse_object
 
 RANGES_ROOT = '/ranges'
 
 def _create_url(device_path, ex_type, exchange_name, range = None):
     '''Creates url object for the "range" branch of Kepware's project tree. Used 
     to build a part of Kepware Configuration API URL structure
 
     Returns the range specific url when a value is passed as the range name.
     '''
     exchange_root = EGD.exchange._create_url(device_path, ex_type, exchange_name)
 
     if range == None:
         return '{}{}'.format(exchange_root, RANGES_ROOT)
     else:
-        return '{}{}/{}'.format(exchange_root, RANGES_ROOT, range)
+        return '{}{}/{}'.format(exchange_root, RANGES_ROOT, _url_parse_object(range))
 
 def add_range(server: server, device_path: str, ex_type: str, exchange_name: str, DATA: Union[dict, list]) -> Union[bool, list]:
     '''Add a `"range"` or multiple `"range"` objects to Kepware. This allows you to 
     create a range or multiple ranges all in one function, if desired.
 
     When passing multiple ranges, they will be populated in the same order
     in the list sent. Ensure you provide the list in the order desired.
```

### Comparing `kepconfig-1.2.0/kepconfig/connectivity/tag.py` & `kepconfig-1.2.1/kepconfig/connectivity/tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 r"""`tag` exposes an API to allow modifications (add, delete, modify) to 
 tag and tag group objects within the Kepware Configuration API
 """
 
 from ..connection import server
 from ..error import KepError, KepHTTPError
+from ..utils import _url_parse_object, path_split
 from typing import Union
-import kepconfig
 from . import channel, device
 import inspect
 
 TAGS_ROOT = '/tags'
 TAG_GRP_ROOT = '/tag_groups'
 
 def _create_tags_url(tag = None):
@@ -24,26 +24,26 @@
     to build a part of Kepware Configuration API URL structure
     
     Returns the tag specific url when a value is passed as the tag name.
     '''
     if tag == None:
         return TAGS_ROOT
     else: 
-        return '{}/{}'.format(TAGS_ROOT,tag)
+        return '{}/{}'.format(TAGS_ROOT, _url_parse_object(tag))
 
 def _create_tag_groups_url(tag_group = None):
     '''Creates url object for the "tag_group" branch of Kepware's project tree. Used 
     to build a part of Kepware Configuration API URL structure
     
     Returns the tag group specific url when a value is passed as the tag group name.
     '''
     if tag_group == None:
         return TAG_GRP_ROOT
     else: 
-        return '{}/{}'.format(TAG_GRP_ROOT,tag_group)
+        return '{}/{}'.format(TAG_GRP_ROOT,_url_parse_object(tag_group))
 
 def add_tag(server: server, tag_path: str, DATA: Union[dict, list]) -> Union[bool, list]:
     '''Add `"tag"` or multiple `"tag"` objects to a specific path in Kepware. 
     Can be used to pass a list of tags to be added at one path location.
 
     :param server: instance of the `server` class
     :param device_path: path identifying where to add tag(s). Standard Kepware address decimal 
@@ -54,15 +54,15 @@
     :return: If a "HTTP 207 - Multi-Status" is received from Kepware with a list of dict error responses for all 
     tags added that failed.
 
     :raises KepHTTPError: If urllib provides an HTTPError
     :raises KepURLError: If urllib provides an URLError
     '''
 
-    path_obj = kepconfig.path_split(tag_path)
+    path_obj = path_split(tag_path)
     try:
         url = server.url+channel._create_url(path_obj['channel'])+device._create_url(path_obj['device'])
         if 'tag_path' in path_obj:
             for tg in path_obj['tag_path']:
                 url += _create_tag_groups_url(tag_group=tg)
         url += _create_tags_url()
     except KeyError as err:
@@ -95,15 +95,15 @@
     :return: If a "HTTP 207 - Multi-Status" is received from Kepware with a list of dict error responses for all 
     tag groups added that failed.
 
     :raises KepHTTPError: If urllib provides an HTTPError
     :raises KepURLError: If urllib provides an URLError
     '''
 
-    path_obj = kepconfig.path_split(tag_group_path)
+    path_obj = path_split(tag_group_path)
     try:
         url = server.url+channel._create_url(path_obj['channel'])+device._create_url(path_obj['device'])
         if 'tag_path' in path_obj:
             for tg in path_obj['tag_path']:
                 url += _create_tag_groups_url(tag_group=tg)
         url += _create_tag_groups_url()
     except KeyError as err:
@@ -197,15 +197,15 @@
 
     :raises KepHTTPError: If urllib provides an HTTPError
     :raises KepURLError: If urllib provides an URLError
     '''
 
     tag_data = server._force_update_check(force, DATA)
 
-    path_obj = kepconfig.path_split(full_tag_path)
+    path_obj = path_split(full_tag_path)
     try:
         url = server.url+channel._create_url(path_obj['channel'])+device._create_url(path_obj['device'])
         for x in range(0, len(path_obj['tag_path'])-1):
             url += _create_tag_groups_url(tag_group=path_obj['tag_path'][x])
         url += _create_tags_url(tag=path_obj['tag_path'][len(path_obj['tag_path'])-1])
     except KeyError as err:
         err_msg = 'Error: No key {} identified | Function: {}'.format(err, inspect.currentframe().f_code.co_name)
@@ -230,15 +230,15 @@
 
     :raises KepHTTPError: If urllib provides an HTTPError
     :raises KepURLError: If urllib provides an URLError
     '''
 
     tag_group_data = server._force_update_check(force, DATA)
 
-    path_obj = kepconfig.path_split(tag_group_path)
+    path_obj = path_split(tag_group_path)
     try:
         url = server.url+channel._create_url(path_obj['channel'])+device._create_url(path_obj['device'])
         for tg in path_obj['tag_path']:
             url += _create_tag_groups_url(tag_group=tg)
     except KeyError as err:
         err_msg = 'Error: No key {} identified | Function: {}'.format(err, inspect.currentframe().f_code.co_name)
         raise KepError(err_msg)
@@ -258,15 +258,15 @@
 
     :return: True - If a "HTTP 200 - OK" is received from Kepware server
 
     :raises KepHTTPError: If urllib provides an HTTPError
     :raises KepURLError: If urllib provides an URLError
     '''
 
-    path_obj = kepconfig.path_split(full_tag_path)
+    path_obj = path_split(full_tag_path)
     try:
         url = server.url+channel._create_url(path_obj['channel'])+device._create_url(path_obj['device'])
         for x in range(0, len(path_obj['tag_path'])-1):
             url += _create_tag_groups_url(tag_group=path_obj['tag_path'][x])
         url += _create_tags_url(tag=path_obj['tag_path'][len(path_obj['tag_path'])-1])
     except KeyError as err:
         err_msg = 'Error: No key {} identified | Function: {}'.format(err, inspect.currentframe().f_code.co_name)
@@ -287,15 +287,15 @@
 
     :return: True - If a "HTTP 200 - OK" is received from Kepware server
 
     :raises KepHTTPError: If urllib provides an HTTPError
     :raises KepURLError: If urllib provides an URLError
     '''
 
-    path_obj = kepconfig.path_split(tag_group_path)
+    path_obj = path_split(tag_group_path)
     try:
         url = server.url+channel._create_url(path_obj['channel'])+device._create_url(path_obj['device'])
         for tg in path_obj['tag_path']:
             url += _create_tag_groups_url(tag_group=tg)
     except KeyError as err:
         err_msg = 'Error: No key {} identified | Function: {}'.format(err, inspect.currentframe().f_code.co_name)
         raise KepError(err_msg)
@@ -315,15 +315,15 @@
 
     :return: Dict of data for the tag requested
 
     :raises KepHTTPError: If urllib provides an HTTPError
     :raises KepURLError: If urllib provides an URLError
     '''
 
-    path_obj = kepconfig.path_split(full_tag_path)
+    path_obj = path_split(full_tag_path)
     try:
         url = server.url+channel._create_url(path_obj['channel'])+device._create_url(path_obj['device'])
         for x in range(0, len(path_obj['tag_path'])-1):
             url += _create_tag_groups_url(tag_group=path_obj['tag_path'][x])
         url += _create_tags_url(tag=path_obj['tag_path'][len(path_obj['tag_path'])-1])
     except KeyError as err:
         err_msg = 'Error: No key {} identified | Function: {}'.format(err, inspect.currentframe().f_code.co_name)
@@ -345,15 +345,15 @@
     
     :return: List of data for all tags
 
     :raises KepHTTPError: If urllib provides an HTTPError
     :raises KepURLError: If urllib provides an URLError
     '''
 
-    path_obj = kepconfig.path_split(full_tag_path)
+    path_obj = path_split(full_tag_path)
     try:
         url = f"{server.url}{channel._create_url(path_obj['channel'])}{device._create_url(path_obj['device'])}"
         if 'tag_path' in path_obj:
             for tg in path_obj['tag_path']:
                 url += _create_tag_groups_url(tag_group=tg)
         url += _create_tags_url()
     except KeyError as err:
@@ -374,15 +374,15 @@
     notation string that tag groups exists such as "channel1.device1.tag_group1"
 
     :return: Dict of data for the tag group requested
 
     :raises KepHTTPError: If urllib provides an HTTPError
     :raises KepURLError: If urllib provides an URLError
     '''
-    path_obj = kepconfig.path_split(tag_group_path)
+    path_obj = path_split(tag_group_path)
     try:
         url = server.url+channel._create_url(path_obj['channel'])+device._create_url(path_obj['device'])
         for tg in path_obj['tag_path']:
             url += _create_tag_groups_url(tag_group=tg)
     except KeyError as err:
         err_msg = 'Error: No key {} identified | Function: {}'.format(err, inspect.currentframe().f_code.co_name)
         raise KepError(err_msg)
@@ -403,15 +403,15 @@
         `sortOrder`, `sortProperty`, `pageNumber`, and `pageSize`
 
     :return: List of data for all tag groups
 
     :raises KepHTTPError: If urllib provides an HTTPError
     :raises KepURLError: If urllib provides an URLError
     '''
-    path_obj = kepconfig.path_split(tag_group_path)
+    path_obj = path_split(tag_group_path)
     try:
         url = f"{server.url}{channel._create_url(path_obj['channel'])}{device._create_url(path_obj['device'])}"
         if 'tag_path' in path_obj:
             for tg in path_obj['tag_path']:
                 url += _create_tag_groups_url(tag_group=tg)
         url += _create_tag_groups_url()
     except KeyError as err:
```

### Comparing `kepconfig-1.2.0/kepconfig/connectivity/udd/profile.py` & `kepconfig-1.2.1/kepconfig/connectivity/udd/profile.py`

 * *Files identical despite different names*

### Comparing `kepconfig-1.2.0/kepconfig/datalogger/log_group.py` & `kepconfig-1.2.1/kepconfig/datalogger/log_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,30 @@
 
 r"""`log_group` exposes an API to allow modifications (add, delete, modify) to 
 log group objects in DataLogger within the Kepware Configuration API
 """
 from typing import Union
 from ..connection import KepServiceResponse, server
 from ..error import KepError, KepHTTPError
+from ..utils import _url_parse_object
 
 ENABLE_PROPERTY = 'datalogger.LOG_GROUP_ENABLED'
 LOG_GROUP_ROOT = '/project/_datalogger/log_groups'
 SERVICES_ROOT = '/services'
 def _create_url(log_group = None):
     '''Creates url object for the "log_group" branch of Kepware's project tree. Used 
     to build a part of Kepware Configuration API URL structure
 
     Returns the agent specific url when a value is passed as the agent name.
     '''
 
     if log_group == None:
         return '{}'.format(LOG_GROUP_ROOT)
     else:
-        return '{}/{}'.format(LOG_GROUP_ROOT, log_group)
+        return '{}/{}'.format(LOG_GROUP_ROOT, _url_parse_object(log_group))
 
 
 def add_log_group(server: server, DATA: Union[dict, list]) -> Union[bool, list]:
     '''Add a `"log group"` or multiple `"log groups"` objects to Kepware's DataLogger. It can be used 
     to pass a list of log groups to be added all at once.
 
     :param server: instance of the `server` class
```

### Comparing `kepconfig-1.2.0/kepconfig/datalogger/log_items.py` & `kepconfig-1.2.1/kepconfig/datalogger/log_items.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,28 +7,29 @@
 r"""`log_items` exposes an API to allow modifications (add, delete, modify) to 
 log item (tag) objects in a Datalogger log group within the Kepware Configuration API
 """
 from typing import Union
 from . import log_group as Log_Group
 from ..error import KepError, KepHTTPError
 from ..connection import server
+from ..utils import _url_parse_object
 
 LOG_ITEMS_ROOT = '/log_items'
 
 def _create_url(log_item = None):
     '''Creates url object for the "log_item" branch of Kepware's project tree. Used 
     to build a part of Kepware Configuration API URL structure
 
     Returns the log_item specific url when a value is passed as the log_item name.
     '''
 
     if log_item == None:
         return '{}'.format(LOG_ITEMS_ROOT)
     else:
-        return '{}/{}'.format(LOG_ITEMS_ROOT, log_item)
+        return '{}/{}'.format(LOG_ITEMS_ROOT, _url_parse_object(log_item))
 
 
 def add_log_item(server: server, log_group: str, DATA: Union[dict, list]) -> Union[bool, list]:
     '''Add a `"log item"` or multiple `"log item"` objects to a log group in Kepware's Datalogger. It can 
     be used to pass a list of log items to be added all at once.
 
     :param server: instance of the `server` class
```

### Comparing `kepconfig-1.2.0/kepconfig/datalogger/mapping.py` & `kepconfig-1.2.1/kepconfig/datalogger/mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,28 +7,29 @@
 r"""`mapping` exposes an API to allow modifications (add, delete, modify) to 
 column mapping objects in a Datalogger log group within the Kepware Configuration API
 """
 
 from . import log_group as Log_Group
 from ..error import KepError, KepHTTPError
 from ..connection import server
+from ..utils import _url_parse_object
 
 MAPPING_ROOT = '/column_mappings'
 
 def _create_url(mapping = None):
     '''Creates url object for the "column_mappings" branch of Kepware's project tree. Used 
     to build a part of Kepware Configuration API URL structure
 
     Returns the mapping specific url when a value is passed as the column_mapping name.
     '''
 
     if mapping == None:
         return '{}'.format(MAPPING_ROOT)
     else:
-        return '{}/{}'.format(MAPPING_ROOT, mapping)
+        return '{}/{}'.format(MAPPING_ROOT, _url_parse_object(mapping))
 
 def modify_mapping(server: server, log_group: str, DATA: dict, *, mapping: str = None, force: bool = False) -> bool:
     '''Modify a column `"mapping"` object and it's properties in Kepware. If a `"mapping"` is not provided as an input,
     you need to identify the column mapping in the *'common.ALLTYPES_NAME'* property field in the `"DATA"`. It will 
     assume that is the column mapping that is to be modified.
 
     :param server: instance of the `server` class
```

### Comparing `kepconfig-1.2.0/kepconfig/datalogger/triggers.py` & `kepconfig-1.2.1/kepconfig/datalogger/triggers.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,28 +8,29 @@
 trigger objects in a Datalogger log group within the Kepware Configuration API
 """
 
 from typing import Union
 from . import log_group as Log_Group
 from ..error import KepError, KepHTTPError
 from ..connection import server
+from ..utils import _url_parse_object
 
 TRIGGERS_ROOT = '/triggers'
 
 def _create_url(trigger = None):
     '''Creates url object for the "trigger" branch of Kepware's project tree. Used 
     to build a part of Kepware Configuration API URL structure
 
     Returns the trigger specific url when a value is passed as the trigger name.
     '''
 
     if trigger == None:
         return '{}'.format(TRIGGERS_ROOT)
     else:
-        return '{}/{}'.format(TRIGGERS_ROOT, trigger)
+        return '{}/{}'.format(TRIGGERS_ROOT, _url_parse_object(trigger))
 
 
 def add_trigger(server: server, log_group: str, DATA: Union[dict, list]) -> Union[bool, list]:
     '''Add a `"trigger"` or multiple `"trigger"` objects to a log group in Kepware's Datalogger. It can 
     be used to pass a list of triggers to be added all at once.
 
     :param server: instance of the `server` class
```

### Comparing `kepconfig-1.2.0/kepconfig/error.py` & `kepconfig-1.2.1/kepconfig/error.py`

 * *Files identical despite different names*

### Comparing `kepconfig-1.2.0/kepconfig/iot_gateway/__init__.py` & `kepconfig-1.2.1/kepconfig/iot_gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `kepconfig-1.2.0/kepconfig/iot_gateway/agent.py` & `kepconfig-1.2.1/kepconfig/iot_gateway/agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 # from .. import connection 
 from typing import Union
 from ..connection import server
 from .. import iot_gateway as IOT
 from ..error import KepError, KepHTTPError
 import inspect
+from ..utils import _url_parse_object
 
 IOT_ROOT_URL = '/project/_iot_gateway'
 MQTT_CLIENT_URL = '/mqtt_clients'
 REST_CLIENT_URL = '/rest_clients'
 REST_SERVER_URL = '/rest_servers'
 THINGWORX_URL = '/thingworx_clients'
 
@@ -38,21 +39,21 @@
             return '{}{}'.format(IOT_ROOT_URL, REST_SERVER_URL)
         elif agent_type == IOT.THINGWORX_AGENT:
             return '{}{}'.format(IOT_ROOT_URL, THINGWORX_URL)
         else:
             pass
     else:
         if agent_type == IOT.MQTT_CLIENT_AGENT:
-            return '{}{}/{}'.format(IOT_ROOT_URL, MQTT_CLIENT_URL, agent)
+            return '{}{}/{}'.format(IOT_ROOT_URL, MQTT_CLIENT_URL, _url_parse_object(agent))
         elif agent_type == IOT.REST_CLIENT_AGENT:
-            return '{}{}/{}'.format(IOT_ROOT_URL, REST_CLIENT_URL, agent)
+            return '{}{}/{}'.format(IOT_ROOT_URL, REST_CLIENT_URL, _url_parse_object(agent))
         elif agent_type == IOT.REST_SERVER_AGENT:
-            return '{}{}/{}'.format(IOT_ROOT_URL, REST_SERVER_URL,agent)
+            return '{}{}/{}'.format(IOT_ROOT_URL, REST_SERVER_URL,_url_parse_object(agent))
         elif agent_type == IOT.THINGWORX_AGENT:
-            return '{}{}/{}'.format(IOT_ROOT_URL, THINGWORX_URL, agent)
+            return '{}{}/{}'.format(IOT_ROOT_URL, THINGWORX_URL, _url_parse_object(agent))
         else:
             pass
 
 
 def add_iot_agent(server: server, DATA: Union[dict, list], agent_type: str = None) -> Union[bool, list]:
     '''Add a  `"agent"` or multiple `"agent"` objects of a specific type to Kepware's IoT Gateway. Can be used to pass children of an
     agent object such as iot items. This allows you to create an agent and iot items if desired. Multiple Agents need to be of the 
@@ -72,30 +73,30 @@
 
     :raises KepHTTPError: If urllib provides an HTTPError
     :raises KepURLError: If urllib provides an URLError
     '''
     
     if agent_type == None:
         try:
-            r = server._config_update(server.url + _create_url(DATA['iot_gateway.AGENTTYPES_TYPE']), DATA)
-            if r.code == 201: return True 
-            else: raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
+            # If it's a list, use the first agents type
+            if isinstance(DATA, list): agent_type = DATA[0]['iot_gateway.AGENTTYPES_TYPE']
+            else: agent_type = DATA['iot_gateway.AGENTTYPES_TYPE']
         except KeyError as err:
             err_msg = 'Error: No agent identified in DATA | Key Error: {}'.format(err)
             raise KepError(err_msg)
-    else:
-        r = server._config_add(server.url + _create_url(agent_type), DATA)
-        if r.code == 201: return True 
-        elif r.code == 207:
-            errors = [] 
-            for item in r.payload:
-                if item['code'] != 201:
-                    errors.append(item)
-            return errors
-        else: raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
+    
+    r = server._config_add(server.url + _create_url(agent_type), DATA)
+    if r.code == 201: return True 
+    elif r.code == 207:
+        errors = [] 
+        for item in r.payload:
+            if item['code'] != 201:
+                errors.append(item)
+        return errors
+    else: raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
 
 def del_iot_agent(server: server, agent: str, agent_type: str) -> bool:
     '''Delete a `"agent"` object in Kepware. This will delete all children as well
     
     :param server: instance of the `server` class
     :param agent: name of IoT Agent to delete
     :param agent_type: *(optional)* agent type to delete in IoT Gateway. Valid values are
```

### Comparing `kepconfig-1.2.0/kepconfig/iot_gateway/iot_items.py` & `kepconfig-1.2.1/kepconfig/iot_gateway/iot_items.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,28 +10,29 @@
 """
 
 from typing import Union
 from .. import utils
 from ..connection import server
 from .. import iot_gateway as IOT
 from ..error import KepError, KepHTTPError
+from ..utils import _url_parse_object
 
 IOT_ITEMS_ROOT = '/iot_items'
 
 def _create_url(tag = None):
     '''Creates url object for the "iot items" branch of Kepware's IoT Agents property model. Used 
     to build a part of Kepware Configuration API URL structure
     
     Returns the device specific url when a value is passed as the iot item name.
     '''
     if tag == None:
         return IOT_ITEMS_ROOT
     else: 
         normalized_tag = utils._address_dedecimal(tag)
-        return '{}/{}'.format(IOT_ITEMS_ROOT,normalized_tag)
+        return '{}/{}'.format(IOT_ITEMS_ROOT, _url_parse_object(normalized_tag))
 
 
 def add_iot_item(server: server, DATA: Union[dict, list], agent: str, agent_type: str) -> Union[bool, list]:
     '''Add a `"iot item"` or multiple `"iot item"` objects to Kepware's IoT Gateway agent. Additionally 
     it can be used to pass a list of iot items to be added to an agent all at once.
 
     :param server: instance of the `server` class
```

### Comparing `kepconfig-1.2.0/kepconfig/structures.py` & `kepconfig-1.2.1/kepconfig/structures.py`

 * *Files identical despite different names*

### Comparing `kepconfig-1.2.0/kepconfig/utils.py` & `kepconfig-1.2.1/kepconfig/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 # license information.
 # --------------------------------------------------------------------------
 
 r"""`utils` provides general utilities to help manage 
 various objects for Kepware's configuration
 """
 
+from urllib import parse
+
 def path_split(path: str):
     '''Used to split the standard Kepware address decimal notation into a dict that contains the 
     *channel*, *device* and *tag_path* keys.
 
     :param path: standard Kepware address in decimal notation ("ch1.dev1.tg1.tg2.tg3")
     :return: dict that contains the "channel", "device" and "tag_path"
     :rtype: dict
@@ -32,11 +34,21 @@
         elif x == 1:
             path_obj['device'] = path_list[1]
         else:
             path_obj['tag_path'] = path_list[2].split('.')
     return path_obj
 
 def _address_dedecimal(tag_address):
+    '''Used to handle URL references where decimal notation isn't supported in object names, i.e. IoT Gateway items.
+    
+    Replaces `.` with `_` and removes leading `_` for system tag references'''
     if tag_address[0] == '_':
         tag_address = tag_address[1::]
     updated = tag_address.replace('.','_')
     return updated
+
+def _url_parse_object(object):
+    '''Common url parse to handle reserved characters. Used to convert object 
+    names when building URLs.
+    
+    Reserved character list that Kepware allows in object names: :/?#[]@!$&'()*+,;='''
+    return parse.quote(object, safe='')
```

### Comparing `kepconfig-1.2.0/kepconfig.egg-info/PKG-INFO` & `kepconfig-1.2.1/kepconfig.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kepconfig
-Version: 1.2.0
+Version: 1.2.1
 Summary: SDK package for Kepware Configuration API
 Home-page: https://github.com/PTCInc/Kepware-ConfigAPI-SDK-Python
 Author: PTC Inc
 License: MIT License
 Keywords: Kepware,OPC,Configuration,Thingworx
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -23,14 +23,16 @@
 
 # Kepware Configuration API SDK for Python
 
 [![Released Version](https://img.shields.io/pypi/v/kepconfig)](https://pypi.org/project/kepconfig) [![Supported Versions](https://img.shields.io/pypi/pyversions/kepconfig)](https://pypi.org/project/kepconfig) ![PyPI - Downloads](https://img.shields.io/pypi/dm/kepconfig) ![PyPI - License](https://img.shields.io/pypi/l/kepconfig)
 
 This is a package to help create Python applications to conduct operations with the Kepware Configuration API. This package is designed to work with all versions of Kepware that support the Configuration API including Thingworx Kepware Server (TKS), Thingworx Kepware Edge (TKE) and KEPServerEX (KEP).
 
+**API reference documentation is available on [Github Pages](https://ptcinc.github.io/Kepware-ConfigAPI-SDK-Python)**
+
 ## Prerequisites
 
 Package supported and tested on Python 3.9 or later. Older versions support earlier Python 3 environments but have less functionality. All HTTP communication is handled by the [urllib](https://docs.python.org/3/library/urllib.html#module-urllib) Python standard library.
 
 ## Features
 
 - Supports both HTTP and HTTPS connections with certificate validation options
@@ -94,15 +96,15 @@
 ## Key Concepts
 
 NOTE: Detailed examples can also be found in the [examples](./examples/) folder.
 
 ### Create server connection
 
 ```python
-import kepconfig.connection
+from kepconfig import connection
 
 server = connection.server(host = '127.0.0.1', port = 57412, user = 'Administrator', pw = '')
 
 # For HTTPS connections:
 server = connection.server(host = '127.0.0.1', port = 57512, user = 'Administrator', pw = '', https=True)
 
 ```
@@ -140,15 +142,15 @@
     },
     {
             "common.ALLTYPES_NAME": "Temp2",
             "servermain.TAG_ADDRESS": "R1"
     }
 ]
 tag_path = '{}.{}.{}'.format(ch_name, dev_name, tag_group_path)
-result = tag.add_tag(server, tag_path, tag_info))
+result = tag.add_tag(server, tag_path, tag_info)
 
 ```
 
 ## Need More Information
 
 **Visit:**
```

### Comparing `kepconfig-1.2.0/kepconfig.egg-info/SOURCES.txt` & `kepconfig-1.2.1/kepconfig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kepconfig-1.2.0/setup.py` & `kepconfig-1.2.1/setup.py`

 * *Files identical despite different names*

