# Comparing `tmp/fast_captcha-0.1.3.tar.gz` & `tmp/fast_captcha-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_captcha-0.1.3.tar", max compression
+gzip compressed data, was "fast_captcha-0.2.0.tar", max compression
```

## Comparing `fast_captcha-0.1.3.tar` & `fast_captcha-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0      185 2022-04-20 11:31:12.153879 fast_captcha-0.1.3/fast_captcha/__init__.py
--rw-r--r--   0        0        0   142224 2022-04-20 11:20:01.994628 fast_captcha-0.1.3/fast_captcha/fonts/3Dumb.ttf
--rw-r--r--   0        0        0    34944 2022-04-20 11:20:02.016648 fast_captcha-0.1.3/fast_captcha/fonts/actionj.ttf
--rw-r--r--   0        0        0    62080 2022-04-20 11:20:01.995629 fast_captcha-0.1.3/fast_captcha/fonts/ApothecaryFont.ttf
--rw-r--r--   0        0        0   472660 2022-04-20 11:20:01.998632 fast_captcha-0.1.3/fast_captcha/fonts/BY-Easy-love-2.ttf
--rw-r--r--   0        0        0    32800 2022-04-20 11:20:01.999632 fast_captcha-0.1.3/fast_captcha/fonts/D3Parallelism.ttf
--rw-r--r--   0        0        0    83188 2022-04-20 11:20:02.000634 fast_captcha-0.1.3/fast_captcha/fonts/DENNEthree-dee.ttf
--rw-r--r--   0        0        0   283156 2022-04-20 11:20:02.002635 fast_captcha-0.1.3/fast_captcha/fonts/Esquisito.ttf
--rw-r--r--   0        0        0   140576 2022-04-20 11:20:02.004637 fast_captcha-0.1.3/fast_captcha/fonts/Flim-Flam.ttf
--rw-r--r--   0        0        0    29368 2022-04-20 11:20:02.004637 fast_captcha-0.1.3/fast_captcha/fonts/Frizon.ttf
--rw-r--r--   0        0        0    69292 2022-04-20 11:20:02.005638 fast_captcha-0.1.3/fast_captcha/fonts/KREMLINGEORGIANI3D.ttf
--rw-r--r--   0        0        0   935888 2022-04-20 11:20:02.011644 fast_captcha-0.1.3/fast_captcha/fonts/Maler.ttf
--rw-r--r--   0        0        0   427596 2022-04-20 11:20:02.014646 fast_captcha-0.1.3/fast_captcha/fonts/MoonRocks.ttf
--rw-r--r--   0        0        0    69896 2022-04-20 11:20:02.015647 fast_captcha-0.1.3/fast_captcha/fonts/Shojumaru.ttf
--rw-r--r--   0        0        0     2830 2022-04-20 12:02:49.381426 fast_captcha-0.1.3/fast_captcha/img_captcha.py
--rw-r--r--   0        0        0      317 2022-04-20 11:42:51.071444 fast_captcha-0.1.3/fast_captcha/text_captcha.py
--rw-r--r--   0        0        0     1084 2022-04-20 11:20:01.992626 fast_captcha-0.1.3/LICENSE
--rw-r--r--   0        0        0      478 2022-04-20 11:53:23.163946 fast_captcha-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2205 2022-04-20 12:05:38.958696 fast_captcha-0.1.3/README.MD
--rw-r--r--   0        0        0     2889 2022-04-20 12:09:59.704247 fast_captcha-0.1.3/setup.py
--rw-r--r--   0        0        0     2790 2022-04-20 12:09:59.705248 fast_captcha-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      284 2023-06-09 06:40:13.831760 fast_captcha-0.2.0/fast_captcha/__init__.py
+-rw-r--r--   0        0        0   142224 2023-06-09 04:25:41.492202 fast_captcha-0.2.0/fast_captcha/fonts/3Dumb.ttf
+-rw-r--r--   0        0        0    34944 2023-06-09 04:25:41.521475 fast_captcha-0.2.0/fast_captcha/fonts/actionj.ttf
+-rw-r--r--   0        0        0    62080 2023-06-09 04:25:41.493203 fast_captcha-0.2.0/fast_captcha/fonts/ApothecaryFont.ttf
+-rw-r--r--   0        0        0   472660 2023-06-09 04:25:41.496444 fast_captcha-0.2.0/fast_captcha/fonts/BY-Easy-love-2.ttf
+-rw-r--r--   0        0        0    32800 2023-06-09 04:25:41.496957 fast_captcha-0.2.0/fast_captcha/fonts/D3Parallelism.ttf
+-rw-r--r--   0        0        0    83188 2023-06-09 04:25:41.497471 fast_captcha-0.2.0/fast_captcha/fonts/DENNEthree-dee.ttf
+-rw-r--r--   0        0        0   283156 2023-06-09 04:25:41.507475 fast_captcha-0.2.0/fast_captcha/fonts/Esquisito.ttf
+-rw-r--r--   0        0        0   140576 2023-06-09 04:25:41.508476 fast_captcha-0.2.0/fast_captcha/fonts/Flim-Flam.ttf
+-rw-r--r--   0        0        0    29368 2023-06-09 04:25:41.509475 fast_captcha-0.2.0/fast_captcha/fonts/Frizon.ttf
+-rw-r--r--   0        0        0    69292 2023-06-09 04:25:41.509475 fast_captcha-0.2.0/fast_captcha/fonts/KREMLINGEORGIANI3D.ttf
+-rw-r--r--   0        0        0   935888 2023-06-09 04:25:41.516475 fast_captcha-0.2.0/fast_captcha/fonts/Maler.ttf
+-rw-r--r--   0        0        0   427596 2023-06-09 04:25:41.519475 fast_captcha-0.2.0/fast_captcha/fonts/MoonRocks.ttf
+-rw-r--r--   0        0        0    69896 2023-06-09 04:25:41.520475 fast_captcha-0.2.0/fast_captcha/fonts/Shojumaru.ttf
+-rw-r--r--   0        0        0     3418 2023-06-09 07:09:31.572554 fast_captcha-0.2.0/fast_captcha/img_captcha.py
+-rw-r--r--   0        0        0      303 2023-06-09 05:21:49.915846 fast_captcha-0.2.0/fast_captcha/text_captcha.py
+-rw-r--r--   0        0        0     1084 2023-06-09 04:25:41.480203 fast_captcha-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1160 2023-06-09 06:59:39.686082 fast_captcha-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2205 2023-06-09 04:25:41.480203 fast_captcha-0.2.0/README.MD
+-rw-r--r--   0        0        0     3162 1970-01-01 00:00:00.000000 fast_captcha-0.2.0/PKG-INFO
```

### Comparing `fast_captcha-0.1.3/fast_captcha/fonts/3Dumb.ttf` & `fast_captcha-0.2.0/fast_captcha/fonts/3Dumb.ttf`

 * *Files identical despite different names*

### Comparing `fast_captcha-0.1.3/fast_captcha/fonts/actionj.ttf` & `fast_captcha-0.2.0/fast_captcha/fonts/actionj.ttf`

 * *Files identical despite different names*

### Comparing `fast_captcha-0.1.3/fast_captcha/fonts/ApothecaryFont.ttf` & `fast_captcha-0.2.0/fast_captcha/fonts/ApothecaryFont.ttf`

 * *Files identical despite different names*

### Comparing `fast_captcha-0.1.3/fast_captcha/fonts/BY-Easy-love-2.ttf` & `fast_captcha-0.2.0/fast_captcha/fonts/BY-Easy-love-2.ttf`

 * *Files identical despite different names*

### Comparing `fast_captcha-0.1.3/fast_captcha/fonts/D3Parallelism.ttf` & `fast_captcha-0.2.0/fast_captcha/fonts/D3Parallelism.ttf`

 * *Files identical despite different names*

### Comparing `fast_captcha-0.1.3/fast_captcha/fonts/DENNEthree-dee.ttf` & `fast_captcha-0.2.0/fast_captcha/fonts/DENNEthree-dee.ttf`

 * *Files identical despite different names*

### Comparing `fast_captcha-0.1.3/fast_captcha/fonts/Esquisito.ttf` & `fast_captcha-0.2.0/fast_captcha/fonts/Esquisito.ttf`

 * *Files identical despite different names*

### Comparing `fast_captcha-0.1.3/fast_captcha/fonts/Flim-Flam.ttf` & `fast_captcha-0.2.0/fast_captcha/fonts/Flim-Flam.ttf`

 * *Files identical despite different names*

### Comparing `fast_captcha-0.1.3/fast_captcha/fonts/Frizon.ttf` & `fast_captcha-0.2.0/fast_captcha/fonts/Frizon.ttf`

 * *Files identical despite different names*

### Comparing `fast_captcha-0.1.3/fast_captcha/fonts/KREMLINGEORGIANI3D.ttf` & `fast_captcha-0.2.0/fast_captcha/fonts/KREMLINGEORGIANI3D.ttf`

 * *Files identical despite different names*

### Comparing `fast_captcha-0.1.3/fast_captcha/fonts/Maler.ttf` & `fast_captcha-0.2.0/fast_captcha/fonts/Maler.ttf`

 * *Files identical despite different names*

### Comparing `fast_captcha-0.1.3/fast_captcha/fonts/MoonRocks.ttf` & `fast_captcha-0.2.0/fast_captcha/fonts/MoonRocks.ttf`

 * *Files identical despite different names*

### Comparing `fast_captcha-0.1.3/fast_captcha/fonts/Shojumaru.ttf` & `fast_captcha-0.2.0/fast_captcha/fonts/Shojumaru.ttf`

 * *Files identical despite different names*

### Comparing `fast_captcha-0.1.3/fast_captcha/img_captcha.py` & `fast_captcha-0.2.0/fast_captcha/img_captcha.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,94 +1,115 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
+from __future__ import annotations
+
 import random
 from io import BytesIO
 from pathlib import Path
