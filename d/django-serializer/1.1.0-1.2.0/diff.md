# Comparing `tmp/django-serializer-1.1.0.tar.gz` & `tmp/django-serializer-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-serializer-1.1.0.tar", last modified: Sun Mar 19 18:51:55 2023, max compression
+gzip compressed data, was "django-serializer-1.2.0.tar", last modified: Fri Jun  9 12:06:17 2023, max compression
```

## Comparing `django-serializer-1.1.0.tar` & `django-serializer-1.2.0.tar`

### file list

```diff
@@ -1,52 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 18:51:55.802844 django-serializer-1.1.0/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1108 2023-03-19 18:51:44.000000 django-serializer-1.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-03-19 18:51:55.802844 django-serializer-1.1.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2361 2023-03-19 18:51:44.000000 django-serializer-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 18:51:55.798844 django-serializer-1.1.0/django_serializer/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-19 18:51:44.000000 django-serializer-1.1.0/django_serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-03-19 18:51:44.000000 django-serializer-1.1.0/django_serializer/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-03-19 18:51:44.000000 django-serializer-1.1.0/django_serializer/base_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-03-19 18:51:44.000000 django-serializer-1.1.0/django_serializer/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 18:51:55.802844 django-serializer-1.1.0/django_serializer/form/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 18:51:44.000000 django-serializer-1.1.0/django_serializer/form/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-03-19 18:51:44.000000 django-serializer-1.1.0/django_serializer/form/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-03-19 18:51:44.000000 django-serializer-1.1.0/django_serializer/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 18:51:55.802844 django-serializer-1.1.0/django_serializer/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 18:51:44.000000 django-serializer-1.1.0/django_serializer/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-03-19 18:51:44.000000 django-serializer-1.1.0/django_serializer/model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-03-19 18:51:44.000000 django-serializer-1.1.0/django_serializer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-03-19 18:51:44.000000 django-serializer-1.1.0/django_serializer/permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 18:51:55.802844 django-serializer-1.1.0/django_serializer/serializer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 18:51:44.000000 django-serializer-1.1.0/django_serializer/serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7387 2023-03-19 18:51:44.000000 django-serializer-1.1.0/django_serializer/serializer/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-03-19 18:51:44.000000 django-serializer-1.1.0/django_serializer/serializer/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 18:51:55.802844 django-serializer-1.1.0/django_serializer/v2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 18:51:44.000000 django-serializer-1.1.0/django_serializer/v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 18:51:55.802844 django-serializer-1.1.0/django_serializer/v2/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-03-19 18:51:44.000000 django-serializer-1.1.0/django_serializer/v2/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-19 18:51:44.000000 django-serializer-1.1.0/django_serializer/v2/exceptions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-03-19 18:51:44.000000 django-serializer-1.1.0/django_serializer/v2/exceptions/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-03-19 18:51:44.000000 django-serializer-1.1.0/django_serializer/v2/exceptions/http.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 18:51:55.802844 django-serializer-1.1.0/django_serializer/v2/serializer/
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-03-19 18:51:44.000000 django-serializer-1.1.0/django_serializer/v2/serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-03-19 18:51:44.000000 django-serializer-1.1.0/django_serializer/v2/serializer/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 18:51:55.802844 django-serializer-1.1.0/django_serializer/v2/swagger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 18:51:44.000000 django-serializer-1.1.0/django_serializer/v2/swagger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-03-19 18:51:44.000000 django-serializer-1.1.0/django_serializer/v2/swagger/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-03-19 18:51:44.000000 django-serializer-1.1.0/django_serializer/v2/swagger/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-03-19 18:51:44.000000 django-serializer-1.1.0/django_serializer/v2/swagger/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 18:51:55.802844 django-serializer-1.1.0/django_serializer/v2/views/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-19 18:51:44.000000 django-serializer-1.1.0/django_serializer/v2/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-03-19 18:51:44.000000 django-serializer-1.1.0/django_serializer/v2/views/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-03-19 18:51:44.000000 django-serializer-1.1.0/django_serializer/v2/views/generics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-03-19 18:51:44.000000 django-serializer-1.1.0/django_serializer/v2/views/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-03-19 18:51:44.000000 django-serializer-1.1.0/django_serializer/v2/views/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-03-19 18:51:44.000000 django-serializer-1.1.0/django_serializer/v2/views/paginator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 18:51:55.802844 django-serializer-1.1.0/django_serializer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-03-19 18:51:55.000000 django-serializer-1.1.0/django_serializer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-03-19 18:51:55.000000 django-serializer-1.1.0/django_serializer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-19 18:51:55.000000 django-serializer-1.1.0/django_serializer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-19 18:51:55.000000 django-serializer-1.1.0/django_serializer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-19 18:51:55.000000 django-serializer-1.1.0/django_serializer.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       79 2023-03-19 18:51:55.802844 django-serializer-1.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1443 2023-03-19 18:51:44.000000 django-serializer-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:06:17.924406 django-serializer-1.2.0/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1108 2023-06-09 12:06:06.000000 django-serializer-1.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-09 12:06:17.924406 django-serializer-1.2.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2361 2023-06-09 12:06:06.000000 django-serializer-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:06:17.920406 django-serializer-1.2.0/django_serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/base_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:06:17.920406 django-serializer-1.2.0/django_serializer/form/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/form/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/form/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:06:17.920406 django-serializer-1.2.0/django_serializer/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:06:17.924406 django-serializer-1.2.0/django_serializer/serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7976 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/serializer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/serializer/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:06:17.924406 django-serializer-1.2.0/django_serializer/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:06:17.924406 django-serializer-1.2.0/django_serializer/v2/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/v2/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/v2/exceptions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/v2/exceptions/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/v2/exceptions/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/v2/exceptions/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/v2/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/v2/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/v2/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/v2/serializer_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/v2/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:06:17.924406 django-serializer-1.2.0/django_serializer/v2/swagger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/v2/swagger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/v2/swagger/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/v2/swagger/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/v2/swagger/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:06:17.924406 django-serializer-1.2.0/django_serializer/v2/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/v2/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/v2/views/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/v2/views/generics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/v2/views/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/v2/views/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-06-09 12:06:06.000000 django-serializer-1.2.0/django_serializer/v2/views/paginator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:06:17.920406 django-serializer-1.2.0/django_serializer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-09 12:06:17.000000 django-serializer-1.2.0/django_serializer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-09 12:06:17.000000 django-serializer-1.2.0/django_serializer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 12:06:17.000000 django-serializer-1.2.0/django_serializer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-09 12:06:17.000000 django-serializer-1.2.0/django_serializer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-09 12:06:17.000000 django-serializer-1.2.0/django_serializer.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       79 2023-06-09 12:06:17.924406 django-serializer-1.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1410 2023-06-09 12:06:06.000000 django-serializer-1.2.0/setup.py
```

### Comparing `django-serializer-1.1.0/LICENSE.txt` & `django-serializer-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-serializer-1.1.0/PKG-INFO` & `django-serializer-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-serializer
-Version: 1.1.0
+Version: 1.2.0
 Summary: Library for creating simple django api
 Home-page: https://github.com/alexopryshko/django-serializer
 Author: Alexander Opryshko
 Author-email: alexopryshko@yandex.ru
 License: MIT
 Keywords: django-serializer setuptools development
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `django-serializer-1.1.0/README.md` & `django-serializer-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `django-serializer-1.1.0/django_serializer/base_views.py` & `django-serializer-1.2.0/django_serializer/base_views.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,59 +1,72 @@
 import json
+from warnings import warn
 
 from django.http import HttpResponse
 from django.views.generic import View
 
 from django_serializer.permissions import PermissionsMixin
-from django_serializer.exceptions import (FormException, ServerError, )
+from django_serializer.exceptions import (
+    FormException,
+    ServerError,
+)
 from django_serializer.exceptions import BaseViewException as BVE_1
 from django_serializer.exceptions import BaseViewException as BVE_2
 from django_serializer.mixins import (
     CsrfExemptMixin,
     SerializerMixin,
     ObjectMixin,
     FormMixin,
     ListMixin,
 )
 
 
 class BaseView(View):
     args_form = None
 
