# Comparing `tmp/nonebot_plugin_bilichat-2.4.1.tar.gz` & `tmp/nonebot_plugin_bilichat-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-2.4.1.tar", last modified: Wed Jun  7 08:38:33 2023, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-2.4.2.tar", last modified: Fri Jun  9 14:15:41 2023, max compression
```

## Comparing `nonebot_plugin_bilichat-2.4.1.tar` & `nonebot_plugin_bilichat-2.4.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    34523 2023-06-07 08:38:24.283974 nonebot_plugin_bilichat-2.4.1/LICENSE
--rw-r--r--   0        0        0    12555 2023-06-07 08:38:24.283974 nonebot_plugin_bilichat-2.4.1/README.md
--rw-r--r--   0        0        0     8790 2023-06-07 08:38:24.287974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     4914 2023-06-07 08:38:24.287974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0      513 2023-06-07 08:38:24.287974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6226 2023-06-07 08:38:24.287974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0     4806 2023-06-07 08:38:24.287974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/lib/bilibili_request.py
--rw-r--r--   0        0        0      871 2023-06-07 08:38:24.287974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/lib/column_resolve.py
--rw-r--r--   0        0        0     6439 2023-06-07 08:38:24.287974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/lib/content_resolve.py
--rw-r--r--   0        0        0     8900 2023-06-07 08:38:24.287974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/lib/draw_bili_image.py
--rw-r--r--   0        0        0     3812 2023-06-07 08:38:24.287974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      555 2023-06-07 08:38:24.287974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     1868 2023-06-07 08:38:24.287974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     4102 2023-06-07 08:38:24.291974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0      341 2023-06-07 08:38:24.291974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/model/arguments.py
--rw-r--r--   0        0        0     2854 2023-06-07 08:38:24.291974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0     1127 2023-06-07 08:38:24.291974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/model/cache.py
--rw-r--r--   0        0        0      387 2023-06-07 08:38:24.291974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/model/content.py
--rw-r--r--   0        0        0      503 2023-06-07 08:38:24.291974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0    27359 2023-06-07 08:38:24.291974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/model/newbing.py
--rw-r--r--   0        0        0      323 2023-06-07 08:38:24.291974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      261 2023-06-07 08:38:24.291974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0   248896 2023-06-07 08:38:24.291974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/static/bing_apology.jpg
--rw-r--r--   0        0        0     1363 2023-06-07 08:38:24.291974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/summary/__init__.py
--rw-r--r--   0        0        0     5904 2023-06-07 08:38:24.291974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/summary/newbing_summarise.py
--rw-r--r--   0        0        0     4916 2023-06-07 08:38:24.291974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     2363 2023-06-07 08:38:24.291974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/summary/openai_summarise.py
--rw-r--r--   0        0        0     1448 2023-06-07 08:38:24.291974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/summary/text_to_image.py
--rw-r--r--   0        0        0     1780 2023-06-07 08:38:24.291974 nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py
--rw-r--r--   0        0        0     1499 2023-06-07 08:38:33.092092 nonebot_plugin_bilichat-2.4.1/pyproject.toml
--rw-r--r--   0        0        0    13996 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.4.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-09 14:15:33.823675 nonebot_plugin_bilichat-2.4.2/LICENSE
+-rw-r--r--   0        0        0    12555 2023-06-09 14:15:33.823675 nonebot_plugin_bilichat-2.4.2/README.md
+-rw-r--r--   0        0        0     8790 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     4914 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0      513 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6226 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0     4806 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/lib/bilibili_request.py
+-rw-r--r--   0        0        0      871 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/lib/column_resolve.py
+-rw-r--r--   0        0        0     6463 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/lib/content_resolve.py
+-rw-r--r--   0        0        0    11809 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/lib/draw_bili_image.py
+-rw-r--r--   0        0        0     3812 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      555 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     1868 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     4102 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0      341 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/model/arguments.py
+-rw-r--r--   0        0        0     2854 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0     1127 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/model/cache.py
+-rw-r--r--   0        0        0      387 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/model/content.py
+-rw-r--r--   0        0        0      503 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0    27359 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/model/newbing.py
+-rw-r--r--   0        0        0      323 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      261 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0   248896 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/static/bing_apology.jpg
+-rw-r--r--   0        0        0     1363 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0     5904 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/summary/newbing_summarise.py
+-rw-r--r--   0        0        0     4916 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2363 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     1448 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/summary/text_to_image.py
+-rw-r--r--   0        0        0     1780 2023-06-09 14:15:33.831675 nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/wordcloud/wordcloud.py
+-rw-r--r--   0        0        0     1499 2023-06-09 14:15:41.951746 nonebot_plugin_bilichat-2.4.2/pyproject.toml
+-rw-r--r--   0        0        0    13996 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.4.2/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-2.4.1/LICENSE` & `nonebot_plugin_bilichat-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.1/README.md` & `nonebot_plugin_bilichat-2.4.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/lib/b23_extract.py` & `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/lib/b23_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/lib/bilibili_request.py` & `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/lib/bilibili_request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/lib/column_resolve.py` & `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/lib/column_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/lib/content_resolve.py` & `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/lib/content_resolve.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from ..config import plugin_config
 from ..model.arguments import Options
 from ..model.cache import Cache, Episode
 from ..model.content import Video, Column
 from ..model.exception import AbortError
 from ..optional import capture_exception  # type: ignore
 from .bilibili_request import get_b23_url, grpc_get_view_info