+from typing import Tuple, Literal
 
 from PIL import Image, ImageDraw, ImageFont
 
 from fast_captcha import text_captcha
 
 
-def use_rgb() -> tuple:
+def use_rgb() -> Tuple[int, ...]:
     """
     random colors for captcha text and distractions
+
     :return:
     """
     return tuple((random.randint(0, 255) for _ in range(3)))
 
 
-def ttf() -> list:
+def get_ttf() -> list[str]:
     """
     get all *.ttf file
+
     :return:
     """
-    fp = Path(__file__).parent.joinpath('fonts')
-    ft = [str(t) for t in fp.glob('*.ttf')]
-    return ft
+    file_path = Path(__file__).parent.joinpath('fonts')
+    ttf = [str(f) for f in file_path.glob('*.ttf')]
+    return ttf
 
 
 def img_captcha(
-        *,
-        code_num=4,
-        width=120,
-        height=40,
-        font_type=random.choice(ttf()),
-        font_size=32,
-        draw_lines=True,
-        lines_num=4,
-        draw_points=False,
-        points_density=4,
-        img_type='jpeg',
-        img_byte=True):
+    *,
+    code_num: int = 4,
+    width: int = 120,
+    height: int = 40,
+    font_type: str = random.choice(get_ttf()),
+    font_size: int = 32,
+    draw_lines: bool = True,
+    lines_num: int = 4,
+    draw_points: bool = False,
+    points_density: int = 4,
+    img_type: str = 'jpeg',
+    img_byte: Literal['file', 'bytesio', 'base64'] = 'bytesio',
+) -> tuple[Image.Image | BytesIO | bytes, str]:
     """
     img captcha
-    :param code_num: number of codes
-    :param width: picture width, default 120
-    :param height: picture height, default 40
-    :param font_size: font display size, default 32
-    :param font_type: captcha font default random
-    :param draw_lines: whether to draw lines
-    :param lines_num: number of lines drawn
-    :param draw_points: whether to draw points
-    :param points_density: draw point's density, the higher the value the higher the density
+
+    :param code_num: number of codes.
+    :param width: picture width, default 120.
+    :param height: picture height, default 40.
+    :param font_size: font display size, default 32.
+    :param font_type: captcha font default random.
+    :param draw_lines: whether to draw lines.
+    :param lines_num: number of lines drawn.
+    :param draw_points: whether to draw points.
+    :param points_density: draw point's density, the higher the value the higher the density.
     :param img_type: image type, for-example: jpeg, png ...
-    :param img_byte: convert image to bytes, if you use byte stream
+    :param img_byte: convert image to bytes, if you are using byte stream.
     :return:
     """
     # create img
     img = Image.new('RGB', (width, height), (255, 255, 255))
     # create draw lines
     draw = ImageDraw.Draw(img)
     # set font type and size
     font = ImageFont.truetype(font_type, font_size)
     # random text code
     text = text_captcha(code_num)
     # draw text
     for i, t in enumerate(text):
