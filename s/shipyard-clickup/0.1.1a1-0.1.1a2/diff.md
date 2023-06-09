# Comparing `tmp/shipyard_clickup-0.1.1a1.tar.gz` & `tmp/shipyard_clickup-0.1.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_clickup-0.1.1a1.tar", max compression
+gzip compressed data, was "shipyard_clickup-0.1.1a2.tar", max compression
```

## Comparing `shipyard_clickup-0.1.1a1.tar` & `shipyard_clickup-0.1.1a2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2023-06-06 18:57:29.881322 shipyard_clickup-0.1.1a1/README.md
--rw-r--r--   0        0        0      497 2023-06-07 13:53:50.666465 shipyard_clickup-0.1.1a1/pyproject.toml
--rw-r--r--   0        0        0       34 2023-06-06 19:37:34.627359 shipyard_clickup-0.1.1a1/shipyard_clickup/__init__.py
--rw-r--r--   0        0        0     1183 2023-06-07 13:32:49.075282 shipyard_clickup-0.1.1a1/shipyard_clickup/cli/add_comment.py
--rw-r--r--   0        0        0     1380 2023-06-07 13:32:49.072399 shipyard_clickup-0.1.1a1/shipyard_clickup/cli/create_task.py
--rw-r--r--   0        0        0     1380 2023-06-07 13:38:04.029507 shipyard_clickup-0.1.1a1/shipyard_clickup/cli/edit_task.py
--rw-r--r--   0        0        0     6365 2023-06-06 18:57:29.882745 shipyard_clickup-0.1.1a1/shipyard_clickup/clickup.py
--rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 shipyard_clickup-0.1.1a1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-06 18:57:29.881322 shipyard_clickup-0.1.1a2/README.md
+-rw-r--r--   0        0        0      497 2023-06-09 14:03:43.528644 shipyard_clickup-0.1.1a2/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-06-08 18:35:19.166767 shipyard_clickup-0.1.1a2/shipyard_clickup/__init__.py
+-rw-r--r--   0        0        0     1183 2023-06-08 18:35:19.167076 shipyard_clickup-0.1.1a2/shipyard_clickup/cli/add_comment.py
+-rw-r--r--   0        0        0     1380 2023-06-08 18:35:19.167288 shipyard_clickup-0.1.1a2/shipyard_clickup/cli/create_task.py
+-rw-r--r--   0        0        0     1366 2023-06-08 19:51:09.374611 shipyard_clickup-0.1.1a2/shipyard_clickup/cli/edit_task.py
+-rw-r--r--   0        0        0     6365 2023-06-06 18:57:29.882745 shipyard_clickup-0.1.1a2/shipyard_clickup/clickup.py
+-rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 shipyard_clickup-0.1.1a2/PKG-INFO
```

### Comparing `shipyard_clickup-0.1.1a1/shipyard_clickup/cli/add_comment.py` & `shipyard_clickup-0.1.1a2/shipyard_clickup/cli/add_comment.py`

 * *Files identical despite different names*

### Comparing `shipyard_clickup-0.1.1a1/shipyard_clickup/cli/create_task.py` & `shipyard_clickup-0.1.1a2/shipyard_clickup/cli/create_task.py`

 * *Files identical despite different names*

### Comparing `shipyard_clickup-0.1.1a1/shipyard_clickup/cli/edit_task.py` & `shipyard_clickup-0.1.1a2/shipyard_clickup/cli/edit_task.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from shipyard_clickup import ClickupClient
 from shipyard_templates import ExitCodeError
 
 
 def get_args():
     parser = argparse.ArgumentParser()
     parser.add_argument('--access-token', required=True, help='Access token for ClickUp API')
-    parser.add_argument('--list-id', required=True, help='ID of the ClickUp List')
-    parser.add_argument('--name', required=True, help='Name of the task')
+    parser.add_argument('--task-id', required=True, help='ID of the ClickUp task')
+    parser.add_argument('--name',  help='Name of the task')
     parser.add_argument('--description')
     parser.add_argument('--tags')
     parser.add_argument('--due-date')
     parser.add_argument('--status')
     parser.add_argument('--parent', help='Use if ticket should be a subtask of another ticket')
     return parser.parse_args()
```

### Comparing `shipyard_clickup-0.1.1a1/shipyard_clickup/clickup.py` & `shipyard_clickup-0.1.1a2/shipyard_clickup/clickup.py`

 * *Files identical despite different names*

