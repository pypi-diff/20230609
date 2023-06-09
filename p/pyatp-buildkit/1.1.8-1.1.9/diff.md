# Comparing `tmp/pyatp_buildkit-1.1.8.tar.gz` & `tmp/pyatp_buildkit-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyatp_buildkit-1.1.8.tar", max compression
+gzip compressed data, was "pyatp_buildkit-1.1.9.tar", max compression
```

## Comparing `pyatp_buildkit-1.1.8.tar` & `pyatp_buildkit-1.1.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      501 2023-06-09 09:15:26.607527 pyatp_buildkit-1.1.8/pyproject.toml
--rw-r--r--   0        0        0     1148 2023-06-06 06:46:33.737928 pyatp_buildkit-1.1.8/src/pyatp_buildkit/__init__.py
--rw-r--r--   0        0        0    12972 2023-06-09 09:15:08.148548 pyatp_buildkit-1.1.8/src/pyatp_buildkit/build.py
--rw-r--r--   0        0        0      542 2023-06-06 06:46:33.738272 pyatp_buildkit-1.1.8/src/pyatp_buildkit/config.py
--rw-r--r--   0        0        0      529 2023-06-06 06:46:33.738346 pyatp_buildkit-1.1.8/src/pyatp_buildkit/dotdict.py
--rw-r--r--   0        0        0      610 2023-06-06 06:46:33.738426 pyatp_buildkit-1.1.8/src/pyatp_buildkit/error.py
--rw-r--r--   0        0        0  2680354 2023-06-06 06:46:33.750086 pyatp_buildkit-1.1.8/src/pyatp_buildkit/get-pip.py
--rw-r--r--   0        0        0     1356 2023-06-09 08:51:30.372907 pyatp_buildkit-1.1.8/src/pyatp_buildkit/templates/Dockerfile.j2
--rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 pyatp_buildkit-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0      501 2023-06-09 09:48:04.798494 pyatp_buildkit-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1148 2023-06-06 06:46:33.737928 pyatp_buildkit-1.1.9/src/pyatp_buildkit/__init__.py
+-rw-r--r--   0        0        0    13271 2023-06-09 09:47:42.839162 pyatp_buildkit-1.1.9/src/pyatp_buildkit/build.py
+-rw-r--r--   0        0        0      542 2023-06-06 06:46:33.738272 pyatp_buildkit-1.1.9/src/pyatp_buildkit/config.py
+-rw-r--r--   0        0        0      529 2023-06-06 06:46:33.738346 pyatp_buildkit-1.1.9/src/pyatp_buildkit/dotdict.py
+-rw-r--r--   0        0        0      610 2023-06-06 06:46:33.738426 pyatp_buildkit-1.1.9/src/pyatp_buildkit/error.py
+-rw-r--r--   0        0        0  2680354 2023-06-06 06:46:33.750086 pyatp_buildkit-1.1.9/src/pyatp_buildkit/get-pip.py
+-rw-r--r--   0        0        0     1356 2023-06-09 09:45:19.922850 pyatp_buildkit-1.1.9/src/pyatp_buildkit/templates/Dockerfile.j2
+-rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 pyatp_buildkit-1.1.9/PKG-INFO
```

### Comparing `pyatp_buildkit-1.1.8/src/pyatp_buildkit/__init__.py` & `pyatp_buildkit-1.1.9/src/pyatp_buildkit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyatp_buildkit-1.1.8/src/pyatp_buildkit/build.py` & `pyatp_buildkit-1.1.9/src/pyatp_buildkit/build.py`

 * *Files 3% similar despite different names*

```diff
@@ -191,15 +191,14 @@
     )
 
     extra_pip_packages: Any = cli.SwitchAttr(
         '--extra_pip_packages',
         str,
         group="Targeted",
         excludes=["--all", ],
-        help="iamge cmd ",
         default="aiges pyatp",
     )
     auto_run: Any = cli.Flag(
         ["--auto_run"],
         help="If Using Github Actions",
         default=True,
     )
@@ -263,18 +262,22 @@
         # todo 拷贝推理文件以及目录
         if self.inference_script_path:
             valid = self.check_inference_path(self.inference_script_path)
             if valid:
                 log.info("copy files to workspace")
                 files = os.listdir(self.inference_script_path)
                 target_dir = os.path.join(dockerfile_dir, 'wrapper')
-                if not os.path.exists(target_dir):
-                    os.makedirs(target_dir)
+                #                if not os.path.exists(target_dir):
+                #                    os.makedirs(target_dir)
                 for f in files:
