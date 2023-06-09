# Comparing `tmp/django_pictures-1.1.1.tar.gz` & `tmp/django_pictures-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_pictures-1.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_pictures-1.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_pictures-1.1.1.tar` & `django_pictures-1.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1324 2023-06-08 06:42:06.891338 django_pictures-1.1.1/LICENSE
--rw-r--r--   0        0        0     9256 2023-06-08 06:42:06.891338 django_pictures-1.1.1/README.md
--rw-r--r--   0        0        0      171 2023-06-08 06:42:06.891338 django_pictures-1.1.1/pictures/__init__.py
--rw-r--r--   0        0        0      160 2023-06-08 06:42:52.298888 django_pictures-1.1.1/pictures/_version.py
--rw-r--r--   0        0        0      155 2023-06-08 06:42:06.891338 django_pictures-1.1.1/pictures/apps.py
--rw-r--r--   0        0        0     1012 2023-06-08 06:42:06.891338 django_pictures-1.1.1/pictures/checks.py
--rw-r--r--   0        0        0      683 2023-06-08 06:42:06.891338 django_pictures-1.1.1/pictures/conf.py
--rw-r--r--   0        0        0        0 2023-06-08 06:42:06.891338 django_pictures-1.1.1/pictures/contrib/__init__.py
--rw-r--r--   0        0        0     2387 2023-06-08 06:42:06.891338 django_pictures-1.1.1/pictures/contrib/rest_framework.py
--rw-r--r--   0        0        0      857 2023-06-08 06:42:43.710974 django_pictures-1.1.1/pictures/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1179 2023-06-08 06:42:06.891338 django_pictures-1.1.1/pictures/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3195 2023-06-08 06:42:06.891338 django_pictures-1.1.1/pictures/migrations.py
--rw-r--r--   0        0        0     8495 2023-06-08 06:42:06.891338 django_pictures-1.1.1/pictures/models.py
--rw-r--r--   0        0        0     3726 2023-06-08 06:42:06.891338 django_pictures-1.1.1/pictures/tasks.py
--rw-r--r--   0        0        0      165 2023-06-08 06:42:06.891338 django_pictures-1.1.1/pictures/templates/pictures/attrs.html
--rw-r--r--   0        0        0      618 2023-06-08 06:42:06.891338 django_pictures-1.1.1/pictures/templates/pictures/picture.html
--rw-r--r--   0        0        0        0 2023-06-08 06:42:06.891338 django_pictures-1.1.1/pictures/templatetags/__init__.py
--rw-r--r--   0        0        0     2281 2023-06-08 06:42:06.891338 django_pictures-1.1.1/pictures/templatetags/pictures.py
--rw-r--r--   0        0        0      214 2023-06-08 06:42:06.891338 django_pictures-1.1.1/pictures/urls.py
--rw-r--r--   0        0        0     4023 2023-06-08 06:42:06.891338 django_pictures-1.1.1/pictures/utils.py
--rw-r--r--   0        0        0     1907 2023-06-08 06:42:06.895338 django_pictures-1.1.1/pictures/validators.py
--rw-r--r--   0        0        0      725 2023-06-08 06:42:06.895338 django_pictures-1.1.1/pictures/views.py
--rw-r--r--   0        0        0     2349 2023-06-08 06:42:06.895338 django_pictures-1.1.1/pyproject.toml
--rw-r--r--   0        0        0    11381 1970-01-01 00:00:00.000000 django_pictures-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1324 2023-06-09 15:51:38.098183 django_pictures-1.1.2/LICENSE
+-rw-r--r--   0        0        0     9256 2023-06-09 15:51:38.098183 django_pictures-1.1.2/README.md
+-rw-r--r--   0        0        0      171 2023-06-09 15:51:38.098183 django_pictures-1.1.2/pictures/__init__.py
+-rw-r--r--   0        0        0      160 2023-06-09 15:52:01.918191 django_pictures-1.1.2/pictures/_version.py
+-rw-r--r--   0        0        0      155 2023-06-09 15:51:38.098183 django_pictures-1.1.2/pictures/apps.py
+-rw-r--r--   0        0        0     1012 2023-06-09 15:51:38.098183 django_pictures-1.1.2/pictures/checks.py
+-rw-r--r--   0        0        0      683 2023-06-09 15:51:38.098183 django_pictures-1.1.2/pictures/conf.py
+-rw-r--r--   0        0        0        0 2023-06-09 15:51:38.098183 django_pictures-1.1.2/pictures/contrib/__init__.py
+-rw-r--r--   0        0        0     2403 2023-06-09 15:51:38.098183 django_pictures-1.1.2/pictures/contrib/rest_framework.py
+-rw-r--r--   0        0        0      857 2023-06-09 15:51:54.422190 django_pictures-1.1.2/pictures/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1179 2023-06-09 15:51:38.098183 django_pictures-1.1.2/pictures/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3195 2023-06-09 15:51:38.098183 django_pictures-1.1.2/pictures/migrations.py
+-rw-r--r--   0        0        0     8495 2023-06-09 15:51:38.098183 django_pictures-1.1.2/pictures/models.py
+-rw-r--r--   0        0        0     3726 2023-06-09 15:51:38.098183 django_pictures-1.1.2/pictures/tasks.py
+-rw-r--r--   0        0        0      165 2023-06-09 15:51:38.098183 django_pictures-1.1.2/pictures/templates/pictures/attrs.html
+-rw-r--r--   0        0        0      618 2023-06-09 15:51:38.098183 django_pictures-1.1.2/pictures/templates/pictures/picture.html
+-rw-r--r--   0        0        0        0 2023-06-09 15:51:38.098183 django_pictures-1.1.2/pictures/templatetags/__init__.py
+-rw-r--r--   0        0        0     2281 2023-06-09 15:51:38.098183 django_pictures-1.1.2/pictures/templatetags/pictures.py
+-rw-r--r--   0        0        0      214 2023-06-09 15:51:38.098183 django_pictures-1.1.2/pictures/urls.py
+-rw-r--r--   0        0        0     4023 2023-06-09 15:51:38.098183 django_pictures-1.1.2/pictures/utils.py
+-rw-r--r--   0        0        0     1907 2023-06-09 15:51:38.098183 django_pictures-1.1.2/pictures/validators.py
+-rw-r--r--   0        0        0      725 2023-06-09 15:51:38.098183 django_pictures-1.1.2/pictures/views.py
+-rw-r--r--   0        0        0     2349 2023-06-09 15:51:38.098183 django_pictures-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0    11381 1970-01-01 00:00:00.000000 django_pictures-1.1.2/PKG-INFO
```

### Comparing `django_pictures-1.1.1/LICENSE` & `django_pictures-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_pictures-1.1.1/README.md` & `django_pictures-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `django_pictures-1.1.1/pictures/checks.py` & `django_pictures-1.1.2/pictures/checks.py`

 * *Files identical despite different names*

