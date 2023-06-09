# Comparing `tmp/odoo_filter_addons-1.2.0.tar.gz` & `tmp/odoo_filter_addons-1.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo_filter_addons-1.2.0.tar", last modified: Fri Jun  9 12:19:34 2023, max compression
+gzip compressed data, was "odoo_filter_addons-1.2.0rc1.tar", last modified: Fri Jun  9 08:43:08 2023, max compression
```

## Comparing `odoo_filter_addons-1.2.0.tar` & `odoo_filter_addons-1.2.0rc1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:19:34.505438 odoo_filter_addons-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-09 12:19:34.505438 odoo_filter_addons-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-09 12:19:16.000000 odoo_filter_addons-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:19:34.501438 odoo_filter_addons-1.2.0/odoo_filter_addons/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-09 12:19:16.000000 odoo_filter_addons-1.2.0/odoo_filter_addons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8550 2023-06-09 12:19:16.000000 odoo_filter_addons-1.2.0/odoo_filter_addons/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-09 12:19:16.000000 odoo_filter_addons-1.2.0/odoo_filter_addons/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:19:34.505438 odoo_filter_addons-1.2.0/odoo_filter_addons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-09 12:19:34.000000 odoo_filter_addons-1.2.0/odoo_filter_addons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-09 12:19:34.000000 odoo_filter_addons-1.2.0/odoo_filter_addons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 12:19:34.000000 odoo_filter_addons-1.2.0/odoo_filter_addons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-09 12:19:34.000000 odoo_filter_addons-1.2.0/odoo_filter_addons.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-09 12:19:34.000000 odoo_filter_addons-1.2.0/odoo_filter_addons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-09 12:19:34.000000 odoo_filter_addons-1.2.0/odoo_filter_addons.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-09 12:19:16.000000 odoo_filter_addons-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 12:19:34.505438 odoo_filter_addons-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-09 12:19:16.000000 odoo_filter_addons-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:43:08.847087 odoo_filter_addons-1.2.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-06-09 08:43:08.847087 odoo_filter_addons-1.2.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-09 08:42:56.000000 odoo_filter_addons-1.2.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:43:08.847087 odoo_filter_addons-1.2.0rc1/odoo_filter_addons/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-09 08:42:56.000000 odoo_filter_addons-1.2.0rc1/odoo_filter_addons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-06-09 08:42:56.000000 odoo_filter_addons-1.2.0rc1/odoo_filter_addons/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-09 08:42:56.000000 odoo_filter_addons-1.2.0rc1/odoo_filter_addons/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:43:08.847087 odoo_filter_addons-1.2.0rc1/odoo_filter_addons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-06-09 08:43:08.000000 odoo_filter_addons-1.2.0rc1/odoo_filter_addons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-09 08:43:08.000000 odoo_filter_addons-1.2.0rc1/odoo_filter_addons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 08:43:08.000000 odoo_filter_addons-1.2.0rc1/odoo_filter_addons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-09 08:43:08.000000 odoo_filter_addons-1.2.0rc1/odoo_filter_addons.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-09 08:43:08.000000 odoo_filter_addons-1.2.0rc1/odoo_filter_addons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-09 08:43:08.000000 odoo_filter_addons-1.2.0rc1/odoo_filter_addons.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-09 08:42:56.000000 odoo_filter_addons-1.2.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 08:43:08.847087 odoo_filter_addons-1.2.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-09 08:42:56.000000 odoo_filter_addons-1.2.0rc1/setup.py
```

### Comparing `odoo_filter_addons-1.2.0/PKG-INFO` & `odoo_filter_addons-1.2.0rc1/odoo_filter_addons.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: odoo_filter_addons
-Version: 1.2.0
+Name: odoo-filter-addons
+Version: 1.2.0rc1
 Summary: Simple utlity to filter odoo addons into a single directory
 Author-email: Pablo Esteban <pablo.esteban@forgeflow.com>
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: Operating System :: POSIX
 Classifier: Framework :: Odoo
 Classifier: Programming Language :: Python :: 3
```

### Comparing `odoo_filter_addons-1.2.0/README.md` & `odoo_filter_addons-1.2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `odoo_filter_addons-1.2.0/odoo_filter_addons/main.py` & `odoo_filter_addons-1.2.0rc1/odoo_filter_addons/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,16 +97,15 @@
         if not repo:
             raise UserException("addons.yml entry {} not found in repos.yml".format(rname))
         repo_message = filter_repo(tmp_path, rname, repo, modules)
         messages.append(repo_message)
     print_header("Finished filtering", '*')
     # Commit changes, if any, and push them to remote if specified
     if not release:
-        git("restore", "--staged", ".")
-        print("Release disabled, nothing commited")
+        print("No changes, nothing commited")
     elif filter(None, messages) and git["diff", "--staged", "--quiet"] & TF(1):
         messages = [f"[AUTO] {__package__} {__version__}"] + messages
         message = "\n".join(messages)
         git("commit", "-m", message)
         print("Changes commited")
         if push:
             if git["rev-parse", "@{u}"] & TF:
```

### Comparing `odoo_filter_addons-1.2.0/odoo_filter_addons.egg-info/PKG-INFO` & `odoo_filter_addons-1.2.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: odoo-filter-addons
-Version: 1.2.0
+Name: odoo_filter_addons
+Version: 1.2.0rc1
 Summary: Simple utlity to filter odoo addons into a single directory
 Author-email: Pablo Esteban <pablo.esteban@forgeflow.com>
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: Operating System :: POSIX
 Classifier: Framework :: Odoo
 Classifier: Programming Language :: Python :: 3
```

### Comparing `odoo_filter_addons-1.2.0/pyproject.toml` & `odoo_filter_addons-1.2.0rc1/pyproject.toml`

 * *Files identical despite different names*

