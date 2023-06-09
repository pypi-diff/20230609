# Comparing `tmp/osw-0.8.0.tar.gz` & `tmp/osw-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osw-0.8.0.tar", last modified: Sun May 21 16:06:29 2023, max compression
+gzip compressed data, was "osw-0.8.1.tar", last modified: Fri Jun  9 16:39:45 2023, max compression
```

## Comparing `osw-0.8.0.tar` & `osw-0.8.1.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:06:29.906982 osw-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-21 16:05:56.000000 osw-0.8.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:06:29.874982 osw-0.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:06:29.886982 osw-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-05-21 16:05:56.000000 osw-0.8.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-21 16:05:56.000000 osw-0.8.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-21 16:05:56.000000 osw-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-21 16:05:56.000000 osw-0.8.0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-21 16:05:56.000000 osw-0.8.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-21 16:05:56.000000 osw-0.8.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-21 16:05:56.000000 osw-0.8.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-21 16:05:56.000000 osw-0.8.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-21 16:05:56.000000 osw-0.8.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-21 16:05:56.000000 osw-0.8.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)    13425 2023-05-21 16:05:56.000000 osw-0.8.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    32387 2023-05-21 16:05:56.000000 osw-0.8.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-21 16:06:29.906982 osw-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-21 16:05:56.000000 osw-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-21 16:05:56.000000 osw-0.8.0/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:06:29.894982 osw-0.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-21 16:05:56.000000 osw-0.8.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:06:29.894982 osw-0.8.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-21 16:05:56.000000 osw-0.8.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-21 16:05:56.000000 osw-0.8.0/docs/auth.md
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-21 16:05:56.000000 osw-0.8.0/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-21 16:05:56.000000 osw-0.8.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10000 2023-05-21 16:05:56.000000 osw-0.8.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-21 16:05:56.000000 osw-0.8.0/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-21 16:05:56.000000 osw-0.8.0/docs/controller.md
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-21 16:05:56.000000 osw-0.8.0/docs/dev.md
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-21 16:05:56.000000 osw-0.8.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-21 16:05:56.000000 osw-0.8.0/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-21 16:05:56.000000 osw-0.8.0/docs/model.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-21 16:05:56.000000 osw-0.8.0/docs/osw.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-21 16:05:56.000000 osw-0.8.0/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-21 16:05:56.000000 osw-0.8.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-21 16:05:56.000000 osw-0.8.0/docs/tools.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:06:29.898982 osw-0.8.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-21 16:05:56.000000 osw-0.8.0/examples/accounts.pwd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-21 16:05:56.000000 osw-0.8.0/examples/controller_logic.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-21 16:05:56.000000 osw-0.8.0/examples/create_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-21 16:05:56.000000 osw-0.8.0/examples/create_page_package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:06:29.902982 osw-0.8.0/examples/data_processing/
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-21 16:05:56.000000 osw-0.8.0/examples/data_processing/local_jsonpath_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-21 16:05:56.000000 osw-0.8.0/examples/database_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-05-21 16:05:56.000000 osw-0.8.0/examples/entity_manipulation.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-21 16:05:56.000000 osw-0.8.0/examples/load_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    15311 2023-05-21 16:05:56.000000 osw-0.8.0/examples/local_editing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-05-21 16:05:56.000000 osw-0.8.0/examples/ontology_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-05-21 16:05:56.000000 osw-0.8.0/examples/page_manipulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-21 16:05:56.000000 osw-0.8.0/examples/register_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-21 16:05:56.000000 osw-0.8.0/examples/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-21 16:05:56.000000 osw-0.8.0/examples/store_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-21 16:05:56.000000 osw-0.8.0/examples/update_local_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-21 16:05:56.000000 osw-0.8.0/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:06:29.874982 osw-0.8.0/nb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:06:29.902982 osw-0.8.0/nb/quantities/
--rw-r--r--   0 runner    (1001) docker     (123)   123529 2023-05-21 16:05:56.000000 osw-0.8.0/nb/quantities/Quantities.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:06:29.902982 osw-0.8.0/nb/quantities/archive/
--rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-05-21 16:05:56.000000 osw-0.8.0/nb/quantities/archive/Onto2Wiki_qudtQuantities.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   107607 2023-05-21 16:05:56.000000 osw-0.8.0/nb/quantities/archive/broader.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    59112 2023-05-21 16:05:56.000000 osw-0.8.0/nb/quantities/archive/buildDictionaryTest.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   152865 2023-05-21 16:05:56.000000 osw-0.8.0/nb/quantities/archive/httpRequest.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    18955 2023-05-21 16:05:56.000000 osw-0.8.0/nb/quantities/archive/idea.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    18386 2023-05-21 16:05:56.000000 osw-0.8.0/nb/quantities/archive/querys.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    31162 2023-05-21 16:05:56.000000 osw-0.8.0/nb/quantities/archive/searchRunaways.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:06:29.902982 osw-0.8.0/nb/translations/
--rw-r--r--   0 runner    (1001) docker     (123)   404547 2023-05-21 16:05:56.000000 osw-0.8.0/nb/translations/DeeplTranslate.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-21 16:05:56.000000 osw-0.8.0/nb/translations/JsObjectToJson.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-21 16:05:56.000000 osw-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-21 16:06:29.910982 osw-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-21 16:05:56.000000 osw-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:06:29.878982 osw-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:06:29.902982 osw-0.8.0/src/osw/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-21 16:05:56.000000 osw-0.8.0/src/osw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-21 16:05:56.000000 osw-0.8.0/src/osw/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:06:29.906982 osw-0.8.0/src/osw/controller/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-21 16:05:56.000000 osw-0.8.0/src/osw/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-05-21 16:05:56.000000 osw-0.8.0/src/osw/controller/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-21 16:05:56.000000 osw-0.8.0/src/osw/controller/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-05-21 16:05:56.000000 osw-0.8.0/src/osw/controller/page_package.py
--rw-r--r--   0 runner    (1001) docker     (123)    22113 2023-05-21 16:05:56.000000 osw-0.8.0/src/osw/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:06:29.906982 osw-0.8.0/src/osw/model/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-21 16:05:56.000000 osw-0.8.0/src/osw/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-05-21 16:05:56.000000 osw-0.8.0/src/osw/model/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    10555 2023-05-21 16:05:56.000000 osw-0.8.0/src/osw/model/page_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-21 16:05:56.000000 osw-0.8.0/src/osw/model/static.py
--rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-05-21 16:05:56.000000 osw-0.8.0/src/osw/sparql_client_smw.py
--rw-r--r--   0 runner    (1001) docker     (123)    37510 2023-05-21 16:05:56.000000 osw-0.8.0/src/osw/wiki_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    22013 2023-05-21 16:05:56.000000 osw-0.8.0/src/osw/wtsite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:06:29.906982 osw-0.8.0/src/osw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-21 16:06:29.000000 osw-0.8.0/src/osw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-21 16:06:29.000000 osw-0.8.0/src/osw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 16:06:29.000000 osw-0.8.0/src/osw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 16:06:29.000000 osw-0.8.0/src/osw.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-21 16:06:29.000000 osw-0.8.0/src/osw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-21 16:06:29.000000 osw-0.8.0/src/osw.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:06:29.906982 osw-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-21 16:05:56.000000 osw-0.8.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-21 16:05:56.000000 osw-0.8.0/tests/controller_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:06:29.906982 osw-0.8.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-05-21 16:05:56.000000 osw-0.8.0/tests/integration/db_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-21 16:05:56.000000 osw-0.8.0/tests/integration/login_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-21 16:05:56.000000 osw-0.8.0/tests/integration/store_and_load_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-21 16:05:56.000000 osw-0.8.0/tests/sparql_client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-21 16:05:56.000000 osw-0.8.0/tests/test_credential_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-21 16:05:56.000000 osw-0.8.0/tests/test_osl.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-21 16:05:56.000000 osw-0.8.0/tests/test_wiki_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-05-21 16:05:56.000000 osw-0.8.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:39:45.249094 osw-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-09 16:39:08.000000 osw-0.8.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:39:45.225094 osw-0.8.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:39:45.229094 osw-0.8.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-06-09 16:39:08.000000 osw-0.8.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-09 16:39:08.000000 osw-0.8.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-09 16:39:08.000000 osw-0.8.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-09 16:39:08.000000 osw-0.8.1/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-09 16:39:08.000000 osw-0.8.1/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-09 16:39:08.000000 osw-0.8.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-09 16:39:08.000000 osw-0.8.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-09 16:39:08.000000 osw-0.8.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-09 16:39:08.000000 osw-0.8.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-09 16:39:08.000000 osw-0.8.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)    13425 2023-06-09 16:39:08.000000 osw-0.8.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    32387 2023-06-09 16:39:08.000000 osw-0.8.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-06-09 16:39:45.249094 osw-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-09 16:39:08.000000 osw-0.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-09 16:39:08.000000 osw-0.8.1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:39:45.233094 osw-0.8.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-09 16:39:08.000000 osw-0.8.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:39:45.233094 osw-0.8.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-09 16:39:08.000000 osw-0.8.1/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-09 16:39:08.000000 osw-0.8.1/docs/auth.md
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-09 16:39:08.000000 osw-0.8.1/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-09 16:39:08.000000 osw-0.8.1/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10000 2023-06-09 16:39:08.000000 osw-0.8.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-09 16:39:08.000000 osw-0.8.1/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-09 16:39:08.000000 osw-0.8.1/docs/controller.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-09 16:39:08.000000 osw-0.8.1/docs/dev.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-09 16:39:08.000000 osw-0.8.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-09 16:39:08.000000 osw-0.8.1/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-09 16:39:08.000000 osw-0.8.1/docs/model.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-09 16:39:08.000000 osw-0.8.1/docs/osw.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-09 16:39:08.000000 osw-0.8.1/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-09 16:39:08.000000 osw-0.8.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-09 16:39:08.000000 osw-0.8.1/docs/tools.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:39:45.237094 osw-0.8.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-09 16:39:08.000000 osw-0.8.1/examples/accounts.pwd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-06-09 16:39:08.000000 osw-0.8.1/examples/controller_logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-09 16:39:08.000000 osw-0.8.1/examples/create_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-09 16:39:08.000000 osw-0.8.1/examples/create_page_package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:39:45.237094 osw-0.8.1/examples/data_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-09 16:39:08.000000 osw-0.8.1/examples/data_processing/local_jsonpath_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-09 16:39:08.000000 osw-0.8.1/examples/database_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-06-09 16:39:08.000000 osw-0.8.1/examples/entity_manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-09 16:39:08.000000 osw-0.8.1/examples/load_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15311 2023-06-09 16:39:08.000000 osw-0.8.1/examples/local_editing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-06-09 16:39:08.000000 osw-0.8.1/examples/ontology_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-06-09 16:39:08.000000 osw-0.8.1/examples/page_manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-09 16:39:08.000000 osw-0.8.1/examples/register_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-09 16:39:08.000000 osw-0.8.1/examples/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-09 16:39:08.000000 osw-0.8.1/examples/store_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-09 16:39:08.000000 osw-0.8.1/examples/update_local_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-09 16:39:08.000000 osw-0.8.1/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:39:45.225094 osw-0.8.1/nb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:39:45.237094 osw-0.8.1/nb/quantities/
+-rw-r--r--   0 runner    (1001) docker     (123)   123529 2023-06-09 16:39:08.000000 osw-0.8.1/nb/quantities/Quantities.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:39:45.237094 osw-0.8.1/nb/quantities/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-06-09 16:39:08.000000 osw-0.8.1/nb/quantities/archive/Onto2Wiki_qudtQuantities.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   107607 2023-06-09 16:39:08.000000 osw-0.8.1/nb/quantities/archive/broader.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    59112 2023-06-09 16:39:08.000000 osw-0.8.1/nb/quantities/archive/buildDictionaryTest.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   152865 2023-06-09 16:39:08.000000 osw-0.8.1/nb/quantities/archive/httpRequest.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    18955 2023-06-09 16:39:08.000000 osw-0.8.1/nb/quantities/archive/idea.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    18386 2023-06-09 16:39:08.000000 osw-0.8.1/nb/quantities/archive/querys.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    31162 2023-06-09 16:39:08.000000 osw-0.8.1/nb/quantities/archive/searchRunaways.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:39:45.241094 osw-0.8.1/nb/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)   404547 2023-06-09 16:39:08.000000 osw-0.8.1/nb/translations/DeeplTranslate.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-09 16:39:08.000000 osw-0.8.1/nb/translations/JsObjectToJson.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-09 16:39:08.000000 osw-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-09 16:39:45.253094 osw-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-09 16:39:08.000000 osw-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:39:45.225094 osw-0.8.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:39:45.241094 osw-0.8.1/src/osw/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-09 16:39:08.000000 osw-0.8.1/src/osw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-06-09 16:39:08.000000 osw-0.8.1/src/osw/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:39:45.245094 osw-0.8.1/src/osw/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-09 16:39:08.000000 osw-0.8.1/src/osw/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-06-09 16:39:08.000000 osw-0.8.1/src/osw/controller/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-09 16:39:08.000000 osw-0.8.1/src/osw/controller/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-06-09 16:39:08.000000 osw-0.8.1/src/osw/controller/page_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22113 2023-06-09 16:39:08.000000 osw-0.8.1/src/osw/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:39:45.249094 osw-0.8.1/src/osw/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-09 16:39:08.000000 osw-0.8.1/src/osw/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-06-09 16:39:08.000000 osw-0.8.1/src/osw/model/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-06-09 16:39:08.000000 osw-0.8.1/src/osw/model/page_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-09 16:39:08.000000 osw-0.8.1/src/osw/model/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-06-09 16:39:08.000000 osw-0.8.1/src/osw/sparql_client_smw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37510 2023-06-09 16:39:08.000000 osw-0.8.1/src/osw/wiki_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22013 2023-06-09 16:39:08.000000 osw-0.8.1/src/osw/wtsite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:39:45.245094 osw-0.8.1/src/osw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-06-09 16:39:45.000000 osw-0.8.1/src/osw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-09 16:39:45.000000 osw-0.8.1/src/osw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 16:39:45.000000 osw-0.8.1/src/osw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 16:39:44.000000 osw-0.8.1/src/osw.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-09 16:39:45.000000 osw-0.8.1/src/osw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-09 16:39:45.000000 osw-0.8.1/src/osw.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:39:45.249094 osw-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-09 16:39:08.000000 osw-0.8.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-09 16:39:08.000000 osw-0.8.1/tests/controller_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:39:45.249094 osw-0.8.1/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-06-09 16:39:08.000000 osw-0.8.1/tests/integration/db_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-09 16:39:08.000000 osw-0.8.1/tests/integration/login_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-09 16:39:08.000000 osw-0.8.1/tests/integration/store_and_load_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-09 16:39:08.000000 osw-0.8.1/tests/sparql_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-09 16:39:08.000000 osw-0.8.1/tests/test_credential_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-09 16:39:08.000000 osw-0.8.1/tests/test_osl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-09 16:39:08.000000 osw-0.8.1/tests/test_wiki_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-09 16:39:08.000000 osw-0.8.1/tox.ini
```

### Comparing `osw-0.8.0/.coveragerc` & `osw-0.8.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/.github/workflows/ci.yml` & `osw-0.8.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/.github/workflows/docs.yml` & `osw-0.8.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/.gitignore` & `osw-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/.pre-commit-config.yaml` & `osw-0.8.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/CHANGELOG.md` & `osw-0.8.1/CHANGELOG.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 # Changelog
 
