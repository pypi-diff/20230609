# Comparing `tmp/nonebot_plugin_record-1.0.4.tar.gz` & `tmp/nonebot_plugin_record-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_record-1.0.4.tar", max compression
+gzip compressed data, was "nonebot_plugin_record-1.0.5.tar", max compression
```

## Comparing `nonebot_plugin_record-1.0.4.tar` & `nonebot_plugin_record-1.0.5.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1062 2023-01-15 14:15:53.000000 nonebot_plugin_record-1.0.4/LICENSE
--rw-r--r--   0        0        0     3390 2023-05-13 07:11:57.207255 nonebot_plugin_record-1.0.4/nonebot_plugin_record/__init__.py
--rw-r--r--   0        0        0     1590 2023-05-13 06:55:12.204661 nonebot_plugin_record-1.0.4/nonebot_plugin_record/baidu.py
--rw-r--r--   0        0        0      381 2023-01-15 15:10:41.532083 nonebot_plugin_record-1.0.4/nonebot_plugin_record/config.py
--rw-r--r--   0        0        0     3870 2023-05-13 06:55:24.424835 nonebot_plugin_record-1.0.4/nonebot_plugin_record/tencent.py
--rw-r--r--   0        0        0      847 2023-05-13 08:02:01.220758 nonebot_plugin_record-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     5425 2023-05-13 07:57:03.354354 nonebot_plugin_record-1.0.4/README.md
--rw-r--r--   0        0        0     6309 1970-01-01 00:00:00.000000 nonebot_plugin_record-1.0.4/setup.py
--rw-r--r--   0        0        0     6280 1970-01-01 00:00:00.000000 nonebot_plugin_record-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-01-15 14:15:53.000000 nonebot_plugin_record-1.0.5/LICENSE
+-rw-r--r--   0        0        0     3870 2023-06-09 01:13:41.845836 nonebot_plugin_record-1.0.5/nonebot_plugin_record/__init__.py
+-rw-r--r--   0        0        0     1590 2023-05-13 06:55:12.204661 nonebot_plugin_record-1.0.5/nonebot_plugin_record/baidu.py
+-rw-r--r--   0        0        0      425 2023-06-09 01:13:53.827328 nonebot_plugin_record-1.0.5/nonebot_plugin_record/config.py
+-rw-r--r--   0        0        0     3870 2023-05-13 06:55:24.424835 nonebot_plugin_record-1.0.5/nonebot_plugin_record/tencent.py
+-rw-r--r--   0        0        0      847 2023-06-09 01:14:12.191188 nonebot_plugin_record-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     6694 2023-06-09 01:39:50.170405 nonebot_plugin_record-1.0.5/README.md
+-rw-r--r--   0        0        0     7522 1970-01-01 00:00:00.000000 nonebot_plugin_record-1.0.5/PKG-INFO
```

### Comparing `nonebot_plugin_record-1.0.4/LICENSE` & `nonebot_plugin_record-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_record-1.0.4/nonebot_plugin_record/__init__.py` & `nonebot_plugin_record-1.0.5/nonebot_plugin_record/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -63,33 +63,42 @@
 
     - bot: Bot 对象
     - event: Event 对象
     """
     if plugin_config.nonebot_plugin_gocqhttp is True:
         path_amr = "./accounts/" + bot.self_id + "/data/voices/" + event.get_message()[0].data["file"]
     else:
-        path_amr = "./data/voices/" + event.get_message()[0].data["file"]
+        path_amr = plugin_config.gocqhttp_address + "data/voices/" + event.get_message()[0].data["file"]
     path_pcm = path_amr[0:-4] + ".pcm"
-    pilk.decode(path_amr, path_pcm)
+    try:
+        pilk.decode(path_amr, path_pcm)
+    except OSError:
+        logger.error("转换音频文件失败，尝试转换的音频文件目录为 " + path_amr + " ,请检查nonebot_plugin_gocqhttp配置项和gocqhttp_address配置项是否正确填写或是否有文件权限问题")
+        return None
+    except:
+        logger.error("转换音频文件失败，发生未知错误")
+        return None
+    else:
+        logger.debug("Successfully Transform The Audio file")
     with open(path_pcm, 'rb') as f:
         speech = base64.b64encode(f.read()).decode('utf-8')
     length = os.path.getsize(path_pcm)
     os.remove(path_pcm)
     if length == 0:
-        logger.error("加载音频文件失败，请检查nonebot_plugin_gocqhttp配置项是否填写正确")
+        logger.error("转换音频文件成功，但加载音频文件失败，发生未知错误")
         return None
     else:
         logger.debug("Successfully Load The Audio file")
         if plugin_config.asr_api_provider == "baidu":
-            text = await baidu_get_text(speech, length)
             logger.debug("Using Baidu API")
+            text = await baidu_get_text(speech, length)
             return text
         elif plugin_config.asr_api_provider == "tencent":
-            text = await tencent_get_text(speech, length)
             logger.debug("Using Tencent API")
+            text = await tencent_get_text(speech, length)
             return text
         elif plugin_config.asr_api_provider == None:
             logger.error("获取配置失败，请检查asr_api_provider配置项是否正确填写")
             return None
         else:
             logger.error("配置填写错误，asr_api_provider配置只能填写“baidu”或“tencent”")
             return None
```

### Comparing `nonebot_plugin_record-1.0.4/nonebot_plugin_record/baidu.py` & `nonebot_plugin_record-1.0.5/nonebot_plugin_record/baidu.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_record-1.0.4/nonebot_plugin_record/tencent.py` & `nonebot_plugin_record-1.0.5/nonebot_plugin_record/tencent.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_record-1.0.4/pyproject.toml` & `nonebot_plugin_record-1.0.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-record"
-version = "1.0.4"
+version = "1.0.5"
 description = "基于 Nonebot2 的语音功能适配插件，包括语音事件响应器，语音识别、语音合成等功能"
 authors = ["ITSevin <itsevin@qq.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/itsevin/nonebot_plugin_record"
 repository = "https://github.com/itsevin/nonebot_plugin_record"
 documentation = "https://github.com/itsevin/nonebot_plugin_record#readme"
```

### Comparing `nonebot_plugin_record-1.0.4/README.md` & `nonebot_plugin_record-1.0.5/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -37,23 +37,45 @@
 
 - 使用 pip
 
 ```
 pip install nonebot_plugin_record
 ```
 
+## 兼容性
+
+### 支持的go-cqhttp（最新版本）协议
+
+|      |      |      |      |
+| ---- | ---- | ---- | ---- |
+|   protocol   |   协议   |   收语音   |   发语音   |
+|   1   |   phone   |   未知   |   未知   |
+|   2   |   watch   |   不兼容   |   兼容   |
+|   3   |   MacOS   |   兼容   |   不兼容   |
+|   4   |   企点   |   未知   |   未知   |
+|   5   |   iPad   |   兼容   |   兼容   |
+|   6   |   aPad   |   兼容   |   不兼容   |
+
+
+> 未知是未测试的情况；不兼容是没通过我的测试的情况，不一定准确，可能是我自己账号的封控问题，具体请自行测试
+
+发现实际与我测试结果有出入的欢迎来这里讨论 https://github.com/itsevin/nonebot_plugin_record/issues/1
+
 ## 配置项
 
 ```
-asr_api_provider="" #必填，API提供商，填写“baidu”或“tencent”
-asr_api_key="" #必填，百度智能云的API_KRY或腾讯云的SECRET_ID
-asr_secret_key="" #必填，百度智能云的SECRET_KRY或腾讯云的SECRET_KEY
-nonebot_plugin_gocqhttp=False #选填，是否使用nonebot2插件版本的go-cqhttp，默认为False
+asr_api_provider="" # 必填，API提供商，填写“baidu”或“tencent”
+asr_api_key="" # 必填，百度智能云的API_KRY或腾讯云的SECRET_ID
+asr_secret_key="" # 必填，百度智能云的SECRET_KRY或腾讯云的SECRET_KEY
+nonebot_plugin_gocqhttp=False # 选填，是否使用nonebot2插件版本的go-cqhttp，默认为False
+gocqhttp_address="" # 选填，非插件版本go-cqhttp的运行目录，默认为“./”，非插件版本go-cqhttp和nonebot运行目录不同时须填写，插件版本不用填写， nonebot_plugin_gocqhttp=True 时该配置无效
 ```
 
+> gocqhttp_address 配置项可填绝对路径（如 /root/gocqhttp/ ）或相对路径（如 ../../gocqhttp/ ）
+
 ## API选择与配置
 
 ### 选什么API?
 
 - 百度智能云-短语音识别标准版：5并发，15万次免费调用量，期限180天
 - 腾讯云-一句话识别：每月5000次免费调用量（推荐）
 
@@ -189,14 +211,19 @@
 2. 确认是否正确按照本插件使用说明使用
 3. 排查日志，通过日志内容尝试找出问题并自行解决
 4. 在配置文件中配置```LOG_LEVEL=DEBUG```，然后在日志中查看debug日志，并同时根据本插件源码尝试找出问题并自行解决（确认是本插件的问题可以提issue或者pr）
 5. 问题仍未解决可以提issue，要求提供详细问题描述和较为完整的debug级别的相关日志
 
 ## 更新日志
 
+### 2023/6/8 \[v1.0.5]
+
+- 修复非插件版本go-cqhttp和nonebot运行目录不相同时的问题
+- 优化日志输出
+
 ### 2023/5/13 \[v1.0.4]
 
 - 重构代码，舍弃CQ码过时写法
 - 增加dubug和info级别的日志输出
 
 ### 2023/1/27 \[v1.0.3]
```

### Comparing `nonebot_plugin_record-1.0.4/PKG-INFO` & `nonebot_plugin_record-1.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-record
-Version: 1.0.4
+Version: 1.0.5
 Summary: 基于 Nonebot2 的语音功能适配插件，包括语音事件响应器，语音识别、语音合成等功能
 Home-page: https://github.com/itsevin/nonebot_plugin_record
 License: MIT
 Keywords: nonebot,nonebot2,nonebot_plugin_record
 Author: ITSevin
 Author-email: itsevin@qq.com
 Requires-Python: >=3.8,<4.0
@@ -61,23 +61,45 @@
 
 - 使用 pip
 
 ```
 pip install nonebot_plugin_record
 ```
 
+## 兼容性
+
+### 支持的go-cqhttp（最新版本）协议
+
+|      |      |      |      |
+| ---- | ---- | ---- | ---- |
+|   protocol   |   协议   |   收语音   |   发语音   |
+|   1   |   phone   |   未知   |   未知   |
+|   2   |   watch   |   不兼容   |   兼容   |
+|   3   |   MacOS   |   兼容   |   不兼容   |
+|   4   |   企点   |   未知   |   未知   |
+|   5   |   iPad   |   兼容   |   兼容   |
+|   6   |   aPad   |   兼容   |   不兼容   |
+
+
+> 未知是未测试的情况；不兼容是没通过我的测试的情况，不一定准确，可能是我自己账号的封控问题，具体请自行测试
+
+发现实际与我测试结果有出入的欢迎来这里讨论 https://github.com/itsevin/nonebot_plugin_record/issues/1
+
 ## 配置项
 
 ```
-asr_api_provider="" #必填，API提供商，填写“baidu”或“tencent”
-asr_api_key="" #必填，百度智能云的API_KRY或腾讯云的SECRET_ID
-asr_secret_key="" #必填，百度智能云的SECRET_KRY或腾讯云的SECRET_KEY
-nonebot_plugin_gocqhttp=False #选填，是否使用nonebot2插件版本的go-cqhttp，默认为False
+asr_api_provider="" # 必填，API提供商，填写“baidu”或“tencent”
+asr_api_key="" # 必填，百度智能云的API_KRY或腾讯云的SECRET_ID
+asr_secret_key="" # 必填，百度智能云的SECRET_KRY或腾讯云的SECRET_KEY
+nonebot_plugin_gocqhttp=False # 选填，是否使用nonebot2插件版本的go-cqhttp，默认为False
+gocqhttp_address="" # 选填，非插件版本go-cqhttp的运行目录，默认为“./”，非插件版本go-cqhttp和nonebot运行目录不同时须填写，插件版本不用填写， nonebot_plugin_gocqhttp=True 时该配置无效
 ```
 
+> gocqhttp_address 配置项可填绝对路径（如 /root/gocqhttp/ ）或相对路径（如 ../../gocqhttp/ ）
+
 ## API选择与配置
 
 ### 选什么API?
 
 - 百度智能云-短语音识别标准版：5并发，15万次免费调用量，期限180天
 - 腾讯云-一句话识别：每月5000次免费调用量（推荐）
 
@@ -213,14 +235,19 @@
 2. 确认是否正确按照本插件使用说明使用
 3. 排查日志，通过日志内容尝试找出问题并自行解决
 4. 在配置文件中配置```LOG_LEVEL=DEBUG```，然后在日志中查看debug日志，并同时根据本插件源码尝试找出问题并自行解决（确认是本插件的问题可以提issue或者pr）
 5. 问题仍未解决可以提issue，要求提供详细问题描述和较为完整的debug级别的相关日志
 
 ## 更新日志
 
+### 2023/6/8 \[v1.0.5]
+
+- 修复非插件版本go-cqhttp和nonebot运行目录不相同时的问题
+- 优化日志输出
+
 ### 2023/5/13 \[v1.0.4]
 
 - 重构代码，舍弃CQ码过时写法
 - 增加dubug和info级别的日志输出
 
 ### 2023/1/27 \[v1.0.3]
```

