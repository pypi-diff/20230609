# Comparing `tmp/tencentcloud-sdk-python-essbasic-3.0.910.tar.gz` & `tmp/tencentcloud-sdk-python-essbasic-3.0.911.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.910.tar", last modified: Thu Jun  8 09:11:08 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.911.tar", last modified: Fri Jun  9 02:19:17 2023, max compression
```

## Comparing `tencentcloud-sdk-python-essbasic-3.0.910.tar` & `tencentcloud-sdk-python-essbasic-3.0.911.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud_sdk_python_essbasic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      678 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      752 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud/essbasic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)    16533 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud/essbasic/v20210526/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    51520 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud/essbasic/v20210526/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)   234248 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud/essbasic/v20210526/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud/essbasic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)     5392 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    53845 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud/essbasic/v20201222/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)   171664 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1016 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud_sdk_python_essbasic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      678 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      752 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud/essbasic/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)    16533 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud/essbasic/v20210526/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    51697 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud/essbasic/v20210526/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   234715 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud/essbasic/v20210526/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud/essbasic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    53845 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud/essbasic/v20201222/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   171664 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-09 02:19:17.000000 tencentcloud-sdk-python-essbasic-3.0.911/setup.cfg
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.910
+Version: 3.0.911
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.910/README.rst` & `tencentcloud-sdk-python-essbasic-3.0.911/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud/__init__.py` & `tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -432,15 +432,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def ChannelCreateUserRoles(self, request):
-        """绑定员工角色
+        """通过此接口，绑定员工角色，支持以电子签userId、客户系统userId两种方式调用。
 
         :param request: Request instance for ChannelCreateUserRoles.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.ChannelCreateUserRolesRequest`
         :rtype: :class:`tencentcloud.essbasic.v20210526.models.ChannelCreateUserRolesResponse`
 
         """
         try:
@@ -455,15 +455,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def ChannelDeleteRoleUsers(self, request):
-        """删除员工绑定角色
+        """通过此接口，删除员工绑定的角色，支持以电子签userId、客户系统userId两种方式调用。
 
         :param request: Request instance for ChannelDeleteRoleUsers.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.ChannelDeleteRoleUsersRequest`
         :rtype: :class:`tencentcloud.essbasic.v20210526.models.ChannelDeleteRoleUsersResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud/essbasic/v20210526/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1508,33 +1508,37 @@
 
     """
 
     def __init__(self):
         r"""
         :param Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 和 Agent.ProxyAppId 必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
-        :param UserIds: 绑定角色的员工id列表，电子签的UserId
-        :type UserIds: list of str
         :param RoleIds: 绑定角色的角色id列表
         :type RoleIds: list of str
+        :param UserIds: 电子签用户ID列表，与OpenIds参数二选一,优先UserIds参数
+        :type UserIds: list of str
+        :param OpenIds: 客户系统用户ID列表，与UserIds参数二选一,优先UserIds参数
+        :type OpenIds: list of str
         :param Operator: 操作者信息
         :type Operator: :class:`tencentcloud.essbasic.v20210526.models.UserInfo`
         """
         self.Agent = None
-        self.UserIds = None
         self.RoleIds = None
+        self.UserIds = None
+        self.OpenIds = None
         self.Operator = None
 
 
     def _deserialize(self, params):
         if params.get("Agent") is not None:
             self.Agent = Agent()
             self.Agent._deserialize(params.get("Agent"))
-        self.UserIds = params.get("UserIds")
         self.RoleIds = params.get("RoleIds")
+        self.UserIds = params.get("UserIds")
+        self.OpenIds = params.get("OpenIds")
         if params.get("Operator") is not None:
             self.Operator = UserInfo()
             self.Operator._deserialize(params.get("Operator"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
@@ -1576,34 +1580,38 @@
 
     def __init__(self):
         r"""
         :param Agent: 代理信息
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param RoleId: 角色Id（非超管或法人角色Id）
         :type RoleId: str
-        :param UserIds: 用户列表，电子签系统的UserId
+        :param UserIds: 电子签用户ID列表，与OpenIds参数二选一,优先UserIds参数
         :type UserIds: list of str
         :param Operator: 操作人信息
         :type Operator: :class:`tencentcloud.essbasic.v20210526.models.UserInfo`
+        :param OpenIds: 客户系统用户ID列表，与UserIds参数二选一,优先UserIds参数
+        :type OpenIds: list of str
         """
         self.Agent = None
         self.RoleId = None
         self.UserIds = None
         self.Operator = None
+        self.OpenIds = None
 
 
     def _deserialize(self, params):
         if params.get("Agent") is not None:
             self.Agent = Agent()
             self.Agent._deserialize(params.get("Agent"))
         self.RoleId = params.get("RoleId")
         self.UserIds = params.get("UserIds")
         if params.get("Operator") is not None:
             self.Operator = UserInfo()
             self.Operator._deserialize(params.get("Operator"))
+        self.OpenIds = params.get("OpenIds")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-essbasic-3.0.911/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.910/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.911/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.910
+Version: 3.0.911
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.910/setup.py` & `tencentcloud-sdk-python-essbasic-3.0.911/setup.py`

 * *Files identical despite different names*

