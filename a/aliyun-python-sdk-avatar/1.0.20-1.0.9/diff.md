# Comparing `tmp/aliyun-python-sdk-avatar-1.0.20.tar.gz` & `tmp/aliyun-python-sdk-avatar-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-avatar-1.0.20.tar", last modified: Fri Jun  9 03:41:40 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-avatar-1.0.9.tar", last modified: Fri Nov 25 07:50:27 2022, max compression
```

## Comparing `aliyun-python-sdk-avatar-1.0.20.tar` & `aliyun-python-sdk-avatar-1.0.9.tar`

### file list

```diff
@@ -1,36 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 03:41:40.000000 aliyun-python-sdk-avatar-1.0.20/
--rw-r--r--   0 root         (0) root         (0)      575 2023-06-09 03:41:40.000000 aliyun-python-sdk-avatar-1.0.20/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-06-09 03:41:40.000000 aliyun-python-sdk-avatar-1.0.20/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1553 2023-06-09 03:41:40.000000 aliyun-python-sdk-avatar-1.0.20/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      533 2023-06-09 03:41:40.000000 aliyun-python-sdk-avatar-1.0.20/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 03:41:40.000000 aliyun-python-sdk-avatar-1.0.20/aliyun_python_sdk_avatar.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1553 2023-06-09 03:41:40.000000 aliyun-python-sdk-avatar-1.0.20/aliyun_python_sdk_avatar.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1491 2023-06-09 03:41:40.000000 aliyun-python-sdk-avatar-1.0.20/aliyun_python_sdk_avatar.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 03:41:40.000000 aliyun-python-sdk-avatar-1.0.20/aliyun_python_sdk_avatar.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-06-09 03:41:40.000000 aliyun-python-sdk-avatar-1.0.20/aliyun_python_sdk_avatar.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-09 03:41:40.000000 aliyun-python-sdk-avatar-1.0.20/aliyun_python_sdk_avatar.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 03:41:40.000000 aliyun-python-sdk-avatar-1.0.20/aliyunsdkavatar/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 03:41:40.000000 aliyun-python-sdk-avatar-1.0.20/aliyunsdkavatar/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 03:41:40.000000 aliyun-python-sdk-avatar-1.0.20/aliyunsdkavatar/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 03:41:40.000000 aliyun-python-sdk-avatar-1.0.20/aliyunsdkavatar/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 03:41:40.000000 aliyun-python-sdk-avatar-1.0.20/aliyunsdkavatar/request/v20220130/
--rw-r--r--   0 root         (0) root         (0)     1530 2023-06-09 03:41:40.000000 aliyun-python-sdk-avatar-1.0.20/aliyunsdkavatar/request/v20220130/CancelVideoTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1383 2023-06-09 03:41:40.000000 aliyun-python-sdk-avatar-1.0.20/aliyunsdkavatar/request/v20220130/CloseTimedResetOperateRequest.py
--rw-r--r--   0 root         (0) root         (0)     2933 2023-06-09 03:41:40.000000 aliyun-python-sdk-avatar-1.0.20/aliyunsdkavatar/request/v20220130/DuplexDecisionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1531 2023-06-09 03:41:40.000000 aliyun-python-sdk-avatar-1.0.20/aliyunsdkavatar/request/v20220130/GetVideoTaskInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1504 2023-06-09 03:41:40.000000 aliyun-python-sdk-avatar-1.0.20/aliyunsdkavatar/request/v20220130/LicenseAuthRequest.py
--rw-r--r--   0 root         (0) root         (0)     1713 2023-06-09 03:41:40.000000 aliyun-python-sdk-avatar-1.0.20/aliyunsdkavatar/request/v20220130/QueryAvatarListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1324 2023-06-09 03:41:40.000000 aliyun-python-sdk-avatar-1.0.20/aliyunsdkavatar/request/v20220130/QueryAvatarRequest.py
--rw-r--r--   0 root         (0) root         (0)     1546 2023-06-09 03:41:40.000000 aliyun-python-sdk-avatar-1.0.20/aliyunsdkavatar/request/v20220130/QueryRunningInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1395 2023-06-09 03:41:40.000000 aliyun-python-sdk-avatar-1.0.20/aliyunsdkavatar/request/v20220130/QueryTimedResetOperateStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1954 2023-06-09 03:41:40.000000 aliyun-python-sdk-avatar-1.0.20/aliyunsdkavatar/request/v20220130/SendMessageRequest.py
--rw-r--r--   0 root         (0) root         (0)     1902 2023-06-09 03:41:40.000000 aliyun-python-sdk-avatar-1.0.20/aliyunsdkavatar/request/v20220130/StartInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1383 2023-06-09 03:41:40.000000 aliyun-python-sdk-avatar-1.0.20/aliyunsdkavatar/request/v20220130/StartTimedResetOperateRequest.py
--rw-r--r--   0 root         (0) root         (0)     1357 2023-06-09 03:41:40.000000 aliyun-python-sdk-avatar-1.0.20/aliyunsdkavatar/request/v20220130/StopInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2091 2023-06-09 03:41:40.000000 aliyun-python-sdk-avatar-1.0.20/aliyunsdkavatar/request/v20220130/SubmitAudioTo2DAvatarVideoTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2091 2023-06-09 03:41:40.000000 aliyun-python-sdk-avatar-1.0.20/aliyunsdkavatar/request/v20220130/SubmitAudioTo3DAvatarVideoTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2292 2023-06-09 03:41:40.000000 aliyun-python-sdk-avatar-1.0.20/aliyunsdkavatar/request/v20220130/SubmitTextTo2DAvatarVideoTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2095 2023-06-09 03:41:40.000000 aliyun-python-sdk-avatar-1.0.20/aliyunsdkavatar/request/v20220130/SubmitTextTo3DAvatarVideoTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 03:41:40.000000 aliyun-python-sdk-avatar-1.0.20/aliyunsdkavatar/request/v20220130/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-06-09 03:41:40.000000 aliyun-python-sdk-avatar-1.0.20/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2467 2023-06-09 03:41:40.000000 aliyun-python-sdk-avatar-1.0.20/setup.py
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

