# Comparing `tmp/tencentcloud-sdk-python-mps-3.0.910.tar.gz` & `tmp/tencentcloud-sdk-python-mps-3.0.911.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-mps-3.0.910.tar", last modified: Thu Jun  8 09:15:17 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-mps-3.0.911.tar", last modified: Fri Jun  9 02:23:23 2023, max compression
```

## Comparing `tencentcloud-sdk-python-mps-3.0.910.tar` & `tencentcloud-sdk-python-mps-3.0.911.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:15:17.000000 tencentcloud-sdk-python-mps-3.0.910/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-08 09:15:16.000000 tencentcloud-sdk-python-mps-3.0.910/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:15:17.000000 tencentcloud-sdk-python-mps-3.0.910/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-08 09:15:16.000000 tencentcloud-sdk-python-mps-3.0.910/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:15:17.000000 tencentcloud-sdk-python-mps-3.0.910/tencentcloud/mps/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:15:17.000000 tencentcloud-sdk-python-mps-3.0.910/tencentcloud/mps/v20190612/
--rw-r--r--   0 root         (0) root         (0)    90653 2023-06-08 09:15:16.000000 tencentcloud-sdk-python-mps-3.0.910/tencentcloud/mps/v20190612/mps_client.py
--rw-r--r--   0 root         (0) root         (0)    13373 2023-06-08 09:15:16.000000 tencentcloud-sdk-python-mps-3.0.910/tencentcloud/mps/v20190612/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 09:15:16.000000 tencentcloud-sdk-python-mps-3.0.910/tencentcloud/mps/v20190612/__init__.py
--rw-r--r--   0 root         (0) root         (0)   817037 2023-06-08 09:15:16.000000 tencentcloud-sdk-python-mps-3.0.910/tencentcloud/mps/v20190612/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 09:15:16.000000 tencentcloud-sdk-python-mps-3.0.910/tencentcloud/mps/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:15:17.000000 tencentcloud-sdk-python-mps-3.0.910/tencentcloud_sdk_python_mps.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 09:15:16.000000 tencentcloud-sdk-python-mps-3.0.910/tencentcloud_sdk_python_mps.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-08 09:15:16.000000 tencentcloud-sdk-python-mps-3.0.910/tencentcloud_sdk_python_mps.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-08 09:15:16.000000 tencentcloud-sdk-python-mps-3.0.910/tencentcloud_sdk_python_mps.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-08 09:15:16.000000 tencentcloud-sdk-python-mps-3.0.910/tencentcloud_sdk_python_mps.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-08 09:15:17.000000 tencentcloud-sdk-python-mps-3.0.910/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-08 09:15:16.000000 tencentcloud-sdk-python-mps-3.0.910/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-08 09:15:17.000000 tencentcloud-sdk-python-mps-3.0.910/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:23:23.000000 tencentcloud-sdk-python-mps-3.0.911/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-09 02:23:23.000000 tencentcloud-sdk-python-mps-3.0.911/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:23:23.000000 tencentcloud-sdk-python-mps-3.0.911/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-09 02:23:23.000000 tencentcloud-sdk-python-mps-3.0.911/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:23:23.000000 tencentcloud-sdk-python-mps-3.0.911/tencentcloud/mps/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:23:23.000000 tencentcloud-sdk-python-mps-3.0.911/tencentcloud/mps/v20190612/
+-rw-r--r--   0 root         (0) root         (0)    90653 2023-06-09 02:23:23.000000 tencentcloud-sdk-python-mps-3.0.911/tencentcloud/mps/v20190612/mps_client.py
+-rw-r--r--   0 root         (0) root         (0)    13373 2023-06-09 02:23:23.000000 tencentcloud-sdk-python-mps-3.0.911/tencentcloud/mps/v20190612/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:23:23.000000 tencentcloud-sdk-python-mps-3.0.911/tencentcloud/mps/v20190612/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   820599 2023-06-09 02:23:23.000000 tencentcloud-sdk-python-mps-3.0.911/tencentcloud/mps/v20190612/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:23:23.000000 tencentcloud-sdk-python-mps-3.0.911/tencentcloud/mps/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:23:23.000000 tencentcloud-sdk-python-mps-3.0.911/tencentcloud_sdk_python_mps.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 02:23:23.000000 tencentcloud-sdk-python-mps-3.0.911/tencentcloud_sdk_python_mps.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-09 02:23:23.000000 tencentcloud-sdk-python-mps-3.0.911/tencentcloud_sdk_python_mps.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-09 02:23:23.000000 tencentcloud-sdk-python-mps-3.0.911/tencentcloud_sdk_python_mps.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-09 02:23:23.000000 tencentcloud-sdk-python-mps-3.0.911/tencentcloud_sdk_python_mps.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-09 02:23:23.000000 tencentcloud-sdk-python-mps-3.0.911/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-09 02:23:23.000000 tencentcloud-sdk-python-mps-3.0.911/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-09 02:23:23.000000 tencentcloud-sdk-python-mps-3.0.911/setup.cfg
```

### Comparing `tencentcloud-sdk-python-mps-3.0.910/README.rst` & `tencentcloud-sdk-python-mps-3.0.911/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mps-3.0.910/tencentcloud/__init__.py` & `tencentcloud-sdk-python-mps-3.0.911/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-mps-3.0.910/tencentcloud/mps/v20190612/mps_client.py` & `tencentcloud-sdk-python-mps-3.0.911/tencentcloud/mps/v20190612/mps_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mps-3.0.910/tencentcloud/mps/v20190612/errorcodes.py` & `tencentcloud-sdk-python-mps-3.0.911/tencentcloud/mps/v20190612/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mps-3.0.910/tencentcloud/mps/v20190612/models.py` & `tencentcloud-sdk-python-mps-3.0.911/tencentcloud/mps/v20190612/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -4160,22 +4160,26 @@
         :param Switch: 语音全文识别任务开关，可选值：
 <li>ON：开启智能语音全文识别任务；</li>
 <li>OFF：关闭智能语音全文识别任务。</li>
         :type Switch: str
         :param SubtitleFormat: 生成的字幕文件格式，不填或者填空字符串表示不生成字幕文件，可选值：
 <li>vtt：生成 WebVTT 字幕文件。</li>
         :type SubtitleFormat: str
