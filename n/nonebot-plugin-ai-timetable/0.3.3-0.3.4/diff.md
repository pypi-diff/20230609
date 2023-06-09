# Comparing `tmp/nonebot_plugin_ai_timetable-0.3.3.tar.gz` & `tmp/nonebot_plugin_ai_timetable-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_ai_timetable-0.3.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_ai_timetable-0.3.4.tar", max compression
```

## Comparing `nonebot_plugin_ai_timetable-0.3.3.tar` & `nonebot_plugin_ai_timetable-0.3.4.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1065 2023-04-23 14:11:01.873509 nonebot_plugin_ai_timetable-0.3.3/LICENSE
--rw-r--r--   0        0        0     7743 2023-04-23 14:11:01.873509 nonebot_plugin_ai_timetable-0.3.3/README.md
--rw-r--r--   0        0        0    10816 2023-04-23 14:11:01.873509 nonebot_plugin_ai_timetable-0.3.3/nonebot_plugin_ai_timetable/__init__.py
--rw-r--r--   0        0        0    16800 2023-04-23 14:11:01.873509 nonebot_plugin_ai_timetable-0.3.3/nonebot_plugin_ai_timetable/utils.py
--rw-r--r--   0        0        0      496 2023-04-23 14:11:01.873509 nonebot_plugin_ai_timetable-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     8462 1970-01-01 00:00:00.000000 nonebot_plugin_ai_timetable-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-09 13:16:28.018178 nonebot_plugin_ai_timetable-0.3.4/LICENSE
+-rw-r--r--   0        0        0     8224 2023-06-09 13:16:28.018178 nonebot_plugin_ai_timetable-0.3.4/README.md
+-rw-r--r--   0        0        0    11638 2023-06-09 13:16:28.018178 nonebot_plugin_ai_timetable-0.3.4/nonebot_plugin_ai_timetable/__init__.py
+-rw-r--r--   0        0        0      359 2023-06-09 13:16:28.018178 nonebot_plugin_ai_timetable-0.3.4/nonebot_plugin_ai_timetable/config.py
+-rw-r--r--   0        0        0    20535 2023-06-09 13:16:28.018178 nonebot_plugin_ai_timetable-0.3.4/nonebot_plugin_ai_timetable/utils.py
+-rw-r--r--   0        0        0      496 2023-06-09 13:16:28.018178 nonebot_plugin_ai_timetable-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     8943 1970-01-01 00:00:00.000000 nonebot_plugin_ai_timetable-0.3.4/PKG-INFO
```

### Comparing `nonebot_plugin_ai_timetable-0.3.3/LICENSE` & `nonebot_plugin_ai_timetable-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ai_timetable-0.3.3/README.md` & `nonebot_plugin_ai_timetable-0.3.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,47 @@
+Metadata-Version: 2.1
+Name: nonebot-plugin-ai-timetable
+Version: 0.3.4
+Summary: 小爱课程表
+Author: maoxiog
+Author-email: 674550338@qq.com
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: httpx (>=0.23.0,<0.24.0)
+Requires-Dist: nonebot-adapter-onebot (>=2.1.0,<3.0.0)
+Requires-Dist: nonebot-plugin-apscheduler (>=0.2.0,<0.3.0)
+Requires-Dist: nonebot-plugin-htmlrender (>=0.2.0,<0.3.0)
+Requires-Dist: nonebot2 (>=2.0.0rc1,<3.0.0)
+Description-Content-Type: text/markdown
+
 <p align="center">
   <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
 </p>
 <div align="center">
 
 # nonebot-plugin-ai-timetable
 
 ✨*基于Nonebot2的对接小爱课程表的插件*✨
   
-<div align="left">
-  
-# 前言
+<a href="https://github.com/nonebot/nonebot2">
+  <img src="https://img.shields.io/badge/nonebot-v2-red" alt="nonebot">
+</a> 
+<a href="./LICENSE">
+    <img src="https://img.shields.io/github/license/maoxig/nonebot-plugin-ai-timetable" alt="license">
+</a>
+<a href="https://pypi.python.org/pypi/nonebot-plugin-ai-timetable">
+    <img src="https://img.shields.io/pypi/v/nonebot-plugin-ai-timetable" alt="pypi">
+</a>
+<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
 
-   这是本人第一次在github发布的项目，也是第一个python项目，完全是萌新，很多地方写的可能很拉，大佬轻喷
-目前还不是很完善，有什么bug或者建议欢迎提issues
+<div align="left">
 
 ## 💿安装
 
 1. 通过`pip`或`nb`安装；
     - 使用nb(极度推荐)
   
        在机器人目录下命令行使用`nb plugin install nonebot_plugin_ai_timetable`
@@ -35,20 +60,20 @@
 
 3. ~~所以为什么不直接用小爱课表呢~~
 
 4. ⚙️插件配置
 
 这些配置都已设好默认值，如果想要修改配置，在机器人目录下的.env.*里面可以填写以下选项(可选)
 
-|         config          | type  | default |          example           | usage                                                                              |
-| :---------------------: | :---: | :-----: | :------------------------: | :--------------------------------------------------------------------------------- |
-|      TIMETABLE_PIC      | bool  |  true   |    TIMETABLE_PIC=false     | 可选择某日课表以图片/文字发送，默认以图片发送(true)                                |
-| TIMETABLE_ALOCK_SOMEDAY |  int  |   22    | TIMETABLE_ALOCK_SOMEDAY=15 | 订阅某日课表的发送时间，必须是0-24的数字                                           |
-|    TIMETABLE_ALOCK_8    |  int  |   21    |    TIMETABLE_ALOCK_8=16    | 订阅早八的发送时间，必须是0-24的数字.这里发送的都是第二天的，所以建议设置为18-23点 |
-|    TIMETABLE_SEND_TIME    |  float  |   0.5    |    TIMETABLE_SEND_TIME=1    | 订阅课程提前发送的时间，单位是`小时`，可以是整数也可以是小数，建议不要设的太大，避免出现无法预料的bug |
+|         config          | type  | default |          example           | usage                                                                                                 |
+| :---------------------: | :---: | :-----: | :------------------------: | :---------------------------------------------------------------------------------------------------- |
+|      TIMETABLE_PIC      | bool  |  true   |    TIMETABLE_PIC=false     | 可选择某日课表以图片/文字发送，默认以图片发送(true)                                                   |
+| TIMETABLE_ALOCK_SOMEDAY |  int  |   22    | TIMETABLE_ALOCK_SOMEDAY=15 | 订阅某日课表的发送时间，必须是0-24的数字                                                              |
+|    TIMETABLE_ALOCK_8    |  int  |   21    |    TIMETABLE_ALOCK_8=16    | 订阅早八的发送时间，必须是0-24的数字.这里发送的都是第二天的，所以建议设置为18-23点                    |
+|   TIMETABLE_SEND_TIME   | float |   0.5   |   TIMETABLE_SEND_TIME=1    | 订阅课程提前发送的时间，单位是`小时`，可以是整数也可以是小数，建议不要设的太大，避免出现无法预料的bug |
 
 ## 💿依赖
 
 ```python
 nb plugin install nonebot_plugin_htmlrender
 nb plugin install nonebot_plugin_apscheduler
 ```
@@ -110,14 +135,20 @@
 2. 删去了文本中所有奇怪的口癖喵
 
 - 2023-04-23:
 
 1. 修改帮助
 2. 修复定时提醒重复发送的bug
 
+- 2023-06-09:
+
+1. 更新插件元数据
+2. 优化配置读取
+3. 格式化代码
+
 </details>
 
 ## 🎉命令
 
 1. 我的课表|小爱课表|本周课表|下周课表：获取本周|下周的完全课表，使用前须先导入课表，这里的课表是在线课表
 
 2. 导入课表：需要有小爱课表分享出来的链接，打开小爱课程表，手动添加课程或从教务导入(已适配了大部分高校)课程后
@@ -174,16 +205,19 @@
 
 - [x] 增加更多的配置项
 
 - [x] 重构代码
 
 - [x] 订阅指定的课
 
+- [ ] 适配插件datastore，接入数据库
+
 - [ ] 完善插件
 
 ## 🐛存在的问题
 
  1. 小爱课表分享的链接大概2周后会过期，会使得`我的课表\下周课表`无法使用，需要重新分享，但是仍能使用本地课表，也可以更新本地课表
 
  2. 机器人重启后定时任务会丢失
 
 ## 喜欢的话就点个star✨吧QAQ
+
```

#### html2text {}

```diff
@@ -1,30 +1,38 @@
+Metadata-Version: 2.1 Name: nonebot-plugin-ai-timetable Version: 0.3.4 Summary:
+å°ç±è¯¾ç¨è¡¨ Author: maoxiog Author-email: 674550338@qq.com Requires-Python:
+>=3.8,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Requires-Dist: httpx (>=0.23.0,<0.24.0)
+Requires-Dist: nonebot-adapter-onebot (>=2.1.0,<3.0.0) Requires-Dist: nonebot-
+plugin-apscheduler (>=0.2.0,<0.3.0) Requires-Dist: nonebot-plugin-htmlrender
+(>=0.2.0,<0.3.0) Requires-Dist: nonebot2 (>=2.0.0rc1,<3.0.0) Description-
+Content-Type: text/markdown
                                    [nonebot]
                          # nonebot-plugin-ai-timetable
