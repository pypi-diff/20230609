# Comparing `tmp/tencentcloud-sdk-python-ses-3.0.910.tar.gz` & `tmp/tencentcloud-sdk-python-ses-3.0.911.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ses-3.0.910.tar", last modified: Thu Jun  8 09:17:56 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ses-3.0.911.tar", last modified: Fri Jun  9 02:25:38 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ses-3.0.910.tar` & `tencentcloud-sdk-python-ses-3.0.911.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:17:56.000000 tencentcloud-sdk-python-ses-3.0.910/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-08 09:17:56.000000 tencentcloud-sdk-python-ses-3.0.910/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:17:56.000000 tencentcloud-sdk-python-ses-3.0.910/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:17:56.000000 tencentcloud-sdk-python-ses-3.0.910/tencentcloud/ses/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 09:17:56.000000 tencentcloud-sdk-python-ses-3.0.910/tencentcloud/ses/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:17:56.000000 tencentcloud-sdk-python-ses-3.0.910/tencentcloud/ses/v20201002/
--rw-r--r--   0 root         (0) root         (0)    11392 2023-06-08 09:17:56.000000 tencentcloud-sdk-python-ses-3.0.910/tencentcloud/ses/v20201002/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    28299 2023-06-08 09:17:56.000000 tencentcloud-sdk-python-ses-3.0.910/tencentcloud/ses/v20201002/ses_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 09:17:56.000000 tencentcloud-sdk-python-ses-3.0.910/tencentcloud/ses/v20201002/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71833 2023-06-08 09:17:56.000000 tencentcloud-sdk-python-ses-3.0.910/tencentcloud/ses/v20201002/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-08 09:17:56.000000 tencentcloud-sdk-python-ses-3.0.910/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:17:56.000000 tencentcloud-sdk-python-ses-3.0.910/tencentcloud_sdk_python_ses.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 09:17:56.000000 tencentcloud-sdk-python-ses-3.0.910/tencentcloud_sdk_python_ses.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-08 09:17:56.000000 tencentcloud-sdk-python-ses-3.0.910/tencentcloud_sdk_python_ses.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-08 09:17:56.000000 tencentcloud-sdk-python-ses-3.0.910/tencentcloud_sdk_python_ses.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-08 09:17:56.000000 tencentcloud-sdk-python-ses-3.0.910/tencentcloud_sdk_python_ses.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-08 09:17:56.000000 tencentcloud-sdk-python-ses-3.0.910/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-08 09:17:56.000000 tencentcloud-sdk-python-ses-3.0.910/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-08 09:17:56.000000 tencentcloud-sdk-python-ses-3.0.910/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:25:38.000000 tencentcloud-sdk-python-ses-3.0.911/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-09 02:25:38.000000 tencentcloud-sdk-python-ses-3.0.911/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:25:38.000000 tencentcloud-sdk-python-ses-3.0.911/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:25:38.000000 tencentcloud-sdk-python-ses-3.0.911/tencentcloud/ses/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:25:38.000000 tencentcloud-sdk-python-ses-3.0.911/tencentcloud/ses/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:25:38.000000 tencentcloud-sdk-python-ses-3.0.911/tencentcloud/ses/v20201002/
+-rw-r--r--   0 root         (0) root         (0)    11392 2023-06-09 02:25:38.000000 tencentcloud-sdk-python-ses-3.0.911/tencentcloud/ses/v20201002/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    28299 2023-06-09 02:25:38.000000 tencentcloud-sdk-python-ses-3.0.911/tencentcloud/ses/v20201002/ses_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:25:38.000000 tencentcloud-sdk-python-ses-3.0.911/tencentcloud/ses/v20201002/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71855 2023-06-09 02:25:38.000000 tencentcloud-sdk-python-ses-3.0.911/tencentcloud/ses/v20201002/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-09 02:25:38.000000 tencentcloud-sdk-python-ses-3.0.911/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:25:38.000000 tencentcloud-sdk-python-ses-3.0.911/tencentcloud_sdk_python_ses.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 02:25:38.000000 tencentcloud-sdk-python-ses-3.0.911/tencentcloud_sdk_python_ses.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-09 02:25:38.000000 tencentcloud-sdk-python-ses-3.0.911/tencentcloud_sdk_python_ses.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-09 02:25:38.000000 tencentcloud-sdk-python-ses-3.0.911/tencentcloud_sdk_python_ses.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-09 02:25:38.000000 tencentcloud-sdk-python-ses-3.0.911/tencentcloud_sdk_python_ses.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-09 02:25:38.000000 tencentcloud-sdk-python-ses-3.0.911/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-09 02:25:38.000000 tencentcloud-sdk-python-ses-3.0.911/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-09 02:25:38.000000 tencentcloud-sdk-python-ses-3.0.911/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ses-3.0.910/README.rst` & `tencentcloud-sdk-python-ses-3.0.911/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ses-3.0.910/tencentcloud/ses/v20201002/errorcodes.py` & `tencentcloud-sdk-python-ses-3.0.911/tencentcloud/ses/v20201002/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ses-3.0.910/tencentcloud/ses/v20201002/ses_client.py` & `tencentcloud-sdk-python-ses-3.0.911/tencentcloud/ses/v20201002/ses_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ses-3.0.910/tencentcloud/ses/v20201002/models.py` & `tencentcloud-sdk-python-ses-3.0.911/tencentcloud/ses/v20201002/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         :type Simple: :class:`tencentcloud.ses.v20201002.models.Simple`
         :param Attachments: 需要发送附件时，填写附件相关参数（暂未支持）
         :type Attachments: list of Attachment
         :param CycleParam: 周期发送任务的必要参数
         :type CycleParam: :class:`tencentcloud.ses.v20201002.models.CycleEmailParam`
         :param TimedParam: 定时发送任务的必要参数
         :type TimedParam: :class:`tencentcloud.ses.v20201002.models.TimedEmailParam`
