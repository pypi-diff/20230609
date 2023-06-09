# Comparing `tmp/tencentcloud-sdk-python-cdwch-3.0.910.tar.gz` & `tmp/tencentcloud-sdk-python-cdwch-3.0.911.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cdwch-3.0.910.tar", last modified: Thu Jun  8 09:05:27 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cdwch-3.0.911.tar", last modified: Fri Jun  9 02:14:36 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cdwch-3.0.910.tar` & `tencentcloud-sdk-python-cdwch-3.0.911.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:05:27.000000 tencentcloud-sdk-python-cdwch-3.0.910/
--rw-r--r--   0 root         (0) root         (0)      743 2023-06-08 09:05:26.000000 tencentcloud-sdk-python-cdwch-3.0.910/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:05:27.000000 tencentcloud-sdk-python-cdwch-3.0.910/tencentcloud_sdk_python_cdwch.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 09:05:27.000000 tencentcloud-sdk-python-cdwch-3.0.910/tencentcloud_sdk_python_cdwch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-06-08 09:05:27.000000 tencentcloud-sdk-python-cdwch-3.0.910/tencentcloud_sdk_python_cdwch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-06-08 09:05:27.000000 tencentcloud-sdk-python-cdwch-3.0.910/tencentcloud_sdk_python_cdwch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-08 09:05:27.000000 tencentcloud-sdk-python-cdwch-3.0.910/tencentcloud_sdk_python_cdwch.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:05:27.000000 tencentcloud-sdk-python-cdwch-3.0.910/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:05:27.000000 tencentcloud-sdk-python-cdwch-3.0.910/tencentcloud/cdwch/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:05:27.000000 tencentcloud-sdk-python-cdwch-3.0.910/tencentcloud/cdwch/v20200915/
--rw-r--r--   0 root         (0) root         (0)      703 2023-06-08 09:05:26.000000 tencentcloud-sdk-python-cdwch-3.0.910/tencentcloud/cdwch/v20200915/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 09:05:26.000000 tencentcloud-sdk-python-cdwch-3.0.910/tencentcloud/cdwch/v20200915/__init__.py
--rw-r--r--   0 root         (0) root         (0)    79067 2023-06-08 09:05:26.000000 tencentcloud-sdk-python-cdwch-3.0.910/tencentcloud/cdwch/v20200915/models.py
--rw-r--r--   0 root         (0) root         (0)    19118 2023-06-08 09:05:26.000000 tencentcloud-sdk-python-cdwch-3.0.910/tencentcloud/cdwch/v20200915/cdwch_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 09:05:26.000000 tencentcloud-sdk-python-cdwch-3.0.910/tencentcloud/cdwch/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-08 09:05:26.000000 tencentcloud-sdk-python-cdwch-3.0.910/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-06-08 09:05:27.000000 tencentcloud-sdk-python-cdwch-3.0.910/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1010 2023-06-08 09:05:26.000000 tencentcloud-sdk-python-cdwch-3.0.910/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-08 09:05:27.000000 tencentcloud-sdk-python-cdwch-3.0.910/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:14:36.000000 tencentcloud-sdk-python-cdwch-3.0.911/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-06-09 02:14:35.000000 tencentcloud-sdk-python-cdwch-3.0.911/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:14:36.000000 tencentcloud-sdk-python-cdwch-3.0.911/tencentcloud_sdk_python_cdwch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 02:14:36.000000 tencentcloud-sdk-python-cdwch-3.0.911/tencentcloud_sdk_python_cdwch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-06-09 02:14:36.000000 tencentcloud-sdk-python-cdwch-3.0.911/tencentcloud_sdk_python_cdwch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-06-09 02:14:36.000000 tencentcloud-sdk-python-cdwch-3.0.911/tencentcloud_sdk_python_cdwch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-09 02:14:36.000000 tencentcloud-sdk-python-cdwch-3.0.911/tencentcloud_sdk_python_cdwch.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:14:36.000000 tencentcloud-sdk-python-cdwch-3.0.911/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:14:36.000000 tencentcloud-sdk-python-cdwch-3.0.911/tencentcloud/cdwch/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:14:36.000000 tencentcloud-sdk-python-cdwch-3.0.911/tencentcloud/cdwch/v20200915/
+-rw-r--r--   0 root         (0) root         (0)      703 2023-06-09 02:14:35.000000 tencentcloud-sdk-python-cdwch-3.0.911/tencentcloud/cdwch/v20200915/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:14:35.000000 tencentcloud-sdk-python-cdwch-3.0.911/tencentcloud/cdwch/v20200915/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    82547 2023-06-09 02:14:35.000000 tencentcloud-sdk-python-cdwch-3.0.911/tencentcloud/cdwch/v20200915/models.py
+-rw-r--r--   0 root         (0) root         (0)    20026 2023-06-09 02:14:35.000000 tencentcloud-sdk-python-cdwch-3.0.911/tencentcloud/cdwch/v20200915/cdwch_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:14:35.000000 tencentcloud-sdk-python-cdwch-3.0.911/tencentcloud/cdwch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-09 02:14:35.000000 tencentcloud-sdk-python-cdwch-3.0.911/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-06-09 02:14:36.000000 tencentcloud-sdk-python-cdwch-3.0.911/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-06-09 02:14:35.000000 tencentcloud-sdk-python-cdwch-3.0.911/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-09 02:14:36.000000 tencentcloud-sdk-python-cdwch-3.0.911/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cdwch-3.0.910/README.rst` & `tencentcloud-sdk-python-cdwch-3.0.911/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdwch-3.0.910/tencentcloud_sdk_python_cdwch.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cdwch-3.0.911/tencentcloud_sdk_python_cdwch.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdwch
-Version: 3.0.910
+Version: 3.0.911
 Summary: Tencent Cloud Cdwch SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdwch-3.0.910/tencentcloud/cdwch/v20200915/errorcodes.py` & `tencentcloud-sdk-python-cdwch-3.0.911/tencentcloud/cdwch/v20200915/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdwch-3.0.910/tencentcloud/cdwch/v20200915/models.py` & `tencentcloud-sdk-python-cdwch-3.0.911/tencentcloud/cdwch/v20200915/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -984,14 +984,89 @@
         self.FlowName = params.get("FlowName")
         self.FlowProgress = params.get("FlowProgress")
         self.InstanceStateDesc = params.get("InstanceStateDesc")
         self.FlowMsg = params.get("FlowMsg")
         self.RequestId = params.get("RequestId")
 
 
