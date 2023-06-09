# Comparing `tmp/tencentcloud-sdk-python-trro-3.0.910.tar.gz` & `tmp/tencentcloud-sdk-python-trro-3.0.911.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-trro-3.0.910.tar", last modified: Thu Jun  8 09:23:57 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-trro-3.0.911.tar", last modified: Fri Jun  9 02:30:31 2023, max compression
```

## Comparing `tencentcloud-sdk-python-trro-3.0.910.tar` & `tencentcloud-sdk-python-trro-3.0.911.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:23:57.000000 tencentcloud-sdk-python-trro-3.0.910/
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-08 09:23:57.000000 tencentcloud-sdk-python-trro-3.0.910/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:23:57.000000 tencentcloud-sdk-python-trro-3.0.910/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:23:57.000000 tencentcloud-sdk-python-trro-3.0.910/tencentcloud/trro/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 09:23:57.000000 tencentcloud-sdk-python-trro-3.0.910/tencentcloud/trro/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:23:57.000000 tencentcloud-sdk-python-trro-3.0.910/tencentcloud/trro/v20220325/
--rw-r--r--   0 root         (0) root         (0)    21281 2023-06-08 09:23:57.000000 tencentcloud-sdk-python-trro-3.0.910/tencentcloud/trro/v20220325/trro_client.py
--rw-r--r--   0 root         (0) root         (0)     1069 2023-06-08 09:23:57.000000 tencentcloud-sdk-python-trro-3.0.910/tencentcloud/trro/v20220325/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 09:23:57.000000 tencentcloud-sdk-python-trro-3.0.910/tencentcloud/trro/v20220325/__init__.py
--rw-r--r--   0 root         (0) root         (0)    60156 2023-06-08 09:23:57.000000 tencentcloud-sdk-python-trro-3.0.910/tencentcloud/trro/v20220325/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-08 09:23:57.000000 tencentcloud-sdk-python-trro-3.0.910/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:23:57.000000 tencentcloud-sdk-python-trro-3.0.910/tencentcloud_sdk_python_trro.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 09:23:57.000000 tencentcloud-sdk-python-trro-3.0.910/tencentcloud_sdk_python_trro.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-06-08 09:23:57.000000 tencentcloud-sdk-python-trro-3.0.910/tencentcloud_sdk_python_trro.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-08 09:23:57.000000 tencentcloud-sdk-python-trro-3.0.910/tencentcloud_sdk_python_trro.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-08 09:23:57.000000 tencentcloud-sdk-python-trro-3.0.910/tencentcloud_sdk_python_trro.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-08 09:23:57.000000 tencentcloud-sdk-python-trro-3.0.910/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-06-08 09:23:57.000000 tencentcloud-sdk-python-trro-3.0.910/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-08 09:23:57.000000 tencentcloud-sdk-python-trro-3.0.910/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:30:31.000000 tencentcloud-sdk-python-trro-3.0.911/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-09 02:30:31.000000 tencentcloud-sdk-python-trro-3.0.911/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:30:31.000000 tencentcloud-sdk-python-trro-3.0.911/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:30:31.000000 tencentcloud-sdk-python-trro-3.0.911/tencentcloud/trro/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:30:31.000000 tencentcloud-sdk-python-trro-3.0.911/tencentcloud/trro/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:30:31.000000 tencentcloud-sdk-python-trro-3.0.911/tencentcloud/trro/v20220325/
+-rw-r--r--   0 root         (0) root         (0)    21281 2023-06-09 02:30:31.000000 tencentcloud-sdk-python-trro-3.0.911/tencentcloud/trro/v20220325/trro_client.py
+-rw-r--r--   0 root         (0) root         (0)     1069 2023-06-09 02:30:31.000000 tencentcloud-sdk-python-trro-3.0.911/tencentcloud/trro/v20220325/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:30:31.000000 tencentcloud-sdk-python-trro-3.0.911/tencentcloud/trro/v20220325/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    60156 2023-06-09 02:30:31.000000 tencentcloud-sdk-python-trro-3.0.911/tencentcloud/trro/v20220325/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-09 02:30:31.000000 tencentcloud-sdk-python-trro-3.0.911/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:30:31.000000 tencentcloud-sdk-python-trro-3.0.911/tencentcloud_sdk_python_trro.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 02:30:31.000000 tencentcloud-sdk-python-trro-3.0.911/tencentcloud_sdk_python_trro.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-06-09 02:30:31.000000 tencentcloud-sdk-python-trro-3.0.911/tencentcloud_sdk_python_trro.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-09 02:30:31.000000 tencentcloud-sdk-python-trro-3.0.911/tencentcloud_sdk_python_trro.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-09 02:30:31.000000 tencentcloud-sdk-python-trro-3.0.911/tencentcloud_sdk_python_trro.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-09 02:30:31.000000 tencentcloud-sdk-python-trro-3.0.911/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-06-09 02:30:31.000000 tencentcloud-sdk-python-trro-3.0.911/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-09 02:30:31.000000 tencentcloud-sdk-python-trro-3.0.911/setup.cfg
```

### Comparing `tencentcloud-sdk-python-trro-3.0.910/README.rst` & `tencentcloud-sdk-python-trro-3.0.911/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trro-3.0.910/tencentcloud/trro/v20220325/trro_client.py` & `tencentcloud-sdk-python-trro-3.0.911/tencentcloud/trro/v20220325/trro_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trro-3.0.910/tencentcloud/trro/v20220325/errorcodes.py` & `tencentcloud-sdk-python-trro-3.0.911/tencentcloud/trro/v20220325/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trro-3.0.910/tencentcloud/trro/v20220325/models.py` & `tencentcloud-sdk-python-trro-3.0.911/tencentcloud/trro/v20220325/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trro-3.0.910/tencentcloud/__init__.py` & `tencentcloud-sdk-python-trro-3.0.911/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.910'
+__version__ = '3.0.911'
```

### Comparing `tencentcloud-sdk-python-trro-3.0.910/tencentcloud_sdk_python_trro.egg-info/PKG-INFO` & `tencentcloud-sdk-python-trro-3.0.911/tencentcloud_sdk_python_trro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trro
-Version: 3.0.910
+Version: 3.0.911
 Summary: Tencent Cloud Trro SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-trro-3.0.910/PKG-INFO` & `tencentcloud-sdk-python-trro-3.0.911/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trro
-Version: 3.0.910
+Version: 3.0.911
 Summary: Tencent Cloud Trro SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-trro-3.0.910/setup.py` & `tencentcloud-sdk-python-trro-3.0.911/setup.py`

 * *Files identical despite different names*
