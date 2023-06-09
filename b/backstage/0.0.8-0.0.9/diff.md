# Comparing `tmp/backstage-0.0.8.tar.gz` & `tmp/backstage-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/backstage-0.0.8.tar", last modified: Tue Jan 18 23:06:07 2022, max compression
+gzip compressed data, was "dist/backstage-0.0.9.tar", last modified: Mon Mar 21 20:23:55 2022, max compression
```

## Comparing `backstage-0.0.8.tar` & `backstage-0.0.9.tar`

### file list

```diff
@@ -1,62 +1,26 @@
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2022-01-18 23:06:07.711961 backstage-0.0.8/
--rw-rw-r--   0 alex      (1002) alex      (1003)     1082 2022-01-16 17:32:01.000000 backstage-0.0.8/LICENSE
--rw-rw-r--   0 alex      (1002) alex      (1003)       71 2021-08-19 18:50:13.000000 backstage-0.0.8/MANIFEST.in
--rw-rw-r--   0 alex      (1002) alex      (1003)     6372 2022-01-18 23:06:07.711961 backstage-0.0.8/PKG-INFO
--rw-rw-r--   0 alex      (1002) alex      (1003)     5678 2022-01-18 22:10:22.000000 backstage-0.0.8/README.md
--rw-rw-r--   0 alex      (1002) alex      (1003)        5 2022-01-18 23:01:17.000000 backstage-0.0.8/VERSION
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2022-01-18 23:06:07.695961 backstage-0.0.8/backstage/
--rw-rw-r--   0 alex      (1002) alex      (1003)      888 2022-01-17 12:17:43.000000 backstage-0.0.8/backstage/__init__.py
--rw-rw-r--   0 alex      (1002) alex      (1003)      947 2022-01-16 14:47:32.000000 backstage-0.0.8/backstage/__main__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2022-01-18 23:06:07.703961 backstage-0.0.8/backstage/core/
--rw-rw-r--   0 alex      (1002) alex      (1003)        0 2021-10-04 09:36:29.000000 backstage-0.0.8/backstage/core/__init__.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     1818 2022-01-15 10:57:07.000000 backstage-0.0.8/backstage/core/backstage_setup.py
--rw-r-----   0 alex      (1002) alex      (1003)      199 2022-01-13 21:54:07.000000 backstage-0.0.8/backstage/core/constant.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     1573 2021-10-09 09:07:00.000000 backstage-0.0.8/backstage/core/dist.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     5656 2022-01-18 23:05:18.000000 backstage-0.0.8/backstage/core/funcs.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     1918 2022-01-16 18:22:32.000000 backstage-0.0.8/backstage/core/initialization.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     2908 2021-10-04 12:13:20.000000 backstage-0.0.8/backstage/core/lite_test_runner.py
--rw-rw-rw-   0 alex      (1002) alex      (1003)     4406 2022-01-16 18:22:32.000000 backstage-0.0.8/backstage/core/pymisc.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     1599 2022-01-15 11:30:15.000000 backstage-0.0.8/backstage/core/tasks.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     2620 2022-01-16 16:51:43.000000 backstage-0.0.8/backstage/core/versioning.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2022-01-18 23:06:07.703961 backstage-0.0.8/backstage/error/
--rw-rw-r--   0 alex      (1002) alex      (1003)       75 2022-01-13 21:54:07.000000 backstage-0.0.8/backstage/error/__init__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2022-01-18 23:06:07.707961 backstage-0.0.8/backstage/script/
--rw-rw-r--   0 alex      (1002) alex      (1003)        0 2021-08-21 22:44:47.000000 backstage-0.0.8/backstage/script/__init__.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     2737 2022-01-16 18:22:32.000000 backstage-0.0.8/backstage/script/build.py
--rw-rw-r--   0 alex      (1002) alex      (1003)      358 2022-01-16 19:29:22.000000 backstage-0.0.8/backstage/script/gitcommit.py
--rw-rw-r--   0 alex      (1002) alex      (1003)      375 2022-01-16 17:12:53.000000 backstage-0.0.8/backstage/script/gitinit.py
--rw-rw-r--   0 alex      (1002) alex      (1003)      188 2022-01-16 19:29:22.000000 backstage-0.0.8/backstage/script/gitpush.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     4233 2022-01-16 18:22:32.000000 backstage-0.0.8/backstage/script/init.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     1561 2022-01-16 19:52:21.000000 backstage-0.0.8/backstage/script/release.py
--rw-rw-r--   0 alex      (1002) alex      (1003)      284 2022-01-16 12:33:48.000000 backstage-0.0.8/backstage/script/run.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     1095 2022-01-16 18:22:32.000000 backstage-0.0.8/backstage/script/version.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2022-01-18 23:06:07.707961 backstage-0.0.8/backstage/template/
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2022-01-18 23:06:07.711961 backstage-0.0.8/backstage/template/app/
--rw-rw-r--   0 alex      (1002) alex      (1003)        0 2021-05-09 11:57:49.000000 backstage-0.0.8/backstage/template/app/changelog_template.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)      204 2022-01-16 18:22:31.000000 backstage-0.0.8/backstage/template/app/gitignore_template.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)        0 2021-05-09 11:52:27.000000 backstage-0.0.8/backstage/template/app/latest_release_template.txt
--rw-r-----   0 alex      (1002) alex      (1003)      121 2022-01-16 12:23:47.000000 backstage-0.0.8/backstage/template/app/main_template.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)       71 2021-05-28 19:07:49.000000 backstage-0.0.8/backstage/template/app/manifest_template.txt
--rw-r-----   0 alex      (1002) alex      (1003)      109 2021-06-21 08:20:32.000000 backstage-0.0.8/backstage/template/app/module_template.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)      100 2021-02-10 19:28:44.000000 backstage-0.0.8/backstage/template/app/pyproject_template.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)      101 2022-01-04 10:46:56.000000 backstage-0.0.8/backstage/template/app/readme_template.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)      712 2022-01-04 10:39:18.000000 backstage-0.0.8/backstage/template/app/setup_cfg_template.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)       70 2021-02-10 19:28:43.000000 backstage-0.0.8/backstage/template/app/setup_py_template.txt
--rw-r-----   0 alex      (1002) alex      (1003)      385 2022-01-04 10:42:50.000000 backstage-0.0.8/backstage/template/app/test_template.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)      360 2022-01-04 10:42:50.000000 backstage-0.0.8/backstage/template/app/tests_main_template.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)        5 2021-05-28 22:01:25.000000 backstage-0.0.8/backstage/template/app/version_template.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)      406 2022-01-16 12:21:57.000000 backstage-0.0.8/backstage/template/tasks.txt
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2022-01-18 23:06:07.699961 backstage-0.0.8/backstage.egg-info/
--rw-rw-r--   0 alex      (1002) alex      (1003)     6372 2022-01-18 23:06:07.000000 backstage-0.0.8/backstage.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1002) alex      (1003)     1551 2022-01-18 23:06:07.000000 backstage-0.0.8/backstage.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)        1 2022-01-18 23:06:07.000000 backstage-0.0.8/backstage.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)       55 2022-01-18 23:06:07.000000 backstage-0.0.8/backstage.egg-info/entry_points.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)        1 2021-08-19 18:50:24.000000 backstage-0.0.8/backstage.egg-info/not-zip-safe
--rw-rw-r--   0 alex      (1002) alex      (1003)       77 2022-01-18 23:06:07.000000 backstage-0.0.8/backstage.egg-info/requires.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)       16 2022-01-18 23:06:07.000000 backstage-0.0.8/backstage.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)      100 2021-04-04 13:48:05.000000 backstage-0.0.8/pyproject.toml
--rw-rw-r--   0 alex      (1002) alex      (1003)      983 2022-01-18 23:06:07.715961 backstage-0.0.8/setup.cfg
--rw-rw-r--   0 alex      (1002) alex      (1003)       70 2021-04-04 13:49:01.000000 backstage-0.0.8/setup.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2022-01-18 23:06:07.711961 backstage-0.0.8/tests/
--rw-rw-r--   0 alex      (1002) alex      (1003)        0 2021-09-01 21:07:34.000000 backstage-0.0.8/tests/__init__.py
--rw-rw-r--   0 alex      (1002) alex      (1003)      365 2021-11-16 18:50:32.000000 backstage-0.0.8/tests/__main__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2022-03-21 20:23:55.665015 backstage-0.0.9/
+-rw-rw-r--   0 alex      (1002) alex      (1003)     1082 2022-01-16 17:32:01.000000 backstage-0.0.9/LICENSE
+-rw-rw-r--   0 alex      (1002) alex      (1003)       71 2021-08-19 18:50:13.000000 backstage-0.0.9/MANIFEST.in
+-rw-rw-r--   0 alex      (1002) alex      (1003)     9164 2022-03-21 20:23:55.665015 backstage-0.0.9/PKG-INFO
+-rw-rw-r--   0 alex      (1002) alex      (1003)     8441 2022-03-18 21:28:26.000000 backstage-0.0.9/README.md
+-rw-rw-r--   0 alex      (1002) alex      (1003)        5 2022-01-18 23:06:09.000000 backstage-0.0.9/VERSION
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2022-03-21 20:23:55.653020 backstage-0.0.9/backstage/
+-rw-rw-r--   0 alex      (1002) alex      (1003)     3123 2022-03-16 17:49:22.000000 backstage-0.0.9/backstage/__init__.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     1843 2022-03-16 13:24:43.000000 backstage-0.0.9/backstage/__main__.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     1057 2022-03-16 17:47:13.000000 backstage-0.0.9/backstage/default_tasks
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2022-03-21 20:23:55.653020 backstage-0.0.9/backstage/error/
+-rw-rw-r--   0 alex      (1002) alex      (1003)       97 2022-03-14 13:30:18.000000 backstage-0.0.9/backstage/error/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2022-03-21 20:23:55.653020 backstage-0.0.9/backstage.egg-info/
+-rw-rw-r--   0 alex      (1002) alex      (1003)     9164 2022-03-21 20:23:55.000000 backstage-0.0.9/backstage.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1002) alex      (1003)      435 2022-03-21 20:23:55.000000 backstage-0.0.9/backstage.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)        1 2022-03-21 20:23:55.000000 backstage-0.0.9/backstage.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)       55 2022-03-21 20:23:55.000000 backstage-0.0.9/backstage.egg-info/entry_points.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)        1 2021-08-19 18:50:24.000000 backstage-0.0.9/backstage.egg-info/not-zip-safe
+-rw-rw-r--   0 alex      (1002) alex      (1003)       37 2022-03-21 20:23:55.000000 backstage-0.0.9/backstage.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)       16 2022-03-21 20:23:55.000000 backstage-0.0.9/backstage.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)      100 2021-04-04 13:48:05.000000 backstage-0.0.9/pyproject.toml
+-rw-rw-r--   0 alex      (1002) alex      (1003)      978 2022-03-21 20:23:55.665015 backstage-0.0.9/setup.cfg
+-rw-rw-r--   0 alex      (1002) alex      (1003)       70 2021-04-04 13:49:01.000000 backstage-0.0.9/setup.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2022-03-21 20:23:55.657018 backstage-0.0.9/tests/
+-rw-rw-r--   0 alex      (1002) alex      (1003)        0 2021-09-01 21:07:34.000000 backstage-0.0.9/tests/__init__.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)      365 2021-11-16 18:50:32.000000 backstage-0.0.9/tests/__main__.py
```

### Comparing `backstage-0.0.8/LICENSE` & `backstage-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `backstage-0.0.8/backstage/core/tasks.py` & `backstage-0.0.9/backstage/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,55 +1,72 @@
 import os
 import os.path
-import shlex
-import subrun
+import sys
 import backstage
-from backstage import constant
+from backstage import error
 
+__all__ = []
 
-def run(*commands, extra_args=None, project_dir=None):
-    for i, command in enumerate(commands):
-        if i == 0:
-            command = _join_command(command, extra_args)
-        info = subrun.run(command, cwd=project_dir)
-        if not info.success:
-            break
-
-
-def get_tasks(project_dir=None):
-    if not project_dir:
-        project_dir = os.getcwd()
-    filename = os.path.join(project_dir, "backstage.tasks")
-    if not os.path.isfile(filename):
-        filename = os.path.join(constant.BACKSTAGE_HOME, "backstage.tasks")
-    if not os.path.isfile(filename):
-        raise backstage.NoTasksFileError
-    return _parse_tasks_file(filename)
-
-
-def _parse_tasks_file(path):
-    tasks = dict()
-    with open(path, "r") as file:
-        raw = file.read()
-    lines = raw.splitlines()
-    current_task = None
-    for line in lines:
-        if not line or line.isspace():
-            continue
-        if line.startswith("[") and line.endswith("]"):
-            current_task = line.lstrip("[").rstrip("]")
-            tasks[current_task] = list()
-            continue
-        if current_task:
-            tasks[current_task].append(line)
-    return tasks
-
-
-def _join_command(command, extra_args):
-    if not extra_args:
-        return command
+
+def main():
+    project_dir = os.getcwd()
+    args = sys.argv[1:]
+    tasks = None
     try:
-        extra_args = " ".join(shlex.quote(item) for item in extra_args)
-    except Exception as e:
-        msg = "Failed to join the extra_args"
-        raise backstage.Error(msg) from None
-    return "{} {}".format(command, extra_args)
+        tasks = backstage.get_tasks(project_dir)
+    except error.NoTasksFileError:
+        pass
+    if not args:
+        help_handler()
+        if tasks:
+            show_available_tasks(tasks)
+        else:
+            if ask_for_default_tasks_creation():
+                create_default_tasks_file(project_dir)
+        return
+    task = args[0]
+    if tasks:
+        if task in tasks:
+            backstage.run(*tasks[task], extra_args=args[1:])
+        else:
+            print("This task doesn't exist\n")
+            show_available_tasks(tasks)
+    else:
+        help_handler()
+        if ask_for_default_tasks_creation():
+            create_default_tasks_file(project_dir)
+
+
+def help_handler():
+    """Help me !"""
+    intro = ("Project Backstage\n",
+             "https://github.com/pyrustic/backstage\n")
+    print("".join(intro))
+
+
+def show_available_tasks(tasks):
+    print("Available Tasks")
+    print("===============\n")
+    print("  ".join(tasks.keys()))
+    print()
+
+
+def ask_for_default_tasks_creation():
+    print("Missing 'backstage.tasks' file in the project root.")
+    print("A default 'backstage.tasks' can be generated !")
+    answer = input("Generate ? (y/N): ")
+    if answer.lower() == "y":
+        return True
+    return False
+
+
+def create_default_tasks_file(project_dir):
+    default_tasks = backstage.get_default_tasks()
+    if backstage.create_tasks_file(default_tasks, project_dir=project_dir, override=True):
+        print("\nSuccessfully generated a default tasks file !\n")
+        tasks = backstage.get_tasks(project_dir)
+        if tasks:
+            show_available_tasks(tasks)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `backstage-0.0.8/setup.cfg` & `backstage-0.0.9/setup.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -2,44 +2,48 @@
 name = backstage
 version = file: VERSION
 url = https://github.com/pyrustic/backstage
 author = Pyrustic Evangelist
 author_email = rusticalex@yahoo.com
 maintainer = Pyrustic Evangelist
 maintainer_email = rusticalex@yahoo.com
-description = Intuitive and extensible command line tool for managing software projects
+description = Extensible command line tool for managing software projects
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 keywords = 
 	project-manager
 	manager
 	packaging
 	release
 	build
 	project-init
 	lightweight
 	pyrustic
 	tool
+	CLI
+	setup
+	versioning
+	git
+	language-agnostic
 	productivity
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 python_requires = >=3.5
 packages = find:
 include_package_data = true
 zip_safe = false
 install_requires = 
-	setuptools
-	wheel
-	importlib-metadata ; python_version < "3.8"
-	shared
+	buildver
+	hackernote
+	setupinit
 	subrun
 
 [options.entry_points]
 console_scripts = 
 	backstage = backstage.__main__:main
 
 [egg_info]
```

