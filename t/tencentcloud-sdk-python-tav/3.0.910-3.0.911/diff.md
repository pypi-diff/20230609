# Comparing `tmp/tencentcloud-sdk-python-tav-3.0.910.tar.gz` & `tmp/tencentcloud-sdk-python-tav-3.0.911.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tav-3.0.910.tar", last modified: Thu Jun  8 09:19:29 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tav-3.0.911.tar", last modified: Fri Jun  9 02:27:17 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tav-3.0.910.tar` & `tencentcloud-sdk-python-tav-3.0.911.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:19:29.000000 tencentcloud-sdk-python-tav-3.0.910/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-08 09:19:28.000000 tencentcloud-sdk-python-tav-3.0.910/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:19:29.000000 tencentcloud-sdk-python-tav-3.0.910/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:19:29.000000 tencentcloud-sdk-python-tav-3.0.910/tencentcloud/tav/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:19:29.000000 tencentcloud-sdk-python-tav-3.0.910/tencentcloud/tav/v20190118/
--rw-r--r--   0 root         (0) root         (0)     4379 2023-06-08 09:19:28.000000 tencentcloud-sdk-python-tav-3.0.910/tencentcloud/tav/v20190118/tav_client.py
--rw-r--r--   0 root         (0) root         (0)      652 2023-06-08 09:19:28.000000 tencentcloud-sdk-python-tav-3.0.910/tencentcloud/tav/v20190118/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 09:19:28.000000 tencentcloud-sdk-python-tav-3.0.910/tencentcloud/tav/v20190118/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8548 2023-06-08 09:19:28.000000 tencentcloud-sdk-python-tav-3.0.910/tencentcloud/tav/v20190118/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 09:19:28.000000 tencentcloud-sdk-python-tav-3.0.910/tencentcloud/tav/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-08 09:19:28.000000 tencentcloud-sdk-python-tav-3.0.910/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:19:29.000000 tencentcloud-sdk-python-tav-3.0.910/tencentcloud_sdk_python_tav.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 09:19:29.000000 tencentcloud-sdk-python-tav-3.0.910/tencentcloud_sdk_python_tav.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-08 09:19:29.000000 tencentcloud-sdk-python-tav-3.0.910/tencentcloud_sdk_python_tav.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-08 09:19:29.000000 tencentcloud-sdk-python-tav-3.0.910/tencentcloud_sdk_python_tav.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-08 09:19:29.000000 tencentcloud-sdk-python-tav-3.0.910/tencentcloud_sdk_python_tav.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-08 09:19:29.000000 tencentcloud-sdk-python-tav-3.0.910/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-08 09:19:28.000000 tencentcloud-sdk-python-tav-3.0.910/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-08 09:19:29.000000 tencentcloud-sdk-python-tav-3.0.910/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:27:17.000000 tencentcloud-sdk-python-tav-3.0.911/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-09 02:27:17.000000 tencentcloud-sdk-python-tav-3.0.911/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:27:17.000000 tencentcloud-sdk-python-tav-3.0.911/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:27:17.000000 tencentcloud-sdk-python-tav-3.0.911/tencentcloud/tav/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:27:17.000000 tencentcloud-sdk-python-tav-3.0.911/tencentcloud/tav/v20190118/
+-rw-r--r--   0 root         (0) root         (0)     4379 2023-06-09 02:27:17.000000 tencentcloud-sdk-python-tav-3.0.911/tencentcloud/tav/v20190118/tav_client.py
+-rw-r--r--   0 root         (0) root         (0)      652 2023-06-09 02:27:17.000000 tencentcloud-sdk-python-tav-3.0.911/tencentcloud/tav/v20190118/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:27:17.000000 tencentcloud-sdk-python-tav-3.0.911/tencentcloud/tav/v20190118/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8548 2023-06-09 02:27:17.000000 tencentcloud-sdk-python-tav-3.0.911/tencentcloud/tav/v20190118/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:27:17.000000 tencentcloud-sdk-python-tav-3.0.911/tencentcloud/tav/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-09 02:27:17.000000 tencentcloud-sdk-python-tav-3.0.911/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:27:17.000000 tencentcloud-sdk-python-tav-3.0.911/tencentcloud_sdk_python_tav.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 02:27:17.000000 tencentcloud-sdk-python-tav-3.0.911/tencentcloud_sdk_python_tav.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-09 02:27:17.000000 tencentcloud-sdk-python-tav-3.0.911/tencentcloud_sdk_python_tav.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-09 02:27:17.000000 tencentcloud-sdk-python-tav-3.0.911/tencentcloud_sdk_python_tav.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-09 02:27:17.000000 tencentcloud-sdk-python-tav-3.0.911/tencentcloud_sdk_python_tav.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-09 02:27:17.000000 tencentcloud-sdk-python-tav-3.0.911/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-09 02:27:17.000000 tencentcloud-sdk-python-tav-3.0.911/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-09 02:27:17.000000 tencentcloud-sdk-python-tav-3.0.911/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tav-3.0.910/README.rst` & `tencentcloud-sdk-python-tav-3.0.911/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tav-3.0.910/tencentcloud/tav/v20190118/tav_client.py` & `tencentcloud-sdk-python-tav-3.0.911/tencentcloud/tav/v20190118/tav_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tav-3.0.910/tencentcloud/tav/v20190118/errorcodes.py` & `tencentcloud-sdk-python-tav-3.0.911/tencentcloud/tav/v20190118/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tav-3.0.910/tencentcloud/tav/v20190118/models.py` & `tencentcloud-sdk-python-tav-3.0.911/tencentcloud/tav/v20190118/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tav-3.0.910/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tav-3.0.911/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tav-3.0.910/tencentcloud_sdk_python_tav.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tav-3.0.911/tencentcloud_sdk_python_tav.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tav
-Version: 3.0.910
+Version: 3.0.911
 Summary: Tencent Cloud Tav SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tav-3.0.910/PKG-INFO` & `tencentcloud-sdk-python-tav-3.0.911/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tav
-Version: 3.0.910
+Version: 3.0.911
 Summary: Tencent Cloud Tav SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tav-3.0.910/setup.py` & `tencentcloud-sdk-python-tav-3.0.911/setup.py`

 * *Files identical despite different names*

