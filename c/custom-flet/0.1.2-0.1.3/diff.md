# Comparing `tmp/custom_flet-0.1.2.tar.gz` & `tmp/custom_flet-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom_flet-0.1.2.tar", last modified: Thu Jun  8 16:21:17 2023, max compression
+gzip compressed data, was "custom_flet-0.1.3.tar", last modified: Fri Jun  9 09:41:09 2023, max compression
```

## Comparing `custom_flet-0.1.2.tar` & `custom_flet-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 16:21:17.658264 custom_flet-0.1.2/
--rw-rw-rw-   0        0        0      184 2023-06-08 16:21:17.658264 custom_flet-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-08 16:21:17.638145 custom_flet-0.1.2/custom_flet/
--rw-rw-rw-   0        0        0      187 2023-06-08 16:12:15.000000 custom_flet-0.1.2/custom_flet/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 16:21:17.657151 custom_flet-0.1.2/custom_flet/components/
--rw-rw-rw-   0        0        0      154 2023-06-08 14:29:04.000000 custom_flet-0.1.2/custom_flet/components/__init__.py
--rw-rw-rw-   0        0        0      607 2023-06-07 13:30:58.000000 custom_flet-0.1.2/custom_flet/components/custom_icon.py
--rw-rw-rw-   0        0        0      962 2023-06-07 13:36:18.000000 custom_flet-0.1.2/custom_flet/components/custom_icon_button.py
--rw-rw-rw-   0        0        0     2102 2023-06-08 16:10:36.000000 custom_flet-0.1.2/custom_flet/components/elevated_custom_logo_button.py
-drwxrwxrwx   0        0        0        0 2023-06-08 16:21:17.653150 custom_flet-0.1.2/custom_flet.egg-info/
--rw-rw-rw-   0        0        0      184 2023-06-08 16:21:17.000000 custom_flet-0.1.2/custom_flet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      344 2023-06-08 16:21:17.000000 custom_flet-0.1.2/custom_flet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 16:21:17.000000 custom_flet-0.1.2/custom_flet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-08 16:21:17.000000 custom_flet-0.1.2/custom_flet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-08 16:21:17.658264 custom_flet-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      324 2023-06-08 16:21:05.000000 custom_flet-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:41:09.556306 custom_flet-0.1.3/
+-rw-rw-rw-   0        0        0      184 2023-06-09 09:41:09.555314 custom_flet-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-09 09:41:09.520270 custom_flet-0.1.3/custom_flet/
+-rw-rw-rw-   0        0        0      187 2023-06-08 16:12:15.000000 custom_flet-0.1.3/custom_flet/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:41:09.554311 custom_flet-0.1.3/custom_flet/components/
+-rw-rw-rw-   0        0        0      154 2023-06-08 14:29:04.000000 custom_flet-0.1.3/custom_flet/components/__init__.py
+-rw-rw-rw-   0        0        0      607 2023-06-07 13:30:58.000000 custom_flet-0.1.3/custom_flet/components/custom_icon.py
+-rw-rw-rw-   0        0        0      962 2023-06-07 13:36:18.000000 custom_flet-0.1.3/custom_flet/components/custom_icon_button.py
+-rw-rw-rw-   0        0        0     2128 2023-06-09 09:40:59.000000 custom_flet-0.1.3/custom_flet/components/elevated_custom_logo_button.py
+drwxrwxrwx   0        0        0        0 2023-06-09 09:41:09.536176 custom_flet-0.1.3/custom_flet.egg-info/
+-rw-rw-rw-   0        0        0      184 2023-06-09 09:41:09.000000 custom_flet-0.1.3/custom_flet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      344 2023-06-09 09:41:09.000000 custom_flet-0.1.3/custom_flet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 09:41:09.000000 custom_flet-0.1.3/custom_flet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-09 09:41:09.000000 custom_flet-0.1.3/custom_flet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 09:41:09.556306 custom_flet-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      324 2023-06-09 09:40:59.000000 custom_flet-0.1.3/setup.py
```

### Comparing `custom_flet-0.1.2/custom_flet/components/custom_icon.py` & `custom_flet-0.1.3/custom_flet/components/custom_icon.py`

 * *Files identical despite different names*

### Comparing `custom_flet-0.1.2/custom_flet/components/custom_icon_button.py` & `custom_flet-0.1.3/custom_flet/components/custom_icon_button.py`

 * *Files identical despite different names*

### Comparing `custom_flet-0.1.2/custom_flet/components/elevated_custom_logo_button.py` & `custom_flet-0.1.3/custom_flet/components/elevated_custom_logo_button.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 class ElevatedCustomLogoButton(ft.UserControl):
     def __init__(
             self,
             text: str,
             icon: str,
             size: Union[int, None] = 21,
-            font_family: str = None,
-            icon_color: str = "white",
+            font_family: Union[str, None] = None,
+            icon_color: Union[str, None] = "white",
             button_color: Union[str, None] = "green",
             text_color: Union[str, None] = "white",
             border_radius: Union[int, None] = 5,
             icon_at_end: Union[bool, None] = True,
             ref: Union[ft.Ref, None] = None
     ):
         super().__init__()
```

