# Comparing `tmp/aliyun-python-sdk-avatar-1.0.2.tar.gz` & `tmp/aliyun-python-sdk-avatar-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-avatar-1.0.2.tar", last modified: Fri Nov  4 03:13:27 2022, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-avatar-1.0.9.tar", last modified: Fri Nov 25 07:50:27 2022, max compression
```

## Comparing `aliyun-python-sdk-avatar-1.0.2.tar` & `aliyun-python-sdk-avatar-1.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-04 03:13:27.000000 aliyun-python-sdk-avatar-1.0.2/
--rw-r--r--   0 root         (0) root         (0)      575 2022-11-04 03:13:27.000000 aliyun-python-sdk-avatar-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2022-11-04 03:13:27.000000 aliyun-python-sdk-avatar-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1552 2022-11-04 03:13:27.000000 aliyun-python-sdk-avatar-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      533 2022-11-04 03:13:27.000000 aliyun-python-sdk-avatar-1.0.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-04 03:13:27.000000 aliyun-python-sdk-avatar-1.0.2/aliyun_python_sdk_avatar.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1552 2022-11-04 03:13:27.000000 aliyun-python-sdk-avatar-1.0.2/aliyun_python_sdk_avatar.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1032 2022-11-04 03:13:27.000000 aliyun-python-sdk-avatar-1.0.2/aliyun_python_sdk_avatar.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-04 03:13:27.000000 aliyun-python-sdk-avatar-1.0.2/aliyun_python_sdk_avatar.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2022-11-04 03:13:27.000000 aliyun-python-sdk-avatar-1.0.2/aliyun_python_sdk_avatar.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2022-11-04 03:13:27.000000 aliyun-python-sdk-avatar-1.0.2/aliyun_python_sdk_avatar.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-04 03:13:27.000000 aliyun-python-sdk-avatar-1.0.2/aliyunsdkavatar/
--rw-r--r--   0 root         (0) root         (0)       21 2022-11-04 03:13:27.000000 aliyun-python-sdk-avatar-1.0.2/aliyunsdkavatar/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-04 03:13:27.000000 aliyun-python-sdk-avatar-1.0.2/aliyunsdkavatar/request/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-04 03:13:27.000000 aliyun-python-sdk-avatar-1.0.2/aliyunsdkavatar/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-04 03:13:27.000000 aliyun-python-sdk-avatar-1.0.2/aliyunsdkavatar/request/v20220130/
--rw-r--r--   0 root         (0) root         (0)     1530 2022-11-04 03:13:27.000000 aliyun-python-sdk-avatar-1.0.2/aliyunsdkavatar/request/v20220130/CancelVideoTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2933 2022-11-04 03:13:27.000000 aliyun-python-sdk-avatar-1.0.2/aliyunsdkavatar/request/v20220130/DuplexDecisionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1531 2022-11-04 03:13:27.000000 aliyun-python-sdk-avatar-1.0.2/aliyunsdkavatar/request/v20220130/GetVideoTaskInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1546 2022-11-04 03:13:27.000000 aliyun-python-sdk-avatar-1.0.2/aliyunsdkavatar/request/v20220130/QueryRunningInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1773 2022-11-04 03:13:27.000000 aliyun-python-sdk-avatar-1.0.2/aliyunsdkavatar/request/v20220130/SendMessageRequest.py
--rw-r--r--   0 root         (0) root         (0)     1902 2022-11-04 03:13:27.000000 aliyun-python-sdk-avatar-1.0.2/aliyunsdkavatar/request/v20220130/StartInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1357 2022-11-04 03:13:27.000000 aliyun-python-sdk-avatar-1.0.2/aliyunsdkavatar/request/v20220130/StopInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1892 2022-11-04 03:13:27.000000 aliyun-python-sdk-avatar-1.0.2/aliyunsdkavatar/request/v20220130/SubmitTextTo2DAvatarVideoTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1892 2022-11-04 03:13:27.000000 aliyun-python-sdk-avatar-1.0.2/aliyunsdkavatar/request/v20220130/SubmitTextTo3DAvatarVideoTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1884 2022-11-04 03:13:27.000000 aliyun-python-sdk-avatar-1.0.2/aliyunsdkavatar/request/v20220130/SubmitTextToSignVideoTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-04 03:13:27.000000 aliyun-python-sdk-avatar-1.0.2/aliyunsdkavatar/request/v20220130/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2022-11-04 03:13:27.000000 aliyun-python-sdk-avatar-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2467 2022-11-04 03:13:27.000000 aliyun-python-sdk-avatar-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 07:50:27.000000 aliyun-python-sdk-avatar-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      575 2022-11-25 07:50:27.000000 aliyun-python-sdk-avatar-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2022-11-25 07:50:27.000000 aliyun-python-sdk-avatar-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1552 2022-11-25 07:50:27.000000 aliyun-python-sdk-avatar-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      533 2022-11-25 07:50:27.000000 aliyun-python-sdk-avatar-1.0.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 07:50:27.000000 aliyun-python-sdk-avatar-1.0.9/aliyun_python_sdk_avatar.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1552 2022-11-25 07:50:27.000000 aliyun-python-sdk-avatar-1.0.9/aliyun_python_sdk_avatar.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1032 2022-11-25 07:50:27.000000 aliyun-python-sdk-avatar-1.0.9/aliyun_python_sdk_avatar.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-25 07:50:27.000000 aliyun-python-sdk-avatar-1.0.9/aliyun_python_sdk_avatar.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2022-11-25 07:50:27.000000 aliyun-python-sdk-avatar-1.0.9/aliyun_python_sdk_avatar.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2022-11-25 07:50:27.000000 aliyun-python-sdk-avatar-1.0.9/aliyun_python_sdk_avatar.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 07:50:27.000000 aliyun-python-sdk-avatar-1.0.9/aliyunsdkavatar/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-11-25 07:50:27.000000 aliyun-python-sdk-avatar-1.0.9/aliyunsdkavatar/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 07:50:27.000000 aliyun-python-sdk-avatar-1.0.9/aliyunsdkavatar/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-25 07:50:27.000000 aliyun-python-sdk-avatar-1.0.9/aliyunsdkavatar/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 07:50:27.000000 aliyun-python-sdk-avatar-1.0.9/aliyunsdkavatar/request/v20220130/
+-rw-r--r--   0 root         (0) root         (0)     1530 2022-11-25 07:50:27.000000 aliyun-python-sdk-avatar-1.0.9/aliyunsdkavatar/request/v20220130/CancelVideoTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2933 2022-11-25 07:50:27.000000 aliyun-python-sdk-avatar-1.0.9/aliyunsdkavatar/request/v20220130/DuplexDecisionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1531 2022-11-25 07:50:27.000000 aliyun-python-sdk-avatar-1.0.9/aliyunsdkavatar/request/v20220130/GetVideoTaskInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1546 2022-11-25 07:50:27.000000 aliyun-python-sdk-avatar-1.0.9/aliyunsdkavatar/request/v20220130/QueryRunningInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1773 2022-11-25 07:50:27.000000 aliyun-python-sdk-avatar-1.0.9/aliyunsdkavatar/request/v20220130/SendMessageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1902 2022-11-25 07:50:27.000000 aliyun-python-sdk-avatar-1.0.9/aliyunsdkavatar/request/v20220130/StartInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1357 2022-11-25 07:50:27.000000 aliyun-python-sdk-avatar-1.0.9/aliyunsdkavatar/request/v20220130/StopInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2292 2022-11-25 07:50:27.000000 aliyun-python-sdk-avatar-1.0.9/aliyunsdkavatar/request/v20220130/SubmitTextTo2DAvatarVideoTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1892 2022-11-25 07:50:27.000000 aliyun-python-sdk-avatar-1.0.9/aliyunsdkavatar/request/v20220130/SubmitTextTo3DAvatarVideoTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1884 2022-11-25 07:50:27.000000 aliyun-python-sdk-avatar-1.0.9/aliyunsdkavatar/request/v20220130/SubmitTextToSignVideoTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-25 07:50:27.000000 aliyun-python-sdk-avatar-1.0.9/aliyunsdkavatar/request/v20220130/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2022-11-25 07:50:27.000000 aliyun-python-sdk-avatar-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2467 2022-11-25 07:50:27.000000 aliyun-python-sdk-avatar-1.0.9/setup.py
```

### Comparing `aliyun-python-sdk-avatar-1.0.2/LICENSE` & `aliyun-python-sdk-avatar-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-avatar-1.0.2/PKG-INFO` & `aliyun-python-sdk-avatar-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-avatar
-Version: 1.0.2
+Version: 1.0.9
 Summary: The avatar module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-avatar
