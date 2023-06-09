# Comparing `tmp/nonebot_plugin_random_ban-0.2.0.tar.gz` & `tmp/nonebot_plugin_random_ban-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_random_ban-0.2.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_random_ban-0.2.1.tar", max compression
```

## Comparing `nonebot_plugin_random_ban-0.2.0.tar` & `nonebot_plugin_random_ban-0.2.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1084 2022-12-03 13:20:36.036837 nonebot_plugin_random_ban-0.2.0/LICENSE
--rw-r--r--   0        0        0    11009 2023-06-08 10:52:01.056272 nonebot_plugin_random_ban-0.2.0/nonebot_plugin_random_ban/__init__.py
--rw-r--r--   0        0        0     1007 2023-06-08 10:52:21.554666 nonebot_plugin_random_ban-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6258 2023-06-08 10:41:06.739392 nonebot_plugin_random_ban-0.2.0/README.md
--rw-r--r--   0        0        0     7036 1970-01-01 00:00:00.000000 nonebot_plugin_random_ban-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2022-12-03 13:20:36.036837 nonebot_plugin_random_ban-0.2.1/LICENSE
+-rw-r--r--   0        0        0    11270 2023-06-09 11:02:26.939177 nonebot_plugin_random_ban-0.2.1/nonebot_plugin_random_ban/__init__.py
+-rw-r--r--   0        0        0     1007 2023-06-09 11:05:24.971341 nonebot_plugin_random_ban-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6372 2023-06-09 11:04:30.729213 nonebot_plugin_random_ban-0.2.1/README.md
+-rw-r--r--   0        0        0     7145 1970-01-01 00:00:00.000000 nonebot_plugin_random_ban-0.2.1/PKG-INFO
```

### Comparing `nonebot_plugin_random_ban-0.2.0/LICENSE` & `nonebot_plugin_random_ban-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_random_ban-0.2.0/nonebot_plugin_random_ban/__init__.py` & `nonebot_plugin_random_ban-0.2.1/nonebot_plugin_random_ban/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     nonebot.logger.warning("random_ban的anyone_can_random_ban没有配置，默认只有bot的超管、群管理和群主可以使用 随机禁言 功能。")
 
 catch_str = on_command('随机禁言', aliases={"随禁"})
 
 
 # 正则匹配时间
 def parse_time_string(time_string):
-    pattern = r'(\d+(?:\.\d+)?)(?:分钟|分|小时|时|天)?'
+    pattern = r'(\d+(?:\.\d+)?)(分钟|分|小时|时|天)?'
     match = re.match(pattern, time_string)
 
     # print(f"time_string={time_string}")
 
     if match:
         groups = match.groups()
         num_groups = len(groups)
@@ -115,14 +115,17 @@
             try:
                 if len(content) > 0:
                     tmp = parse_time_string(content)
                     if tmp is None:
                         msg = "参数解析失败（请传入正整数的最大禁言时间）"
                         await catch_str.finish(Message(f'{msg}'), reply_message=True)
                     max_ban_time = random.randint(1, tmp)
+
+                # 最大只能30天
+                max_ban_time = min(max_ban_time, 43199)
             except FinishedException:
                 pass
             except Exception as e:
                 print(e)
                 msg = "参数解析失败（请传入正整数的最大禁言时间）"
                 await catch_str.finish(Message(f'{msg}'), reply_message=True)
             # 获取群号 event.group_id
@@ -155,14 +158,17 @@
             if len(content) > 0:
                 tmp = parse_time_string(content)
                 # print(f"tmp={tmp}")
                 if tmp is None:
                     msg = "参数解析失败（请传入正整数的最大禁言时间）"
                     await catch_str.finish(Message(f'{msg}'), reply_message=True)
                 max_ban_time = random.randint(1, tmp)
+
+            # 最大只能30天
+            max_ban_time = min(max_ban_time, 43199)
         except FinishedException:
             pass
         except Exception as e:
             print(e)
             msg = "参数解析失败（请传入正整数的最大禁言时间）"
             await catch_str.finish(Message(f'{msg}'), reply_message=True)
         # 获取群号 event.group_id
@@ -199,14 +205,17 @@
     try:
         if len(content) > 0:
             tmp = parse_time_string(content)
             if tmp is None:
                 msg = "参数解析失败（请传入正整数的最大禁言时间）"
                 await catch_str.finish(Message(f'{msg}'), reply_message=True)
             max_ban_time = random.randint(1, tmp)
+        
+        # 最大只能30天
+        max_ban_time = min(max_ban_time, 43199)
     except FinishedException:
         pass
     except Exception as e:
         print(e)
         msg = "参数解析失败（请传入正整数的最大禁言时间）"
         await catch_str2.finish(Message(f'{msg}'), reply_message=True)
     # 获取群号 event.group_id
```

### Comparing `nonebot_plugin_random_ban-0.2.0/pyproject.toml` & `nonebot_plugin_random_ban-0.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-random_ban"
-version = "0.2.0"
+version = "0.2.1"
 description = "随机禁言一名群员或自己n分钟（n通过参入数字然后随机实现），简单粗暴。"
 authors = ["Ikaros <327209194@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_random_ban"}]
 homepage = "https://github.com/Ikaros-521/nonebot_plugin_random_ban"
 repository = "https://github.com/Ikaros-521/nonebot_plugin_random_ban"
