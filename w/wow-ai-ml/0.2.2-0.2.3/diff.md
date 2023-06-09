# Comparing `tmp/wow_ai_ml-0.2.2.tar.gz` & `tmp/wow_ai_ml-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wow_ai_ml-0.2.2.tar", max compression
+gzip compressed data, was "wow_ai_ml-0.2.3.tar", max compression
```

## Comparing `wow_ai_ml-0.2.2.tar` & `wow_ai_ml-0.2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     6415 2023-02-14 16:37:26.303084 wow_ai_ml-0.2.2/README.md
--rw-r--r--   0        0        0      261 2023-06-09 10:00:38.307173 wow_ai_ml-0.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-30 05:04:46.921613 wow_ai_ml-0.2.2/wow_ai_ml/__init__.py
--rw-r--r--   0        0        0     8168 2023-06-09 09:58:48.295647 wow_ai_ml-0.2.2/wow_ai_ml/api.py
--rw-r--r--   0        0        0      267 2023-01-29 17:47:59.351874 wow_ai_ml-0.2.2/wow_ai_ml/default_configs/Dockerfile
--rw-r--r--   0        0        0     2701 2023-01-29 17:47:59.457372 wow_ai_ml-0.2.2/wow_ai_ml/default_configs/README.md
--rw-r--r--   0        0        0     3861 2023-01-29 17:47:57.963857 wow_ai_ml-0.2.2/wow_ai_ml/default_configs/_wsgi.py.tmpl
--rw-r--r--   0        0        0      563 2023-01-29 17:47:59.127706 wow_ai_ml-0.2.2/wow_ai_ml/default_configs/docker-compose.yml
--rw-r--r--   0        0        0       28 2023-01-29 17:47:59.904560 wow_ai_ml-0.2.2/wow_ai_ml/default_configs/requirements.txt
--rw-r--r--   0        0        0     1899 2023-01-29 17:47:56.017679 wow_ai_ml-0.2.2/wow_ai_ml/exceptions.py
--rw-r--r--   0        0        0     2375 2023-01-29 17:48:02.301568 wow_ai_ml-0.2.2/wow_ai_ml/helpers.py
--rw-r--r--   0        0        0    33543 2023-06-09 09:09:50.321748 wow_ai_ml-0.2.2/wow_ai_ml/model.py
--rw-r--r--   0        0        0     7542 2023-01-29 17:48:02.879893 wow_ai_ml-0.2.2/wow_ai_ml/server.py
--rw-r--r--   0        0        0        6 2023-02-01 14:28:47.129345 wow_ai_ml-0.2.2/wow_ai_ml/templates/preview.html
--rw-r--r--   0        0        0     1999 2023-01-29 17:48:03.663323 wow_ai_ml-0.2.2/wow_ai_ml/utils.py
--rw-r--r--   0        0        0     6846 1970-01-01 00:00:00.000000 wow_ai_ml-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     6415 2023-02-14 16:37:26.303084 wow_ai_ml-0.2.3/README.md
+-rw-r--r--   0        0        0      261 2023-06-09 10:27:47.518575 wow_ai_ml-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-01-30 05:04:46.921613 wow_ai_ml-0.2.3/wow_ai_ml/__init__.py
+-rw-r--r--   0        0        0     8234 2023-06-09 10:27:50.721177 wow_ai_ml-0.2.3/wow_ai_ml/api.py
+-rw-r--r--   0        0        0      267 2023-01-29 17:47:59.351874 wow_ai_ml-0.2.3/wow_ai_ml/default_configs/Dockerfile
+-rw-r--r--   0        0        0     2701 2023-01-29 17:47:59.457372 wow_ai_ml-0.2.3/wow_ai_ml/default_configs/README.md
+-rw-r--r--   0        0        0     3861 2023-01-29 17:47:57.963857 wow_ai_ml-0.2.3/wow_ai_ml/default_configs/_wsgi.py.tmpl
+-rw-r--r--   0        0        0      563 2023-01-29 17:47:59.127706 wow_ai_ml-0.2.3/wow_ai_ml/default_configs/docker-compose.yml
+-rw-r--r--   0        0        0       28 2023-01-29 17:47:59.904560 wow_ai_ml-0.2.3/wow_ai_ml/default_configs/requirements.txt
+-rw-r--r--   0        0        0     1899 2023-01-29 17:47:56.017679 wow_ai_ml-0.2.3/wow_ai_ml/exceptions.py
+-rw-r--r--   0        0        0     2375 2023-01-29 17:48:02.301568 wow_ai_ml-0.2.3/wow_ai_ml/helpers.py
+-rw-r--r--   0        0        0    33543 2023-06-09 09:09:50.321748 wow_ai_ml-0.2.3/wow_ai_ml/model.py
+-rw-r--r--   0        0        0     7542 2023-01-29 17:48:02.879893 wow_ai_ml-0.2.3/wow_ai_ml/server.py
+-rw-r--r--   0        0        0        6 2023-02-01 14:28:47.129345 wow_ai_ml-0.2.3/wow_ai_ml/templates/preview.html
+-rw-r--r--   0        0        0     1999 2023-01-29 17:48:03.663323 wow_ai_ml-0.2.3/wow_ai_ml/utils.py
+-rw-r--r--   0        0        0     6846 1970-01-01 00:00:00.000000 wow_ai_ml-0.2.3/PKG-INFO
```

### Comparing `wow_ai_ml-0.2.2/README.md` & `wow_ai_ml-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.2/wow_ai_ml/api.py` & `wow_ai_ml-0.2.3/wow_ai_ml/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -176,21 +176,21 @@
     image = data.get('image')
     clickpoint = data.get('clickpoint')
     polygons = data.get('polygons')
     vertices = data.get('vertices')
     label_config = data.get('label_config')
     force_reload = data.get('force_reload', False)
     try_fetch = data.get('try_fetch', True)
