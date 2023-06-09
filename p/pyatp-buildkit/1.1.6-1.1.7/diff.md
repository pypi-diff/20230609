# Comparing `tmp/pyatp_buildkit-1.1.6.tar.gz` & `tmp/pyatp_buildkit-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyatp_buildkit-1.1.6.tar", max compression
+gzip compressed data, was "pyatp_buildkit-1.1.7.tar", max compression
```

## Comparing `pyatp_buildkit-1.1.6.tar` & `pyatp_buildkit-1.1.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      501 2023-06-09 03:17:33.433895 pyatp_buildkit-1.1.6/pyproject.toml
--rw-r--r--   0        0        0     1148 2023-06-06 06:46:33.737928 pyatp_buildkit-1.1.6/src/pyatp_buildkit/__init__.py
--rw-r--r--   0        0        0    12346 2023-06-09 03:17:11.456109 pyatp_buildkit-1.1.6/src/pyatp_buildkit/build.py
--rw-r--r--   0        0        0      542 2023-06-06 06:46:33.738272 pyatp_buildkit-1.1.6/src/pyatp_buildkit/config.py
--rw-r--r--   0        0        0      529 2023-06-06 06:46:33.738346 pyatp_buildkit-1.1.6/src/pyatp_buildkit/dotdict.py
--rw-r--r--   0        0        0      610 2023-06-06 06:46:33.738426 pyatp_buildkit-1.1.6/src/pyatp_buildkit/error.py
--rw-r--r--   0        0        0  2680354 2023-06-06 06:46:33.750086 pyatp_buildkit-1.1.6/src/pyatp_buildkit/get-pip.py
--rw-r--r--   0        0        0     1249 2023-06-06 07:31:52.608041 pyatp_buildkit-1.1.6/src/pyatp_buildkit/templates/Dockerfile.j2
--rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 pyatp_buildkit-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0      501 2023-06-09 08:51:54.310008 pyatp_buildkit-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1148 2023-06-06 06:46:33.737928 pyatp_buildkit-1.1.7/src/pyatp_buildkit/__init__.py
+-rw-r--r--   0        0        0    12653 2023-06-09 08:51:22.159483 pyatp_buildkit-1.1.7/src/pyatp_buildkit/build.py
+-rw-r--r--   0        0        0      542 2023-06-06 06:46:33.738272 pyatp_buildkit-1.1.7/src/pyatp_buildkit/config.py
+-rw-r--r--   0        0        0      529 2023-06-06 06:46:33.738346 pyatp_buildkit-1.1.7/src/pyatp_buildkit/dotdict.py
+-rw-r--r--   0        0        0      610 2023-06-06 06:46:33.738426 pyatp_buildkit-1.1.7/src/pyatp_buildkit/error.py
+-rw-r--r--   0        0        0  2680354 2023-06-06 06:46:33.750086 pyatp_buildkit-1.1.7/src/pyatp_buildkit/get-pip.py
+-rw-r--r--   0        0        0     1356 2023-06-09 08:51:30.372907 pyatp_buildkit-1.1.7/src/pyatp_buildkit/templates/Dockerfile.j2
+-rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 pyatp_buildkit-1.1.7/PKG-INFO
```

### Comparing `pyatp_buildkit-1.1.6/src/pyatp_buildkit/__init__.py` & `pyatp_buildkit-1.1.7/src/pyatp_buildkit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyatp_buildkit-1.1.6/src/pyatp_buildkit/build.py` & `pyatp_buildkit-1.1.7/src/pyatp_buildkit/build.py`

 * *Files 3% similar despite different names*

```diff
@@ -185,14 +185,23 @@
         "--cmd",
         str,
         group="Targeted",
         excludes=["--all", ],
         help="iamge cmd ",
         default=None,
     )
+
+    extra_pip_packages :Any = cli.SwitchAttr(
+        '--extra_pip_packages',
+        str,
+        group="Targeted",
+        excludes=["--all", ],
+        help="iamge cmd ",
+        default="aiges pyatp",
+    )
     auto_run: Any = cli.Flag(
         ["--auto_run"],
         help="If Using Github Actions",
         default=True,
     )
 
     # extracts arbitrary keys and inserts them into the templating context
@@ -323,14 +332,16 @@
             render_vars['dockerfile'] = dockerfile_content
         global dockerfile_dir
         dockerfile_dir = os.path.join(TEMP_GEN_DIR, 'run')
         if not os.path.exists(dockerfile_dir):
             os.makedirs(dockerfile_dir)
 
         self.prepare_inference_task_and_module()
+        # extra pip packages
+        self.vars['extra_pip_packages'] = self.extra_pip_packages
 
         st = self.render(render_vars)
         with open(os.path.join(dockerfile_dir, Dockerfile), 'w') as dockerfile:
             dockerfile.write(st)
             dockerfile.close()
             log.info("write %s success" % os.path.abspath(os.path.join(dockerfile_dir, Dockerfile)))
```

### Comparing `pyatp_buildkit-1.1.6/src/pyatp_buildkit/config.py` & `pyatp_buildkit-1.1.7/src/pyatp_buildkit/config.py`

 * *Files identical despite different names*

### Comparing `pyatp_buildkit-1.1.6/src/pyatp_buildkit/dotdict.py` & `pyatp_buildkit-1.1.7/src/pyatp_buildkit/dotdict.py`

 * *Files identical despite different names*

### Comparing `pyatp_buildkit-1.1.6/src/pyatp_buildkit/error.py` & `pyatp_buildkit-1.1.7/src/pyatp_buildkit/error.py`

 * *Files identical despite different names*

### Comparing `pyatp_buildkit-1.1.6/src/pyatp_buildkit/get-pip.py` & `pyatp_buildkit-1.1.7/src/pyatp_buildkit/get-pip.py`

 * *Files identical despite different names*

### Comparing `pyatp_buildkit-1.1.6/src/pyatp_buildkit/templates/Dockerfile.j2` & `pyatp_buildkit-1.1.7/src/pyatp_buildkit/templates/Dockerfile.j2`

 * *Files 11% similar despite different names*

```diff
@@ -25,14 +25,18 @@
 {% if vars.requirements_txt %}
 RUN pip install --no-cache-dir pip==22.3.1
 RUN --mount=target=requirements.txt,source={{vars.requirements_txt}}  	pip install --no-cache-dir -r requirements.txt
 {% else %}
 
 {% endif %}
 
+{% if vars.extra_pip_pacakges %}
+RUN pip install --no-cache-dir  {{vars.extra_pip_packages }}
+
+{% endif %}
 
 
 {% if vars.model  %}
 ENV MODE_NAME={{vars.model}}
 {% endif %}
 {% if vars.model_path  %}
 ENV MODE_NAME={{vars.model_path}}
```

### Comparing `pyatp_buildkit-1.1.6/PKG-INFO` & `pyatp_buildkit-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatp-buildkit
-Version: 1.1.6
+Version: 1.1.7
 Summary: a iflytek ailab library ...
 License: Apache License 2
 Author: mjchen
 Author-email: mjchen@iflytek.com
 Requires-Python: >3.7
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