```

### Comparing `nonebot_plugin_random_ban-0.2.0/README.md` & `nonebot_plugin_random_ban-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -176,9 +176,14 @@
 
 ### 0.2.0
 
 - 新增 传参的单位兼容，分、分钟、时、小时、天。
 - 修改 艾特 为 回复的形式。
 - 优化代码。
 
+### 0.2.1
+
+- 修复 传参只匹配数字不匹配单位的bug
+- 修复 传入禁言时长大于30天的bug
+
 </details>
```

#### html2text {}

```diff
@@ -56,8 +56,10 @@
 è³ææ¶å»ï¼ä¸çæ¢å¤åå¹³ã ``` ![](docs/result.jpg) ## â æå±
 èªè¡ä¿®æ¹æºç åµ~ ## ð æ´æ°æ¥å¿  å±å¼/æ¶èµ· ### 0.0.1 -
 æä»¶åæ¬¡åå¸ ### 0.0.2 - è¡¥åæä»¶åä¿¡æ¯ - ä¼åææ¡£ ### 0.0.3 -
 æ°å¢å½ä»¤ å£ç æ ç¦æï¼èªå·±ç¦èªå·± ### 0.0.4 - ä¼åææ¡£ ###
 0.0.5 - æ°å¢å¯ä»¥å¼å¯ä»»ä½äººé½ä½¿ç¨éæºç¦è¨çéç½®é¡¹ ### 0.1.0
 - æ°å¢ è³ææ¶å»ï¼å°±æ¯ææäººå¯ä»¥ä½¿ç¨`éç¦`å½ä»¤ï¼åºæ¿ã
 ### 0.2.0 - æ°å¢ ä¼ åçåä½å¼å®¹ï¼åãåéãæ¶ãå°æ¶ãå¤©ã
-- ä¿®æ¹ è¾ç¹ ä¸º åå¤çå½¢å¼ã - ä¼åä»£ç ã
+- ä¿®æ¹ è¾ç¹ ä¸º åå¤çå½¢å¼ã - ä¼åä»£ç ã ### 0.2.1 - ä¿®å¤
+ä¼ ååªå¹éæ°å­ä¸å¹éåä½çbug - ä¿®å¤
+ä¼ å¥ç¦è¨æ¶é¿å¤§äº30å¤©çbug
```

### Comparing `nonebot_plugin_random_ban-0.2.0/PKG-INFO` & `nonebot_plugin_random_ban-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-random-ban
-Version: 0.2.0
+Version: 0.2.1
 Summary: 随机禁言一名群员或自己n分钟（n通过参入数字然后随机实现），简单粗暴。
 Home-page: https://github.com/Ikaros-521/nonebot_plugin_random_ban
 License: MIT
 Author: Ikaros
 Author-email: 327209194@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -197,10 +197,15 @@
 
 ### 0.2.0
 
 - 新增 传参的单位兼容，分、分钟、时、小时、天。
 - 修改 艾特 为 回复的形式。
 - 优化代码。
 
+### 0.2.1
+
+- 修复 传参只匹配数字不匹配单位的bug
+- 修复 传入禁言时长大于30天的bug
+
 </details>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-random-ban Version: 0.2.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-random-ban Version: 0.2.1 Summary:
 éæºç¦è¨ä¸åç¾¤åæèªå·±nåéï¼néè¿åå¥æ°å­ç¶åéæºå®ç°ï¼ï¼ç®åç²æ´ã
 Home-page: https://github.com/Ikaros-521/nonebot_plugin_random_ban License: MIT
 Author: Ikaros Author-email: 327209194@qq.com Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
@@ -69,8 +69,10 @@
 è³ææ¶å»ï¼ä¸çæ¢å¤åå¹³ã ``` ![](docs/result.jpg) ## â æå±
 èªè¡ä¿®æ¹æºç åµ~ ## ð æ´æ°æ¥å¿  å±å¼/æ¶èµ· ### 0.0.1 -
 æä»¶åæ¬¡åå¸ ### 0.0.2 - è¡¥åæä»¶åä¿¡æ¯ - ä¼åææ¡£ ### 0.0.3 -
 æ°å¢å½ä»¤ å£ç æ ç¦æï¼èªå·±ç¦èªå·± ### 0.0.4 - ä¼åææ¡£ ###
 0.0.5 - æ°å¢å¯ä»¥å¼å¯ä»»ä½äººé½ä½¿ç¨éæºç¦è¨çéç½®é¡¹ ### 0.1.0
 - æ°å¢ è³ææ¶å»ï¼å°±æ¯ææäººå¯ä»¥ä½¿ç¨`éç¦`å½ä»¤ï¼åºæ¿ã
 ### 0.2.0 - æ°å¢ ä¼ åçåä½å¼å®¹ï¼åãåéãæ¶ãå°æ¶ãå¤©ã
-- ä¿®æ¹ è¾ç¹ ä¸º åå¤çå½¢å¼ã - ä¼åä»£ç ã
+- ä¿®æ¹ è¾ç¹ ä¸º åå¤çå½¢å¼ã - ä¼åä»£ç ã ### 0.2.1 - ä¿®å¤
+ä¼ ååªå¹éæ°å­ä¸å¹éåä½çbug - ä¿®å¤
+ä¼ å¥ç¦è¨æ¶é¿å¤§äº30å¤©çbug
```

