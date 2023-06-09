# Comparing `tmp/tencentcloud-sdk-python-ckafka-3.0.910.tar.gz` & `tmp/tencentcloud-sdk-python-ckafka-3.0.911.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ckafka-3.0.910.tar", last modified: Thu Jun  8 09:06:26 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ckafka-3.0.911.tar", last modified: Fri Jun  9 02:15:29 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ckafka-3.0.910.tar` & `tencentcloud-sdk-python-ckafka-3.0.911.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:06:26.000000 tencentcloud-sdk-python-ckafka-3.0.910/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:06:26.000000 tencentcloud-sdk-python-ckafka-3.0.910/tencentcloud_sdk_python_ckafka.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 09:06:26.000000 tencentcloud-sdk-python-ckafka-3.0.910/tencentcloud_sdk_python_ckafka.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-06-08 09:06:26.000000 tencentcloud-sdk-python-ckafka-3.0.910/tencentcloud_sdk_python_ckafka.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-08 09:06:26.000000 tencentcloud-sdk-python-ckafka-3.0.910/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-08 09:06:26.000000 tencentcloud-sdk-python-ckafka-3.0.910/tencentcloud_sdk_python_ckafka.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      746 2023-06-08 09:06:26.000000 tencentcloud-sdk-python-ckafka-3.0.910/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:06:26.000000 tencentcloud-sdk-python-ckafka-3.0.910/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-08 09:06:26.000000 tencentcloud-sdk-python-ckafka-3.0.910/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:06:26.000000 tencentcloud-sdk-python-ckafka-3.0.910/tencentcloud/ckafka/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:06:26.000000 tencentcloud-sdk-python-ckafka-3.0.910/tencentcloud/ckafka/v20190819/
--rw-r--r--   0 root         (0) root         (0)     3315 2023-06-08 09:06:26.000000 tencentcloud-sdk-python-ckafka-3.0.910/tencentcloud/ckafka/v20190819/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 09:06:26.000000 tencentcloud-sdk-python-ckafka-3.0.910/tencentcloud/ckafka/v20190819/__init__.py
--rw-r--r--   0 root         (0) root         (0)   472962 2023-06-08 09:06:26.000000 tencentcloud-sdk-python-ckafka-3.0.910/tencentcloud/ckafka/v20190819/models.py
--rw-r--r--   0 root         (0) root         (0)    70499 2023-06-08 09:06:26.000000 tencentcloud-sdk-python-ckafka-3.0.910/tencentcloud/ckafka/v20190819/ckafka_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 09:06:26.000000 tencentcloud-sdk-python-ckafka-3.0.910/tencentcloud/ckafka/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-08 09:06:26.000000 tencentcloud-sdk-python-ckafka-3.0.910/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1012 2023-06-08 09:06:26.000000 tencentcloud-sdk-python-ckafka-3.0.910/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-08 09:06:26.000000 tencentcloud-sdk-python-ckafka-3.0.910/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:15:29.000000 tencentcloud-sdk-python-ckafka-3.0.911/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:15:29.000000 tencentcloud-sdk-python-ckafka-3.0.911/tencentcloud_sdk_python_ckafka.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 02:15:29.000000 tencentcloud-sdk-python-ckafka-3.0.911/tencentcloud_sdk_python_ckafka.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-06-09 02:15:29.000000 tencentcloud-sdk-python-ckafka-3.0.911/tencentcloud_sdk_python_ckafka.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-09 02:15:29.000000 tencentcloud-sdk-python-ckafka-3.0.911/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-09 02:15:29.000000 tencentcloud-sdk-python-ckafka-3.0.911/tencentcloud_sdk_python_ckafka.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      746 2023-06-09 02:15:29.000000 tencentcloud-sdk-python-ckafka-3.0.911/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:15:29.000000 tencentcloud-sdk-python-ckafka-3.0.911/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-09 02:15:29.000000 tencentcloud-sdk-python-ckafka-3.0.911/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:15:29.000000 tencentcloud-sdk-python-ckafka-3.0.911/tencentcloud/ckafka/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:15:29.000000 tencentcloud-sdk-python-ckafka-3.0.911/tencentcloud/ckafka/v20190819/
+-rw-r--r--   0 root         (0) root         (0)     3315 2023-06-09 02:15:29.000000 tencentcloud-sdk-python-ckafka-3.0.911/tencentcloud/ckafka/v20190819/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:15:29.000000 tencentcloud-sdk-python-ckafka-3.0.911/tencentcloud/ckafka/v20190819/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   475045 2023-06-09 02:15:29.000000 tencentcloud-sdk-python-ckafka-3.0.911/tencentcloud/ckafka/v20190819/models.py
+-rw-r--r--   0 root         (0) root         (0)    70499 2023-06-09 02:15:29.000000 tencentcloud-sdk-python-ckafka-3.0.911/tencentcloud/ckafka/v20190819/ckafka_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:15:29.000000 tencentcloud-sdk-python-ckafka-3.0.911/tencentcloud/ckafka/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-09 02:15:29.000000 tencentcloud-sdk-python-ckafka-3.0.911/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-06-09 02:15:29.000000 tencentcloud-sdk-python-ckafka-3.0.911/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-09 02:15:29.000000 tencentcloud-sdk-python-ckafka-3.0.911/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.910/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ckafka-3.0.911/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ckafka
-Version: 3.0.910
+Version: 3.0.911
 Summary: Tencent Cloud Ckafka SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.910/README.rst` & `tencentcloud-sdk-python-ckafka-3.0.911/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.910/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ckafka-3.0.911/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ckafka-3.0.910/tencentcloud/ckafka/v20190819/errorcodes.py` & `tencentcloud-sdk-python-ckafka-3.0.911/tencentcloud/ckafka/v20190819/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.910/tencentcloud/ckafka/v20190819/models.py` & `tencentcloud-sdk-python-ckafka-3.0.911/tencentcloud/ckafka/v20190819/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2333,27 +2333,37 @@
         r"""
         :param FlowId: CreateInstancePre返回固定为0，不能作为CheckTaskStatus的查询条件。只是为了保证和后台数据结构对齐。
 注意：此字段可能返回 null，表示取不到有效值。
         :type FlowId: int
         :param DealNames: 订单号列表
 注意：此字段可能返回 null，表示取不到有效值。
         :type DealNames: list of str
-        :param InstanceId: 实例Id
+        :param InstanceId: 实例Id，当购买多个实例时，默认返回购买的第一个实例 id
 注意：此字段可能返回 null，表示取不到有效值。
         :type InstanceId: str
+        :param DealNameInstanceIdMapping: 订单和购买实例对应映射列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DealNameInstanceIdMapping: list of DealInstanceDTO
         """
         self.FlowId = None
         self.DealNames = None
         self.InstanceId = None
