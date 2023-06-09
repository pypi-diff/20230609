# Comparing `tmp/tencentcloud-sdk-python-cls-3.0.910.tar.gz` & `tmp/tencentcloud-sdk-python-cls-3.0.911.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cls-3.0.910.tar", last modified: Thu Jun  8 09:06:58 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cls-3.0.911.tar", last modified: Fri Jun  9 02:15:57 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cls-3.0.910.tar` & `tencentcloud-sdk-python-cls-3.0.911.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:06:58.000000 tencentcloud-sdk-python-cls-3.0.910/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-08 09:06:58.000000 tencentcloud-sdk-python-cls-3.0.910/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:06:58.000000 tencentcloud-sdk-python-cls-3.0.910/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:06:58.000000 tencentcloud-sdk-python-cls-3.0.910/tencentcloud/cls/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:06:58.000000 tencentcloud-sdk-python-cls-3.0.910/tencentcloud/cls/v20201016/
--rw-r--r--   0 root         (0) root         (0)     8559 2023-06-08 09:06:58.000000 tencentcloud-sdk-python-cls-3.0.910/tencentcloud/cls/v20201016/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 09:06:58.000000 tencentcloud-sdk-python-cls-3.0.910/tencentcloud/cls/v20201016/__init__.py
--rw-r--r--   0 root         (0) root         (0)   254636 2023-06-08 09:06:58.000000 tencentcloud-sdk-python-cls-3.0.910/tencentcloud/cls/v20201016/models.py
--rw-r--r--   0 root         (0) root         (0)    67925 2023-06-08 09:06:58.000000 tencentcloud-sdk-python-cls-3.0.910/tencentcloud/cls/v20201016/cls_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 09:06:58.000000 tencentcloud-sdk-python-cls-3.0.910/tencentcloud/cls/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-08 09:06:58.000000 tencentcloud-sdk-python-cls-3.0.910/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:06:58.000000 tencentcloud-sdk-python-cls-3.0.910/tencentcloud_sdk_python_cls.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 09:06:58.000000 tencentcloud-sdk-python-cls-3.0.910/tencentcloud_sdk_python_cls.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-08 09:06:58.000000 tencentcloud-sdk-python-cls-3.0.910/tencentcloud_sdk_python_cls.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-08 09:06:58.000000 tencentcloud-sdk-python-cls-3.0.910/tencentcloud_sdk_python_cls.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-08 09:06:58.000000 tencentcloud-sdk-python-cls-3.0.910/tencentcloud_sdk_python_cls.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-08 09:06:58.000000 tencentcloud-sdk-python-cls-3.0.910/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-08 09:06:58.000000 tencentcloud-sdk-python-cls-3.0.910/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-08 09:06:58.000000 tencentcloud-sdk-python-cls-3.0.910/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:15:57.000000 tencentcloud-sdk-python-cls-3.0.911/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-09 02:15:57.000000 tencentcloud-sdk-python-cls-3.0.911/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:15:57.000000 tencentcloud-sdk-python-cls-3.0.911/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:15:57.000000 tencentcloud-sdk-python-cls-3.0.911/tencentcloud/cls/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:15:57.000000 tencentcloud-sdk-python-cls-3.0.911/tencentcloud/cls/v20201016/
+-rw-r--r--   0 root         (0) root         (0)     8559 2023-06-09 02:15:57.000000 tencentcloud-sdk-python-cls-3.0.911/tencentcloud/cls/v20201016/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:15:57.000000 tencentcloud-sdk-python-cls-3.0.911/tencentcloud/cls/v20201016/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   254636 2023-06-09 02:15:57.000000 tencentcloud-sdk-python-cls-3.0.911/tencentcloud/cls/v20201016/models.py
+-rw-r--r--   0 root         (0) root         (0)    67913 2023-06-09 02:15:57.000000 tencentcloud-sdk-python-cls-3.0.911/tencentcloud/cls/v20201016/cls_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:15:57.000000 tencentcloud-sdk-python-cls-3.0.911/tencentcloud/cls/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-09 02:15:57.000000 tencentcloud-sdk-python-cls-3.0.911/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:15:57.000000 tencentcloud-sdk-python-cls-3.0.911/tencentcloud_sdk_python_cls.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 02:15:57.000000 tencentcloud-sdk-python-cls-3.0.911/tencentcloud_sdk_python_cls.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-09 02:15:57.000000 tencentcloud-sdk-python-cls-3.0.911/tencentcloud_sdk_python_cls.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-09 02:15:57.000000 tencentcloud-sdk-python-cls-3.0.911/tencentcloud_sdk_python_cls.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-09 02:15:57.000000 tencentcloud-sdk-python-cls-3.0.911/tencentcloud_sdk_python_cls.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-09 02:15:57.000000 tencentcloud-sdk-python-cls-3.0.911/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-09 02:15:57.000000 tencentcloud-sdk-python-cls-3.0.911/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-09 02:15:57.000000 tencentcloud-sdk-python-cls-3.0.911/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cls-3.0.910/README.rst` & `tencentcloud-sdk-python-cls-3.0.911/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.910/tencentcloud/cls/v20201016/errorcodes.py` & `tencentcloud-sdk-python-cls-3.0.911/tencentcloud/cls/v20201016/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.910/tencentcloud/cls/v20201016/models.py` & `tencentcloud-sdk-python-cls-3.0.911/tencentcloud/cls/v20201016/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.910/tencentcloud/cls/v20201016/cls_client.py` & `tencentcloud-sdk-python-cls-3.0.911/tencentcloud/cls/v20201016/cls_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1519,15 +1519,15 @@
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def UploadLog(self, request, body):
         """## 提示
-        为了保障您日志数据的可靠性以及更高效地使用日志服务，建议您使用CLS优化后的接口[上传结构化日志](https://cloud.tencent.com/document/product/614/16873)上传日志。
+        为了保障您日志数据的可靠性以及更高效地使用日志服务，建议您使用CLS优化后的接口[上传结构化日志](https://cloud.tencent.com/document/product/614/16873)。
 
         同时我们给此接口专门优化定制了多个语言版本的SDK供您选择，SDK提供统一的异步发送、资源控制、自动重试、优雅关闭、感知上报等功能，使上报日志功能更完善，详情请参考[SDK采集](https://cloud.tencent.com/document/product/614/67157)。
 
         同时云API上传日志接口也支持同步上传日志数据，如果您选择继续使用此接口请参考下文。
 
         ## 功能描述
```

### Comparing `tencentcloud-sdk-python-cls-3.0.910/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cls-3.0.911/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cls-3.0.910/tencentcloud_sdk_python_cls.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cls-3.0.911/tencentcloud_sdk_python_cls.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cls
-Version: 3.0.910
+Version: 3.0.911
 Summary: Tencent Cloud Cls SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cls-3.0.910/PKG-INFO` & `tencentcloud-sdk-python-cls-3.0.911/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cls
-Version: 3.0.910
+Version: 3.0.911
 Summary: Tencent Cloud Cls SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cls-3.0.910/setup.py` & `tencentcloud-sdk-python-cls-3.0.911/setup.py`

 * *Files identical despite different names*