-## Version v0.8.x (development)
+## Version v0.9.x (development)
+
+## Version v0.8.0
+
+- fix #18
+- fix #19
+
+## Version v0.8.0
 
 - Restructure package package creation
 - fix namespace mappings (e. g. for the SMW Property namespace)
 
 ## Version v0.7.x
 
 - add database controller
```

### Comparing `osw-0.8.0/CONTRIBUTING.md` & `osw-0.8.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/LICENSE.txt` & `osw-0.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/PKG-INFO` & `osw-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osw
-Version: 0.8.0
+Version: 0.8.1
 Summary: Python toolset for data processing, queries, wikicode generation and page manipulation
 Home-page: https://github.com/OpenSemanticLab/osw-python
 Author: "Simon Stier"
 Author-email: simon.stier@isc.fraunhofer.de
 License: AGPL-3.0-or-later
 Project-URL: Documentation, https://opensemanticlab.github.io/osw-python/
 Project-URL: Source, https://github.com/OpenSemanticLab/osw-python
```

### Comparing `osw-0.8.0/README.md` & `osw-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/docs/Makefile` & `osw-0.8.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/docs/conf.py` & `osw-0.8.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/docs/index.md` & `osw-0.8.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/examples/controller_logic.py` & `osw-0.8.1/examples/controller_logic.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/examples/create_page_package.py` & `osw-0.8.1/examples/create_page_package.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/examples/data_processing/local_jsonpath_queries.py` & `osw-0.8.1/examples/data_processing/local_jsonpath_queries.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/examples/database_access.py` & `osw-0.8.1/examples/database_access.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/examples/entity_manipulation.py` & `osw-0.8.1/examples/entity_manipulation.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/examples/load_entity.py` & `osw-0.8.1/examples/load_entity.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/examples/local_editing.py` & `osw-0.8.1/examples/local_editing.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/examples/ontology_import.py` & `osw-0.8.1/examples/ontology_import.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/examples/page_manipulation.py` & `osw-0.8.1/examples/page_manipulation.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/examples/register_model.py` & `osw-0.8.1/examples/register_model.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/examples/settings.json` & `osw-0.8.1/examples/settings.json`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/examples/store_entity.py` & `osw-0.8.1/examples/store_entity.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/examples/update_local_model.py` & `osw-0.8.1/examples/update_local_model.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/nb/quantities/Quantities.ipynb` & `osw-0.8.1/nb/quantities/Quantities.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/nb/quantities/archive/Onto2Wiki_qudtQuantities.ipynb` & `osw-0.8.1/nb/quantities/archive/Onto2Wiki_qudtQuantities.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/nb/quantities/archive/broader.ipynb` & `osw-0.8.1/nb/quantities/archive/broader.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/nb/quantities/archive/buildDictionaryTest.ipynb` & `osw-0.8.1/nb/quantities/archive/buildDictionaryTest.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/nb/quantities/archive/httpRequest.ipynb` & `osw-0.8.1/nb/quantities/archive/httpRequest.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/nb/quantities/archive/idea.ipynb` & `osw-0.8.1/nb/quantities/archive/idea.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/nb/quantities/archive/querys.ipynb` & `osw-0.8.1/nb/quantities/archive/querys.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/nb/quantities/archive/searchRunaways.ipynb` & `osw-0.8.1/nb/quantities/archive/searchRunaways.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/nb/translations/DeeplTranslate.ipynb` & `osw-0.8.1/nb/translations/DeeplTranslate.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/nb/translations/JsObjectToJson.ipynb` & `osw-0.8.1/nb/translations/JsObjectToJson.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/setup.cfg` & `osw-0.8.1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 package_dir = 
 	=src
 install_requires = 
 	pydantic
 	datamodel-code-generator==0.15.0
 	mwclient
 	mwparserfromhell
+	rdflib
+	PyLD
 	SPARQLWrapper
 	jsonpath-ng
 	numpy
 	pyyaml
 	pandas
 	typing_extensions
 	dataclasses
```

