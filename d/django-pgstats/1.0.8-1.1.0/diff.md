# Comparing `tmp/django-pgstats-1.0.8.tar.gz` & `tmp/django_pgstats-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pgstats-1.0.8.tar", max compression
+gzip compressed data, was "django_pgstats-1.1.0.tar", max compression
```

## Comparing `django-pgstats-1.0.8.tar` & `django_pgstats-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1456 2022-10-14 16:27:03.723368 django-pgstats-1.0.8/LICENSE
--rw-r--r--   0        0        0     1407 2022-10-14 16:27:03.723368 django-pgstats-1.0.8/README.rst
--rw-r--r--   0        0        0       67 2022-10-14 16:27:03.723368 django-pgstats-1.0.8/pgstats/__init__.py
--rw-r--r--   0        0        0        0 2022-10-14 16:27:03.727368 django-pgstats-1.0.8/pgstats/management/__init__.py
--rw-r--r--   0        0        0        0 2022-10-14 16:27:03.727368 django-pgstats-1.0.8/pgstats/management/commands/__init__.py
--rw-r--r--   0        0        0      319 2022-10-14 16:27:03.727368 django-pgstats-1.0.8/pgstats/management/commands/snapshot_pgstats.py
--rw-r--r--   0        0        0     1639 2022-10-14 16:27:03.727368 django-pgstats-1.0.8/pgstats/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-10-14 16:27:03.727368 django-pgstats-1.0.8/pgstats/migrations/__init__.py
--rw-r--r--   0        0        0     1951 2022-10-14 16:27:03.727368 django-pgstats-1.0.8/pgstats/models.py
--rw-r--r--   0        0        0      152 2022-10-14 16:27:03.727368 django-pgstats-1.0.8/pgstats/version.py
--rw-r--r--   0        0        0     2260 2022-10-14 16:27:46.475344 django-pgstats-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     2331 1970-01-01 00:00:00.000000 django-pgstats-1.0.8/setup.py
--rw-r--r--   0        0        0     2824 1970-01-01 00:00:00.000000 django-pgstats-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1456 2023-06-09 00:36:07.733619 django_pgstats-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1548 2023-06-09 00:36:07.733619 django_pgstats-1.1.0/README.rst
+-rw-r--r--   0        0        0       67 2023-06-09 00:36:07.737619 django_pgstats-1.1.0/pgstats/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 00:36:07.737619 django_pgstats-1.1.0/pgstats/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 00:36:07.737619 django_pgstats-1.1.0/pgstats/management/commands/__init__.py
+-rw-r--r--   0        0        0      319 2023-06-09 00:36:07.737619 django_pgstats-1.1.0/pgstats/management/commands/snapshot_pgstats.py
+-rw-r--r--   0        0        0     1639 2023-06-09 00:36:07.737619 django_pgstats-1.1.0/pgstats/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-09 00:36:07.737619 django_pgstats-1.1.0/pgstats/migrations/__init__.py
+-rw-r--r--   0        0        0     1971 2023-06-09 00:36:07.737619 django_pgstats-1.1.0/pgstats/models.py
+-rw-r--r--   0        0        0      152 2023-06-09 00:36:07.737619 django_pgstats-1.1.0/pgstats/version.py
+-rw-r--r--   0        0        0     2301 2023-06-09 00:36:39.405583 django_pgstats-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2816 1970-01-01 00:00:00.000000 django_pgstats-1.1.0/PKG-INFO
```

### Comparing `django-pgstats-1.0.8/LICENSE` & `django_pgstats-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-pgstats-1.0.8/README.rst` & `django_pgstats-1.1.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 as [Celery](http://www.celeryproject.org/).
 
 Stats are stored as JSON fields in the respective `IndexStats` and `TableStats`
 models. Each key in the JSON field is in the format of
 ``{schema}.{table}`` for table stats or ``{schema}.{table}.{index}`` for index
 stats.
 
+Compatibility
+=============
+
+``django-pgstats`` is compatible with Python 3.7 - 3.11, Django 3.2 - 4.2, Psycopg 2 - 3 and Postgres 12 - 15.
+
 Documentation
 =============
 
 `View the django-pgstats docs here
 <https://django-pgstats.readthedocs.io/>`_.
 
 Installation
```

### Comparing `django-pgstats-1.0.8/pgstats/migrations/0001_initial.py` & `django_pgstats-1.1.0/pgstats/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-pgstats-1.0.8/pgstats/models.py` & `django_pgstats-1.1.0/pgstats/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from django.db import connection
 from django.db import models
 
 
 # Django>=3.1 changes the location of JSONField
 if django.VERSION >= (3, 1):
     from django.db.models import JSONField as DjangoJSONField
-else:
+else:  # pragma: no cover
     from django.contrib.postgres.fields import JSONField as DjangoJSONField
 
 
 class JSONField(DjangoJSONField):
     """
     Creates a consistent import path for JSONField regardless of Django
     version.
```

### Comparing `django-pgstats-1.0.8/pyproject.toml` & `django_pgstats-1.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -25,30 +25,31 @@
 name = "django-pgstats"
 packages = [
   { include = "pgstats" }
 ]
 exclude = [
   "*/tests/"
 ]
-version = "1.0.8"
+version = "1.1.0"
 description = "Commands and models for tracking internal postgres stats."
 authors = ["Wes Kendall", "Tómas Árni Jónasson"]
 classifiers = [
   "Framework :: Django",
-  "Framework :: Django :: 2.2",
   "Framework :: Django :: 3.2",
   "Framework :: Django :: 4.0",
   "Framework :: Django :: 4.1",
+  "Framework :: Django :: 4.2",
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3 :: Only",
   "Framework :: Django",
 ]
 license = "BSD-3-Clause"
 readme = "README.rst"
 homepage = "https://github.com/Opus10/django-pgstats"
 repository = "https://github.com/Opus10/django-pgstats"
@@ -64,21 +65,21 @@
 dj-database-url = "0.5.0"
 flake8 = "3.9.2"
 flake8-bugbear = "22.1.11"
 flake8-comprehensions = "3.8.0"
 flake8-import-order = "0.18.1"
 flake8-logging-format = "0.6.0"
 flake8-mutable = "1.2.0"
-git-tidy = "1.1.2"
+git-tidy = "1.2.0"
 myst-parser = "0.18.0"
 packaging = ">=19.2"
 pip = "*"
-poetry-core = "1.1.0rc3"
+poetry-core = "1.3.2"
 pre-commit = "2.13.0"
-psycopg2-binary = "2.9.3"
+psycopg2-binary = "2.9.6"
 pytest = "7.0.0"
 pytest-cov = "3.0.0"
 pytest-dotenv = "0.5.2"
 pytest-django = "4.5.2"
 requests = "2.25.1"
 Sphinx = "4.4.0"
 sphinx-rtd-theme = "1.0.0"
```

### Comparing `django-pgstats-1.0.8/PKG-INFO` & `django_pgstats-1.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 Metadata-Version: 2.1
 Name: django-pgstats
-Version: 1.0.8
+Version: 1.1.0
 Summary: Commands and models for tracking internal postgres stats.
 Home-page: https://github.com/Opus10/django-pgstats
 License: BSD-3-Clause
 Author: Wes Kendall
 Requires-Python: >=3.7.0,<4
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: django (>=2)
-Requires-Dist: importlib_metadata (>=4); python_version >= "3.7" and python_version < "3.8"
+Requires-Dist: importlib_metadata (>=4) ; python_version >= "3.7" and python_version < "3.8"
 Project-URL: Documentation, https://django-pgstats.readthedocs.io
 Project-URL: Repository, https://github.com/Opus10/django-pgstats
 Description-Content-Type: text/x-rst
 
 django-pgstats
 ########################################################################
 
@@ -45,14 +42,19 @@
 as [Celery](http://www.celeryproject.org/).
 
 Stats are stored as JSON fields in the respective `IndexStats` and `TableStats`
 models. Each key in the JSON field is in the format of
 ``{schema}.{table}`` for table stats or ``{schema}.{table}.{index}`` for index
 stats.
 
+Compatibility
+=============
+
+``django-pgstats`` is compatible with Python 3.7 - 3.11, Django 3.2 - 4.2, Psycopg 2 - 3 and Postgres 12 - 15.
+
 Documentation
 =============
 
 `View the django-pgstats docs here
 <https://django-pgstats.readthedocs.io/>`_.
 
 Installation
```

