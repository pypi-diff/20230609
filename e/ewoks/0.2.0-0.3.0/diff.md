# Comparing `tmp/ewoks-0.2.0.tar.gz` & `tmp/ewoks-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ewoks-0.2.0.tar", last modified: Mon Mar 27 18:36:15 2023, max compression
+gzip compressed data, was "dist/ewoks-0.3.0.tar", last modified: Fri Jun  9 09:51:42 2023, max compression
```

## Comparing `ewoks-0.2.0.tar` & `ewoks-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 18:36:15.000000 ewoks-0.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     1102 2023-03-27 15:52:19.000000 ewoks-0.2.0/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     2097 2023-03-27 18:36:15.000000 ewoks-0.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1307 2023-03-27 15:52:19.000000 ewoks-0.2.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-03-27 15:52:19.000000 ewoks-0.2.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1575 2023-03-27 18:36:15.000000 ewoks-0.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-03-27 15:52:19.000000 ewoks-0.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 18:36:15.000000 ewoks-0.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 18:36:15.000000 ewoks-0.2.0/src/ewoks/
--rw-rw-rw-   0 root         (0) root         (0)      217 2023-03-27 18:32:39.000000 ewoks-0.2.0/src/ewoks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2426 2023-03-27 17:59:59.000000 ewoks-0.2.0/src/ewoks/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     5018 2023-03-27 17:59:59.000000 ewoks-0.2.0/src/ewoks/bindings.py
--rw-rw-rw-   0 root         (0) root         (0)     1250 2023-03-27 17:59:59.000000 ewoks-0.2.0/src/ewoks/cliutils.py
--rw-rw-rw-   0 root         (0) root         (0)     1152 2023-03-27 15:52:19.000000 ewoks-0.2.0/src/ewoks/graph_cache.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 18:36:15.000000 ewoks-0.2.0/src/ewoks/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-27 18:36:09.000000 ewoks-0.2.0/src/ewoks/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 18:36:15.000000 ewoks-0.2.0/src/ewoks/tests/notebooks/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-27 18:36:09.000000 ewoks-0.2.0/src/ewoks/tests/notebooks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1732 2023-03-27 15:52:19.000000 ewoks-0.2.0/src/ewoks/tests/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)      489 2023-03-27 15:52:19.000000 ewoks-0.2.0/src/ewoks/tests/test_notebooks.py
--rw-rw-rw-   0 root         (0) root         (0)      193 2023-03-27 15:52:19.000000 ewoks-0.2.0/src/ewoks/tests/test_projects.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 18:36:15.000000 ewoks-0.2.0/src/ewoks.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2097 2023-03-27 18:36:15.000000 ewoks-0.2.0/src/ewoks.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      528 2023-03-27 18:36:15.000000 ewoks-0.2.0/src/ewoks.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-27 18:36:15.000000 ewoks-0.2.0/src/ewoks.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2023-03-27 18:36:15.000000 ewoks-0.2.0/src/ewoks.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      662 2023-03-27 18:36:15.000000 ewoks-0.2.0/src/ewoks.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-03-27 18:36:15.000000 ewoks-0.2.0/src/ewoks.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:51:42.000000 ewoks-0.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2023-06-09 09:47:32.000000 ewoks-0.3.0/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     2097 2023-06-09 09:51:42.000000 ewoks-0.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1307 2023-06-09 09:47:32.000000 ewoks-0.3.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-09 09:47:32.000000 ewoks-0.3.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2023-06-09 09:51:42.000000 ewoks-0.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-09 09:47:32.000000 ewoks-0.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:51:42.000000 ewoks-0.3.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:51:42.000000 ewoks-0.3.0/src/ewoks/
+-rw-rw-rw-   0 root         (0) root         (0)      217 2023-06-09 09:47:32.000000 ewoks-0.3.0/src/ewoks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2426 2023-06-09 09:47:32.000000 ewoks-0.3.0/src/ewoks/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5028 2023-06-09 09:47:32.000000 ewoks-0.3.0/src/ewoks/bindings.py
+-rw-rw-rw-   0 root         (0) root         (0)     1250 2023-06-09 09:47:32.000000 ewoks-0.3.0/src/ewoks/cliutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1152 2023-06-09 09:47:32.000000 ewoks-0.3.0/src/ewoks/graph_cache.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:51:42.000000 ewoks-0.3.0/src/ewoks/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-09 09:51:36.000000 ewoks-0.3.0/src/ewoks/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:51:42.000000 ewoks-0.3.0/src/ewoks/tests/notebooks/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-09 09:51:36.000000 ewoks-0.3.0/src/ewoks/tests/notebooks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1757 2023-06-09 09:47:32.000000 ewoks-0.3.0/src/ewoks/tests/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      489 2023-06-09 09:47:32.000000 ewoks-0.3.0/src/ewoks/tests/test_notebooks.py
+-rw-rw-rw-   0 root         (0) root         (0)      193 2023-06-09 09:47:32.000000 ewoks-0.3.0/src/ewoks/tests/test_projects.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:51:42.000000 ewoks-0.3.0/src/ewoks.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2097 2023-06-09 09:51:42.000000 ewoks-0.3.0/src/ewoks.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      528 2023-06-09 09:51:42.000000 ewoks-0.3.0/src/ewoks.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 09:51:42.000000 ewoks-0.3.0/src/ewoks.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-06-09 09:51:42.000000 ewoks-0.3.0/src/ewoks.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      636 2023-06-09 09:51:42.000000 ewoks-0.3.0/src/ewoks.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-09 09:51:42.000000 ewoks-0.3.0/src/ewoks.egg-info/top_level.txt
```

### Comparing `ewoks-0.2.0/LICENSE.md` & `ewoks-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ewoks-0.2.0/PKG-INFO` & `ewoks-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoks
-Version: 0.2.0
+Version: 0.3.0
 Summary: ESRF Workflow System
 Home-page: https://gitlab.esrf.fr/workflow/ewoks/ewoks/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoks/ewoks/
 Project-URL: Documentation, https://ewoks.readthedocs.io/
