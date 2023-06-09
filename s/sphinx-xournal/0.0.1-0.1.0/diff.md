# Comparing `tmp/sphinx_xournal-0.0.1.tar.gz` & `tmp/sphinx_xournal-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_xournal-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sphinx_xournal-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sphinx_xournal-0.0.1.tar` & `sphinx_xournal-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,18 @@
--rw-r--r--   0        0        0      268 2023-06-09 14:52:42.773620 sphinx_xournal-0.0.1/.editorconfig
--rw-r--r--   0        0        0       62 2023-06-09 14:52:42.773620 sphinx_xournal-0.0.1/.gitignore
--rw-r--r--   0        0        0     2165 2023-06-09 15:07:41.905317 sphinx_xournal-0.0.1/.gitlab-ci.yml
--rw-r--r--   0        0        0      178 2023-06-09 14:52:42.773620 sphinx_xournal-0.0.1/AUTHORS.rst
--rw-r--r--   0        0        0       89 2023-06-09 14:52:42.773620 sphinx_xournal-0.0.1/HISTORY.rst
--rw-r--r--   0        0        0     7642 2023-06-09 14:52:42.773620 sphinx_xournal-0.0.1/LICENSE
--rw-r--r--   0        0        0      167 2023-06-09 14:52:42.773620 sphinx_xournal-0.0.1/README.rst
--rw-r--r--   0        0        0     1222 2023-06-09 14:52:42.773620 sphinx_xournal-0.0.1/docs/templates/pyproject.toml
--rw-r--r--   0        0        0     1052 2023-06-09 14:52:42.773620 sphinx_xournal-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      283 2023-06-09 14:52:42.773620 sphinx_xournal-0.0.1/requirements.txt
--rw-r--r--   0        0        0      202 2023-06-09 14:52:42.777621 sphinx_xournal-0.0.1/sphinx_xournal/__init__.py
--rw-r--r--   0        0        0     3320 2023-06-09 14:52:42.777621 sphinx_xournal-0.0.1/tasks.py
--rw-r--r--   0        0        0     1390 1970-01-01 00:00:00.000000 sphinx_xournal-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      268 2023-06-09 14:52:42.773620 sphinx_xournal-0.1.0/.editorconfig
+-rw-r--r--   0        0        0       62 2023-06-09 14:52:42.773620 sphinx_xournal-0.1.0/.gitignore
+-rw-r--r--   0        0        0     2244 2023-06-09 19:39:40.610842 sphinx_xournal-0.1.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0      178 2023-06-09 14:52:42.773620 sphinx_xournal-0.1.0/AUTHORS.rst
+-rw-r--r--   0        0        0      156 2023-06-09 19:39:40.614842 sphinx_xournal-0.1.0/HISTORY.rst
+-rw-r--r--   0        0        0     7642 2023-06-09 14:52:42.773620 sphinx_xournal-0.1.0/LICENSE
+-rw-r--r--   0        0        0      167 2023-06-09 14:52:42.773620 sphinx_xournal-0.1.0/README.rst
+-rw-r--r--   0        0        0     1222 2023-06-09 14:52:42.773620 sphinx_xournal-0.1.0/docs/templates/pyproject.toml
+-rw-r--r--   0        0        0     1052 2023-06-09 14:52:42.773620 sphinx_xournal-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      283 2023-06-09 14:52:42.773620 sphinx_xournal-0.1.0/requirements.txt
+-rw-r--r--   0        0        0      241 2023-06-09 19:39:40.614842 sphinx_xournal-0.1.0/sphinx_xournal/__init__.py
+-rw-r--r--   0        0        0     3774 2023-06-09 19:39:40.614842 sphinx_xournal-0.1.0/sphinx_xournal/convert.py
+-rw-r--r--   0        0        0     1713 2023-06-09 19:39:40.614842 sphinx_xournal-0.1.0/sphinx_xournal/directives.py
+-rw-r--r--   0        0        0      945 2023-06-09 19:39:40.614842 sphinx_xournal-0.1.0/sphinx_xournal/exceptions.py
+-rw-r--r--   0        0        0     1453 2023-06-09 19:39:40.614842 sphinx_xournal-0.1.0/sphinx_xournal/main.py
+-rw-r--r--   0        0        0        0 2023-06-09 19:50:18.135236 sphinx_xournal-0.1.0/sphinx_xournal/xournal.css
+-rw-r--r--   0        0        0     3320 2023-06-09 14:52:42.777621 sphinx_xournal-0.1.0/tasks.py
+-rw-r--r--   0        0        0     1390 1970-01-01 00:00:00.000000 sphinx_xournal-0.1.0/PKG-INFO
```

### Comparing `sphinx_xournal-0.0.1/.gitlab-ci.yml` & `sphinx_xournal-0.1.0/.gitlab-ci.yml`

 * *Files 12% similar despite different names*

```diff
@@ -15,17 +15,20 @@
   image: python:3.11
   stage: release
   before_script:
     - python -V
     - echo "${CI_API_V4_URL}/projects/${CI_PROJECT_ID}/packages/pypi"
   script:
     - pip install build twine flit
-    - FLIT_NO_NETWORK=1
+    #- FLIT_NO_NETWORK=1
     - FLIT_INDEX_URL=${CI_API_V4_URL}/projects/${CI_PROJECT_ID}/packages/pypi flit build
     - TWINE_PASSWORD=${CI_JOB_TOKEN} TWINE_USERNAME=gitlab-ci-token python -m twine upload --repository-url ${CI_API_V4_URL}/projects/${CI_PROJECT_ID}/packages/pypi dist/*
+  cache:
+    paths:
+      - .cache/pip
   rules:
     - if: $CI_COMMIT_TAG
     - if: $CI_PIPELINE_SOURCE == "push" || $CI_COMMIT_BRANCH == "dev"
       when: manual
       allow_failure: true
 
 build-upload-pypi:
@@ -34,14 +37,17 @@
   before_script:
     - python -V
     - echo "${CI_API_V4_URL}/projects/${CI_PROJECT_ID}/packages/pypi"
   script:
     - pip install build twine flit
     - flit build
     - python -m twine upload dist/*
+  cache:
+    paths:
+      - .cache/pip
   rules:
     - if: $CI_COMMIT_TAG
     - if: $CI_PIPELINE_SOURCE == "push" || $CI_COMMIT_BRANCH == "dev"
       when: manual
       allow_failure: true
 
 deploy-docs:
```

### Comparing `sphinx_xournal-0.0.1/LICENSE` & `sphinx_xournal-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_xournal-0.0.1/docs/templates/pyproject.toml` & `sphinx_xournal-0.1.0/docs/templates/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sphinx_xournal-0.0.1/pyproject.toml` & `sphinx_xournal-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sphinx_xournal-0.0.1/tasks.py` & `sphinx_xournal-0.1.0/tasks.py`

 * *Files identical despite different names*

### Comparing `sphinx_xournal-0.0.1/PKG-INFO` & `sphinx_xournal-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-xournal
-Version: 0.0.1
+Version: 0.1.0
 Summary: Sphinx extension to generate images from xournal files.
 Keywords: sphinx,xournal,notes
 Author-email: Arkadiusz Michał Ryś <Arkadiusz.Michal.Rys@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Programming Language :: Python :: 3
```