-            â¨*åºäºNonebot2çå¯¹æ¥å°ç±è¯¾ç¨è¡¨çæä»¶*â¨
-# åè¨
-è¿æ¯æ¬äººç¬¬ä¸æ¬¡å¨githubåå¸çé¡¹ç®ï¼ä¹æ¯ç¬¬ä¸ä¸ªpythoné¡¹ç®ï¼å®å¨æ¯èæ°ï¼å¾å¤å°æ¹åçå¯è½å¾æï¼å¤§ä½¬è½»å·
-ç®åè¿ä¸æ¯å¾å®åï¼æä»ä¹bugæèå»ºè®®æ¬¢è¿æissues ##
-ð¿å®è£ 1. éè¿`pip`æ`nb`å®è£ï¼ - ä½¿ç¨nb(æåº¦æ¨è)
+ â¨*åºäºNonebot2çå¯¹æ¥å°ç±è¯¾ç¨è¡¨çæä»¶*â¨ [nonebot] [license]
+                                [pypi] [python]
+## ð¿å®è£ 1. éè¿`pip`æ`nb`å®è£ï¼ - ä½¿ç¨nb(æåº¦æ¨è)
 å¨æºå¨äººç®å½ä¸å½ä»¤è¡ä½¿ç¨`nb plugin install
 nonebot_plugin_ai_timetable` - ä½¿ç¨pip(ä¸æ¨è):
 ~~æ¢ç¶ä¸æ¨èå°±ä¸è¦æ³çè¿æ ·å®è£äºåå~~ 2.
 æ¬å°æ°æ®ä¿å­å¨`data/ai_timetable/userdata.json`ä»¥å`data/ai_timetable/
 usertable.json`ï¼åå«å¯¹åºç¨æ·åéçé¾æ¥åæ¬å°ä¿å­çè¯¾è¡¨ ##
 ðç®ä» 1.
 å»çå¼ä¸é®å¯¼å¥å°ç±è¯¾è¡¨ï¼è®©ä½ çbotå®ç°å°ç±è¯¾è¡¨çåè½ 2.
 ç¨æ·è¯¾è¡¨æ°æ®éç¦»ï¼æ éæå¿è¯¾ç¨æ¶é´å²çªãä¸åå­¦æ ¡è¯¾è¡¨ä¸åç­é®é¢
 3. ~~æä»¥ä¸ºä»ä¹ä¸ç´æ¥ç¨å°ç±è¯¾è¡¨å¢~~ 4. âï¸æä»¶éç½®
 è¿äºéç½®é½å·²è®¾å¥½é»è®¤å¼ï¼å¦ææ³è¦ä¿®æ¹éç½®ï¼å¨æºå¨äººç®å½ä¸ç.env.*éé¢å¯ä»¥å¡«åä»¥ä¸éé¡¹
 (å¯é) | config | type | default | example | usage | | :--------------------
 -: | :---: | :-----: | :------------------------: | :--------------------------
-------------------------------------------------------- | | TIMETABLE_PIC |
-bool | true | TIMETABLE_PIC=false | å¯éæ©ææ¥è¯¾è¡¨ä»¥å¾ç/
-æå­åéï¼é»è®¤ä»¥å¾çåé(true) | | TIMETABLE_ALOCK_SOMEDAY | int |
-22 | TIMETABLE_ALOCK_SOMEDAY=15 |
+-------------------------------------------------------------------------- | |
+TIMETABLE_PIC | bool | true | TIMETABLE_PIC=false |
+å¯éæ©ææ¥è¯¾è¡¨ä»¥å¾ç/æå­åéï¼é»è®¤ä»¥å¾çåé(true) | |
+TIMETABLE_ALOCK_SOMEDAY | int | 22 | TIMETABLE_ALOCK_SOMEDAY=15 |
 è®¢éææ¥è¯¾è¡¨çåéæ¶é´ï¼å¿é¡»æ¯0-24çæ°å­ | |
 TIMETABLE_ALOCK_8 | int | 21 | TIMETABLE_ALOCK_8=16 |
 è®¢éæ©å«çåéæ¶é´ï¼å¿é¡»æ¯0-
 24çæ°å­.è¿éåéçé½æ¯ç¬¬äºå¤©çï¼æä»¥å»ºè®®è®¾ç½®ä¸º18-23ç¹ |
 | TIMETABLE_SEND_TIME | float | 0.5 | TIMETABLE_SEND_TIME=1 |
 è®¢éè¯¾ç¨æååéçæ¶é´ï¼åä½æ¯`å°æ¶`ï¼å¯ä»¥æ¯æ´æ°ä¹å¯ä»¥æ¯å°æ°ï¼å»ºè®®ä¸è¦è®¾çå¤ªå¤§ï¼é¿ååºç°æ æ³é¢æçbug
 | ## ð¿ä¾èµ ```python nb plugin install nonebot_plugin_htmlrender nb plugin
@@ -48,15 +56,16 @@
 éæäºä»£ç ï¼ä¼åäºè®¸å¤å°æ¹~~ççç´¯æ­»äº~~ 2.
 ä¿®å¤äºä¸äºbugï¼ä¼åäºä½éª 3. å¢å äºæ©å«|ææ¥æ©å«çæ¥è¯¢
 4. æ´æ°çæ¬åå»ºè®®éæ°`å¯¼å¥è¯¾è¡¨`ï¼é¿ååºç°æäºbug - 2023-04-
 02: 1. ä¿®å¤bug 2. ä¼åå¸®å©å¾ç 3. å®æ¶ä»»å¡éæºå»¶å0-
 60sï¼é²æ­¢é£æ§ 4. å¢å è®¢éæå®è¯¾ç¨çåè½ - 2023-04-14: 1.
 ä¿®å¤äºè®¢éè¯¾ç¨åéæ¶é´éè¯¯çbug 2.
 å å»äºææ¬ä¸­ææå¥æªçå£çåµ - 2023-04-23: 1. ä¿®æ¹å¸®å© 2.
-ä¿®å¤å®æ¶æééå¤åéçbug  ## ðå½ä»¤ 1.
+ä¿®å¤å®æ¶æééå¤åéçbug - 2023-06-09: 1. æ´æ°æä»¶åæ°æ® 2.
+ä¼åéç½®è¯»å 3. æ ¼å¼åä»£ç   ## ðå½ä»¤ 1.
 æçè¯¾è¡¨|å°ç±è¯¾è¡¨|æ¬å¨è¯¾è¡¨|ä¸å¨è¯¾è¡¨ï¼è·åæ¬å¨|ä¸å¨çå®å¨è¯¾è¡¨ï¼ä½¿ç¨åé¡»åå¯¼å¥è¯¾è¡¨ï¼è¿éçè¯¾è¡¨æ¯å¨çº¿è¯¾è¡¨
 2.
 å¯¼å¥è¯¾è¡¨ï¼éè¦æå°ç±è¯¾è¡¨åäº«åºæ¥çé¾æ¥ï¼æå¼å°ç±è¯¾ç¨è¡¨ï¼æå¨æ·»å è¯¾ç¨æä»æå¡å¯¼å¥
 (å·²ééäºå¤§é¨åé«æ ¡)è¯¾ç¨å ![Image text](https://github.com/maoxig/
 nonebot-plugin-ai-timetable/blob/main/resource/export.jpg)
 å¨åºæ¬è®¾ç½®éæå¼å§ä¸è¯¾æ¶é´ç­è°æ´å¥½ä¹å
 (å°¤å¶æ¯æ¶é´ãèæ°)ï¼æåäº«è¯¾è¡¨å¾å°çé¾æ¥åéç»botå³å¯å¯¼å¥æ¬å°
@@ -95,12 +104,13 @@
 -
 å¦æå¯¼å¥è¯¾è¡¨åå¨å°ç±è¯¾è¡¨åä¿®æ¹äºè¯¾ç¨ï¼ç´æ¥ç»botåéæ´æ°è¯¾è¡¨å³å¯æ´æ°æ¬å°è¯¾è¡¨
 -
 å½ä½ ä¸»é¡µçè¯¾è¡¨åå­¦æ ¡è¯¾è¡¨åºæ¬ä¸è´æ¶ï¼é£ä¹å°ç±è¯¾ç¨è¡¨å°±è¢«è°æå¥½äºï¼å¯ä»¥å¯¼å¥äº
 ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/
 resource/settings.jpg) ## ð¦è®¡å - [x] æ¥è¯¢ä¸èè¯¾çä¿¡æ¯ - [x]
 å¯éæ©æ¯å¦åéå¾çä»¥é¿åé£æ§ - [x] å¢å æ´å¤çéç½®é¡¹ - [x]
-éæä»£ç  - [x] è®¢éæå®çè¯¾ - [ ] å®åæä»¶ ## ðå­å¨çé®é¢
-1.
+éæä»£ç  - [x] è®¢éæå®çè¯¾ - [ ]
+ééæä»¶datastoreï¼æ¥å¥æ°æ®åº - [ ] å®åæä»¶ ##
+ðå­å¨çé®é¢ 1.
 å°ç±è¯¾è¡¨åäº«çé¾æ¥å¤§æ¦2å¨åä¼è¿æï¼ä¼ä½¿å¾`æçè¯¾è¡¨\ä¸å¨è¯¾è¡¨`æ æ³ä½¿ç¨ï¼éè¦éæ°åäº«ï¼ä½æ¯ä»è½ä½¿ç¨æ¬å°è¯¾è¡¨ï¼ä¹å¯ä»¥æ´æ°æ¬å°è¯¾è¡¨
 2. æºå¨äººéå¯åå®æ¶ä»»å¡ä¼ä¸¢å¤± ##
 åæ¬¢çè¯å°±ç¹ä¸ªstarâ¨å§QAQ
```

### Comparing `nonebot_plugin_ai_timetable-0.3.3/nonebot_plugin_ai_timetable/__init__.py` & `nonebot_plugin_ai_timetable-0.3.4/nonebot_plugin_ai_timetable/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,71 +1,91 @@
-from .utils import *
+from .utils import (
+    AiTimetable,
+    scheduler,
+    logger,
+    config,
+    md_to_pic,
+    userdata,
+    usertable,
+)
 from nonebot.plugin import PluginMetadata
 from nonebot.params import RegexMatched, ArgStr, CommandArg, ArgPlainText
 from nonebot.matcher import Matcher
 from nonebot import on_command, on_regex
+import datetime
+import re
+import random
 from nonebot.adapters.onebot.v11 import Bot, MessageSegment, MessageEvent, Message