-from .draw_bili_image import binfo_image_create
+from .draw_bili_image import BiliVideoImage
 from .video_subtitle import get_subtitle
 from .column_resolve import get_cv
 
 
 cd: Dict[str, int] = {}
 cd_size_limit = plugin_config.bilichat_cd_time // 2
 
@@ -80,15 +80,15 @@
     if not check_cd(f"{aid}_{uid}"):
         logger.warning(f"Duplicate video {aid}. Skip the video parsing process")
         return (None, None, None)
     # generate video information
     try:
         b23_url = await get_b23_url(f"https://www.bilibili.com/video/{bvid}")
         data = (
-            (await binfo_image_create(video_info, b23_url))
+            (await (await BiliVideoImage.from_view_rely(video_info, b23_url)).render())
             if plugin_config.bilichat_basic_info
             else "IMG_RENDER_DISABLED"
         )
         logger.debug(f"Video parsing complete - aid:{aid} cid:{cid} title:{title}")
         return (b23_url, data, Video(aid, cid, title))
     except TimeoutException:
         logger.warning("Video parsing API call timeout")
```

### Comparing `nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/lib/store.py` & `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/lib/store.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/model/cache.py` & `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/model/cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/model/newbing.py` & `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/model/newbing.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/static/bing_apology.jpg` & `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/static/bing_apology.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/summary/__init__.py` & `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/summary/newbing_summarise.py` & `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/summary/newbing_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/summary/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/summary/openai_summarise.py` & `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/summary/text_to_image.py` & `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/summary/text_to_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py` & `nonebot_plugin_bilichat-2.4.2/nonebot_plugin_bilichat/wordcloud/wordcloud.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.4.1/pyproject.toml` & `nonebot_plugin_bilichat-2.4.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "py311",
 ]
 include = "\\.pyi?$"
 extend-exclude = ""
 
 [project]
 name = "nonebot-plugin-bilichat"
-version = "2.4.1"
+version = "2.4.2"
 description = "一个通过 OpenAI 来对b站视频进行总结插件"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "bilireq>=0.2.4",
```

### Comparing `nonebot_plugin_bilichat-2.4.1/PKG-INFO` & `nonebot_plugin_bilichat-2.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 2.4.1
+Version: 2.4.2
 Summary: 一个通过 OpenAI 来对b站视频进行总结插件
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.8
 Requires-Dist: bilireq>=0.2.4
 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.4.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.4.2 Summary:
 ä¸ä¸ªéè¿ OpenAI æ¥å¯¹bç«è§é¢è¿è¡æ»ç»æä»¶ Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.8 Requires-Dist:
 bilireq>=0.2.4 Requires-Dist: qrcode>=7.4.2 Requires-Dist: pillow>=9.5.0
 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-plugin-localstore>=0.4.1
 Requires-Dist: nonebot-adapter-onebot>=2.2.2 Requires-Dist: nonebot-plugin-
 segbuilder>=0.2.0 Requires-Dist: nonebot2>=2.0.0 Requires-Dist: nonebot-plugin-
```