+class DescribeInstancesNewRequest(AbstractModel):
+    """DescribeInstancesNew请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param SearchInstanceId: 搜索的集群id名称
+        :type SearchInstanceId: str
+        :param SearchInstanceName: 搜索的集群name
+        :type SearchInstanceName: str
+        :param Offset: 分页参数，第一页为0，第二页为10
+        :type Offset: int
+        :param Limit: 分页参数，分页步长，默认为10
+        :type Limit: int
+        :param SearchTags: 搜索标签列表
+        :type SearchTags: list of SearchTags
+        """
+        self.SearchInstanceId = None
+        self.SearchInstanceName = None
+        self.Offset = None
+        self.Limit = None
+        self.SearchTags = None
+
+
+    def _deserialize(self, params):
+        self.SearchInstanceId = params.get("SearchInstanceId")
+        self.SearchInstanceName = params.get("SearchInstanceName")
+        self.Offset = params.get("Offset")
+        self.Limit = params.get("Limit")
+        if params.get("SearchTags") is not None:
+            self.SearchTags = []
+            for item in params.get("SearchTags"):
+                obj = SearchTags()
+                obj._deserialize(item)
+                self.SearchTags.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeInstancesNewResponse(AbstractModel):
+    """DescribeInstancesNew返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TotalCount: 实例总数
+        :type TotalCount: int
+        :param InstancesList: 实例数组
+        :type InstancesList: list of InstanceInfo
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TotalCount = None
+        self.InstancesList = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TotalCount = params.get("TotalCount")
+        if params.get("InstancesList") is not None:
+            self.InstancesList = []
+            for item in params.get("InstancesList"):
+                obj = InstanceInfo()
+                obj._deserialize(item)
+                self.InstancesList.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeSpecRequest(AbstractModel):
     """DescribeSpec请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -2251,14 +2326,46 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
+
+
+class SearchTags(AbstractModel):
+    """列表页搜索的标记列表
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TagKey: 标签的键
+        :type TagKey: str
+        :param TagValue: 标签的值
+        :type TagValue: str
+        :param AllValue: 1表示只输入标签的键，没有输入值；0表示输入键时且输入值
+        :type AllValue: int
+        """
+        self.TagKey = None
+        self.TagValue = None
+        self.AllValue = None
+
+
+    def _deserialize(self, params):
+        self.TagKey = params.get("TagKey")
+        self.TagValue = params.get("TagValue")
+        self.AllValue = params.get("AllValue")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class ServiceInfo(AbstractModel):
     """服务详细信息描述。
 
     """
```

### Comparing `tencentcloud-sdk-python-cdwch-3.0.910/tencentcloud/cdwch/v20200915/cdwch_client.py` & `tencentcloud-sdk-python-cdwch-3.0.911/tencentcloud/cdwch/v20200915/cdwch_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -275,14 +275,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeInstancesNew(self, request):
+        """获取实例列表，供外部sdk使用
+
+        :param request: Request instance for DescribeInstancesNew.
+        :type request: :class:`tencentcloud.cdwch.v20200915.models.DescribeInstancesNewRequest`
+        :rtype: :class:`tencentcloud.cdwch.v20200915.models.DescribeInstancesNewResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeInstancesNew", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeInstancesNewResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeSpec(self, request):
         """购买页拉取集群的数据节点和zookeeper节点的规格列表
 
         :param request: Request instance for DescribeSpec.
         :type request: :class:`tencentcloud.cdwch.v20200915.models.DescribeSpecRequest`
         :rtype: :class:`tencentcloud.cdwch.v20200915.models.DescribeSpecResponse`
```

### Comparing `tencentcloud-sdk-python-cdwch-3.0.910/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cdwch-3.0.911/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cdwch-3.0.910/PKG-INFO` & `tencentcloud-sdk-python-cdwch-3.0.911/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdwch
-Version: 3.0.910
+Version: 3.0.911
 Summary: Tencent Cloud Cdwch SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdwch-3.0.910/setup.py` & `tencentcloud-sdk-python-cdwch-3.0.911/setup.py`

 * *Files identical despite different names*

