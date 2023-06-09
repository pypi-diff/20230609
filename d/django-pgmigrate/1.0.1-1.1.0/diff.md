# Comparing `tmp/django-pgmigrate-1.0.1.tar.gz` & `tmp/django_pgmigrate-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pgmigrate-1.0.1.tar", max compression
+gzip compressed data, was "django_pgmigrate-1.1.0.tar", max compression
```

## Comparing `django-pgmigrate-1.0.1.tar` & `django_pgmigrate-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     1456 2022-11-04 02:32:04.242143 django-pgmigrate-1.0.1/LICENSE
--rw-r--r--   0        0        0     2842 2022-11-04 02:32:04.242143 django-pgmigrate-1.0.1/README.rst
--rw-r--r--   0        0        0      300 2022-11-04 02:32:04.246143 django-pgmigrate-1.0.1/pgmigrate/__init__.py
--rw-r--r--   0        0        0     2153 2022-11-04 02:32:04.246143 django-pgmigrate-1.0.1/pgmigrate/action.py
--rw-r--r--   0        0        0      188 2022-11-04 02:32:04.246143 django-pgmigrate-1.0.1/pgmigrate/apps.py
--rw-r--r--   0        0        0     1073 2022-11-04 02:32:04.246143 django-pgmigrate-1.0.1/pgmigrate/config.py
--rw-r--r--   0        0        0      631 2022-11-04 02:32:04.246143 django-pgmigrate-1.0.1/pgmigrate/core.py
--rw-r--r--   0        0        0        0 2022-11-04 02:32:04.246143 django-pgmigrate-1.0.1/pgmigrate/management/__init__.py
--rw-r--r--   0        0        0        0 2022-11-04 02:32:04.246143 django-pgmigrate-1.0.1/pgmigrate/management/commands/__init__.py
--rw-r--r--   0        0        0     1986 2022-11-04 02:32:04.246143 django-pgmigrate-1.0.1/pgmigrate/management/commands/pgmigrate.py
--rw-r--r--   0        0        0      154 2022-11-04 02:32:04.246143 django-pgmigrate-1.0.1/pgmigrate/version.py
--rw-r--r--   0        0        0     2282 2022-11-04 02:32:52.658663 django-pgmigrate-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3797 1970-01-01 00:00:00.000000 django-pgmigrate-1.0.1/setup.py
--rw-r--r--   0        0        0     4292 1970-01-01 00:00:00.000000 django-pgmigrate-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1456 2023-06-09 00:20:17.213098 django_pgmigrate-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2855 2023-06-09 00:20:17.213098 django_pgmigrate-1.1.0/README.rst
+-rw-r--r--   0        0        0      320 2023-06-09 00:20:17.217099 django_pgmigrate-1.1.0/pgmigrate/__init__.py
+-rw-r--r--   0        0        0     2153 2023-06-09 00:20:17.217099 django_pgmigrate-1.1.0/pgmigrate/action.py
+-rw-r--r--   0        0        0      188 2023-06-09 00:20:17.217099 django_pgmigrate-1.1.0/pgmigrate/apps.py
+-rw-r--r--   0        0        0     1073 2023-06-09 00:20:17.217099 django_pgmigrate-1.1.0/pgmigrate/config.py
+-rw-r--r--   0        0        0      631 2023-06-09 00:20:17.217099 django_pgmigrate-1.1.0/pgmigrate/core.py
+-rw-r--r--   0        0        0        0 2023-06-09 00:20:17.217099 django_pgmigrate-1.1.0/pgmigrate/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 00:20:17.217099 django_pgmigrate-1.1.0/pgmigrate/management/commands/__init__.py
+-rw-r--r--   0        0        0     2248 2023-06-09 00:20:17.217099 django_pgmigrate-1.1.0/pgmigrate/management/commands/pgmigrate.py
+-rw-r--r--   0        0        0      154 2023-06-09 00:20:17.217099 django_pgmigrate-1.1.0/pgmigrate/version.py
+-rw-r--r--   0        0        0     2326 2023-06-09 00:20:50.393141 django_pgmigrate-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4156 1970-01-01 00:00:00.000000 django_pgmigrate-1.1.0/PKG-INFO
```

### Comparing `django-pgmigrate-1.0.1/LICENSE` & `django_pgmigrate-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-pgmigrate-1.0.1/README.rst` & `django_pgmigrate-1.1.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -49,16 +49,15 @@
 killing them, and you can also set the lock timeout to automatically cancel migrations if
 they block for too long.
 See the documentation section below for more details.
 
 Compatibility
 =============
 