-        draw.text(xy=(i * width // code_num + random.randint((random.randint(i, code_num)), code_num), code_num / 2),
-                  text=t,
-                  font=font,
-                  fill=use_rgb())
+        draw.text(
+            xy=(i * width // code_num + random.randint((random.randint(i, code_num)), code_num), code_num / 2),
+            text=t,
+            font=font,
+            fill=use_rgb(),
+        )
     # draw lines
     if draw_lines:
         for i in range(lines_num):
-            draw.line(xy=[random.randint(0, width), random.randint(0, height),
-                          random.randint(0, width), random.randint(0, height)],
-                      fill=use_rgb())
+            draw.line(
+                xy=[
+                    random.randint(0, width),
+                    random.randint(0, height),
+                    random.randint(0, width),
+                    random.randint(0, height),
+                ],
+                fill=use_rgb(),
+            )
     # draw points
     if draw_points:
         chance = min(100, max(0, int(points_density)))
         for w in range(width):
             for h in range(height):
                 tmp = random.randint(0, 100)
                 if tmp > 100 - chance:
                     draw.point((w, h), fill=use_rgb())
-    # img type
-    if img_byte:
-        io = BytesIO()
-        img.save(io, img_type)
-        io.seek(0)
+    # img save
+    io = BytesIO()
+    img.save(io, img_type)
+    io.seek(0)
+    if img_byte == 'file':
+        img = img
+    elif img_byte == 'bytesio':
         img = io
+    elif img_byte == 'base64':
+        import base64
+
+        img = base64.b64encode(io.getvalue()).decode('utf-8')
     else:
-        img = img
+        raise ValueError('img_byte must be one of file, bytesio, base64')
     return img, text
```

### Comparing `fast_captcha-0.1.3/LICENSE` & `fast_captcha-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_captcha-0.1.3/README.MD` & `fast_captcha-0.2.0/README.MD`

 * *Files identical despite different names*

### Comparing `fast_captcha-0.1.3/PKG-INFO` & `fast_captcha-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 Metadata-Version: 2.1
 Name: fast-captcha
-Version: 0.1.3
-Summary: fast to use captcha
-Home-page: https://gitee.com/wu_cl/fast_captcha
+Version: 0.2.0
+Summary: Fast to use captcha
+Home-page: https://github.com/wu-clan/fast_captcha
 License: MIT
 Author: wu
 Author-email: jianhengwu0407@gmail.com
 Requires-Python: >=3.7,<4.0
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: Pillow (>=8.2.0,<9.0.0)
-Project-URL: Repository, https://gitee.com/wu_cl/fast_captcha
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: Pillow (>=9.2.0,<10.0.0)
+Requires-Dist: pytest (>=7.3.1,<8.0.0)
+Project-URL: Repository, https://github.com/wu-clan/fast_captcha
 Description-Content-Type: text/markdown
 
 # fast_captcha
 
 fast to use captcha
 
 # install
```

