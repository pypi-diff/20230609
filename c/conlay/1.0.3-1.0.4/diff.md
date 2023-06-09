# Comparing `tmp/conlay-1.0.3.tar.gz` & `tmp/conlay-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conlay-1.0.3.tar", last modified: Fri Jun  9 13:46:02 2023, max compression
+gzip compressed data, was "conlay-1.0.4.tar", last modified: Fri Jun  9 14:34:46 2023, max compression
```

## Comparing `conlay-1.0.3.tar` & `conlay-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 13:46:02.779812 conlay-1.0.3/
--rw-rw-rw-   0        0        0     1085 2023-06-09 13:08:51.000000 conlay-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     1555 2023-06-09 13:46:02.778312 conlay-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1250 2023-06-09 13:25:18.000000 conlay-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 13:46:02.770311 conlay-1.0.3/conlay/
--rw-rw-rw-   0        0        0       19 2023-06-09 13:30:45.000000 conlay-1.0.3/conlay/__init__.py
--rw-rw-rw-   0        0        0    11531 2023-06-09 11:38:45.000000 conlay-1.0.3/conlay/main.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:46:02.776812 conlay-1.0.3/conlay.egg-info/
--rw-rw-rw-   0        0        0     1555 2023-06-09 13:46:02.000000 conlay-1.0.3/conlay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2023-06-09 13:46:02.000000 conlay-1.0.3/conlay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 13:46:02.000000 conlay-1.0.3/conlay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-09 13:46:02.000000 conlay-1.0.3/conlay.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 13:46:02.780312 conlay-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      568 2023-06-09 13:44:29.000000 conlay-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 14:34:46.928444 conlay-1.0.4/
+-rw-rw-rw-   0        0        0     1085 2023-06-09 13:08:51.000000 conlay-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1543 2023-06-09 14:34:46.926823 conlay-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-06-09 14:30:21.000000 conlay-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 14:34:46.919322 conlay-1.0.4/conlay/
+-rw-rw-rw-   0        0        0       19 2023-06-09 13:59:21.000000 conlay-1.0.4/conlay/__init__.py
+-rw-rw-rw-   0        0        0    11535 2023-06-09 14:30:53.000000 conlay-1.0.4/conlay/main.py
+drwxrwxrwx   0        0        0        0 2023-06-09 14:34:46.925823 conlay-1.0.4/conlay.egg-info/
+-rw-rw-rw-   0        0        0     1543 2023-06-09 14:34:46.000000 conlay-1.0.4/conlay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2023-06-09 14:34:46.000000 conlay-1.0.4/conlay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 14:34:46.000000 conlay-1.0.4/conlay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-09 14:34:46.000000 conlay-1.0.4/conlay.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 14:34:46.928444 conlay-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      685 2023-06-09 14:31:29.000000 conlay-1.0.4/setup.py
```

### Comparing `conlay-1.0.3/LICENSE` & `conlay-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `conlay-1.0.3/PKG-INFO` & `conlay-1.0.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,50 +1,52 @@
-Metadata-Version: 2.1
-Name: conlay
-Version: 1.0.3
-Summary: A python library for creating nice layouts in the console environment
-Home-page: https://github.com/Salliii/conlay
-Author: Salliii
-Keywords: python,library,console,layout
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 Conlay - Console Layout
 =======================
 
 [![PyPi version][shields-pypi_version]][url-pypi_version]
 [![Github Issues][shields-issues]][url-issues]
 [![Github License][shields-license]][url-license]
 
 Create visually pleasing console layouts with this easy-to-use Python library. 
 
-___________________________________________________________________________________________________
-
 
 Installing
 ----------
 
 Install using <a href="https://pip.pypa.io/en/stable/">pip</a>
 
 ```bash
 pip install conlay
 ```
 
 or install it from <a href="https://pypi.org/project/conlay/#files">PyPi</a>
 
-___________________________________________________________________________________________________
 
-Getting Started
----------------
+Example
+-------
+
+```python
+from conlay import *
+
+layout = Conlay()
+
+blank_box = BoldBox(0, 0, 30, 5)
+layout.add(blank_box)
+
+label = ThinLabel(0, 0, "this is a test")
+blank_box.add(label)
+
+layout.print()
+``` 
+
 
 
 
 
 <!-- shields -->
 [shields-pypi_version]: https://img.shields.io/pypi/v/conlay?label=PyPi%20Version&style=for-the-badge
 [shields-issues]: https://img.shields.io/github/issues/Salliii/conlay?style=for-the-badge
 [shields-license]: https://img.shields.io/github/license/Salliii/conlay?style=for-the-badge
 
 <!-- url -->
 [url-pypi_version]: https://pypi.org/project/conlay/
 [url-issues]: https://github.com/Salliii/conlay/issues
-[url-license]: https://github.com/Salliii/conlay/blob/main/LICENSE
+[url-license]: https://github.com/Salliii/conlay/blob/main/LICENSE
```