-``django-pgmigrate`` is compatible with Python 3.7 - 3.10, Django 2.2 - 4.1, and Postgres 10 - 15.
-
+``django-pgmigrate`` is compatible with Python 3.7 - 3.11, Django 3.2 - 4.2, Psycopg 2 - 3 and Postgres 12 - 15.
 
 Documentation
 =============
 
 `View the django-pgmigrate docs here
 <https://django-pgmigrate.readthedocs.io/>`_ to learn more about:
```

### Comparing `django-pgmigrate-1.0.1/pgmigrate/action.py` & `django_pgmigrate-1.1.0/pgmigrate/action.py`

 * *Files identical despite different names*

### Comparing `django-pgmigrate-1.0.1/pgmigrate/config.py` & `django_pgmigrate-1.1.0/pgmigrate/config.py`

 * *Files identical despite different names*

### Comparing `django-pgmigrate-1.0.1/pgmigrate/core.py` & `django_pgmigrate-1.1.0/pgmigrate/core.py`

 * *Files identical despite different names*

### Comparing `django-pgmigrate-1.0.1/pgmigrate/management/commands/pgmigrate.py` & `django_pgmigrate-1.1.0/pgmigrate/management/commands/pgmigrate.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 import functools
 import inspect
 import sys
 
+from django.core.exceptions import ImproperlyConfigured
 from django.core.management.commands.migrate import Command as MigrateCommand
 from django.db import connections
 from django.db.utils import OperationalError
 import pgactivity
 import pglock
-import psycopg2.errors
+
+try:
+    import psycopg.errors as psycopg_errors
+except ImportError:
+    import psycopg2.errors as psycopg_errors
+except ImportError:  # pragma: no cover
+    raise ImproperlyConfigured("Error loading psycopg2 or psycopg module")
 
 from pgmigrate import action, config
 
 
 class Command(MigrateCommand):
     def handle(self, *args, **options):
         if (
@@ -44,14 +51,14 @@
             }
             if config.lock_timeout():
                 prioritize_kwargs["timeout"] = config.lock_timeout()
 
             with pglock.prioritize(**prioritize_kwargs):
                 return super().handle(*args, **options)
         except OperationalError as exc:
-            if exc.__cause__.__class__ == psycopg2.errors.LockNotAvailable:
+            if exc.__cause__.__class__ == psycopg_errors.LockNotAvailable:
                 if self.verbosity:  # pragma: no branch
                     self.stdout.write(self.style.ERROR("\nLock timeout expired. Aborting..."))
 
                 sys.exit(1)
             else:  # pragma: no cover
                 raise
```

### Comparing `django-pgmigrate-1.0.1/pyproject.toml` & `django_pgmigrate-1.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -25,61 +25,62 @@
 name = "django-pgmigrate"
 packages = [
   { include = "pgmigrate" }
 ]
 exclude = [
   "*/tests/"
 ]
-version = "1.0.1"
+version = "1.1.0"
 description = "Less downtime during migrations."
 authors = ["Opus 10 Engineering"]
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
 homepage = "https://github.com/Opus10/django-pgmigrate"
 repository = "https://github.com/Opus10/django-pgmigrate"
 documentation = "https://django-pgmigrate.readthedocs.io"
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<4"
 django = ">=2"