+        :param SourceLanguage: 视频源语言。
+        :type SourceLanguage: str
         """
         self.Switch = None
         self.SubtitleFormat = None
+        self.SourceLanguage = None
 
 
     def _deserialize(self, params):
         self.Switch = params.get("Switch")
         self.SubtitleFormat = params.get("SubtitleFormat")
+        self.SourceLanguage = params.get("SourceLanguage")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -4191,22 +4195,26 @@
         :param Switch: 语音全文识别任务开关，可选值：
 <li>ON：开启智能语音全文识别任务；</li>
 <li>OFF：关闭智能语音全文识别任务。</li>
         :type Switch: str
         :param SubtitleFormat: 生成的字幕文件格式，填空字符串表示不生成字幕文件，可选值：
 <li>vtt：生成 WebVTT 字幕文件。</li>
         :type SubtitleFormat: str
+        :param SourceLanguage: 视频源语言。
+        :type SourceLanguage: str
         """
         self.Switch = None
         self.SubtitleFormat = None
+        self.SourceLanguage = None
 
 
     def _deserialize(self, params):
         self.Switch = params.get("Switch")
         self.SubtitleFormat = params.get("SubtitleFormat")
+        self.SourceLanguage = params.get("SourceLanguage")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -4899,22 +4907,25 @@
         :type OcrFullTextConfigure: :class:`tencentcloud.mps.v20190612.models.OcrFullTextConfigureInfo`
         :param OcrWordsConfigure: 文本关键词识别控制参数。
         :type OcrWordsConfigure: :class:`tencentcloud.mps.v20190612.models.OcrWordsConfigureInfo`
         :param AsrFullTextConfigure: 语音全文识别控制参数。
         :type AsrFullTextConfigure: :class:`tencentcloud.mps.v20190612.models.AsrFullTextConfigureInfo`
         :param AsrWordsConfigure: 语音关键词识别控制参数。
         :type AsrWordsConfigure: :class:`tencentcloud.mps.v20190612.models.AsrWordsConfigureInfo`
