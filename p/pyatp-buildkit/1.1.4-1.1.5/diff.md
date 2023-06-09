# Comparing `tmp/pyatp_buildkit-1.1.4.tar.gz` & `tmp/pyatp_buildkit-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyatp_buildkit-1.1.4.tar", max compression
+gzip compressed data, was "pyatp_buildkit-1.1.5.tar", max compression
```

## Comparing `pyatp_buildkit-1.1.4.tar` & `pyatp_buildkit-1.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      501 2023-06-07 06:31:24.569362 pyatp_buildkit-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     1148 2023-06-06 06:46:33.737928 pyatp_buildkit-1.1.4/src/pyatp_buildkit/__init__.py
--rw-r--r--   0        0        0    11845 2023-06-07 03:47:47.377047 pyatp_buildkit-1.1.4/src/pyatp_buildkit/build.py
--rw-r--r--   0        0        0      542 2023-06-06 06:46:33.738272 pyatp_buildkit-1.1.4/src/pyatp_buildkit/config.py
--rw-r--r--   0        0        0      529 2023-06-06 06:46:33.738346 pyatp_buildkit-1.1.4/src/pyatp_buildkit/dotdict.py
--rw-r--r--   0        0        0      610 2023-06-06 06:46:33.738426 pyatp_buildkit-1.1.4/src/pyatp_buildkit/error.py
--rw-r--r--   0        0        0  2680354 2023-06-06 06:46:33.750086 pyatp_buildkit-1.1.4/src/pyatp_buildkit/get-pip.py
--rw-r--r--   0        0        0     1249 2023-06-06 07:31:52.608041 pyatp_buildkit-1.1.4/src/pyatp_buildkit/templates/Dockerfile.j2
--rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 pyatp_buildkit-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      501 2023-06-09 03:05:48.521038 pyatp_buildkit-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1148 2023-06-06 06:46:33.737928 pyatp_buildkit-1.1.5/src/pyatp_buildkit/__init__.py
+-rw-r--r--   0        0        0    12371 2023-06-09 03:00:38.319936 pyatp_buildkit-1.1.5/src/pyatp_buildkit/build.py
+-rw-r--r--   0        0        0      542 2023-06-06 06:46:33.738272 pyatp_buildkit-1.1.5/src/pyatp_buildkit/config.py
+-rw-r--r--   0        0        0      529 2023-06-06 06:46:33.738346 pyatp_buildkit-1.1.5/src/pyatp_buildkit/dotdict.py
+-rw-r--r--   0        0        0      610 2023-06-06 06:46:33.738426 pyatp_buildkit-1.1.5/src/pyatp_buildkit/error.py
+-rw-r--r--   0        0        0  2680354 2023-06-06 06:46:33.750086 pyatp_buildkit-1.1.5/src/pyatp_buildkit/get-pip.py
+-rw-r--r--   0        0        0     1249 2023-06-06 07:31:52.608041 pyatp_buildkit-1.1.5/src/pyatp_buildkit/templates/Dockerfile.j2
+-rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 pyatp_buildkit-1.1.5/PKG-INFO
```

### Comparing `pyatp_buildkit-1.1.4/src/pyatp_buildkit/__init__.py` & `pyatp_buildkit-1.1.5/src/pyatp_buildkit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyatp_buildkit-1.1.4/src/pyatp_buildkit/build.py` & `pyatp_buildkit-1.1.5/src/pyatp_buildkit/build.py`

 * *Files 7% similar despite different names*

```diff
@@ -59,14 +59,23 @@
         "--action",
         str,
         group="Targeted",
 
         excludes=["--all", ],
         default='build',
     )
+
+    build_name: Any = cli.SwitchAttr(
+        "--build_name",
+        str,
+        group="Targeted",
+
+        excludes=["--all", ],
+        default='test_aiservice',
+    )
     dockerfile: Any = cli.SwitchAttr(
         "--dockerfile",
         str,
         group="Targeted",
         excludes=["--all", ],
         default='',
     )
