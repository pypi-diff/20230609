# Comparing `tmp/tencentcloud-sdk-python-cdn-3.0.910.tar.gz` & `tmp/tencentcloud-sdk-python-cdn-3.0.911.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cdn-3.0.910.tar", last modified: Thu Jun  8 09:05:07 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cdn-3.0.911.tar", last modified: Fri Jun  9 02:14:18 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cdn-3.0.910.tar` & `tencentcloud-sdk-python-cdn-3.0.911.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:05:07.000000 tencentcloud-sdk-python-cdn-3.0.910/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-08 09:05:07.000000 tencentcloud-sdk-python-cdn-3.0.910/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:05:07.000000 tencentcloud-sdk-python-cdn-3.0.910/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-08 09:05:07.000000 tencentcloud-sdk-python-cdn-3.0.910/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:05:07.000000 tencentcloud-sdk-python-cdn-3.0.910/tencentcloud/cdn/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 09:05:07.000000 tencentcloud-sdk-python-cdn-3.0.910/tencentcloud/cdn/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:05:07.000000 tencentcloud-sdk-python-cdn-3.0.910/tencentcloud/cdn/v20180606/
--rw-r--r--   0 root         (0) root         (0)    21972 2023-06-08 09:05:07.000000 tencentcloud-sdk-python-cdn-3.0.910/tencentcloud/cdn/v20180606/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    80657 2023-06-08 09:05:07.000000 tencentcloud-sdk-python-cdn-3.0.910/tencentcloud/cdn/v20180606/cdn_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 09:05:07.000000 tencentcloud-sdk-python-cdn-3.0.910/tencentcloud/cdn/v20180606/__init__.py
--rw-r--r--   0 root         (0) root         (0)   573199 2023-06-08 09:05:07.000000 tencentcloud-sdk-python-cdn-3.0.910/tencentcloud/cdn/v20180606/models.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-08 09:05:07.000000 tencentcloud-sdk-python-cdn-3.0.910/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:05:07.000000 tencentcloud-sdk-python-cdn-3.0.910/tencentcloud_sdk_python_cdn.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 09:05:07.000000 tencentcloud-sdk-python-cdn-3.0.910/tencentcloud_sdk_python_cdn.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-08 09:05:07.000000 tencentcloud-sdk-python-cdn-3.0.910/tencentcloud_sdk_python_cdn.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-08 09:05:07.000000 tencentcloud-sdk-python-cdn-3.0.910/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-08 09:05:07.000000 tencentcloud-sdk-python-cdn-3.0.910/tencentcloud_sdk_python_cdn.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-08 09:05:07.000000 tencentcloud-sdk-python-cdn-3.0.910/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-08 09:05:07.000000 tencentcloud-sdk-python-cdn-3.0.910/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:14:18.000000 tencentcloud-sdk-python-cdn-3.0.911/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-09 02:14:18.000000 tencentcloud-sdk-python-cdn-3.0.911/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:14:18.000000 tencentcloud-sdk-python-cdn-3.0.911/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-09 02:14:18.000000 tencentcloud-sdk-python-cdn-3.0.911/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:14:18.000000 tencentcloud-sdk-python-cdn-3.0.911/tencentcloud/cdn/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:14:18.000000 tencentcloud-sdk-python-cdn-3.0.911/tencentcloud/cdn/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:14:18.000000 tencentcloud-sdk-python-cdn-3.0.911/tencentcloud/cdn/v20180606/
+-rw-r--r--   0 root         (0) root         (0)    21972 2023-06-09 02:14:18.000000 tencentcloud-sdk-python-cdn-3.0.911/tencentcloud/cdn/v20180606/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    80657 2023-06-09 02:14:18.000000 tencentcloud-sdk-python-cdn-3.0.911/tencentcloud/cdn/v20180606/cdn_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:14:18.000000 tencentcloud-sdk-python-cdn-3.0.911/tencentcloud/cdn/v20180606/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   573526 2023-06-09 02:14:18.000000 tencentcloud-sdk-python-cdn-3.0.911/tencentcloud/cdn/v20180606/models.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-09 02:14:18.000000 tencentcloud-sdk-python-cdn-3.0.911/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:14:18.000000 tencentcloud-sdk-python-cdn-3.0.911/tencentcloud_sdk_python_cdn.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 02:14:18.000000 tencentcloud-sdk-python-cdn-3.0.911/tencentcloud_sdk_python_cdn.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-09 02:14:18.000000 tencentcloud-sdk-python-cdn-3.0.911/tencentcloud_sdk_python_cdn.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-09 02:14:18.000000 tencentcloud-sdk-python-cdn-3.0.911/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-09 02:14:18.000000 tencentcloud-sdk-python-cdn-3.0.911/tencentcloud_sdk_python_cdn.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-09 02:14:18.000000 tencentcloud-sdk-python-cdn-3.0.911/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-09 02:14:18.000000 tencentcloud-sdk-python-cdn-3.0.911/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.910/README.rst` & `tencentcloud-sdk-python-cdn-3.0.911/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.910/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cdn-3.0.911/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cdn-3.0.910/tencentcloud/cdn/v20180606/errorcodes.py` & `tencentcloud-sdk-python-cdn-3.0.911/tencentcloud/cdn/v20180606/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.910/tencentcloud/cdn/v20180606/cdn_client.py` & `tencentcloud-sdk-python-cdn-3.0.911/tencentcloud/cdn/v20180606/cdn_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.910/tencentcloud/cdn/v20180606/models.py` & `tencentcloud-sdk-python-cdn-3.0.911/tencentcloud/cdn/v20180606/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1388,36 +1388,44 @@
     def __init__(self):
         r"""
         :param Switch: 防盗链配置开关，取值有：
 on：开启
 off：关闭
 开启时必须且只配置一种模式，其余模式需要设置为 null
         :type Switch: str
+        :param AuthAlgorithm: 鉴权算法，取值有：
+md5：按MD5算法取hash值
+sha256：按SHA-256算法取hash值
+默认为 md5
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AuthAlgorithm: str
         :param TypeA: 时间戳防盗链模式 A 配置
 注意：此字段可能返回 null，表示取不到有效值。
         :type TypeA: :class:`tencentcloud.cdn.v20180606.models.AuthenticationTypeA`
         :param TypeB: 时间戳防盗链模式 B 配置（模式 B 后台升级中，暂时不支持配置）
 注意：此字段可能返回 null，表示取不到有效值。
         :type TypeB: :class:`tencentcloud.cdn.v20180606.models.AuthenticationTypeB`
         :param TypeC: 时间戳防盗链模式 C 配置
 注意：此字段可能返回 null，表示取不到有效值。
         :type TypeC: :class:`tencentcloud.cdn.v20180606.models.AuthenticationTypeC`
         :param TypeD: 时间戳防盗链模式 D 配置
 注意：此字段可能返回 null，表示取不到有效值。
         :type TypeD: :class:`tencentcloud.cdn.v20180606.models.AuthenticationTypeD`
         """
         self.Switch = None
+        self.AuthAlgorithm = None
         self.TypeA = None
         self.TypeB = None
         self.TypeC = None
         self.TypeD = None
 
 
     def _deserialize(self, params):
         self.Switch = params.get("Switch")
+        self.AuthAlgorithm = params.get("AuthAlgorithm")
         if params.get("TypeA") is not None:
             self.TypeA = AuthenticationTypeA()
             self.TypeA._deserialize(params.get("TypeA"))
         if params.get("TypeB") is not None:
             self.TypeB = AuthenticationTypeB()
             self.TypeB._deserialize(params.get("TypeB"))
         if params.get("TypeC") is not None:
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.910/PKG-INFO` & `tencentcloud-sdk-python-cdn-3.0.911/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdn
-Version: 3.0.910
+Version: 3.0.911
 Summary: Tencent Cloud Cdn SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.910/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cdn-3.0.911/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdn
-Version: 3.0.910
+Version: 3.0.911
 Summary: Tencent Cloud Cdn SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.910/setup.py` & `tencentcloud-sdk-python-cdn-3.0.911/setup.py`

 * *Files identical despite different names*

