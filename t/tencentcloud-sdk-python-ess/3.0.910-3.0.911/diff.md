# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.910.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.911.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.910.tar", last modified: Thu Jun  8 09:11:03 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.911.tar", last modified: Fri Jun  9 02:19:12 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.910.tar` & `tencentcloud-sdk-python-ess-3.0.911.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:11:03.000000 tencentcloud-sdk-python-ess-3.0.910/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-08 09:11:03.000000 tencentcloud-sdk-python-ess-3.0.910/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:11:03.000000 tencentcloud-sdk-python-ess-3.0.910/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-08 09:11:03.000000 tencentcloud-sdk-python-ess-3.0.910/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:11:03.000000 tencentcloud-sdk-python-ess-3.0.910/tencentcloud/ess/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 09:11:03.000000 tencentcloud-sdk-python-ess-3.0.910/tencentcloud/ess/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:11:03.000000 tencentcloud-sdk-python-ess-3.0.910/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    55323 2023-06-08 09:11:03.000000 tencentcloud-sdk-python-ess-3.0.910/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)    24361 2023-06-08 09:11:03.000000 tencentcloud-sdk-python-ess-3.0.910/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 09:11:03.000000 tencentcloud-sdk-python-ess-3.0.910/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   238847 2023-06-08 09:11:03.000000 tencentcloud-sdk-python-ess-3.0.910/tencentcloud/ess/v20201111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:11:03.000000 tencentcloud-sdk-python-ess-3.0.910/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 09:11:03.000000 tencentcloud-sdk-python-ess-3.0.910/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-08 09:11:03.000000 tencentcloud-sdk-python-ess-3.0.910/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-08 09:11:03.000000 tencentcloud-sdk-python-ess-3.0.910/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-08 09:11:03.000000 tencentcloud-sdk-python-ess-3.0.910/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-08 09:11:03.000000 tencentcloud-sdk-python-ess-3.0.910/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-08 09:11:03.000000 tencentcloud-sdk-python-ess-3.0.910/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-08 09:11:03.000000 tencentcloud-sdk-python-ess-3.0.910/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:19:12.000000 tencentcloud-sdk-python-ess-3.0.911/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-09 02:19:12.000000 tencentcloud-sdk-python-ess-3.0.911/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:19:12.000000 tencentcloud-sdk-python-ess-3.0.911/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-09 02:19:12.000000 tencentcloud-sdk-python-ess-3.0.911/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:19:12.000000 tencentcloud-sdk-python-ess-3.0.911/tencentcloud/ess/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:19:12.000000 tencentcloud-sdk-python-ess-3.0.911/tencentcloud/ess/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:19:12.000000 tencentcloud-sdk-python-ess-3.0.911/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    56524 2023-06-09 02:19:12.000000 tencentcloud-sdk-python-ess-3.0.911/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)    24640 2023-06-09 02:19:12.000000 tencentcloud-sdk-python-ess-3.0.911/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:19:12.000000 tencentcloud-sdk-python-ess-3.0.911/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   240704 2023-06-09 02:19:12.000000 tencentcloud-sdk-python-ess-3.0.911/tencentcloud/ess/v20201111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:19:12.000000 tencentcloud-sdk-python-ess-3.0.911/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 02:19:12.000000 tencentcloud-sdk-python-ess-3.0.911/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-09 02:19:12.000000 tencentcloud-sdk-python-ess-3.0.911/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-09 02:19:12.000000 tencentcloud-sdk-python-ess-3.0.911/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-09 02:19:12.000000 tencentcloud-sdk-python-ess-3.0.911/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-09 02:19:12.000000 tencentcloud-sdk-python-ess-3.0.911/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-09 02:19:12.000000 tencentcloud-sdk-python-ess-3.0.911/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-09 02:19:12.000000 tencentcloud-sdk-python-ess-3.0.911/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ess-3.0.910/README.rst` & `tencentcloud-sdk-python-ess-3.0.911/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.910/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.911/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.910/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.911/tencentcloud/ess/v20201111/ess_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,14 +93,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def CancelUserAutoSignEnableUrl(self, request):
+        """此接口（CancelUserAutoSignEnableUrl）用来撤销发送给个人用户的自动签开通链接，撤销后对应的个人用户开通链接失效。若个人用户已经完成开通，将无法撤销。（处方单场景专用，使用此接口请与客户经理确认）
+
+        :param request: Request instance for CancelUserAutoSignEnableUrl.
+        :type request: :class:`tencentcloud.ess.v20201111.models.CancelUserAutoSignEnableUrlRequest`
+        :rtype: :class:`tencentcloud.ess.v20201111.models.CancelUserAutoSignEnableUrlResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CancelUserAutoSignEnableUrl", params, headers=headers)
+            response = json.loads(body)
+            model = models.CancelUserAutoSignEnableUrlResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def CreateBatchCancelFlowUrl(self, request):
         """注：此接口将会废弃，请使用撤销单个签署流程（CancelFlow）接口。
         指定需要批量撤回的签署流程Id，获取批量撤销链接。
         客户指定需要撤回的签署流程Id，最多100个，超过100不处理；接口调用成功返回批量撤回合同的链接，通过链接跳转到电子签小程序完成批量撤回。
 
         :param request: Request instance for CreateBatchCancelFlowUrl.
         :type request: :class:`tencentcloud.ess.v20201111.models.CreateBatchCancelFlowUrlRequest`
