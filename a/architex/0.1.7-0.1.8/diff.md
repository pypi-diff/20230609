# Comparing `tmp/architex-0.1.7.tar.gz` & `tmp/architex-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "architex-0.1.7.tar", max compression
+gzip compressed data, was "architex-0.1.8.tar", max compression
```

## Comparing `architex-0.1.7.tar` & `architex-0.1.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      208 2023-05-18 04:41:44.332373 architex-0.1.7/README.md
--rw-r--r--   0        0        0      426 2023-05-22 03:23:32.832400 architex-0.1.7/architex/__init__.py
--rw-r--r--   0        0        0      167 2023-05-10 05:11:37.507795 architex-0.1.7/architex/__main__.py
--rw-r--r--   0        0        0    10347 2023-05-18 10:49:45.779180 architex-0.1.7/architex/controller.py
--rw-r--r--   0        0        0      942 2023-05-18 06:55:18.830557 architex-0.1.7/architex/view.py
--rw-r--r--   0        0        0      538 2023-05-22 03:23:32.666026 architex-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      977 1970-01-01 00:00:00.000000 architex-0.1.7/setup.py
--rw-r--r--   0        0        0      994 1970-01-01 00:00:00.000000 architex-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      208 2023-05-18 04:41:44.332373 architex-0.1.8/README.md
+-rw-r--r--   0        0        0      426 2023-06-09 01:24:08.536924 architex-0.1.8/architex/__init__.py
+-rw-r--r--   0        0        0      167 2023-05-10 05:11:37.507795 architex-0.1.8/architex/__main__.py
+-rw-r--r--   0        0        0    10396 2023-06-09 01:15:34.207401 architex-0.1.8/architex/controller.py
+-rw-r--r--   0        0        0      942 2023-05-18 06:55:18.830557 architex-0.1.8/architex/view.py
+-rw-r--r--   0        0        0      538 2023-06-09 01:24:08.529003 architex-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      977 1970-01-01 00:00:00.000000 architex-0.1.8/setup.py
+-rw-r--r--   0        0        0      994 1970-01-01 00:00:00.000000 architex-0.1.8/PKG-INFO
```

### Comparing `architex-0.1.7/architex/controller.py` & `architex-0.1.8/architex/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         for name, service in docker_compose["services"].items():
             containers[name] = service_to_container(name, service)
 
             global global_names
             if "nginx" in name or (service.get("image") is not None and "nginx" in service.get("image")) or (service.get("volumes") is not None and len([volume_string for volume_string in service['volumes'] if 'nginx' in volume_string])):
                 path_strings = compose_file.split('/')[:-1]
                 to_be_appended = [
-                    volume_string for volume_string in service['volumes']if 'nginx' in volume_string and 'conf' in volume_string][0].split(':')[0]
+                    volume_string for volume_string in service['volumes'] if 'nginx' in volume_string and 'conf' in volume_string][0].split(':')[0] if service.get("volumes") is not None else None
                 if (to_be_appended is None and service.get('build')):
                     to_be_appended = f'{service["build"]["context"]}/nginx.conf'
                 path_strings.append(to_be_appended)
                 global_names.append({'service_name': name, 'container_name':  service.get(
                     "container_name") if "container_name" in service else name, 'nginx_path': '/'.join(path_strings)})
             else:
                 global_names.append({'service_name': name, 'container_name':  service.get(
```

### Comparing `architex-0.1.7/architex/view.py` & `architex-0.1.8/architex/view.py`

 * *Files identical despite different names*

### Comparing `architex-0.1.7/pyproject.toml` & `architex-0.1.8/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "architex"
-version = "0.1.7"
+version = "0.1.8"
 description = "Draw your software architecture diagram automagically"
 authors = ["Miko <jherjati@gmail.com>"]
 readme = "README.md"
 packages = [{include = "architex"}]
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `architex-0.1.7/setup.py` & `architex-0.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'pytest==6.2.4',
  'pyyaml>=5.0,<6.0',
  'shellingham==1.4.0',
  'typer==0.3.2']
 
 setup_kwargs = {
     'name': 'architex',
-    'version': '0.1.7',
+    'version': '0.1.8',
     'description': 'Draw your software architecture diagram automagically',
     'long_description': 'A package to auto draw your software architecture diagram from your source code.\n\nCurrent limitation :\nYour source code should be consist of docker compose (required) and nginx (optional) configuration file.\n',
     'author': 'Miko',
     'author_email': 'jherjati@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `architex-0.1.7/PKG-INFO` & `architex-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: architex
-Version: 0.1.7
+Version: 0.1.8
 Summary: Draw your software architecture diagram automagically
 Author: Miko
 Author-email: jherjati@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