#### html2text {}

```diff
@@ -1,19 +1,14 @@
-Metadata-Version: 2.1 Name: conlay Version: 1.0.3 Summary: A python library for
-creating nice layouts in the console environment Home-page: https://github.com/
-Salliii/conlay Author: Salliii Keywords: python,library,console,layout
-Description-Content-Type: text/markdown License-File: LICENSE Conlay - Console
-Layout ======================= [![PyPi version][shields-pypi_version]][url-
-pypi_version] [![Github Issues][shields-issues]][url-issues] [![Github License]
-[shields-license]][url-license] Create visually pleasing console layouts with
-this easy-to-use Python library.
-___________________________________________________________________________________________________
-Installing ---------- Install using pip ```bash pip install conlay ``` or
-install it from PyPi
-___________________________________________________________________________________________________
-Getting Started ---------------  [shields-pypi_version]: https://
-img.shields.io/pypi/v/conlay?label=PyPi%20Version&style=for-the-badge [shields-
-issues]: https://img.shields.io/github/issues/Salliii/conlay?style=for-the-
-badge [shields-license]: https://img.shields.io/github/license/Salliii/
-conlay?style=for-the-badge  [url-pypi_version]: https://pypi.org/project/
-conlay/ [url-issues]: https://github.com/Salliii/conlay/issues [url-license]:
-https://github.com/Salliii/conlay/blob/main/LICENSE
+Conlay - Console Layout ======================= [![PyPi version][shields-
+pypi_version]][url-pypi_version] [![Github Issues][shields-issues]][url-issues]
+[![Github License][shields-license]][url-license] Create visually pleasing
+console layouts with this easy-to-use Python library. Installing ---------
+- Install using pip ```bash pip install conlay ``` or install it from PyPi
+Example ------- ```python from conlay import * layout = Conlay() blank_box =
+BoldBox(0, 0, 30, 5) layout.add(blank_box) label = ThinLabel(0, 0, "this is a
+test") blank_box.add(label) layout.print() ```  [shields-pypi_version]: https:/
+/img.shields.io/pypi/v/conlay?label=PyPi%20Version&style=for-the-badge
+[shields-issues]: https://img.shields.io/github/issues/Salliii/
+conlay?style=for-the-badge [shields-license]: https://img.shields.io/github/
+license/Salliii/conlay?style=for-the-badge  [url-pypi_version]: https://
+pypi.org/project/conlay/ [url-issues]: https://github.com/Salliii/conlay/issues
+[url-license]: https://github.com/Salliii/conlay/blob/main/LICENSE
```

### Comparing `conlay-1.0.3/conlay/main.py` & `conlay-1.0.4/conlay/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,15 +185,15 @@
     """ main layout """
 
     # child list
     childs = []
 
     # reset console and set cursor to (0, 0) after class call
     Console.reset()
-    Cursor.setPosition(0, 0)
+    Cursor.setPosition(1, 1)
 
     def __init__(self) -> None:
         # class attributes
         self.relative_x = int()
         self.relative_y = int()
         self.absolute_x = int()
         self.absolute_y = int()
@@ -272,15 +272,15 @@
                 pass
             
 
             # iterate through y axis
             for y in range(element.height):
 
                 # set cursors position
-                Cursor.setPosition(element.absolute_x, element.absolute_y + y + 1)
+                Cursor.setPosition(element.absolute_x, element.absolute_y + y)
 
 
                 # iterate through x axis
                 for x in range(element.width):
 
                     # print top left border
                     if x == 0 and y == 0:
@@ -326,18 +326,18 @@
 
 
 
 class LayoutElement(Conlay):
     def __init__(self, x:int, y:int, w:int, h:int, border:Border) -> None:
         super().__init__()
 
-        self.relative_x = x
-        self.relative_y = y
-        self.width = w + 2
-        self.height = h + 2
+        self.relative_x = x + 1
+        self.relative_y = y + 1
+        self.width = w
+        self.height = h
         self.border = border
 
 
 
 
 class Box(LayoutElement):
     def __init__(self, x:int, y:int, w:int, h:int, border:Border) -> None:
@@ -371,16 +371,16 @@
 
         super().__init__(x, y, w, h, border)
 
         self.text = text
 
 
     def __preprint__(self) -> int:
-        self.width = self.width + self.padding_x * 2
-        self.height = self.height + self.padding_y * 2
+        self.width = self.width + self.padding_x * 2 + 2
+        self.height = self.height + self.padding_y * 2 + 2
 
         return 1
 
 
     def __pastprint__(self) -> int:
         Cursor.setPosition(self.absolute_x + 1 + self.padding_x, self.absolute_y + 1 + self.padding_y)
         print(self.text, end="")
```