+        :param TranslateConfigure: 语音翻译控制参数。
+        :type TranslateConfigure: :class:`tencentcloud.mps.v20190612.models.TranslateConfigureInfo`
         """
         self.Name = None
         self.Comment = None
         self.FaceConfigure = None
         self.OcrFullTextConfigure = None
         self.OcrWordsConfigure = None
         self.AsrFullTextConfigure = None
         self.AsrWordsConfigure = None
+        self.TranslateConfigure = None
 
 
     def _deserialize(self, params):
         self.Name = params.get("Name")
         self.Comment = params.get("Comment")
         if params.get("FaceConfigure") is not None:
             self.FaceConfigure = FaceConfigureInfo()
@@ -4927,14 +4938,17 @@
             self.OcrWordsConfigure._deserialize(params.get("OcrWordsConfigure"))
         if params.get("AsrFullTextConfigure") is not None:
             self.AsrFullTextConfigure = AsrFullTextConfigureInfo()
             self.AsrFullTextConfigure._deserialize(params.get("AsrFullTextConfigure"))
         if params.get("AsrWordsConfigure") is not None:
             self.AsrWordsConfigure = AsrWordsConfigureInfo()
             self.AsrWordsConfigure._deserialize(params.get("AsrWordsConfigure"))
+        if params.get("TranslateConfigure") is not None:
+            self.TranslateConfigure = TranslateConfigureInfo()
+            self.TranslateConfigure._deserialize(params.get("TranslateConfigure"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -9759,27 +9773,30 @@
 <li>Preset：系统预置模板；</li>
 <li>Custom：用户自定义模板。</li>
         :type Type: str
         :param ContainerType: 封装格式过滤条件，可选值：
 <li>Video：视频格式，可以同时包含视频流和音频流的封装格式板；</li>
 <li>PureAudio：纯音频格式，只能包含音频流的封装格式。</li>
         :type ContainerType: str
-        :param TEHDType: 极速高清过滤条件，用于过滤普通转码或极速高清转码模板，可选值：
+        :param TEHDType: （建议使用TranscodeType代替）极速高清过滤条件，用于过滤普通转码或极速高清转码模板，可选值：
 <li>Common：普通转码模板；</li>
 <li>TEHD：极速高清模板。</li>
         :type TEHDType: str
         :param Offset: 分页偏移量，默认值：0。
         :type Offset: int
         :param Limit: 返回记录条数，默认值：10，最大值：100。
         :type Limit: int
         :param TranscodeType: 模板类型（替换旧版本 TEHDType），可选值：
 <li>Common：普通转码模板；</li>
-<li>TEHD：极速高清模板。</li>
+<li>TEHD：视频极速高清，老的类型（建议使用 TEHD-100） 。</li>
+<li>TEHD-100：视频极速高清</li>
+<li>TEHD-200：音频极速高清</li>
 <li>Enhance：音视频增强模板。</li>
 默认空，不限制类型。
+
         :type TranscodeType: str
         """
         self.Definitions = None
         self.Type = None
         self.ContainerType = None
         self.TEHDType = None
         self.Offset = None
@@ -14507,23 +14524,26 @@
         :type OcrFullTextConfigure: :class:`tencentcloud.mps.v20190612.models.OcrFullTextConfigureInfoForUpdate`
         :param OcrWordsConfigure: 文本关键词识别控制参数。
         :type OcrWordsConfigure: :class:`tencentcloud.mps.v20190612.models.OcrWordsConfigureInfoForUpdate`
         :param AsrFullTextConfigure: 语音全文识别控制参数。
         :type AsrFullTextConfigure: :class:`tencentcloud.mps.v20190612.models.AsrFullTextConfigureInfoForUpdate`
         :param AsrWordsConfigure: 语音关键词识别控制参数。
         :type AsrWordsConfigure: :class:`tencentcloud.mps.v20190612.models.AsrWordsConfigureInfoForUpdate`