+from .config import Config
 
 logger.opt(colors=True).info(
     "已检测到软依赖<y>nonebot_plugin_apscheduler</y>, <g>开启定时任务功能</g>"
     if scheduler
     else "未检测到软依赖<y>nonebot_plugin_apscheduler</y>,<r>禁用定时任务功能</r>"
 )
 
 __plugin_meta__ = PluginMetadata(
     name="小爱课表",
     description="一键导入课表、查看课表、提醒上课、查询课程",
     usage=AiTimetable.ai_timetable__usage,
+    type="application",
+    homepage="https://github.com/maoxig/nonebot-plugin-ai-timetable",
+    config=Config,
+    supported_adapters={"~onebot.v11"},
 )
 
 
-my_table = on_regex(r'^(小爱|我的|本周|下周)(课表)', priority=20, block=False)
-new_table = on_command('导入课表', priority=20, block=False, aliases={'创建课表'})
-table_help = on_command("课表帮助", priority=20, block=False,
-                        aliases={"课表介绍", "课表怎么用"})
+my_table = on_regex(r"^(小爱|我的|本周|下周)(课表)", priority=20, block=False)
+new_table = on_command("导入课表", priority=20, block=False, aliases={"创建课表"})
+table_help = on_command("课表帮助", priority=20, block=False, aliases={"课表介绍", "课表怎么用"})
 someday_table = on_regex(
-    r'^(((今|明|昨|后)(天|日))|(星期|周)(一|二|三|四|五|六|日|天))(课表|的课|课程|((上|有)(什么|啥)课))', priority=20, block=False)
+    r"^(((今|明|昨|后)(天|日))|(星期|周)(一|二|三|四|五|六|日|天))(课表|的课|课程|((上|有)(什么|啥)课))",
+    priority=20,
+    block=False,
+)
 add_alock_someday = on_regex(
-    r'^(订阅|提醒)((周|星期)(一|二|三|四|五|六|日|天))(课程|课表|的课)', priority=20, block=True)
-add_alock_morningcalss = on_regex(
-    r'^(订阅|提醒)早八', priority=20, block=True)
+    r"^(订阅|提醒)((周|星期)(一|二|三|四|五|六|日|天))(课程|课表|的课)", priority=20, block=True
+)
+add_alock_morningcalss = on_command("订阅早八", priority=20, block=True, aliases={"提醒早八"})
 remove_alock_someday = on_regex(
-    r'^(取消)(订阅|提醒)((周|星期)(一|二|三|四|五|六|日|天))(课程|的课|课表)', priority=20, block=False)
+    r"^(取消)(订阅|提醒)((周|星期)(一|二|三|四|五|六|日|天))(课程|的课|课表)", priority=20, block=False
+)
 sub_class = on_command("订阅课程", priority=25, block=False, aliases={"提醒课程"})
-remove_sub_class = on_command(
-    "取消订阅课程", priority=25, block=False, aliases={"取消提醒课程"})
+remove_sub_class = on_command("取消订阅课程", priority=25, block=False, aliases={"取消提醒课程"})
 remove_alock_morningclass = on_command(
-    "取消订阅早八", priority=20, block=False, aliases={"取消提醒早八"})
-renew_table = on_command("更新本地课表", priority=20, block=False, aliases={'更新课表'})
+    "取消订阅早八", priority=20, block=False, aliases={"取消提醒早八"}
+)
+renew_table = on_command("更新本地课表", priority=20, block=False, aliases={"更新课表"})
 send_next_class = on_command("上课", priority=20, block=False, aliases={"下节课"})
-next_morningclass = on_command(
-    "早八", priority=20, block=False, aliases={"明日早八", "明天早八"})
+next_morningclass = on_command("早八", priority=20, block=False, aliases={"明日早八", "明天早八"})
 
 
 @table_help.handle()
 async def _():
     """课表帮助"""
-    if timetable_pic:
-        await table_help.finish(MessageSegment.image(await md_to_pic(AiTimetable.ai_timetable__usage)))
+    if config.timetable_pic:
+        await table_help.finish(
+            MessageSegment.image(await md_to_pic(AiTimetable.ai_timetable__usage))
+        )
     else:
         await table_help.finish(AiTimetable.ai_timetable__usage)
 
 
 @my_table.handle()
 async def _(event: MessageEvent, key: str = RegexMatched()):
     """获取本周/下周的课表"""
     uid = event.get_user_id()
     if uid in userdata:
         pic = await AiTimetable.my_table(uid=uid, key=key)
         await my_table.finish(MessageSegment.image(pic))
     else:
-        await my_table.finish('你还没有导入课表,发送/导入课表来导入吧！', at_sender=True)
+        await my_table.finish("你还没有导入课表,发送/导入课表来导入吧！", at_sender=True)
 
 
-@new_table.got('key', '请发送小爱课程表导出的链接,发送/取消以退出')
+@new_table.got("key", "请发送小爱课程表导出的链接,发送/取消以退出")
 async def _(event: MessageEvent, key: str = ArgStr()):
     """更新本地的课表"""
     uid = event.get_user_id()
     url = str(key)
     if re.match(AiTimetable.base_url_re, url):  # 用户发送的链接匹配
         msg = await AiTimetable.new_table(uid=uid, base_url=key)
         await new_table.finish(msg)
@@ -74,156 +94,181 @@
 
 
 @someday_table.handle()
 async def _(event: MessageEvent, key: str = RegexMatched()):
     """发送某天的课表"""
     uid = event.get_user_id()
     if uid not in userdata:
-        await someday_table.finish('你还没有导入课表,发送/导入课表来导入吧！', at_sender=True)
+        await someday_table.finish("你还没有导入课表,发送/导入课表来导入吧！", at_sender=True)
     else:
-        if timetable_pic:
+        if config.timetable_pic:
             pic = await AiTimetable.someday_table(uid=uid, key=key)
             await someday_table.finish(MessageSegment.image(pic))
         else:
-            await someday_table.finish(await AiTimetable.someday_table(uid=uid, key=key))
+            await someday_table.finish(
+                await AiTimetable.someday_table(uid=uid, key=key)
+            )
 
 
 @renew_table.handle()  # 更新本地课表
 async def _(event: MessageEvent):
     uid = event.get_user_id()
     if uid not in userdata:
-        await renew_table.finish('你还没有导入课表,发送/导入课表来导入吧！', at_sender=True)
+        await renew_table.finish("你还没有导入课表,发送/导入课表来导入吧！", at_sender=True)
     else:
         msg = await AiTimetable.renew_table(uid=uid)
         await renew_table.finish(msg, at_sender=True)
 
 
 @send_next_class.handle()  # 发送本节课、以及下节课信息
 async def _(event: MessageEvent):
     uid = event.get_user_id()
     if uid not in userdata:
-        await send_next_class.finish('你还没有导入课表,发送/导入课表来导入吧！', at_sender=True)
+        await send_next_class.finish("你还没有导入课表,发送/导入课表来导入吧！", at_sender=True)
     else:
-        msg = "现在时间是"+datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
+        msg = "现在时间是" + datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
         msg += AiTimetable.now_class(uid)
         msg += AiTimetable.next_class(uid)
         await send_next_class.finish(msg, at_sender=True)
 
 
 @next_morningclass.handle()
 async def _(bot: Bot, event: MessageEvent):
     """发送早八"""
     uid = event.get_user_id()
     if uid not in userdata:
-        await send_next_class.finish('你还没有导入课表,发送/导入课表来导入吧！', at_sender=True)
+        await send_next_class.finish("你还没有导入课表,发送/导入课表来导入吧！", at_sender=True)
     else:
         await AiTimetable.post_alock_morningclass(uid=uid, bot=bot, event=event)
 
-#-----------以下为定时任务----------------#
+
+# -----------以下为定时任务----------------#
 
 
 @add_alock_someday.handle()
 async def _(bot: Bot, event: MessageEvent, key: str = RegexMatched()):
     """订阅课表"""
     uid = event.get_user_id()
     if uid not in userdata:
-        await add_alock_someday.finish('你还没有导入课表,发送/导入课表来导入吧！', at_sender=True)
+        await add_alock_someday.finish("你还没有导入课表,发送/导入课表来导入吧！", at_sender=True)
     else:
         if scheduler:
-            send_day = (AiTimetable.weekday_int(key)+5) % 7
-            if scheduler.get_job(str(uid+"post_alock"+str(send_day))):
+            send_day = (AiTimetable.weekday_int(key) + 5) % 7
+            if scheduler.get_job(str(uid + "post_alock" + str(send_day))):
                 await add_alock_someday.finish("出错了！你好像已经订阅过这天的课表了呢", at_sender=True)
-            scheduler.add_job(AiTimetable.post_alock, "cron", hour=timetable_alock_someday, second=random.randint(0, 60), id=str(
-                uid+"post_alock"+str(send_day)), day_of_week=send_day,kwargs={"key": key, "uid": uid, "bot": bot, "event": event})
+            scheduler.add_job(
+                AiTimetable.post_alock,
+                "cron",
+                hour=config.timetable_alock_someday,
+                second=random.randint(0, 60),
+                id=str(uid + "post_alock" + str(send_day)),
+                day_of_week=send_day,
+                kwargs={"key": key, "uid": uid, "bot": bot, "event": event},
+            )
             await add_alock_someday.finish("定时提醒添加成功！", at_sender=True)
         else:
             await add_alock_someday.finish("apscheduler插件未载入,无法添加定时提醒", at_sender=True)
 
 
 @remove_alock_someday.handle()
 async def _(bot: Bot, event: MessageEvent, key: str = RegexMatched()):
     """删除订阅课表"""
     uid = event.get_user_id()
     if uid not in userdata:
-        await add_alock_someday.finish('你还没有导入课表,发送/导入课表来导入吧！', at_sender=True)
+        await add_alock_someday.finish("你还没有导入课表,发送/导入课表来导入吧！", at_sender=True)
     else:
         if scheduler:
