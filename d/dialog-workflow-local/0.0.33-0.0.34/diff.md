# Comparing `tmp/dialog-workflow-local-0.0.33.tar.gz` & `tmp/dialog-workflow-local-0.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dialog-workflow-local-0.0.33.tar", last modified: Fri Jun  9 11:58:34 2023, max compression
+gzip compressed data, was "dialog-workflow-local-0.0.34.tar", last modified: Fri Jun  9 12:36:59 2023, max compression
```

## Comparing `dialog-workflow-local-0.0.33.tar` & `dialog-workflow-local-0.0.34.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:58:34.717612 dialog-workflow-local-0.0.33/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-09 11:58:34.717612 dialog-workflow-local-0.0.33/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-09 11:58:24.000000 dialog-workflow-local-0.0.33/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:58:34.713612 dialog-workflow-local-0.0.33/dialog_workflow/
--rw-r--r--   0 runner    (1001) docker     (123)    20876 2023-06-09 11:58:24.000000 dialog-workflow-local-0.0.33/dialog_workflow/Act.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-09 11:58:24.000000 dialog-workflow-local-0.0.33/dialog_workflow/Constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-09 11:58:24.000000 dialog-workflow-local-0.0.33/dialog_workflow/DialogWorkflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-06-09 11:58:24.000000 dialog-workflow-local-0.0.33/dialog_workflow/TablesAsObjects.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:58:24.000000 dialog-workflow-local-0.0.33/dialog_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-06-09 11:58:24.000000 dialog-workflow-local-0.0.33/dialog_workflow/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-06-09 11:58:24.000000 dialog-workflow-local-0.0.33/dialog_workflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:58:34.717612 dialog-workflow-local-0.0.33/dialog_workflow_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-09 11:58:34.000000 dialog-workflow-local-0.0.33/dialog_workflow_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-09 11:58:34.000000 dialog-workflow-local-0.0.33/dialog_workflow_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 11:58:34.000000 dialog-workflow-local-0.0.33/dialog_workflow_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-09 11:58:34.000000 dialog-workflow-local-0.0.33/dialog_workflow_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-09 11:58:24.000000 dialog-workflow-local-0.0.33/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 11:58:34.717612 dialog-workflow-local-0.0.33/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-09 11:58:24.000000 dialog-workflow-local-0.0.33/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:36:59.970797 dialog-workflow-local-0.0.34/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-09 12:36:59.970797 dialog-workflow-local-0.0.34/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-09 12:36:50.000000 dialog-workflow-local-0.0.34/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:36:59.966797 dialog-workflow-local-0.0.34/dialog_workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    20908 2023-06-09 12:36:50.000000 dialog-workflow-local-0.0.34/dialog_workflow/Act.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-09 12:36:50.000000 dialog-workflow-local-0.0.34/dialog_workflow/Constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-09 12:36:50.000000 dialog-workflow-local-0.0.34/dialog_workflow/DialogWorkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-06-09 12:36:50.000000 dialog-workflow-local-0.0.34/dialog_workflow/TablesAsObjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:36:50.000000 dialog-workflow-local-0.0.34/dialog_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-06-09 12:36:50.000000 dialog-workflow-local-0.0.34/dialog_workflow/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-06-09 12:36:50.000000 dialog-workflow-local-0.0.34/dialog_workflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:36:59.966797 dialog-workflow-local-0.0.34/dialog_workflow_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-09 12:36:59.000000 dialog-workflow-local-0.0.34/dialog_workflow_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-09 12:36:59.000000 dialog-workflow-local-0.0.34/dialog_workflow_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 12:36:59.000000 dialog-workflow-local-0.0.34/dialog_workflow_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-09 12:36:59.000000 dialog-workflow-local-0.0.34/dialog_workflow_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-09 12:36:50.000000 dialog-workflow-local-0.0.34/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 12:36:59.970797 dialog-workflow-local-0.0.34/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-09 12:36:50.000000 dialog-workflow-local-0.0.34/setup.py
```

### Comparing `dialog-workflow-local-0.0.33/dialog_workflow/Act.py` & `dialog-workflow-local-0.0.34/dialog_workflow/Act.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dialog_workflow.utils import *
 from dialog_workflow.TablesAsObjects import DialogWorkflowRecord, Variable, ProfileContext
 import time
 # import msvcrt
 # import requests
