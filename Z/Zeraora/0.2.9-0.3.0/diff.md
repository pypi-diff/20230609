# Comparing `tmp/Zeraora-0.2.9.tar.gz` & `tmp/Zeraora-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Zeraora-0.2.9.tar", last modified: Sun May 14 17:06:30 2023, max compression
+gzip compressed data, was "dist/Zeraora-0.3.0.tar", last modified: Fri Jun  9 03:01:13 2023, max compression
```

## Comparing `Zeraora-0.2.9.tar` & `Zeraora-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:06:30.000000 Zeraora-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-05-14 17:06:30.000000 Zeraora-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-05-14 17:06:17.000000 Zeraora-0.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:06:30.000000 Zeraora-0.2.9/Zeraora.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-05-14 17:06:30.000000 Zeraora-0.2.9/Zeraora.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-14 17:06:30.000000 Zeraora-0.2.9/Zeraora.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 17:06:30.000000 Zeraora-0.2.9/Zeraora.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-14 17:06:30.000000 Zeraora-0.2.9/Zeraora.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 17:06:30.000000 Zeraora-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-14 17:06:17.000000 Zeraora-0.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:06:30.000000 Zeraora-0.2.9/zeraora/
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-14 17:06:17.000000 Zeraora-0.2.9/zeraora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-14 17:06:17.000000 Zeraora-0.2.9/zeraora/charsets.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-14 17:06:17.000000 Zeraora-0.2.9/zeraora/checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-05-14 17:06:17.000000 Zeraora-0.2.9/zeraora/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-05-14 17:06:17.000000 Zeraora-0.2.9/zeraora/divisions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:06:30.000000 Zeraora-0.2.9/zeraora/djangobase/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-14 17:06:17.000000 Zeraora-0.2.9/zeraora/djangobase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-05-14 17:06:17.000000 Zeraora-0.2.9/zeraora/djangobase/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-05-14 17:06:17.000000 Zeraora-0.2.9/zeraora/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-05-14 17:06:17.000000 Zeraora-0.2.9/zeraora/typeclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-05-14 17:06:17.000000 Zeraora-0.2.9/zeraora/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:01:13.000000 Zeraora-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-06-09 03:01:13.000000 Zeraora-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-09 03:00:58.000000 Zeraora-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:01:13.000000 Zeraora-0.3.0/Zeraora.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-06-09 03:01:13.000000 Zeraora-0.3.0/Zeraora.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-09 03:01:13.000000 Zeraora-0.3.0/Zeraora.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 03:01:13.000000 Zeraora-0.3.0/Zeraora.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-09 03:01:13.000000 Zeraora-0.3.0/Zeraora.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 03:01:13.000000 Zeraora-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-09 03:00:58.000000 Zeraora-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:01:13.000000 Zeraora-0.3.0/zeraora/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-09 03:00:58.000000 Zeraora-0.3.0/zeraora/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:01:13.000000 Zeraora-0.3.0/zeraora/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-09 03:00:58.000000 Zeraora-0.3.0/zeraora/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-09 03:00:58.000000 Zeraora-0.3.0/zeraora/constants/charsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-09 03:00:58.000000 Zeraora-0.3.0/zeraora/constants/division.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-06-09 03:00:58.000000 Zeraora-0.3.0/zeraora/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:01:13.000000 Zeraora-0.3.0/zeraora/dj/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-09 03:00:58.000000 Zeraora-0.3.0/zeraora/dj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-06-09 03:00:58.000000 Zeraora-0.3.0/zeraora/dj/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:01:13.000000 Zeraora-0.3.0/zeraora/drf/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-09 03:00:58.000000 Zeraora-0.3.0/zeraora/drf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-06-09 03:00:58.000000 Zeraora-0.3.0/zeraora/drf/viewsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-06-09 03:00:58.000000 Zeraora-0.3.0/zeraora/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12256 2023-06-09 03:00:58.000000 Zeraora-0.3.0/zeraora/typeclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12159 2023-06-09 03:00:58.000000 Zeraora-0.3.0/zeraora/utils.py
```

### Comparing `Zeraora-0.2.9/PKG-INFO` & `Zeraora-0.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 Metadata-Version: 2.1
 Name: Zeraora
-Version: 0.2.9
-Summary: 一个包含原创工具类及快捷函数的工具库。A original utility Python package.
+Version: 0.3.0
+Summary: 一个长期维护的个人开源工具库。A utility Python package supports for my personal and company projects.
 Home-page: https://github.com/aixcyi/zeraora
 Author: aixcyi
 Author-email: 75880483+aixcyi@users.noreply.github.com
 License: MIT
 Project-URL: Source, https://github.com/aixcyi/zeraora
 Project-URL: Tracker, https://github.com/aixcyi/zeraora/issues
 Description: <h1 align="center" style="padding-top: 32px">Zeraora</h1>
         
         <div align="center">
-            <a href="https://docs.python.org/zh-cn/3/whatsnew/index.html"><img src="https://img.shields.io/badge/Python-3.7%20%2B-blue.svg?logo=python&logoColor=yellow"></a>
+            <a href="https://docs.python.org/zh-cn/3/whatsnew/index.html"><img src="https://img.shields.io/pypi/pyversions/zeraora?label=Python&logo=python&logoColor=yellow"></a>
             <a href="https://en.wikipedia.org/wiki/MIT_License"><img src="https://img.shields.io/badge/License-MIT-purple.svg"></a>
             <a href="https://pypi.org/project/Zeraora/"><img src="https://img.shields.io/pypi/v/zeraora?color=darkgreen&label=PyPI"></a>
             <a href=""><img src="https://img.shields.io/conda/v/conda-forge/zeraora"></a>
         </div>
         <div align="center">
             <i>长期维护的个人开源工具库</i>
             <br>
             <i>An utility Python package supports for my personal and company projects</i>
         </div>
         
-        ## 特点
+        ## 特性
         
