# Comparing `tmp/pyatp_buildkit-1.1.5.tar.gz` & `tmp/pyatp_buildkit-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyatp_buildkit-1.1.5.tar", max compression
+gzip compressed data, was "pyatp_buildkit-1.1.6.tar", max compression
```

## Comparing `pyatp_buildkit-1.1.5.tar` & `pyatp_buildkit-1.1.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      501 2023-06-09 03:05:48.521038 pyatp_buildkit-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     1148 2023-06-06 06:46:33.737928 pyatp_buildkit-1.1.5/src/pyatp_buildkit/__init__.py
--rw-r--r--   0        0        0    12371 2023-06-09 03:00:38.319936 pyatp_buildkit-1.1.5/src/pyatp_buildkit/build.py
--rw-r--r--   0        0        0      542 2023-06-06 06:46:33.738272 pyatp_buildkit-1.1.5/src/pyatp_buildkit/config.py
--rw-r--r--   0        0        0      529 2023-06-06 06:46:33.738346 pyatp_buildkit-1.1.5/src/pyatp_buildkit/dotdict.py
--rw-r--r--   0        0        0      610 2023-06-06 06:46:33.738426 pyatp_buildkit-1.1.5/src/pyatp_buildkit/error.py
--rw-r--r--   0        0        0  2680354 2023-06-06 06:46:33.750086 pyatp_buildkit-1.1.5/src/pyatp_buildkit/get-pip.py
--rw-r--r--   0        0        0     1249 2023-06-06 07:31:52.608041 pyatp_buildkit-1.1.5/src/pyatp_buildkit/templates/Dockerfile.j2
--rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 pyatp_buildkit-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0      501 2023-06-09 03:17:33.433895 pyatp_buildkit-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1148 2023-06-06 06:46:33.737928 pyatp_buildkit-1.1.6/src/pyatp_buildkit/__init__.py
+-rw-r--r--   0        0        0    12346 2023-06-09 03:17:11.456109 pyatp_buildkit-1.1.6/src/pyatp_buildkit/build.py
+-rw-r--r--   0        0        0      542 2023-06-06 06:46:33.738272 pyatp_buildkit-1.1.6/src/pyatp_buildkit/config.py
+-rw-r--r--   0        0        0      529 2023-06-06 06:46:33.738346 pyatp_buildkit-1.1.6/src/pyatp_buildkit/dotdict.py
+-rw-r--r--   0        0        0      610 2023-06-06 06:46:33.738426 pyatp_buildkit-1.1.6/src/pyatp_buildkit/error.py
+-rw-r--r--   0        0        0  2680354 2023-06-06 06:46:33.750086 pyatp_buildkit-1.1.6/src/pyatp_buildkit/get-pip.py
+-rw-r--r--   0        0        0     1249 2023-06-06 07:31:52.608041 pyatp_buildkit-1.1.6/src/pyatp_buildkit/templates/Dockerfile.j2
+-rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 pyatp_buildkit-1.1.6/PKG-INFO
```

### Comparing `pyatp_buildkit-1.1.5/src/pyatp_buildkit/__init__.py` & `pyatp_buildkit-1.1.6/src/pyatp_buildkit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyatp_buildkit-1.1.5/src/pyatp_buildkit/build.py` & `pyatp_buildkit-1.1.6/src/pyatp_buildkit/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -357,15 +357,16 @@
         if os.path.exists(docker_bin):
             mock = False
 
         if mock:
             self.mock_buildx()
             return
         pwd = os.getcwd()
-        cmd = f"docker buildx build . -t artifacts.iflytek.com/docker-private/atp/train/{self.inference_task}:{self.tag} --push"
+        cmd = f"docker buildx build . -t {self.docker_repo}/{self.build_name}:{self.image_tag} --push"
+
         log.info(cmd)
         os.chdir(dockerfile_dir)
         subprocess.call(cmd, shell=True)
         os.chdir(pwd)
 
     def render(self, render_vars):
         s = self.template.render(**render_vars)
```

### Comparing `pyatp_buildkit-1.1.5/src/pyatp_buildkit/config.py` & `pyatp_buildkit-1.1.6/src/pyatp_buildkit/config.py`

 * *Files identical despite different names*

### Comparing `pyatp_buildkit-1.1.5/src/pyatp_buildkit/dotdict.py` & `pyatp_buildkit-1.1.6/src/pyatp_buildkit/dotdict.py`

 * *Files identical despite different names*

### Comparing `pyatp_buildkit-1.1.5/src/pyatp_buildkit/error.py` & `pyatp_buildkit-1.1.6/src/pyatp_buildkit/error.py`

 * *Files identical despite different names*

### Comparing `pyatp_buildkit-1.1.5/src/pyatp_buildkit/get-pip.py` & `pyatp_buildkit-1.1.6/src/pyatp_buildkit/get-pip.py`

 * *Files identical despite different names*

### Comparing `pyatp_buildkit-1.1.5/src/pyatp_buildkit/templates/Dockerfile.j2` & `pyatp_buildkit-1.1.6/src/pyatp_buildkit/templates/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `pyatp_buildkit-1.1.5/PKG-INFO` & `pyatp_buildkit-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatp-buildkit
-Version: 1.1.5
+Version: 1.1.6
 Summary: a iflytek ailab library ...
 License: Apache License 2
 Author: mjchen
 Author-email: mjchen@iflytek.com
 Requires-Python: >3.7
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

