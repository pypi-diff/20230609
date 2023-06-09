# Comparing `tmp/manim_mobject_svg-0.2.0.tar.gz` & `tmp/manim_mobject_svg-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manim_mobject_svg-0.2.0.tar", max compression
+gzip compressed data, was "manim_mobject_svg-0.3.0.tar", max compression
```

## Comparing `manim_mobject_svg-0.2.0.tar` & `manim_mobject_svg-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1088 2023-01-31 14:46:17.167455 manim_mobject_svg-0.2.0/LICENSE
--rw-r--r--   0        0        0      628 2023-01-31 14:47:34.595658 manim_mobject_svg-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1008 2023-01-26 11:54:58.661866 manim_mobject_svg-0.2.0/README.md
--rw-r--r--   0        0        0      210 2023-01-26 11:43:20.625741 manim_mobject_svg-0.2.0/src/manim_mobject_svg/__init__.py
--rw-r--r--   0        0        0     5072 2023-01-31 14:39:04.136625 manim_mobject_svg-0.2.0/src/manim_mobject_svg/svg.py
--rw-r--r--   0        0        0     1895 1970-01-01 00:00:00.000000 manim_mobject_svg-0.2.0/setup.py
--rw-r--r--   0        0        0     1728 1970-01-01 00:00:00.000000 manim_mobject_svg-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-09 16:03:41.454657 manim_mobject_svg-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1479 2023-06-09 16:03:41.454657 manim_mobject_svg-0.3.0/README.md
+-rw-r--r--   0        0        0      603 2023-06-09 16:03:41.454657 manim_mobject_svg-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      203 2023-06-09 16:03:41.454657 manim_mobject_svg-0.3.0/src/manim_mobject_svg/__init__.py
+-rw-r--r--   0        0        0     6694 2023-06-09 16:03:41.454657 manim_mobject_svg-0.3.0/src/manim_mobject_svg/svg.py
+-rw-r--r--   0        0        0     2229 1970-01-01 00:00:00.000000 manim_mobject_svg-0.3.0/PKG-INFO
```

### Comparing `manim_mobject_svg-0.2.0/LICENSE` & `manim_mobject_svg-0.3.0/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Naveen M K
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Naveen M K
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `manim_mobject_svg-0.2.0/PKG-INFO` & `manim_mobject_svg-0.3.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,63 @@
 Metadata-Version: 2.1
 Name: manim-mobject-svg
-Version: 0.2.0
+Version: 0.3.0
 Summary: Create SVG files from VMobject and VGroup
 Home-page: https://github.com/naveen521kk/manim-mobject-svg
 License: MIT
 Author: Naveen M K
 Author-email: naveen521kk@gmail.com
-Requires-Python: >=3.8,<=3.11
+Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: manim (>=0.16.0)
 Requires-Dist: pycairo (>=1,<2)
 Project-URL: Repository, https://github.com/naveen521kk/manim-mobject-svg
 Description-Content-Type: text/markdown
 
 # manim-mobject-svg
 
-Create SVG files from [VMobject](https://docs.manim.community/en/stable/reference/manim.mobject.types.vectorized_mobject.VMobject.html).
+Create SVG files from [VMobject](https://docs.manim.community/en/stable/reference/manim.mobject.types.vectorized_mobject.VMobject.html) and [VGroup](https://docs.manim.community/en/stable/reference/manim.mobject.types.vectorized_mobject.VGroup.html).
 
 Install: `pip install manim-mobject-svg`
 
 Here's an example of how to use this plugin:
 
 ```python
 from manim import *
 from manim_mobject_svg import *
 
 a = Square(color=BLUE)
 a.to_svg("square.svg")
 ```
 This should create a file `square.svg` in the current directory and return the path to the file. The output should look like this:
-![svg square manim](https://user-images.githubusercontent.com/49693820/214828793-bf764d46-93b2-4622-bd1e-c68c42206b46.svg)
+
+![svg square manim](https://github.com/naveen521kk/manim-mobject-svg/assets/49693820/ba232f4c-7a11-4d6f-b36e-7c49867bc6a8)
 
 It's also possible to create a SVG file for VGroup.
 
 ```python
 from manim import *
 from manim_mobject_svg import *
 
 a = Square(color=BLUE)
 b = Circle(color=RED)
 c = VGroup(a, b)
 c.to_svg("group.svg")
 ```
 It'll create a SVG file like this:
-![svg vgroup manim](https://user-images.githubusercontent.com/49693820/214829098-6680ca28-6f2b-4bb6-b376-f7858532c1c3.svg)
+
+![svg vgroup manim](https://github.com/naveen521kk/manim-mobject-svg/assets/49693820/4073c65f-0397-450a-90d6-6a2226dade15)
+
+## Parameters for `to_svg()`
+
+`to_svg()` takes the following parameters:
+- `path`: Path to the SVG file to be created. If not specified, it'll create a temporary file and return the path to the file.
+- `crop`: Crop the SVG file to the bounding box of the VMobject. Default: `True`
+- `padding`: Padding around the VMobject. Default: `0.5`
+
+This method returns the path to the SVG file.
```