### Comparing `osw-0.8.0/setup.py` & `osw-0.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/src/osw/auth.py` & `osw-0.8.1/src/osw/auth.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/src/osw/controller/__init__.py` & `osw-0.8.1/src/osw/controller/__init__.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/src/osw/controller/database.py` & `osw-0.8.1/src/osw/controller/database.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/src/osw/controller/page_package.py` & `osw-0.8.1/src/osw/controller/page_package.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/src/osw/core.py` & `osw-0.8.1/src/osw/core.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/src/osw/model/entity.py` & `osw-0.8.1/src/osw/model/entity.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/src/osw/model/page_package.py` & `osw-0.8.1/src/osw/model/page_package.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 from pathlib import Path
-from typing import List, Optional, Union
+from typing import Dict, List, Optional, Union
 
 from pydantic import BaseModel
 
 
 class PagePackagePageSlot(BaseModel):
     url: Optional[str]
     urlPath: Optional[str]
@@ -34,15 +34,15 @@
     fileURL: Optional[str]
     """ If this is a file/image page (i.e. with a "namespace" value of "NS_FILE"), this
     parameter holds the actual file, while the "url" parameter holds a URL containing
     the text contents of the wiki page."""
     fileURLPath: Optional[str]
     """Similar to fileURL, but gets appended to the baseURL value set for the package,
     if one was set."""