-            send_day = (AiTimetable.weekday_int(key)+5) % 7
-            if scheduler.get_job(str(uid+"post_alock"+str(send_day))):
-                scheduler.remove_job(str(uid+"post_alock"+str(send_day)))
+            send_day = (AiTimetable.weekday_int(key) + 5) % 7
+            if scheduler.get_job(str(uid + "post_alock" + str(send_day))):
+                scheduler.remove_job(str(uid + "post_alock" + str(send_day)))
                 await remove_alock_someday.finish("定时提醒删除成功！", at_sender=True)
             else:
                 await remove_alock_someday.finish("出错了,好像没有订阅过这天的课表呢", at_sender=True)
         else:
-            await remove_alock_someday.finish("apscheduler插件未载入,无法删除定时提醒", at_sender=True)
+            await remove_alock_someday.finish(
+                "apscheduler插件未载入,无法删除定时提醒", at_sender=True
+            )
+
 
-#-----------以下为订阅早八----------------#
+# -----------以下为订阅早八----------------#
 
 
 @add_alock_morningcalss.handle()
 async def _(bot: Bot, event: MessageEvent):
     uid = event.get_user_id()
     if uid not in userdata:
-        await add_alock_morningcalss.finish('你还没有导入课表,发送/导入课表来导入吧！', at_sender=True)
+        await add_alock_morningcalss.finish("你还没有导入课表,发送/导入课表来导入吧！", at_sender=True)
     else:
         if scheduler:
-            if scheduler.get_job(str(uid+"post_alock_morningclass")):
-                await add_alock_morningcalss.finish("出错了！你好像已经订阅过早八提醒了呢", at_sender=True)
-            scheduler.add_job(AiTimetable.post_alock_morningclass, "cron", hour=timetable_alock_8, second=random.randint(
-                0, 60), id=str(uid+"post_alock_morningclass"), kwargs={"uid": uid, "bot": bot, "event": event})
+            if scheduler.get_job(str(uid + "post_alock_morningclass")):
+                await add_alock_morningcalss.finish(
+                    "出错了！你好像已经订阅过早八提醒了呢", at_sender=True
+                )
+            scheduler.add_job(
+                AiTimetable.post_alock_morningclass,
+                "cron",
+                hour=config.timetable_alock_8,
+                second=random.randint(0, 60),
+                id=str(uid + "post_alock_morningclass"),
+                kwargs={"uid": uid, "bot": bot, "event": event},
+            )
             await add_alock_morningcalss.finish("定时提醒添加成功！", at_sender=True)
         else:
-            await add_alock_morningcalss.finish("apscheduler插件未载入,无法添加定时提醒", at_sender=True)
+            await add_alock_morningcalss.finish(
+                "apscheduler插件未载入,无法添加定时提醒", at_sender=True
+            )
 
 
 @remove_alock_morningclass.handle()
 async def _(event: MessageEvent):
     uid = event.get_user_id()
     if uid not in userdata:
-        await add_alock_morningcalss.finish('你还没有导入课表,发送/导入课表来导入吧！', at_sender=True)
+        await remove_alock_morningclass.finish("你还没有导入课表,发送/导入课表来导入吧！", at_sender=True)
     else:
         if scheduler:
-            if scheduler.get_job(str(uid+"post_alock_morningclass")):
-                scheduler.remove_job(str(uid+"post_alock_morningclass"))
+            if scheduler.get_job(str(uid + "post_alock_morningclass")):
+                scheduler.remove_job(str(uid + "post_alock_morningclass"))
                 await remove_alock_morningclass.finish("定时提醒删除成功！", at_sender=True)
             else:
                 await remove_alock_morningclass.finish("出错了,好像没有订阅过早八呢", at_sender=True)
         else:
-            await remove_alock_morningclass.finish("apscheduler插件未载入,无法删除定时提醒", at_sender=True)
+            await remove_alock_morningclass.finish(
+                "apscheduler插件未载入,无法删除定时提醒", at_sender=True
+            )
 
 
 @sub_class.handle()
-async def _(matcher:Matcher,args: Message = CommandArg()):
+async def _(matcher: Matcher, args: Message = CommandArg()):
     if args.extract_plain_text():
-        matcher.set_arg("text",args)
+        matcher.set_arg("text", args)
 
 
 @sub_class.got("text", prompt="请告诉我课程名~")
-async def sub_handler(bot: Bot, event: MessageEvent,text:str=ArgPlainText()):
+async def sub_handler(bot: Bot, event: MessageEvent, text: str = ArgPlainText()):
     uid = event.get_user_id()
     if uid not in userdata:
-        await sub_class.finish('你还没有导入课表,发送/导入课表来导入吧！', at_sender=True)
+        await sub_class.finish("你还没有导入课表,发送/导入课表来导入吧！", at_sender=True)
     else:
         if scheduler:
             msg = AiTimetable.sub_class(uid=uid, key=text, event=event, bot=bot)
             await sub_class.finish(msg, at_sender=True)
         else:
             await sub_class.finish("apscheduler插件未载入,无法添加定时提醒", at_sender=True)
 
 
 @remove_sub_class.handle()
-async def _(matcher:Matcher,args: Message = CommandArg()):
+async def _(matcher: Matcher, args: Message = CommandArg()):
     if args.extract_plain_text():
-        matcher.set_arg("text",args)
+        matcher.set_arg("text", args)
 
 
 @remove_sub_class.got("text", prompt="请告诉我课程名~")
-async def remove_sub_handler(event: MessageEvent,text:str=ArgPlainText()):
+async def remove_sub_handler(event: MessageEvent, text: str = ArgPlainText()):
     uid = event.get_user_id()
     if uid not in userdata:
-        await remove_sub_class.finish('你还没有导入课表,发送/导入课表来导入吧！', at_sender=True)
+        await remove_sub_class.finish("你还没有导入课表,发送/导入课表来导入吧！", at_sender=True)
     else:
         if scheduler:
             msg = AiTimetable.remove_sub_class(uid=uid, key=text)
             await remove_sub_class.finish(msg, at_sender=True)
         else:
             await remove_sub_class.finish("apscheduler插件未载入,无法添加定时提醒", at_sender=True)
```

### Comparing `nonebot_plugin_ai_timetable-0.3.3/nonebot_plugin_ai_timetable/utils.py` & `nonebot_plugin_ai_timetable-0.3.4/nonebot_plugin_ai_timetable/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,327 +1,500 @@
-from nonebot.adapters.onebot.v11 import ActionFailed,MessageSegment
+from nonebot.adapters.onebot.v11 import ActionFailed, MessageSegment
 from nonebot import get_driver, logger, require
-require('nonebot_plugin_htmlrender')
-require('nonebot_plugin_apscheduler')
+
+require("nonebot_plugin_htmlrender")
+require("nonebot_plugin_apscheduler")
 from nonebot_plugin_apscheduler import scheduler
 from nonebot_plugin_htmlrender import get_new_page, md_to_pic
 import os
 import re
 import json
 import time
 import datetime
 import httpx
 import random
+from .config import Config
 
-
-config = get_driver().config
-timetable_pic: bool = getattr(config, "timetable_pic", True)
-timetable_alock_someday: int = getattr(config, "timetable_alock_someday", 22)
-timetable_alock_8: int = getattr(config, "timetable_alock_8", 21)
-timetable_send_time:float=getattr(config,"timetable_send_time",0.5)
-
+global_config = get_driver().config
+config = Config.parse_obj(global_config)
 if os.path.exists("data/ai_timetable/userdata.json"):
-    with open("data/ai_timetable/userdata.json", 'r', encoding='utf-8') as f:
+    with open("data/ai_timetable/userdata.json", "r", encoding="utf-8") as f:
         userdata = json.load(f)
 else:
     if not os.path.exists("data/ai_timetable"):
         os.makedirs("data/ai_timetable")
     userdata = {}
-    with open("data/ai_timetable/userdata.json", 'w', encoding='utf-8') as f:
+    with open("data/ai_timetable/userdata.json", "w", encoding="utf-8") as f:
         json.dump(userdata, f)
-    
+
 if os.path.exists("data/ai_timetable/usertable.json"):
-    with open("data/ai_timetable/usertable.json", 'r', encoding='utf-8') as f:
+    with open("data/ai_timetable/usertable.json", "r", encoding="utf-8") as f:
         usertable = json.load(f)
 else:
     if not os.path.exists("data/ai_timetable"):
         os.makedirs("data/ai_timetable")
     usertable = {}
-    with open("data/ai_timetable/usertable.json", 'w', encoding='utf-8') as f:
+    with open("data/ai_timetable/usertable.json", "w", encoding="utf-8") as f:
         json.dump(usertable, f, ensure_ascii=False)
-        
-
 
 
 class AiTimetable:
-    res_url_re = r'^(https://i\.ai\.mi\.com/course-multi/table\?)*(ctId=)\d+(&userId=)\d*[1-9]\d*(&deviceId=)[0-9a-zA-Z]*(&sourceName=course-app-browser)'
-    base_url_re = r'https://cdn\.cnbj1\.fds\.api\.mi-img.com/miai-fe-aischedule-wx-redirect-fe/redirect.html\?linkToken=.+'
+    res_url_re = r"^(https://i\.ai\.mi\.com/course-multi/table\?)*(ctId=)\d+(&userId=)\d*[1-9]\d*(&deviceId=)[0-9a-zA-Z]*(&sourceName=course-app-browser)"
+    base_url_re = r"https://cdn\.cnbj1\.fds\.api\.mi-img.com/miai-fe-aischedule-wx-redirect-fe/redirect.html\?linkToken=.+"
 
     ai_timetable__usage = "## 小爱课表帮助:\n- 我的/本周课表: 获取本周课表,也可以是下周\n- 导入课表: 使用小爱课程表分享的链接一键导入\n- 某日课表: 获取某日课表,如今日课表、周一课表\n- 更新课表: 更新本地课表信息,如果线上修改过小爱课表,发送该指令即可更新本地课表\n- 订阅/取消订阅xx课表: 可以订阅某天(如周一)的课表,在前一天晚上10点推送\n- 订阅/取消订阅早八: 订阅所有早八,在前一天晚上发出提醒\n- 订阅/取消订阅课程+课程名：订阅某节课程\n- 上课/下节课: 获取当前课程信息以及今天以内的下节课信息\n- 早八|明日早八: 查询明天的早八"
 
     headers = {
-        'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/110.0.0.0 Safari/537.36 Edg/110.0.1587.63'
+        "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/110.0.0.0 Safari/537.36 Edg/110.0.1587.63"
     }