-        :param Unsubscribe: 退订链接选项 0: 不加入退订链接 1: 简体中文 2: 英文 3: 繁体中文 4: 西班牙语 5: 法语 6: 德语 7: 日语 8: 韩语 9: 阿拉伯语
+        :param Unsubscribe: 退订链接选项 0: 不加入退订链接 1: 简体中文 2: 英文 3: 繁体中文 4: 西班牙语 5: 法语 6: 德语 7: 日语 8: 韩语 9: 阿拉伯语 10: 泰语
         :type Unsubscribe: str
         :param ADLocation: 是否添加广告标识 0:不添加 1:添加到subject前面，2:添加到subject后面
         :type ADLocation: int
         """
         self.FromEmailAddress = None
         self.ReceiverId = None
         self.Subject = None
@@ -1513,15 +1513,15 @@
         :type Bcc: list of str
         :param Template: 使用模板发送时，填写的模板相关参数。因 Simple 已经废除使用，Template 为必填项
         :type Template: :class:`tencentcloud.ses.v20201002.models.Template`
         :param Simple: 已废弃
         :type Simple: :class:`tencentcloud.ses.v20201002.models.Simple`
         :param Attachments: 需要发送附件时，填写附件相关参数。腾讯云接口请求最大支持 8M 的请求包，附件内容经过 Base64 预期扩大1.5倍，应该控制所有附件的总大小最大在 4M 以内，整体请求超出 8M 时接口会返回错误
         :type Attachments: list of Attachment
-        :param Unsubscribe: 退订链接选项 0: 不加入退订链接 1: 简体中文 2: 英文 3: 繁体中文 4: 西班牙语 5: 法语 6: 德语 7: 日语 8: 韩语 9: 阿拉伯语
+        :param Unsubscribe: 退订链接选项 0: 不加入退订链接 1: 简体中文 2: 英文 3: 繁体中文 4: 西班牙语 5: 法语 6: 德语 7: 日语 8: 韩语 9: 阿拉伯语 10: 泰语
         :type Unsubscribe: str
         :param TriggerType: 邮件触发类型 0:非触发类，默认类型，营销类邮件、非即时类邮件等选择此类型  1:触发类，验证码等即时发送类邮件，若邮件超过一定大小，系统会自动选择非触发类型通道
         :type TriggerType: int
         """
         self.FromEmailAddress = None
         self.Destination = None
         self.Subject = None
```

### Comparing `tencentcloud-sdk-python-ses-3.0.910/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ses-3.0.911/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ses-3.0.910/tencentcloud_sdk_python_ses.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ses-3.0.911/tencentcloud_sdk_python_ses.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ses
-Version: 3.0.910
+Version: 3.0.911
 Summary: Tencent Cloud Ses SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ses-3.0.910/PKG-INFO` & `tencentcloud-sdk-python-ses-3.0.911/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ses
-Version: 3.0.910
+Version: 3.0.911
 Summary: Tencent Cloud Ses SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ses-3.0.910/setup.py` & `tencentcloud-sdk-python-ses-3.0.911/setup.py`

 * *Files identical despite different names*

