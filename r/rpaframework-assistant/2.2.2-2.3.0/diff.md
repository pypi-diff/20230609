# Comparing `tmp/rpaframework_assistant-2.2.2.tar.gz` & `tmp/rpaframework_assistant-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpaframework_assistant-2.2.2.tar", max compression
+gzip compressed data, was "rpaframework_assistant-2.3.0.tar", max compression
```

## Comparing `rpaframework_assistant-2.2.2.tar` & `rpaframework_assistant-2.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11358 2023-02-08 14:04:37.406505 rpaframework_assistant-2.2.2/LICENSE
--rw-r--r--   0        0        0      288 2023-02-08 14:04:37.406609 rpaframework_assistant-2.2.2/README.rst
--rw-r--r--   0        0        0     2456 2023-05-12 07:53:19.051682 rpaframework_assistant-2.2.2/pyproject.toml
--rw-r--r--   0        0        0       94 2023-03-02 10:36:58.328764 rpaframework_assistant-2.2.2/src/RPA/Assistant/__init__.py
--rw-r--r--   0        0        0     3387 2023-04-04 10:42:49.583449 rpaframework_assistant-2.2.2/src/RPA/Assistant/background_flet.py
--rw-r--r--   0        0        0     5168 2023-04-04 10:42:49.583708 rpaframework_assistant-2.2.2/src/RPA/Assistant/callback_runner.py
--rw-r--r--   0        0        0    11936 2023-04-04 10:42:49.584044 rpaframework_assistant-2.2.2/src/RPA/Assistant/flet_client.py
--rw-r--r--   0        0        0    52984 2023-05-12 07:53:48.535675 rpaframework_assistant-2.2.2/src/RPA/Assistant/library.py
--rw-r--r--   0        0        0     1530 2023-03-14 14:53:39.551068 rpaframework_assistant-2.2.2/src/RPA/Assistant/types.py
--rw-r--r--   0        0        0     3646 2023-03-14 09:01:07.895769 rpaframework_assistant-2.2.2/src/RPA/Assistant/utils.py
--rw-r--r--   0        0        0     1829 1970-01-01 00:00:00.000000 rpaframework_assistant-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-02-08 22:30:10.093540 rpaframework_assistant-2.3.0/LICENSE
+-rw-r--r--   0        0        0      288 2023-02-08 22:30:10.093718 rpaframework_assistant-2.3.0/README.rst
+-rw-r--r--   0        0        0     2456 2023-06-09 08:55:37.434752 rpaframework_assistant-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0       94 2023-03-14 14:16:25.880080 rpaframework_assistant-2.3.0/src/RPA/Assistant/__init__.py
+-rw-r--r--   0        0        0     3387 2023-05-31 09:03:32.486581 rpaframework_assistant-2.3.0/src/RPA/Assistant/background_flet.py
+-rw-r--r--   0        0        0     5168 2023-04-11 14:11:24.774147 rpaframework_assistant-2.3.0/src/RPA/Assistant/callback_runner.py
+-rw-r--r--   0        0        0    11936 2023-04-11 14:11:24.774258 rpaframework_assistant-2.3.0/src/RPA/Assistant/flet_client.py
+-rw-r--r--   0        0        0    55865 2023-06-09 08:55:37.435338 rpaframework_assistant-2.3.0/src/RPA/Assistant/library.py
+-rw-r--r--   0        0        0     1530 2023-03-14 14:16:25.880895 rpaframework_assistant-2.3.0/src/RPA/Assistant/types.py
+-rw-r--r--   0        0        0     3646 2023-03-14 14:16:25.881009 rpaframework_assistant-2.3.0/src/RPA/Assistant/utils.py
+-rw-r--r--   0        0        0     1679 1970-01-01 00:00:00.000000 rpaframework_assistant-2.3.0/PKG-INFO
```

### Comparing `rpaframework_assistant-2.2.2/LICENSE` & `rpaframework_assistant-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rpaframework_assistant-2.2.2/pyproject.toml` & `rpaframework_assistant-2.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rpaframework-assistant"
-version = "2.2.2"
+version = "2.3.0"
 description = "Interactive UI library for RPA Framework"
 authors = ["RPA Framework <rpafw@robocorp.com>"]
 license = "Apache-2.0"
 readme = "README.rst"
 
 homepage = "https://rpaframework.org/"
 documentation = "https://rpaframework.org/"
```

### Comparing `rpaframework_assistant-2.2.2/src/RPA/Assistant/background_flet.py` & `rpaframework_assistant-2.3.0/src/RPA/Assistant/background_flet.py`

 * *Files identical despite different names*

### Comparing `rpaframework_assistant-2.2.2/src/RPA/Assistant/callback_runner.py` & `rpaframework_assistant-2.3.0/src/RPA/Assistant/callback_runner.py`

 * *Files identical despite different names*

### Comparing `rpaframework_assistant-2.2.2/src/RPA/Assistant/flet_client.py` & `rpaframework_assistant-2.3.0/src/RPA/Assistant/flet_client.py`

 * *Files identical despite different names*

### Comparing `rpaframework_assistant-2.2.2/src/RPA/Assistant/library.py` & `rpaframework_assistant-2.3.0/src/RPA/Assistant/library.py`

 * *Files 3% similar despite different names*

```diff
@@ -1263,21 +1263,91 @@
             label=thumb_text,
             value=default,
             round=decimals,
         )
         self._client.add_element(name=name, element=slider)
 
     @keyword(tags=["dialog", "running"])