@@ -142,15 +165,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateConvertTaskApi(self, request):
-        """上传了word、excel文件后，通过该接口发起文件转换任务，将word、excel文件转换为pdf文件。
+        """上传了word、excel、图片文件后，通过该接口发起文件转换任务，将word、excel、图片文件转换为pdf文件。
 
         :param request: Request instance for CreateConvertTaskApi.
         :type request: :class:`tencentcloud.ess.v20201111.models.CreateConvertTaskApiRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.CreateConvertTaskApiResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-ess-3.0.910/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.911/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,14 +67,20 @@
 
 # 请求的次数超过了频率限制，请联系客服处理。
 FAILEDOPERATION_REQUESTLIMITEXCEEDED = 'FailedOperation.RequestLimitExceeded'
 
 # 模板无资源信息。
 FAILEDOPERATION_TEMPLATEHASNORESOURCE = 'FailedOperation.TemplateHasNoResource'
 
+# 无法撤销，用户已开通自动签。
+FAILEDOPERATION_USERAUTOSIGNENABLEALREADY = 'FailedOperation.UserAutoSignEnableAlready'
+
+# 无法撤销，用户未生成开通链接。
+FAILEDOPERATION_USERAUTOSIGNENABLEURLNOTEXIST = 'FailedOperation.UserAutoSignEnableUrlNotExist'
+
 # 用户信息不匹配，请检查后重试。
 FAILEDOPERATION_USERINFONOMATCH = 'FailedOperation.UserInfoNoMatch'
 
 # 内部错误。
 INTERNALERROR = 'InternalError'
 
 # 第三方接口失败。
```

### Comparing `tencentcloud-sdk-python-ess-3.0.910/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.911/tencentcloud/ess/v20201111/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -557,14 +557,68 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class CancelUserAutoSignEnableUrlRequest(AbstractModel):
+    """CancelUserAutoSignEnableUrl请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Operator: 操作人信息，UseId必填	
+        :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
+        :param SceneKey: 自动签场景: E_PRESCRIPTION_AUTO_SIGN 电子处方
+        :type SceneKey: str
+        :param UserInfo: 指定撤销链接的用户指定撤销链接的用户信息，包含姓名、证件类型、证件号码。
+
+        :type UserInfo: :class:`tencentcloud.ess.v20201111.models.UserThreeFactor`
+        """
+        self.Operator = None
+        self.SceneKey = None
+        self.UserInfo = None
+
+
+    def _deserialize(self, params):
+        if params.get("Operator") is not None:
+            self.Operator = UserInfo()
+            self.Operator._deserialize(params.get("Operator"))
+        self.SceneKey = params.get("SceneKey")
+        if params.get("UserInfo") is not None:
+            self.UserInfo = UserThreeFactor()
+            self.UserInfo._deserialize(params.get("UserInfo"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CancelUserAutoSignEnableUrlResponse(AbstractModel):
+    """CancelUserAutoSignEnableUrl返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class CcInfo(AbstractModel):
     """抄送信息
 
     """
 
     def __init__(self):
         r"""
@@ -957,15 +1011,15 @@
 class CreateConvertTaskApiRequest(AbstractModel):
     """CreateConvertTaskApi请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param ResourceType: 资源类型 取值范围doc,docx,html,xls,xlsx之一
+        :param ResourceType: 资源类型 支持doc,docx,html,xls,xlsx,jpg,jpeg,png,bmp文件类型
         :type ResourceType: str
         :param ResourceName: 资源名称，长度限制为256字符
         :type ResourceName: str
         :param ResourceId: 资源Id，通过UploadFiles获取
         :type ResourceId: str
         :param Operator: 调用方用户信息，userId 必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
```

### Comparing `tencentcloud-sdk-python-ess-3.0.910/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.911/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.910
+Version: 3.0.911
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.910/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.911/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.910
+Version: 3.0.911
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.910/setup.py` & `tencentcloud-sdk-python-ess-3.0.911/setup.py`

 * *Files identical despite different names*

