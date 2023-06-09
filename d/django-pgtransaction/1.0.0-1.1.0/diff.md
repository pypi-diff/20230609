# Comparing `tmp/django-pgtransaction-1.0.0.tar.gz` & `tmp/django_pgtransaction-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pgtransaction-1.0.0.tar", max compression
+gzip compressed data, was "django_pgtransaction-1.1.0.tar", max compression
```

## Comparing `django-pgtransaction-1.0.0.tar` & `django_pgtransaction-1.1.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1456 2022-09-20 20:41:22.297262 django-pgtransaction-1.0.0/LICENSE
--rw-r--r--   0        0        0     3081 2022-09-20 20:41:22.297262 django-pgtransaction-1.0.0/README.rst
--rw-r--r--   0        0        0      224 2022-09-20 20:41:22.297262 django-pgtransaction-1.0.0/pgtransaction/__init__.py
--rw-r--r--   0        0        0      457 2022-09-20 20:41:22.297262 django-pgtransaction-1.0.0/pgtransaction/config.py
--rw-r--r--   0        0        0     7156 2022-09-20 20:41:22.297262 django-pgtransaction-1.0.0/pgtransaction/transaction.py
--rw-r--r--   0        0        0      158 2022-09-20 20:41:22.297262 django-pgtransaction-1.0.0/pgtransaction/version.py
--rw-r--r--   0        0        0     2403 2022-09-20 20:42:01.789497 django-pgtransaction-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4078 1970-01-01 00:00:00.000000 django-pgtransaction-1.0.0/setup.py
--rw-r--r--   0        0        0     4616 1970-01-01 00:00:00.000000 django-pgtransaction-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1456 2023-06-09 00:29:24.429535 django_pgtransaction-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3225 2023-06-09 00:29:24.429535 django_pgtransaction-1.1.0/README.rst
+-rw-r--r--   0        0        0      224 2023-06-09 00:29:24.429535 django_pgtransaction-1.1.0/pgtransaction/__init__.py
+-rw-r--r--   0        0        0      717 2023-06-09 00:29:24.429535 django_pgtransaction-1.1.0/pgtransaction/config.py
+-rw-r--r--   0        0        0     7174 2023-06-09 00:29:24.433535 django_pgtransaction-1.1.0/pgtransaction/transaction.py
+-rw-r--r--   0        0        0      158 2023-06-09 00:29:24.433535 django_pgtransaction-1.1.0/pgtransaction/version.py
+-rw-r--r--   0        0        0     2444 2023-06-09 00:29:55.053598 django_pgtransaction-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4611 1970-01-01 00:00:00.000000 django_pgtransaction-1.1.0/PKG-INFO
```

### Comparing `django-pgtransaction-1.0.0/LICENSE` & `django_pgtransaction-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-pgtransaction-1.0.0/README.rst` & `django_pgtransaction-1.1.0/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -37,24 +37,29 @@
     @pgtransaction.atomic(isolation_level=pgtransaction.SERIALIZABLE, retry=3)
     def do_queries():
         # Do queries...
 
 Note that the ``retry`` argument will not work when used as a context manager. A ``RuntimeError``
 will be thrown.
 
-By default, retries are only performed when ``psycopg2.errors.SerializationError`` or
-``psycopg2.errors.DeadlockDetected`` errors are raised. Configure retried psycopg2 errors with
+By default, retries are only performed when ``psycopg.errors.SerializationError`` or
+``psycopg.errors.DeadlockDetected`` errors are raised. Configure retried psycopg errors with
 ``settings.PGTRANSACTION_RETRY_EXCEPTIONS``. You can set a default retry amount with
 ``settings.PGTRANSACTION_RETRY``.
 
 ``pgtransaction.atomic`` can be nested, but keep the following in mind:
 
 1. The isolation level cannot be changed once a query has been performed.
 2. The retry argument only works on the outermost invocation as a decorator, otherwise ``RuntimeError`` is raised.
 
+Compatibility
+=============
+
+``django-pgtransaction`` is compatible with Python 3.7 - 3.11, Django 3.2 - 4.2, Psycopg 2 - 3 and Postgres 12 - 15.
+
 Documentation
 =============
 
 Check out the `Postgres docs <https://www.postgresql.org/docs/current/transaction-iso.html>`__
 to learn about transaction isolation in Postgres. 
 
 `View the django-pgtransaction docs here
```

### Comparing `django-pgtransaction-1.0.0/pgtransaction/transaction.py` & `django_pgtransaction-1.1.0/pgtransaction/transaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         savepoint,
         durable,
         isolation_level,
         retry,
     ):
         if django.VERSION >= (3, 2):
             super().__init__(using, savepoint, durable)
-        else:
+        else:  # pragma: no cover
             super().__init__(using, savepoint)
 
         self.isolation_level = isolation_level
         self.retry = retry
         self._used_as_context_manager = True
 
         if self.isolation_level:  # pragma: no cover
