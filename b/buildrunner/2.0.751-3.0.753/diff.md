# Comparing `tmp/buildrunner-2.0.751.tar.gz` & `tmp/buildrunner-3.0.753.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildrunner-2.0.751.tar", last modified: Tue Feb 14 21:09:56 2023, max compression
+gzip compressed data, was "buildrunner-3.0.753.tar", last modified: Thu Jun  8 22:28:55 2023, max compression
```

## Comparing `buildrunner-2.0.751.tar` & `buildrunner-3.0.753.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 21:09:56.426912 buildrunner-2.0.751/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-02-14 21:09:53.000000 buildrunner-2.0.751/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-02-14 21:09:53.000000 buildrunner-2.0.751/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    69064 2023-02-14 21:09:56.426912 buildrunner-2.0.751/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    57583 2023-02-14 21:09:53.000000 buildrunner-2.0.751/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 21:09:56.422912 buildrunner-2.0.751/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      159 2023-02-14 21:09:53.000000 buildrunner-2.0.751/bin/buildrunner
--rwxr-xr-x   0 runner    (1001) docker     (123)      166 2023-02-14 21:09:53.000000 buildrunner-2.0.751/bin/buildrunner-cleanup
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 21:09:56.422912 buildrunner-2.0.751/buildrunner/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-02-14 21:09:53.000000 buildrunner-2.0.751/buildrunner/SourceDockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    27497 2023-02-14 21:09:53.000000 buildrunner-2.0.751/buildrunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-02-14 21:09:53.000000 buildrunner-2.0.751/buildrunner/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    15265 2023-02-14 21:09:53.000000 buildrunner-2.0.751/buildrunner/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 21:09:56.422912 buildrunner-2.0.751/buildrunner/docker/
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-02-14 21:09:53.000000 buildrunner-2.0.751/buildrunner/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-02-14 21:09:53.000000 buildrunner-2.0.751/buildrunner/docker/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-02-14 21:09:53.000000 buildrunner-2.0.751/buildrunner/docker/daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-02-14 21:09:53.000000 buildrunner-2.0.751/buildrunner/docker/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)    22485 2023-02-14 21:09:53.000000 buildrunner-2.0.751/buildrunner/docker/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-02-14 21:09:53.000000 buildrunner-2.0.751/buildrunner/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 21:09:56.422912 buildrunner-2.0.751/buildrunner/fetch/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-02-14 21:09:53.000000 buildrunner-2.0.751/buildrunner/fetch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-02-14 21:09:53.000000 buildrunner-2.0.751/buildrunner/fetch/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-02-14 21:09:53.000000 buildrunner-2.0.751/buildrunner/fetch/github.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-02-14 21:09:53.000000 buildrunner-2.0.751/buildrunner/fetch/http.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 21:09:56.422912 buildrunner-2.0.751/buildrunner/provisioners/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-02-14 21:09:53.000000 buildrunner-2.0.751/buildrunner/provisioners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-02-14 21:09:53.000000 buildrunner-2.0.751/buildrunner/provisioners/salt.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-02-14 21:09:53.000000 buildrunner-2.0.751/buildrunner/provisioners/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 21:09:56.422912 buildrunner-2.0.751/buildrunner/sshagent/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 21:09:56.422912 buildrunner-2.0.751/buildrunner/sshagent/SSHAgentProxyImage/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-02-14 21:09:53.000000 buildrunner-2.0.751/buildrunner/sshagent/SSHAgentProxyImage/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (123)      212 2023-02-14 21:09:53.000000 buildrunner-2.0.751/buildrunner/sshagent/SSHAgentProxyImage/login.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      338 2023-02-14 21:09:53.000000 buildrunner-2.0.751/buildrunner/sshagent/SSHAgentProxyImage/run.sh
--rw-r--r--   0 runner    (1001) docker     (123)    14860 2023-02-14 21:09:53.000000 buildrunner-2.0.751/buildrunner/sshagent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 21:09:56.422912 buildrunner-2.0.751/buildrunner/steprunner/
--rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-02-14 21:09:53.000000 buildrunner-2.0.751/buildrunner/steprunner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 21:09:56.426912 buildrunner-2.0.751/buildrunner/steprunner/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-02-14 21:09:53.000000 buildrunner-2.0.751/buildrunner/steprunner/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-02-14 21:09:53.000000 buildrunner-2.0.751/buildrunner/steprunner/tasks/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-02-14 21:09:53.000000 buildrunner-2.0.751/buildrunner/steprunner/tasks/push.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-02-14 21:09:53.000000 buildrunner-2.0.751/buildrunner/steprunner/tasks/pypipush.py
--rw-r--r--   0 runner    (1001) docker     (123)     6628 2023-02-14 21:09:53.000000 buildrunner-2.0.751/buildrunner/steprunner/tasks/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)    43606 2023-02-14 21:09:53.000000 buildrunner-2.0.751/buildrunner/steprunner/tasks/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    13163 2023-02-14 21:09:53.000000 buildrunner-2.0.751/buildrunner/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-14 21:09:56.000000 buildrunner-2.0.751/buildrunner/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 21:09:56.422912 buildrunner-2.0.751/buildrunner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    69064 2023-02-14 21:09:56.000000 buildrunner-2.0.751/buildrunner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-02-14 21:09:56.000000 buildrunner-2.0.751/buildrunner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 21:09:56.000000 buildrunner-2.0.751/buildrunner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-02-14 21:09:56.000000 buildrunner-2.0.751/buildrunner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-14 21:09:56.000000 buildrunner-2.0.751/buildrunner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-02-14 21:09:53.000000 buildrunner-2.0.751/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-02-14 21:09:56.426912 buildrunner-2.0.751/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-02-14 21:09:53.000000 buildrunner-2.0.751/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-02-14 21:09:53.000000 buildrunner-2.0.751/test_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:28:55.680530 buildrunner-3.0.753/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-08 22:28:47.000000 buildrunner-3.0.753/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-08 22:28:47.000000 buildrunner-3.0.753/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    69064 2023-06-08 22:28:55.680530 buildrunner-3.0.753/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    57583 2023-06-08 22:28:47.000000 buildrunner-3.0.753/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:28:55.672530 buildrunner-3.0.753/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      159 2023-06-08 22:28:47.000000 buildrunner-3.0.753/bin/buildrunner
+-rwxr-xr-x   0 runner    (1001) docker     (123)      166 2023-06-08 22:28:47.000000 buildrunner-3.0.753/bin/buildrunner-cleanup
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:28:55.676530 buildrunner-3.0.753/buildrunner/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/SourceDockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    27674 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15314 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:28:55.676530 buildrunner-3.0.753/buildrunner/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/docker/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/docker/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/docker/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22485 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/docker/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:28:55.676530 buildrunner-3.0.753/buildrunner/fetch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/fetch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/fetch/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/fetch/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/fetch/http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:28:55.676530 buildrunner-3.0.753/buildrunner/provisioners/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/provisioners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/provisioners/salt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/provisioners/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:28:55.676530 buildrunner-3.0.753/buildrunner/sshagent/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:28:55.676530 buildrunner-3.0.753/buildrunner/sshagent/SSHAgentProxyImage/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/sshagent/SSHAgentProxyImage/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (123)      212 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/sshagent/SSHAgentProxyImage/login.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      338 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/sshagent/SSHAgentProxyImage/run.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    14938 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/sshagent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:28:55.676530 buildrunner-3.0.753/buildrunner/steprunner/
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/steprunner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:28:55.680530 buildrunner-3.0.753/buildrunner/steprunner/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/steprunner/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/steprunner/tasks/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/steprunner/tasks/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/steprunner/tasks/pypipush.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6628 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/steprunner/tasks/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43785 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/steprunner/tasks/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-08 22:28:54.000000 buildrunner-3.0.753/buildrunner/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:28:55.676530 buildrunner-3.0.753/buildrunner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    69064 2023-06-08 22:28:55.000000 buildrunner-3.0.753/buildrunner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-08 22:28:55.000000 buildrunner-3.0.753/buildrunner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 22:28:55.000000 buildrunner-3.0.753/buildrunner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-08 22:28:55.000000 buildrunner-3.0.753/buildrunner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-08 22:28:55.000000 buildrunner-3.0.753/buildrunner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-08 22:28:47.000000 buildrunner-3.0.753/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-08 22:28:55.680530 buildrunner-3.0.753/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-06-08 22:28:47.000000 buildrunner-3.0.753/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-08 22:28:47.000000 buildrunner-3.0.753/test_requirements.txt
```

### Comparing `buildrunner-2.0.751/LICENSE` & `buildrunner-3.0.753/LICENSE`

 * *Files identical despite different names*

### Comparing `buildrunner-2.0.751/PKG-INFO` & `buildrunner-3.0.753/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildrunner
-Version: 2.0.751
+Version: 3.0.753
 Summary: Docker-based build tool
 Home-page: https://github.com/adobe/buildrunner
 Author: Adobe
 Author-email: noreply@adobe.com
 License: MIT
 Description: #############
          Buildrunner