### Comparing `aliyun-python-sdk-avatar-1.0.20/LICENSE` & `aliyun-python-sdk-avatar-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-avatar-1.0.20/PKG-INFO` & `aliyun-python-sdk-avatar-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-avatar
-Version: 1.0.20
+Version: 1.0.9
 Summary: The avatar module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-avatar
```

### Comparing `aliyun-python-sdk-avatar-1.0.20/README.rst` & `aliyun-python-sdk-avatar-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-avatar-1.0.20/aliyun_python_sdk_avatar.egg-info/PKG-INFO` & `aliyun-python-sdk-avatar-1.0.9/aliyun_python_sdk_avatar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-avatar
-Version: 1.0.20
+Version: 1.0.9
 Summary: The avatar module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-avatar
```

### Comparing `aliyun-python-sdk-avatar-1.0.20/aliyunsdkavatar/request/v20220130/CancelVideoTaskRequest.py` & `aliyun-python-sdk-avatar-1.0.9/aliyunsdkavatar/request/v20220130/CancelVideoTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-avatar-1.0.20/aliyunsdkavatar/request/v20220130/CloseTimedResetOperateRequest.py` & `aliyun-python-sdk-avatar-1.0.9/aliyunsdkavatar/request/v20220130/QueryRunningInstanceRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,24 +14,30 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
+import json
 
-class CloseTimedResetOperateRequest(RpcRequest):
+class QueryRunningInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'avatar', '2022-01-30', 'CloseTimedResetOperate')
+		RpcRequest.__init__(self, 'avatar', '2022-01-30', 'QueryRunningInstance')
 		self.set_method('POST')
 
-	def get_InstanceId(self): # String
-		return self.get_query_params().get('InstanceId')
+	def get_App(self): # Struct
+		return self.get_query_params().get('App')
 
-	def set_InstanceId(self, InstanceId):  # String
-		self.add_query_param('InstanceId', InstanceId)
+	def set_App(self, App):  # Struct
+		self.add_query_param("App", json.dumps(App))
 	def get_TenantId(self): # Long
 		return self.get_query_params().get('TenantId')
 
 	def set_TenantId(self, TenantId):  # Long
 		self.add_query_param('TenantId', TenantId)
+	def get_SessionId(self): # String
+		return self.get_query_params().get('SessionId')
+
+	def set_SessionId(self, SessionId):  # String
+		self.add_query_param('SessionId', SessionId)
```

### Comparing `aliyun-python-sdk-avatar-1.0.20/aliyunsdkavatar/request/v20220130/DuplexDecisionRequest.py` & `aliyun-python-sdk-avatar-1.0.9/aliyunsdkavatar/request/v20220130/DuplexDecisionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-avatar-1.0.20/aliyunsdkavatar/request/v20220130/GetVideoTaskInfoRequest.py` & `aliyun-python-sdk-avatar-1.0.9/aliyunsdkavatar/request/v20220130/GetVideoTaskInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-avatar-1.0.20/aliyunsdkavatar/request/v20220130/LicenseAuthRequest.py` & `aliyun-python-sdk-avatar-1.0.9/aliyunsdkavatar/request/v20220130/SubmitTextTo3DAvatarVideoTaskRequest.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,29 +14,40 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
+import json
 
