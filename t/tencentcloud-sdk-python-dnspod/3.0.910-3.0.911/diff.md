# Comparing `tmp/tencentcloud-sdk-python-dnspod-3.0.910.tar.gz` & `tmp/tencentcloud-sdk-python-dnspod-3.0.911.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dnspod-3.0.910.tar", last modified: Thu Jun  8 09:09:07 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dnspod-3.0.911.tar", last modified: Fri Jun  9 02:17:57 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dnspod-3.0.910.tar` & `tencentcloud-sdk-python-dnspod-3.0.911.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:09:07.000000 tencentcloud-sdk-python-dnspod-3.0.910/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:09:07.000000 tencentcloud-sdk-python-dnspod-3.0.910/tencentcloud_sdk_python_dnspod.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 09:09:07.000000 tencentcloud-sdk-python-dnspod-3.0.910/tencentcloud_sdk_python_dnspod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-06-08 09:09:07.000000 tencentcloud-sdk-python-dnspod-3.0.910/tencentcloud_sdk_python_dnspod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-08 09:09:07.000000 tencentcloud-sdk-python-dnspod-3.0.910/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-08 09:09:07.000000 tencentcloud-sdk-python-dnspod-3.0.910/tencentcloud_sdk_python_dnspod.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      746 2023-06-08 09:09:07.000000 tencentcloud-sdk-python-dnspod-3.0.910/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:09:07.000000 tencentcloud-sdk-python-dnspod-3.0.910/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:09:07.000000 tencentcloud-sdk-python-dnspod-3.0.910/tencentcloud/dnspod/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:09:07.000000 tencentcloud-sdk-python-dnspod-3.0.910/tencentcloud/dnspod/v20210323/
--rw-r--r--   0 root         (0) root         (0)    23568 2023-06-08 09:09:07.000000 tencentcloud-sdk-python-dnspod-3.0.910/tencentcloud/dnspod/v20210323/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 09:09:07.000000 tencentcloud-sdk-python-dnspod-3.0.910/tencentcloud/dnspod/v20210323/__init__.py
--rw-r--r--   0 root         (0) root         (0)   207929 2023-06-08 09:09:07.000000 tencentcloud-sdk-python-dnspod-3.0.910/tencentcloud/dnspod/v20210323/models.py
--rw-r--r--   0 root         (0) root         (0)    59836 2023-06-08 09:09:07.000000 tencentcloud-sdk-python-dnspod-3.0.910/tencentcloud/dnspod/v20210323/dnspod_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 09:09:07.000000 tencentcloud-sdk-python-dnspod-3.0.910/tencentcloud/dnspod/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-08 09:09:07.000000 tencentcloud-sdk-python-dnspod-3.0.910/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-08 09:09:07.000000 tencentcloud-sdk-python-dnspod-3.0.910/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1012 2023-06-08 09:09:07.000000 tencentcloud-sdk-python-dnspod-3.0.910/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-08 09:09:07.000000 tencentcloud-sdk-python-dnspod-3.0.910/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:17:57.000000 tencentcloud-sdk-python-dnspod-3.0.911/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:17:57.000000 tencentcloud-sdk-python-dnspod-3.0.911/tencentcloud_sdk_python_dnspod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 02:17:57.000000 tencentcloud-sdk-python-dnspod-3.0.911/tencentcloud_sdk_python_dnspod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-06-09 02:17:57.000000 tencentcloud-sdk-python-dnspod-3.0.911/tencentcloud_sdk_python_dnspod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-09 02:17:57.000000 tencentcloud-sdk-python-dnspod-3.0.911/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-09 02:17:57.000000 tencentcloud-sdk-python-dnspod-3.0.911/tencentcloud_sdk_python_dnspod.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      746 2023-06-09 02:17:57.000000 tencentcloud-sdk-python-dnspod-3.0.911/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:17:57.000000 tencentcloud-sdk-python-dnspod-3.0.911/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:17:57.000000 tencentcloud-sdk-python-dnspod-3.0.911/tencentcloud/dnspod/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:17:57.000000 tencentcloud-sdk-python-dnspod-3.0.911/tencentcloud/dnspod/v20210323/
+-rw-r--r--   0 root         (0) root         (0)    23568 2023-06-09 02:17:57.000000 tencentcloud-sdk-python-dnspod-3.0.911/tencentcloud/dnspod/v20210323/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:17:57.000000 tencentcloud-sdk-python-dnspod-3.0.911/tencentcloud/dnspod/v20210323/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   209672 2023-06-09 02:17:57.000000 tencentcloud-sdk-python-dnspod-3.0.911/tencentcloud/dnspod/v20210323/models.py
+-rw-r--r--   0 root         (0) root         (0)    59836 2023-06-09 02:17:57.000000 tencentcloud-sdk-python-dnspod-3.0.911/tencentcloud/dnspod/v20210323/dnspod_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:17:57.000000 tencentcloud-sdk-python-dnspod-3.0.911/tencentcloud/dnspod/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-09 02:17:57.000000 tencentcloud-sdk-python-dnspod-3.0.911/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-09 02:17:57.000000 tencentcloud-sdk-python-dnspod-3.0.911/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-06-09 02:17:57.000000 tencentcloud-sdk-python-dnspod-3.0.911/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-09 02:17:57.000000 tencentcloud-sdk-python-dnspod-3.0.911/setup.cfg
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.910/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dnspod-3.0.911/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dnspod
-Version: 3.0.910
+Version: 3.0.911
 Summary: Tencent Cloud Dnspod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.910/README.rst` & `tencentcloud-sdk-python-dnspod-3.0.911/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dnspod-3.0.910/tencentcloud/dnspod/v20210323/errorcodes.py` & `tencentcloud-sdk-python-dnspod-3.0.911/tencentcloud/dnspod/v20210323/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dnspod-3.0.910/tencentcloud/dnspod/v20210323/models.py` & `tencentcloud-sdk-python-dnspod-3.0.911/tencentcloud/dnspod/v20210323/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -3622,14 +3622,35 @@
 注意：此字段可能返回 null，表示取不到有效值。
         :type ActualNsList: list of str
         :param RecordCount: 域名的记录数量
         :type RecordCount: int
         :param OwnerNick: 域名所有者的账户昵称
 注意：此字段可能返回 null，表示取不到有效值。
         :type OwnerNick: str