-django-pglock = ">=1.1.0,<2"
+django-pglock = ">=1.3.0,<2"
 importlib_metadata = { version = ">=4", python = "~3.7" }
 
 [tool.poetry.dev-dependencies]
 black = "22.6.0"
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
 poetry-core = "1.3.2"
 pre-commit = "2.13.0"
-psycopg2-binary = "2.9.3"
+psycopg2-binary = "2.9.6"
 pytest = "7.0.0"
 pytest-cov = "3.0.0"
 pytest-dotenv = "0.5.2"
 pytest-django = "4.5.2"
 pytest-reraise = "2.1.2"
 requests = "2.25.1"
 Sphinx = "4.4.0"
```

### Comparing `django-pgmigrate-1.0.1/setup.py` & `django_pgmigrate-1.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,112 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: django-pgmigrate
+Version: 1.1.0
+Summary: Less downtime during migrations.
+Home-page: https://github.com/Opus10/django-pgmigrate
+License: BSD-3-Clause
+Author: Opus 10 Engineering
+Requires-Python: >=3.7.0,<4
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Dist: django (>=2)
+Requires-Dist: django-pglock (>=1.3.0,<2)
+Requires-Dist: importlib_metadata (>=4) ; python_version >= "3.7" and python_version < "3.8"
+Project-URL: Documentation, https://django-pgmigrate.readthedocs.io
+Project-URL: Repository, https://github.com/Opus10/django-pgmigrate
+Description-Content-Type: text/x-rst
+
+django-pgmigrate
+################
+
+``django-pgmigrate`` helps you avoid costly downtime with Postgres migrations.
+
+Imagine the following happens:
+
+1. A long-running task queries a model in a transaction and keeps the transaction open.
+2. ``python manage.py migrate`` tries to change a field on the model.
+
+Because of how Postgres queues locks, this common scenario causes **every**
+subsequent query on the model to block until the query from 1) has finished.
+
+``django-pgmigrate`` provides the following features to alleviate problematic locking
+scenarios when running migrations:
+
+* Detect blocking queries and terminate them automatically (the default behavior).
+* Print blocking queries so that you can inspect
+  and terminate them manually.
+* Set the lock timeout so that migrations are terminated if they block too long.
+
+Installation
+============
+
+Install django-pgmigrate with::
+
+    pip3 install django-pgmigrate
+
+After this, add ``pgactivity``, ``pglock``, and ``pgmigrate`` to the ``INSTALLED_APPS``
+setting of your Django project.
+
+Quick Start
+===========
+
+After following the installation instructions, running
+``python manage.py migrate`` will automatically terminate any blocking
+queries. Here's an example of what it looks like:
+
+.. image:: docs/static/terminate_blocking.png
+
+There are two additional outputs in the ``migrate`` command versus the original:
+
+1. The first output line shows the Postgres process ID. This is useful for
+   querying activity that's blocking the process.
+2. The yellow text shows when a blocking query was detected and terminated.
+   In our case, it was blocking auth migration 12.
+
+You can configure ``django-pgmigrate`` to show blocked queries instead of automatically
+killing them, and you can also set the lock timeout to automatically cancel migrations if
+they block for too long.
+See the documentation section below for more details.
+
+Compatibility
+=============
+
+``django-pgmigrate`` is compatible with Python 3.7 - 3.11, Django 3.2 - 4.2, Psycopg 2 - 3 and Postgres 12 - 15.
+
+Documentation
+=============
+
+`View the django-pgmigrate docs here
+<https://django-pgmigrate.readthedocs.io/>`_ to learn more about:
+
+* How blocking queries are automatically terminated.
+* Configuring the command to show blocking activity instead of terminating it, along
+  with instructions on how to manually view and terminate activity.
+* Configuring lock timeouts to automatically stop migrations if they block for too long.
+* Advanced usage such as creating custom actions to run when queries are blocked.
+
+Contributing Guide
+==================
 