-    slots: dict[str, PagePackagePageSlot]
+    slots: Dict[str, PagePackagePageSlot]
     """Slots used to store data, e.g., the main slot, storing the wiki text of the
     page. Other slots could be jsondata, jsonschema etc."""
 
 
 class PagePackageNamespaceSettings(BaseModel):
     """The group of settings, per namespace, that together dictate the structure of the
     directory.
@@ -151,15 +151,15 @@
     author: Optional[List[str]]
     """The default author."""
     language: Optional[str] = "en"
     """The default language for all defined packages, using the
     (usually) two-letter IETF language tag for that language."""
     licenseName: Optional[str] = "CC BY-NC 4.0"
     """The default license under which these packages are published."""
-    packages: dict[str, PagePackage]
+    packages: Dict[str, PagePackage]
     """Holds the set of packages, with the package name as the key
     and the set of package parameters as the values."""
 
 
 class PagePackageConfig(BaseModel):
     """A config for a page package"""
```

### Comparing `osw-0.8.0/src/osw/model/static.py` & `osw-0.8.1/src/osw/model/static.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/src/osw/sparql_client_smw.py` & `osw-0.8.1/src/osw/sparql_client_smw.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/src/osw/wiki_tools.py` & `osw-0.8.1/src/osw/wiki_tools.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/src/osw/wtsite.py` & `osw-0.8.1/src/osw/wtsite.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/src/osw.egg-info/PKG-INFO` & `osw-0.8.1/src/osw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osw
-Version: 0.8.0
+Version: 0.8.1
 Summary: Python toolset for data processing, queries, wikicode generation and page manipulation
 Home-page: https://github.com/OpenSemanticLab/osw-python
 Author: "Simon Stier"
 Author-email: simon.stier@isc.fraunhofer.de
 License: AGPL-3.0-or-later
 Project-URL: Documentation, https://opensemanticlab.github.io/osw-python/
 Project-URL: Source, https://github.com/OpenSemanticLab/osw-python
```

### Comparing `osw-0.8.0/src/osw.egg-info/SOURCES.txt` & `osw-0.8.1/src/osw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/tests/conftest.py` & `osw-0.8.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/tests/controller_mixin.py` & `osw-0.8.1/tests/controller_mixin.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/tests/integration/db_test.py` & `osw-0.8.1/tests/integration/db_test.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/tests/integration/store_and_load_test.py` & `osw-0.8.1/tests/integration/store_and_load_test.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/tests/sparql_client_test.py` & `osw-0.8.1/tests/sparql_client_test.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/tests/test_credential_manager.py` & `osw-0.8.1/tests/test_credential_manager.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.0/tox.ini` & `osw-0.8.1/tox.ini`

 * *Files identical despite different names*

