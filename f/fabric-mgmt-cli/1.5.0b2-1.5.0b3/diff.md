# Comparing `tmp/fabric-mgmt-cli-1.5.0b2.tar.gz` & `tmp/fabric-mgmt-cli-1.5.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric-mgmt-cli-1.5.0b2.tar", last modified: Fri Jun  9 20:59:43 2023, max compression
+gzip compressed data, was "fabric-mgmt-cli-1.5.0b3.tar", last modified: Fri Jun  9 21:01:40 2023, max compression
```

## Comparing `fabric-mgmt-cli-1.5.0b2.tar` & `fabric-mgmt-cli-1.5.0b3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1806 2023-06-09 20:57:01.647957 fabric-mgmt-cli-1.5.0b2/.gitignore
--rw-r--r--   0        0        0     1071 2022-10-13 16:37:50.489741 fabric-mgmt-cli-1.5.0b2/LICENSE
--rw-r--r--   0        0        0     9452 2023-01-19 19:01:44.980822 fabric-mgmt-cli-1.5.0b2/README.md
--rw-r--r--   0        0        0     2046 2022-10-13 16:37:50.490228 fabric-mgmt-cli-1.5.0b2/config.yml
--rw-r--r--   0        0        0       51 2023-06-09 20:59:42.229416 fabric-mgmt-cli-1.5.0b2/fabric_mgmt_cli/__init__.py
--rw-r--r--   0        0        0        0 2022-10-13 16:37:50.490498 fabric-mgmt-cli-1.5.0b2/fabric_mgmt_cli/managecli/__init__.py
--rw-r--r--   0        0        0     2002 2022-10-13 16:37:50.490695 fabric-mgmt-cli-1.5.0b2/fabric_mgmt_cli/managecli/command.py
--rw-r--r--   0        0        0     9832 2022-10-13 16:37:50.490796 fabric-mgmt-cli-1.5.0b2/fabric_mgmt_cli/managecli/config_processor.py
--rw-r--r--   0        0        0     7461 2022-10-13 16:37:50.490934 fabric-mgmt-cli-1.5.0b2/fabric_mgmt_cli/managecli/configuration.py
--rw-r--r--   0        0        0     9957 2023-01-19 18:49:45.717500 fabric-mgmt-cli-1.5.0b2/fabric_mgmt_cli/managecli/kafka_processor.py
--rw-r--r--   0        0        0    45398 2023-05-22 15:02:49.188025 fabric-mgmt-cli-1.5.0b2/fabric_mgmt_cli/managecli/manage_command.py
--rw-r--r--   0        0        0    27720 2023-05-17 03:26:00.969252 fabric-mgmt-cli-1.5.0b2/fabric_mgmt_cli/managecli/managecli.py
--rw-r--r--   0        0        0        0 2022-10-13 16:37:50.491613 fabric-mgmt-cli-1.5.0b2/fabric_mgmt_cli/managecli/net/__init__.py
--rw-r--r--   0        0        0     8830 2022-10-13 16:37:50.491743 fabric-mgmt-cli-1.5.0b2/fabric_mgmt_cli/managecli/net/commands.py
--rw-r--r--   0        0        0     3657 2022-10-13 16:37:50.491891 fabric-mgmt-cli-1.5.0b2/fabric_mgmt_cli/managecli/net/nso.py
--rw-r--r--   0        0        0     1072 2022-10-13 16:37:50.492004 fabric-mgmt-cli-1.5.0b2/fabric_mgmt_cli/managecli/net/resources.py
--rw-r--r--   0        0        0     6728 2023-05-09 13:25:27.691022 fabric-mgmt-cli-1.5.0b2/fabric_mgmt_cli/managecli/net/services.py
--rw-r--r--   0        0        0      535 2022-10-13 16:37:50.492246 fabric-mgmt-cli-1.5.0b2/fabric_mgmt_cli/managecli/net/util.py
--rw-r--r--   0        0        0    19237 2023-06-04 20:42:05.646655 fabric-mgmt-cli-1.5.0b2/fabric_mgmt_cli/managecli/show_command.py
--rw-r--r--   0        0        0        0 2022-10-13 16:37:50.492509 fabric-mgmt-cli-1.5.0b2/fabric_mgmt_cli/managecli/test/__init__.py
--rw-r--r--   0        0        0     1828 2022-10-13 16:37:50.492603 fabric-mgmt-cli-1.5.0b2/fabric_mgmt_cli/managecli/test/config.yml
--rw-r--r--   0        0        0     8401 2022-10-13 16:37:50.492732 fabric-mgmt-cli-1.5.0b2/fabric_mgmt_cli/managecli/test/test_managecli.py
--rw-r--r--   0        0        0      983 2022-10-13 16:37:50.492848 fabric-mgmt-cli-1.5.0b2/net_inventory.yml
--rw-r--r--   0        0        0     1068 2023-06-09 20:59:13.897133 fabric-mgmt-cli-1.5.0b2/pyproject.toml
--rw-r--r--   0        0        0    10352 1970-01-01 00:00:00.000000 fabric-mgmt-cli-1.5.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1806 2023-06-09 20:57:01.647957 fabric-mgmt-cli-1.5.0b3/.gitignore
+-rw-r--r--   0        0        0     1071 2022-10-13 16:37:50.489741 fabric-mgmt-cli-1.5.0b3/LICENSE
+-rw-r--r--   0        0        0     9452 2023-01-19 19:01:44.980822 fabric-mgmt-cli-1.5.0b3/README.md
+-rw-r--r--   0        0        0     2046 2022-10-13 16:37:50.490228 fabric-mgmt-cli-1.5.0b3/config.yml
+-rw-r--r--   0        0        0       51 2023-06-09 21:01:38.487105 fabric-mgmt-cli-1.5.0b3/fabric_mgmt_cli/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-13 16:37:50.490498 fabric-mgmt-cli-1.5.0b3/fabric_mgmt_cli/managecli/__init__.py
+-rw-r--r--   0        0        0     2002 2022-10-13 16:37:50.490695 fabric-mgmt-cli-1.5.0b3/fabric_mgmt_cli/managecli/command.py
+-rw-r--r--   0        0        0     9832 2022-10-13 16:37:50.490796 fabric-mgmt-cli-1.5.0b3/fabric_mgmt_cli/managecli/config_processor.py
+-rw-r--r--   0        0        0     7461 2022-10-13 16:37:50.490934 fabric-mgmt-cli-1.5.0b3/fabric_mgmt_cli/managecli/configuration.py
+-rw-r--r--   0        0        0     9957 2023-01-19 18:49:45.717500 fabric-mgmt-cli-1.5.0b3/fabric_mgmt_cli/managecli/kafka_processor.py
+-rw-r--r--   0        0        0    45398 2023-05-22 15:02:49.188025 fabric-mgmt-cli-1.5.0b3/fabric_mgmt_cli/managecli/manage_command.py
+-rw-r--r--   0        0        0    27720 2023-05-17 03:26:00.969252 fabric-mgmt-cli-1.5.0b3/fabric_mgmt_cli/managecli/managecli.py
+-rw-r--r--   0        0        0        0 2022-10-13 16:37:50.491613 fabric-mgmt-cli-1.5.0b3/fabric_mgmt_cli/managecli/net/__init__.py
+-rw-r--r--   0        0        0     8830 2022-10-13 16:37:50.491743 fabric-mgmt-cli-1.5.0b3/fabric_mgmt_cli/managecli/net/commands.py
+-rw-r--r--   0        0        0     3657 2022-10-13 16:37:50.491891 fabric-mgmt-cli-1.5.0b3/fabric_mgmt_cli/managecli/net/nso.py
+-rw-r--r--   0        0        0     1072 2022-10-13 16:37:50.492004 fabric-mgmt-cli-1.5.0b3/fabric_mgmt_cli/managecli/net/resources.py
+-rw-r--r--   0        0        0     6728 2023-05-09 13:25:27.691022 fabric-mgmt-cli-1.5.0b3/fabric_mgmt_cli/managecli/net/services.py
+-rw-r--r--   0        0        0      535 2022-10-13 16:37:50.492246 fabric-mgmt-cli-1.5.0b3/fabric_mgmt_cli/managecli/net/util.py
+-rw-r--r--   0        0        0    19237 2023-06-04 20:42:05.646655 fabric-mgmt-cli-1.5.0b3/fabric_mgmt_cli/managecli/show_command.py
+-rw-r--r--   0        0        0        0 2022-10-13 16:37:50.492509 fabric-mgmt-cli-1.5.0b3/fabric_mgmt_cli/managecli/test/__init__.py
+-rw-r--r--   0        0        0     1828 2022-10-13 16:37:50.492603 fabric-mgmt-cli-1.5.0b3/fabric_mgmt_cli/managecli/test/config.yml
+-rw-r--r--   0        0        0     8401 2022-10-13 16:37:50.492732 fabric-mgmt-cli-1.5.0b3/fabric_mgmt_cli/managecli/test/test_managecli.py
+-rw-r--r--   0        0        0      983 2022-10-13 16:37:50.492848 fabric-mgmt-cli-1.5.0b3/net_inventory.yml
+-rw-r--r--   0        0        0     1070 2023-06-09 21:01:32.437234 fabric-mgmt-cli-1.5.0b3/pyproject.toml
+-rw-r--r--   0        0        0    10354 1970-01-01 00:00:00.000000 fabric-mgmt-cli-1.5.0b3/PKG-INFO
```

### Comparing `fabric-mgmt-cli-1.5.0b2/.gitignore` & `fabric-mgmt-cli-1.5.0b3/.gitignore`

 * *Files identical despite different names*

### Comparing `fabric-mgmt-cli-1.5.0b2/LICENSE` & `fabric-mgmt-cli-1.5.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric-mgmt-cli-1.5.0b2/README.md` & `fabric-mgmt-cli-1.5.0b3/README.md`

 * *Files identical despite different names*

### Comparing `fabric-mgmt-cli-1.5.0b2/config.yml` & `fabric-mgmt-cli-1.5.0b3/config.yml`

 * *Files identical despite different names*

### Comparing `fabric-mgmt-cli-1.5.0b2/fabric_mgmt_cli/managecli/command.py` & `fabric-mgmt-cli-1.5.0b3/fabric_mgmt_cli/managecli/command.py`

 * *Files identical despite different names*

### Comparing `fabric-mgmt-cli-1.5.0b2/fabric_mgmt_cli/managecli/config_processor.py` & `fabric-mgmt-cli-1.5.0b3/fabric_mgmt_cli/managecli/config_processor.py`

 * *Files identical despite different names*

### Comparing `fabric-mgmt-cli-1.5.0b2/fabric_mgmt_cli/managecli/configuration.py` & `fabric-mgmt-cli-1.5.0b3/fabric_mgmt_cli/managecli/configuration.py`

 * *Files identical despite different names*

### Comparing `fabric-mgmt-cli-1.5.0b2/fabric_mgmt_cli/managecli/kafka_processor.py` & `fabric-mgmt-cli-1.5.0b3/fabric_mgmt_cli/managecli/kafka_processor.py`

 * *Files identical despite different names*

### Comparing `fabric-mgmt-cli-1.5.0b2/fabric_mgmt_cli/managecli/manage_command.py` & `fabric-mgmt-cli-1.5.0b3/fabric_mgmt_cli/managecli/manage_command.py`

 * *Files identical despite different names*

### Comparing `fabric-mgmt-cli-1.5.0b2/fabric_mgmt_cli/managecli/managecli.py` & `fabric-mgmt-cli-1.5.0b3/fabric_mgmt_cli/managecli/managecli.py`

 * *Files identical despite different names*

### Comparing `fabric-mgmt-cli-1.5.0b2/fabric_mgmt_cli/managecli/net/commands.py` & `fabric-mgmt-cli-1.5.0b3/fabric_mgmt_cli/managecli/net/commands.py`

 * *Files identical despite different names*

### Comparing `fabric-mgmt-cli-1.5.0b2/fabric_mgmt_cli/managecli/net/nso.py` & `fabric-mgmt-cli-1.5.0b3/fabric_mgmt_cli/managecli/net/nso.py`

 * *Files identical despite different names*

### Comparing `fabric-mgmt-cli-1.5.0b2/fabric_mgmt_cli/managecli/net/resources.py` & `fabric-mgmt-cli-1.5.0b3/fabric_mgmt_cli/managecli/net/resources.py`

 * *Files identical despite different names*

### Comparing `fabric-mgmt-cli-1.5.0b2/fabric_mgmt_cli/managecli/net/services.py` & `fabric-mgmt-cli-1.5.0b3/fabric_mgmt_cli/managecli/net/services.py`

 * *Files identical despite different names*

### Comparing `fabric-mgmt-cli-1.5.0b2/fabric_mgmt_cli/managecli/net/util.py` & `fabric-mgmt-cli-1.5.0b3/fabric_mgmt_cli/managecli/net/util.py`

 * *Files identical despite different names*

### Comparing `fabric-mgmt-cli-1.5.0b2/fabric_mgmt_cli/managecli/show_command.py` & `fabric-mgmt-cli-1.5.0b3/fabric_mgmt_cli/managecli/show_command.py`

 * *Files identical despite different names*

### Comparing `fabric-mgmt-cli-1.5.0b2/fabric_mgmt_cli/managecli/test/config.yml` & `fabric-mgmt-cli-1.5.0b3/fabric_mgmt_cli/managecli/test/config.yml`

 * *Files identical despite different names*

### Comparing `fabric-mgmt-cli-1.5.0b2/fabric_mgmt_cli/managecli/test/test_managecli.py` & `fabric-mgmt-cli-1.5.0b3/fabric_mgmt_cli/managecli/test/test_managecli.py`

 * *Files identical despite different names*

### Comparing `fabric-mgmt-cli-1.5.0b2/net_inventory.yml` & `fabric-mgmt-cli-1.5.0b3/net_inventory.yml`

 * *Files identical despite different names*

### Comparing `fabric-mgmt-cli-1.5.0b2/pyproject.toml` & `fabric-mgmt-cli-1.5.0b3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 keywords = ["Swagger", "Fabric Management Cli"]
 
 requires-python = '>=3.9'
 dependencies = [
     "click==7.1.2",
     "pytest==7.1.1",
-    "fabric-cf==1.4.0",
+    "fabric-cf==1.5.0b4",
     "fabric-credmgr-client==1.5.0rc1"
     ]
 
 scripts = { "fabric-mgmt-cli" = "fabric_mgmt_cli.managecli.managecli:managecli"}
 
 [project.optional-dependencies]
 test = ["coverage>=4.0.3",
```

### Comparing `fabric-mgmt-cli-1.5.0b2/PKG-INFO` & `fabric-mgmt-cli-1.5.0b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: fabric-mgmt-cli
-Version: 1.5.0b2
+Version: 1.5.0b3
 Summary: FABRIC Management CLI
 Keywords: Swagger,Fabric Management Cli
 Author-email: Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: click==7.1.2
 Requires-Dist: pytest==7.1.1
-Requires-Dist: fabric-cf==1.4.0
+Requires-Dist: fabric-cf==1.5.0b4
 Requires-Dist: fabric-credmgr-client==1.5.0rc1
 Requires-Dist: coverage>=4.0.3 ; extra == "test"
 Requires-Dist: nose>=1.3.7 ; extra == "test"
 Requires-Dist: pluggy>=0.3.1 ; extra == "test"
 Requires-Dist: py>=1.4.31 ; extra == "test"
 Requires-Dist: randomize>=0.13 ; extra == "test"
 Project-URL: Home, https://fabric-testbed.net/
```