-        - 支持with、注解和实例化三种方式调用的计时器 [`BearTimer`](https://github.com/aixcyi/zeraora/blob/master/docs/zeraora/BearTimer.md) ；
-        - 生成通用representation方便调试时查看对象内部信息的 [`ReprMixin`](https://github.com/aixcyi/zeraora/blob/master/docs/zeraora/ReprMixin.md) ；
-        - 将字典的任意层级递归转化为对象，以便支持点分法访问数据的 [`OnionObject`](https://github.com/aixcyi/zeraora/blob/master/docs/zeraora/OnionObject.md) ；
-        - 安全转换的 `casting()` 和链式调用安全转换的 `Cast` ；
+        - 支持with、注解和实例化三种方式调用的计时器 `BearTimer` ；
+        - 生成通用representation方便调试时查看对象内部信息的 `ReprMixin` ；
+        - 将字典的任意层级递归转化为对象，以便支持点分法访问数据的 `OnionObject` ；
+        - 受 Django 的 `Choices` 启发的、可为枚举添加任意属性的 `Items` ；
         - 用以简化 `.as_view()` 传参的 `EasyViewSetMixin` ；
         - 仿照 `DestroyModelMixin` 实现的 `SoftDeleteModelMixin` ；
+        - 安全转换快捷函数 `safecast()` 和链式调用安全转换的 `SafeCast` ；
         - 不强制依赖任何非[标准库](https://docs.python.org/zh-cn/3/library/index.html)；
         - 更多……
         
         ## 安装
         
         使用 pip 直接安装：
         
@@ -51,33 +52,39 @@
         
         ```shell
         pip install zeraora -i http://pypi.mirrors.ustc.edu.cn/simple/
         ```
         
         ## 文档
         
-        部分文档以Markdown格式存放在docs目录下，查看该目录下的 [README.md](https://github.com/aixcyi/zeraora/blob/master/docs/README.md) 可以浏览全局公开符号的索引。
+        见[全局符号索引](./docs/README.md)。
         
-        源代码多数附带[类型标注](https://docs.python.org/zh-cn/3/glossary.html#term-type-hint)和[文档字符串](https://docs.python.org/zh-cn/3/glossary.html#term-docstring)（[reStructuredText](https://zh.wikipedia.org/wiki/ReStructuredText)格式），文档未尽事宜请移步源代码浏览。
+        ## 版本
         
-        ## 兼容性
+        |      | 状态[^1] | 支持时间 | 依赖              | 备注                                       |
+        | ---- | -------- | -------- | ----------------- | ------------------------------------------ |
+        | v0.3 | 🆕feature | 长期     | Python 3.7 或更新 | 趋于稳定，但改了包结构，不向下兼容。       |
+        | v0.2 | ✅bugfix  | 长期     | Python 3.7 或更新 | 探索包结构，完善核心特性，补充非核心特性。 |
+        | v0.1 | ❌EOL     | 不再支持 | Python 3.7 或更新 | 试验自动部署，只有核心特性。               |
         
-        [Python 3.7](https://docs.python.org/zh-cn/3/whatsnew/3.7.html#summary-release-highlights) 开始 `dict` 正式按照插入顺序存储，考虑到 `dict` 是 Python 的基石，为了避免出现难以察觉的错误，因而将该版本定为兼容下限。这也是我接触过的项目中的最低运行版本，故而不太希望维护对更低版本的兼容。
+        [^1]: 概念参见[Python版本状态](https://devguide.python.org/versions/#status-key)，目前只借用了以上三种。
         
-        项目会尽力保证向后兼容性，但还是建议在requirements中写明特定的版本号，避免因为版本更新或回退而出现棘手的错误。
+        ## 计划
         
+        - [ ] 打包到conda（未来，未来。）
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
```

#### html2text {}

```diff
@@ -1,53 +1,50 @@
-Metadata-Version: 2.1 Name: Zeraora Version: 0.2.9 Summary:
-ä¸ä¸ªåå«ååå·¥å·ç±»åå¿«æ·å½æ°çå·¥å·åºãA original utility
-Python package. Home-page: https://github.com/aixcyi/zeraora Author: aixcyi
-Author-email: 75880483+aixcyi@users.noreply.github.com License: MIT Project-
-URL: Source, https://github.com/aixcyi/zeraora Project-URL: Tracker, https://
-github.com/aixcyi/zeraora/issues Description:
+Metadata-Version: 2.1 Name: Zeraora Version: 0.3.0 Summary:
+ä¸ä¸ªé¿æç»´æ¤çä¸ªäººå¼æºå·¥å·åºãA utility Python package supports
+for my personal and company projects. Home-page: https://github.com/aixcyi/
+zeraora Author: aixcyi Author-email: 75880483+aixcyi@users.noreply.github.com
+License: MIT Project-URL: Source, https://github.com/aixcyi/zeraora Project-
+URL: Tracker, https://github.com/aixcyi/zeraora/issues Description:
                              ****** Zeraora ******
-                [https://img.shields.io/badge/Python-3.7%20%2B-
- blue.svg?logo=python&logoColor=yellow] [https://img.shields.io/badge/License-
-                MIT-purple.svg] [https://img.shields.io/pypi/v/
+                   [https://img.shields.io/pypi/pyversions/
+  zeraora?label=Python&logo=python&logoColor=yellow] [https://img.shields.io/
+         badge/License-MIT-purple.svg] [https://img.shields.io/pypi/v/
   zeraora?color=darkgreen&label=PyPI] [https://img.shields.io/conda/v/conda-
                                 forge/zeraora]
                      é¿æç»´æ¤çä¸ªäººå¼æºå·¥å·åº
     An utility Python package supports for my personal and company projects
-## ç¹ç¹ - æ¯æwithãæ³¨è§£åå®ä¾åä¸ç§æ¹å¼è°ç¨çè®¡æ¶å¨
-[`BearTimer`](https://github.com/aixcyi/zeraora/blob/master/docs/zeraora/
-BearTimer.md) ï¼ -
+## ç¹æ§ - æ¯æwithãæ³¨è§£åå®ä¾åä¸ç§æ¹å¼è°ç¨çè®¡æ¶å¨
+`BearTimer` ï¼ -
 çæéç¨representationæ¹ä¾¿è°è¯æ¶æ¥çå¯¹è±¡åé¨ä¿¡æ¯ç
-[`ReprMixin`](https://github.com/aixcyi/zeraora/blob/master/docs/zeraora/
-ReprMixin.md) ï¼ -
+`ReprMixin` ï¼ -
 å°å­å¸çä»»æå±çº§éå½è½¬åä¸ºå¯¹è±¡ï¼ä»¥ä¾¿æ¯æç¹åæ³è®¿é®æ°æ®ç
-[`OnionObject`](https://github.com/aixcyi/zeraora/blob/master/docs/zeraora/
-OnionObject.md) ï¼ - å®å¨è½¬æ¢ç `casting()`
-åé¾å¼è°ç¨å®å¨è½¬æ¢ç `Cast` ï¼ - ç¨ä»¥ç®å `.as_view()` ä¼ åç
-`EasyViewSetMixin` ï¼ - ä»¿ç§ `DestroyModelMixin` å®ç°ç
-`SoftDeleteModelMixin` ï¼ - ä¸å¼ºå¶ä¾èµä»»ä½é[æ ååº](https://
-docs.python.org/zh-cn/3/library/index.html)ï¼ - æ´å¤â¦â¦ ## å®è£ ä½¿ç¨
-pip ç´æ¥å®è£ï¼ ```shell pip install zeraora ```
-ä¸´æ¶éè¿æ¬å°ä»£çä½¿ç¨ pip å®è£ï¼ ```shell pip install zeraora --
-proxy=127.0.0.1:6666 ``` ä½¿ç¨ pip æ¶ä¸´æ¶æå®å®è£æºæ¥å®è£ï¼
+`OnionObject` ï¼ - å Django ç `Choices`
+å¯åçãå¯ä¸ºæä¸¾æ·»å ä»»æå±æ§ç `Items` ï¼ - ç¨ä»¥ç®å
+`.as_view()` ä¼ åç `EasyViewSetMixin` ï¼ - ä»¿ç§ `DestroyModelMixin`
+å®ç°ç `SoftDeleteModelMixin` ï¼ - å®å¨è½¬æ¢å¿«æ·å½æ° `safecast()`
+åé¾å¼è°ç¨å®å¨è½¬æ¢ç `SafeCast` ï¼ - ä¸å¼ºå¶ä¾èµä»»ä½é
+[æ ååº](https://docs.python.org/zh-cn/3/library/index.html)ï¼ -
+æ´å¤â¦â¦ ## å®è£ ä½¿ç¨ pip ç´æ¥å®è£ï¼ ```shell pip install zeraora
+``` ä¸´æ¶éè¿æ¬å°ä»£çä½¿ç¨ pip å®è£ï¼ ```shell pip install zeraora -
+-proxy=127.0.0.1:6666 ``` ä½¿ç¨ pip æ¶ä¸´æ¶æå®å®è£æºæ¥å®è£ï¼
 ```shell pip install zeraora -i http://pypi.mirrors.ustc.edu.cn/simple/ ``` ##
-ææ¡£
-é¨åææ¡£ä»¥Markdownæ ¼å¼å­æ¾å¨docsç®å½ä¸ï¼æ¥çè¯¥ç®å½ä¸ç
-[README.md](https://github.com/aixcyi/zeraora/blob/master/docs/README.md)
-å¯ä»¥æµè§å¨å±å¬å¼ç¬¦å·çç´¢å¼ã æºä»£ç å¤æ°éå¸¦[ç±»åæ æ³¨]
-(https://docs.python.org/zh-cn/3/glossary.html#term-type-hint)å
-[ææ¡£å­ç¬¦ä¸²](https://docs.python.org/zh-cn/3/glossary.html#term-
-docstring)ï¼[reStructuredText](https://zh.wikipedia.org/wiki/
-ReStructuredText)æ ¼å¼ï¼ï¼ææ¡£æªå°½äºå®è¯·ç§»æ­¥æºä»£ç æµè§ã ##
-å¼å®¹æ§ [Python 3.7](https://docs.python.org/zh-cn/3/whatsnew/
-3.7.html#summary-release-highlights) å¼å§ `dict`
-æ­£å¼æç§æå¥é¡ºåºå­å¨ï¼èèå° `dict` æ¯ Python
-çåºç³ï¼ä¸ºäºé¿ååºç°é¾ä»¥å¯è§çéè¯¯ï¼å èå°è¯¥çæ¬å®ä¸ºå¼å®¹ä¸éãè¿ä¹æ¯ææ¥è§¦è¿çé¡¹ç®ä¸­çæä½è¿è¡çæ¬ï¼æèä¸å¤ªå¸æç»´æ¤å¯¹æ´ä½çæ¬çå¼å®¹ã
-é¡¹ç®ä¼å°½åä¿è¯ååå¼å®¹æ§ï¼ä½è¿æ¯å»ºè®®å¨requirementsä¸­åæç¹å®ççæ¬å·ï¼é¿åå ä¸ºçæ¬æ´æ°æåéèåºç°æ£æçéè¯¯ã
-Platform: UNKNOWN Classifier: Development Status :: 4 - Beta Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Intended Audience :: Developers Classifier: Operating System :: OS Independent
-Classifier: Natural Language :: Chinese (Simplified) Classifier: License :: OSI
-Approved :: MIT License Classifier: Topic :: Utilities Classifier: Typing ::
-Typed Requires-Python: >=3.7 Description-Content-Type: text/markdown
+ææ¡£ è§[å¨å±ç¬¦å·ç´¢å¼](./docs/README.md)ã ## çæ¬ | | ç¶æ[^1] |
+æ¯ææ¶é´ | ä¾èµ | å¤æ³¨ | | ---- | -------- | -------- | ---------------
+-- | ------------------------------------------ | | v0.3 | ðfeature | é¿æ
+| Python 3.7 ææ´æ° | è¶äºç¨³å®ï¼ä½æ¹äºåç»æï¼ä¸åä¸å¼å®¹ã
+| | v0.2 | âbugfix | é¿æ | Python 3.7 ææ´æ° |
+æ¢ç´¢åç»æï¼å®åæ ¸å¿ç¹æ§ï¼è¡¥åéæ ¸å¿ç¹æ§ã | | v0.1 |
+âEOL | ä¸åæ¯æ | Python 3.7 ææ´æ° |
+è¯éªèªå¨é¨ç½²ï¼åªææ ¸å¿ç¹æ§ã | [^1]: æ¦å¿µåè§
+[Pythonçæ¬ç¶æ](https://devguide.python.org/versions/#status-
+key)ï¼ç®ååªåç¨äºä»¥ä¸ä¸ç§ã ## è®¡å - [ ]
+æåå°condaï¼æªæ¥ï¼æªæ¥ãï¼ Platform: UNKNOWN Classifier:
+Development Status :: 4 - Beta Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Classifier: Intended Audience :: Developers Classifier: Operating System :: OS
+Independent Classifier: Natural Language :: Chinese (Simplified) Classifier:
+License :: OSI Approved :: MIT License Classifier: Topic :: Utilities
+Classifier: Typing :: Typed Requires-Python: >=3.7 Description-Content-Type:
+text/markdown
```

### Comparing `Zeraora-0.2.9/Zeraora.egg-info/PKG-INFO` & `Zeraora-0.3.0/Zeraora.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 Metadata-Version: 2.1
 Name: Zeraora
-Version: 0.2.9
-Summary: 一个包含原创工具类及快捷函数的工具库。A original utility Python package.
+Version: 0.3.0
+Summary: 一个长期维护的个人开源工具库。A utility Python package supports for my personal and company projects.
 Home-page: https://github.com/aixcyi/zeraora
 Author: aixcyi
 Author-email: 75880483+aixcyi@users.noreply.github.com
 License: MIT
 Project-URL: Source, https://github.com/aixcyi/zeraora
 Project-URL: Tracker, https://github.com/aixcyi/zeraora/issues
 Description: <h1 align="center" style="padding-top: 32px">Zeraora</h1>
         
         <div align="center">
-            <a href="https://docs.python.org/zh-cn/3/whatsnew/index.html"><img src="https://img.shields.io/badge/Python-3.7%20%2B-blue.svg?logo=python&logoColor=yellow"></a>
+            <a href="https://docs.python.org/zh-cn/3/whatsnew/index.html"><img src="https://img.shields.io/pypi/pyversions/zeraora?label=Python&logo=python&logoColor=yellow"></a>
             <a href="https://en.wikipedia.org/wiki/MIT_License"><img src="https://img.shields.io/badge/License-MIT-purple.svg"></a>
             <a href="https://pypi.org/project/Zeraora/"><img src="https://img.shields.io/pypi/v/zeraora?color=darkgreen&label=PyPI"></a>
             <a href=""><img src="https://img.shields.io/conda/v/conda-forge/zeraora"></a>
         </div>
         <div align="center">
             <i>长期维护的个人开源工具库</i>
             <br>
             <i>An utility Python package supports for my personal and company projects</i>
         </div>
         
-        ## 特点
+        ## 特性
         
-        - 支持with、注解和实例化三种方式调用的计时器 [`BearTimer`](https://github.com/aixcyi/zeraora/blob/master/docs/zeraora/BearTimer.md) ；
-        - 生成通用representation方便调试时查看对象内部信息的 [`ReprMixin`](https://github.com/aixcyi/zeraora/blob/master/docs/zeraora/ReprMixin.md) ；
-        - 将字典的任意层级递归转化为对象，以便支持点分法访问数据的 [`OnionObject`](https://github.com/aixcyi/zeraora/blob/master/docs/zeraora/OnionObject.md) ；
-        - 安全转换的 `casting()` 和链式调用安全转换的 `Cast` ；
+        - 支持with、注解和实例化三种方式调用的计时器 `BearTimer` ；
+        - 生成通用representation方便调试时查看对象内部信息的 `ReprMixin` ；
+        - 将字典的任意层级递归转化为对象，以便支持点分法访问数据的 `OnionObject` ；
+        - 受 Django 的 `Choices` 启发的、可为枚举添加任意属性的 `Items` ；
         - 用以简化 `.as_view()` 传参的 `EasyViewSetMixin` ；
         - 仿照 `DestroyModelMixin` 实现的 `SoftDeleteModelMixin` ；
+        - 安全转换快捷函数 `safecast()` 和链式调用安全转换的 `SafeCast` ；
         - 不强制依赖任何非[标准库](https://docs.python.org/zh-cn/3/library/index.html)；
         - 更多……
         
         ## 安装
         
         使用 pip 直接安装：
         
@@ -51,33 +52,39 @@
         
         ```shell
         pip install zeraora -i http://pypi.mirrors.ustc.edu.cn/simple/
         ```
         
         ## 文档
         
-        部分文档以Markdown格式存放在docs目录下，查看该目录下的 [README.md](https://github.com/aixcyi/zeraora/blob/master/docs/README.md) 可以浏览全局公开符号的索引。
+        见[全局符号索引](./docs/README.md)。
         
-        源代码多数附带[类型标注](https://docs.python.org/zh-cn/3/glossary.html#term-type-hint)和[文档字符串](https://docs.python.org/zh-cn/3/glossary.html#term-docstring)（[reStructuredText](https://zh.wikipedia.org/wiki/ReStructuredText)格式），文档未尽事宜请移步源代码浏览。
+        ## 版本
         
-        ## 兼容性
+        |      | 状态[^1] | 支持时间 | 依赖              | 备注                                       |
+        | ---- | -------- | -------- | ----------------- | ------------------------------------------ |
+        | v0.3 | 🆕feature | 长期     | Python 3.7 或更新 | 趋于稳定，但改了包结构，不向下兼容。       |
+        | v0.2 | ✅bugfix  | 长期     | Python 3.7 或更新 | 探索包结构，完善核心特性，补充非核心特性。 |
+        | v0.1 | ❌EOL     | 不再支持 | Python 3.7 或更新 | 试验自动部署，只有核心特性。               |
         
-        [Python 3.7](https://docs.python.org/zh-cn/3/whatsnew/3.7.html#summary-release-highlights) 开始 `dict` 正式按照插入顺序存储，考虑到 `dict` 是 Python 的基石，为了避免出现难以察觉的错误，因而将该版本定为兼容下限。这也是我接触过的项目中的最低运行版本，故而不太希望维护对更低版本的兼容。
+        [^1]: 概念参见[Python版本状态](https://devguide.python.org/versions/#status-key)，目前只借用了以上三种。
         
-        项目会尽力保证向后兼容性，但还是建议在requirements中写明特定的版本号，避免因为版本更新或回退而出现棘手的错误。
+        ## 计划
         
+        - [ ] 打包到conda（未来，未来。）
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
```

#### html2text {}

```diff
@@ -1,53 +1,50 @@
-Metadata-Version: 2.1 Name: Zeraora Version: 0.2.9 Summary:
-ä¸ä¸ªåå«ååå·¥å·ç±»åå¿«æ·å½æ°çå·¥å·åºãA original utility
-Python package. Home-page: https://github.com/aixcyi/zeraora Author: aixcyi
-Author-email: 75880483+aixcyi@users.noreply.github.com License: MIT Project-
-URL: Source, https://github.com/aixcyi/zeraora Project-URL: Tracker, https://
-github.com/aixcyi/zeraora/issues Description:
+Metadata-Version: 2.1 Name: Zeraora Version: 0.3.0 Summary:
+ä¸ä¸ªé¿æç»´æ¤çä¸ªäººå¼æºå·¥å·åºãA utility Python package supports
+for my personal and company projects. Home-page: https://github.com/aixcyi/
+zeraora Author: aixcyi Author-email: 75880483+aixcyi@users.noreply.github.com
+License: MIT Project-URL: Source, https://github.com/aixcyi/zeraora Project-
+URL: Tracker, https://github.com/aixcyi/zeraora/issues Description:
                              ****** Zeraora ******
-                [https://img.shields.io/badge/Python-3.7%20%2B-
- blue.svg?logo=python&logoColor=yellow] [https://img.shields.io/badge/License-
-                MIT-purple.svg] [https://img.shields.io/pypi/v/
+                   [https://img.shields.io/pypi/pyversions/
+  zeraora?label=Python&logo=python&logoColor=yellow] [https://img.shields.io/
+         badge/License-MIT-purple.svg] [https://img.shields.io/pypi/v/
   zeraora?color=darkgreen&label=PyPI] [https://img.shields.io/conda/v/conda-
                                 forge/zeraora]
                      é¿æç»´æ¤çä¸ªäººå¼æºå·¥å·åº
     An utility Python package supports for my personal and company projects
-## ç¹ç¹ - æ¯æwithãæ³¨è§£åå®ä¾åä¸ç§æ¹å¼è°ç¨çè®¡æ¶å¨
-[`BearTimer`](https://github.com/aixcyi/zeraora/blob/master/docs/zeraora/
-BearTimer.md) ï¼ -
+## ç¹æ§ - æ¯æwithãæ³¨è§£åå®ä¾åä¸ç§æ¹å¼è°ç¨çè®¡æ¶å¨
+`BearTimer` ï¼ -
 çæéç¨representationæ¹ä¾¿è°è¯æ¶æ¥çå¯¹è±¡åé¨ä¿¡æ¯ç
-[`ReprMixin`](https://github.com/aixcyi/zeraora/blob/master/docs/zeraora/
-ReprMixin.md) ï¼ -
+`ReprMixin` ï¼ -
 å°å­å¸çä»»æå±çº§éå½è½¬åä¸ºå¯¹è±¡ï¼ä»¥ä¾¿æ¯æç¹åæ³è®¿é®æ°æ®ç
-[`OnionObject`](https://github.com/aixcyi/zeraora/blob/master/docs/zeraora/
-OnionObject.md) ï¼ - å®å¨è½¬æ¢ç `casting()`
-åé¾å¼è°ç¨å®å¨è½¬æ¢ç `Cast` ï¼ - ç¨ä»¥ç®å `.as_view()` ä¼ åç
-`EasyViewSetMixin` ï¼ - ä»¿ç§ `DestroyModelMixin` å®ç°ç
-`SoftDeleteModelMixin` ï¼ - ä¸å¼ºå¶ä¾èµä»»ä½é[æ ååº](https://
-docs.python.org/zh-cn/3/library/index.html)ï¼ - æ´å¤â¦â¦ ## å®è£ ä½¿ç¨
-pip ç´æ¥å®è£ï¼ ```shell pip install zeraora ```
-ä¸´æ¶éè¿æ¬å°ä»£çä½¿ç¨ pip å®è£ï¼ ```shell pip install zeraora --
-proxy=127.0.0.1:6666 ``` ä½¿ç¨ pip æ¶ä¸´æ¶æå®å®è£æºæ¥å®è£ï¼
+`OnionObject` ï¼ - å Django ç `Choices`
+å¯åçãå¯ä¸ºæä¸¾æ·»å ä»»æå±æ§ç `Items` ï¼ - ç¨ä»¥ç®å
+`.as_view()` ä¼ åç `EasyViewSetMixin` ï¼ - ä»¿ç§ `DestroyModelMixin`
+å®ç°ç `SoftDeleteModelMixin` ï¼ - å®å¨è½¬æ¢å¿«æ·å½æ° `safecast()`
+åé¾å¼è°ç¨å®å¨è½¬æ¢ç `SafeCast` ï¼ - ä¸å¼ºå¶ä¾èµä»»ä½é
+[æ ååº](https://docs.python.org/zh-cn/3/library/index.html)ï¼ -
+æ´å¤â¦â¦ ## å®è£ ä½¿ç¨ pip ç´æ¥å®è£ï¼ ```shell pip install zeraora
+``` ä¸´æ¶éè¿æ¬å°ä»£çä½¿ç¨ pip å®è£ï¼ ```shell pip install zeraora -
+-proxy=127.0.0.1:6666 ``` ä½¿ç¨ pip æ¶ä¸´æ¶æå®å®è£æºæ¥å®è£ï¼
 ```shell pip install zeraora -i http://pypi.mirrors.ustc.edu.cn/simple/ ``` ##
-ææ¡£
-é¨åææ¡£ä»¥Markdownæ ¼å¼å­æ¾å¨docsç®å½ä¸ï¼æ¥çè¯¥ç®å½ä¸ç
-[README.md](https://github.com/aixcyi/zeraora/blob/master/docs/README.md)
-å¯ä»¥æµè§å¨å±å¬å¼ç¬¦å·çç´¢å¼ã æºä»£ç å¤æ°éå¸¦[ç±»åæ æ³¨]
-(https://docs.python.org/zh-cn/3/glossary.html#term-type-hint)å
-[ææ¡£å­ç¬¦ä¸²](https://docs.python.org/zh-cn/3/glossary.html#term-
-docstring)ï¼[reStructuredText](https://zh.wikipedia.org/wiki/
-ReStructuredText)æ ¼å¼ï¼ï¼ææ¡£æªå°½äºå®è¯·ç§»æ­¥æºä»£ç æµè§ã ##
-å¼å®¹æ§ [Python 3.7](https://docs.python.org/zh-cn/3/whatsnew/
-3.7.html#summary-release-highlights) å¼å§ `dict`
-æ­£å¼æç§æå¥é¡ºåºå­å¨ï¼èèå° `dict` æ¯ Python
-çåºç³ï¼ä¸ºäºé¿ååºç°é¾ä»¥å¯è§çéè¯¯ï¼å èå°è¯¥çæ¬å®ä¸ºå¼å®¹ä¸éãè¿ä¹æ¯ææ¥è§¦è¿çé¡¹ç®ä¸­çæä½è¿è¡çæ¬ï¼æèä¸å¤ªå¸æç»´æ¤å¯¹æ´ä½çæ¬çå¼å®¹ã
-é¡¹ç®ä¼å°½åä¿è¯ååå¼å®¹æ§ï¼ä½è¿æ¯å»ºè®®å¨requirementsä¸­åæç¹å®ççæ¬å·ï¼é¿åå ä¸ºçæ¬æ´æ°æåéèåºç°æ£æçéè¯¯ã
-Platform: UNKNOWN Classifier: Development Status :: 4 - Beta Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Intended Audience :: Developers Classifier: Operating System :: OS Independent
-Classifier: Natural Language :: Chinese (Simplified) Classifier: License :: OSI
-Approved :: MIT License Classifier: Topic :: Utilities Classifier: Typing ::
-Typed Requires-Python: >=3.7 Description-Content-Type: text/markdown
+ææ¡£ è§[å¨å±ç¬¦å·ç´¢å¼](./docs/README.md)ã ## çæ¬ | | ç¶æ[^1] |
+æ¯ææ¶é´ | ä¾èµ | å¤æ³¨ | | ---- | -------- | -------- | ---------------
+-- | ------------------------------------------ | | v0.3 | ðfeature | é¿æ
+| Python 3.7 ææ´æ° | è¶äºç¨³å®ï¼ä½æ¹äºåç»æï¼ä¸åä¸å¼å®¹ã
+| | v0.2 | âbugfix | é¿æ | Python 3.7 ææ´æ° |
+æ¢ç´¢åç»æï¼å®åæ ¸å¿ç¹æ§ï¼è¡¥åéæ ¸å¿ç¹æ§ã | | v0.1 |
+âEOL | ä¸åæ¯æ | Python 3.7 ææ´æ° |
+è¯éªèªå¨é¨ç½²ï¼åªææ ¸å¿ç¹æ§ã | [^1]: æ¦å¿µåè§
+[Pythonçæ¬ç¶æ](https://devguide.python.org/versions/#status-
+key)ï¼ç®ååªåç¨äºä»¥ä¸ä¸ç§ã ## è®¡å - [ ]
+æåå°condaï¼æªæ¥ï¼æªæ¥ãï¼ Platform: UNKNOWN Classifier:
+Development Status :: 4 - Beta Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Classifier: Intended Audience :: Developers Classifier: Operating System :: OS
+Independent Classifier: Natural Language :: Chinese (Simplified) Classifier:
+License :: OSI Approved :: MIT License Classifier: Topic :: Utilities
+Classifier: Typing :: Typed Requires-Python: >=3.7 Description-Content-Type:
+text/markdown
```

### Comparing `Zeraora-0.2.9/setup.py` & `Zeraora-0.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,26 +16,27 @@
 setup(
     name='Zeraora',
     version=version,
     url='https://github.com/aixcyi/zeraora',
     license='MIT',
     author='aixcyi',
     author_email='75880483+aixcyi@users.noreply.github.com',
-    description="一个包含原创工具类及快捷函数的工具库。"
-                "A original utility Python package.",
+    description="一个长期维护的个人开源工具库。"
+                "A utility Python package supports for my personal and company projects.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
         "Development Status :: 4 - Beta",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Natural Language :: Chinese (Simplified)",
         "License :: OSI Approved :: MIT License",
         "Topic :: Utilities",
         "Typing :: Typed",
     ],
```

### Comparing `Zeraora-0.2.9/zeraora/charsets.py` & `Zeraora-0.3.0/zeraora/constants/charsets.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.9/zeraora/converters.py` & `Zeraora-0.3.0/zeraora/converters.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 """
 用于将一种值转换为另一种值的转换器。
 """
+
+__all__ = [
+    'delta2hms', 'delta2ms', 'delta2s',
+    'represent', 'datasize', 'dsz', 'true',
+    'SafeCaster', 'safecast', 'safecasts',
+    'remove_exponent',
+]
+
 import re
 from datetime import timedelta, datetime, date
 from decimal import Decimal
 from typing import Callable, Any, Tuple, Union
 from uuid import UUID
 
 from .typeclasses import Throwable, UNSET
@@ -52,26 +60,28 @@
 
     :param delta: 时间增量。
     :return: 一个小数。
     """
     return delta.seconds + delta.microseconds / 1000000
 
 
-def represent(value) -> str:
+def represent(value: Any) -> str:
     """
     将任意值转换为一个易于阅读的字符串。
 
     也是 ReprMixin 的默认格式化函数。
 
     默认使用 repr() 函数进行转换。如果自定义的类需要实现被此函数转换，请重写 .__repr__() 方法。
 
     :param value: 任意值。
     :return: 字符串。
     """
-    if isinstance(value, str):
+    if hasattr(value, 'label'):  # 兼容像 Django 的 Choices 那样的枚举
+        return value.label
+    elif isinstance(value, str):
         return f'"{value}"'
     elif isinstance(value, timedelta):
         return f'[{value.days}d+{value.seconds}.{value.microseconds:06d}s]'
     elif isinstance(value, datetime):
         return f'[{value:%Y-%m-%d %H:%M:%S,%f}]'
     elif isinstance(value, date):
         return f'[{value:%Y-%m-%d}]'
@@ -115,14 +125,17 @@
     shift = 'BKMGTPEZY'.index(result.group(2))
     power = (1024 if 'i' in result.group(3) else 1000) ** shift
     power = (power / 8) if 'b' in result.group(3) else power
 
     return base * power
 
 
+dsz = datasize
+
+
 def true(value) -> bool:
     """
     将HTTP请求中 query 部分的参数值转换为 Python 的逻辑值。
 
     :param value: query 中的参数值。
     :return: True 或 False。
     """
@@ -156,48 +169,65 @@
         return mapper(raw)
     except (TypeError, ValueError, KeyboardInterrupt) + exceptions:
         return default
 
 
 class SafeCaster:
 
-    def __init__(self, *exceptions: Throwable):
+    def __init__(self, raw: Any = UNSET):
+        """
+        创建一个安全转换器，用于转换某个值而不发生特定异常。若不提供初值，则第一个转换器也必须允许无参调用。
         """
-        创建一个安全转换器。
+        self._value = raw
+        self._default = None
+        self._converters = tuple()
+        self._exceptions = tuple()
+
+    def __call__(self, raw: Any = UNSET) -> 'SafeCaster':
+        self._value = raw
+        return self
 
-        :param exceptions: 可能发生的异常。应当提供可被 except 语句接受的值。
+    def catch(self, *exceptions: Throwable) -> 'SafeCaster':
+        """
+        置入需要捕获的异常。应当提供可被 except 语句接受的值。
         """
         self._exceptions = tuple(
             exc for exc in exceptions
             if exc.__class__ is type
             and issubclass(exc, BaseException)
             or isinstance(exc, BaseException)
         )
+        return self
 
-    def __call__(self, raw: Any = UNSET, *mappers: Callable, default=None):
+    def by(self, *mappers: Callable) -> 'SafeCaster':
+        """
+        置入转换器。若未提供初值，则第一个转换器也必须允许无参调用。
         """
-        转换一个值，转换失败时返回默认值，确保不会发生预先定义好的异常。
+        self._converters = tuple(
+            mapper for mapper in mappers
+            if callable(mapper)
+        )
+        return self
 
-        :param raw: 被转换的值。
-        :param mappers: 用来转换raw的转换器。如果某个转换器不可调用，将不会执行这个转换。
-        :param default: 默认值。
-        :return: 转换后的结果，或默认值。
+    def get(self, default=None) -> Any:
+        """
+        执行转换并返回转换结果。若触发置入的异常或没有置入转换器则返回默认值；若触发未被置入的异常将原样抛出。
         """
-        if len(mappers) <= 0:
+        if len(self._converters) <= 0:
             return default
 
-        if raw is UNSET:
-            result = mappers[0]()
-            converters = mappers[1:]
+        if self._value is UNSET:
+            result = self._converters[0]()
+            converters = self._converters[1:]
         else:
-            result = raw
-            converters = mappers
+            result = self._value
+            converters = self._converters
 
         try:
             for converter in converters:
                 result = converter(result) if callable(converter) else result
             return result
         except self._exceptions:
             return default
 
 
-safecasts = SafeCaster(TypeError, ValueError, KeyboardInterrupt)
+safecasts = SafeCaster().catch(TypeError, ValueError, KeyboardInterrupt)
```

### Comparing `Zeraora-0.2.9/zeraora/djangobase/mixins.py` & `Zeraora-0.3.0/zeraora/drf/viewsets.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""
+对 Django REST Framework 视图集（viewset）的增强。
+"""
 from typing import Any, Dict
 
 try:
     from django.utils.decorators import classonlymethod
     from rest_framework import status
     from rest_framework.response import Response
     from rest_framework.viewsets import ViewSetMixin
@@ -9,14 +12,19 @@
     print('需要安装Django以及DRF框架：pip install django djangorestframework')
     raise
 
 
 class EasyViewSetMixin(ViewSetMixin):
     """
     提供了两个方法来简化 ``.as_view()`` 的传参。
+
+    适用于：
+      - ``rest_framework.viewsets.ViewSet`` 的子类
+      - ``rest_framework.viewsets.GenericViewSet`` 的子类
+      - 需要 ``rest_framework.viewsets.ViewSetMixin`` 的类
     """
 
     @classonlymethod
     def to_view(cls, initkwargs: Dict[str, Any] = None, **actions: str):
         """
         将视图类存储在一个视图函数上，方便URL反向查找。
 
@@ -74,14 +82,19 @@
         }
         return cls.as_view(dict(mapper[a] for a in actions), **initkwargs)
 
 
 class SoftDeleteModelMixin:
     """
     将一个模型实例标记为已删除。（软删除）
+
+    - 通过 ``self.deletion_field`` 配置存储标记的字段，默认是 ``deleted``。
+    - 通过 ``self.deletion_mark`` 配置标记是什么，默认是布尔值 ``True`` 。
+
+    适用于：``rest_framework.generics.GenericAPIView`` 的子类
     """
     deletion_field = 'deleted'
     deletion_mark = True
 
     def soft_delete(self, request, *args, **kwargs):
         instance = self.get_object()
         self.perform_soft_delete(instance)
```

### Comparing `Zeraora-0.2.9/zeraora/generators.py` & `Zeraora-0.3.0/zeraora/generators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 """
 用于随机生成和特定顺序生成的生成器。
 """
+
+__all__ = [
+    'randbytes', 'SnowflakeWorker',
+    'randb62', 'SnowflakeMultiWorker',
+    'randb64', 'SnowflakeSingleWorker',
+]
+
 import os
 from random import getrandbits
 from time import time
 
-from .charsets import BASE62, BASE64
+from .constants.charsets import BASE62, BASE64
 
 
 def randbytes(n: int) -> bytes:
     """
     生成 n 个随机字节。
 
     此函数用于在 Python 3.9 以前代替 random.randbytes(n) 方法。
```

### Comparing `Zeraora-0.2.9/zeraora/typeclasses.py` & `Zeraora-0.3.0/zeraora/typeclasses.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 """
-数据类型类、枚举类、空类、类型别名等。
+类型包。包含数据类型类、枚举类、枚举元类、类型别名等。
 """
+
+__all__ = [
+    'Throwable', 'UNSET', 'OnionObject', 'RadixInteger',
+    'ItemsMeta', 'Items',
+]
+
 import enum
-from types import DynamicClassAttribute
-from typing import Type, Union, Tuple, Dict
+import typing as t
 
-Throwable = Union[BaseException, Type[BaseException]]
+Throwable = t.Union[BaseException, t.Type[BaseException]]
 
 
 class UNSET:
     pass
 
 
 class OnionObject(object):
@@ -105,24 +110,28 @@
             for attr, value in self.__dict__.items()
             if not attr.startswith('__') or attr.startswith(prefix)
         )
         return f'OnionObject({attrs})'
 
 
 # Little Endian
-class RadixInteger(Tuple[int, ...]):
+class RadixInteger(t.Tuple[int, ...]):
 
-    def __new__(cls, x: Union[int, Tuple[int, ...]], n: int, be=False, negative=False) -> 'RadixInteger':
+    def __new__(cls,
+                x: t.Union[int, t.Tuple[int, ...], t.List[int], bytes, bytearray],
+                n: int,
+                be=False,
+                negative=False) -> 'RadixInteger':
         """
         一个以元组表述各个数位的 N 进制整数。
 
-        :param x: 一个int类型的整数，或者一个包含非负整数的元组。
+        :param x: 一个int类型的整数，一个包含非负整数的元组，或者一个字节串。
         :param n: 进位制（的基数）。必须是一个大于等于 2 的正整数。
-        :param be: 给定元组使用大端字节序？
-        :param negative: 给定元组应当表示一个负数？
+        :param be: 表示给定元组是否使用大端字节序。
+        :param negative: 表示给定元组是否应当表示一个负数，或给定字节串是否使用二进制补码表示整数。
         """
 
         def dec2seq(i: int):
             while i >= n:
                 yield i % n
                 i //= n
             yield i
@@ -136,21 +145,27 @@
             self._integer = x
 
         elif isinstance(x, cls):
             self = tuple.__new__(cls, dec2seq(abs(x.numeric)))
             self._radix = n
             self._integer = x.numeric
 
-        elif isinstance(x, tuple):
-            bits = (i for i in x if i < 0 or i % 1 != 0)
-            if tuple(bits):
-                raise ValueError(
-                    'x 只能包含非负整数。'
-                )
-            radix = max(bits)
+        elif isinstance(x, (bytes, bytearray)):
+            self = tuple.__new__(cls, x[::-1] if be else x)
+            self._radix = 256
+            self._integer = (
+                int.from_bytes(x, 'big', signed=negative)
+                if be else
+                int.from_bytes(x, 'little', signed=negative)
+            )
+
+        elif isinstance(x, (tuple, list)):
+            if min(x) < 0:
+                raise ValueError('x 只能包含非负整数。')
+            radix = max(x)
             if not radix <= n:
                 raise ValueError(
                     f'x 的进位制最低是 {radix}，高于给定的 {n} 。'
                 )
             pairs = zip(x, reversed(range(len(x))))
             self = tuple.__new__(cls, x[::-1] if be else x)
             self._radix = n
@@ -170,131 +185,41 @@
         return self._radix
 
     @property
     def numeric(self):
         """对应的以阿拉伯数字表述的十进制整数。"""
         return self._integer
 
-    def map2str(self, mapping: Union[str, Dict[int, str]], be=True) -> str:
+    def map2str(self, mapping: t.Union[str, t.Dict[int, str]], be=True) -> str:
         """
         按照规则将每一位数映射到一个字符串中。
         """
         return ''.join(map(lambda i: mapping[i], self[::-1] if be else self))
 
-    def map2bytes(self, mapping: Union[bytes, Dict[int, bytes]], be=True) -> bytes:
+    def map2bytes(self, mapping: t.Union[bytes, t.Dict[int, bytes]], be=True) -> bytes:
         """
         按照规则将每一位数映射到一个字节串中。
         """
         return bytes(map(lambda i: mapping[i], self[::-1] if be else self))
 
 
-# copy from https://github.com/django/django/blob/stable/4.2.x/django/db/models/enums.py
-class ChoicesMeta(enum.EnumMeta):
-    """用于创建带有标签文本的枚举的类（元类）。"""
-
-    def __new__(metacls, classname, bases, classdict, **kwds):
-        labels = []
-        for key in classdict._member_names:
-            value = classdict[key]
-            if (
-                    isinstance(value, (list, tuple))
-                    and len(value) > 1
-                    and isinstance(value[-1], (str,))
-            ):
-                *value, label = value
-                value = tuple(value)
-            else:
-                label = key.replace("_", " ").title()
-            labels.append(label)
-            # Use dict.__setitem__() to suppress defenses against double
-            # assignment in enum's classdict.
-            dict.__setitem__(classdict, key, value)
-        cls = super().__new__(metacls, classname, bases, classdict, **kwds)
-        for member, label in zip(cls.__members__.values(), labels):
-            member._label_ = label
-        return enum.unique(cls)
-
-    def __contains__(cls, member):
-        if not isinstance(member, enum.Enum):
-            # Allow non-enums to match against member values.
-            return any(x.value == member for x in cls)
-        return super().__contains__(member)
-
-    @property
-    def names(cls):
-        empty = ["__empty__"] if hasattr(cls, "__empty__") else []
-        return empty + [member.name for member in cls]
-
-    @property
-    def choices(cls):
-        empty = [(None, cls.__empty__)] if hasattr(cls, "__empty__") else []
-        return empty + [(member.value, member.label) for member in cls]
-
-    @property
-    def labels(cls):
-        return [label for _, label in cls.choices]
-
-    @property
-    def values(cls):
-        return [value for value, _ in cls.choices]
-
-
-# copy from https://github.com/django/django/blob/stable/4.2.x/django/db/models/enums.py
-class Choices(enum.Enum, metaclass=ChoicesMeta):
-    """用于创建带有标签文本的枚举。"""
-
-    @DynamicClassAttribute
-    def label(self):
-        return self._label_
-
-    @property
-    def do_not_call_in_templates(self):
-        return True
-
-    def __str__(self):
-        """
-        Use value when cast to str, so that Choices set as model instance
-        attributes are rendered as expected in templates and similar contexts.
-        """
-        return str(self.value)
-
-    # A similar format was proposed for Python 3.10.
-    def __repr__(self):
-        return f"{self.__class__.__qualname__}.{self._name_}"
-
-
-# copy from https://github.com/django/django/blob/stable/4.2.x/django/db/models/enums.py
-class IntegerChoices(int, Choices):
-    """用于创建值是整数的带有标签文本的枚举。"""
-
-    pass
-
-
-# copy from https://github.com/django/django/blob/stable/4.2.x/django/db/models/enums.py
-class TextChoices(str, Choices):
-    """用于创建值是字符串的带有标签文本的枚举。"""
-
-    def _generate_next_value_(name, start, count, last_values):
-        return name
-
-
 class ItemsMeta(enum.EnumMeta):
     """用于创建带有任意属性的枚举的类（元类）。"""
 
     def __new__(metacls, classname, bases, classdict, **kwds):
         # 获取属性名（pks）
         if '__properties__' not in classdict:
             raise AttributeError(
                 f'{classname} 使用了 {metacls.__name__}，'
                 f'因此必须定义一个名为 __properties__ 的属性。'
             )
         pks = classdict['__properties__']
         if not isinstance(pks, (tuple, list)):
             raise TypeError(
-                f'{classname}.__properties__ 的值只允许是 tuple 或 list 。'
+                f'{classname}.__properties__ 只允许是一个 tuple 或 list 。'
             )
         if not all(isinstance(pk, str) and not pk.startswith('_') for pk in pks):
             raise TypeError(
                 f'{classname}.__properties__ 的值必须是字符串且不以下划线 “_” 开头。'
             )
         pks = tuple(f'_{pk}_' for pk in pks)
         qty = len(pks) + 1  # 等号右侧所有元素的总数
@@ -328,37 +253,63 @@
             raise TypeError
         if name[:-1] in cls.__properties__ and name.endswith('s'):
             return [getattr(member, name[:-1]) for member in cls]
         if name[:-2] in cls.__properties__ and name.endswith('es'):
             return [getattr(member, name[:-2]) for member in cls]
         return object.__getattribute__(cls, name)
 
+    # 对 __empty__ 属性的支持是为了与 Django 的 Choices 相兼容，可参见：
+    # https://docs.djangoproject.com/zh-hans/4.2/ref/models/fields/#enumeration-types
+
     @property
-    def names(cls):
+    def names(cls) -> t.List[str]:
         empty = ["__empty__"] if hasattr(cls, "__empty__") else []
         return empty + [member.name for member in cls]
 
     @property
-    def values(cls):
+    def values(cls) -> list:
         empty = [None] if hasattr(cls, "__empty__") else []
         return empty + [member.value for member in cls]
 
     @property
-    def choices(cls):
+    def items(cls) -> t.Dict[str, t.Any]:
+        its = {"__empty__": None} if hasattr(cls, "__empty__") else {}
+        its.update({member.name: member.value for member in cls})
+        return its
+
+    @property
+    def choices(cls) -> t.List[t.Tuple[t.Union[str, None], t.Any]]:
+        if 'label' not in cls.__properties__:
+            raise AttributeError(
+                '使用 .choices 属性前必须在 __properties__ 中'
+                '添加一个名为 "label" 的属性，且必须保证枚举值中有相应的属性值。'
+            )
         empty = [(None, cls.__empty__)] if hasattr(cls, "__empty__") else []
         return empty + [(member.value, member.label) for member in cls]
 
+    def value_of(cls, value: str) -> enum.Enum:
+        """
+        将一个枚举值转换为一个枚举。
+
+        :raise ValueError: 在枚举类中没有找到相应的枚举.
+        """
+        if value not in cls._value2member_map_:
+            raise ValueError(
+                f'{cls.__name__} 不存在值为 {value!s} 的枚举。'
+            )
+        return cls._value2member_map_[value]
+
 
 class Items(enum.Enum, metaclass=ItemsMeta):
     """
     用于创建带有任意属性的枚举。
 
     >>> from enum import Enum
     >>>
-    >>> class YearInSchool(Items):
+    >>> class Grade(Items):
     >>>     FRESHMAN = 1, 'FR', 0xE35314, 'Freshman'
     >>>     SOPHOMORE = 2, 'SO', 0xED15B4, 'Sophomore'
     >>>     JUNIOR = 3, 'JR', 0x9B3CED, 'Junior'
     >>>     SENIOR = 4, 'SR', 0xA0408E, 'Senior'
     >>>     GRADUATE = 5, 'GR', 0x518CCC, 'Graduate'
     >>>
     >>>     __properties__ = 'code', 'color', 'label'
@@ -371,24 +322,27 @@
     >>>     def color(self) -> int:
     >>>         return self._color_
     >>>
     >>>     @property
     >>>     def label(self) -> str:
     >>>         return self._label_
     >>>
-    >>> print(YearInSchool.SENIOR.name)  # 'SENIOR'
-    >>> print(YearInSchool.SENIOR.value)  # 4
-    >>> print(YearInSchool.SENIOR.code)  # 'SR'
-    >>> print(hex(YearInSchool.SENIOR.color))  # '0xa0408e'
-    >>> print(YearInSchool.SENIOR.label)  # 'Senior'
+    >>> print(Grade.SENIOR.name)  # 'SENIOR'
+    >>> print(Grade.SENIOR.value)  # 4
+    >>> print(Grade.SENIOR.code)  # 'SR'
+    >>> print(hex(Grade.SENIOR.color))  # '0xa0408e'
+    >>> print(Grade.SENIOR.label)  # 'Senior'
     >>>
-    >>> print(YearInSchool.names)  # ['FRESHMAN', 'SOPHOMORE', ...]
-    >>> print(YearInSchool.values)  # [1, 2, 3, 4, 5]
-    >>> print(YearInSchool.codes)  # ['FR', 'SO', 'JR', 'SR', 'GR']
-    >>> print(YearInSchool.colors)  # [14897940, 15537588, ...]
-    >>> print(YearInSchool.labels)  # ['Freshman', 'Sophomore', ...]
+    >>> print(Grade.names)  # ['FRESHMAN', 'SOPHOMORE', ...]
+    >>> print(Grade.values)  # [1, 2, 3, 4, 5]
+    >>> print(Grade.codes)  # ['FR', 'SO', 'JR', 'SR', 'GR']
+    >>> print(Grade.colors)  # [14897940, 15537588, ...]
+    >>> print(Grade.labels)  # ['Freshman', 'Sophomore', ...]
     """
+
     __properties__ = ()
 
+    def __str__(self):
+        return str(self.value)
+
     def __repr__(self):
-        # 枚举也算一种常量，直接按路径查找即可，故舍去附加的属性
         return f"{self.__class__.__qualname__}.{self._name_}"
```

