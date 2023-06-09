# Comparing `tmp/fractal_repositories-0.0.2.tar.gz` & `tmp/fractal_repositories-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_repositories-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fractal_repositories-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fractal_repositories-0.0.2.tar` & `fractal_repositories-0.0.3.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0      187 2023-06-08 07:39:25.673841 fractal_repositories-0.0.2/.coveragerc
--rw-r--r--   0        0        0      100 2023-06-08 07:39:25.673841 fractal_repositories-0.0.2/.flake8
--rw-r--r--   0        0        0      945 2023-06-08 07:39:25.673841 fractal_repositories-0.0.2/.github/workflows/build.yml
--rw-r--r--   0        0        0      662 2023-06-08 07:39:25.673841 fractal_repositories-0.0.2/.github/workflows/publish.yml
--rw-r--r--   0        0        0      832 2023-06-08 07:39:25.673841 fractal_repositories-0.0.2/.gitignore
--rw-r--r--   0        0        0      161 2023-06-08 07:39:25.673841 fractal_repositories-0.0.2/.isort.cfg
--rw-r--r--   0        0        0       43 2023-06-08 07:39:25.673841 fractal_repositories-0.0.2/.mypy.ini
--rw-r--r--   0        0        0     1691 2023-06-08 07:39:25.673841 fractal_repositories-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1075 2023-06-08 07:39:25.673841 fractal_repositories-0.0.2/LICENSE
--rw-r--r--   0        0        0     1557 2023-06-08 07:39:25.673841 fractal_repositories-0.0.2/Makefile
--rw-r--r--   0        0        0     2276 2023-06-08 07:39:25.673841 fractal_repositories-0.0.2/README.md
--rw-r--r--   0        0        0      780 2023-06-08 07:39:25.673841 fractal_repositories-0.0.2/align_version.py
--rw-r--r--   0        0        0      182 2023-06-08 07:39:25.673841 fractal_repositories-0.0.2/fractal_repositories/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 07:39:25.673841 fractal_repositories-0.0.2/fractal_repositories/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 07:39:25.673841 fractal_repositories-0.0.2/fractal_repositories/contrib/django/__init__.py
--rw-r--r--   0        0        0     3291 2023-06-08 07:39:25.673841 fractal_repositories-0.0.2/fractal_repositories/contrib/django/mixins.py
--rw-r--r--   0        0        0        0 2023-06-08 07:39:25.673841 fractal_repositories-0.0.2/fractal_repositories/contrib/elastic/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 07:39:25.673841 fractal_repositories-0.0.2/fractal_repositories/contrib/gcp/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 07:39:25.673841 fractal_repositories-0.0.2/fractal_repositories/contrib/gcp/firestore/__init__.py
--rw-r--r--   0        0        0     5051 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/fractal_repositories/contrib/gcp/firestore/mixins.py
--rw-r--r--   0        0        0        0 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/fractal_repositories/contrib/mongo/__init__.py
--rw-r--r--   0        0        0     3253 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/fractal_repositories/contrib/mongo/mixins.py
--rw-r--r--   0        0        0        0 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/fractal_repositories/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0    11960 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/fractal_repositories/contrib/sqlalchemy/mixins.py
--rw-r--r--   0        0        0        0 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/fractal_repositories/core/__init__.py
--rw-r--r--   0        0        0     1451 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/fractal_repositories/core/entity.py
--rw-r--r--   0        0        0     2434 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/fractal_repositories/core/repositories.py
--rw-r--r--   0        0        0      343 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/fractal_repositories/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/fractal_repositories/mixins/__init__.py
--rw-r--r--   0        0        0     1219 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/fractal_repositories/mixins/external_data_inmemory_repository_mixin.py
--rw-r--r--   0        0        0     2965 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/fractal_repositories/mixins/file_repository_mixin.py
--rw-r--r--   0        0        0      957 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/fractal_repositories/mixins/filter_repository_mixin.py
--rw-r--r--   0        0        0     3044 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/fractal_repositories/mixins/inmemory_repository_mixin.py
--rw-r--r--   0        0        0       77 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/fractal_repositories/py.typed
--rw-r--r--   0        0        0        0 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/fractal_repositories/utils/__init__.py
--rw-r--r--   0        0        0     2299 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/fractal_repositories/utils/cached_repository.py
--rw-r--r--   0        0        0     2381 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/fractal_repositories/utils/distributed_read_repository.py
--rw-r--r--   0        0        0      636 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/fractal_repositories/utils/json_encoder.py
--rw-r--r--   0        0        0      235 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/poetry.lock
--rw-r--r--   0        0        0     1667 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       69 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/setup.py
--rw-r--r--   0        0        0        0 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0       37 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/contrib/__init__.py
--rw-r--r--   0        0        0     4177 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/contrib/test_django.py
--rw-r--r--   0        0        0     4438 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/contrib/test_firestore.py
--rw-r--r--   0        0        0     4100 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/contrib/test_mongo.py
--rw-r--r--   0        0        0    12220 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/contrib/test_sqlalchemy.py
--rw-r--r--   0        0        0        0 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/core/__init__.py
--rw-r--r--   0        0        0     3168 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/core/test_models.py
--rw-r--r--   0        0        0     1046 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/core/test_repositories.py
--rw-r--r--   0        0        0      232 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/fixtures/__init__.py
--rw-r--r--   0        0        0     2164 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/fixtures/django/__init__.py
--rw-r--r--   0        0        0      643 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/fixtures/django/models.py
--rw-r--r--   0        0        0     1126 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/fixtures/firestore.py
--rw-r--r--   0        0        0      888 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/fixtures/mongo.py
--rw-r--r--   0        0        0     6786 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/fixtures/repositories.py
--rw-r--r--   0        0        0     7674 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/fixtures/sqlalchemy.py
--rw-r--r--   0        0        0        0 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/mixins/__init__.py
--rw-r--r--   0        0        0     1154 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/mixins/test_external_data_inmemory_repository_mixin.py
--rw-r--r--   0        0        0      601 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/mixins/test_file_file_repository_mixin.py
--rw-r--r--   0        0        0     3764 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/mixins/test_file_repository_mixin.py
--rw-r--r--   0        0        0     3542 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/mixins/test_filter_repository_mixin.py
--rw-r--r--   0        0        0      827 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/mixins/test_inmemory_file_repository_mixin.py
--rw-r--r--   0        0        0     3150 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/mixins/test_inmemory_repository_mixin.py
--rw-r--r--   0        0        0        0 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/utils/__init__.py
--rw-r--r--   0        0        0     4025 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/utils/test_cached_repository.py
--rw-r--r--   0        0        0     2381 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/utils/test_distributed_read_repository.py
--rw-r--r--   0        0        0      996 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/utils/test_json_encoder.py
--rw-r--r--   0        0        0      826 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tox.ini
--rw-r--r--   0        0        0     3195 1970-01-01 00:00:00.000000 fractal_repositories-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      187 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/.coveragerc
+-rw-r--r--   0        0        0      100 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/.flake8
+-rw-r--r--   0        0        0      945 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/.github/workflows/build.yml
+-rw-r--r--   0        0        0      662 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      832 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/.gitignore
+-rw-r--r--   0        0        0      161 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/.isort.cfg
+-rw-r--r--   0        0        0       43 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/.mypy.ini
+-rw-r--r--   0        0        0     1691 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1075 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1557 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/Makefile
+-rw-r--r--   0        0        0     2276 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/README.md
+-rw-r--r--   0        0        0      780 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/align_version.py
+-rw-r--r--   0        0        0      182 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/fractal_repositories/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/fractal_repositories/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/fractal_repositories/contrib/django/__init__.py
+-rw-r--r--   0        0        0     3291 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/fractal_repositories/contrib/django/mixins.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/fractal_repositories/contrib/elastic/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/fractal_repositories/contrib/gcp/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/fractal_repositories/contrib/gcp/firestore/__init__.py
+-rw-r--r--   0        0        0     5318 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/fractal_repositories/contrib/gcp/firestore/mixins.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/fractal_repositories/contrib/mongo/__init__.py
+-rw-r--r--   0        0        0     3253 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/fractal_repositories/contrib/mongo/mixins.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:54:55.650446 fractal_repositories-0.0.3/fractal_repositories/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0    11960 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/fractal_repositories/contrib/sqlalchemy/mixins.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/fractal_repositories/core/__init__.py
+-rw-r--r--   0        0        0     1466 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/fractal_repositories/core/entity.py
+-rw-r--r--   0        0        0     2434 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/fractal_repositories/core/repositories.py
+-rw-r--r--   0        0        0      343 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/fractal_repositories/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/fractal_repositories/mixins/__init__.py
+-rw-r--r--   0        0        0     1219 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/fractal_repositories/mixins/external_data_inmemory_repository_mixin.py
+-rw-r--r--   0        0        0     2965 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/fractal_repositories/mixins/file_repository_mixin.py
+-rw-r--r--   0        0        0      957 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/fractal_repositories/mixins/filter_repository_mixin.py
+-rw-r--r--   0        0        0     3044 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/fractal_repositories/mixins/inmemory_repository_mixin.py
+-rw-r--r--   0        0        0       77 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/fractal_repositories/py.typed
+-rw-r--r--   0        0        0        0 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/fractal_repositories/utils/__init__.py
+-rw-r--r--   0        0        0     2299 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/fractal_repositories/utils/cached_repository.py
+-rw-r--r--   0        0        0     2381 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/fractal_repositories/utils/distributed_read_repository.py
+-rw-r--r--   0        0        0      636 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/fractal_repositories/utils/json_encoder.py
+-rw-r--r--   0        0        0      235 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/poetry.lock
+-rw-r--r--   0        0        0     1667 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/setup.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0       37 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/contrib/__init__.py
+-rw-r--r--   0        0        0     4177 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/contrib/test_django.py
+-rw-r--r--   0        0        0     4438 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/contrib/test_firestore.py
+-rw-r--r--   0        0        0     4100 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/contrib/test_mongo.py
+-rw-r--r--   0        0        0    12220 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/contrib/test_sqlalchemy.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/core/__init__.py
+-rw-r--r--   0        0        0     3168 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/core/test_models.py
+-rw-r--r--   0        0        0     1046 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/core/test_repositories.py
+-rw-r--r--   0        0        0      232 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     2164 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/fixtures/django/__init__.py
+-rw-r--r--   0        0        0      643 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/fixtures/django/models.py
+-rw-r--r--   0        0        0     1144 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/fixtures/firestore.py
+-rw-r--r--   0        0        0      898 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/fixtures/mongo.py
+-rw-r--r--   0        0        0     6786 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/fixtures/repositories.py
+-rw-r--r--   0        0        0     7674 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/fixtures/sqlalchemy.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/mixins/__init__.py
+-rw-r--r--   0        0        0     1154 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/mixins/test_external_data_inmemory_repository_mixin.py
+-rw-r--r--   0        0        0      601 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/mixins/test_file_file_repository_mixin.py
+-rw-r--r--   0        0        0     3764 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/mixins/test_file_repository_mixin.py
+-rw-r--r--   0        0        0     3542 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/mixins/test_filter_repository_mixin.py
+-rw-r--r--   0        0        0      827 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/mixins/test_inmemory_file_repository_mixin.py
+-rw-r--r--   0        0        0     3150 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/mixins/test_inmemory_repository_mixin.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/utils/__init__.py
+-rw-r--r--   0        0        0     4025 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/utils/test_cached_repository.py
+-rw-r--r--   0        0        0     2381 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/utils/test_distributed_read_repository.py
+-rw-r--r--   0        0        0      996 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tests/utils/test_json_encoder.py
+-rw-r--r--   0        0        0      826 2023-06-09 06:54:55.658446 fractal_repositories-0.0.3/tox.ini
+-rw-r--r--   0        0        0     3195 1970-01-01 00:00:00.000000 fractal_repositories-0.0.3/PKG-INFO
```

### Comparing `fractal_repositories-0.0.2/.github/workflows/build.yml` & `fractal_repositories-0.0.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.2/.github/workflows/publish.yml` & `fractal_repositories-0.0.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.2/.gitignore` & `fractal_repositories-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.2/.pre-commit-config.yaml` & `fractal_repositories-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.2/LICENSE` & `fractal_repositories-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.2/Makefile` & `fractal_repositories-0.0.3/Makefile`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.2/README.md` & `fractal_repositories-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.2/align_version.py` & `fractal_repositories-0.0.3/align_version.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.2/fractal_repositories/contrib/django/mixins.py` & `fractal_repositories-0.0.3/fractal_repositories/contrib/django/mixins.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.2/fractal_repositories/contrib/gcp/firestore/mixins.py` & `fractal_repositories-0.0.3/fractal_repositories/contrib/gcp/firestore/mixins.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from datetime import date
-from typing import Iterator, Optional, Union
+from typing import Iterable, Iterator, Union
 
 from fractal_specifications.contrib.google_firestore.specifications import (
     FirestoreSpecificationBuilder,
 )
 from fractal_specifications.generic.specification import Specification
-from google.cloud.firestore_v1 import Client, Query
+from google.cloud.firestore_v1 import Client, DocumentSnapshot, Query
 from google.cloud.firestore_v1.base_collection import BaseCollectionReference
 from google.cloud.firestore_v1.base_query import BaseQuery
 
-from fractal_repositories.core.entity import Entity
 from fractal_repositories.core.repositories import EntityType, Repository
 
 
 class FirestoreClient(object):
     instance = None
 
     def __new__(cls, *args, **kwargs):
@@ -50,22 +49,20 @@
 
 
 class FirestoreRepositoryMixin(Repository[EntityType]):
     """
     https://github.com/GoogleCloudPlatform/python-docs-samples/blob/46fa5a588858021ea32350584a4ee178cd7c1f33/firestore/cloud-client/snippets.py#L62-L66
     """
 
-    entity: EntityType = Entity
-
     def __init__(self, collection: str = "", *, collection_prefix: str = ""):
         super(FirestoreRepositoryMixin, self).__init__()
 
         client: Client = FirestoreClient().get_firestore_client()
-        if not collection:
-            collection = self.entity.__name__
+        if not collection and self.entity:
+            collection = self.entity.__name__  # type: ignore
         if collection_prefix:
             collection = "-".join([collection_prefix, collection])
         self.collection = client.collection(collection.lower().replace(" ", "-"))
 
     def add(self, entity: EntityType) -> EntityType:
         doc_ref = self.collection.document(entity.id)
         doc_ref.set(entity.asdict(skip_types=(date,)))
@@ -78,29 +75,39 @@
             doc_ref.set(entity.asdict(skip_types=(date,)))
             return entity
         elif upsert:
             return self.add(entity)
         raise self._object_not_found()
 
     def remove_one(self, specification: Specification):
-        entity = self.find_one(specification)
-        self.collection.document(entity.id).delete()
+        if entity := self.find_one(specification):
+            self.collection.document(entity.id).delete()
+
+    @staticmethod
+    def _get_collection_stream(collection) -> Iterable[DocumentSnapshot]:
+        for i in collection.stream():
+            yield i
 
-    def find_one(self, specification: Specification) -> Optional[EntityType]:
+    def find_one(self, specification: Specification) -> EntityType:
         _filter = FirestoreSpecificationBuilder.build(specification)
         collection: Union[BaseCollectionReference, BaseQuery] = self.collection
         if _filter:
             if isinstance(_filter, list):
                 for f in _filter:
                     collection = collection.where(*f)
             else:
                 collection = collection.where(*_filter)
+
+        def _spec_filter(i: DocumentSnapshot):
+            if data := i.to_dict():
+                return specification.is_satisfied_by(AttrDict(**data))
+
         for doc in filter(
-            lambda i: specification.is_satisfied_by(AttrDict(**i.to_dict())),
-            collection.stream(),
+            _spec_filter,
+            self._get_collection_stream(collection),
         ):
             return self.entity.from_dict(doc.to_dict())
         raise self._object_not_found()
 
     def find(
         self,
         specification: Specification = None,
@@ -125,16 +132,16 @@
         order_by = order_by or self.order_by
         if order_by:
             collection = collection.order_by(order_by, direction=direction)
 
         if limit:
             if offset and (last := list(collection.limit(offset).stream())[-1]):
                 collection = collection.start_after(
-                    {order_by: last.to_dict().get(order_by)}
+                    {order_by: (last.to_dict() or {}).get(order_by)}
                 ).limit(limit)
             else:
                 collection = collection.limit(limit)
-        for doc in collection.stream():
+        for doc in self._get_collection_stream(collection):
             yield self.entity.from_dict(doc.to_dict())
 
     def is_healthy(self) -> bool:
         return True
```