### Comparing `django_pictures-1.1.1/pictures/conf.py` & `django_pictures-1.1.2/pictures/conf.py`

 * *Files identical despite different names*

### Comparing `django_pictures-1.1.1/pictures/contrib/rest_framework.py` & `django_pictures-1.1.2/pictures/contrib/rest_framework.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,26 +37,26 @@
             },
         }
         try:
             query_params: QueryDict = self.context["request"].GET
         except KeyError:
             pass
         else:
-            ratio = query_params.get(f"{self.source}_ratio")
-            container = query_params.get(f"{self.source}_container")
+            ratio = query_params.get(f"{self.field_name}_ratio")
+            container = query_params.get(f"{self.field_name}_container")
             try:
                 container = int(container)
             except TypeError:
                 container = None
             except ValueError as e:
                 raise ValueError(f"Container width is not a number: {container}") from e
             breakpoints = {
-                bp: int(query_params.get(f"{self.source}_{bp}"))
+                bp: int(query_params.get(f"{self.field_name}_{bp}"))
                 for bp in get_settings().BREAKPOINTS
-                if f"{self.source}_{bp}" in query_params
+                if f"{self.field_name}_{bp}" in query_params
             }
             if ratio is not None:
                 try:
                     payload["ratios"] = {ratio: payload["ratios"][ratio]}
                 except KeyError as e:
                     raise ValueError(
                         f"Invalid ratio: {ratio}. Choices are: {', '.join(filter(None, obj.aspect_ratios.keys()))}"
```

### Comparing `django_pictures-1.1.1/pictures/locale/de/LC_MESSAGES/django.mo` & `django_pictures-1.1.2/pictures/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_pictures-1.1.1/pictures/locale/de/LC_MESSAGES/django.po` & `django_pictures-1.1.2/pictures/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_pictures-1.1.1/pictures/migrations.py` & `django_pictures-1.1.2/pictures/migrations.py`

 * *Files identical despite different names*

### Comparing `django_pictures-1.1.1/pictures/models.py` & `django_pictures-1.1.2/pictures/models.py`

 * *Files identical despite different names*

### Comparing `django_pictures-1.1.1/pictures/tasks.py` & `django_pictures-1.1.2/pictures/tasks.py`

 * *Files identical despite different names*

### Comparing `django_pictures-1.1.1/pictures/templates/pictures/picture.html` & `django_pictures-1.1.2/pictures/templates/pictures/picture.html`

 * *Files identical despite different names*

### Comparing `django_pictures-1.1.1/pictures/templatetags/pictures.py` & `django_pictures-1.1.2/pictures/templatetags/pictures.py`

 * *Files identical despite different names*

### Comparing `django_pictures-1.1.1/pictures/utils.py` & `django_pictures-1.1.2/pictures/utils.py`

 * *Files identical despite different names*

### Comparing `django_pictures-1.1.1/pictures/validators.py` & `django_pictures-1.1.2/pictures/validators.py`

 * *Files identical despite different names*

### Comparing `django_pictures-1.1.1/pictures/views.py` & `django_pictures-1.1.2/pictures/views.py`

 * *Files identical despite different names*

### Comparing `django_pictures-1.1.1/pyproject.toml` & `django_pictures-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django_pictures-1.1.1/PKG-INFO` & `django_pictures-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pictures
-Version: 1.1.1
+Version: 1.1.2
 Summary: Responsive cross-browser image library using modern codes like AVIF & WebP.
 Keywords: pillow,Django,image,pictures,WebP,AVIF
 Author-email: Johannes Maron <johannes@maron.family>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