-    text = data.get('text')
-    question = data.get('question')
+    voice = data.get('voice')
+    prompt = data.get('prompt')
+    image_pref = data.get('image_pref')
+    draw_polygons = data.get('draw_polygons')
     params = data.get('params') or {}
-    params['text'] = text
-    params['question'] = question
-    predictions, model = _manager.toolbar_predict(
-        image, clickpoint, polygons, vertices, project, label_config, force_reload, try_fetch, **params)
+    predictions, model = _manager.toolbar_predict_sam(
+        image, clickpoint, polygons, vertices, project, voice,prompt,image_pref,draw_polygons,label_config, force_reload, try_fetch, **params)
     response = {
         'results': predictions,
         'model_version': model.model_version
     }
     return jsonify(response)
 
 @_server.route('/preview', methods=['GET'])
```

### Comparing `wow_ai_ml-0.2.2/wow_ai_ml/default_configs/README.md` & `wow_ai_ml-0.2.3/wow_ai_ml/default_configs/README.md`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.2/wow_ai_ml/default_configs/_wsgi.py.tmpl` & `wow_ai_ml-0.2.3/wow_ai_ml/default_configs/_wsgi.py.tmpl`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.2/wow_ai_ml/default_configs/docker-compose.yml` & `wow_ai_ml-0.2.3/wow_ai_ml/default_configs/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.2/wow_ai_ml/exceptions.py` & `wow_ai_ml-0.2.3/wow_ai_ml/exceptions.py`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.2/wow_ai_ml/helpers.py` & `wow_ai_ml-0.2.3/wow_ai_ml/helpers.py`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.2/wow_ai_ml/model.py` & `wow_ai_ml-0.2.3/wow_ai_ml/model.py`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.2/wow_ai_ml/server.py` & `wow_ai_ml-0.2.3/wow_ai_ml/server.py`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.2/wow_ai_ml/utils.py` & `wow_ai_ml-0.2.3/wow_ai_ml/utils.py`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.2/PKG-INFO` & `wow_ai_ml-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wow-ai-ml
-Version: 0.2.2
+Version: 0.2.3
 Summary: 
 Author: TonyShark
 Author-email: quoi@wow-ai.inc
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