+    def __init_subclass__(cls, **kwargs):
+        warn(
+            f"{cls.__name__} inherits `django_serializer.base_views.BaseView` which is deprecated. "
+            f"Use `django_serializer.v2` version instead",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        super().__init_subclass__(**kwargs)
+
     @property
     def request_args(self):
-        return getattr(self, '_request_args', {})
+        return getattr(self, "_request_args", {})
 
     def get_args_form(self):
         return self.args_form
 
     @property
     def request_body(self):
-        if hasattr(self, '_request_body'):
-            return getattr(self, '_request_body')
+        if hasattr(self, "_request_body"):
+            return getattr(self, "_request_body")
         try:
-            data = json.loads(self.request.body.decode('utf-8'))
+            data = json.loads(self.request.body.decode("utf-8"))
         except Exception:
             data = {}
-        setattr(self, '_request_body', data)
+        setattr(self, "_request_body", data)
         return data
 
     def clean_args(self):
         if not self.get_args_form():
             return
-        if hasattr(self, '_request_args'):
+        if hasattr(self, "_request_args"):
             return
 
-        kwargs = {'data': self.request.GET}
-        if self.request.method in ('POST', 'PUT'):
-            kwargs.update({'data': self.request_body})
+        kwargs = {"data": self.request.GET}
+        if self.request.method in ("POST", "PUT"):
+            kwargs.update({"data": self.request_body})
         form = self.get_args_form()(**kwargs)
 
         if form.is_valid():
-            setattr(self, '_request_args', form.cleaned_data)
+            setattr(self, "_request_args", form.cleaned_data)
         else:
             raise FormException(form)
 
     def dispatch(self, request, *args, **kwargs):
         try:
             self.clean_args()
             response = super().dispatch(request, *args, **kwargs)
@@ -62,27 +75,32 @@
         except (BVE_1, BVE_2) as e:
             return self.exception_wrapper(e)
 
     def response_middleware(self, response):
         return response
 
     def response_wrapper(self, response):
-        return HttpResponse(json.dumps({'status': 'ok', 'data': response}), content_type="application/json")
+        return HttpResponse(
+            json.dumps({"status": "ok", "data": response}),
+            content_type="application/json",
+        )
 
     @staticmethod
     def exception_wrapper(exception):
         response = {
-            'status': exception.get_alias(),
-            'message': exception.get_description(),
-            'data': {}
+            "status": exception.get_alias(),
+            "message": exception.get_description(),
+            "data": {},
         }
         if exception.get_field_problems():
-            response['field_problems'] = exception.get_field_problems()
+            response["field_problems"] = exception.get_field_problems()
         http_code = exception.get_http_code()
-        return HttpResponse(json.dumps(response), content_type="application/json", status=http_code)
+        return HttpResponse(
+            json.dumps(response), content_type="application/json", status=http_code
+        )
 
     def get(self, *args, **kwargs):
         raise ServerError(ServerError.NOT_IMPLEMENTED)
 
     def post(self, *args, **kwargs):
         raise ServerError(ServerError.NOT_IMPLEMENTED)
 
@@ -101,26 +119,30 @@
     def options(self, *args, **kwargs):
         raise ServerError(ServerError.NOT_IMPLEMENTED)
 
     def trace(self, *args, **kwargs):
         raise ServerError(ServerError.NOT_IMPLEMENTED)
 
 
-class CreateView(CsrfExemptMixin, PermissionsMixin, FormMixin, SerializerMixin, BaseView):
+class CreateView(
+    CsrfExemptMixin, PermissionsMixin, FormMixin, SerializerMixin, BaseView
+):
     def post(self, request, *args, **kwargs):
         self.check_w_permission(self.request.user)
         form = self.get_form()
         if form.is_valid():
             instance = form.save()
         else:
             raise FormException(form)
         return instance
 
 
-class DetailsView(CsrfExemptMixin, PermissionsMixin, ObjectMixin, FormMixin, SerializerMixin, BaseView):
+class DetailsView(
+    CsrfExemptMixin, PermissionsMixin, ObjectMixin, FormMixin, SerializerMixin, BaseView
+):
     def get(self, request, *args, **kwargs):
         self.check_r_permission(self.request.user)
         return self.get_object()
 
     def post(self, request, *args, **kwargs):
         self.check_w_permission(self.request.user)
         form = self.get_form()
@@ -144,8 +166,7 @@
         self.check_r_permission(self.request.user)
         paginator = self.get_paginator()
         if paginator:
             instances = paginator.page()
         else:
             instances = self.get_queryset()
         return instances
-
```

### Comparing `django-serializer-1.1.0/django_serializer/exceptions.py` & `django-serializer-1.2.0/django_serializer/exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,37 +30,53 @@
     def __init__(self, status_alias, status_description, http_code=200):
         self.alias = status_alias
         self.description = status_description
         self.http_code = http_code
 
 
 class BaseViewException(Exception):
-    BAD_REQUEST = ServerResponseStatus('bad_request', 'Bad request', 400)
-    INVALID_PARAMETER = ServerResponseStatus('invalid_param', 'Invalid parameter', 400)
-    AUTH_NOT_REQUIRED = ServerResponseStatus('auth_not_required', 'Authentication not required', 400)
-
-    AUTH_REQUIRED = ServerResponseStatus('auth_required', 'Authentication required', 401)
-    ACCESS_DENIED = ServerResponseStatus('access_denied', 'Access denied', 401)
-
-    FORBIDDEN = ServerResponseStatus('forbidden', 'Forbidden', 403)
-    INVALID_CREDENTIALS = ServerResponseStatus('invalid_credentials', 'Invalid credentials', 403)
-    ROLE_FORBIDDEN = ServerResponseStatus('role_forbidden', 'For your role access denied', 403)
-    ACCOUNT_INACTIVE = ServerResponseStatus('account_not_active', 'Account is not active', 403)
-
-    NOT_FOUND = ServerResponseStatus('not_found', 'Not found', 404)
-
-    NOT_IMPLEMENTED = ServerResponseStatus('not_implemented', 'Not implemented', 405)
-
-    TOO_MANY_REQUESTS = ServerResponseStatus('too_many_requests', 'Too many requests', 429)
-
-    MIX_FIELDS_FILTER = ServerResponseStatus('mix_fields_filter', 'Cannot have a mix of inclusion and exclusion', 500)
-    STORAGE_ERROR = ServerResponseStatus('storage_error', 'Storage error', 500)
-    INTERNAL_SERVER_ERROR = ServerResponseStatus('internal_error', 'Internal server error', 500)
-    UNKNOWN = ServerResponseStatus('unknown_error', 'Unknown error', 500)
-    FILE_SAVE_ERROR = ServerResponseStatus('file_save_error', "Can't save data", 500)
+    BAD_REQUEST = ServerResponseStatus("bad_request", "Bad request", 400)
+    INVALID_PARAMETER = ServerResponseStatus("invalid_param", "Invalid parameter", 400)
+    AUTH_NOT_REQUIRED = ServerResponseStatus(
+        "auth_not_required", "Authentication not required", 400
+    )
+
+    AUTH_REQUIRED = ServerResponseStatus(
+        "auth_required", "Authentication required", 401
+    )
+    ACCESS_DENIED = ServerResponseStatus("access_denied", "Access denied", 401)
+
+    FORBIDDEN = ServerResponseStatus("forbidden", "Forbidden", 403)
+    INVALID_CREDENTIALS = ServerResponseStatus(
+        "invalid_credentials", "Invalid credentials", 403
+    )
+    ROLE_FORBIDDEN = ServerResponseStatus(
+        "role_forbidden", "For your role access denied", 403
+    )
+    ACCOUNT_INACTIVE = ServerResponseStatus(
+        "account_not_active", "Account is not active", 403
+    )
+
+    NOT_FOUND = ServerResponseStatus("not_found", "Not found", 404)
+
+    NOT_IMPLEMENTED = ServerResponseStatus("not_implemented", "Not implemented", 405)
+
+    TOO_MANY_REQUESTS = ServerResponseStatus(
+        "too_many_requests", "Too many requests", 429
+    )
+
+    MIX_FIELDS_FILTER = ServerResponseStatus(
+        "mix_fields_filter", "Cannot have a mix of inclusion and exclusion", 500
+    )
+    STORAGE_ERROR = ServerResponseStatus("storage_error", "Storage error", 500)
+    INTERNAL_SERVER_ERROR = ServerResponseStatus(
+        "internal_error", "Internal server error", 500
+    )
+    UNKNOWN = ServerResponseStatus("unknown_error", "Unknown error", 500)
+    FILE_SAVE_ERROR = ServerResponseStatus("file_save_error", "Can't save data", 500)
 
     def __init__(self, status, description=None, field_problems=None):
         if not isinstance(status, ServerResponseStatus):
             status = self.UNKNOWN
 
         self.status = status
         self.description = self.status.description
```

### Comparing `django-serializer-1.1.0/django_serializer/form/fields.py` & `django-serializer-1.2.0/django_serializer/form/fields.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 from django import forms
 from django.core.exceptions import ValidationError
 import json
 
 
 class ObjectField(forms.Field):
-    default_error_messages = {
-        'invalid_type': 'Object is incorrect'
-    }
+    default_error_messages = {"invalid_type": "Object is incorrect"}
 
     @staticmethod
     def get_field_problems(form):
         field_problems = []
         for field, error in form.errors.items():
             for data_item in error.data:
                 for message in data_item.messages:
-                    field_problems.append('{}: {}'.format(field, message))
+                    field_problems.append("{}: {}".format(field, message))
         return field_problems
 
     def form_validator(self, value):
         if self.multiple:
             for item in value:
                 form = self.form_class(data=item)
                 if not form.is_valid():
-                    raise ValidationError(self.get_field_problems(form), code='invalid_form')
+                    raise ValidationError(
+                        self.get_field_problems(form), code="invalid_form"
+                    )
                 else:
                     self._validate_forms.append(form)
         else:
             form = self.form_class(data=value)
             if not form.is_valid():
-                raise ValidationError(self.get_field_problems(form), code='invalid_form')
+                raise ValidationError(
+                    self.get_field_problems(form), code="invalid_form"
+                )
             self._validate_forms.append(form)
 
     def __init__(self, form_class, multiple=False, *args, **kwargs):
-        validators = kwargs.pop('validators', [])
+        validators = kwargs.pop("validators", [])
         if isinstance(validators, tuple):
             validators += (self.form_validator,)
         else:
             validators.append(self.form_validator)
         self.form_class = form_class
         self.multiple = multiple
         self._validate_forms = []
@@ -56,20 +58,26 @@
         super().validate(value)
 
         if value is None:
             return
 
         if self.multiple:
             if not isinstance(value, list):
-                raise ValidationError(self.error_messages['invalid_type'], code='invalid_type')
+                raise ValidationError(
+                    self.error_messages["invalid_type"], code="invalid_type"
+                )
             if any([not isinstance(item, dict) for item in value]):
-                raise ValidationError(self.error_messages['invalid_type'], code='invalid_type')
+                raise ValidationError(
+                    self.error_messages["invalid_type"], code="invalid_type"
+                )
         else:
             if not isinstance(value, dict):
-                raise ValidationError(self.error_messages['invalid_type'], code='invalid_type')
+                raise ValidationError(
+                    self.error_messages["invalid_type"], code="invalid_type"
+                )
 
     def clean(self, value):
         super().clean(value)
         if self.multiple:
             return [form.cleaned_data for form in self._validate_forms]
         if len(self._validate_forms) > 0:
             return self._validate_forms[0].cleaned_data
```

### Comparing `django-serializer-1.1.0/django_serializer/mixins.py` & `django-serializer-1.2.0/django_serializer/mixins.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,36 +18,34 @@
         id = forms.IntegerField()
 
     def get_args_form(self):
         return self.ObjectForm
 
     def get_object(self):
         try:
-            return self.model.objects.get(pk=self.request_args['id'])
+            return self.model.objects.get(pk=self.request_args["id"])
         except self.model.DoesNotExist:
             raise ServerError(ServerError.NOT_FOUND)
         except (ValueError, KeyError):
             raise ServerError(ServerError.BAD_REQUEST)
 
     def get_form_kwargs(self):
         kwargs = super().get_form_kwargs()
-        kwargs['instance'] = self.get_object()
+        kwargs["instance"] = self.get_object()
         return kwargs
 
 
 class SerializerMixin:
     serializer = None
 
     def get_serializer_class(self, obj=None):
         return self.serializer
 
     def get_serializer_kwargs(self, obj, **kwargs):
-        serializer_kwargs = {
-            'obj': obj
-        }
+        serializer_kwargs = {"obj": obj}
         serializer_kwargs.update(kwargs)
         return serializer_kwargs
 
     def get_serializer(self, obj, **kwargs):
         serializer_class = self.get_serializer_class(obj)
         return serializer_class(**self.get_serializer_kwargs(obj, **kwargs))
 
@@ -59,22 +57,24 @@
 
 
 class FormMixin:
     form_class = None
 
     def get_form_kwargs(self):
         kwargs = {
-            'data': self.request.GET,
+            "data": self.request.GET,
         }
 
-        if self.request.method in ('POST', 'PUT'):
-            kwargs.update({
-                'data': self.request_body,
-                'files': self.request.FILES,
-            })
+        if self.request.method in ("POST", "PUT"):
+            kwargs.update(
+                {
+                    "data": self.request_body,
+                    "files": self.request.FILES,
+                }
+            )
         return kwargs
 
     def get_form_class(self):
         return self.form_class
 
     def get_form(self):
         """
@@ -88,34 +88,32 @@
     model = None
     paginator = None
 
     def get_paginator_class(self):
         return self.paginator
 
     def get_paginator_kwargs(self):
-        return {
-            'object_list': self.get_queryset(),
-            'arguments': self.request.GET
-        }
+        return {"object_list": self.get_queryset(), "arguments": self.request.GET}
 
     def get_paginator(self):
-        if hasattr(self, '_paginator'):
-            return getattr(self, '_paginator')
+        if hasattr(self, "_paginator"):
+            return getattr(self, "_paginator")
         if self.paginator:
-            setattr(self, '_paginator', self.get_paginator_class()(**self.get_paginator_kwargs()))
-            return getattr(self, '_paginator')
+            setattr(
+                self,
+                "_paginator",
+                self.get_paginator_class()(**self.get_paginator_kwargs()),
+            )
+            return getattr(self, "_paginator")
 
     def get_queryset(self):
-        return self.model.objects.all().order_by('id')
+        return self.model.objects.all().order_by("id")
 
     def get_serializer_kwargs(self, obj, **kwargs):
-        return super().get_serializer_kwargs(obj, **{'multiple': True})
+        return super().get_serializer_kwargs(obj, **{"multiple": True})
 
     def response_middleware(self, response):
         response = super().response_middleware(response)
         paginator = self.get_paginator()
         if paginator:
-            response = {
-                'count': self.get_paginator().count,
-                'list': response
-            }
+            response = {"count": self.get_paginator().count, "list": response}
         return response
```

### Comparing `django-serializer-1.1.0/django_serializer/model/base.py` & `django-serializer-1.2.0/django_serializer/model/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,47 @@
 from django.db import models
 from django.core.exceptions import ValidationError
 from django.db.models.base import ModelBase
 
-from django_serializer.exceptions import MissEntityTypeException, DuplicateEntityTypeException
+from django_serializer.exceptions import (
+    MissEntityTypeException,
+    DuplicateEntityTypeException,
+)
 
 
 ENTITY_TYPE_LENGTH = 16
 ENTITY_ID_LENGTH = 64 - ENTITY_TYPE_LENGTH
-_ENTITY_TYPE_MAX_VALUE = int('1' * ENTITY_TYPE_LENGTH, 2)
-_ENTITY_ID_MAX_VALUE = int('1' * ENTITY_ID_LENGTH, 2)
+_ENTITY_TYPE_MAX_VALUE = int("1" * ENTITY_TYPE_LENGTH, 2)
+_ENTITY_ID_MAX_VALUE = int("1" * ENTITY_ID_LENGTH, 2)
 _ENTITY_TYPE_MASK = _ENTITY_TYPE_MAX_VALUE << ENTITY_ID_LENGTH
 _ENTITY_ID_MASK = ~_ENTITY_TYPE_MASK
 
 
 class EntityMixinMeta(ModelBase):
     entity_types = {}
 
     def __new__(mcs, name, bases, attrs):
-        if 'EntityMixin' == name or 'ENTITY_TYPE' not in attrs:
+        if "EntityMixin" == name or "ENTITY_TYPE" not in attrs:
             new = super(EntityMixinMeta, mcs).__new__(mcs, name, bases, attrs)
             return new
 
-        entity_type = attrs['ENTITY_TYPE']
+        entity_type = attrs["ENTITY_TYPE"]
         if entity_type is None:
-            raise MissEntityTypeException('You have missed entity_type in {}'.format(name))
+            raise MissEntityTypeException(
+                "You have missed entity_type in {}".format(name)
+            )
 
         if entity_type in mcs.entity_types:
             raise DuplicateEntityTypeException(
-                'Model({}) with the same entity type already exist'.format(mcs.entity_types[entity_type].__name__)
+                "Model({}) with the same entity type already exist".format(
+                    mcs.entity_types[entity_type].__name__
+                )
             )
 
-        attrs['entity_types'] = mcs.entity_types
+        attrs["entity_types"] = mcs.entity_types
 
         new = super(EntityMixinMeta, mcs).__new__(mcs, name, bases, attrs)
         mcs.entity_types[entity_type] = new
 
         return new
 
     def check_entity_type(cls, entity_type):
@@ -59,22 +66,21 @@
         return self.entity_types[entity_type].objects.get(pk=entity_id)
 
 
 class EntityField(models.BigIntegerField):
     @staticmethod
     def validate_object_id(value):
         if not check_object_id(value):
-            raise ValidationError('%(value)s is not valid object id', params={'value': value})
+            raise ValidationError(
+                "%(value)s is not valid object id", params={"value": value}
+            )
 
     def __init__(self, *args, **kwargs):
-        self.available_entities = kwargs.pop('available_entities', [])
-        kwargs.update({
-            'db_index': True,
-            'validators': [self.validate_object_id]
-        })
+        self.available_entities = kwargs.pop("available_entities", [])
+        kwargs.update({"db_index": True, "validators": [self.validate_object_id]})
         super().__init__(*args, **kwargs)
 
 
 def split_object_id(object_id):
     object_id = int(object_id)
     entity_type = (object_id & _ENTITY_TYPE_MASK) >> ENTITY_ID_LENGTH
     entity_id = object_id & _ENTITY_ID_MASK
```

### Comparing `django-serializer-1.1.0/django_serializer/paginator.py` & `django-serializer-1.2.0/django_serializer/paginator.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     def get_form(self):
         return self.get_form_class()(**self.get_form_kwargs())
 
     def get_form_class(self):
         return self.form
 
     def get_form_kwargs(self):
-        return {'data': self._arguments}
+        return {"data": self._arguments}
 
     def validate_arguments(self):
         form = self.get_form()
         if form.is_valid():
             self.validated_arguments = form.cleaned_data
         else:
             raise FormException(form)
@@ -31,14 +31,15 @@
     def _get_count(self):
         if self._count is None:
             try:
                 self._count = self.object_list.count()
             except (AttributeError, TypeError):
                 self._count = len(self.object_list)
         return self._count
+
     count = property(_get_count)
 
     def page(self):
         if self.validated_arguments is None:
             self.validate_arguments()
 
 
@@ -50,10 +51,10 @@
         limit = forms.IntegerField(min_value=1, max_value=100, required=False)
         offset = forms.IntegerField(min_value=0, required=False)
 
     form = LimitOffsetForm
 
     def page(self):
         super().page()
-        bottom = self.validated_arguments['offset'] or self.OFFSET
-        top = bottom + (self.validated_arguments['limit'] or self.LIMIT)
+        bottom = self.validated_arguments["offset"] or self.OFFSET
+        top = bottom + (self.validated_arguments["limit"] or self.LIMIT)
         return self.object_list[bottom:top]
```

### Comparing `django-serializer-1.1.0/django_serializer/permissions.py` & `django-serializer-1.2.0/django_serializer/permissions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 from django_serializer.exceptions import ServerError
 
 
 class PermissionsModelMixin:
     class Permission:
-        R = 1       # read permission
+        R = 1  # read permission
         W = 1 << 1  # write permission
         D = 1 << 2  # delete permission
 
     owner_permission = (Permission.R, Permission.W, Permission.D)
     group_permission = (Permission.R, Permission.W)
-    authorized_permission = (Permission.R, )
+    authorized_permission = (Permission.R,)
     unauthorized_permission = ()
 
     def is_owner(self, user):
         pass
 
     def in_group(self, user):
         pass
 
 
 class PermissionsMixin(PermissionsModelMixin):
     class DefaultPermissions(PermissionsModelMixin):
-        authorized_permission = (PermissionsModelMixin.Permission.R, PermissionsModelMixin.Permission.W)
+        authorized_permission = (
+            PermissionsModelMixin.Permission.R,
+            PermissionsModelMixin.Permission.W,
+        )
 
     owner_permission = ()
     group_permission = ()
     authorized_permission = ()
     unauthorized_permission = ()
 
     def get_permissions_object(self):
@@ -34,37 +37,37 @@
             bool(self.group_permission),
             bool(self.authorized_permission),
             bool(self.unauthorized_permission),
         )
 
         if any(conditions):
             obj = self
-        elif hasattr(self, 'get_object'):
+        elif hasattr(self, "get_object"):
             obj = self.get_object()
         else:
             obj = self.DefaultPermissions()
 
         return obj
 
     def get_permissions(self, user):
-        if hasattr(self, '_permissions'):
-            return getattr(self, '_permissions')
+        if hasattr(self, "_permissions"):
+            return getattr(self, "_permissions")
 
         obj = self.get_permissions_object()
 
         if user.is_authenticated and obj.is_owner(user):
             permissions = obj.owner_permission
         elif user.is_authenticated and obj.in_group(user):
             permissions = obj.group_permission
         elif user.is_authenticated:
             permissions = obj.authorized_permission
         else:
             permissions = obj.unauthorized_permission
 
-        setattr(self, '_permissions', permissions)
+        setattr(self, "_permissions", permissions)
 
         return permissions
 
     def check_permission(self, user, permission):
         if user.is_superuser:
             return
         if permission not in self.get_permissions(user):
```

### Comparing `django-serializer-1.1.0/django_serializer/serializer/base.py` & `django-serializer-1.2.0/django_serializer/serializer/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,17 @@
+from warnings import warn
+
 from django.conf import settings
 from django.db import models
 
 from django_serializer.model.base import EntityField
-from django_serializer.exceptions import MetaSerializerException, MappingSerializerException
+from django_serializer.exceptions import (
+    MetaSerializerException,
+    MappingSerializerException,
+)
 from django_serializer.serializer.fields import (
     Field,
     IntegerField,
     BooleanField,
     CharField,
     DateField,
     DateTimeField,
@@ -34,53 +39,61 @@
     models.IntegerField: IntegerField,
     models.PositiveIntegerField: IntegerField,
     models.PositiveSmallIntegerField: IntegerField,
     models.SmallIntegerField: IntegerField,
     models.TextField: CharField,
     EntityField: IntegerField,
     models.ImageField: ImageField,
-    models.URLField: CharField
+    models.URLField: CharField,
 }
-EXTRA_SERIALIZER_FIELD_MAPPING = getattr(
-    settings, 'SERIALIZER_FIELD_MAPPING', None
-)
+EXTRA_SERIALIZER_FIELD_MAPPING = getattr(settings, "SERIALIZER_FIELD_MAPPING", None)
 if EXTRA_SERIALIZER_FIELD_MAPPING:
-    assert isinstance(EXTRA_SERIALIZER_FIELD_MAPPING, dict), \
-        'SERIALIZER_FIELD_MAPPING should be dict'
+    assert isinstance(
+        EXTRA_SERIALIZER_FIELD_MAPPING, dict
+    ), "SERIALIZER_FIELD_MAPPING should be dict"
     SERIALIZER_FIELD_MAPPING.update(EXTRA_SERIALIZER_FIELD_MAPPING)
 
 
 class SerializerMeta(type):
     def __new__(mcs, name, bases, attrs):
         serializer_attrs = attrs.copy()
 
         for base_class in bases:
             serializer_attrs.update(base_class.__dict__)
             for c in reversed(base_class.__mro__):
                 serializer_attrs.update(c.__dict__)
 
-        attrs['serializer_attrs'] = []
+        attrs["serializer_attrs"] = []
 
         for field_name, field in serializer_attrs.items():
             if isinstance(field, Field):
-                attrs['serializer_attrs'].append((field_name, field))
+                attrs["serializer_attrs"].append((field_name, field))
 
         new = super(SerializerMeta, mcs).__new__(mcs, name, bases, attrs)
         return new
 
 
 class Serializer(metaclass=SerializerMeta):
-    def __init__(self, obj, multiple=False, dict_format=False, dict_key='id'):
+    def __init_subclass__(cls, **kwargs):
+        warn(
+            f"{cls.__name__} inherits `django_serializer.serializer.base.Serializer` which is deprecated. "
+            f"Use `django_serializer.v2` version instead",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        super().__init_subclass__(**kwargs)
+
+    def __init__(self, obj, multiple=False, dict_format=False, dict_key="id"):
         self.obj = obj
         self.multiple = multiple
         self.dict_format = dict_format
         self.dict_key = dict_key
 
     def _get_fields(self):
-        return getattr(self, 'serializer_attrs')
+        return getattr(self, "serializer_attrs")
 
     def _get_extractor(self, obj):
         def obj_extractor(inner_obj, field):
             try:
                 return getattr(inner_obj, field)
             except AttributeError:
                 return getattr(self, field)(inner_obj)
@@ -105,98 +118,110 @@
         for field_name, field in fields:
             try:
                 if isinstance(field, SerializerField):
                     field.serializer = self
                     serialized_field_value = field.serialize(field_value=obj)
                 else:
                     obj_field_value = extractor(obj, field_name)
-                    serialized_field_value = field.serialize(field_value=obj_field_value)
+                    serialized_field_value = field.serialize(
+                        field_value=obj_field_value
+                    )
             except AttributeError:
                 serialized_field_value = field.serialize()
             serialized[field_name] = serialized_field_value
 
         return serialized
 
     def serialize(self):
         if self.obj is None:
             return None
 
         if self.multiple:
             if self.dict_format:
                 result = {}
                 for obj_item in self.obj:
-                    result[getattr(obj_item, self.dict_key)] = self._serialize_obj(obj_item)
+                    result[getattr(obj_item, self.dict_key)] = self._serialize_obj(
+                        obj_item
+                    )
             else:
                 result = []
                 for obj_item in self.obj:
                     result.append(self._serialize_obj(obj_item))
         else:
             if self.dict_format:
-                result = {getattr(self.obj, self.dict_key): self._serialize_obj(self.obj)}
+                result = {
+                    getattr(self.obj, self.dict_key): self._serialize_obj(self.obj)
+                }
             else:
                 result = self._serialize_obj(self.obj)
 
         return result
 
 
 class ModelSerializerMeta(SerializerMeta):
     def __new__(mcs, name, bases, attrs):
-        if name == 'ModelSerializer':
+        if name == "ModelSerializer":
             new = super(ModelSerializerMeta, mcs).__new__(mcs, name, bases, attrs)
             return new
 
         Meta = None
         try:
-            Meta = attrs['Meta']
+            Meta = attrs["Meta"]
         except KeyError:
             for base in bases:
-                if 'Meta' in base.__dict__:
-                    Meta = base.__dict__['Meta']
+                if "Meta" in base.__dict__:
+                    Meta = base.__dict__["Meta"]
                     break
                 for c in reversed(base.__mro__):
-                    if 'Meta' in c.__dict__:
-                        Meta = c.__dict__['Meta']
+                    if "Meta" in c.__dict__:
+                        Meta = c.__dict__["Meta"]
                         break
         if not Meta:
-            raise MetaSerializerException('{} serializer have not Meta'.format(name))
+            raise MetaSerializerException("{} serializer have not Meta".format(name))
 
         try:
             model = Meta.model
         except AttributeError:
-            raise MetaSerializerException('{}.Meta have not model'.format(name))
+            raise MetaSerializerException("{}.Meta have not model".format(name))
 
-        meta_fields = getattr(Meta, 'fields', None)
+        meta_fields = getattr(Meta, "fields", None)
         if meta_fields and not isinstance(meta_fields, (tuple, list)):
-            raise MetaSerializerException('{}.Meta.fields have incorrect format'.format(name))
+            raise MetaSerializerException(
+                "{}.Meta.fields have incorrect format".format(name)
+            )
 
         meta_fields = set(meta_fields) if meta_fields else None
 
-        meta_exclude = getattr(Meta, 'exclude', None)
+        meta_exclude = getattr(Meta, "exclude", None)
         if meta_exclude and not isinstance(meta_exclude, (tuple, list)):
-            raise MetaSerializerException('{}.Meta.meta_exclude have incorrect format'.format(name))
+            raise MetaSerializerException(
+                "{}.Meta.meta_exclude have incorrect format".format(name)
+            )
 
         meta_exclude = set(meta_exclude) if meta_exclude else None
 
         model_fields = model._meta.fields
         for model_field in model_fields:
             model_field_class = model_field.__class__
 
             if meta_fields is not None and model_field.attname not in meta_fields:
                 continue
 
             if meta_exclude is not None and model_field.attname in meta_exclude:
                 continue
 
-            if hasattr(model_field_class, 'serializer'):
+            if hasattr(model_field_class, "serializer"):
                 serializer_field_class = model_field_class.serializer
             else:
                 try:
                     serializer_field_class = SERIALIZER_FIELD_MAPPING[model_field_class]
                 except KeyError:
-                    raise MappingSerializerException('{} is not supported'.format(model_field_class))
+                    raise MappingSerializerException(
+                        "{} is not supported".format(model_field_class)
+                    )
 
             attrs[model_field.attname] = serializer_field_class()
 
         new = super(ModelSerializerMeta, mcs).__new__(mcs, name, bases, attrs)
         return new
 
 
@@ -207,14 +232,12 @@
 class MultiSerializer(Serializer):
     serializers = {}
 
     def get_serializer_class(self, obj, **kwargs):
         raise NotImplementedError
 
     def get_serializer_kwargs(self, obj, **kwargs):
-        return {
-            'obj': obj
-        }
+        return {"obj": obj}
 
     def _serialize_obj(self, obj):
         serializer_class = self.get_serializer_class(obj)
         return serializer_class(**self.get_serializer_kwargs(obj)).serialize()
```

### Comparing `django-serializer-1.1.0/django_serializer/serializer/fields.py` & `django-serializer-1.2.0/django_serializer/serializer/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 class Field:
     def __init__(self, required=True, default=None, name=None):
         self.default = default
         self.required = required
         self.name = name
 
     def serialize(self, **kwargs):
-        if 'field_value' not in kwargs:
+        if "field_value" not in kwargs:
             if not self.required:
                 serialized = self.default
             else:
-                raise SerializerFieldException('Field missed or has no default value')
+                raise SerializerFieldException("Field missed or has no default value")
         else:
-            serialized = kwargs['field_value']
+            serialized = kwargs["field_value"]
             serialized = self.serialization_handler(serialized)
 
         return serialized
 
     def serialization_handler(self, value):
         pass
 
@@ -37,21 +37,23 @@
     def serialization_handler(self, value):
         return str(value) if value is not None else None
 
 
 class DateField(Field):
     def serialization_handler(self, value):
         from django.utils.dateformat import format
-        return format(value, 'U') if value is not None else None
+
+        return format(value, "U") if value is not None else None
 
 
 class DateTimeField(Field):
     def serialization_handler(self, value):
         from django.utils.dateformat import format
-        return format(value, 'U') if value is not None else None
+
+        return format(value, "U") if value is not None else None
 
 
 class TimeField(Field):
     def serialization_handler(self, value):
         return str(value) if value is not None else None
 
 
@@ -93,15 +95,15 @@
                 return value.url
             except ValueError:
                 return None
 
 
 class SerializerField(Field):
     def __init__(self, **kwargs):
-        source = kwargs.pop('source')
+        source = kwargs.pop("source")
         self.source = source
         self.serializer = None
         super().__init__(**kwargs)
 
     def serialization_handler(self, obj):
         if callable(self.source):
             return self.source(obj)
```

### Comparing `django-serializer-1.1.0/django_serializer/v2/exceptions/conf.py` & `django-serializer-1.2.0/django_serializer/v2/exceptions/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 
 class IncorrectMetaException(SerializerException):
     def __init__(self, clazz: str, errors: Sequence[str]):
         self.clazz = clazz
         self.errors = errors
 
     def __str__(self):
-        errors = '\n'.join(map(lambda s: f'* {s}', self.errors))
-        return f'Meta class of {self.clazz} is incorrect \n{errors}'
+        errors = "\n".join(map(lambda s: f"* {s}", self.errors))
+        return f"Meta class of {self.clazz} is incorrect \n{errors}"
 
     def __repr__(self):
         return self.__str__()
 
 
 class IncorrectSettingsException(SerializerException):
     def __init__(self, msg):
         self.msg = msg
 
     def __str__(self):
-        return f'setting is incorrect: {self.msg}'
+        return f"setting is incorrect: {self.msg}"
 
     def __repr__(self):
         return self.__str__()
```

### Comparing `django-serializer-1.1.0/django_serializer/v2/exceptions/http.py` & `django-serializer-1.2.0/django_serializer/v2/exceptions/http.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,81 +1,72 @@
 from .base import ApiViewException
 
 __all__ = (
-    'HttpError', 'HttpNotImplementedError', 'BadRequestError',
-    'InternalServerError', 'HttpFormError', 'NotFoundError',
-    'AuthRequiredError', 'ForbiddenError'
+    "HttpError",
+    "HttpNotImplementedError",
+    "BadRequestError",
+    "InternalServerError",
+    "HttpFormError",
+    "NotFoundError",
+    "AuthRequiredError",
+    "ForbiddenError",
 )
 
 
 class HttpError(ApiViewException):
+    """
+    Base class for any error happened during execution
+
+    :param http_code: response http_code
+    :param alias: unique key describing error
+    :param description: human readable description
+    """
+
     def __init__(self, http_code, alias, description):
         self.http_code = http_code
         self.alias = alias
         self.description = description
 
     def get_dict(self):
-        return {
-            'status': self.alias,
-            'message': self.description,
-            'data': {}
-        }
+        return {"status": self.alias, "message": self.description, "data": {}}
 
 
 class HttpNotImplementedError(HttpError):
     def __init__(self):
         super().__init__(
-            http_code=405,
-            alias='not_implemented',
-            description='Not implemented'
+            http_code=405, alias="not_implemented", description="Not implemented"
         )
 
 
 class BadRequestError(HttpError):
-    def __init__(self, description='Bad request'):
-        super().__init__(
-            http_code=400,
-            alias='bad_request',
-            description=description
-        )
+    def __init__(self, description="Bad request"):
+        super().__init__(http_code=400, alias="bad_request", description=description)
 
 
 class AuthRequiredError(HttpError):
     def __init__(self):
         super().__init__(
-            http_code=401,
-            alias='auth_required',
-            description='Authentication required'
+            http_code=401, alias="auth_required", description="Authentication required"
         )
 
 
 class ForbiddenError(HttpError):
     def __init__(self):
-        super().__init__(
-            http_code=403,
-            alias='forbidden',
-            description='Forbidden'
-        )
+        super().__init__(http_code=403, alias="forbidden", description="Forbidden")
 
 
 class NotFoundError(HttpError):
     def __init__(self):
-        super().__init__(
-            http_code=404,
-            alias='not_found',
-            description='Not Found'
-        )
+        super().__init__(http_code=404, alias="not_found", description="Not Found")
 
 
 class InternalServerError(HttpError):
     def __init__(self):
         super().__init__(
-            http_code=500,
-            alias='internal_error',
-            description='Internal server error'
+            http_code=500, alias="internal_error", description="Internal server error"
         )
 
 
 class HttpFormError(BadRequestError):
     def __init__(self, form):
         self.form = form
         super().__init__()
@@ -86,9 +77,9 @@
             for data_item in error.data:
                 for message in data_item.messages:
                     problems.append(message)
             self.field_problems[field] = problems
 
     def get_dict(self):
         d = super().get_dict()
-        d['field_problems'] = self.field_problems
+        d["field_problems"] = self.field_problems
         return d
```

### Comparing `django-serializer-1.1.0/django_serializer/v2/swagger/base.py` & `django-serializer-1.2.0/django_serializer/v2/swagger/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 from django_serializer.v2.swagger import utils
 from django_serializer.v2.exceptions import HttpError, HttpFormError
 from django_serializer.v2.views import ApiView
 
 
 class Swagger:
     def __init__(self):
-        self.project_name = getattr(settings, 'SWAGGER_PROJECT_NAME', 'default')
-        self.version = getattr(settings, 'SWAGGER_PROJECT_VERSION', '1.0.0')
-        self.openapi = getattr(settings, 'SWAGGER_OPENAPI_VERSION', '3.0.2')
+        self.project_name = getattr(settings, "SWAGGER_PROJECT_NAME", "default")
+        self.version = getattr(settings, "SWAGGER_PROJECT_VERSION", "1.0.0")
+        self.openapi = getattr(settings, "SWAGGER_OPENAPI_VERSION", "3.0.2")
         self._spec = APISpec(
             title=self.project_name,
             version=self.version,
             openapi_version=self.openapi,
             plugins=[MarshmallowPlugin()],
         )
         self.urls_views = {}
@@ -33,17 +33,15 @@
     def spec(self):
         return self._spec.to_dict()
 
     def generate_view_list(
         self, resolver: Union[urls.URLResolver, urls.URLPattern], prefix: str
     ):
         if isinstance(resolver, urls.URLPattern):
-            available_paths = normalize(
-                f"{prefix}{resolver.pattern.regex.pattern}"
-            )
+            available_paths = normalize(f"{prefix}{resolver.pattern.regex.pattern}")
             for path, args in available_paths:
                 yield resolver.callback, path
         elif isinstance(resolver, urls.URLResolver):
             for pattern in resolver.url_patterns:
                 yield from self.generate_view_list(
                     pattern, f"{prefix}{str(resolver.pattern.regex.pattern)}"
                 )
@@ -57,45 +55,55 @@
             try:
                 class_ = view.view_class
                 if issubclass(class_, ApiView):
                     self.urls_views[url] = class_
             except AttributeError:
                 continue
 
-    def _generate_response(self, schema, description='success'):
+    def _generate_response(self, schema, description="success"):
         if issubclass(type(schema), HttpError):
             description = schema.description
             schema = utils.generate_error_schema(self, schema)
         if schema is None:
-            return {'description': description}
-        return {'description': description,
-                'content': {'application/json': {'schema': schema}}}
+            return {"description": description}
+        return {
+            "description": description,
+            "content": {"application/json": {"schema": schema}},
+        }
 
     def _generate_request_body(self, schema):
-        return {'content': {'application/json': {
-            'schema': self.ma_spec.converter.schema2jsonschema(schema)
-        }}}
+        return {
+            "content": {
+                "application/json": {
+                    "schema": self.ma_spec.converter.schema2jsonschema(schema)
+                }
+            }
+        }
 
     def _resolve_forms(self, meta):
         query_schema = utils.merge_schemas(
-            utils.form2schema(getattr(meta, 'query_form', None)),
-            utils.form2schema(getattr(getattr(meta, 'paginator', None),
-                                      'form', None)))
+            utils.form2schema(getattr(meta, "query_form", None)),
+            utils.form2schema(getattr(getattr(meta, "paginator", None), "form", None)),
+        )
         body_schema = utils.merge_schemas(
-            utils.form2schema(getattr(meta, 'body_form', None)),
-            utils.form2schema(getattr(meta, 'model_form', None)))
+            utils.form2schema(getattr(meta, "body_form", None)),
+            utils.form2schema(getattr(meta, "model_form", None)),
+        )
 
         parameters = {}
         if query_schema is not None:
-            parameters.update({'query': self.ma_spec.converter
-                              .schema2parameters(query_schema,
-                                                 location='query')})
-        if body_schema is not None:
             parameters.update(
-                {'requestBody': self._generate_request_body(body_schema)})
+                {
+                    "query": self.ma_spec.converter.schema2parameters(
+                        query_schema, location="query"
+                    )
+                }
+            )
+        if body_schema is not None:
+            parameters.update({"requestBody": self._generate_request_body(body_schema)})
         return parameters
 
     def _generate_operations(self, meta):
         parameters = self._resolve_forms(meta)
         if len(parameters) != 0:
             meta.errors.append(HttpFormError)
 
@@ -106,24 +114,21 @@
             else:
                 err = err()
             responses.update({err.http_code: self._generate_response(err)})
 
         for tag in meta.tags:
             self.tags.add(tag)
 
-        operation = {
-            'responses': responses,
-            'tags': meta.tags
-        }
+        operation = {"responses": responses, "tags": meta.tags}
 
-        if parameters.get('query', False):
-            operation.update({'parameters': parameters['query']})
+        if parameters.get("query", False):
+            operation.update({"parameters": parameters["query"]})
 
-        if parameters.get('requestBody', False):
-            operation.update({'requestBody': parameters['requestBody']})
+        if parameters.get("requestBody", False):
+            operation.update({"requestBody": parameters["requestBody"]})
 
         if getattr(meta, "description"):
             operation.update({"description": meta.description})
 
         if getattr(meta, "summary"):
             operation.update({"summary": meta.summary})
 
@@ -138,13 +143,13 @@
                 description=view.Meta.description,
                 view=view,
                 operations=self._generate_operations(view.Meta),
             )
 
     def _generate_tags(self):
         for tag in self.tags:
-            self._spec.tag({'name': tag, 'description': tag})
+            self._spec.tag({"name": tag, "description": tag})
 
     def generate(self):
         self._get_views()
         self._generate_paths()
         self._generate_tags()
```

### Comparing `django-serializer-1.1.0/django_serializer/v2/swagger/utils.py` & `django-serializer-1.2.0/django_serializer/v2/swagger/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from django import forms
 from django.conf import settings
 from django.forms import ModelForm
 from marshmallow import Schema, fields
 
-from django_serializer.v2.exceptions import HttpError, \
-    IncorrectSettingsException
+from django_serializer.v2.exceptions import HttpError, IncorrectSettingsException
 
 
 class IntList(fields.List):
     def __init__(self, *args, **kwargs):
         super().__init__(fields.Integer, *args, **kwargs)
 
 
@@ -31,21 +30,19 @@
     forms.URLField: fields.Url,
     forms.ModelMultipleChoiceField: IntList,
     forms.MultipleChoiceField: StrList,
     forms.ModelChoiceField: fields.Int,
     forms.TypedChoiceField: fields.Str,
 }
 
-extra_fields = getattr(
-    settings, 'SERIALIZER_FORM_FIELD_MAPPING', None
-)
+extra_fields = getattr(settings, "SERIALIZER_FORM_FIELD_MAPPING", None)
 if extra_fields:
     if not isinstance(extra_fields, dict):
         raise IncorrectSettingsException(
-            '`SERIALIZER_FORM_FIELD_MAPPING` has incorrect type'
+            "`SERIALIZER_FORM_FIELD_MAPPING` has incorrect type"
         )
     FORM_FIELD_MAPPING.update(extra_fields)
 
 
 def form2schema(field: forms.Form) -> Schema:
     if field is None:
         return None
@@ -54,32 +51,34 @@
         form_fields = field().base_fields
     else:
         form_fields = field.declared_fields
 
     schema_fields = {}
     for name, field in form_fields.items():
         schema_fields.update(
-            {name: FORM_FIELD_MAPPING[type(field)](required=field.required)})
+            {name: FORM_FIELD_MAPPING[type(field)](required=field.required)}
+        )
     schema = Schema.from_dict(schema_fields)
     return schema
 
 
 def generate_error_schema(swagger, error: HttpError) -> Schema:
-    key = ''.join([str(error.http_code), error.alias])
+    key = "".join([str(error.http_code), error.alias])
     if swagger.error_classes.get(key) is not None:
         return swagger.error_classes[key]
-    schema_fields = dict(status=fields.String(example=error.alias),
-                         message=fields.String(example=error.description),
-                         data=fields.Dict())
-    if getattr(error, 'field_problems', None) is not None:
-        schema_fields.update({'fields_problems': fields.Dict()})
+    schema_fields = dict(
+        status=fields.String(example=error.alias),
+        message=fields.String(example=error.description),
+        data=fields.Dict(),
+    )
+    if getattr(error, "field_problems", None) is not None:
+        schema_fields.update({"fields_problems": fields.Dict()})
 
     schema = Schema.from_dict(
-        schema_fields,
-        name=''.join([i.capitalize() for i in error.description.split()])
+        schema_fields, name="".join([i.capitalize() for i in error.description.split()])
     )
     swagger.error_classes[key] = schema
     return schema
 
 
 def merge_schemas(first_schema: Schema, second_schema: Schema) -> Schema:
     if first_schema is None and second_schema is None:
```

### Comparing `django-serializer-1.1.0/django_serializer/v2/views/generics.py` & `django-serializer-1.2.0/django_serializer/v2/views/generics.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,28 +11,36 @@
     FormMixin,
     ObjectMixin,
     CheckPermissionsMixin,
 )
 from django_serializer.v2.views.paginator import BasePaginator
 
 __all__ = (
-    'CreateApiView', 'GetApiView', 'UpdateApiView', 'DeleteApiView',
-    'ListApiView',
+    "CreateApiView",
+    "GetApiView",
+    "UpdateApiView",
+    "DeleteApiView",
+    "ListApiView",
 )
 
 
 class CreateApiViewMeta(ApiViewMeta):
     class Meta(ApiViewMeta.Meta):
         method: HttpMethod = HttpMethod.POST
         model_form: Type[forms.ModelForm] = None
         serializer: Type[Serializer] = None
 
 
-class CreateApiView(CheckPermissionsMixin, FormMixin, ApiView,
-                    metaclass=CreateApiViewMeta, checkmeta=False):
+class CreateApiView(
+    CheckPermissionsMixin,
+    FormMixin,
+    ApiView,
+    metaclass=CreateApiViewMeta,
+    checkmeta=False,
+):
     Meta = CreateApiViewMeta.Meta
 
     def has_permissions(self) -> bool:
         return True
 
     def execute(self, request, *args, **kwargs):
         self.check_permissions()
@@ -49,20 +57,25 @@
 
 
 class GetApiViewMeta(ApiViewMeta):
     class Meta(ApiViewMeta.Meta):
         method: HttpMethod = HttpMethod.GET
         model: Type[Model] = None
         query_form: Type[forms.Form] = GetApiForm
-        object_key: str = 'id'
+        object_key: str = "id"
         serializer: Type[Serializer] = None
 
 
-class GetApiView(CheckPermissionsMixin, ObjectMixin, ApiView,
-                 metaclass=GetApiViewMeta, checkmeta=False):
+class GetApiView(
+    CheckPermissionsMixin,
+    ObjectMixin,
+    ApiView,
+    metaclass=GetApiViewMeta,
+    checkmeta=False,
+):
     Meta = GetApiViewMeta.Meta
 
     def get_object(self):
         m: Type[Model] = self.Meta.model
         key: str = self.Meta.object_key
         return m.objects.get(**{key: self.request_query[key]})
 
@@ -77,20 +90,21 @@
 
 class UpdateApiViewMeta(ApiViewMeta):
     class Meta(ApiViewMeta.Meta):
         method: HttpMethod = HttpMethod.POST
         body_form: Type[forms.BaseForm] = GetApiForm
         model: Type[Model] = None
         model_form: Type[forms.ModelForm] = None
-        object_key: str = 'id'
+        object_key: str = "id"
         serializer: Type[Serializer] = None
 
 
-class UpdateApiView(ObjectMixin, FormMixin, ApiView,
-                    metaclass=UpdateApiViewMeta, checkmeta=False):
+class UpdateApiView(
+    ObjectMixin, FormMixin, ApiView, metaclass=UpdateApiViewMeta, checkmeta=False
+):
     Meta = UpdateApiViewMeta.Meta
 
     def has_permissions(self, obj: Model) -> bool:
         return True
 
     def execute(self, request, *args, **kwargs):
         obj = self._get_object()
@@ -105,19 +119,24 @@
 
 
 class DeleteApiViewMeta(ApiViewMeta):
     class Meta(ApiViewMeta.Meta):
         method: HttpMethod = HttpMethod.POST
         body_form: Type[forms.BaseForm] = GetApiForm
         model: Type[Model] = None
-        object_key: str = 'id'
+        object_key: str = "id"
 
 
-class DeleteApiView(CheckPermissionsMixin, ObjectMixin, ApiView,
-                    metaclass=DeleteApiViewMeta, checkmeta=False):
+class DeleteApiView(
+    CheckPermissionsMixin,
+    ObjectMixin,
+    ApiView,
+    metaclass=DeleteApiViewMeta,
+    checkmeta=False,
+):
     Meta = DeleteApiViewMeta.Meta
 
     def has_permissions(self, obj: Model) -> bool:
         return True
 
     def execute(self, request, *args, **kwargs):
         obj = self._get_object()
@@ -129,19 +148,20 @@
 class ListApiViewMeta(ApiViewMeta):
     class Meta(ApiViewMeta.Meta):
         method: HttpMethod = HttpMethod.GET
         model: Type[Model] = None
         serializer: Type[Serializer] = None
         serializer_many: bool = True
         paginator: Optional[Type[BasePaginator]] = None
-        ordering: tuple = ('id',)
+        ordering: tuple = ("id",)
 
 
-class ListApiView(CheckPermissionsMixin, ApiView,
-                  metaclass=ListApiViewMeta, checkmeta=False):
+class ListApiView(
+    CheckPermissionsMixin, ApiView, metaclass=ListApiViewMeta, checkmeta=False
+):
     Meta = ListApiViewMeta.Meta
 
     def has_permissions(self) -> bool:
         return True
 
     def get_queryset(self):
         return self.Meta.model.objects.all().order_by(*self.Meta.ordering)
@@ -163,11 +183,8 @@
         self.check_permissions()
         qs = self.get_queryset()
         qs_after_paginator = None
         paginator = self.get_paginator(qs)
         if paginator:
             paginator.validate_form()
             qs_after_paginator = paginator.paginate(qs)
-        return self.build_response(
-            qs=qs,
-            qs_after_paginator=qs_after_paginator
-        )
+        return self.build_response(qs=qs, qs_after_paginator=qs_after_paginator)
```

### Comparing `django-serializer-1.1.0/django_serializer/v2/views/meta.py` & `django-serializer-1.2.0/django_serializer/v2/views/meta.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,156 +3,163 @@
 import inspect
 import sys
 from typing import Optional, List, Type, Union
 
 from django.forms import BaseForm
 
 from django_serializer.v2.exceptions import IncorrectMetaException, HttpError
+from django_serializer.v2.parsers import BaseParser
+from django_serializer.v2.renderers import BaseRenderer
 from django_serializer.v2.serializer import Serializer
+from django_serializer.v2.settings import settings
 
 
 class HttpMethod(enum.Enum):
-    GET = 'get'
-    POST = 'post'
-    PUT = 'put'
-    PATCH = 'patch'
-    DELETE = 'delete'
-    HEAD = 'head'
-    OPTIONS = 'options'
-    TRACE = 'trace'
+    GET = "get"
+    POST = "post"
+    PUT = "put"
+    PATCH = "patch"
+    DELETE = "delete"
+    HEAD = "head"
+    OPTIONS = "options"
+    TRACE = "trace"
 
 
 class ApiViewMeta(type):
     class Meta:
         method: HttpMethod = None
         tags: List[str] = []
         summary: Optional[str] = None
         description: Optional[str] = None
         query_form: Optional[Type[BaseForm]] = None
         body_form: Optional[Type[BaseForm]] = None
+        body_parser: Optional[
+            Type[BaseParser]
+        ] = settings.SERIALIZER_DEFAULT_PARSER_CLASS
         serializer: Optional[Type[Serializer]] = None
         serializer_many: bool = False
         errors: List[Type[HttpError]] = []
+        renderer: Type[BaseRenderer] = settings.SERIALIZER_DEFAULT_RENDERER_CLASS
 
-        __manual_validation__: List[str] = ['tags', 'errors']
+        __manual_validation__: List[str] = ["tags", "errors"]
 
     def __new__(mcs, name, bases, attrs, *args, **kwargs):
-        checkmeta = kwargs.pop('checkmeta', True)
+        checkmeta = kwargs.pop("checkmeta", True)
         # noinspection PyArgumentList
         cls = super().__new__(mcs, name, bases, attrs, *args, **kwargs)
 
         if checkmeta:
-            options = attrs.get('Meta')
+            options = attrs.get("Meta")
             base_options = mcs.find_base_options(bases)
             meta = mcs.merge_options(options, base_options)
             errors = []
             mcs.check_meta_extra(meta, errors)
             mj, mn = sys.version_info[:2]
             if mj >= 3 and mn >= 7:
                 mcs.check_meta(meta, errors)
             if errors:
                 raise IncorrectMetaException(name, errors)
-            attrs['Meta'] = meta
+            attrs["Meta"] = meta
 
         return cls
 
     @staticmethod
     def find_base_options(bases):
         for b in reversed(bases):
-            options = getattr(b, 'Meta', None)
+            options = getattr(b, "Meta", None)
             if options is not None:
                 return options
 
     @staticmethod
     def merge_options(options, base_options):
         if options is None:
             return base_options
         elif base_options is None:
             return options
 
         members = inspect.getmembers(base_options)
         for name, obj in members:
-            if name.startswith('_'):
+            if name.startswith("_"):
                 continue
             setattr(options, name, copy.copy(getattr(options, name, obj)))
 
         return options
 
     @staticmethod
     def get_annotation(base_cls, name):
         for cls in base_cls.__mro__:
-            if hasattr(cls, '__annotations__'):
+            if hasattr(cls, "__annotations__"):
                 annt = cls.__annotations__.get(name)
                 if annt is not None:
                     return annt
 
     @classmethod
     def check_meta_extra(mcs, meta: Type, errors: List):
-        tags = getattr(meta, 'tags', None)
+        tags = getattr(meta, "tags", None)
         if not tags:
-            errors.append('`tags` is required')
+            errors.append("`tags` is required")
         else:
             if not isinstance(tags, List):
-                errors.append('`tags` variable has incorrect type, '
-                              'should be list')
+                errors.append("`tags` variable has incorrect type, " "should be list")
             else:
-                if any([not isinstance(item, str) for item in tags]):
-                    errors.append('`tags` item has incorrect type, '
-                                  'should be str')
+                if any(not isinstance(item, str) for item in tags):
+                    errors.append("`tags` item has incorrect type, " "should be str")
 
-        meta_errors = getattr(meta, 'errors', [])
+        meta_errors = getattr(meta, "errors", [])
         if meta_errors:
             if not isinstance(meta_errors, List):
-                errors.append('`errors` variable has incorrect type, '
-                              'should be list')
+                errors.append("`errors` variable has incorrect type, " "should be list")
             else:
                 try:
-                    if any([not issubclass(item, HttpError)
-                            for item in meta_errors]):
+                    if any(not issubclass(item, HttpError) for item in meta_errors):
                         raise TypeError
                 except TypeError:
-                    errors.append('`errors` item has incorrect type, '
-                                  'should be subtype of HttpError')
+                    errors.append(
+                        "`errors` item has incorrect type, "
+                        "should be subtype of HttpError"
+                    )
 
         return errors
 
     @classmethod
     def check_meta(mcs, meta: Type, errors: List):
         from typing import _GenericAlias
 
         manual_validation = mcs.Meta.__manual_validation__
         for field_name in dir(mcs.Meta):
-            if field_name.startswith('_') or field_name in manual_validation:
+            if field_name.startswith("_") or field_name in manual_validation:
                 continue
 
             field = getattr(meta, field_name, None)
             annt = mcs.get_annotation(mcs.Meta, field_name)
 
             if isinstance(annt, _GenericAlias) and annt.__origin__ == Union:
                 # Union[..., ] type is unsupported
                 required = False
                 _type = annt.__args__[0]
             else:
                 required = True
                 _type = annt
-            is_type = isinstance(_type, _GenericAlias) and \
-                      _type.__origin__ == type
+            is_type = isinstance(_type, _GenericAlias) and _type.__origin__ == type
             if is_type:
                 _type = _type.__args__[0]
 
             if required and field is None:
-                errors.append(f'`{field_name}` is required')
+                errors.append(f"`{field_name}` is required")
                 continue
             if field:
                 if is_type:
                     try:
                         is_correct_type = issubclass(field, _type)
                     except TypeError:
                         is_correct_type = False
                     if not is_correct_type:
-                        errors.append(f'`{field_name}` has incorrect type, '
-                                      f'should be subclass of `{_type}`')
+                        errors.append(
+                            f"`{field_name}` has incorrect type, "
+                            f"should be subclass of `{_type}`"
+                        )
                 elif not isinstance(field, _type):
-                    errors.append(f'`{field_name}` has incorrect type, '
-                                  f'should be `{_type}`')
+                    errors.append(
+                        f"`{field_name}` has incorrect type, " f"should be `{_type}`"
+                    )
 
         return errors
```

### Comparing `django-serializer-1.1.0/django_serializer/v2/views/mixins.py` & `django-serializer-1.2.0/django_serializer/v2/views/mixins.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,64 +1,72 @@
 from typing import Type
 
 from django.core.exceptions import ObjectDoesNotExist
 from django.db.models import Model
+from django.http import HttpRequest
 
 from django_serializer.v2.exceptions import (
     NotFoundError,
     AuthRequiredError,
     ForbiddenError,
 )
 
 
 class FormMixin:
     def get_form_kwargs(self):
         kwargs = {}
-        if self.request.method in ('POST', 'PUT', 'PATCH'):
-            kwargs.update({
-                'data': self.get_request_json(),
-                'files': self.request.FILES,
-            })
+        if self.request.method in ("POST", "PUT", "PATCH"):
+            kwargs.update(
+                {
+                    "data": self.get_request_json(self.request),
+                    "files": self.request.FILES,
+                }
+            )
         return kwargs
 
     def get_form_class(self):
         return self.Meta.model_form
 
     def get_form(self):
         form_class = self.get_form_class()
         return form_class(**self.get_form_kwargs())
 
 
 class ObjectMixin:
     def _get_object(self):
-        if hasattr(self, '_object'):
-            return getattr(self, '_object')
+        if hasattr(self, "_object"):
+            return getattr(self, "_object")
         try:
             obj = self.get_object()
-            setattr(self, '_object', obj)
+            setattr(self, "_object", obj)
             return obj
         except ObjectDoesNotExist:
             raise NotFoundError
 
     def get_object(self):
         m: Type[Model] = self.Meta.model
         key: str = self.Meta.object_key
         return m.objects.get(**{key: self.request_body[key]})
 
     def get_form_kwargs(self):
         kwargs = super().get_form_kwargs()
-        kwargs['instance'] = self._get_object()
+        kwargs["instance"] = self._get_object()
         return kwargs
 
 
 class LoginRequiredMixin:
-    def perform_request_pipelines(self):
-        if not self.request.user.is_authenticated:
+    """
+    Allow request only for authorized user
+    """
+
+    def _check_section_permission(self, request: HttpRequest):
+        if not request.user.is_authenticated:
             raise AuthRequiredError
-        super().perform_request_pipelines()
+
+        return super()._check_section_permission(request)
 
 
 class CheckPermissionsMixin:
     def has_permissions(self, **kwargs) -> bool:
         return True
 
     def check_permissions(self, **kwargs):
```

### Comparing `django-serializer-1.1.0/django_serializer/v2/views/paginator.py` & `django-serializer-1.2.0/django_serializer/v2/views/paginator.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 from warnings import warn
 
 from django import forms
 from django.db.models import QuerySet
 
 from django_serializer.v2.views import ApiView
 
-deprecated_names = [('Paginator', 'BasePaginator')]
+deprecated_names = [("Paginator", "BasePaginator")]
 
 
 class BasePaginator:
     form: Type[forms.Form] = None
 
     def __init__(self, view: ApiView, qs: Optional[Union[Collection, QuerySet]] = None):
         self.view: ApiView = view
         self._queryset = qs
         self.data = None
         self._count = None
 
         if self._queryset is None:
             warn(
                 (
-                    '`qs` argument will become mandatory in the future. '
-                    '`total_count` method may not work properly without `_queryset`'
+                    "`qs` argument will become mandatory in the future. "
+                    "`total_count` method may not work properly without `_queryset`"
                 ),
                 FutureWarning,
                 stacklevel=2,
             )
 
     @property
     def total_count(self) -> int:
@@ -58,31 +58,31 @@
         limit = forms.IntegerField(min_value=1, max_value=100, required=False)
 
     default_limit = 10
     condition_kwarg = None
     form = FromIdForm
 
     def _get_limit(self) -> int:
-        return self.data['limit'] or self.default_limit
+        return self.data["limit"] or self.default_limit
 
     def paginate(self, qs: Optional[QuerySet] = None) -> QuerySet:
-        from_id = self.data['from_id']
+        from_id = self.data["from_id"]
         limit = self._get_limit()
         queryset = self._get_queryset(qs)
         if from_id:
             queryset = queryset.filter(**{self.condition_kwarg: from_id})
         return queryset[:limit]
 
 
 class AscFromIdPaginator(FromIdPaginator):
-    condition_kwarg = 'id__gt'
+    condition_kwarg = "id__gt"
 
 
 class DescFromIdPaginator(FromIdPaginator):
-    condition_kwarg = 'id__lt'
+    condition_kwarg = "id__lt"
 
 
 class LimitOffsetPaginator(BasePaginator):
     class LimitOffsetPaginatorForm(forms.Form):
         limit = forms.IntegerField(min_value=1, max_value=100, required=False)
         offset = forms.IntegerField(min_value=0, required=False)
         all = forms.BooleanField(required=False)
@@ -116,28 +116,28 @@
             return 0
         try:
             return ceil(self.total_count / self._get_limit())
         except (TypeError, ZeroDivisionError):
             return 1
 
     def _get_limit(self) -> int:
-        if self.data['all']:
+        if self.data["all"]:
             return self.total_count
-        return self.data['limit'] or self.default_limit
+        return self.data["limit"] or self.default_limit
 
     def _get_offset(self) -> int:
-        if self.data['all']:
+        if self.data["all"]:
             return 0
-        return self.data['offset'] or self.default_offset
+        return self.data["offset"] or self.default_offset
 
     def paginate(
         self, qs: Optional[Union[Collection, QuerySet]] = None
     ) -> Union[Collection, QuerySet]:
         queryset = self._get_queryset(qs)
-        if self.data['all']:
+        if self.data["all"]:
             return queryset
         limit = self._get_limit()
         offset = self._get_offset()
         return queryset[offset : limit + offset]
 
 
 def __getattr__(name):
@@ -145,8 +145,8 @@
         if name == old_name:
             warn(
                 f"The '{old_name}' class or function is renamed '{new_name}'",
                 DeprecationWarning,
                 stacklevel=2,
             )
             return globals()[new_name]
-    raise AttributeError(f'module {__name__} has no attribute {name}')
+    raise AttributeError(f"module {__name__} has no attribute {name}")
```

### Comparing `django-serializer-1.1.0/django_serializer.egg-info/PKG-INFO` & `django-serializer-1.2.0/django_serializer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-serializer
-Version: 1.1.0
+Version: 1.2.0
 Summary: Library for creating simple django api
 Home-page: https://github.com/alexopryshko/django-serializer
 Author: Alexander Opryshko
 Author-email: alexopryshko@yandex.ru
 License: MIT
 Keywords: django-serializer setuptools development
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `django-serializer-1.1.0/django_serializer.egg-info/SOURCES.txt` & `django-serializer-1.2.0/django_serializer.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -18,20 +18,24 @@
 django_serializer/form/fields.py
 django_serializer/model/__init__.py
 django_serializer/model/base.py
 django_serializer/serializer/__init__.py
 django_serializer/serializer/base.py
 django_serializer/serializer/fields.py
 django_serializer/v2/__init__.py
+django_serializer/v2/parsers.py
+django_serializer/v2/renderers.py
+django_serializer/v2/serializer.py
+django_serializer/v2/serializer_fields.py
+django_serializer/v2/settings.py
 django_serializer/v2/exceptions/__init__.py
 django_serializer/v2/exceptions/base.py
 django_serializer/v2/exceptions/conf.py
 django_serializer/v2/exceptions/http.py
-django_serializer/v2/serializer/__init__.py
-django_serializer/v2/serializer/fields.py
+django_serializer/v2/exceptions/parser.py
 django_serializer/v2/swagger/__init__.py
 django_serializer/v2/swagger/base.py
 django_serializer/v2/swagger/utils.py
 django_serializer/v2/swagger/views.py
 django_serializer/v2/views/__init__.py
 django_serializer/v2/views/base.py
 django_serializer/v2/views/generics.py
```

### Comparing `django-serializer-1.1.0/setup.py` & `django-serializer-1.2.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,47 +2,40 @@
 from os import path
 from setuptools import setup, find_packages
 
 BASE_DIR = path.abspath(path.dirname(__file__))
 
 
 def find_version():
-    for line in open(path.join(BASE_DIR, 'django_serializer/__init__.py')):
-        if line.startswith('__version__'):
-            return re.match(r"""__version__\s*=\s*(['"])([^'"]+)\1""",
-                            line).group(2)
+    for line in open(path.join(BASE_DIR, "django_serializer/__init__.py")):
+        if line.startswith("__version__"):
+            return re.match(r"""__version__\s*=\s*(['"])([^'"]+)\1""", line).group(2)
 
 
 setup(
-    name='django-serializer',
+    name="django-serializer",
     version=find_version(),
-    description='Library for creating simple django api',
-    long_description='Library for creating simple django api',
-
-    author='Alexander Opryshko',
-    author_email='alexopryshko@yandex.ru',
-    url='https://github.com/alexopryshko/django-serializer',
-
-    license='MIT',
-
+    description="Library for creating simple django api",
+    long_description="Library for creating simple django api",
+    author="Alexander Opryshko",
+    author_email="alexopryshko@yandex.ru",
+    url="https://github.com/alexopryshko/django-serializer",
+    license="MIT",
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
-        'Development Status :: 3 - Alpha',
-
-        'Intended Audience :: Developers',
-        'Topic :: Software Development :: Build Tools',
-
-        'License :: OSI Approved :: MIT License',
-
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
+        "Development Status :: 3 - Alpha",
+        "Intended Audience :: Developers",
+        "Topic :: Software Development :: Build Tools",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
     ],
-    keywords='django-serializer setuptools development',
-    packages=find_packages(exclude=['contrib', 'docs', 'tests*']),
+    keywords="django-serializer setuptools development",
+    packages=find_packages(exclude=["contrib", "docs", "tests*"]),
     install_requires=[
-        'Django>=2.2',
-        'marshmallow>=3.14.0',
-        'apispec>=5.1.1',
-    ]
+        "Django>=3.2",
+        "marshmallow>=3.14.0",
+        "apispec>=5.1.1",
+    ],
 )
```

