# Comparing `tmp/autora-experiment-runner-recruitment-manager-prolific-1.0.0a1.tar.gz` & `tmp/autora-experiment-runner-recruitment-manager-prolific-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-experiment-runner-recruitment-manager-prolific-1.0.0a1.tar", last modified: Fri Jun  9 14:24:03 2023, max compression
+gzip compressed data, was "autora-experiment-runner-recruitment-manager-prolific-1.0.0a2.tar", last modified: Fri Jun  9 15:04:00 2023, max compression
```

## Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0a1.tar` & `autora-experiment-runner-recruitment-manager-prolific-1.0.0a2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:24:03.069054 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:24:03.065053 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:24:03.065053 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-09 14:23:49.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-09 14:23:49.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-09 14:23:49.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-09 14:24:03.069054 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-09 14:23:49.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:24:03.065053 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-06-09 14:23:49.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/docs/Basic Usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-09 14:23:49.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:24:03.065053 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-09 14:23:49.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-09 14:23:49.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:24:03.069054 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-09 14:23:49.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-09 14:23:49.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-09 14:23:49.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 14:24:03.069054 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:24:03.065053 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:24:03.065053 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:24:03.065053 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/src/autora/experiment_runner/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:24:03.065053 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/src/autora/experiment_runner/recruitment_manager/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:24:03.069054 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/src/autora/experiment_runner/recruitment_manager/prolific/
--rw-r--r--   0 runner    (1001) docker     (123)    10592 2023-06-09 14:23:49.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/src/autora/experiment_runner/recruitment_manager/prolific/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:24:03.069054 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-09 14:24:03.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-09 14:24:03.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 14:24:03.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-09 14:24:03.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-09 14:24:03.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:24:03.069054 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-09 14:23:49.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 14:23:49.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-09 14:23:49.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/tests/test_recruitment_manager_prolific.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:04:00.309410 autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:04:00.301410 autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:04:00.305410 autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-09 15:03:45.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-09 15:03:45.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-09 15:03:45.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-09 15:04:00.309410 autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-09 15:03:45.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:04:00.305410 autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-06-09 15:03:45.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/docs/Basic Usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-09 15:03:45.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:04:00.305410 autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-09 15:03:45.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-09 15:03:45.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:04:00.305410 autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-09 15:03:45.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-09 15:03:45.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-09 15:03:45.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 15:04:00.309410 autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:04:00.301410 autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:04:00.301410 autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:04:00.301410 autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/src/autora/experiment_runner/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:04:00.301410 autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/src/autora/experiment_runner/recruitment_manager/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:04:00.305410 autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/src/autora/experiment_runner/recruitment_manager/prolific/
+-rw-r--r--   0 runner    (1001) docker     (123)    10587 2023-06-09 15:03:45.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/src/autora/experiment_runner/recruitment_manager/prolific/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:04:00.309410 autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-09 15:04:00.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-09 15:04:00.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 15:04:00.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-09 15:04:00.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-09 15:04:00.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:04:00.309410 autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-09 15:03:45.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 15:03:45.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-09 15:03:45.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/tests/test_recruitment_manager_prolific.py
```

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/.github/workflows/python-publish.yml` & `autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/.gitignore` & `autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/.pre-commit-config.yaml` & `autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/PKG-INFO` & `autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experiment-runner-recruitment-manager-prolific
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: AutoRA Prolific Recruitment Manager provides functionality to recruit participants via Prolific to set up an experiment runner for AutoRA
 Author-email: Kevin Phan <kphan@princeton.edu>, Younes Strittmatter <younes_strittmatter@brown.edu>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-experiment-runner-recruitment-manager-prolific
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/README.md` & `autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/README.md`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/docs/Basic Usage.ipynb` & `autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/docs/Basic Usage.ipynb`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/mkdocs/base.yml` & `autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/pyproject.toml` & `autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/src/autora/experiment_runner/recruitment_manager/prolific/__init__.py` & `autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/src/autora/experiment_runner/recruitment_manager/prolific/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,15 +197,15 @@
     )
 
     # save to temp_file
     if temp_file != '':
         if not str.endswith(temp_file, '.json'):
             raise ValueError(f"Error: File '{temp_file}' is not in the correct JSON format.")
         with open(temp_file, 'w') as file:
-            json.dump(study_dict, temp_file)
+            json.dump(study_dict, file)
 
     return study_dict
 
 
 def _update_study_status(study_id: str, action: str, prolific_token: str):
     """
     Performs action on specified study. Default action is to publish
```

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/PKG-INFO` & `autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experiment-runner-recruitment-manager-prolific
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: AutoRA Prolific Recruitment Manager provides functionality to recruit participants via Prolific to set up an experiment runner for AutoRA
 Author-email: Kevin Phan <kphan@princeton.edu>, Younes Strittmatter <younes_strittmatter@brown.edu>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-experiment-runner-recruitment-manager-prolific
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/SOURCES.txt` & `autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0a1/tests/README.md` & `autora-experiment-runner-recruitment-manager-prolific-1.0.0a2/tests/README.md`

 * *Files identical despite different names*