@@ -152,15 +152,15 @@
         Note that setting ``isolation_level`` in a nested atomic block is permitted as long
         as no queries have been made.
 
         When used as a decorator, one can also specify a ``retry`` argument. This
         defines the number of times the transaction will be retried upon encountering
         the exceptions referenced by ``settings.PGTRANSACTION_RETRY_EXCEPTIONS``,
         which defaults to
-        ``(psycopg2.errors.SerializationFailure, psycopg2.errors.DeadlockDetected)``.
+        ``(psycopg.errors.SerializationFailure, psycopg.errors.DeadlockDetected)``.
         For example:
 
         .. code-block:: python
 
             @pgtransaction.atomic(retry=3)
             def update():
                 # will retry update function up to 3 times
```

### Comparing `django-pgtransaction-1.0.0/pyproject.toml` & `django_pgtransaction-1.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -25,30 +25,31 @@
 name = "django-pgtransaction"
 packages = [
   { include = "pgtransaction" }
 ]
 exclude = [
   "*/tests/"
 ]
-version = "1.0.0"
+version = "1.1.0"
 description = "A context manager/decorator which extends Django's atomic function with the ability to set isolation level and retries for a given transaction."
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
 homepage = "https://github.com/Opus10/django-pgtransaction"
 repository = "https://github.com/Opus10/django-pgtransaction"
@@ -65,21 +66,21 @@
 django-dynamic-fixture = "3.1.2"
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

### Comparing `django-pgtransaction-1.0.0/setup.py` & `django_pgtransaction-1.1.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,119 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: django-pgtransaction
+Version: 1.1.0
+Summary: A context manager/decorator which extends Django's atomic function with the ability to set isolation level and retries for a given transaction.
+Home-page: https://github.com/Opus10/django-pgtransaction
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
+Requires-Dist: importlib_metadata (>=4) ; python_version >= "3.7" and python_version < "3.8"
+Project-URL: Documentation, https://django-pgtransaction.readthedocs.io
+Project-URL: Repository, https://github.com/Opus10/django-pgtransaction
+Description-Content-Type: text/x-rst
+
+django-pgtransaction
+====================
+
+django-pgtransaction offers a drop-in replacement for the
+default ``django.db.transaction`` module which, when used on top of a PostgreSQL
+database, extends the functionality of that module with Postgres-specific features.
+
+At present, django-pgtransaction offers an extension of the
+``django.db.transaction.atomic`` context manager/decorator which allows one to
+dynamically set the `isolation level <https://www.postgresql.org/docs/current/transaction-iso.html>`__
+when opening a transaction, as well as specifying
+a retry policy for when an operation in that transaction results in a Postgres locking
+exception. See the quickstart below or `the docs <https://django-pgtransaction.readthedocs.io/>`__ for examples.
+
+Quickstart
+==========
+
+Set the isolation level of a transaction by using ``pgtransaction.atomic``:
+
+.. code-block:: python
+
+    import pgtransaction
+
+    with pgtransaction.atomic(isolation_level=pgtransaction.SERIALIZABLE):
+        # Do queries...
+
+There are three isolation levels: ``pgtransaction.READ_COMMITTED``, ``pgtransaction.REPEATABLE_READ``,
+and ``pgtransaction.SERIALIZABLE``. By default it inherits the parent isolation level, which is Django's
+default of "READ COMMITTED".
+
+When using stricter isolation levels like ``pgtransaction.SERIALIZABLE``, Postgres will throw
+serialization errors upon concurrent updates to rows. Use the ``retry`` argument with the decorator
+to retry these failures:
+
+.. code-block:: python
+
+    @pgtransaction.atomic(isolation_level=pgtransaction.SERIALIZABLE, retry=3)
+    def do_queries():
+        # Do queries...
+
+Note that the ``retry`` argument will not work when used as a context manager. A ``RuntimeError``
+will be thrown.
+
+By default, retries are only performed when ``psycopg.errors.SerializationError`` or
+``psycopg.errors.DeadlockDetected`` errors are raised. Configure retried psycopg errors with
+``settings.PGTRANSACTION_RETRY_EXCEPTIONS``. You can set a default retry amount with
+``settings.PGTRANSACTION_RETRY``.
+
+``pgtransaction.atomic`` can be nested, but keep the following in mind:
+
+1. The isolation level cannot be changed once a query has been performed.
+2. The retry argument only works on the outermost invocation as a decorator, otherwise ``RuntimeError`` is raised.
+
+Compatibility
+=============
+
+``django-pgtransaction`` is compatible with Python 3.7 - 3.11, Django 3.2 - 4.2, Psycopg 2 - 3 and Postgres 12 - 15.
+
+Documentation
+=============
+
+Check out the `Postgres docs <https://www.postgresql.org/docs/current/transaction-iso.html>`__
+to learn about transaction isolation in Postgres. 
+
+`View the django-pgtransaction docs here
+<https://django-pgtransaction.readthedocs.io/>`_.
+
+Installation
+============
+
+Install django-pgtransaction with::
+
+    pip3 install django-pgtransaction
+
+After this, add ``pgtransaction`` to the ``INSTALLED_APPS``
+setting of your Django project.
+
+Contributing Guide
+==================
 
