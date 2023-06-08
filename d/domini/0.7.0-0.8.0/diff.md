# Comparing `tmp/domini-0.7.0.tar.gz` & `tmp/domini-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domini-0.7.0.tar", max compression
+gzip compressed data, was "domini-0.8.0.tar", max compression
```

## Comparing `domini-0.7.0.tar` & `domini-0.8.0.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0    35066 2022-09-30 02:05:07.299772 domini-0.7.0/LICENSE
--rw-r--r--   0        0        0     1411 2023-04-15 00:45:13.796552 domini-0.7.0/README.md
--rw-r--r--   0        0        0        0 2023-04-15 00:46:21.435310 domini-0.7.0/domini/__init__.py
--rw-r--r--   0        0        0    16388 2023-04-15 00:38:47.966969 domini-0.7.0/domini/html.py
--rw-r--r--   0        0        0      418 2023-04-15 00:42:22.126370 domini-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     2040 1970-01-01 00:00:00.000000 domini-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    35066 2022-09-30 02:05:07.299772 domini-0.8.0/LICENSE
+-rw-r--r--   0        0        0     2070 2023-06-08 23:04:06.895144 domini-0.8.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-15 00:46:21.435310 domini-0.8.0/domini/__init__.py
+-rw-r--r--   0        0        0       19 2023-06-08 14:31:26.952321 domini-0.8.0/domini/html/__init__.py
+-rw-r--r--   0        0        0     2139 2023-06-08 22:40:23.979848 domini-0.8.0/domini/html/events.py
+-rw-r--r--   0        0        0    16293 2023-06-08 14:49:43.940214 domini-0.8.0/domini/html/tags.py
+-rw-r--r--   0        0        0      418 2023-06-08 23:04:35.254714 domini-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     2699 1970-01-01 00:00:00.000000 domini-0.8.0/PKG-INFO
```

### Comparing `domini-0.7.0/LICENSE` & `domini-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `domini-0.7.0/domini/html.py` & `domini-0.8.0/domini/html/tags.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import re
 from contextlib import suppress
-from typing import Any, Sequence, Iterator, Generator, Union
+from typing import Any, Iterable, Union
 
 
 def conform_attribute_name(key: str) -> str:
     """
     Format an attribute name to fit the standard.
     """
     key = key.strip('_')
@@ -69,15 +69,15 @@
     # Close tag off if content is provided
     if content is not None:
         return f'{elm}>{content}</{tag}>'
     else:
         return f'{elm}>'
 
 
-Content = Union[str, 'HTMLTag', Sequence, Iterator, Generator]
+Content = Union[str, 'HTMLTag', Iterable]
 
 
 class HTMLTag:
     """
     Base class for all HTML tags
 
     Inherit from it to define a new tag type.
@@ -119,17 +119,17 @@
 
         # Add children
 
         # o) Strings and HTML tags are obviously singular
         if isinstance(content, (str, HTMLTag)):
             return copy.add(content)
         
-        # o) Any other sequence, iterator, or generator
-        # should be unravelled and have its elements added
-        if isinstance(content, (Sequence, Iterator, Generator)):
+        # o) Any iterable should be unravelled
+        # and have its elements added
+        if isinstance(content, Iterable):
             return copy.add(*content)
         
         # o) Anything else, add it singularly
         return copy.add(content)
 
     def __contains__(self, attribute: str, /) -> bool:
         """
```

### Comparing `domini-0.7.0/PKG-INFO` & `domini-0.8.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domini
-Version: 0.7.0
+Version: 0.8.0
 Summary: Create HTML documents using Pythonic syntax that mimics the real deal.
 Home-page: https://gitlab.com/deepadmax/domini
 License: GPL-3.0-or-later
 Author: Maximillian Strand
 Author-email: maxi@millian.se
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -15,14 +15,20 @@
 Description-Content-Type: text/markdown
 
 # Domini
 
 A small, simple package for generating HTML documents.
 The syntax aims to immitate HTML as closely as possible for legibility and easy of use.
 
+### Index
+
+- [Attributes](#attributes)
+- [Content](#content)
+- [Extras](#extras)
+
 ## Attributes
 
 Attributes *without* a value are entered as *positional arguments*.<br>
 Attributes *with* a value are entered as *keyword arguments*.
 
 To specify attributes that collide with reserved Python keywords,
 append an underscore and it will be removed.
@@ -39,30 +45,48 @@
 
 ```html
 <dialog open class='mydialog'>
 ```
 
 ## Content
 
-To add children to an element, you can use either the `add` method or the short-hand greater-than operator. The right-hand side can be either any sequence, iterator, or generator of elements or a lone element. These elements can be either other tags or plain strings.
+To add children to an element, you can use either the `add` method or the short-hand greater-than operator. The right-hand side can be either an iterable or a lone element. These elements can be either other tags or plain strings.
 
 **NOTE**: `add` does add them to the current object. `>` returns a new, identical element with those children added.
 
 ```py
 ul(class_='todo')> (
     li()> 'Buy a fruit basket.',
     li()> (
         'Read ', a(href='https://wikipedia.org/')> 'Wikipedia',
-        ' to learn more about things you may have not otherwise cared about.',
+        ' to learn more about things you may not have otherwise cared about.',
     ),
 )
 ```
 
 ## Closing tags
 
 A tag is only closed if content is provided. E.g. `<p></p>` as opposed to `<p>`. This can be an empty tuple.
 
 ```py
-section()> ()
+p()> ()
 ```
 
 For open tags like `<br>` and `<hr>`, you simply do `br()` and `hr()`.
+
+## Extras
+
+These are small, miscellaneous additions that can be useful but don't really serve any wider purpose within the context of the package itself. Though this might change in the future.
+
+### Event attributes
+
+Enumerators for event attributes are available at `domini.html.events`. You can either use `Event`, which contains all different event attributes in one, or use an enumerator for a specific category of events.
+
+```py
+from domini.html.events import (
+    # These are the categories.
+    WindowEvent, FormEvent, KeyboardEvent,
+    MouseEvent, DragEvent, ClipboardEvent,
+    MediaEvent, MiscEvent,
+)
+```
+
```

