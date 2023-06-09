# Comparing `tmp/promptx-0.0.6.tar.gz` & `tmp/promptx-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptx-0.0.6.tar", last modified: Mon Apr 17 02:28:30 2023, max compression
+gzip compressed data, was "promptx-0.0.7.tar", last modified: Fri Jun  9 01:06:12 2023, max compression
```

## Comparing `promptx-0.0.6.tar` & `promptx-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-17 02:28:30.159267 promptx-0.0.6/
--rw-r--r--   0 anon      (1000) wheel      (998)    34880 2022-09-15 20:58:55.000000 promptx-0.0.6/LICENSE.md
--rw-r--r--   0 anon      (1000) wheel      (998)     2839 2023-04-17 02:28:30.159267 promptx-0.0.6/PKG-INFO
--rw-r--r--   0 anon      (1000) wheel      (998)     2526 2022-09-21 20:19:44.000000 promptx-0.0.6/README.md
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-17 02:28:30.159267 promptx-0.0.6/promptx/
--rw-r--r--   0 anon      (1000) wheel      (998)      145 2022-09-15 21:02:32.000000 promptx-0.0.6/promptx/__init__.py
--rw-r--r--   0 anon      (1000) wheel      (998)     5090 2023-04-17 02:26:29.000000 promptx-0.0.6/promptx/promptx.py
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-17 02:28:30.159267 promptx-0.0.6/promptx.egg-info/
--rw-r--r--   0 anon      (1000) wheel      (998)     2839 2023-04-17 02:28:30.000000 promptx-0.0.6/promptx.egg-info/PKG-INFO
--rw-r--r--   0 anon      (1000) wheel      (998)      198 2023-04-17 02:28:30.000000 promptx-0.0.6/promptx.egg-info/SOURCES.txt
--rw-r--r--   0 anon      (1000) wheel      (998)        1 2023-04-17 02:28:30.000000 promptx-0.0.6/promptx.egg-info/dependency_links.txt
--rw-r--r--   0 anon      (1000) wheel      (998)        8 2023-04-17 02:28:30.000000 promptx-0.0.6/promptx.egg-info/top_level.txt
--rw-r--r--   0 anon      (1000) wheel      (998)      463 2023-04-17 02:26:45.000000 promptx-0.0.6/pyproject.toml
--rw-r--r--   0 anon      (1000) wheel      (998)       38 2023-04-17 02:28:30.159267 promptx-0.0.6/setup.cfg
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-06-09 01:06:12.365372 promptx-0.0.7/
+-rw-r--r--   0 anon      (1000) wheel      (998)    34880 2022-09-15 20:58:55.000000 promptx-0.0.7/LICENSE.md
+-rw-r--r--   0 anon      (1000) wheel      (998)     2839 2023-06-09 01:06:12.365372 promptx-0.0.7/PKG-INFO
+-rw-r--r--   0 anon      (1000) wheel      (998)     2526 2022-09-21 20:19:44.000000 promptx-0.0.7/README.md
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-06-09 01:06:12.365372 promptx-0.0.7/promptx/
+-rw-r--r--   0 anon      (1000) wheel      (998)      145 2022-09-15 21:02:32.000000 promptx-0.0.7/promptx/__init__.py
+-rw-r--r--   0 anon      (1000) wheel      (998)     5100 2023-06-09 01:03:01.000000 promptx-0.0.7/promptx/promptx.py
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-06-09 01:06:12.365372 promptx-0.0.7/promptx.egg-info/
+-rw-r--r--   0 anon      (1000) wheel      (998)     2839 2023-06-09 01:06:12.000000 promptx-0.0.7/promptx.egg-info/PKG-INFO
+-rw-r--r--   0 anon      (1000) wheel      (998)      198 2023-06-09 01:06:12.000000 promptx-0.0.7/promptx.egg-info/SOURCES.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)        1 2023-06-09 01:06:12.000000 promptx-0.0.7/promptx.egg-info/dependency_links.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)        8 2023-06-09 01:06:12.000000 promptx-0.0.7/promptx.egg-info/top_level.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)      463 2023-06-09 01:05:06.000000 promptx-0.0.7/pyproject.toml
+-rw-r--r--   0 anon      (1000) wheel      (998)       38 2023-06-09 01:06:12.365372 promptx-0.0.7/setup.cfg
```

### Comparing `promptx-0.0.6/LICENSE.md` & `promptx-0.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `promptx-0.0.6/PKG-INFO` & `promptx-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptx
-Version: 0.0.6
+Version: 0.0.7
 Summary: Flexible prompt wrapper for dmenu, fzf, and rofi.
 License: GNU General Public License v3 (GPLv3)
 Project-URL: repository, https://codeberg.org/johndovern/promptx
 Keywords: dmenu,fzf,rofi
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `promptx-0.0.6/README.md` & `promptx-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `promptx-0.0.6/promptx/promptx.py` & `promptx-0.0.7/promptx/promptx.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,45 +86,45 @@
         if prompt_cmd == "rofi":
             default_args = " ".join((default_args, "-dmenu"))
         self.prompt_cmd = prompt_cmd
         self.default_args = default_args
         # Create a basic list of command args
         self.base_cmd = shlex.split(" ".join((prompt_cmd, default_args)))
         self.temp_args = []
+        # fzf uses stderr to show prompt so we need to check for that
+        self.stderr_file = None if self.prompt_cmd == "fzf" else subprocess.PIPE
 
     def ask(
         self,
         options: List,
         prompt: str | None = None,
         additional_args: str | None = None,
         deliminator: str = "\n",
     ) -> List[str]:
         """
         Ask the user to make a selection from the given options
         """
         cmd = []
         cmd.extend(self.base_cmd)
         cmd.extend(self.temp_args)
-        # fzf uses stderr to show prompt so we need to check for that
-        stderr_file = None if self.prompt_cmd == "fzf" else subprocess.PIPE
         if additional_args is not None:
             cmd.extend(shlex.split(additional_args))
         if self.prompt_cmd == "fzf" and prompt is not None:
             cmd.append(f"--prompt={prompt}")
         elif prompt is not None:
             cmd.extend(["-p", prompt])
 
         # Start prompt_cmd with given args
         try:
             proc = subprocess.Popen(
                 cmd,
                 universal_newlines=True,
                 stdin=subprocess.PIPE,
                 stdout=subprocess.PIPE,
-                stderr=stderr_file,
+                stderr=self.stderr_file,
             )
         # Failed to execute constructed command
         except OSError as err:
             raise PromptXError(cmd=cmd, err=err)
 
         # Reset temp_args
         self.temp_args = []
```

### Comparing `promptx-0.0.6/promptx.egg-info/PKG-INFO` & `promptx-0.0.7/promptx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptx
-Version: 0.0.6
+Version: 0.0.7
 Summary: Flexible prompt wrapper for dmenu, fzf, and rofi.
 License: GNU General Public License v3 (GPLv3)
 Project-URL: repository, https://codeberg.org/johndovern/promptx
 Keywords: dmenu,fzf,rofi
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