```

### Comparing `buildrunner-2.0.751/README.rst` & `buildrunner-3.0.753/README.rst`

 * *Files identical despite different names*

### Comparing `buildrunner-2.0.751/buildrunner/__init__.py` & `buildrunner-3.0.753/buildrunner/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,15 +215,15 @@
         #   the global config object
         self.env = self._get_config_context(base_context, self.global_config.get('env', {}))
         # assign back to the global config env for loading files
         self.global_config.env = self.env
 
         # print out env vars
         # pylint: disable=consider-iterating-dictionary
-        key_len = max([len(key) for key in self.env.keys()])
+        key_len = max(len(key) for key in self.env.keys())
         for key in sorted(self.env.keys()):
             val = self.env[key]
             LOGGER.debug(f'Environment: {key!s:>{key_len}}: {val}')
 
         # cleanup local cache
         if self.cleanup_cache:
             self.clean_cache(self.global_config)
@@ -270,15 +270,16 @@
             except OSError as exc:
                 if exc.errno != errno.EEXIST:
                     sys.stderr.write(f'ERROR: {str(exc)}\n')
                     sys.exit(os.EX_UNAVAILABLE)
 
             try:
                 log_file_path = os.path.join(self.build_results_dir, 'build.log')
-                self._log_file = open(log_file_path, 'w')
+                # pylint: disable=consider-using-with
+                self._log_file = open(log_file_path, 'w', encoding='utf8')
                 self._log = ConsoleLogger(self.colorize_log, self._log_file)
 
                 self.add_artifact(
                     os.path.basename(log_file_path),
                     {'type': 'log'},
                 )
             except Exception as exc:  # pylint: disable=broad-except