-                    shutil.copy(os.path.join(self.inference_script_path, f), target_dir)
+                    if os.path.isdir(os.path.join(self.inference_script_path, f)):
+                        shutil.copytree(os.path.join(self.inference_script_path, f), target_dir)
+                    else:
+                        shutil.copy(os.path.join(self.inference_script_path, f), os.path.join(dockerfile_dir, f))
+
                 if 'requirements.txt' in files:
                     log.info("finding. requirements.txt")
                     self.vars['requirements_txt'] = "wrapper/requirements.txt"
                 if 'packages.txt' in files:
                     log.info("finding. packages.txt")
                     self.vars['packages_txt'] = "wrapper/packages.txt"
             else:
@@ -325,32 +328,35 @@
             shutil.rmtree(TEMP_GEN_DIR)
 
         if not os.path.exists(TEMP_GEN_DIR):
             os.makedirs(TEMP_GEN_DIR)
         dockerfile_content = ''
         if os.path.exists(self.dockerfile):
             dockerfile_content = open(self.dockerfile).read()
-        render_vars = {
-            "vars": self.vars
-        }
+
         self.vars["base_image"] = self.base_image
         self.vars['maintainer'] = self.maintainer
         self.vars['pip_source'] = 'https://pypi.mirrors.ustc.edu.cn/simple/'
 
         if dockerfile_content:
-            render_vars['dockerfile'] = dockerfile_content
+            self.vars['dockerfile'] = dockerfile_content
         global dockerfile_dir
         dockerfile_dir = os.path.join(TEMP_GEN_DIR, 'run')
         if not os.path.exists(dockerfile_dir):
             os.makedirs(dockerfile_dir)
 
         self.prepare_inference_task_and_module()
         # extra pip packages
-        self.vars['extra_pip_packages'] = self.extra_pip_packages
+        if self.extra_pip_packages:
+            self.vars['extra_pip_packages'] = self.extra_pip_packages
 
+        # for render
+        render_vars = {
+            "vars": self.vars
+        }
         st = self.render(render_vars)
         log.info("Generated Dockerfile %s " % st)
         with open(os.path.join(dockerfile_dir, Dockerfile), 'w') as dockerfile:
             dockerfile.write(st)
             dockerfile.close()
             log.info("write %s success" % os.path.abspath(os.path.join(dockerfile_dir, Dockerfile)))
```

### Comparing `pyatp_buildkit-1.1.8/src/pyatp_buildkit/config.py` & `pyatp_buildkit-1.1.9/src/pyatp_buildkit/config.py`

 * *Files identical despite different names*

### Comparing `pyatp_buildkit-1.1.8/src/pyatp_buildkit/dotdict.py` & `pyatp_buildkit-1.1.9/src/pyatp_buildkit/dotdict.py`

 * *Files identical despite different names*

### Comparing `pyatp_buildkit-1.1.8/src/pyatp_buildkit/error.py` & `pyatp_buildkit-1.1.9/src/pyatp_buildkit/error.py`

 * *Files identical despite different names*

### Comparing `pyatp_buildkit-1.1.8/src/pyatp_buildkit/get-pip.py` & `pyatp_buildkit-1.1.9/src/pyatp_buildkit/get-pip.py`

 * *Files identical despite different names*

### Comparing `pyatp_buildkit-1.1.8/src/pyatp_buildkit/templates/Dockerfile.j2` & `pyatp_buildkit-1.1.9/src/pyatp_buildkit/templates/Dockerfile.j2`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 {% if vars.requirements_txt %}
 RUN pip install --no-cache-dir pip==22.3.1
 RUN --mount=target=requirements.txt,source={{vars.requirements_txt}}  	pip install --no-cache-dir -r requirements.txt
 {% else %}
 
 {% endif %}
 
-{% if vars.extra_pip_pacakges %}
+{% if vars.extra_pip_packages %}
 RUN pip install --no-cache-dir  {{vars.extra_pip_packages }}
 
 {% endif %}
 
 
 {% if vars.model  %}
 ENV MODE_NAME={{vars.model}}
```

### Comparing `pyatp_buildkit-1.1.8/PKG-INFO` & `pyatp_buildkit-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatp-buildkit
-Version: 1.1.8
+Version: 1.1.9
 Summary: a iflytek ailab library ...
 License: Apache License 2
 Author: mjchen
 Author-email: mjchen@iflytek.com
 Requires-Python: >3.7
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