```

### Comparing `ewoks-0.2.0/README.md` & `ewoks-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ewoks-0.2.0/setup.cfg` & `ewoks-0.3.0/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -19,30 +19,30 @@
 
 [options]
 package_dir = 
 	=src
 packages = find:
 python_requires = >=3.6
 install_requires = 
-	ewokscore >=0.4,<0.5
+	ewokscore >=0.5,<1
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	ewoks=ewoks.__main__:main
 
 [options.extras_require]
 dask = 
-	ewoksdask >=0.1.1,<0.2
+	ewoksdask >=0.1.1,<1
 ppf = 
-	ewoksppf >=0.1.1,<0.2
+	ewoksppf >=0.1.1,<1
 orange = 
-	ewoksorange >=0.1.4,<0.2
+	ewoksorange >=0.1.4,<1
 esrf-data-portal = 
 	pyicat-plus
 test = 
 	%(dask)s
 	%(ppf)s
 	%(orange)s
 	%(esrf-data-portal)s
@@ -69,19 +69,14 @@
 exclude = 
 	.eggs
 
 [flake8_nb]
 ignore = E501, E203, W503, E402
 max-line-length = 88
 
-[build_sphinx]
-project = ewoks
-version = attr: ewoks.__version__
-source-dir = ./doc
-
 [coverage:run]
 omit = 
 	setup.py
 	*/tests/*
 
 [egg_info]
 tag_build =
```

### Comparing `ewoks-0.2.0/src/ewoks/__main__.py` & `ewoks-0.3.0/src/ewoks/__main__.py`

 * *Files identical despite different names*

### Comparing `ewoks-0.2.0/src/ewoks/bindings.py` & `ewoks-0.3.0/src/ewoks/bindings.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 def import_binding(engine: Optional[str]):
     if not engine or engine.lower() == "none":
         binding = "ewokscore"
     elif engine.startswith("ewoks"):
         warn(
             f"engine = '{engine}' is deprecated in favor of '{engine[5:]}'",
-            FutureWarning,
+            DeprecationWarning,
         )
         binding = engine
     else:
         binding = "ewoks" + engine
     return importlib.import_module(binding)
 
 
@@ -52,15 +52,15 @@
     upload_parameters: Optional[dict] = None,
     **execute_options,
 ):
     if binding:
         if engine:
             raise ValueError("'binding' and 'engine' cannot be used together")
         engine = binding
-        warn("'binding' is deprecated in favor of 'engine'", FutureWarning)
+        warn("'binding' is deprecated in favor of 'engine'", DeprecationWarning)
     with job_context(execinfo, engine=engine) as execinfo:
         if environment:
             environment = {k: str(v) for k, v in environment.items()}
             os.environ.update(environment)
 
         # Load the graph
         if load_options is None:
```

### Comparing `ewoks-0.2.0/src/ewoks/cliutils.py` & `ewoks-0.3.0/src/ewoks/cliutils.py`

 * *Files identical despite different names*

### Comparing `ewoks-0.2.0/src/ewoks/graph_cache.py` & `ewoks-0.3.0/src/ewoks/graph_cache.py`

 * *Files identical despite different names*

### Comparing `ewoks-0.2.0/src/ewoks/tests/test_cli.py` & `ewoks-0.3.0/src/ewoks/tests/test_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,25 +10,21 @@
 
 
 @pytest.mark.parametrize("graph_name", graph_names())
 @pytest.mark.parametrize("scheme", (None, "json"))
 @pytest.mark.parametrize("engine", (None, "dask", "ppf"))
 def test_execute(graph_name, scheme, engine, tmpdir):
     graph, expected = get_graph(graph_name)
-    argv = [
-        sys.executable,
-        "execute",
-        graph_name,
-        "--test",
-        "--outputs",
-        "all",
-        "--merge-outputs",
-    ]
+    argv = [sys.executable, "execute", graph_name, "--test", "--merge-outputs"]
     if engine:
         argv += ["--engine", engine]
+    if engine == "ppf":
+        argv += ["--outputs", "end"]
+    else:
+        argv += ["--outputs", "all"]
     if scheme:
         argv += ["--data-root-uri", str(tmpdir), "--data-scheme", scheme]
         varinfo = {"root_uri": str(tmpdir), "scheme": scheme}
     else:
         varinfo = None
 
     keep = graph
```

### Comparing `ewoks-0.2.0/src/ewoks.egg-info/PKG-INFO` & `ewoks-0.3.0/src/ewoks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoks
-Version: 0.2.0
+Version: 0.3.0
 Summary: ESRF Workflow System
 Home-page: https://gitlab.esrf.fr/workflow/ewoks/ewoks/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoks/ewoks/
 Project-URL: Documentation, https://ewoks.readthedocs.io/
```

### Comparing `ewoks-0.2.0/src/ewoks.egg-info/SOURCES.txt` & `ewoks-0.3.0/src/ewoks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ewoks-0.2.0/src/ewoks.egg-info/requires.txt` & `ewoks-0.3.0/src/ewoks.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-ewokscore<0.5,>=0.4
+ewokscore<1,>=0.5
 
 [dask]
-ewoksdask<0.2,>=0.1.1
+ewoksdask<1,>=0.1.1
 
 [dev]
-ewoksdask<0.2,>=0.1.1
-ewoksppf<0.2,>=0.1.1
-ewoksorange<0.2,>=0.1.4
+ewoksdask<1,>=0.1.1
+ewoksppf<1,>=0.1.1
+ewoksorange<1,>=0.1.4
 pyicat-plus
 pytest>=7
 testbook
 ipykernel
 importlib_resources
 black[jupyter]>=22
 flake8>=4
 flake8_nb>=0.3.1
 
 [doc]
-ewoksdask<0.2,>=0.1.1
-ewoksppf<0.2,>=0.1.1
-ewoksorange<0.2,>=0.1.4
+ewoksdask<1,>=0.1.1
+ewoksppf<1,>=0.1.1
+ewoksorange<1,>=0.1.4
 pyicat-plus
 pytest>=7
 testbook
 ipykernel
 importlib_resources
 sphinx>=4.5
 sphinx-autodoc-typehints>=1.16
 nbsphinx
 nbsphinx_link
 
 [esrf-data-portal]
 pyicat-plus
 
 [orange]
-ewoksorange<0.2,>=0.1.4
+ewoksorange<1,>=0.1.4
 
 [ppf]
-ewoksppf<0.2,>=0.1.1
+ewoksppf<1,>=0.1.1
 
 [test]
-ewoksdask<0.2,>=0.1.1
-ewoksppf<0.2,>=0.1.1
-ewoksorange<0.2,>=0.1.4
+ewoksdask<1,>=0.1.1
+ewoksppf<1,>=0.1.1
+ewoksorange<1,>=0.1.4
 pyicat-plus
 pytest>=7
 testbook
 ipykernel
 importlib_resources
```