+    def add_loading_spinner(
+        self,
+        name: str,
+        width: int = 16,
+        height: int = 16,
+        stroke_width: int = 2,
+        color: Optional[str] = None,
+        tooltip: Optional[str] = None,
+        value: Optional[float] = None,
+    ):
+        """Add a loading spinner.
+
+        :param name:        Name of the element
+        :param width:       Width of the spinner
+        :param height:      Height of the spinner
+        :param stroke_width: Width of the spinner's stroke
+        :param color:       Color of the spinner's stroke.
+                            Allowed values are colors from
+                            [https://github.com/flet-dev/flet/blob/035b00104f782498d084c2fd7ee96132a542ab7f/sdk/python/packages/flet-core/src/flet_core/colors.py#L37|Flet Documentation] (in the format ``black12``, ``red500``)
+                            or ARGB/RGB (#FFXXYYZZ or #XXYYZZ).XXYYZZ
+        :param tooltip:     Tooltip to be displayed
+                            on mouse hover.
+        :param value:       Between 0.0 and 1.0 if you want to manually control it's completion.
+                            If `None` it will spin endlessy.
+        """  # noqa: E501
+        pr = flet.ProgressRing(
+            width=width,
+            height=height,
+            stroke_width=stroke_width,
+            color=color,
+            tooltip=tooltip,
+            value=value,
+        )
+        self._client.add_element(pr, name)
+        return pr
+
+    @keyword(tags=["dialog", "running"])
+    def add_loading_bar(
+        self,
+        name: str,
+        width: int = 16,
+        bar_height: int = 16,
+        color: Optional[str] = None,
+        tooltip: Optional[str] = None,
+        value: Optional[float] = None,
+    ):
+        """Add a loading bar.
+
+        :param name:        Name of the element
+        :param width:       Width of the bar
+        :param bar_height:  Height of the bar
+        :param color:       Color of the bar's stroke.
+                            Allowed values are colors from
+                            [https://github.com/flet-dev/flet/blob/035b00104f782498d084c2fd7ee96132a542ab7f/sdk/python/packages/flet-core/src/flet_core/colors.py#L37|Flet Documentation] (in the format ``black12``, ``red500``)
+                            or ARGB/RGB (#FFXXYYZZ or #XXYYZZ).XXYYZZ
+        :param tooltip:     Tooltip to be displayed on mouse hover.
+        :param value:       Between 0.0 and 1.0 if you want to manually control it's completion.
+                            Use `None` for indeterminate progress indicator.
+        """  # noqa: E501
+        pb = flet.ProgressBar(
+            width=width,
+            bar_height=bar_height,
+            color=color,
+            tooltip=tooltip,
+            value=value,
+        )
+        self._client.add_element(pb, name)
+        return pb
+
+    @keyword(tags=["dialog", "running"])
     def set_title(self, title: str):
         """Set dialog title when it is running."""
         self._client.set_title(title)
 
     def _close_layouting_element(self, layouting_element: str):
-        """Checkhat if the last opened layout element matches what is being closed,
-        otherwise raise ValueError. If the check passes, close the layout element.
+        """Check if the last opened layout element matches what is being closed,
+        otherwise raise `ValueError`. If the check passes, close the layout element.
         """
         if not self._open_layouting:
             raise LayoutError(f"Cannot close {layouting_element}, no open layout")
 
         last_opened = self._open_layouting[-1]
         if not last_opened == layouting_element:
             raise LayoutError(
```

### Comparing `rpaframework_assistant-2.2.2/src/RPA/Assistant/types.py` & `rpaframework_assistant-2.3.0/src/RPA/Assistant/types.py`

 * *Files identical despite different names*

### Comparing `rpaframework_assistant-2.2.2/src/RPA/Assistant/utils.py` & `rpaframework_assistant-2.3.0/src/RPA/Assistant/utils.py`

 * *Files identical despite different names*

### Comparing `rpaframework_assistant-2.2.2/PKG-INFO` & `rpaframework_assistant-2.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpaframework-assistant
-Version: 2.2.2
+Version: 2.3.0
 Summary: Interactive UI library for RPA Framework
 Home-page: https://rpaframework.org/
 License: Apache-2.0
 Keywords: robotframework,rpa,automation,dialogs,assistant
 Author: RPA Framework
 Author-email: rpafw@robocorp.com
 Requires-Python: >=3.7,<4.0
@@ -16,17 +16,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: flet (==0.4.2)
 Requires-Dist: robotframework (>=4.0.0,!=4.0.1,<6.0.0)
 Requires-Dist: rpaframework-core (>=11.0.0,<12.0.0)
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
 Project-URL: Documentation, https://rpaframework.org/
```