@@ -381,14 +382,15 @@
                 local_path = os.path.realpath(
                     os.path.expanduser(os.path.expandvars(local_file))
                 )
                 if os.path.exists(local_path):
                     return local_path
 
                 # need to put the contents in a tmp file and return the path
+                # pylint: disable=consider-using-with
                 _fileobj = tempfile.NamedTemporaryFile(
                     delete=False,
                     dir=self.global_config.get_temp_dir(),
                 )
                 _fileobj.write(local_file)
                 tmp_path = os.path.realpath(_fileobj.name)
                 _fileobj.close()
@@ -466,14 +468,15 @@
                     if fnmatch.fnmatch(tarinfo.name, _ex):
                         return None
                 return tarinfo
 
             self.log.write('Creating source archive\n')
             _fileobj = None
             try:
+                # pylint: disable=consider-using-with
                 _fileobj = tempfile.NamedTemporaryFile(
                     delete=False,
                     dir=self.global_config.get_temp_dir(),
                 )
                 with tarfile.open(mode='w', fileobj=_fileobj) as tfile:
                     tfile.add(
                         self.build_dir,
```

### Comparing `buildrunner-2.0.751/buildrunner/cli.py` & `buildrunner-3.0.753/buildrunner/cli.py`

 * *Files identical despite different names*

### Comparing `buildrunner-2.0.751/buildrunner/config.py` & `buildrunner-3.0.753/buildrunner/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     """
 
     @staticmethod
     def _raise_exception_jinja(message):
         """
         Raises an exception from a jinja template.
         """
+        # pylint: disable=broad-exception-raised
         raise Exception(message)
 
     @staticmethod
     def _re_sub_filter(text, pattern, replace, count=0, flags=0):
         """
         Filter for regular expression replacement.
         :param text: The string being examined for ``pattern``
```

### Comparing `buildrunner-2.0.751/buildrunner/docker/__init__.py` & `buildrunner-3.0.753/buildrunner/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `buildrunner-2.0.751/buildrunner/docker/builder.py` & `buildrunner-3.0.753/buildrunner/docker/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         self.temp_dir = temp_dir
         self.dockerfile = None
         self.cleanup_dockerfile = False
         if dockerfile:
             if os.path.exists(dockerfile):
                 self.dockerfile = dockerfile
             else:
+                # pylint: disable=consider-using-with
                 df_file = tempfile.NamedTemporaryFile(delete=False, dir=self.temp_dir)
                 try:
                     df_file.write(dockerfile.encode('utf-8'))
                     self.cleanup_dockerfile = True
                     self.dockerfile = df_file.name
                 finally:
                     df_file.close()
@@ -84,24 +85,24 @@
         context tar file if necessary.
         """
         if cache_from is None:
             cache_from = []
         if buildargs is None:
             buildargs = {}
         # create our own tar file, injecting the appropriate paths
+        # pylint: disable=consider-using-with
         _fileobj = tempfile.NamedTemporaryFile(dir=self.temp_dir)
-        tfile = tarfile.open(mode='w', fileobj=_fileobj)
-        if self.path:
-            tfile.add(self.path, arcname='.')
-        if self.inject:
-            for to_inject, dest in self.inject.items():
-                tfile.add(to_inject, arcname=dest)
-        if self.dockerfile:
-            tfile.add(self.dockerfile, arcname='./Dockerfile')
-        tfile.close()
+        with tarfile.open(mode='w', fileobj=_fileobj) as tfile:
+            if self.path:
+                tfile.add(self.path, arcname='.')
+            if self.inject:
+                for to_inject, dest in self.inject.items():
+                    tfile.add(to_inject, arcname=dest)
+            if self.dockerfile:
+                tfile.add(self.dockerfile, arcname='./Dockerfile')
         _fileobj.seek(0)
 
         # Always add default registry to build args
         buildargs['DOCKER_REGISTRY'] = self.docker_registry
 
         stream = self.docker_client.build(
             path=None,
```

### Comparing `buildrunner-2.0.751/buildrunner/docker/daemon.py` & `buildrunner-3.0.753/buildrunner/docker/daemon.py`

 * *Files identical despite different names*

### Comparing `buildrunner-2.0.751/buildrunner/docker/importer.py` & `buildrunner-3.0.753/buildrunner/docker/importer.py`

 * *Files identical despite different names*

### Comparing `buildrunner-2.0.751/buildrunner/docker/runner.py` & `buildrunner-3.0.753/buildrunner/docker/runner.py`

 * *Files identical despite different names*

### Comparing `buildrunner-2.0.751/buildrunner/errors.py` & `buildrunner-3.0.753/buildrunner/errors.py`

 * *Files identical despite different names*

### Comparing `buildrunner-2.0.751/buildrunner/fetch/__init__.py` & `buildrunner-3.0.753/buildrunner/fetch/__init__.py`

 * *Files identical despite different names*

### Comparing `buildrunner-2.0.751/buildrunner/fetch/github.py` & `buildrunner-3.0.753/buildrunner/fetch/github.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,26 +31,26 @@
     auth = (username, config.get('app_token', ''))
     url = '/'.join((
         endpoint,
         version,
         'users',
         username,
     ))
-    resp = requests.get(url, auth=auth)
+    resp = requests.get(url, auth=auth, timeout=180)
     if resp.status_code != 200:
         raise BuildRunnerProtocolError(f'Failed authenticating {username} on {endpoint}')
 
     if not parsed_url.path.startswith('/'):
         raise ValueError('URL must begin with "/"')
 
     fpath = parsed_url.path.split('/')
     ubuild = [endpoint, version, 'repos', fpath[1], fpath[2], 'contents']
     ubuild.extend(fpath[3:])
     url = '/'.join(ubuild)
-    resp = requests.get(url, auth=auth)
+    resp = requests.get(url, auth=auth, timeout=180)
     if resp.status_code != 200:
         raise BuildRunnerProtocolError(f'Failed fetching URL: {url}')
     json_c = resp.json()
 
     encoding = json_c.get('encoding')
     enc_contents = json_c.get('content')
     if encoding == 'base64':
```

### Comparing `buildrunner-2.0.751/buildrunner/provisioners/__init__.py` & `buildrunner-3.0.753/buildrunner/provisioners/__init__.py`

 * *Files identical despite different names*

### Comparing `buildrunner-2.0.751/buildrunner/provisioners/salt.py` & `buildrunner-3.0.753/buildrunner/provisioners/salt.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         """
         if self.console:
             self.console.write('Running salt provisioner...\n')
 
         # see if salt is installed, bootstrap if it isn't
         if runner.run('salt-call -h') != 0:
             # pull bootstrap and run as a script
-            bootstrap_response = requests.get('http://bootstrap.saltstack.org')
+            bootstrap_response = requests.get('http://bootstrap.saltstack.org', timeout=600)
             if bootstrap_response.status_code != 200:
                 raise BuildRunnerProvisionerError(
                     "Unable to get salt bootstrap"
                 )
             if self.console:
                 self.console.write(
                     'Cannot detect salt installation--bootstrapping...\n'
```

### Comparing `buildrunner-2.0.751/buildrunner/provisioners/shell.py` & `buildrunner-3.0.753/buildrunner/provisioners/shell.py`

 * *Files identical despite different names*

### Comparing `buildrunner-2.0.751/buildrunner/sshagent/SSHAgentProxyImage/Dockerfile` & `buildrunner-3.0.753/buildrunner/sshagent/SSHAgentProxyImage/Dockerfile`

 * *Files identical despite different names*

### Comparing `buildrunner-2.0.751/buildrunner/sshagent/__init__.py` & `buildrunner-3.0.753/buildrunner/sshagent/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,16 @@
     RSAKey,
     ECDSAKey,
     Ed25519Key,
     SSHClient,
     SSHException,
 )
 from paramiko.agent import AgentSSH
-from paramiko.common import asbytes, io_sleep
+from paramiko.common import io_sleep
+from paramiko.util import asbytes
 from paramiko.message import Message
 
 from buildrunner.errors import (
     BuildRunnerConfigurationError,
     BuildRunnerProcessingError,
 )
 from buildrunner.docker.builder import DockerBuilder
@@ -220,14 +221,15 @@
                 self.log.write(f'there was an issue trying to connect to container : {exc}')
             next_backoff = backoff + previous_backoff
             previous_backoff = backoff
             backoff = next_backoff
             time.sleep(backoff)
         else:
             self.log.write(f'Unable to successfully connect to {ssh_host}')
+            # pylint: disable=broad-exception-raised
             raise Exception(f'Unable to successfully connect to {ssh_host}')
 
     def stop(self):
         """
         Stops the custom agent thread, kills the persistant ssh connection to
         the remote container, and kills the container.
         """
```

### Comparing `buildrunner-2.0.751/buildrunner/steprunner/__init__.py` & `buildrunner-3.0.753/buildrunner/steprunner/__init__.py`

 * *Files identical despite different names*

### Comparing `buildrunner-2.0.751/buildrunner/steprunner/tasks/__init__.py` & `buildrunner-3.0.753/buildrunner/steprunner/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `buildrunner-2.0.751/buildrunner/steprunner/tasks/build.py` & `buildrunner-3.0.753/buildrunner/steprunner/tasks/build.py`

 * *Files identical despite different names*

### Comparing `buildrunner-2.0.751/buildrunner/steprunner/tasks/push.py` & `buildrunner-3.0.753/buildrunner/steprunner/tasks/push.py`

 * *Files identical despite different names*

### Comparing `buildrunner-2.0.751/buildrunner/steprunner/tasks/pypipush.py` & `buildrunner-3.0.753/buildrunner/steprunner/tasks/pypipush.py`

 * *Files identical despite different names*

### Comparing `buildrunner-2.0.751/buildrunner/steprunner/tasks/remote.py` & `buildrunner-3.0.753/buildrunner/steprunner/tasks/remote.py`

 * *Files identical despite different names*

### Comparing `buildrunner-2.0.751/buildrunner/steprunner/tasks/run.py` & `buildrunner-3.0.753/buildrunner/steprunner/tasks/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,14 +222,15 @@
                 # process are set as the owner of the files
                 exit_code = artifact_lister.run(
                     f'chown -R {int(os.getuid())}:{int(os.getgid())} /stepresults',
                     console=console,
                     log=self.step_runner.log,
                 )
                 if exit_code != 0:
+                    # pylint: disable=broad-exception-raised
                     raise Exception(
                         "Error gathering artifacts--unable to change ownership"
                     )
 
                 artifact_lister.cleanup()
 
     def _archive_dir(
@@ -270,14 +271,15 @@
                         '/stepresults/' + _dir_name,
                     )
                     exit_code = artifact_lister.run(
                         archive_command,
                         log=self.step_runner.log,
                     )
                     if exit_code != 0:
+                        # pylint: disable=broad-exception-raised
                         raise Exception(
                             f"Error gathering artifact {artifact_file}",
                         )
                     archive_command = (
                         'cp',
                         '-r',
                         _file,
@@ -379,14 +381,15 @@
 
         exit_code = artifact_lister.run(
             archive_command,
             log=self.step_runner.log,
             workdir=workdir,
         )
         if exit_code != 0:
+            # pylint: disable=broad-exception-raised
             raise Exception(
                 f"Error gathering artifact {artifact_file}",
             )
 
         if not properties or (isinstance(properties, dict) and properties.get('push', True)):
             # register the artifact with the run controller
             self.step_runner.build_runner.add_artifact(
```

### Comparing `buildrunner-2.0.751/buildrunner/utils.py` & `buildrunner-3.0.753/buildrunner/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,14 +197,15 @@
         if not isinstance(output, str):
             output = str(output, encoding=sys.stdout.encoding, errors='replace')
         _stdout = output
 
         # colorize stdout
         if color and self.colorize_log:
             # Colorize stdout
+            # pylint: disable=invalid-character-esc
             _stdout = f'[01;3{color}m{_stdout}\033[00;00m'
         self.stdout.write(_stdout)
 
         # do not colorize output to other streams
         for stream in self.streams:
             try:
                 if stream.closed:
@@ -335,14 +336,15 @@
     :param lock_file: path and file name of file open and lock
     :param logger: logger to log messages
     :param mode: mode used by open()
     :param timeout_seconds: number of seconds for timeout
     :param exclusive: config exclusive lock (True) or shared lock (False), defaults to True
     :return: opened file object if successful else None
     """
+    # pylint: disable=unspecified-encoding,consider-using-with
     file_obj = open(lock_file, mode)
     pid = os.getpid()
     lock_file_obj = None
     retry_sleep_seconds = 0.5
 
     start_time = current_time = time.time()
     duration_seconds = current_time - start_time
```

### Comparing `buildrunner-2.0.751/buildrunner.egg-info/PKG-INFO` & `buildrunner-3.0.753/buildrunner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildrunner
-Version: 2.0.751
+Version: 3.0.753
 Summary: Docker-based build tool
 Home-page: https://github.com/adobe/buildrunner
 Author: Adobe
 Author-email: noreply@adobe.com
 License: MIT
 Description: #############
          Buildrunner
```

### Comparing `buildrunner-2.0.751/buildrunner.egg-info/SOURCES.txt` & `buildrunner-3.0.753/buildrunner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `buildrunner-2.0.751/requirements.txt` & `buildrunner-3.0.753/requirements.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,116 +1,115 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile
 #
-bcrypt==3.2.0
+bcrypt==4.0.1
     # via
     #   -r requirements.in
     #   paramiko
-bleach==4.1.0
+bleach==6.0.0
     # via readme-renderer
-certifi==2022.6.15
+certifi==2023.5.7
     # via requests
-cffi==1.15.0
+cffi==1.15.1
     # via
-    #   bcrypt
     #   cryptography
     #   pynacl
-charset-normalizer==2.0.12
+charset-normalizer==3.1.0
     # via requests
-colorama==0.4.5
-    # via twine
-cryptography==37.0.2
+cryptography==41.0.1
     # via paramiko
-decorator==5.1.0
-    # via -r requirements.in
-docker==4.4.4
+decorator==5.1.1
+    # via
+    #   -r requirements.in
+    #   fabric
+docker==6.1.3
     # via -r requirements.in
-docutils==0.18.1
+docutils==0.20.1
     # via readme-renderer
-fabric==2.5.0
+fabric==3.1.0
     # via -r requirements.in
-gitdb==4.0.9
+gitdb==4.0.10
     # via
     #   gitpython
     #   vcsinfo
-gitpython==3.1.18
-    # via
-    #   -r requirements.in
-    #   vcsinfo
+gitpython==3.1.31
+    # via vcsinfo
 graphlib-backport==1.0.3
     # via -r requirements.in
-idna==3.3
+idna==3.4
     # via requests
-importlib-metadata==4.8.3
-    # via keyring
-invoke==1.7.1
+importlib-metadata==6.6.0
+    # via
+    #   keyring
+    #   twine
+invoke==2.1.2
     # via fabric
-jinja2==2.11.2
+jaraco-classes==3.2.3
+    # via keyring
+jinja2==3.1.2
     # via -r requirements.in
-keyring==23.4.1
+keyring==23.13.1
     # via twine
-markupsafe==1.1.1
-    # via
-    #   -r requirements.in
-    #   jinja2
-packaging==21.3
-    # via bleach
-paramiko==2.10.3
+markdown-it-py==2.2.0
+    # via rich
+markupsafe==2.1.3
+    # via jinja2
+mdurl==0.1.2
+    # via markdown-it-py
+more-itertools==9.1.0
+    # via jaraco-classes
+packaging==23.1
+    # via docker
+paramiko==3.2.0
     # via
     #   -r requirements.in
     #   fabric
-pkginfo==1.8.3
+pkginfo==1.9.6
     # via twine
 pycparser==2.21
     # via cffi
-pygments==2.12.0
-    # via readme-renderer
+pygments==2.15.1
+    # via
+    #   readme-renderer
+    #   rich
 pynacl==1.5.0
     # via paramiko
-pyparsing==3.0.9
-    # via packaging
 pyyaml==6.0
     # via -r requirements.in
-readme-renderer==34.0
+readme-renderer==37.3
     # via twine
-requests==2.27.0
+requests==2.31.0
     # via
     #   -r requirements.in
     #   docker
     #   requests-toolbelt
     #   twine
-requests-toolbelt==0.9.1
+requests-toolbelt==1.0.0
+    # via twine
+rfc3986==2.0.0
     # via twine
-rfc3986==1.5.0
+rich==13.4.1
     # via twine
 six==1.16.0
-    # via
-    #   bcrypt
-    #   bleach
-    #   docker
-    #   paramiko
+    # via bleach
 smmap==5.0.0
     # via gitdb
 timeout-decorator==0.5.0
     # via -r requirements.in
-tqdm==4.64.0
-    # via twine
-twine==3.2.0
-    # via -r requirements.in
-typing-extensions==4.1.1
+twine==4.0.2
     # via -r requirements.in
-urllib3==1.26.9
-    # via requests
+urllib3==2.0.3
+    # via
+    #   docker
+    #   requests
+    #   twine
 vcsinfo==2.1.105
     # via -r requirements.in
 webencodings==0.5.1
     # via bleach
-websocket-client==1.3.1
+websocket-client==1.5.2
     # via docker
-zipp==3.6.0
+zipp==3.15.0
     # via importlib-metadata
-
-# The following packages are considered to be unsafe in a requirements file:
-# setuptools
```

### Comparing `buildrunner-2.0.751/setup.py` & `buildrunner-3.0.753/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import subprocess
 import sys
 import types
 
 from setuptools import setup, find_packages
 
 
-BASE_VERSION = '2.0'
+BASE_VERSION = '3.0'
 
 SOURCE_DIR = os.path.dirname(
     os.path.abspath(__file__)
 )
 BUILDRUNNER_DIR = os.path.join(SOURCE_DIR, 'buildrunner')
 VERSION_FILE = os.path.join(BUILDRUNNER_DIR, 'version.py')
```

### Comparing `buildrunner-2.0.751/test_requirements.txt` & `buildrunner-3.0.753/test_requirements.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,61 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile test_requirements.in
 #
-astroid==2.5.0
+astroid==2.15.5
     # via pylint
-attrs==21.4.0
-    # via pytest
-coverage==6.2
+coverage[toml]==7.2.7
     # via pytest-cov
-exceptiongroup==1.1.0
+dill==0.3.6
+    # via pylint
+exceptiongroup==1.1.1
     # via pytest
 execnet==1.9.0
     # via pytest-xdist
 graphlib-backport==1.0.3
     # via -r test_requirements.in
-iniconfig==1.1.1
+iniconfig==2.0.0
     # via pytest
-isort==5.10.1
+isort==5.12.0
     # via pylint
-lazy-object-proxy==1.7.1
+lazy-object-proxy==1.9.0
     # via astroid
-mccabe==0.6.1
+mccabe==0.7.0
     # via pylint
-packaging==21.3
+packaging==23.1
     # via pytest
-pluggy==0.13.1
+platformdirs==3.5.1
+    # via pylint
+pluggy==1.0.0
     # via pytest
-py==1.11.0
-    # via pytest-forked
 pycodestyle==2.10.0
     # via -r test_requirements.in
-pylint==2.7.1
+pylint==2.17.4
     # via -r test_requirements.in
-pylintfileheader==0.3.0
+pylintfileheader==0.3.2
     # via -r test_requirements.in
-pyparsing==3.0.9
-    # via packaging
-pytest==7.2.1
+pytest==7.3.1
     # via
     #   -r test_requirements.in
     #   pytest-cov
-    #   pytest-forked
     #   pytest-randomly
     #   pytest-xdist
-pytest-cov==2.10.1
+pytest-cov==4.1.0
     # via -r test_requirements.in
-pytest-forked==1.4.0
-    # via pytest-xdist
-pytest-randomly==3.5.0
+pytest-randomly==3.12.0
     # via -r test_requirements.in
-pytest-xdist==2.4.0
+pytest-xdist==3.3.1
     # via -r test_requirements.in
-toml==0.10.2
-    # via pylint
 tomli==2.0.1
-    # via pytest
-wrapt==1.12.1
+    # via
+    #   coverage
+    #   pylint
+    #   pytest
+tomlkit==0.11.8
+    # via pylint
+typing-extensions==4.6.3
+    # via astroid
+wrapt==1.15.0
     # via astroid
```