-class LicenseAuthRequest(RpcRequest):
+class SubmitTextTo3DAvatarVideoTaskRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'avatar', '2022-01-30', 'LicenseAuth')
+		RpcRequest.__init__(self, 'avatar', '2022-01-30', 'SubmitTextTo3DAvatarVideoTask')
 		self.set_method('POST')
 
-	def get_License(self): # String
-		return self.get_query_params().get('License')
+	def get_App(self): # Struct
+		return self.get_query_params().get('App')
 
-	def set_License(self, License):  # String
-		self.add_query_param('License', License)
-	def get_AppId(self): # String
-		return self.get_query_params().get('AppId')
+	def set_App(self, App):  # Struct
+		self.add_query_param("App", json.dumps(App))
+	def get_VideoInfo(self): # Struct
+		return self.get_query_params().get('VideoInfo')
 
-	def set_AppId(self, AppId):  # String
-		self.add_query_param('AppId', AppId)
+	def set_VideoInfo(self, VideoInfo):  # Struct
+		self.add_query_param("VideoInfo", json.dumps(VideoInfo))
 	def get_TenantId(self): # Long
 		return self.get_query_params().get('TenantId')
 
 	def set_TenantId(self, TenantId):  # Long
 		self.add_query_param('TenantId', TenantId)
+	def get_Text(self): # String
+		return self.get_query_params().get('Text')
+
+	def set_Text(self, Text):  # String
+		self.add_query_param('Text', Text)
+	def get_Title(self): # String
+		return self.get_query_params().get('Title')
+
+	def set_Title(self, Title):  # String
+		self.add_query_param('Title', Title)
```

### Comparing `aliyun-python-sdk-avatar-1.0.20/aliyunsdkavatar/request/v20220130/QueryAvatarListRequest.py` & `aliyun-python-sdk-avatar-1.0.9/aliyunsdkavatar/request/v20220130/SendMessageRequest.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,34 +14,35 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
+import json
 
-class QueryAvatarListRequest(RpcRequest):
+class SendMessageRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'avatar', '2022-01-30', 'QueryAvatarList')
+		RpcRequest.__init__(self, 'avatar', '2022-01-30', 'SendMessage')
 		self.set_method('POST')
 
-	def get_ModelType(self): # String
-		return self.get_query_params().get('ModelType')
+	def get_TextRequest(self): # String
+		return self.get_query_params().get('TextRequest')
 
-	def set_ModelType(self, ModelType):  # String
-		self.add_query_param('ModelType', ModelType)
-	def get_PageNo(self): # Integer
-		return self.get_query_params().get('PageNo')
-
-	def set_PageNo(self, PageNo):  # Integer
-		self.add_query_param('PageNo', PageNo)
+	def set_TextRequest(self, TextRequest):  # String
+		self.add_query_param('TextRequest', TextRequest)
 	def get_TenantId(self): # Long
 		return self.get_query_params().get('TenantId')
 
 	def set_TenantId(self, TenantId):  # Long
 		self.add_query_param('TenantId', TenantId)
-	def get_PageSize(self): # Integer
-		return self.get_query_params().get('PageSize')
+	def get_VAMLRequest(self): # Struct
+		return self.get_query_params().get('VAMLRequest')
+
+	def set_VAMLRequest(self, VAMLRequest):  # Struct
+		self.add_query_param("VAMLRequest", json.dumps(VAMLRequest))
+	def get_SessionId(self): # String
+		return self.get_query_params().get('SessionId')
 
-	def set_PageSize(self, PageSize):  # Integer
-		self.add_query_param('PageSize', PageSize)
+	def set_SessionId(self, SessionId):  # String
+		self.add_query_param('SessionId', SessionId)
```

### Comparing `aliyun-python-sdk-avatar-1.0.20/aliyunsdkavatar/request/v20220130/QueryAvatarRequest.py` & `aliyun-python-sdk-avatar-1.0.9/aliyunsdkavatar/request/v20220130/StopInstanceRequest.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,23 +15,23 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
-class QueryAvatarRequest(RpcRequest):
+class StopInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'avatar', '2022-01-30', 'QueryAvatar')
-		self.set_method('GET')
+		RpcRequest.__init__(self, 'avatar', '2022-01-30', 'StopInstance')
+		self.set_method('POST')
 
-	def get_Code(self): # String
-		return self.get_query_params().get('Code')
-
-	def set_Code(self, Code):  # String
-		self.add_query_param('Code', Code)
 	def get_TenantId(self): # Long
 		return self.get_query_params().get('TenantId')
 
 	def set_TenantId(self, TenantId):  # Long
 		self.add_query_param('TenantId', TenantId)