+        :param IsGracePeriod: 是否在付费套餐宽限期
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IsGracePeriod: str
+        :param VipBuffered: 是否在付费套餐缓冲期
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VipBuffered: str
+        :param VipStartAt: VIP套餐有效期开始时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VipStartAt: str
+        :param VipEndAt: VIP套餐有效期结束时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VipEndAt: str
+        :param VipAutoRenew: VIP套餐自动续费标识。可能的值为：default-默认；no-不自动续费；yes-自动续费
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VipAutoRenew: str
+        :param VipResourceId: VIP套餐资源ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VipResourceId: str
+        :param IsSubDomain: 是否是子域名。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IsSubDomain: bool
         """
         self.DomainId = None
         self.Status = None
         self.Grade = None
         self.GroupId = None
         self.IsMark = None
         self.TTL = None
@@ -3646,14 +3667,21 @@
         self.GradeTitle = None
         self.CreatedOn = None
         self.UpdatedOn = None
         self.Uin = None
         self.ActualNsList = None
         self.RecordCount = None
         self.OwnerNick = None
+        self.IsGracePeriod = None
+        self.VipBuffered = None
+        self.VipStartAt = None
+        self.VipEndAt = None
+        self.VipAutoRenew = None
+        self.VipResourceId = None
+        self.IsSubDomain = None
 
 
     def _deserialize(self, params):
         self.DomainId = params.get("DomainId")
         self.Status = params.get("Status")
         self.Grade = params.get("Grade")
         self.GroupId = params.get("GroupId")
@@ -3672,14 +3700,21 @@
         self.GradeTitle = params.get("GradeTitle")
         self.CreatedOn = params.get("CreatedOn")
         self.UpdatedOn = params.get("UpdatedOn")
         self.Uin = params.get("Uin")
         self.ActualNsList = params.get("ActualNsList")
         self.RecordCount = params.get("RecordCount")
         self.OwnerNick = params.get("OwnerNick")
+        self.IsGracePeriod = params.get("IsGracePeriod")
+        self.VipBuffered = params.get("VipBuffered")
+        self.VipStartAt = params.get("VipStartAt")
+        self.VipEndAt = params.get("VipEndAt")
+        self.VipAutoRenew = params.get("VipAutoRenew")
+        self.VipResourceId = params.get("VipResourceId")
+        self.IsSubDomain = params.get("IsSubDomain")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.910/tencentcloud/dnspod/v20210323/dnspod_client.py` & `tencentcloud-sdk-python-dnspod-3.0.911/tencentcloud/dnspod/v20210323/dnspod_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dnspod-3.0.910/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dnspod-3.0.911/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dnspod-3.0.910/PKG-INFO` & `tencentcloud-sdk-python-dnspod-3.0.911/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dnspod
-Version: 3.0.910
+Version: 3.0.911
 Summary: Tencent Cloud Dnspod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.910/setup.py` & `tencentcloud-sdk-python-dnspod-3.0.911/setup.py`

 * *Files identical despite different names*