-packages = \
-['pgtransaction']
+For information on setting up django-pgtransaction for development and
+contributing changes, view `CONTRIBUTING.rst <CONTRIBUTING.rst>`_.
 
-package_data = \
-{'': ['*']}
+Primary Authors
+===============
 
-install_requires = \
-['django>=2']
-
-extras_require = \
-{':python_version >= "3.7" and python_version < "3.8"': ['importlib_metadata>=4']}
-
-setup_kwargs = {
-    'name': 'django-pgtransaction',
-    'version': '1.0.0',
-    'description': "A context manager/decorator which extends Django's atomic function with the ability to set isolation level and retries for a given transaction.",
-    'long_description': 'django-pgtransaction\n====================\n\ndjango-pgtransaction offers a drop-in replacement for the\ndefault ``django.db.transaction`` module which, when used on top of a PostgreSQL\ndatabase, extends the functionality of that module with Postgres-specific features.\n\nAt present, django-pgtransaction offers an extension of the\n``django.db.transaction.atomic`` context manager/decorator which allows one to\ndynamically set the `isolation level <https://www.postgresql.org/docs/current/transaction-iso.html>`__\nwhen opening a transaction, as well as specifying\na retry policy for when an operation in that transaction results in a Postgres locking\nexception. See the quickstart below or `the docs <https://django-pgtransaction.readthedocs.io/>`__ for examples.\n\nQuickstart\n==========\n\nSet the isolation level of a transaction by using ``pgtransaction.atomic``:\n\n.. code-block:: python\n\n    import pgtransaction\n\n    with pgtransaction.atomic(isolation_level=pgtransaction.SERIALIZABLE):\n        # Do queries...\n\nThere are three isolation levels: ``pgtransaction.READ_COMMITTED``, ``pgtransaction.REPEATABLE_READ``,\nand ``pgtransaction.SERIALIZABLE``. By default it inherits the parent isolation level, which is Django\'s\ndefault of "READ COMMITTED".\n\nWhen using stricter isolation levels like ``pgtransaction.SERIALIZABLE``, Postgres will throw\nserialization errors upon concurrent updates to rows. Use the ``retry`` argument with the decorator\nto retry these failures:\n\n.. code-block:: python\n\n    @pgtransaction.atomic(isolation_level=pgtransaction.SERIALIZABLE, retry=3)\n    def do_queries():\n        # Do queries...\n\nNote that the ``retry`` argument will not work when used as a context manager. A ``RuntimeError``\nwill be thrown.\n\nBy default, retries are only performed when ``psycopg2.errors.SerializationError`` or\n``psycopg2.errors.DeadlockDetected`` errors are raised. Configure retried psycopg2 errors with\n``settings.PGTRANSACTION_RETRY_EXCEPTIONS``. You can set a default retry amount with\n``settings.PGTRANSACTION_RETRY``.\n\n``pgtransaction.atomic`` can be nested, but keep the following in mind:\n\n1. The isolation level cannot be changed once a query has been performed.\n2. The retry argument only works on the outermost invocation as a decorator, otherwise ``RuntimeError`` is raised.\n\nDocumentation\n=============\n\nCheck out the `Postgres docs <https://www.postgresql.org/docs/current/transaction-iso.html>`__\nto learn about transaction isolation in Postgres. \n\n`View the django-pgtransaction docs here\n<https://django-pgtransaction.readthedocs.io/>`_.\n\nInstallation\n============\n\nInstall django-pgtransaction with::\n\n    pip3 install django-pgtransaction\n\nAfter this, add ``pgtransaction`` to the ``INSTALLED_APPS``\nsetting of your Django project.\n\nContributing Guide\n==================\n\nFor information on setting up django-pgtransaction for development and\ncontributing changes, view `CONTRIBUTING.rst <CONTRIBUTING.rst>`_.\n\nPrimary Authors\n===============\n\n- `Paul Gilmartin <https://github.com/PaulGilmartin>`__\n- `Wes Kendall <https://github.com/wesleykendall>`__\n',
-    'author': 'Opus 10 Engineering',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/Opus10/django-pgtransaction',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7.0,<4',
-}
+- `Paul Gilmartin <https://github.com/PaulGilmartin>`__
+- `Wes Kendall <https://github.com/wesleykendall>`__
 
-
-setup(**setup_kwargs)
```