### Comparing `fractal_repositories-0.0.2/fractal_repositories/contrib/mongo/mixins.py` & `fractal_repositories-0.0.3/fractal_repositories/contrib/mongo/mixins.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.2/fractal_repositories/contrib/sqlalchemy/mixins.py` & `fractal_repositories-0.0.3/fractal_repositories/contrib/sqlalchemy/mixins.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.2/fractal_repositories/core/entity.py` & `fractal_repositories-0.0.3/fractal_repositories/core/entity.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         if skip_types is None:
             skip_types = []
         field_names = set(
             f.name for f in fields(self) if f.name not in self.calculated_fields()
         )
 
         def _asdict(v):
-            if isinstance(v, Entity):
+            if issubclass(type(v), (Model, Entity)):
                 return v.asdict(skip_types=skip_types)
             elif isinstance(v, list) and list not in skip_types:
                 return [_asdict(i) for i in v]
             elif isinstance(v, Decimal) and Decimal not in skip_types:
                 return f"{v:.2f}"
             elif isinstance(v, date) and date not in skip_types:
                 return v.isoformat()
```

### Comparing `fractal_repositories-0.0.2/fractal_repositories/core/repositories.py` & `fractal_repositories-0.0.3/fractal_repositories/core/repositories.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.2/fractal_repositories/mixins/external_data_inmemory_repository_mixin.py` & `fractal_repositories-0.0.3/fractal_repositories/mixins/external_data_inmemory_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.2/fractal_repositories/mixins/file_repository_mixin.py` & `fractal_repositories-0.0.3/fractal_repositories/mixins/file_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.2/fractal_repositories/mixins/filter_repository_mixin.py` & `fractal_repositories-0.0.3/fractal_repositories/mixins/filter_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.2/fractal_repositories/mixins/inmemory_repository_mixin.py` & `fractal_repositories-0.0.3/fractal_repositories/mixins/inmemory_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.2/fractal_repositories/utils/cached_repository.py` & `fractal_repositories-0.0.3/fractal_repositories/utils/cached_repository.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.2/fractal_repositories/utils/distributed_read_repository.py` & `fractal_repositories-0.0.3/fractal_repositories/utils/distributed_read_repository.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.2/fractal_repositories/utils/json_encoder.py` & `fractal_repositories-0.0.3/fractal_repositories/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.2/pyproject.toml` & `fractal_repositories-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-repositories"
-version = "0.0.2"
+version = "0.0.3"
 description = "Fractal Repositories is an implementation of the repository pattern for building SOLID logic for your Python applications."
 authors = ["Douwe van der Meij <douwe@karibu-online.nl>"]
 
 [build-system]
 requires = ["flit_core >=2,<4"]
 build-backend = "flit_core.buildapi"