+        :param TranslateConfigure: 语音翻译控制参数。
+        :type TranslateConfigure: :class:`tencentcloud.mps.v20190612.models.TranslateConfigureInfoForUpdate`
         """
         self.Definition = None
         self.Name = None
         self.Comment = None
         self.FaceConfigure = None
         self.OcrFullTextConfigure = None
         self.OcrWordsConfigure = None
         self.AsrFullTextConfigure = None
         self.AsrWordsConfigure = None
+        self.TranslateConfigure = None
 
 
     def _deserialize(self, params):
         self.Definition = params.get("Definition")
         self.Name = params.get("Name")
         self.Comment = params.get("Comment")
         if params.get("FaceConfigure") is not None:
@@ -14537,14 +14557,17 @@
             self.OcrWordsConfigure._deserialize(params.get("OcrWordsConfigure"))
         if params.get("AsrFullTextConfigure") is not None:
             self.AsrFullTextConfigure = AsrFullTextConfigureInfoForUpdate()
             self.AsrFullTextConfigure._deserialize(params.get("AsrFullTextConfigure"))
         if params.get("AsrWordsConfigure") is not None:
             self.AsrWordsConfigure = AsrWordsConfigureInfoForUpdate()
             self.AsrWordsConfigure._deserialize(params.get("AsrWordsConfigure"))
+        if params.get("TranslateConfigure") is not None:
+            self.TranslateConfigure = TranslateConfigureInfoForUpdate()
+            self.TranslateConfigure._deserialize(params.get("TranslateConfigure"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -19920,14 +19943,82 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
+
+
+class TranslateConfigureInfo(AbstractModel):
+    """语音翻译任务控制参数
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Switch: 语音翻译任务开关，可选值：
+<li>ON：开启智能语音翻译任务；</li>
+<li>OFF：关闭智能语音翻译任务。</li>
+        :type Switch: str
+        :param SourceLanguage: 视频源语言。
+        :type SourceLanguage: str
+        :param DestinationLanguage: 翻译目标语言。
+        :type DestinationLanguage: str
+        """
+        self.Switch = None
+        self.SourceLanguage = None
+        self.DestinationLanguage = None
+
+
+    def _deserialize(self, params):
+        self.Switch = params.get("Switch")
+        self.SourceLanguage = params.get("SourceLanguage")
+        self.DestinationLanguage = params.get("DestinationLanguage")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class TranslateConfigureInfoForUpdate(AbstractModel):
+    """语音翻译任务控制参数
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Switch: 语音翻译任务开关，可选值：
+<li>ON：开启智能语音翻译任务；</li>
+<li>OFF：关闭智能语音翻译任务。</li>
+        :type Switch: str
+        :param SourceLanguage: 视频源语言。
+        :type SourceLanguage: str
+        :param DestinationLanguage: 翻译目标语言。
+        :type DestinationLanguage: str
+        """
+        self.Switch = None
+        self.SourceLanguage = None
+        self.DestinationLanguage = None
+
+
+    def _deserialize(self, params):
+        self.Switch = params.get("Switch")
+        self.SourceLanguage = params.get("SourceLanguage")
+        self.DestinationLanguage = params.get("DestinationLanguage")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class UrlInputInfo(AbstractModel):
     """媒体处理 URL 对象信息。
 
     """
```

### Comparing `tencentcloud-sdk-python-mps-3.0.910/tencentcloud_sdk_python_mps.egg-info/PKG-INFO` & `tencentcloud-sdk-python-mps-3.0.911/tencentcloud_sdk_python_mps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mps
-Version: 3.0.910
+Version: 3.0.911
 Summary: Tencent Cloud Mps SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mps-3.0.910/PKG-INFO` & `tencentcloud-sdk-python-mps-3.0.911/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mps
-Version: 3.0.910
+Version: 3.0.911
 Summary: Tencent Cloud Mps SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mps-3.0.910/setup.py` & `tencentcloud-sdk-python-mps-3.0.911/setup.py`

 * *Files identical despite different names*

