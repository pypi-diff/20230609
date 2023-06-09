# Comparing `tmp/tencentcloud-sdk-python-ocr-3.0.910.tar.gz` & `tmp/tencentcloud-sdk-python-ocr-3.0.911.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.910.tar", last modified: Thu Jun  8 09:16:32 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.911.tar", last modified: Fri Jun  9 02:24:12 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ocr-3.0.910.tar` & `tencentcloud-sdk-python-ocr-3.0.911.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:16:32.000000 tencentcloud-sdk-python-ocr-3.0.910/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:16:32.000000 tencentcloud-sdk-python-ocr-3.0.910/tencentcloud_sdk_python_ocr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 09:16:32.000000 tencentcloud-sdk-python-ocr-3.0.910/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-08 09:16:32.000000 tencentcloud-sdk-python-ocr-3.0.910/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-08 09:16:32.000000 tencentcloud-sdk-python-ocr-3.0.910/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-08 09:16:32.000000 tencentcloud-sdk-python-ocr-3.0.910/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-08 09:16:32.000000 tencentcloud-sdk-python-ocr-3.0.910/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:16:32.000000 tencentcloud-sdk-python-ocr-3.0.910/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:16:32.000000 tencentcloud-sdk-python-ocr-3.0.910/tencentcloud/ocr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:16:32.000000 tencentcloud-sdk-python-ocr-3.0.910/tencentcloud/ocr/v20181119/
--rw-r--r--   0 root         (0) root         (0)   114877 2023-06-08 09:16:32.000000 tencentcloud-sdk-python-ocr-3.0.910/tencentcloud/ocr/v20181119/ocr_client.py
--rw-r--r--   0 root         (0) root         (0)     5894 2023-06-08 09:16:32.000000 tencentcloud-sdk-python-ocr-3.0.910/tencentcloud/ocr/v20181119/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 09:16:32.000000 tencentcloud-sdk-python-ocr-3.0.910/tencentcloud/ocr/v20181119/__init__.py
--rw-r--r--   0 root         (0) root         (0)   512616 2023-06-08 09:16:32.000000 tencentcloud-sdk-python-ocr-3.0.910/tencentcloud/ocr/v20181119/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 09:16:32.000000 tencentcloud-sdk-python-ocr-3.0.910/tencentcloud/ocr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-08 09:16:32.000000 tencentcloud-sdk-python-ocr-3.0.910/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-08 09:16:32.000000 tencentcloud-sdk-python-ocr-3.0.910/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-08 09:16:32.000000 tencentcloud-sdk-python-ocr-3.0.910/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-08 09:16:32.000000 tencentcloud-sdk-python-ocr-3.0.910/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:24:12.000000 tencentcloud-sdk-python-ocr-3.0.911/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:24:12.000000 tencentcloud-sdk-python-ocr-3.0.911/tencentcloud_sdk_python_ocr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 02:24:12.000000 tencentcloud-sdk-python-ocr-3.0.911/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-09 02:24:12.000000 tencentcloud-sdk-python-ocr-3.0.911/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-09 02:24:12.000000 tencentcloud-sdk-python-ocr-3.0.911/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-09 02:24:12.000000 tencentcloud-sdk-python-ocr-3.0.911/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-09 02:24:12.000000 tencentcloud-sdk-python-ocr-3.0.911/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:24:12.000000 tencentcloud-sdk-python-ocr-3.0.911/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:24:12.000000 tencentcloud-sdk-python-ocr-3.0.911/tencentcloud/ocr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:24:12.000000 tencentcloud-sdk-python-ocr-3.0.911/tencentcloud/ocr/v20181119/
+-rw-r--r--   0 root         (0) root         (0)   114877 2023-06-09 02:24:12.000000 tencentcloud-sdk-python-ocr-3.0.911/tencentcloud/ocr/v20181119/ocr_client.py
+-rw-r--r--   0 root         (0) root         (0)     5894 2023-06-09 02:24:12.000000 tencentcloud-sdk-python-ocr-3.0.911/tencentcloud/ocr/v20181119/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:24:12.000000 tencentcloud-sdk-python-ocr-3.0.911/tencentcloud/ocr/v20181119/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   512681 2023-06-09 02:24:12.000000 tencentcloud-sdk-python-ocr-3.0.911/tencentcloud/ocr/v20181119/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:24:12.000000 tencentcloud-sdk-python-ocr-3.0.911/tencentcloud/ocr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-09 02:24:12.000000 tencentcloud-sdk-python-ocr-3.0.911/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-09 02:24:12.000000 tencentcloud-sdk-python-ocr-3.0.911/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-09 02:24:12.000000 tencentcloud-sdk-python-ocr-3.0.911/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-09 02:24:12.000000 tencentcloud-sdk-python-ocr-3.0.911/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.910/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.911/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.910
+Version: 3.0.911
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.910/README.rst` & `tencentcloud-sdk-python-ocr-3.0.911/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.910/tencentcloud/ocr/v20181119/ocr_client.py` & `tencentcloud-sdk-python-ocr-3.0.911/tencentcloud/ocr/v20181119/ocr_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.910/tencentcloud/ocr/v20181119/errorcodes.py` & `tencentcloud-sdk-python-ocr-3.0.911/tencentcloud/ocr/v20181119/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.910/tencentcloud/ocr/v20181119/models.py` & `tencentcloud-sdk-python-ocr-3.0.911/tencentcloud/ocr/v20181119/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -562,22 +562,26 @@
         :type ImageBase64: str
         :param ImageUrl: 图片的 Url 地址。
 支持的图片格式：PNG、JPG、JPEG，暂不支持 GIF 格式。
 支持的图片大小：所下载图片经 Base64 编码后不超过 7M。图片下载时间不超过 3 秒。
 图片存储于腾讯云的 Url 可保障更高的下载速度和稳定性，建议图片存储于腾讯云。
 非腾讯云存储的 Url 速度和稳定性可能受一定影响。
         :type ImageUrl: str
+        :param EnableCopyWarn: 是否返回黑白复印件告警码，默认为false
+        :type EnableCopyWarn: bool
         """
         self.ImageBase64 = None
         self.ImageUrl = None
+        self.EnableCopyWarn = None
 
 
     def _deserialize(self, params):
         self.ImageBase64 = params.get("ImageBase64")
         self.ImageUrl = params.get("ImageUrl")
+        self.EnableCopyWarn = params.get("EnableCopyWarn")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -607,22 +611,18 @@
         :param Period: 营业期限
         :type Period: str
         :param ComposingForm: 组成形式
         :type ComposingForm: str
         :param SetDate: 成立日期
         :type SetDate: str
         :param RecognizeWarnCode: Code 告警码列表和释义：
--20001 非营业执照
 -9102 黑白复印件告警
-注：告警码可以同时存在多个
         :type RecognizeWarnCode: list of int
         :param RecognizeWarnMsg: 告警码说明：
-OCR_WARNING_TYPE_NOT_MATCH 非营业执照
 WARN_COPY_CARD 黑白复印件告警
-注：告警信息可以同时存在多个
         :type RecognizeWarnMsg: list of str
         :param IsDuplication: 是否为副本。1为是，-1为不是。
         :type IsDuplication: int
         :param RegistrationDate: 登记日期
         :type RegistrationDate: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.910/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ocr-3.0.911/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ocr-3.0.910/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.911/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.910
+Version: 3.0.911
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.910/setup.py` & `tencentcloud-sdk-python-ocr-3.0.911/setup.py`

 * *Files identical despite different names*