+
     def __init__(self, uid) -> None:
-        self.uid=uid
+        self.uid = uid
 
     @staticmethod
     def weekday_int(key) -> int:
         """中文日期转数字"""
-        cn2an = {'今': datetime.datetime.now().weekday()+1, '明': datetime.datetime.now().weekday()+2, '昨': datetime.datetime.now().weekday(),
-                '后': datetime.datetime.now().weekday()+3, '一': 1, '二': 2, '三': 3, '四': 4, '五': 5, '六': 6, '日': 7, '天': 7}
+        cn2an = {
+            "今": datetime.datetime.now().weekday() + 1,
+            "明": datetime.datetime.now().weekday() + 2,
+            "昨": datetime.datetime.now().weekday(),
+            "后": datetime.datetime.now().weekday() + 3,
+            "一": 1,
+            "二": 2,
+            "三": 3,
+            "四": 4,
+            "五": 5,
+            "六": 6,
+            "日": 7,
+            "天": 7,
+        }
         for i in cn2an:
             if i in key:
                 return cn2an[i]
         return 7
 
     @classmethod
     def next_class(cls, uid) -> str:
         """
         获得下节课程信息
         """
         now_time = datetime.datetime.now().strftime("%H:%M")
-        presentweek = int((time.time() - int(
-            usertable[uid]["data"]["setting"]['startSemester'][0:10]))//604800)+1
+        presentweek = (
+            int(
+                (
+                    time.time()
+                    - int(usertable[uid]["data"]["setting"]["startSemester"][0:10])
+                )
+                // 604800
+            )
+            + 1
+        )
         today = cls.weekday_int("今")
         for courses in usertable[uid]["data"]["courses"]:
             # 遍历当前天的所有存在的课
-            if str(presentweek) in courses["weeks"].split(",") and today == courses["day"]:
+            if (
+                str(presentweek) in courses["weeks"].split(",")
+                and today == courses["day"]
+            ):
                 next_class_section = int(courses["sections"].split(",")[0])
-                next_class_section_end = int(
-                    courses["sections"].split(",")[-1])
-                if eval(usertable[uid]["data"]["setting"]["sectionTimes"])[next_class_section-1]["s"] > now_time:
-                    return "\n你今天的下一节课程信息为：\n"+eval(usertable[uid]["data"]["setting"]["sectionTimes"])[next_class_section-1]["s"]+"-"+eval(usertable[uid]["data"]["setting"]["sectionTimes"])[next_class_section_end-1]["e"]+"\n"+courses["name"]+"\n@"+courses["position"]+"\n"+courses["teacher"]
-                #这里是因为之前已经按照顺序排好了课程,所以第一个找到的就是下节课
+                next_class_section_end = int(courses["sections"].split(",")[-1])
+                if (
+                    eval(usertable[uid]["data"]["setting"]["sectionTimes"])[
+                        next_class_section - 1
+                    ]["s"]
+                    > now_time
+                ):
+                    return (
+                        "\n你今天的下一节课程信息为：\n"
+                        + eval(usertable[uid]["data"]["setting"]["sectionTimes"])[
+                            next_class_section - 1
+                        ]["s"]
+                        + "-"
+                        + eval(usertable[uid]["data"]["setting"]["sectionTimes"])[
+                            next_class_section_end - 1
+                        ]["e"]
+                        + "\n"
+                        + courses["name"]
+                        + "\n@"
+                        + courses["position"]
+                        + "\n"
+                        + courses["teacher"]
+                    )
+                # 这里是因为之前已经按照顺序排好了课程,所以第一个找到的就是下节课
         return "\n你今天接下来没有课了呢,好好休息吧"
+
     @classmethod
     def now_class(cls, uid) -> str:
-        """ 
+        """
         构造出当前课程信息
         """
-        presentweek = int((time.time() - int(
-            usertable[uid]["data"]["setting"]['startSemester'][0:10]))//604800)+1
+        presentweek = (
+            int(
+                (
+                    time.time()
+                    - int(usertable[uid]["data"]["setting"]["startSemester"][0:10])
+                )
+                // 604800
+            )
+            + 1
+        )
         today = cls.weekday_int("今")
         now_section = 0
         now_time = datetime.datetime.now().strftime("%H:%M")
         msg = ""
         for course_time in eval(usertable[uid]["data"]["setting"]["sectionTimes"]):
             if course_time["s"] < now_time < course_time["e"]:
                 now_section = course_time["i"]
         if now_section:
             count = 0
             for courses in usertable[uid]["data"]["courses"]:
-                if (str(presentweek) in courses["weeks"].split(",")) and (today == courses["day"]) and (str(now_section) in courses["sections"].split(",")):
-                    msg += "\n你现在在上的课程信息如下:\n"+eval(usertable[uid]["data"]["setting"]["sectionTimes"])[int(courses["sections"].split(",")[0])-1]["s"]+"-"+eval(
-                        usertable[uid]["data"]["setting"]["sectionTimes"])[int(courses["sections"].split(",")[-1])-1]["e"]+'\n'+courses["name"]+"\n@"+courses["position"]+"\n"+courses["teacher"]
+                if (
+                    (str(presentweek) in courses["weeks"].split(","))
+                    and (today == courses["day"])
+                    and (str(now_section) in courses["sections"].split(","))
+                ):
+                    msg += (
+                        "\n你现在在上的课程信息如下:\n"
+                        + eval(usertable[uid]["data"]["setting"]["sectionTimes"])[
+                            int(courses["sections"].split(",")[0]) - 1
+                        ]["s"]
+                        + "-"
+                        + eval(usertable[uid]["data"]["setting"]["sectionTimes"])[
+                            int(courses["sections"].split(",")[-1]) - 1
+                        ]["e"]
+                        + "\n"
+                        + courses["name"]
+                        + "\n@"
+                        + courses["position"]
+                        + "\n"
+                        + courses["teacher"]
+                    )
                     count += 1
             if not count:
                 msg += "\n你现在没有课呢,空闲时间好好休息吧"
         else:
             msg += "\n你现在没有课呢,空闲时间好好休息吧"
         return msg
+
     @classmethod
     def table_msg(cls, key, uid) -> str:
         """
         构造今日课表信息
         """
-        presentweek = int((time.time() - int(
-            usertable[uid]["data"]["setting"]['startSemester'][0:10]))//604800)+1  # 这里算出的结果是小数,转换成整数
+        presentweek = (
+            int(
+                (
+                    time.time()
+                    - int(usertable[uid]["data"]["setting"]["startSemester"][0:10])
+                )
+                // 604800
+            )
+            + 1
+        )  # 这里算出的结果是小数,转换成整数
         someday = cls.weekday_int(key)
         # 日期变时周数也会变
         if someday < 0:
             someday += 7
             presentweek -= 1
         elif someday > 7:
             someday -= 7
             presentweek += 1
             # 构造发送的信息
-        if timetable_pic:
+        if config.timetable_pic:
             msg = "|时间|课程|地点|\n| :-----| :----: | :----: |"
         else:
             msg = "课表来了~"
         for courses in usertable[uid]["data"]["courses"]:
-            if(courses["day"] == someday) and (str(presentweek) in courses["weeks"].split(',')):
-
+            if (courses["day"] == someday) and (
+                str(presentweek) in courses["weeks"].split(",")
+            ):
                 sections = courses["sections"].split(",")
                 startsection = int(sections[0])
                 endsection = int(sections[-1])
                 starttime = eval(usertable[uid]["data"]["setting"]["sectionTimes"])[
-                    startsection-1]["s"]
+                    startsection - 1
+                ]["s"]
                 endtime = eval(usertable[uid]["data"]["setting"]["sectionTimes"])[
-                    endsection-1]["e"]
-                if timetable_pic:
-                    msg = msg+'\n'+'|'+starttime+'-'+endtime + \
-                        '|'+courses["name"]+'|'+courses["position"]
+                    endsection - 1
+                ]["e"]
+                if config.timetable_pic:
+                    msg = (
+                        msg
+                        + "\n"
+                        + "|"
+                        + starttime
+                        + "-"
+                        + endtime
+                        + "|"
+                        + courses["name"]
+                        + "|"
+                        + courses["position"]
+                    )
 
                 else:
-                    msg = msg+'\n'+starttime+'-'+endtime+'\n' + \
-                        courses["name"]+"\n@"+courses["position"]+'\n'
+                    msg = (
+                        msg
+                        + "\n"
+                        + starttime
+                        + "-"
+                        + endtime
+                        + "\n"
+                        + courses["name"]
+                        + "\n@"
+                        + courses["position"]
+                        + "\n"
+                    )
         return msg
 
     @staticmethod
     async def my_table(uid, key):
         """
         获取本周或者下周课表
         """
         try:
             async with get_new_page(viewport={"width": 1000, "height": 1000}) as page:
-                await page.goto(userdata[uid][0],wait_until="networkidle")
+                await page.goto(userdata[uid][0], wait_until="networkidle")
                 # 这里使小爱课程表的导入按钮隐藏,防止遮挡课表
-                await page.evaluate('var t = document.querySelector("#root>div>div.importSchedule___UjEKt>div.footer___1iAis.toUp___2mciB"); t.style.display = "none"')
-                if '下' in key:  # 如果命令中有下字,就点击下一周的按钮
-                    await page.click("#schedule-view > div.header___26sI1 > div.presentWeek___-o65e > div.rightBtn___2ZhSY")
-                pic = await page.screenshot(full_page=True,type="jpeg",quality=70)
+                await page.evaluate(
+                    'var t = document.querySelector("#root>div>div.importSchedule___UjEKt>div.footer___1iAis.toUp___2mciB"); t.style.display = "none"'
+                )
+                if "下" in key:  # 如果命令中有下字,就点击下一周的按钮
+                    await page.click(
+                        "#schedule-view > div.header___26sI1 > div.presentWeek___-o65e > div.rightBtn___2ZhSY"
+                    )
+                pic = await page.screenshot(full_page=True, type="jpeg", quality=70)
                 return pic
         except Exception as e:
             logger.warning(f"获取课表时出错：{e}")
+
     @classmethod
-    async def response_listener(cls,base_url, uid, response):
-        """监听请求"""  
-        if re.match(cls.res_url_re,response.url):
-                userdata.update({uid:(base_url,response.url)})
+    async def response_listener(cls, base_url, uid, response):
+        """监听请求"""
+        if re.match(cls.res_url_re, response.url):
+            userdata.update({uid: (base_url, response.url)})
+
     @staticmethod
     async def write_data() -> None:
         """写入用户数据"""
-        with open("data/ai_timetable/userdata.json", 'w', encoding='utf-8') as f:
+        with open("data/ai_timetable/userdata.json", "w", encoding="utf-8") as f:
             json.dump(userdata, f)
 
     @staticmethod
     async def write_table() -> None:
         """写入用户课表"""
-        with open("data/ai_timetable/usertable.json", 'w', encoding='utf-8') as f:
+        with open("data/ai_timetable/usertable.json", "w", encoding="utf-8") as f:
             json.dump(usertable, f, ensure_ascii=False)
+
     @classmethod
-    async def new_table(cls,uid,base_url)->str:
+    async def new_table(cls, uid, base_url) -> str:
         """更新课表"""
         try:
             async with get_new_page(viewport={"width": 1000, "height": 1200}) as page:
-                page.on("response", lambda response: cls.response_listener(response=response,uid=uid,base_url=base_url))
-                await page.goto(url=base_url,wait_until="networkidle")
+                page.on(
+                    "response",
+                    lambda response: cls.response_listener(
+                        response=response, uid=uid, base_url=base_url
+                    ),
+                )
+                await page.goto(url=base_url, wait_until="networkidle")
                 if uid in userdata:
                     async with httpx.AsyncClient() as client:
-                        res=await client.get(userdata[uid][1],headers=cls.headers)
-                        usertable.update({uid:res.json()})
-                        #更新课表
+                        res = await client.get(userdata[uid][1], headers=cls.headers)
+                        usertable.update({uid: res.json()})
+                        # 更新课表
                         usertable[uid]["data"]["courses"].sort(
-                    key=lambda x: int(x["sections"].split(",")[0]))
-                        #对课表排序
+                            key=lambda x: int(x["sections"].split(",")[0])
+                        )
+                        # 对课表排序
                         await cls.write_table()
                         await cls.write_data()
                         return "成功导入课表！"
                 else:
                     return "出错了，可能是没有在小爱课表内登录账户"
         except Exception as e:
             logger.warning(f"获取课表时出错：{e}")
             return f"出错了：{e}"
-            
+
     @classmethod
-    async def renew_table(cls,uid):
+    async def renew_table(cls, uid):
         """
         用户已有url的情况下更新本地课表
         """
         try:
             async with httpx.AsyncClient() as client:
-                res=await client.get(userdata[uid][1],headers=cls.headers)
-                usertable.update({uid:res.json()})
-                        #更新课表
+                res = await client.get(userdata[uid][1], headers=cls.headers)
+                usertable.update({uid: res.json()})
+                # 更新课表
                 usertable[uid]["data"]["courses"].sort(
-                    key=lambda x: int(x["sections"].split(",")[0]))
-                        #对课表排序
+                    key=lambda x: int(x["sections"].split(",")[0])
+                )
+                # 对课表排序
                 await cls.write_table()
                 await cls.write_data()
                 return "更新成功"
         except Exception as e:
             return f"{e}"
 
     @classmethod
-    async def someday_table(cls,uid,key): 
+    async def someday_table(cls, uid, key):
         """某天的课表"""
         try:
-            msg=cls.table_msg(uid=uid,key=key)
-            if not timetable_pic:
+            msg = cls.table_msg(uid=uid, key=key)
+            if not config.timetable_pic:
                 return msg
             else:
-                pic=await md_to_pic(md=msg)
+                pic = await md_to_pic(md=msg)
                 return pic
         except Exception as e:
             logger.warning(f"出错了，出错原因：{e}")
+
     @classmethod
-    async def post_alock_morningclass(cls,**kwargs):
+    async def post_alock_morningclass(cls, **kwargs):
         """发送早八消息"""
-        uid,bot,event=kwargs["uid"],kwargs["bot"],kwargs["event"]
+        uid, bot, event = kwargs["uid"], kwargs["bot"], kwargs["event"]
         try:
-            someday=cls.weekday_int("明")
-            someweek=int((time.time() - int(
-                usertable[uid]["data"]["setting"]['startSemester'][0:10]))//604800)
-            if someday==8:#星期天发送时时第二天是星期一,周数加1
-                someday=1
-                someweek=someweek+1  
-            count=0
-            msg = "现在时间是"+datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
+            someday = cls.weekday_int("明")
+            someweek = int(
+                (
+                    time.time()
+                    - int(usertable[uid]["data"]["setting"]["startSemester"][0:10])
+                )
+                // 604800
+            )
+            if someday == 8:  # 星期天发送时时第二天是星期一,周数加1
+                someday = 1
+                someweek = someweek + 1
+            count = 0
+            msg = "现在时间是" + datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
             for courses in usertable[uid]["data"]["courses"]:
-                if (courses["day"] == someday) and str(someweek) in courses["weeks"].split(",") and "1" in courses["sections"].split(","):
-                    count+=1
-                    msg+='\n'+courses["name"] + '\n@' + courses["position"]+'\n'+courses["teacher"]
-            if count==0:
-                msg+="\n你明天没有早八呢！享受夜生活吧！"
+                if (
+                    (courses["day"] == someday)
+                    and str(someweek) in courses["weeks"].split(",")
+                    and "1" in courses["sections"].split(",")
+                ):
+                    count += 1
+                    msg += (
+                        "\n"
+                        + courses["name"]
+                        + "\n@"
+                        + courses["position"]
+                        + "\n"
+                        + courses["teacher"]
+                    )
+            if count == 0:
+                msg += "\n你明天没有早八呢！享受夜生活吧！"
             else:
-                msg+=f"\n你明天有{count}节早八呢！今晚早点休息吧！"
-            await bot.send(event,message=msg,at_sender=True)
+                msg += f"\n你明天有{count}节早八呢！今晚早点休息吧！"
+            await bot.send(event, message=msg, at_sender=True)
         except ActionFailed as e:
             logger.warning(f"发送消息给{event.get_user_id()}失败：{e}")
+
     @classmethod
-    async def post_alock(cls,**kwargs):
+    async def post_alock(cls, **kwargs):
         """发送第二天课程消息"""
-        key,uid,bot,event=kwargs["key"],kwargs["uid"],kwargs["bot"],kwargs["event"]
+        key, uid, bot, event = (
+            kwargs["key"],
+            kwargs["uid"],
+            kwargs["bot"],
+            kwargs["event"],
+        )
         if "一" in key:
-            key="明"
-        msg=cls.table_msg(key=key,uid=uid)
+            key = "明"
+        msg = cls.table_msg(key=key, uid=uid)
         try:
-            if timetable_pic:
-                pic=await md_to_pic(md=msg)
-                await bot.send(event,MessageSegment.image(file=pic),at_sender=True)
+            if config.timetable_pic:
+                pic = await md_to_pic(md=msg)
+                await bot.send(event, MessageSegment.image(file=pic), at_sender=True)
             else:
-                await bot.send(event,message=msg,at_sender=True)
+                await bot.send(event, message=msg, at_sender=True)
         except ActionFailed as e:
             logger.warning(f"发送消息失败：{e}")
-            
+
     @classmethod
-    def sub_class(cls,**kwargs)->str:
+    def sub_class(cls, **kwargs) -> str:
         """订阅一周内所有课程名中有key的课程"""
-        uid,key,bot,event=kwargs["uid"],kwargs["key"],kwargs["bot"],kwargs["event"]
-        i=0
+        uid, key, bot, event = (
+            kwargs["uid"],
+            kwargs["key"],
+            kwargs["bot"],
+            kwargs["event"],
+        )
+        i = 0
         for courses in usertable[uid]["data"]["courses"]:
             # 遍历当前天的所有存在的课
             if key in courses["name"]:
-                i+=1
-                if scheduler.get_job(job_id=uid+courses["name"]+str(i)):
+                i += 1
+                if scheduler.get_job(job_id=uid + courses["name"] + str(i)):
                     continue
                 else:
                     class_section = int(courses["sections"].split(",")[0])
-                    starttime = eval(usertable[uid]["data"]["setting"]["sectionTimes"])[class_section-1]["s"]#获取课程开始时间
-                    hours = int(timetable_send_time)#从设置中获取提前的小时数
-                    minutes = int((timetable_send_time - hours) * 60)#从设置中获取提前的分钟数
-                    time_obj = datetime.datetime.strptime(starttime, "%H:%M")#将字符串转换为datetime
-                    new_time_obj = time_obj - datetime.timedelta(hours=hours, minutes=minutes)#进行时间的运算
-                    sub_hour=new_time_obj.hour#获取发送时间的小时
-                    sub_minute=new_time_obj.minute#获取发送时间的分钟
-                    sub_day=courses["day"]-1
-                    scheduler.add_job(cls.send_sub_class,"cron",id=uid+courses["name"]+str(i), hour=sub_hour, minute=sub_minute, day_of_week=sub_day, second=random.randint(0, 60),kwargs={"uid": uid, "bot": bot, "event": event,"course":{"name":courses["name"],"position":courses["position"],"teacher":courses["teacher"]}})
+                    starttime = eval(usertable[uid]["data"]["setting"]["sectionTimes"])[
+                        class_section - 1
+                    ][
+                        "s"
+                    ]  # 获取课程开始时间
+                    hours = int(config.timetable_send_time)  # 从设置中获取提前的小时数
+                    minutes = int((config.timetable_send_time - hours) * 60)  # 从设置中获取提前的分钟数
+                    time_obj = datetime.datetime.strptime(
+                        starttime, "%H:%M"
+                    )  # 将字符串转换为datetime
+                    new_time_obj = time_obj - datetime.timedelta(
+                        hours=hours, minutes=minutes
+                    )  # 进行时间的运算
+                    sub_hour = new_time_obj.hour  # 获取发送时间的小时
+                    sub_minute = new_time_obj.minute  # 获取发送时间的分钟
+                    sub_day = courses["day"] - 1
+                    scheduler.add_job(
+                        cls.send_sub_class,
+                        "cron",
+                        id=uid + courses["name"] + str(i),
+                        hour=sub_hour,
+                        minute=sub_minute,
+                        day_of_week=sub_day,
+                        second=random.randint(0, 60),
+                        kwargs={
+                            "uid": uid,
+                            "bot": bot,
+                            "event": event,
+                            "course": {
+                                "name": courses["name"],
+                                "position": courses["position"],
+                                "teacher": courses["teacher"],
+                            },
+                        },
+                    )
         return f"成功订阅了{i}节课~"
-    
+
     @classmethod
-    def remove_sub_class(cls,**kwargs):
-        uid,key=kwargs["uid"],kwargs["key"]
-        i=0
+    def remove_sub_class(cls, **kwargs):
+        uid, key = kwargs["uid"], kwargs["key"]
+        i = 0
         for courses in usertable[uid]["data"]["courses"]:
             # 遍历当前天的所有存在的课
             if key in courses["name"]:
-                i+=1
-                if scheduler.get_job(job_id=uid+courses["name"]+str(i)):
-                    scheduler.remove_job(job_id=uid+courses["name"]+str(i))
+                i += 1
+                if scheduler.get_job(job_id=uid + courses["name"] + str(i)):
+                    scheduler.remove_job(job_id=uid + courses["name"] + str(i))
                 else:
                     continue
         return f"成功取消订阅{i}节课~"
+
     @classmethod
-    async def send_sub_class(cls,**kwargs):
+    async def send_sub_class(cls, **kwargs):
         """发送订阅课程"""
-        uid,bot,event,course=kwargs["uid"],kwargs["bot"],kwargs["event"],kwargs["course"]
+        uid, bot, event, course = (
+            kwargs["uid"],
+            kwargs["bot"],
+            kwargs["event"],
+            kwargs["course"],
+        )
         try:
-            msg = "现在时间是"+datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
-            msg+="\n还有{}小时，你订阅的课程就要开始啦！课程信息如下:\n{}\n{}\n{}".format(timetable_send_time,course["name"],course["position"],course["teacher"])
-            await bot.send(event, message=MessageSegment.at(uid)+msg, at_sender=True)
+            msg = "现在时间是" + datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
+            msg += "\n还有{}小时，你订阅的课程就要开始啦！课程信息如下:\n{}\n{}\n{}".format(
+                config.timetable_send_time,
+                course["name"],
+                course["position"],
+                course["teacher"],
+            )
+            await bot.send(event, message=MessageSegment.at(uid) + msg, at_sender=True)
         except ActionFailed as e:
             logger.warning(f"发送消息给{event.get_user_id()}失败：{e}")
-        
-        
-
```

### Comparing `nonebot_plugin_ai_timetable-0.3.3/PKG-INFO` & `nonebot_plugin_ai_timetable-0.3.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,28 @@
-Metadata-Version: 2.1
-Name: nonebot-plugin-ai-timetable
-Version: 0.3.3
-Summary: 小爱课程表
-Author: maoxiog
-Author-email: 674550338@qq.com
-Requires-Python: >=3.8,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: httpx (>=0.23.0,<0.24.0)
-Requires-Dist: nonebot-adapter-onebot (>=2.1.0,<3.0.0)
-Requires-Dist: nonebot-plugin-apscheduler (>=0.2.0,<0.3.0)
-Requires-Dist: nonebot-plugin-htmlrender (>=0.2.0,<0.3.0)
-Requires-Dist: nonebot2 (>=2.0.0rc1,<3.0.0)
-Description-Content-Type: text/markdown
-
 <p align="center">
   <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
 </p>
 <div align="center">
 
 # nonebot-plugin-ai-timetable
 
 ✨*基于Nonebot2的对接小爱课程表的插件*✨
   
-<div align="left">
-  
-# 前言
+<a href="https://github.com/nonebot/nonebot2">
+  <img src="https://img.shields.io/badge/nonebot-v2-red" alt="nonebot">
+</a> 
+<a href="./LICENSE">
+    <img src="https://img.shields.io/github/license/maoxig/nonebot-plugin-ai-timetable" alt="license">
+</a>
+<a href="https://pypi.python.org/pypi/nonebot-plugin-ai-timetable">
+    <img src="https://img.shields.io/pypi/v/nonebot-plugin-ai-timetable" alt="pypi">
+</a>
+<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
 
-   这是本人第一次在github发布的项目，也是第一个python项目，完全是萌新，很多地方写的可能很拉，大佬轻喷
-目前还不是很完善，有什么bug或者建议欢迎提issues
+<div align="left">
 
 ## 💿安装
 
 1. 通过`pip`或`nb`安装；
     - 使用nb(极度推荐)
   
        在机器人目录下命令行使用`nb plugin install nonebot_plugin_ai_timetable`
@@ -54,20 +41,20 @@
 
 3. ~~所以为什么不直接用小爱课表呢~~
 
 4. ⚙️插件配置
 
 这些配置都已设好默认值，如果想要修改配置，在机器人目录下的.env.*里面可以填写以下选项(可选)
 
-|         config          | type  | default |          example           | usage                                                                              |
-| :---------------------: | :---: | :-----: | :------------------------: | :--------------------------------------------------------------------------------- |
-|      TIMETABLE_PIC      | bool  |  true   |    TIMETABLE_PIC=false     | 可选择某日课表以图片/文字发送，默认以图片发送(true)                                |
-| TIMETABLE_ALOCK_SOMEDAY |  int  |   22    | TIMETABLE_ALOCK_SOMEDAY=15 | 订阅某日课表的发送时间，必须是0-24的数字                                           |
-|    TIMETABLE_ALOCK_8    |  int  |   21    |    TIMETABLE_ALOCK_8=16    | 订阅早八的发送时间，必须是0-24的数字.这里发送的都是第二天的，所以建议设置为18-23点 |
-|    TIMETABLE_SEND_TIME    |  float  |   0.5    |    TIMETABLE_SEND_TIME=1    | 订阅课程提前发送的时间，单位是`小时`，可以是整数也可以是小数，建议不要设的太大，避免出现无法预料的bug |
+|         config          | type  | default |          example           | usage                                                                                                 |
+| :---------------------: | :---: | :-----: | :------------------------: | :---------------------------------------------------------------------------------------------------- |
+|      TIMETABLE_PIC      | bool  |  true   |    TIMETABLE_PIC=false     | 可选择某日课表以图片/文字发送，默认以图片发送(true)                                                   |
+| TIMETABLE_ALOCK_SOMEDAY |  int  |   22    | TIMETABLE_ALOCK_SOMEDAY=15 | 订阅某日课表的发送时间，必须是0-24的数字                                                              |
+|    TIMETABLE_ALOCK_8    |  int  |   21    |    TIMETABLE_ALOCK_8=16    | 订阅早八的发送时间，必须是0-24的数字.这里发送的都是第二天的，所以建议设置为18-23点                    |
+|   TIMETABLE_SEND_TIME   | float |   0.5   |   TIMETABLE_SEND_TIME=1    | 订阅课程提前发送的时间，单位是`小时`，可以是整数也可以是小数，建议不要设的太大，避免出现无法预料的bug |
 
 ## 💿依赖
 
 ```python
 nb plugin install nonebot_plugin_htmlrender
 nb plugin install nonebot_plugin_apscheduler
 ```
@@ -129,14 +116,20 @@
 2. 删去了文本中所有奇怪的口癖喵
 
 - 2023-04-23:
 
 1. 修改帮助
 2. 修复定时提醒重复发送的bug
 
+- 2023-06-09:
+
+1. 更新插件元数据
+2. 优化配置读取
+3. 格式化代码
+
 </details>
 
 ## 🎉命令
 
 1. 我的课表|小爱课表|本周课表|下周课表：获取本周|下周的完全课表，使用前须先导入课表，这里的课表是在线课表
 
 2. 导入课表：需要有小爱课表分享出来的链接，打开小爱课程表，手动添加课程或从教务导入(已适配了大部分高校)课程后
@@ -193,17 +186,18 @@
 
 - [x] 增加更多的配置项
 
 - [x] 重构代码
 
 - [x] 订阅指定的课
 
+- [ ] 适配插件datastore，接入数据库
+
 - [ ] 完善插件
 
 ## 🐛存在的问题
 
  1. 小爱课表分享的链接大概2周后会过期，会使得`我的课表\下周课表`无法使用，需要重新分享，但是仍能使用本地课表，也可以更新本地课表
 
  2. 机器人重启后定时任务会丢失
 
 ## 喜欢的话就点个star✨吧QAQ
-
```

#### html2text {}

```diff
@@ -1,40 +1,28 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-ai-timetable Version: 0.3.3 Summary:
-å°ç±è¯¾ç¨è¡¨ Author: maoxiog Author-email: 674550338@qq.com Requires-Python:
->=3.8,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Requires-Dist: httpx (>=0.23.0,<0.24.0)
-Requires-Dist: nonebot-adapter-onebot (>=2.1.0,<3.0.0) Requires-Dist: nonebot-
-plugin-apscheduler (>=0.2.0,<0.3.0) Requires-Dist: nonebot-plugin-htmlrender
-(>=0.2.0,<0.3.0) Requires-Dist: nonebot2 (>=2.0.0rc1,<3.0.0) Description-
-Content-Type: text/markdown
                                    [nonebot]
                          # nonebot-plugin-ai-timetable
-            â¨*åºäºNonebot2çå¯¹æ¥å°ç±è¯¾ç¨è¡¨çæä»¶*â¨
-# åè¨
-è¿æ¯æ¬äººç¬¬ä¸æ¬¡å¨githubåå¸çé¡¹ç®ï¼ä¹æ¯ç¬¬ä¸ä¸ªpythoné¡¹ç®ï¼å®å¨æ¯èæ°ï¼å¾å¤å°æ¹åçå¯è½å¾æï¼å¤§ä½¬è½»å·
-ç®åè¿ä¸æ¯å¾å®åï¼æä»ä¹bugæèå»ºè®®æ¬¢è¿æissues ##
-ð¿å®è£ 1. éè¿`pip`æ`nb`å®è£ï¼ - ä½¿ç¨nb(æåº¦æ¨è)
+ â¨*åºäºNonebot2çå¯¹æ¥å°ç±è¯¾ç¨è¡¨çæä»¶*â¨ [nonebot] [license]
+                                [pypi] [python]
+## ð¿å®è£ 1. éè¿`pip`æ`nb`å®è£ï¼ - ä½¿ç¨nb(æåº¦æ¨è)
 å¨æºå¨äººç®å½ä¸å½ä»¤è¡ä½¿ç¨`nb plugin install
 nonebot_plugin_ai_timetable` - ä½¿ç¨pip(ä¸æ¨è):
 ~~æ¢ç¶ä¸æ¨èå°±ä¸è¦æ³çè¿æ ·å®è£äºåå~~ 2.
 æ¬å°æ°æ®ä¿å­å¨`data/ai_timetable/userdata.json`ä»¥å`data/ai_timetable/
 usertable.json`ï¼åå«å¯¹åºç¨æ·åéçé¾æ¥åæ¬å°ä¿å­çè¯¾è¡¨ ##
 ðç®ä» 1.
 å»çå¼ä¸é®å¯¼å¥å°ç±è¯¾è¡¨ï¼è®©ä½ çbotå®ç°å°ç±è¯¾è¡¨çåè½ 2.
 ç¨æ·è¯¾è¡¨æ°æ®éç¦»ï¼æ éæå¿è¯¾ç¨æ¶é´å²çªãä¸åå­¦æ ¡è¯¾è¡¨ä¸åç­é®é¢
 3. ~~æä»¥ä¸ºä»ä¹ä¸ç´æ¥ç¨å°ç±è¯¾è¡¨å¢~~ 4. âï¸æä»¶éç½®
 è¿äºéç½®é½å·²è®¾å¥½é»è®¤å¼ï¼å¦ææ³è¦ä¿®æ¹éç½®ï¼å¨æºå¨äººç®å½ä¸ç.env.*éé¢å¯ä»¥å¡«åä»¥ä¸éé¡¹
 (å¯é) | config | type | default | example | usage | | :--------------------
 -: | :---: | :-----: | :------------------------: | :--------------------------
-------------------------------------------------------- | | TIMETABLE_PIC |
-bool | true | TIMETABLE_PIC=false | å¯éæ©ææ¥è¯¾è¡¨ä»¥å¾ç/
-æå­åéï¼é»è®¤ä»¥å¾çåé(true) | | TIMETABLE_ALOCK_SOMEDAY | int |
-22 | TIMETABLE_ALOCK_SOMEDAY=15 |
+-------------------------------------------------------------------------- | |
+TIMETABLE_PIC | bool | true | TIMETABLE_PIC=false |
+å¯éæ©ææ¥è¯¾è¡¨ä»¥å¾ç/æå­åéï¼é»è®¤ä»¥å¾çåé(true) | |
+TIMETABLE_ALOCK_SOMEDAY | int | 22 | TIMETABLE_ALOCK_SOMEDAY=15 |
 è®¢éææ¥è¯¾è¡¨çåéæ¶é´ï¼å¿é¡»æ¯0-24çæ°å­ | |
 TIMETABLE_ALOCK_8 | int | 21 | TIMETABLE_ALOCK_8=16 |
 è®¢éæ©å«çåéæ¶é´ï¼å¿é¡»æ¯0-
 24çæ°å­.è¿éåéçé½æ¯ç¬¬äºå¤©çï¼æä»¥å»ºè®®è®¾ç½®ä¸º18-23ç¹ |
 | TIMETABLE_SEND_TIME | float | 0.5 | TIMETABLE_SEND_TIME=1 |
 è®¢éè¯¾ç¨æååéçæ¶é´ï¼åä½æ¯`å°æ¶`ï¼å¯ä»¥æ¯æ´æ°ä¹å¯ä»¥æ¯å°æ°ï¼å»ºè®®ä¸è¦è®¾çå¤ªå¤§ï¼é¿ååºç°æ æ³é¢æçbug
 | ## ð¿ä¾èµ ```python nb plugin install nonebot_plugin_htmlrender nb plugin
@@ -58,15 +46,16 @@
 éæäºä»£ç ï¼ä¼åäºè®¸å¤å°æ¹~~ççç´¯æ­»äº~~ 2.
 ä¿®å¤äºä¸äºbugï¼ä¼åäºä½éª 3. å¢å äºæ©å«|ææ¥æ©å«çæ¥è¯¢
 4. æ´æ°çæ¬åå»ºè®®éæ°`å¯¼å¥è¯¾è¡¨`ï¼é¿ååºç°æäºbug - 2023-04-
 02: 1. ä¿®å¤bug 2. ä¼åå¸®å©å¾ç 3. å®æ¶ä»»å¡éæºå»¶å0-
 60sï¼é²æ­¢é£æ§ 4. å¢å è®¢éæå®è¯¾ç¨çåè½ - 2023-04-14: 1.
 ä¿®å¤äºè®¢éè¯¾ç¨åéæ¶é´éè¯¯çbug 2.
 å å»äºææ¬ä¸­ææå¥æªçå£çåµ - 2023-04-23: 1. ä¿®æ¹å¸®å© 2.
-ä¿®å¤å®æ¶æééå¤åéçbug  ## ðå½ä»¤ 1.
+ä¿®å¤å®æ¶æééå¤åéçbug - 2023-06-09: 1. æ´æ°æä»¶åæ°æ® 2.
+ä¼åéç½®è¯»å 3. æ ¼å¼åä»£ç   ## ðå½ä»¤ 1.
 æçè¯¾è¡¨|å°ç±è¯¾è¡¨|æ¬å¨è¯¾è¡¨|ä¸å¨è¯¾è¡¨ï¼è·åæ¬å¨|ä¸å¨çå®å¨è¯¾è¡¨ï¼ä½¿ç¨åé¡»åå¯¼å¥è¯¾è¡¨ï¼è¿éçè¯¾è¡¨æ¯å¨çº¿è¯¾è¡¨
 2.
 å¯¼å¥è¯¾è¡¨ï¼éè¦æå°ç±è¯¾è¡¨åäº«åºæ¥çé¾æ¥ï¼æå¼å°ç±è¯¾ç¨è¡¨ï¼æå¨æ·»å è¯¾ç¨æä»æå¡å¯¼å¥
 (å·²ééäºå¤§é¨åé«æ ¡)è¯¾ç¨å ![Image text](https://github.com/maoxig/
 nonebot-plugin-ai-timetable/blob/main/resource/export.jpg)
 å¨åºæ¬è®¾ç½®éæå¼å§ä¸è¯¾æ¶é´ç­è°æ´å¥½ä¹å
 (å°¤å¶æ¯æ¶é´ãèæ°)ï¼æåäº«è¯¾è¡¨å¾å°çé¾æ¥åéç»botå³å¯å¯¼å¥æ¬å°
@@ -105,12 +94,13 @@
 -
 å¦æå¯¼å¥è¯¾è¡¨åå¨å°ç±è¯¾è¡¨åä¿®æ¹äºè¯¾ç¨ï¼ç´æ¥ç»botåéæ´æ°è¯¾è¡¨å³å¯æ´æ°æ¬å°è¯¾è¡¨
 -
 å½ä½ ä¸»é¡µçè¯¾è¡¨åå­¦æ ¡è¯¾è¡¨åºæ¬ä¸è´æ¶ï¼é£ä¹å°ç±è¯¾ç¨è¡¨å°±è¢«è°æå¥½äºï¼å¯ä»¥å¯¼å¥äº
 ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/
 resource/settings.jpg) ## ð¦è®¡å - [x] æ¥è¯¢ä¸èè¯¾çä¿¡æ¯ - [x]
 å¯éæ©æ¯å¦åéå¾çä»¥é¿åé£æ§ - [x] å¢å æ´å¤çéç½®é¡¹ - [x]
-éæä»£ç  - [x] è®¢éæå®çè¯¾ - [ ] å®åæä»¶ ## ðå­å¨çé®é¢
-1.
+éæä»£ç  - [x] è®¢éæå®çè¯¾ - [ ]
+ééæä»¶datastoreï¼æ¥å¥æ°æ®åº - [ ] å®åæä»¶ ##
+ðå­å¨çé®é¢ 1.
 å°ç±è¯¾è¡¨åäº«çé¾æ¥å¤§æ¦2å¨åä¼è¿æï¼ä¼ä½¿å¾`æçè¯¾è¡¨\ä¸å¨è¯¾è¡¨`æ æ³ä½¿ç¨ï¼éè¦éæ°åäº«ï¼ä½æ¯ä»è½ä½¿ç¨æ¬å°è¯¾è¡¨ï¼ä¹å¯ä»¥æ´æ°æ¬å°è¯¾è¡¨
 2. æºå¨äººéå¯åå®æ¶ä»»å¡ä¼ä¸¢å¤± ##
 åæ¬¢çè¯å°±ç¹ä¸ªstarâ¨å§QAQ
```