+        self.DealNameInstanceIdMapping = None
 
 
     def _deserialize(self, params):
         self.FlowId = params.get("FlowId")
         self.DealNames = params.get("DealNames")
         self.InstanceId = params.get("InstanceId")
+        if params.get("DealNameInstanceIdMapping") is not None:
+            self.DealNameInstanceIdMapping = []
+            for item in params.get("DealNameInstanceIdMapping"):
+                obj = DealInstanceDTO()
+                obj._deserialize(item)
+                self.DealNameInstanceIdMapping.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -2399,14 +2409,16 @@
         :type Tags: list of Tag
         :param DiskType: 磁盘类型（ssd填写CLOUD_SSD，sata填写CLOUD_BASIC）
         :type DiskType: str
         :param MultiZoneFlag: 跨可用区，zoneIds必填
         :type MultiZoneFlag: bool
         :param ZoneIds: 可用区列表，购买多可用区实例时为必填项
         :type ZoneIds: list of int
+        :param PublicNetworkMonthly: 公网带宽大小，单位 Mbps。默认是没有加上免费 3Mbps 带宽。例如总共需要 3Mbps 公网带宽，此处传 0；总共需要 4Mbps 公网带宽，此处传 1。默认值为 0
+        :type PublicNetworkMonthly: int
         """
         self.InstanceName = None
         self.ZoneId = None
         self.Period = None
         self.InstanceType = None
         self.VpcId = None
         self.SubnetId = None
@@ -2418,14 +2430,15 @@
         self.DiskSize = None
         self.BandWidth = None
         self.Partition = None
         self.Tags = None
         self.DiskType = None
         self.MultiZoneFlag = None
         self.ZoneIds = None
+        self.PublicNetworkMonthly = None
 
 
     def _deserialize(self, params):
         self.InstanceName = params.get("InstanceName")
         self.ZoneId = params.get("ZoneId")
         self.Period = params.get("Period")
         self.InstanceType = params.get("InstanceType")
@@ -2444,38 +2457,39 @@
             for item in params.get("Tags"):
                 obj = Tag()
                 obj._deserialize(item)
                 self.Tags.append(obj)
         self.DiskType = params.get("DiskType")
         self.MultiZoneFlag = params.get("MultiZoneFlag")
         self.ZoneIds = params.get("ZoneIds")
+        self.PublicNetworkMonthly = params.get("PublicNetworkMonthly")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class CreateInstancePreResp(AbstractModel):
-    """创建预付费实例返回结构
+    """预付费实例相关接口返回结构
 
     """
 
     def __init__(self):
         r"""
         :param ReturnCode: 返回的code，0为正常，非0为错误
         :type ReturnCode: str
         :param ReturnMessage: 成功消息
         :type ReturnMessage: str
         :param Data: 操作型返回的Data数据
 注意：此字段可能返回 null，表示取不到有效值。
         :type Data: :class:`tencentcloud.ckafka.v20190819.models.CreateInstancePreData`
-        :param DeleteRouteTimestamp: 删除是时间
+        :param DeleteRouteTimestamp: 删除时间。目前该参数字段已废弃，将会在未来被删除
 注意：此字段可能返回 null，表示取不到有效值。
         :type DeleteRouteTimestamp: str
         """
         self.ReturnCode = None
         self.ReturnMessage = None
         self.Data = None
         self.DeleteRouteTimestamp = None
@@ -3428,14 +3442,44 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
+
+
+class DealInstanceDTO(AbstractModel):
+    """预付费/后付费接口中，订单和 CKafka 实例映射数据结构
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DealName: 订单流水
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DealName: str
+        :param InstanceIdList: 订单流水对应购买的 CKafka 实例 id 列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InstanceIdList: list of str
+        """
+        self.DealName = None
+        self.InstanceIdList = None
+
+
+    def _deserialize(self, params):
+        self.DealName = params.get("DealName")
+        self.InstanceIdList = params.get("InstanceIdList")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class DeleteAclRequest(AbstractModel):
     """DeleteAcl请求参数结构体
 
     """
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.910/tencentcloud/ckafka/v20190819/ckafka_client.py` & `tencentcloud-sdk-python-ckafka-3.0.911/tencentcloud/ckafka/v20190819/ckafka_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.910/PKG-INFO` & `tencentcloud-sdk-python-ckafka-3.0.911/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ckafka
-Version: 3.0.910
+Version: 3.0.911
 Summary: Tencent Cloud Ckafka SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.910/setup.py` & `tencentcloud-sdk-python-ckafka-3.0.911/setup.py`

 * *Files identical despite different names*