@@ -134,25 +143,33 @@
     )
     base_image: Any = cli.SwitchAttr(
         "--base_image",
         str,
         group="Targeted",
         excludes=["--all", ],
         help="base_image tag ",
-        default="artifacts.iflytek.com/docker-private/atp/atp_general_image:v1.0.8",
+        default="artifacts.iflytek.com/docker-private/atp/atp_general_image:v1.0.9",
+    )
+    docker_repo :Any = cli.SwitchAttr(
+        "--docker_repo",
+        str,
+        group="Targeted",
+        excludes=["--all",],
+        help="",
+        default="artifacts.iflytek.com/docker-private/atp/train",
     )
     maintainer: Any = cli.SwitchAttr(
         "--maintainer",
         str,
         group="Targeted",
         excludes=["--all", ],
         help="image entrypoint ",
         default="ybyang7@iflytek.com",
     )
-    tag: Any = cli.SwitchAttr(
+    image_tag: Any = cli.SwitchAttr(
         "--tag",
         str,
         group="Targeted",
         excludes=["--all", ],
         default="latest",
     )
     entrypoint: Any = cli.SwitchAttr(
@@ -239,16 +256,18 @@
                     shutil.copy(os.path.join(self.inference_script_path, f), target_dir)
                 if 'requirements.txt' in files:
                     log.info("finding. requirements.txt")
                     self.vars['requirements_txt'] = "wrapper/requirements.txt"
                 if 'packages.txt' in files:
                     log.info("finding. packages.txt")
                     self.vars['packages_txt'] = "wrapper/packages.txt"
+            else:
+                raise FileNotFoundError(self.inference_script_path)
         # transformer 内置
-        if self.is_transformers and self.inference_task:
+        elif self.is_transformers and self.inference_task:
             valid, m_path_dict = self.check_inference_task(self.inference_task)
             if valid:
                 self.vars['inference_wrapper_path'] = m_path_dict[self.inference_task]
                 log.info("is transformer.. using internal module: %s" % m_path_dict[self.inference_task])
 
             else:
                 log.info("not valid %s" % self.inference_task)
@@ -321,15 +340,17 @@
     def mock_buildx(self):
         global dockerfile_dir
         log.info("buildx dockerfile in %s" % dockerfile_dir)
         log.info("building: ")
         with open(os.path.abspath(os.path.join(dockerfile_dir, Dockerfile)), 'r') as f:
             log.info(f.read())
         f.close()
-        cmd = f"docker buildx build . -t artifacts.iflytek.com/docker-private/atp/train/{self.inference_task}:{self.tag} --push"
+        if not self.image_tag:
+            image_tag = "latest"
+        cmd = f"docker buildx build . -t {self.docker_repo}/{self.build_name}:{self.image_tag} --push"
         log.info(cmd)
 
     def buildx(self):
         # 1. check buildx command
         global dockerfile_dir
         mock = True
         docker_bin = "/usr/local/bin/docker"
```

### Comparing `pyatp_buildkit-1.1.4/src/pyatp_buildkit/config.py` & `pyatp_buildkit-1.1.5/src/pyatp_buildkit/config.py`

 * *Files identical despite different names*

### Comparing `pyatp_buildkit-1.1.4/src/pyatp_buildkit/dotdict.py` & `pyatp_buildkit-1.1.5/src/pyatp_buildkit/dotdict.py`

 * *Files identical despite different names*

### Comparing `pyatp_buildkit-1.1.4/src/pyatp_buildkit/error.py` & `pyatp_buildkit-1.1.5/src/pyatp_buildkit/error.py`

 * *Files identical despite different names*

### Comparing `pyatp_buildkit-1.1.4/src/pyatp_buildkit/get-pip.py` & `pyatp_buildkit-1.1.5/src/pyatp_buildkit/get-pip.py`

 * *Files identical despite different names*

### Comparing `pyatp_buildkit-1.1.4/src/pyatp_buildkit/templates/Dockerfile.j2` & `pyatp_buildkit-1.1.5/src/pyatp_buildkit/templates/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `pyatp_buildkit-1.1.4/PKG-INFO` & `pyatp_buildkit-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatp-buildkit
-Version: 1.1.4
+Version: 1.1.5
 Summary: a iflytek ailab library ...
 License: Apache License 2
 Author: mjchen
 Author-email: mjchen@iflytek.com
 Requires-Python: >3.7
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