+	def get_SessionId(self): # String
+		return self.get_query_params().get('SessionId')
+
+	def set_SessionId(self, SessionId):  # String
+		self.add_query_param('SessionId', SessionId)
```

### Comparing `aliyun-python-sdk-avatar-1.0.20/aliyunsdkavatar/request/v20220130/QueryRunningInstanceRequest.py` & `aliyun-python-sdk-avatar-1.0.9/aliyunsdkavatar/request/v20220130/SubmitTextToSignVideoTaskRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,28 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 import json
 
-class QueryRunningInstanceRequest(RpcRequest):
+class SubmitTextToSignVideoTaskRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'avatar', '2022-01-30', 'QueryRunningInstance')
+		RpcRequest.__init__(self, 'avatar', '2022-01-30', 'SubmitTextToSignVideoTask')
 		self.set_method('POST')
 
 	def get_App(self): # Struct
 		return self.get_query_params().get('App')
 
 	def set_App(self, App):  # Struct
 		self.add_query_param("App", json.dumps(App))
+	def get_VideoInfo(self): # Struct
+		return self.get_query_params().get('VideoInfo')
+
+	def set_VideoInfo(self, VideoInfo):  # Struct
+		self.add_query_param("VideoInfo", json.dumps(VideoInfo))
 	def get_TenantId(self): # Long
 		return self.get_query_params().get('TenantId')
 
 	def set_TenantId(self, TenantId):  # Long
 		self.add_query_param('TenantId', TenantId)
-	def get_SessionId(self): # String
-		return self.get_query_params().get('SessionId')
+	def get_Text(self): # String
+		return self.get_query_params().get('Text')
+
+	def set_Text(self, Text):  # String
+		self.add_query_param('Text', Text)
+	def get_Title(self): # String
+		return self.get_query_params().get('Title')
 
-	def set_SessionId(self, SessionId):  # String
-		self.add_query_param('SessionId', SessionId)
+	def set_Title(self, Title):  # String
+		self.add_query_param('Title', Title)
```

### Comparing `aliyun-python-sdk-avatar-1.0.20/aliyunsdkavatar/request/v20220130/StartInstanceRequest.py` & `aliyun-python-sdk-avatar-1.0.9/aliyunsdkavatar/request/v20220130/StartInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-avatar-1.0.20/aliyunsdkavatar/request/v20220130/SubmitAudioTo2DAvatarVideoTaskRequest.py` & `aliyun-python-sdk-avatar-1.0.9/aliyunsdkavatar/request/v20220130/SubmitTextTo2DAvatarVideoTaskRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,43 +16,48 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 import json
 
-class SubmitAudioTo2DAvatarVideoTaskRequest(RpcRequest):
+class SubmitTextTo2DAvatarVideoTaskRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'avatar', '2022-01-30', 'SubmitAudioTo2DAvatarVideoTask')
+		RpcRequest.__init__(self, 'avatar', '2022-01-30', 'SubmitTextTo2DAvatarVideoTask')
 		self.set_method('POST')
 
 	def get_App(self): # Struct
 		return self.get_query_params().get('App')
 
 	def set_App(self, App):  # Struct
 		self.add_query_param("App", json.dumps(App))
 	def get_VideoInfo(self): # Struct
 		return self.get_query_params().get('VideoInfo')
 
 	def set_VideoInfo(self, VideoInfo):  # Struct
 		self.add_query_param("VideoInfo", json.dumps(VideoInfo))
+	def get_AudioInfo(self): # Struct
+		return self.get_query_params().get('AudioInfo')
+
+	def set_AudioInfo(self, AudioInfo):  # Struct
+		self.add_query_param("AudioInfo", json.dumps(AudioInfo))
 	def get_AvatarInfo(self): # Struct
 		return self.get_query_params().get('AvatarInfo')
 
 	def set_AvatarInfo(self, AvatarInfo):  # Struct
 		self.add_query_param("AvatarInfo", json.dumps(AvatarInfo))
 	def get_TenantId(self): # Long
 		return self.get_query_params().get('TenantId')
 
 	def set_TenantId(self, TenantId):  # Long
 		self.add_query_param('TenantId', TenantId)
+	def get_Text(self): # String
+		return self.get_query_params().get('Text')
+
+	def set_Text(self, Text):  # String
+		self.add_query_param('Text', Text)
 	def get_Title(self): # String
 		return self.get_query_params().get('Title')
 
 	def set_Title(self, Title):  # String
 		self.add_query_param('Title', Title)
-	def get_Url(self): # String
-		return self.get_query_params().get('Url')
-
-	def set_Url(self, Url):  # String
-		self.add_query_param('Url', Url)
```

### Comparing `aliyun-python-sdk-avatar-1.0.20/setup.py` & `aliyun-python-sdk-avatar-1.0.9/setup.py`

 * *Files identical despite different names*