-packages = \
-['pgmigrate', 'pgmigrate.management', 'pgmigrate.management.commands']
+For information on setting up django-pgmigrate for development and
+contributing changes, view `CONTRIBUTING.rst <CONTRIBUTING.rst>`_.
 
-package_data = \
-{'': ['*']}
+Primary Authors
+===============
 
-install_requires = \
-['django-pglock>=1.1.0,<2', 'django>=2']
-
-extras_require = \
-{':python_version >= "3.7" and python_version < "3.8"': ['importlib_metadata>=4']}
-
-setup_kwargs = {
-    'name': 'django-pgmigrate',
-    'version': '1.0.1',
-    'description': 'Less downtime during migrations.',
-    'long_description': "django-pgmigrate\n################\n\n``django-pgmigrate`` helps you avoid costly downtime with Postgres migrations.\n\nImagine the following happens:\n\n1. A long-running task queries a model in a transaction and keeps the transaction open.\n2. ``python manage.py migrate`` tries to change a field on the model.\n\nBecause of how Postgres queues locks, this common scenario causes **every**\nsubsequent query on the model to block until the query from 1) has finished.\n\n``django-pgmigrate`` provides the following features to alleviate problematic locking\nscenarios when running migrations:\n\n* Detect blocking queries and terminate them automatically (the default behavior).\n* Print blocking queries so that you can inspect\n  and terminate them manually.\n* Set the lock timeout so that migrations are terminated if they block too long.\n\nInstallation\n============\n\nInstall django-pgmigrate with::\n\n    pip3 install django-pgmigrate\n\nAfter this, add ``pgactivity``, ``pglock``, and ``pgmigrate`` to the ``INSTALLED_APPS``\nsetting of your Django project.\n\nQuick Start\n===========\n\nAfter following the installation instructions, running\n``python manage.py migrate`` will automatically terminate any blocking\nqueries. Here's an example of what it looks like:\n\n.. image:: docs/static/terminate_blocking.png\n\nThere are two additional outputs in the ``migrate`` command versus the original:\n\n1. The first output line shows the Postgres process ID. This is useful for\n   querying activity that's blocking the process.\n2. The yellow text shows when a blocking query was detected and terminated.\n   In our case, it was blocking auth migration 12.\n\nYou can configure ``django-pgmigrate`` to show blocked queries instead of automatically\nkilling them, and you can also set the lock timeout to automatically cancel migrations if\nthey block for too long.\nSee the documentation section below for more details.\n\nCompatibility\n=============\n\n``django-pgmigrate`` is compatible with Python 3.7 - 3.10, Django 2.2 - 4.1, and Postgres 10 - 15.\n\n\nDocumentation\n=============\n\n`View the django-pgmigrate docs here\n<https://django-pgmigrate.readthedocs.io/>`_ to learn more about:\n\n* How blocking queries are automatically terminated.\n* Configuring the command to show blocking activity instead of terminating it, along\n  with instructions on how to manually view and terminate activity.\n* Configuring lock timeouts to automatically stop migrations if they block for too long.\n* Advanced usage such as creating custom actions to run when queries are blocked.\n\nContributing Guide\n==================\n\nFor information on setting up django-pgmigrate for development and\ncontributing changes, view `CONTRIBUTING.rst <CONTRIBUTING.rst>`_.\n\nPrimary Authors\n===============\n\n- `Wes Kendall <https://github.com/wesleykendall>`__\n- `Paul Gilmartin <https://github.com/PaulGilmartin>`__\n",
-    'author': 'Opus 10 Engineering',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/Opus10/django-pgmigrate',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7.0,<4',
-}
+- `Wes Kendall <https://github.com/wesleykendall>`__
+- `Paul Gilmartin <https://github.com/PaulGilmartin>`__
 
-
-setup(**setup_kwargs)
```

