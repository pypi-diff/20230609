# Comparing `tmp/manim_mobject_svg-0.3.0.tar.gz` & `tmp/manim_mobject_svg-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manim_mobject_svg-0.3.0.tar", max compression
+gzip compressed data, was "manim_mobject_svg-0.4.0.tar", max compression
```

## Comparing `manim_mobject_svg-0.3.0.tar` & `manim_mobject_svg-0.4.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2023-06-09 16:03:41.454657 manim_mobject_svg-0.3.0/LICENSE
--rw-r--r--   0        0        0     1479 2023-06-09 16:03:41.454657 manim_mobject_svg-0.3.0/README.md
--rw-r--r--   0        0        0      603 2023-06-09 16:03:41.454657 manim_mobject_svg-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      203 2023-06-09 16:03:41.454657 manim_mobject_svg-0.3.0/src/manim_mobject_svg/__init__.py
--rw-r--r--   0        0        0     6694 2023-06-09 16:03:41.454657 manim_mobject_svg-0.3.0/src/manim_mobject_svg/svg.py
--rw-r--r--   0        0        0     2229 1970-01-01 00:00:00.000000 manim_mobject_svg-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-09 17:09:11.077655 manim_mobject_svg-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1479 2023-06-09 17:09:11.077655 manim_mobject_svg-0.4.0/README.md
+-rw-r--r--   0        0        0      603 2023-06-09 17:09:11.081655 manim_mobject_svg-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      404 2023-06-09 17:09:11.081655 manim_mobject_svg-0.4.0/src/manim_mobject_svg/__init__.py
+-rw-r--r--   0        0        0     6694 2023-06-09 17:09:11.081655 manim_mobject_svg-0.4.0/src/manim_mobject_svg/svg.py
+-rw-r--r--   0        0        0     2229 1970-01-01 00:00:00.000000 manim_mobject_svg-0.4.0/PKG-INFO
```

### Comparing `manim_mobject_svg-0.3.0/LICENSE` & `manim_mobject_svg-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `manim_mobject_svg-0.3.0/README.md` & `manim_mobject_svg-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `manim_mobject_svg-0.3.0/pyproject.toml` & `manim_mobject_svg-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "manim-mobject-svg"
-version = "0.3.0"
+version = "0.4.0"
 description = "Create SVG files from VMobject and VGroup"
 authors = ["Naveen M K <naveen521kk@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/naveen521kk/manim-mobject-svg"
 
 [tool.poetry.dependencies]
```

### Comparing `manim_mobject_svg-0.3.0/src/manim_mobject_svg/svg.py` & `manim_mobject_svg-0.4.0/src/manim_mobject_svg/svg.py`

 * *Files identical despite different names*

### Comparing `manim_mobject_svg-0.3.0/PKG-INFO` & `manim_mobject_svg-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manim-mobject-svg
-Version: 0.3.0
+Version: 0.4.0
 Summary: Create SVG files from VMobject and VGroup
 Home-page: https://github.com/naveen521kk/manim-mobject-svg
 License: MIT
 Author: Naveen M K
 Author-email: naveen521kk@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