-from AgeDetection import DetectAge
+# from AgeDetection import DetectAge
 
 class action(object):
     def __init__(self, incoming_message: str, profile_id: int, language: str, profile_curr_state: int, variables: Variable):
         self.incoming_message = incoming_message
         self.profile_id = profile_id
         self.language = language
         self.variables = variables
@@ -184,29 +184,29 @@
         if outgoing_message != None: #returns the outgoing message to send to the user.
             return False, outgoing_message
         self.profile_curr_state = next_state_id
         self.accumulated_message = ""
         return is_state_changed, None
         
     def age_detection(self):
-        """Action that recieves a path to a picture (for now the picture has to be stored in the folder) 
-            and returns the approximate age of the person in the picture.
-            Stores the picture in database storage."""
-        if not self.got_response:
-            self.accumulated_message += "Please insert a path to the picture~"
-            outgoing_message = process_message(communication_type= COMMUNICATION_TYPE, action_type= action_enum.AGE_DETECTION.value, message= self.accumulated_message) 
-            if COMMUNICATION_TYPE == communication_type_enum.WEBSOCKET.value:
-                return False, outgoing_message
-            else:
-                self.accumulated_message = ""         
-                self.incoming_message = input()
-        age_range = DetectAge.detect(self.incoming_message)
-        self.accumulated_message += f'The approximate age of the picture you have sent is: {age_range}~'
-        insert_profile_variable_value(self.profile_id, self.record.variable1_id, age_range, self.profile_curr_state)
-        store_age_detection_picture(age_range, self.profile_curr_state)
+    #     """Action that recieves a path to a picture (for now the picture has to be stored in the folder) 
+    #         and returns the approximate age of the person in the picture.
+    #         Stores the picture in database storage."""
+    #     if not self.got_response:
+    #         self.accumulated_message += "Please insert a path to the picture~"
+    #         outgoing_message = process_message(communication_type= COMMUNICATION_TYPE, action_type= action_enum.AGE_DETECTION.value, message= self.accumulated_message) 
+    #         if COMMUNICATION_TYPE == communication_type_enum.WEBSOCKET.value:
+    #             return False, outgoing_message
+    #         else:
+    #             self.accumulated_message = ""         
+    #             self.incoming_message = input()
+    #     age_range = DetectAge.detect(self.incoming_message)
+    #     self.accumulated_message += f'The approximate age of the picture you have sent is: {age_range}~'
+    #     insert_profile_variable_value(self.profile_id, self.record.variable1_id, age_range, self.profile_curr_state)
+    #     store_age_detection_picture(age_range, self.profile_curr_state)
         return False, None
     
     def multi_choice_poll(self):
         """ Similar to Menu Action. If the user chose a single option we jump to next_state_id of the chosen option. 
             Otherwise we save the answers and jump to the next_state_id of the parent."""
         fields_to_select = ["parameter1", "next_state_id"]
         table_name = "dialog_workflow_state_view"
```

### Comparing `dialog-workflow-local-0.0.33/dialog_workflow/Constants.py` & `dialog-workflow-local-0.0.34/dialog_workflow/Constants.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.33/dialog_workflow/DialogWorkflow.py` & `dialog-workflow-local-0.0.34/dialog_workflow/DialogWorkflow.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.33/dialog_workflow/TablesAsObjects.py` & `dialog-workflow-local-0.0.34/dialog_workflow/TablesAsObjects.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.33/dialog_workflow/test.py` & `dialog-workflow-local-0.0.34/dialog_workflow/test.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.33/dialog_workflow/utils.py` & `dialog-workflow-local-0.0.34/dialog_workflow/utils.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.33/setup.py` & `dialog-workflow-local-0.0.34/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
      name='dialog-workflow-local',  
-     version='0.0.33',
+     version='0.0.34',
      author="Circles",
      author_email="info@circle.life",
      description="PyPI Package for dialog workflow",
      long_description="This is a package for running the dialog workflow",
      long_description_content_type="text/markdown",
      url="https://github.com/javatechy/dokr",
      packages=setuptools.find_packages(),
```