```

### Comparing `fractal_repositories-0.0.2/tests/contrib/test_django.py` & `fractal_repositories-0.0.3/tests/contrib/test_django.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.2/tests/contrib/test_firestore.py` & `fractal_repositories-0.0.3/tests/contrib/test_firestore.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.2/tests/contrib/test_mongo.py` & `fractal_repositories-0.0.3/tests/contrib/test_mongo.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.2/tests/contrib/test_sqlalchemy.py` & `fractal_repositories-0.0.3/tests/contrib/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.2/tests/core/test_models.py` & `fractal_repositories-0.0.3/tests/core/test_models.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.2/tests/core/test_repositories.py` & `fractal_repositories-0.0.3/tests/core/test_repositories.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.2/tests/fixtures/django/__init__.py` & `fractal_repositories-0.0.3/tests/fixtures/django/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.2/tests/fixtures/django/models.py` & `fractal_repositories-0.0.3/tests/fixtures/django/models.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.2/tests/fixtures/firestore.py` & `fractal_repositories-0.0.3/tests/fixtures/firestore.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 
 
 @pytest.fixture
 def firestore_test_model():
     from fractal_repositories.core.entity import Entity
 
     @dataclass
-    class TestModel(Entity):
+    class TestModelFirestore(Entity):
         id: str
         name: str = "test"
         description: str = "test"
 
