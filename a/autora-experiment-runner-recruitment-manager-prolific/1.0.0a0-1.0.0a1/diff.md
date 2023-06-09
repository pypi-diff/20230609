# Comparing `tmp/autora-experiment-runner-recruitment-manager-prolific-1.0.0a0.tar.gz` & `tmp/autora-experiment-runner-recruitment-manager-prolific-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-experiment-runner-recruitment-manager-prolific-1.0.0a0.tar", last modified: Sun May  7 22:00:05 2023, max compression
+gzip compressed data, was "autora-experiment-runner-recruitment-manager-prolific-1.0.0a1.tar", last modified: Fri Jun  9 14:24:03 2023, max compression
```

## Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0a0.tar` & `autora-experiment-runner-recruitment-manager-prolific-1.0.0a1.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:00:05.537287 autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:00:05.533287 autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:00:05.533287 autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-07 21:59:51.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-07 21:59:51.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-07 21:59:51.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-07 22:00:05.537287 autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-07 21:59:51.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:00:05.533287 autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-07 21:59:51.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:00:05.533287 autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-07 21:59:51.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/docs/javascripts/mathjax.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:00:05.533287 autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-07 21:59:51.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-07 21:59:51.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-07 21:59:51.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 22:00:05.537287 autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:00:05.533287 autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:00:05.533287 autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:00:05.533287 autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/src/autora/experiment_runner/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:00:05.533287 autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/src/autora/experiment_runner/recruitment_manager/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:00:05.533287 autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/src/autora/experiment_runner/recruitment_manager/prolific/
--rw-r--r--   0 runner    (1001) docker     (123)     9985 2023-05-07 21:59:51.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/src/autora/experiment_runner/recruitment_manager/prolific/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:00:05.537287 autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-07 22:00:05.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-07 22:00:05.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 22:00:05.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-07 22:00:05.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-07 22:00:05.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:00:05.537287 autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-07 21:59:51.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 21:59:51.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-07 21:59:51.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/tests/test_recruitment_manager_prolific.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:24:03.069054 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:24:03.065053 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:24:03.065053 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-09 14:23:49.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-09 14:23:49.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-09 14:23:49.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-09 14:24:03.069054 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-09 14:23:49.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:24:03.065053 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-06-09 14:23:49.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/docs/Basic Usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-09 14:23:49.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:24:03.065053 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-09 14:23:49.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-09 14:23:49.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:24:03.069054 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-09 14:23:49.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-09 14:23:49.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-09 14:23:49.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 14:24:03.069054 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:24:03.065053 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:24:03.065053 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:24:03.065053 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/src/autora/experiment_runner/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:24:03.065053 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/src/autora/experiment_runner/recruitment_manager/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:24:03.069054 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/src/autora/experiment_runner/recruitment_manager/prolific/
+-rw-r--r--   0 runner    (1001) docker     (123)    10592 2023-06-09 14:23:49.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/src/autora/experiment_runner/recruitment_manager/prolific/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:24:03.069054 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-09 14:24:03.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-09 14:24:03.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 14:24:03.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-09 14:24:03.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-09 14:24:03.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:24:03.069054 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-09 14:23:49.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 14:23:49.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-09 14:23:49.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/tests/test_recruitment_manager_prolific.py
```

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/.github/workflows/python-publish.yml` & `autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/.gitignore` & `autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/.pre-commit-config.yaml` & `autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/PKG-INFO` & `autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 Metadata-Version: 2.1
 Name: autora-experiment-runner-recruitment-manager-prolific
-Version: 1.0.0a0
-Summary: AutoRA Prolific Recruitment Manager provides functionality to recruite participants via Prolific to setup an experiment runner for AutoRA
+Version: 1.0.0a1
+Summary: AutoRA Prolific Recruitment Manager provides functionality to recruit participants via Prolific to set up an experiment runner for AutoRA
 Author-email: Kevin Phan <kphan@princeton.edu>, Younes Strittmatter <younes_strittmatter@brown.edu>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-experiment-runner-recruitment-manager-prolific
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # AutoRA Prolific Recruitment Manager
 
-AutoRA Prolific Recruitment Manager provides functionality to recruit participants via Prolific to set up an experiment runner for AutoRA.
+Prolific Recruitment Manager provides functionality to recruit participants via Prolific to set up an experiment runner for AutoRA.
 
-Website: https://autoresearch.github.io/autora/
+# Quickstart Guide
 
