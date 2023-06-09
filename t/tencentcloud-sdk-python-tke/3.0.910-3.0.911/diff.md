# Comparing `tmp/tencentcloud-sdk-python-tke-3.0.910.tar.gz` & `tmp/tencentcloud-sdk-python-tke-3.0.911.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tke-3.0.910.tar", last modified: Thu Jun  8 09:23:13 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tke-3.0.911.tar", last modified: Fri Jun  9 02:29:49 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tke-3.0.910.tar` & `tencentcloud-sdk-python-tke-3.0.911.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:23:13.000000 tencentcloud-sdk-python-tke-3.0.910/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-08 09:23:13.000000 tencentcloud-sdk-python-tke-3.0.910/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:23:13.000000 tencentcloud-sdk-python-tke-3.0.910/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:23:13.000000 tencentcloud-sdk-python-tke-3.0.910/tencentcloud/tke/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 09:23:13.000000 tencentcloud-sdk-python-tke-3.0.910/tencentcloud/tke/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:23:13.000000 tencentcloud-sdk-python-tke-3.0.910/tencentcloud/tke/v20180525/
--rw-r--r--   0 root         (0) root         (0)   183327 2023-06-08 09:23:13.000000 tencentcloud-sdk-python-tke-3.0.910/tencentcloud/tke/v20180525/tke_client.py
--rw-r--r--   0 root         (0) root         (0)    19455 2023-06-08 09:23:13.000000 tencentcloud-sdk-python-tke-3.0.910/tencentcloud/tke/v20180525/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 09:23:13.000000 tencentcloud-sdk-python-tke-3.0.910/tencentcloud/tke/v20180525/__init__.py
--rw-r--r--   0 root         (0) root         (0)   671889 2023-06-08 09:23:13.000000 tencentcloud-sdk-python-tke-3.0.910/tencentcloud/tke/v20180525/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-08 09:23:13.000000 tencentcloud-sdk-python-tke-3.0.910/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-08 09:23:13.000000 tencentcloud-sdk-python-tke-3.0.910/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:23:13.000000 tencentcloud-sdk-python-tke-3.0.910/tencentcloud_sdk_python_tke.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 09:23:13.000000 tencentcloud-sdk-python-tke-3.0.910/tencentcloud_sdk_python_tke.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-08 09:23:13.000000 tencentcloud-sdk-python-tke-3.0.910/tencentcloud_sdk_python_tke.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-08 09:23:13.000000 tencentcloud-sdk-python-tke-3.0.910/tencentcloud_sdk_python_tke.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-08 09:23:13.000000 tencentcloud-sdk-python-tke-3.0.910/tencentcloud_sdk_python_tke.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-08 09:23:13.000000 tencentcloud-sdk-python-tke-3.0.910/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-08 09:23:13.000000 tencentcloud-sdk-python-tke-3.0.910/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:29:49.000000 tencentcloud-sdk-python-tke-3.0.911/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-09 02:29:49.000000 tencentcloud-sdk-python-tke-3.0.911/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:29:49.000000 tencentcloud-sdk-python-tke-3.0.911/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:29:49.000000 tencentcloud-sdk-python-tke-3.0.911/tencentcloud/tke/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:29:49.000000 tencentcloud-sdk-python-tke-3.0.911/tencentcloud/tke/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:29:49.000000 tencentcloud-sdk-python-tke-3.0.911/tencentcloud/tke/v20180525/
+-rw-r--r--   0 root         (0) root         (0)   183327 2023-06-09 02:29:49.000000 tencentcloud-sdk-python-tke-3.0.911/tencentcloud/tke/v20180525/tke_client.py
+-rw-r--r--   0 root         (0) root         (0)    19455 2023-06-09 02:29:49.000000 tencentcloud-sdk-python-tke-3.0.911/tencentcloud/tke/v20180525/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:29:49.000000 tencentcloud-sdk-python-tke-3.0.911/tencentcloud/tke/v20180525/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   672036 2023-06-09 02:29:49.000000 tencentcloud-sdk-python-tke-3.0.911/tencentcloud/tke/v20180525/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-09 02:29:49.000000 tencentcloud-sdk-python-tke-3.0.911/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-09 02:29:49.000000 tencentcloud-sdk-python-tke-3.0.911/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:29:49.000000 tencentcloud-sdk-python-tke-3.0.911/tencentcloud_sdk_python_tke.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 02:29:49.000000 tencentcloud-sdk-python-tke-3.0.911/tencentcloud_sdk_python_tke.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-09 02:29:49.000000 tencentcloud-sdk-python-tke-3.0.911/tencentcloud_sdk_python_tke.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-09 02:29:49.000000 tencentcloud-sdk-python-tke-3.0.911/tencentcloud_sdk_python_tke.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-09 02:29:49.000000 tencentcloud-sdk-python-tke-3.0.911/tencentcloud_sdk_python_tke.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-09 02:29:49.000000 tencentcloud-sdk-python-tke-3.0.911/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-09 02:29:49.000000 tencentcloud-sdk-python-tke-3.0.911/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tke-3.0.910/README.rst` & `tencentcloud-sdk-python-tke-3.0.911/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.910/tencentcloud/tke/v20180525/tke_client.py` & `tencentcloud-sdk-python-tke-3.0.911/tencentcloud/tke/v20180525/tke_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.910/tencentcloud/tke/v20180525/errorcodes.py` & `tencentcloud-sdk-python-tke-3.0.911/tencentcloud/tke/v20180525/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.910/tencentcloud/tke/v20180525/models.py` & `tencentcloud-sdk-python-tke-3.0.911/tencentcloud/tke/v20180525/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1563,38 +1563,42 @@
         :type Message: str
         :param OldLevel: 变配前规模
         :type OldLevel: str
         :param NewLevel: 变配后规模
         :type NewLevel: str
         :param TriggerType: 变配触发类型：manual 手动,auto 自动
         :type TriggerType: str
+        :param CreatedAt: 创建时间
+        :type CreatedAt: str
         :param StartedAt: 开始时间
         :type StartedAt: str
         :param EndedAt: 结束时间
         :type EndedAt: str
         """
         self.ID = None
         self.ClusterID = None
         self.Status = None
         self.Message = None
         self.OldLevel = None
         self.NewLevel = None
         self.TriggerType = None
+        self.CreatedAt = None
         self.StartedAt = None
         self.EndedAt = None
 
 
     def _deserialize(self, params):
         self.ID = params.get("ID")
         self.ClusterID = params.get("ClusterID")
         self.Status = params.get("Status")
         self.Message = params.get("Message")
         self.OldLevel = params.get("OldLevel")
         self.NewLevel = params.get("NewLevel")
         self.TriggerType = params.get("TriggerType")
+        self.CreatedAt = params.get("CreatedAt")
         self.StartedAt = params.get("StartedAt")
         self.EndedAt = params.get("EndedAt")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
```

### Comparing `tencentcloud-sdk-python-tke-3.0.910/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tke-3.0.911/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tke-3.0.910/PKG-INFO` & `tencentcloud-sdk-python-tke-3.0.911/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tke
-Version: 3.0.910
+Version: 3.0.911
 Summary: Tencent Cloud Tke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tke-3.0.910/tencentcloud_sdk_python_tke.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tke-3.0.911/tencentcloud_sdk_python_tke.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tke
-Version: 3.0.910
+Version: 3.0.911
 Summary: Tencent Cloud Tke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tke-3.0.910/setup.py` & `tencentcloud-sdk-python-tke-3.0.911/setup.py`

 * *Files identical despite different names*