-    return TestModel
+    return TestModelFirestore
 
 
 @pytest.fixture
 def firebase_client_mock(mocker):
     from mockfirestore import MockFirestore  # type: ignore
 
     mocker.patch("firebase_admin.firestore.client", lambda: MockFirestore())
```

### Comparing `fractal_repositories-0.0.2/tests/fixtures/mongo.py` & `fractal_repositories-0.0.3/tests/fixtures/mongo.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 
 
 @pytest.fixture
 def mongo_test_model():
     from fractal_repositories.core.entity import Entity
 
     @dataclass
-    class TestModel(Entity):
+    class TestModelMongo(Entity):
         id: str
         name: str = "test"
         description: str = "test"
 
-    return TestModel
+    return TestModelMongo
 
 
 @pytest.fixture
 def mongo_test_repository(mongo_test_model):
     from fractal_repositories.contrib.mongo.mixins import MongoRepositoryMixin
     from fractal_repositories.core.repositories import Repository
```

### Comparing `fractal_repositories-0.0.2/tests/fixtures/repositories.py` & `fractal_repositories-0.0.3/tests/fixtures/repositories.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.2/tests/fixtures/sqlalchemy.py` & `fractal_repositories-0.0.3/tests/fixtures/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.2/tests/mixins/test_external_data_inmemory_repository_mixin.py` & `fractal_repositories-0.0.3/tests/mixins/test_external_data_inmemory_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.2/tests/mixins/test_file_file_repository_mixin.py` & `fractal_repositories-0.0.3/tests/mixins/test_file_file_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.2/tests/mixins/test_file_repository_mixin.py` & `fractal_repositories-0.0.3/tests/mixins/test_file_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.2/tests/mixins/test_filter_repository_mixin.py` & `fractal_repositories-0.0.3/tests/mixins/test_filter_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.2/tests/mixins/test_inmemory_file_repository_mixin.py` & `fractal_repositories-0.0.3/tests/mixins/test_inmemory_file_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.2/tests/mixins/test_inmemory_repository_mixin.py` & `fractal_repositories-0.0.3/tests/mixins/test_inmemory_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.2/tests/utils/test_cached_repository.py` & `fractal_repositories-0.0.3/tests/utils/test_cached_repository.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.2/tests/utils/test_distributed_read_repository.py` & `fractal_repositories-0.0.3/tests/utils/test_distributed_read_repository.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.2/tests/utils/test_json_encoder.py` & `fractal_repositories-0.0.3/tests/utils/test_json_encoder.py`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.2/tox.ini` & `fractal_repositories-0.0.3/tox.ini`

 * *Files identical despite different names*

### Comparing `fractal_repositories-0.0.2/PKG-INFO` & `fractal_repositories-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-repositories
-Version: 0.0.2
+Version: 0.0.3
 Summary: Fractal Repositories is an implementation of the repository pattern of Domain Driven Design (DDD) for building SOLID logic for your Python applications.
 Home-page: https://github.com/douwevandermeij/fractal-repositories
 Author: Douwe van der Meij
 Author-email: douwe@karibu-online.nl
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
```