```

### Comparing `aliyun-python-sdk-avatar-1.0.2/README.rst` & `aliyun-python-sdk-avatar-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-avatar-1.0.2/aliyun_python_sdk_avatar.egg-info/PKG-INFO` & `aliyun-python-sdk-avatar-1.0.9/aliyun_python_sdk_avatar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-avatar
-Version: 1.0.2
+Version: 1.0.9
 Summary: The avatar module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-avatar
```

### Comparing `aliyun-python-sdk-avatar-1.0.2/aliyun_python_sdk_avatar.egg-info/SOURCES.txt` & `aliyun-python-sdk-avatar-1.0.9/aliyun_python_sdk_avatar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-avatar-1.0.2/aliyunsdkavatar/request/v20220130/CancelVideoTaskRequest.py` & `aliyun-python-sdk-avatar-1.0.9/aliyunsdkavatar/request/v20220130/CancelVideoTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-avatar-1.0.2/aliyunsdkavatar/request/v20220130/DuplexDecisionRequest.py` & `aliyun-python-sdk-avatar-1.0.9/aliyunsdkavatar/request/v20220130/DuplexDecisionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-avatar-1.0.2/aliyunsdkavatar/request/v20220130/GetVideoTaskInfoRequest.py` & `aliyun-python-sdk-avatar-1.0.9/aliyunsdkavatar/request/v20220130/GetVideoTaskInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-avatar-1.0.2/aliyunsdkavatar/request/v20220130/QueryRunningInstanceRequest.py` & `aliyun-python-sdk-avatar-1.0.9/aliyunsdkavatar/request/v20220130/QueryRunningInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-avatar-1.0.2/aliyunsdkavatar/request/v20220130/SendMessageRequest.py` & `aliyun-python-sdk-avatar-1.0.9/aliyunsdkavatar/request/v20220130/SendMessageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-avatar-1.0.2/aliyunsdkavatar/request/v20220130/StartInstanceRequest.py` & `aliyun-python-sdk-avatar-1.0.9/aliyunsdkavatar/request/v20220130/StartInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-avatar-1.0.2/aliyunsdkavatar/request/v20220130/StopInstanceRequest.py` & `aliyun-python-sdk-avatar-1.0.9/aliyunsdkavatar/request/v20220130/StopInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-avatar-1.0.2/aliyunsdkavatar/request/v20220130/SubmitTextTo2DAvatarVideoTaskRequest.py` & `aliyun-python-sdk-avatar-1.0.9/aliyunsdkavatar/request/v20220130/SubmitTextToSignVideoTaskRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 import json
 
-class SubmitTextTo2DAvatarVideoTaskRequest(RpcRequest):
+class SubmitTextToSignVideoTaskRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'avatar', '2022-01-30', 'SubmitTextTo2DAvatarVideoTask')
+		RpcRequest.__init__(self, 'avatar', '2022-01-30', 'SubmitTextToSignVideoTask')
 		self.set_method('POST')
 
 	def get_App(self): # Struct
 		return self.get_query_params().get('App')
 
 	def set_App(self, App):  # Struct
 		self.add_query_param("App", json.dumps(App))
```

### Comparing `aliyun-python-sdk-avatar-1.0.2/aliyunsdkavatar/request/v20220130/SubmitTextTo3DAvatarVideoTaskRequest.py` & `aliyun-python-sdk-avatar-1.0.9/aliyunsdkavatar/request/v20220130/SubmitTextTo3DAvatarVideoTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-avatar-1.0.2/setup.py` & `aliyun-python-sdk-avatar-1.0.9/setup.py`

 * *Files identical despite different names*

