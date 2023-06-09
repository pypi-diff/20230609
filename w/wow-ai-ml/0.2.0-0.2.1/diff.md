# Comparing `tmp/wow_ai_ml-0.2.0.tar.gz` & `tmp/wow_ai_ml-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wow_ai_ml-0.2.0.tar", max compression
+gzip compressed data, was "wow_ai_ml-0.2.1.tar", max compression
```

## Comparing `wow_ai_ml-0.2.0.tar` & `wow_ai_ml-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     6415 2023-02-14 16:37:26.303084 wow_ai_ml-0.2.0/README.md
--rw-r--r--   0        0        0      261 2023-06-05 09:29:58.859979 wow_ai_ml-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-30 05:04:46.921613 wow_ai_ml-0.2.0/wow_ai_ml/__init__.py
--rw-r--r--   0        0        0     7256 2023-03-30 07:20:26.331095 wow_ai_ml-0.2.0/wow_ai_ml/api.py
--rw-r--r--   0        0        0      267 2023-01-29 17:47:59.351874 wow_ai_ml-0.2.0/wow_ai_ml/default_configs/Dockerfile
--rw-r--r--   0        0        0     2701 2023-01-29 17:47:59.457372 wow_ai_ml-0.2.0/wow_ai_ml/default_configs/README.md
--rw-r--r--   0        0        0     3861 2023-01-29 17:47:57.963857 wow_ai_ml-0.2.0/wow_ai_ml/default_configs/_wsgi.py.tmpl
--rw-r--r--   0        0        0      563 2023-01-29 17:47:59.127706 wow_ai_ml-0.2.0/wow_ai_ml/default_configs/docker-compose.yml
--rw-r--r--   0        0        0       28 2023-01-29 17:47:59.904560 wow_ai_ml-0.2.0/wow_ai_ml/default_configs/requirements.txt
--rw-r--r--   0        0        0     1899 2023-01-29 17:47:56.017679 wow_ai_ml-0.2.0/wow_ai_ml/exceptions.py
--rw-r--r--   0        0        0     2375 2023-01-29 17:48:02.301568 wow_ai_ml-0.2.0/wow_ai_ml/helpers.py
--rw-r--r--   0        0        0    32398 2023-06-05 10:29:36.423042 wow_ai_ml-0.2.0/wow_ai_ml/model.py
--rw-r--r--   0        0        0     7542 2023-01-29 17:48:02.879893 wow_ai_ml-0.2.0/wow_ai_ml/server.py
--rw-r--r--   0        0        0        6 2023-02-01 14:28:47.129345 wow_ai_ml-0.2.0/wow_ai_ml/templates/preview.html
--rw-r--r--   0        0        0     1999 2023-01-29 17:48:03.663323 wow_ai_ml-0.2.0/wow_ai_ml/utils.py
--rw-r--r--   0        0        0     6846 1970-01-01 00:00:00.000000 wow_ai_ml-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     6415 2023-02-14 16:37:26.303084 wow_ai_ml-0.2.1/README.md
+-rw-r--r--   0        0        0      261 2023-06-09 09:44:49.334384 wow_ai_ml-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-01-30 05:04:46.921613 wow_ai_ml-0.2.1/wow_ai_ml/__init__.py
+-rw-r--r--   0        0        0     7256 2023-03-30 07:20:26.331095 wow_ai_ml-0.2.1/wow_ai_ml/api.py
+-rw-r--r--   0        0        0      267 2023-01-29 17:47:59.351874 wow_ai_ml-0.2.1/wow_ai_ml/default_configs/Dockerfile
+-rw-r--r--   0        0        0     2701 2023-01-29 17:47:59.457372 wow_ai_ml-0.2.1/wow_ai_ml/default_configs/README.md
+-rw-r--r--   0        0        0     3861 2023-01-29 17:47:57.963857 wow_ai_ml-0.2.1/wow_ai_ml/default_configs/_wsgi.py.tmpl
+-rw-r--r--   0        0        0      563 2023-01-29 17:47:59.127706 wow_ai_ml-0.2.1/wow_ai_ml/default_configs/docker-compose.yml
+-rw-r--r--   0        0        0       28 2023-01-29 17:47:59.904560 wow_ai_ml-0.2.1/wow_ai_ml/default_configs/requirements.txt
+-rw-r--r--   0        0        0     1899 2023-01-29 17:47:56.017679 wow_ai_ml-0.2.1/wow_ai_ml/exceptions.py
+-rw-r--r--   0        0        0     2375 2023-01-29 17:48:02.301568 wow_ai_ml-0.2.1/wow_ai_ml/helpers.py
+-rw-r--r--   0        0        0    33543 2023-06-09 09:09:50.321748 wow_ai_ml-0.2.1/wow_ai_ml/model.py
+-rw-r--r--   0        0        0     7542 2023-01-29 17:48:02.879893 wow_ai_ml-0.2.1/wow_ai_ml/server.py
+-rw-r--r--   0        0        0        6 2023-02-01 14:28:47.129345 wow_ai_ml-0.2.1/wow_ai_ml/templates/preview.html
+-rw-r--r--   0        0        0     1999 2023-01-29 17:48:03.663323 wow_ai_ml-0.2.1/wow_ai_ml/utils.py
+-rw-r--r--   0        0        0     6846 1970-01-01 00:00:00.000000 wow_ai_ml-0.2.1/PKG-INFO
```

### Comparing `wow_ai_ml-0.2.0/README.md` & `wow_ai_ml-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.0/wow_ai_ml/api.py` & `wow_ai_ml-0.2.1/wow_ai_ml/api.py`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.0/wow_ai_ml/default_configs/README.md` & `wow_ai_ml-0.2.1/wow_ai_ml/default_configs/README.md`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.0/wow_ai_ml/default_configs/_wsgi.py.tmpl` & `wow_ai_ml-0.2.1/wow_ai_ml/default_configs/_wsgi.py.tmpl`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.0/wow_ai_ml/default_configs/docker-compose.yml` & `wow_ai_ml-0.2.1/wow_ai_ml/default_configs/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.0/wow_ai_ml/exceptions.py` & `wow_ai_ml-0.2.1/wow_ai_ml/exceptions.py`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.0/wow_ai_ml/helpers.py` & `wow_ai_ml-0.2.1/wow_ai_ml/helpers.py`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.0/wow_ai_ml/model.py` & `wow_ai_ml-0.2.1/wow_ai_ml/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -304,15 +304,18 @@
         self.hostname = kwargs.get('hostname', '')
         self.access_token = kwargs.get('access_token', '')
 
     @abstractmethod
     def predict(self, tasks, **kwargs):
         pass
     @abstractmethod
-    def toolbar_predict(self, image, clickpoint, polygons, vertices,project,voice,prompt,image_pref,draw_polygons, **kwargs):
+    def toolbar_predict(self, image, clickpoint, polygons, vertices,project, **kwargs):
+        pass
+    @abstractmethod
+    def toolbar_predict_sam(self, image, clickpoint, polygons, vertices,project,voice,prompt,image_pref,draw_polygons, **kwargs):
         pass
     @abstractmethod
     def model(self,project, **kwargs):
         pass
     @abstractmethod
     def preview(self,project, **kwargs):
         pass
@@ -597,29 +600,47 @@
         if not cls._current_model:
             raise ValueError(f'Model is not loaded for {cls.__class__.__name__}: run setup() before using predict()')
 
         predictions = cls._current_model.model.predict(tasks, **kwargs)
         return predictions, cls._current_model
     @classmethod
     def toolbar_predict(
+        cls, image, clickpoint, polygons, vertices, project=None, label_config=None, force_reload=True, try_fetch=False, **kwargs
+    ):
+        if not os.getenv('LABEL_STUDIO_ML_BACKEND_V2', default=LABEL_STUDIO_ML_BACKEND_V2_DEFAULT):
+            if try_fetch:
+                m = cls.fetch(project, label_config, force_reload)
+            else:
+                m = cls.get(project)
+                if not m:
+                    raise FileNotFoundError('No model loaded. Specify "try_fetch=True" option.')
+            predictions = m.model.toolbar_predict(image, clickpoint, polygons, vertices,project, **kwargs)
+            return predictions, m
+
+        if not cls._current_model:
+            raise ValueError(f'Model is not loaded for {cls.__class__.__name__}: run setup() before using toolbar_predict()')
+        predictions = m.model.toolbar_predict( image, clickpoint, polygons, vertices,project, **kwargs)
+        return predictions, m
+    @classmethod
+    def toolbar_predict_sam(
         cls, image, clickpoint, polygons, vertices, project=None, voice=None,prompt=None,image_pref=None,draw_polygons=None,label_config=None, force_reload=True, try_fetch=False, **kwargs
     ):
         if not os.getenv('LABEL_STUDIO_ML_BACKEND_V2', default=LABEL_STUDIO_ML_BACKEND_V2_DEFAULT):
             if try_fetch:
                 m = cls.fetch(project, label_config, force_reload)
             else:
                 m = cls.get(project)
                 if not m:
                     raise FileNotFoundError('No model loaded. Specify "try_fetch=True" option.')
-            predictions = m.model.toolbar_predict(image, clickpoint, polygons, vertices,project, voice,prompt,image_pref,draw_polygons,**kwargs)
+            predictions = m.model.toolbar_predict_sam(image, clickpoint, polygons, vertices,project, voice,prompt,image_pref,draw_polygons,**kwargs)
             return predictions, m
 
         if not cls._current_model:
             raise ValueError(f'Model is not loaded for {cls.__class__.__name__}: run setup() before using toolbar_predict()')
-        predictions = m.model.toolbar_predict( image, clickpoint, polygons, vertices,project, voice,prompt,image_pref,draw_polygons,**kwargs)
+        predictions = m.model.toolbar_predict_sam( image, clickpoint, polygons, vertices,project, voice,prompt,image_pref,draw_polygons,**kwargs)
         return predictions, m
     @classmethod
     def model(cls,project=None,label_config=None, force_reload=True, try_fetch=False, **kwargs):
         if not os.getenv('LABEL_STUDIO_ML_BACKEND_V2', default=LABEL_STUDIO_ML_BACKEND_V2_DEFAULT):
             if try_fetch:
                 m = cls.fetch(project, label_config, force_reload)
             else:
```

### Comparing `wow_ai_ml-0.2.0/wow_ai_ml/server.py` & `wow_ai_ml-0.2.1/wow_ai_ml/server.py`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.0/wow_ai_ml/utils.py` & `wow_ai_ml-0.2.1/wow_ai_ml/utils.py`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.0/PKG-INFO` & `wow_ai_ml-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wow-ai-ml
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: TonyShark
 Author-email: quoi@wow-ai.inc
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