-## User Guide
+You will need:
+`python` >=3.8,<4: [https://www.python.org/downloads/](https://www.python.org/downloads/)
 
-Install this in an environment using your chosen package manager. In this example we are using virtualenv
+!!! It is recommended to use a python environment manger like virtualenv
 
-Install:
-- python (3.8 or greater): https://www.python.org/downloads/
-- virtualenv: https://virtualenv.pypa.io/en/latest/installation.html
+Install the package via pip:
 
-Install the Prolific Recruitment Manager as part of the autora package:
+```shell
+pip install "aurora[experiment-runner-recruitment-manager-prolific]"
+```
 
-pip install -U "autora[experiment-runner-recruitment-manager-prolific]"
+## Test
+```shell
+python -c "from autora.experiment_runner.recruitment_manager.prolific import setup_study"
+```
+
+
+## Dependencies
+
+autora-core
```

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/README.md` & `autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 # AutoRA Prolific Recruitment Manager
 
-AutoRA Prolific Recruitment Manager provides functionality to recruit participants via Prolific to set up an experiment runner for AutoRA.
+Prolific Recruitment Manager provides functionality to recruit participants via Prolific to set up an experiment runner for AutoRA.
 
-Website: https://autoresearch.github.io/autora/
+# Quickstart Guide
 
-## User Guide
+You will need:
+`python` >=3.8,<4: [https://www.python.org/downloads/](https://www.python.org/downloads/)
 
-Install this in an environment using your chosen package manager. In this example we are using virtualenv
+!!! It is recommended to use a python environment manger like virtualenv
 
-Install:
-- python (3.8 or greater): https://www.python.org/downloads/
-- virtualenv: https://virtualenv.pypa.io/en/latest/installation.html
+Install the package via pip:
 
-Install the Prolific Recruitment Manager as part of the autora package:
+```shell
+pip install "aurora[experiment-runner-recruitment-manager-prolific]"
+```
 
-pip install -U "autora[experiment-runner-recruitment-manager-prolific]"
+## Test
+```shell
+python -c "from autora.experiment_runner.recruitment_manager.prolific import setup_study"
+```
+
+
+## Dependencies
+
+autora-core
```

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/mkdocs/base.yml` & `autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/pyproject.toml` & `autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 # UPDATE THIS BEFORE PUBLISHING
 name = "autora-experiment-runner-recruitment-manager-prolific"
-description = "AutoRA Prolific Recruitment Manager provides functionality to recruite participants via Prolific to setup an experiment runner for AutoRA"
+description = "AutoRA Prolific Recruitment Manager provides functionality to recruit participants via Prolific to set up an experiment runner for AutoRA"
 authors = [
     { name = "Kevin Phan", email = "kphan@princeton.edu"},
     { name = "Younes Strittmatter", email = "younes_strittmatter@brown.edu" }]
 dynamic = ["version"]
 
 readme = "README.md"
 license = { text = "MIT License" }
```

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/src/autora/experiment_runner/recruitment_manager/prolific/__init__.py` & `autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/src/autora/experiment_runner/recruitment_manager/prolific/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import random
 import string
 from typing import Any, List
 import requests
+import json
 
 
 def _list_studies(prolific_token: str):
     """
     Returns list of all studies on Prolific account.
     """
     studies = requests.get(
@@ -94,49 +95,54 @@
 
 
 def setup_study(
         name: str,
         description: str,
         external_study_url: str,
         estimated_completion_time: int,
+        prolific_token: str,
         exclude_studies: List[str] = ["default"],
         reward: int = 0,
         prolific_id_option: str = "url_parameters",
         completion_code: str = "",
         completion_option: str = "url",
         total_available_places: int = 1,
         eligibility_requirements: List[str] = ["default"],
         device_compatibility: List[str] = ["desktop"],
         peripheral_requirements=None,
-        prolific_token: str = "",
+        temp_file='',
+
 ) -> Any:
     """
     Allows for a study to be drafted given the following parameters.
 
     Args:
         name (str): Name that will be displayed on prolific
         description (str): Description of study for participants
         external_study_url (str): URL to experiment website
         estimated_completion_time (int): How long the study takes
+        prolific_token: (str): The Api token from your prolific-account
+            (https://app.prolific.co/ under settings)
         exclude_studies (list): Exclude participants that participated in previous studies
             (default is studies with the same name)
         prolific_id_option (ProlificIdOptions): Method of collecting subject ID
         completion_code (str): Code subject uses to mark experiment completion
         completion_option (CompletionOptions): Method of signifying participation
         total_available_places (int): Participant limit
         reward (int): Amount of payment for completion
         eligibility_requirements (list, optional): Allows various options to filter participants.
             Defaults to [] (no requirements).
         device_compatibility (list[DeviceOptions], optional): Allows selecting required devices.
             Defaults to [] (any device).
         peripheral_requirements (list[PeripheralOptions], optional):
             Allows specifying additional requirements. Defaults to [] (no other requirements).
+        temp_file (str, optional): File to save the study_id and max_allowed_time for restarting later
 
     Returns:
-        bool: Whether the request was successful or not
+        dictionary: A dictionary with the id and maximum allowed time for the study (or False if something went wrong)
     """
     if eligibility_requirements is None:
         eligibility_requirements = []
     if exclude_studies is None:
         exclude_studies = []
     if exclude_studies == ["default"]:
         exclude_studies = [name]
@@ -181,20 +187,28 @@
         json=data,
     )
 
     # handles request failure
     if study.status_code >= 400:
         print(study.json())
         return False
-    print(study.json())
     keys_to_include = ["id", "maximum_allowed_time"]
-    return dict(
+    study_dict = dict(
         (key, value) for key, value in study.json().items() if key in keys_to_include
     )
 
+    # save to temp_file
+    if temp_file != '':
+        if not str.endswith(temp_file, '.json'):
+            raise ValueError(f"Error: File '{temp_file}' is not in the correct JSON format.")
+        with open(temp_file, 'w') as file:
+            json.dump(study_dict, temp_file)
+
+    return study_dict
+
 
 def _update_study_status(study_id: str, action: str, prolific_token: str):
     """
     Performs action on specified study. Default action is to publish
     the study.
     """
     data = {"action": action}
```

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/PKG-INFO` & `autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 Metadata-Version: 2.1
 Name: autora-experiment-runner-recruitment-manager-prolific
-Version: 1.0.0a0
-Summary: AutoRA Prolific Recruitment Manager provides functionality to recruite participants via Prolific to setup an experiment runner for AutoRA
+Version: 1.0.0a1
+Summary: AutoRA Prolific Recruitment Manager provides functionality to recruit participants via Prolific to set up an experiment runner for AutoRA
 Author-email: Kevin Phan <kphan@princeton.edu>, Younes Strittmatter <younes_strittmatter@brown.edu>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-experiment-runner-recruitment-manager-prolific
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # AutoRA Prolific Recruitment Manager
 
-AutoRA Prolific Recruitment Manager provides functionality to recruit participants via Prolific to set up an experiment runner for AutoRA.
+Prolific Recruitment Manager provides functionality to recruit participants via Prolific to set up an experiment runner for AutoRA.
 
-Website: https://autoresearch.github.io/autora/
+# Quickstart Guide
 
-## User Guide
+You will need:
+`python` >=3.8,<4: [https://www.python.org/downloads/](https://www.python.org/downloads/)
 
-Install this in an environment using your chosen package manager. In this example we are using virtualenv
+!!! It is recommended to use a python environment manger like virtualenv
 
-Install:
-- python (3.8 or greater): https://www.python.org/downloads/
-- virtualenv: https://virtualenv.pypa.io/en/latest/installation.html
+Install the package via pip:
 
-Install the Prolific Recruitment Manager as part of the autora package:
+```shell
+pip install "aurora[experiment-runner-recruitment-manager-prolific]"
+```
 
-pip install -U "autora[experiment-runner-recruitment-manager-prolific]"
+## Test
+```shell
+python -c "from autora.experiment_runner.recruitment_manager.prolific import setup_study"
+```
+
+
+## Dependencies
+
+autora-core
```

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/SOURCES.txt` & `autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 .gitignore
 .pre-commit-config.yaml
 README.md
 mkdocs.yml
 pyproject.toml
 .github/workflows/python-publish.yml
+docs/Basic Usage.ipynb
 docs/index.md
+docs/quickstart.md
 docs/javascripts/mathjax.js
 mkdocs/base.yml
 src/autora/experiment_runner/recruitment_manager/prolific/__init__.py
 src/autora_experiment_runner_recruitment_manager_prolific.egg-info/PKG-INFO
 src/autora_experiment_runner_recruitment_manager_prolific.egg-info/SOURCES.txt
 src/autora_experiment_runner_recruitment_manager_prolific.egg-info/dependency_links.txt
 src/autora_experiment_runner_recruitment_manager_prolific.egg-info/requires.txt
```

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0a0/tests/README.md` & `autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/tests/README.md`

 * *Files identical despite different names*

