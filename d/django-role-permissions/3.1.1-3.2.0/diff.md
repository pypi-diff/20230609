# Comparing `tmp/django-role-permissions-3.1.1.tar.gz` & `tmp/django-role-permissions-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-role-permissions-3.1.1.tar", last modified: Tue Nov 10 20:30:52 2020, max compression
+gzip compressed data, was "django-role-permissions-3.2.0.tar", last modified: Fri Jun  9 20:31:22 2023, max compression
```

## Comparing `django-role-permissions-3.1.1.tar` & `django-role-permissions-3.2.0.tar`

### file list

```diff
@@ -1,44 +1,43 @@
-drwxr-xr-x   0 filipeximenes   (501) staff       (20)        0 2020-11-10 20:30:52.000000 django-role-permissions-3.1.1/
--rw-r--r--   0 filipeximenes   (501) staff       (20)      686 2020-11-10 20:30:52.000000 django-role-permissions-3.1.1/PKG-INFO
-drwxr-xr-x   0 filipeximenes   (501) staff       (20)        0 2020-11-10 20:30:52.000000 django-role-permissions-3.1.1/django_role_permissions.egg-info/
--rw-r--r--   0 filipeximenes   (501) staff       (20)      686 2020-11-10 20:30:52.000000 django-role-permissions-3.1.1/django_role_permissions.egg-info/PKG-INFO
--rw-r--r--   0 filipeximenes   (501) staff       (20)     1237 2020-11-10 20:30:52.000000 django-role-permissions-3.1.1/django_role_permissions.egg-info/SOURCES.txt
--rw-r--r--   0 filipeximenes   (501) staff       (20)       39 2020-11-10 20:30:52.000000 django-role-permissions-3.1.1/django_role_permissions.egg-info/requires.txt
--rw-r--r--   0 filipeximenes   (501) staff       (20)      130 2020-11-10 20:30:52.000000 django-role-permissions-3.1.1/django_role_permissions.egg-info/top_level.txt
--rw-r--r--   0 filipeximenes   (501) staff       (20)        1 2020-11-10 20:30:52.000000 django-role-permissions-3.1.1/django_role_permissions.egg-info/dependency_links.txt
--rw-r--r--   0 filipeximenes   (501) staff       (20)     1899 2020-11-10 20:30:22.000000 django-role-permissions-3.1.1/README.md
--rwxr-xr-x   0 filipeximenes   (501) staff       (20)     2546 2020-07-23 18:38:41.000000 django-role-permissions-3.1.1/setup.py
-drwxr-xr-x   0 filipeximenes   (501) staff       (20)        0 2020-11-10 20:30:52.000000 django-role-permissions-3.1.1/rolepermissions/
-drwxr-xr-x   0 filipeximenes   (501) staff       (20)        0 2020-11-10 20:30:52.000000 django-role-permissions-3.1.1/rolepermissions/templatetags/
--rw-r--r--   0 filipeximenes   (501) staff       (20)        0 2020-07-23 18:38:41.000000 django-role-permissions-3.1.1/rolepermissions/templatetags/__init__.py
--rw-r--r--   0 filipeximenes   (501) staff       (20)      829 2020-07-23 18:38:41.000000 django-role-permissions-3.1.1/rolepermissions/templatetags/permission_tags.py
--rw-r--r--   0 filipeximenes   (501) staff       (20)      865 2020-07-23 18:38:41.000000 django-role-permissions-3.1.1/rolepermissions/mixins.py
--rw-r--r--   0 filipeximenes   (501) staff       (20)       30 2020-07-23 18:38:41.000000 django-role-permissions-3.1.1/rolepermissions/models.py
--rw-r--r--   0 filipeximenes   (501) staff       (20)     1697 2020-07-23 18:45:26.000000 django-role-permissions-3.1.1/rolepermissions/checkers.py
--rw-r--r--   0 filipeximenes   (501) staff       (20)     7914 2020-11-10 18:54:27.000000 django-role-permissions-3.1.1/rolepermissions/roles.py
-drwxr-xr-x   0 filipeximenes   (501) staff       (20)        0 2020-11-10 20:30:52.000000 django-role-permissions-3.1.1/rolepermissions/tests/
--rw-r--r--   0 filipeximenes   (501) staff       (20)     3717 2020-07-23 18:38:41.000000 django-role-permissions-3.1.1/rolepermissions/tests/test_admin.py
--rw-r--r--   0 filipeximenes   (501) staff       (20)      906 2020-07-23 18:38:41.000000 django-role-permissions-3.1.1/rolepermissions/tests/test_utils.py
--rw-r--r--   0 filipeximenes   (501) staff       (20)     3674 2020-07-23 18:38:41.000000 django-role-permissions-3.1.1/rolepermissions/tests/test_template_tags.py
--rw-r--r--   0 filipeximenes   (501) staff       (20)     6894 2020-07-23 18:38:41.000000 django-role-permissions-3.1.1/rolepermissions/tests/test_decorators.py
--rw-r--r--   0 filipeximenes   (501) staff       (20)       64 2020-07-23 18:38:41.000000 django-role-permissions-3.1.1/rolepermissions/tests/mock_urls.py
--rw-r--r--   0 filipeximenes   (501) staff       (20)        0 2020-07-23 18:38:41.000000 django-role-permissions-3.1.1/rolepermissions/tests/__init__.py
--rw-r--r--   0 filipeximenes   (501) staff       (20)     5683 2020-07-23 18:45:26.000000 django-role-permissions-3.1.1/rolepermissions/tests/test_verifications.py
--rw-r--r--   0 filipeximenes   (501) staff       (20)    18744 2020-07-23 18:38:41.000000 django-role-permissions-3.1.1/rolepermissions/tests/test_shortcuts.py
--rw-r--r--   0 filipeximenes   (501) staff       (20)     4856 2020-07-23 18:38:41.000000 django-role-permissions-3.1.1/rolepermissions/tests/test_mixins.py
--rw-r--r--   0 filipeximenes   (501) staff       (20)     6175 2020-07-23 18:38:41.000000 django-role-permissions-3.1.1/rolepermissions/tests/test_roles.py
--rw-r--r--   0 filipeximenes   (501) staff       (20)     1892 2020-07-23 18:38:41.000000 django-role-permissions-3.1.1/rolepermissions/tests/test_permissions.py
-drwxr-xr-x   0 filipeximenes   (501) staff       (20)        0 2020-11-10 20:30:52.000000 django-role-permissions-3.1.1/rolepermissions/management/
--rw-r--r--   0 filipeximenes   (501) staff       (20)        0 2020-07-23 18:38:41.000000 django-role-permissions-3.1.1/rolepermissions/management/__init__.py
-drwxr-xr-x   0 filipeximenes   (501) staff       (20)        0 2020-11-10 20:30:52.000000 django-role-permissions-3.1.1/rolepermissions/management/commands/
--rw-r--r--   0 filipeximenes   (501) staff       (20)     2236 2020-07-23 18:38:41.000000 django-role-permissions-3.1.1/rolepermissions/management/commands/sync_roles.py
--rw-r--r--   0 filipeximenes   (501) staff       (20)        0 2020-07-23 18:38:41.000000 django-role-permissions-3.1.1/rolepermissions/management/commands/__init__.py
--rw-r--r--   0 filipeximenes   (501) staff       (20)       84 2020-11-10 20:30:22.000000 django-role-permissions-3.1.1/rolepermissions/__init__.py
--rw-r--r--   0 filipeximenes   (501) staff       (20)      267 2020-07-23 18:38:41.000000 django-role-permissions-3.1.1/rolepermissions/apps.py
--rw-r--r--   0 filipeximenes   (501) staff       (20)     1638 2020-07-23 18:38:41.000000 django-role-permissions-3.1.1/rolepermissions/admin.py
--rw-r--r--   0 filipeximenes   (501) staff       (20)      923 2020-11-10 18:54:27.000000 django-role-permissions-3.1.1/rolepermissions/utils.py
--rw-r--r--   0 filipeximenes   (501) staff       (20)      808 2020-07-23 18:38:41.000000 django-role-permissions-3.1.1/rolepermissions/loader.py
--rw-r--r--   0 filipeximenes   (501) staff       (20)     3725 2020-11-10 18:54:27.000000 django-role-permissions-3.1.1/rolepermissions/permissions.py
--rw-r--r--   0 filipeximenes   (501) staff       (20)      194 2020-07-23 18:38:41.000000 django-role-permissions-3.1.1/rolepermissions/exceptions.py
--rw-r--r--   0 filipeximenes   (501) staff       (20)     1808 2020-07-23 18:38:41.000000 django-role-permissions-3.1.1/rolepermissions/decorators.py
--rw-r--r--   0 filipeximenes   (501) staff       (20)      127 2020-11-10 20:30:52.000000 django-role-permissions-3.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:31:22.951765 django-role-permissions-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-09 20:31:04.000000 django-role-permissions-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-09 20:31:22.951765 django-role-permissions-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-06-09 20:31:04.000000 django-role-permissions-3.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:31:22.947765 django-role-permissions-3.2.0/django_role_permissions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-09 20:31:22.000000 django-role-permissions-3.2.0/django_role_permissions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-09 20:31:22.000000 django-role-permissions-3.2.0/django_role_permissions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 20:31:22.000000 django-role-permissions-3.2.0/django_role_permissions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-09 20:31:22.000000 django-role-permissions-3.2.0/django_role_permissions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-09 20:31:22.000000 django-role-permissions-3.2.0/django_role_permissions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:31:22.947765 django-role-permissions-3.2.0/rolepermissions/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-09 20:31:04.000000 django-role-permissions-3.2.0/rolepermissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-09 20:31:04.000000 django-role-permissions-3.2.0/rolepermissions/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-09 20:31:04.000000 django-role-permissions-3.2.0/rolepermissions/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-09 20:31:04.000000 django-role-permissions-3.2.0/rolepermissions/checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-09 20:31:04.000000 django-role-permissions-3.2.0/rolepermissions/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-09 20:31:04.000000 django-role-permissions-3.2.0/rolepermissions/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-09 20:31:04.000000 django-role-permissions-3.2.0/rolepermissions/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:31:22.947765 django-role-permissions-3.2.0/rolepermissions/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 20:31:04.000000 django-role-permissions-3.2.0/rolepermissions/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:31:22.947765 django-role-permissions-3.2.0/rolepermissions/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 20:31:04.000000 django-role-permissions-3.2.0/rolepermissions/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-09 20:31:04.000000 django-role-permissions-3.2.0/rolepermissions/management/commands/sync_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-09 20:31:04.000000 django-role-permissions-3.2.0/rolepermissions/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 20:31:04.000000 django-role-permissions-3.2.0/rolepermissions/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-06-09 20:31:04.000000 django-role-permissions-3.2.0/rolepermissions/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-06-09 20:31:04.000000 django-role-permissions-3.2.0/rolepermissions/roles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:31:22.947765 django-role-permissions-3.2.0/rolepermissions/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 20:31:04.000000 django-role-permissions-3.2.0/rolepermissions/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-09 20:31:04.000000 django-role-permissions-3.2.0/rolepermissions/templatetags/permission_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-09 20:31:04.000000 django-role-permissions-3.2.0/rolepermissions/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-09 20:31:22.951765 django-role-permissions-3.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2334 2023-06-09 20:31:04.000000 django-role-permissions-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:31:22.951765 django-role-permissions-3.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-09 20:31:04.000000 django-role-permissions-3.2.0/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-06-09 20:31:04.000000 django-role-permissions-3.2.0/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-06-09 20:31:04.000000 django-role-permissions-3.2.0/tests/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-09 20:31:04.000000 django-role-permissions-3.2.0/tests/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-06-09 20:31:04.000000 django-role-permissions-3.2.0/tests/test_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18744 2023-06-09 20:31:04.000000 django-role-permissions-3.2.0/tests/test_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-06-09 20:31:04.000000 django-role-permissions-3.2.0/tests/test_template_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-09 20:31:04.000000 django-role-permissions-3.2.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-06-09 20:31:04.000000 django-role-permissions-3.2.0/tests/test_verifications.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-role-permissions-3.1.1/README.md` & `django-role-permissions-3.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # django-role-permissions
 
-[![Build Status](https://travis-ci.org/vintasoftware/django-role-permissions.svg?branch=master)](https://travis-ci.org/vintasoftware/django-role-permissions)
+[![Build Status](https://github.com/vintasoftware/django-role-permissions/actions/workflows/build.yml/badge.svg)](https://github.com/vintasoftware/django-role-permissions/actions/workflows/build.yml)
+[![Coverage Status](https://coveralls.io/repos/github/vintasoftware/django-role-permissions/badge.svg?branch=master)](https://coveralls.io/github/vintasoftware/django-role-permissions?branch=master)
 [![Current version at PyPI](https://img.shields.io/pypi/v/django-role-permissions.svg)](https://pypi.python.org/pypi/django-role-permissions)
 ![Supported Python Versions](https://img.shields.io/pypi/pyversions/django-role-permissions.svg)
 
 ``django-role-permissions`` is a django app for role based permissions. It's built on top of django ``contrib.auth`` user ```Group``` and ``Permission`` functionalities and it does not add any other models to your project.  
 
 ``django-role-permissions`` supports Django versions from 1.5 until the latest.
 
@@ -23,18 +24,34 @@
 ## Running tests
 
 This packages uses `tox` to run tests on multiple evironments, please make sure they are passing before submitting a pull request.
 To run tests, install tox and run it in the command line from this project's folder:
 
 ``$ tox``
 
+## Maintainers
+
+### How to Release:
+
+#### Pre release:
+- Include the changes in `CHANGELOG`
+- Update the version in `rolepermissions/__init__.py`
+- Update the classifiers in `setup.py`
+
+#### Release:
+- Run the github action [release](https://github.com/vintasoftware/django-role-permissions/actions/workflows/release.yml)
+
+#### Post release:
+- Check if docs were updated at [readthedocs](http://django-role-permissions.readthedocs.org/).
+
 ## Help
 
 If you have any questions or need help, please send an email to: contact@vinta.com.br
 
 ## Commercial Support
-[![alt text](https://avatars2.githubusercontent.com/u/5529080?s=200&v=4 "Vinta Logo")](https://vintasoftware.com)
 
-This project, as other Vinta open-source projects, is used in products of Vinta's clients. We are always looking for exciting work, so if you need any commercial support, feel free to get in touch: contact@vinta.com.br
+[![alt text](https://avatars2.githubusercontent.com/u/5529080?s=80&v=4 "Vinta Logo")](https://www.vinta.com.br/)
+
+This project is maintained by [Vinta Software](https://www.vinta.com.br/) and is used in products of Vinta's clients. We are always looking for exciting work, so if you need any commercial support, feel free to get in touch: contact@vinta.com.br
 
 Copyright (c) 2019 Vinta Serviços e Soluções Tecnológicas Ltda.
 [MIT License](LICENSE.txt)
```

### Comparing `django-role-permissions-3.1.1/setup.py` & `django-role-permissions-3.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 import sys
 
 
 package = 'rolepermissions'
 
 requirements = [
     'Django>=1.5',
-    'django-discover-runner',
-    'six',
 ]
 test_requirements = [
     'model-mommy==1.3.1',
     'mock'
 ]
 
 
@@ -48,41 +46,38 @@
 
     filepaths = []
     for base, filenames in walk:
         filepaths.extend([os.path.join(base, filename)
                           for filename in filenames])
     return {package: filepaths}
 
-# python setup.py register
-if sys.argv[-1] == 'publish':
-    os.system("python setup.py sdist upload")
-    args = {'version': get_version(package)}
-    print("You probably want to also tag the version now:")
-    print("  git tag -a %(version)s -m 'version %(version)s'" % args)
-    print("  git push --tags")
+
+if sys.argv[-1] == 'version':
+    print(get_version(package))
     sys.exit()
 
 
 setup(
     name='django-role-permissions',
     version=get_version(package),
     url='http://github.com/vintasoftware/django-role-permissions',
     license='MIT',
     description='A django app for role based permissions.',
+    long_description_content_type="text/markdown",
     author='Filipe Ximenes',
     author_email='filipeximenes@gmail.com',
     packages=get_packages(package),
     package_data=get_package_data(package),
     install_requires=requirements,
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
-    test_suite='rolepermissions.tests',
-    tests_require=test_requirements
 )
```

### Comparing `django-role-permissions-3.1.1/rolepermissions/templatetags/permission_tags.py` & `django-role-permissions-3.2.0/rolepermissions/templatetags/permission_tags.py`

 * *Files identical despite different names*

### Comparing `django-role-permissions-3.1.1/rolepermissions/mixins.py` & `django-role-permissions-3.2.0/rolepermissions/mixins.py`

 * *Files identical despite different names*

### Comparing `django-role-permissions-3.1.1/rolepermissions/checkers.py` & `django-role-permissions-3.2.0/rolepermissions/checkers.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 def has_permission(user, permission_name):
     """Check if a user has a given permission."""
     if _check_superpowers(user):
         return True
 
     return permission_name in available_perm_names(user)
 
+
 def has_object_permission(checker_name, user, obj):
     """Check if a user has permission to perform an action on an object."""
     if _check_superpowers(user):
         return True
 
     checker = PermissionsManager.retrieve_checker(checker_name)
     user_roles = get_user_roles(user)
```

### Comparing `django-role-permissions-3.1.1/rolepermissions/roles.py` & `django-role-permissions-3.2.0/rolepermissions/roles.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from __future__ import unicode_literals
 
 import inspect
 
-from six import add_metaclass
-
 from django.contrib.auth.models import Group, Permission
 from django.contrib.auth import get_user_model
 from django.contrib.contenttypes.models import ContentType
 
 from rolepermissions.utils import camelToSnake, camel_or_snake_to_title
 from rolepermissions.exceptions import RoleDoesNotExist
 
@@ -32,23 +30,33 @@
     @classmethod
     def get_roles(cls):
         return registered_roles.values()
 
 
 class RolesClassRegister(type):
 
+    @staticmethod
+    def is_abstract(meta):
+        if meta is not None:
+            return getattr(meta, 'abstract', False)
+        else:
+            return False
+
     def __new__(cls, name, parents, dct):
+        meta = dct.get("Meta", None)
         role_class = super(RolesClassRegister, cls).__new__(cls, name, parents, dct)
-        if object not in parents:
+        if not cls.is_abstract(meta):
             registered_roles[role_class.get_name()] = role_class
         return role_class
 
 
-@add_metaclass(RolesClassRegister)
-class AbstractUserRole(object):
+class AbstractUserRole(metaclass=RolesClassRegister):
+
+    class Meta:
+        abstract = True
 
     @classmethod
     def get_name(cls):
         if hasattr(cls, 'role_name'):
             return cls.role_name
 
         return camelToSnake(cls.__name__)
```

### Comparing `django-role-permissions-3.1.1/rolepermissions/tests/test_admin.py` & `django-role-permissions-3.2.0/tests/test_admin.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 from collections import namedtuple
+from io import StringIO
+
 from django.core.management import call_command
 from django.test import TestCase
 
-try:
-    # django 3 don't have django.utils.six
-    from django.utils.six import StringIO
-except ImportError:
-    from io import StringIO
-
 from django.contrib.auth import get_user_model
 from django.contrib.auth.models import Group, Permission
 
 from model_mommy import mommy
 
 from rolepermissions.roles import AbstractUserRole, get_user_roles
 from rolepermissions.admin import RolePermissionsUserAdminMixin
```

### Comparing `django-role-permissions-3.1.1/rolepermissions/tests/test_utils.py` & `django-role-permissions-3.2.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-role-permissions-3.1.1/rolepermissions/tests/test_template_tags.py` & `django-role-permissions-3.2.0/tests/test_template_tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,22 @@
 
 class TemRole1(AbstractUserRole):
     available_permissions = {
         'permission1': True,
         'permission2': True,
     }
 
+
 class TemRole2(AbstractUserRole):
     available_permissions = {
         'permission3': True,
         'permission4': False,
     }
 
+
 class TemRole3(AbstractUserRole):
     role_name = 'new_name'
     available_permissions = {
         'permission5': False,
         'permission6': False,
     }
```

### Comparing `django-role-permissions-3.1.1/rolepermissions/tests/test_decorators.py` & `django-role-permissions-3.2.0/tests/test_decorators.py`

 * *Files 12% similar despite different names*

```diff
@@ -136,14 +136,40 @@
     def get_object(self):
         return True
 
     def render_to_response(self, context, **response_kwargs):
         return HttpResponse("Test")
 
 
+class PermissionOverhiddenRedirectViewRedirectUrl(DetailView):
+
+    @method_decorator(has_permission_decorator('permission2', redirect_url='/new_redirect'))
+    def dispatch(self, request, *args, **kwargs):
+        return super(PermissionOverhiddenRedirectViewRedirectUrl, self).dispatch(request, *args, **kwargs)
+
+    def get_object(self):
+        return True
+
+    def render_to_response(self, context, **response_kwargs):
+        return HttpResponse("Test")
+
+
+class RoleOverhiddenRedirectViewRedirectUrl(DetailView):
+
+    @method_decorator(has_role_decorator('permission2', redirect_url='/new_redirect'))
+    def dispatch(self, request, *args, **kwargs):
+        return super(RoleOverhiddenRedirectViewRedirectUrl, self).dispatch(request, *args, **kwargs)
+
+    def get_object(self):
+        return True
+
+    def render_to_response(self, context, **response_kwargs):
+        return HttpResponse("Test")
+
+
 class HasPermissionDecoratorTests(TestCase):
 
     def setUp(self):
         self.user = mommy.make(get_user_model())
 
         self.factory = RequestFactory()
 
@@ -169,16 +195,16 @@
 
         with self.assertRaises(PermissionDenied):
             HasPermissionDetailView.as_view()(request)
 
 
 @override_settings(
     ROLEPERMISSIONS_REDIRECT_TO_LOGIN=True, LOGIN_URL='/login/',
-    ROOT_URLCONF='rolepermissions.tests.mock_urls')
-class RedirectToLoginTests(TestCase):
+    ROOT_URLCONF='tests.mock_urls')
+class RedirectTests(TestCase):
 
     def setUp(self):
         self.user = mommy.make(get_user_model())
 
         self.factory = RequestFactory()
 
         self.request = self.factory.get('/')
@@ -209,18 +235,32 @@
 
     def test_role_overhiding_setting(self):
         request = self.request
 
         with self.assertRaises(PermissionDenied):
             RoleOverhiddenRedirectView.as_view()(request)
 
+    def test_role_overhiding_new_redirect(self):
+        request = self.request
+
+        response = RoleOverhiddenRedirectViewRedirectUrl.as_view()(request)
+        self.assertEquals(response.status_code, 302)
+        self.assertIn('/new_redirect', response['Location'])
+
+    def test_permission_overhiding_new_redirect(self):
+        request = self.request
+
+        response = PermissionOverhiddenRedirectViewRedirectUrl.as_view()(request)
+        self.assertEquals(response.status_code, 302)
+        self.assertIn('/new_redirect', response['Location'])
+
 
 @override_settings(
     ROLEPERMISSIONS_REDIRECT_TO_LOGIN=False, LOGIN_URL='/login/',
-    ROOT_URLCONF='rolepermissions.tests.mock_urls')
+    ROOT_URLCONF='tests.mock_urls')
 class NotRedirectToLoginTests(TestCase):
 
     def setUp(self):
         self.user = mommy.make(get_user_model())
 
         self.factory = RequestFactory()
```

### Comparing `django-role-permissions-3.1.1/rolepermissions/tests/test_verifications.py` & `django-role-permissions-3.2.0/tests/test_verifications.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,20 +11,22 @@
 
 class VerRole1(AbstractUserRole):
     available_permissions = {
         'permission1': True,
         'permission2': True,
     }
 
+
 class VerRole2(AbstractUserRole):
     available_permissions = {
         'permission3': True,
         'permission4': False,
     }
 
+
 class VerRole3(AbstractUserRole):
     role_name = 'ver_new_name'
     available_permissions = {
         'permission5': False,
         'permission6': False,
     }
```

### Comparing `django-role-permissions-3.1.1/rolepermissions/tests/test_shortcuts.py` & `django-role-permissions-3.2.0/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `django-role-permissions-3.1.1/rolepermissions/tests/test_mixins.py` & `django-role-permissions-3.2.0/tests/test_mixins.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
         response = MultipleHasRoleDetailView.as_view()(request)
 
         self.assertEquals(response.status_code, 200)
 
     @override_settings(
         ROLEPERMISSIONS_REDIRECT_TO_LOGIN=True, LOGIN_URL='/login/',
-        ROOT_URLCONF='rolepermissions.tests.mock_urls')
+        ROOT_URLCONF='tests.mock_urls')
     def test_overhidden_redirect_to_login(self):
         request = self.request
 
         with self.assertRaises(PermissionDenied):
             RoleOverhiddenRedirectView.as_view()(request)
 
     def tearDown(self):
@@ -166,15 +166,15 @@
         MixRole2.assign_role_to_user(user)
 
         with self.assertRaises(PermissionDenied):
             HasPermissionDetailView.as_view()(request)
 
     @override_settings(
         ROLEPERMISSIONS_REDIRECT_TO_LOGIN=True, LOGIN_URL='/login/',
-        ROOT_URLCONF='rolepermissions.tests.mock_urls')
+        ROOT_URLCONF='tests.mock_urls')
     def test_overhidden_redirect_to_login(self):
         request = self.request
 
         with self.assertRaises(PermissionDenied):
             PermissionOverhiddenRedirectView.as_view()(request)
 
     def tearDown(self):
```

### Comparing `django-role-permissions-3.1.1/rolepermissions/tests/test_roles.py` & `django-role-permissions-3.2.0/tests/test_roles.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,20 +25,27 @@
 class RolRole3(AbstractUserRole):
     role_name = 'new_name'
     available_permissions = {
         'permission5': False,
         'permission6': False,
     }
 
+
 class RolRole4(AbstractUserRole):
     available_permissions = {
         'permission_number_7': True,
         'PermissionNumber8': True,
     }
 
+
+class AnotherAbstractRole(RolRole4):
+    class Meta:
+        abstract = True
+
+
 class AbstractUserRoleTests(TestCase):
 
     def setUp(self):
         pass
 
     def test_get_name(self):
         self.assertEquals(RolRole1.get_name(), 'rol_role1')
@@ -143,14 +150,26 @@
 
         permission_labels = [perm.name for perm in permissions]
 
         self.assertIn('Permission Number 7', permission_labels)
         self.assertIn('Permission Number8', permission_labels)
         self.assertEquals(len(permissions), 2)
 
+    def test_meta_abstract_inheritance(self):
+        self.assertTrue('rol_role1' in RolesManager.get_roles_names())
+        self.assertTrue('rol_role2' in RolesManager.get_roles_names())
+        self.assertTrue('new_name' in RolesManager.get_roles_names())
+        self.assertTrue('rol_role4' in RolesManager.get_roles_names())
+        self.assertFalse('abstract_user_role' in RolesManager.get_roles_names())
+        self.assertFalse('another_abstract_role' in RolesManager.get_roles_names())
+
+        self.assertTrue(hasattr(AbstractUserRole(), 'Meta'))
+        self.assertTrue(hasattr(RolRole4(), 'Meta'))
+        self.assertTrue(hasattr(AnotherAbstractRole(), 'Meta'))
+
 
 class RolesManagerTests(TestCase):
 
     def setUp(self):
         pass
 
     def test_retrieve_role(self):
@@ -166,26 +185,26 @@
     def test_create_default_named_permission(self):
         perm_snake, _created = get_or_create_permission("my_perm_name1")
         self.assertEqual(perm_snake.name, "My Perm Name1")
 
         perm_camel, _created = get_or_create_permission("myPermName2")
         self.assertEqual(perm_camel.name, "My Perm Name2")
 
-    def test_create_and_get_named_permission(self) :
+    def test_create_and_get_named_permission(self):
         perm1, _created = get_or_create_permission("my_perm_name", name="My Custom Name")
         self.assertEqual(perm1.name, "My Custom Name")
 
         perm2, _created = get_or_create_permission("my_perm_name", name="My Custom Name")
         self.assertEqual(perm1, perm2)
 
-    def test_create_and_get_specialty_named_permission(self) :
+    def test_create_and_get_specialty_named_permission(self):
         def name_perm(codename):
             return "Custom-"+codename
         perm, _created = get_or_create_permission("my_perm_name", name_perm)
         self.assertEqual(perm.name, "Custom-my_perm_name")
 
-    def test_backwards_compat_with_unnamed_permission(self) :
+    def test_backwards_compat_with_unnamed_permission(self):
         unnamed_perm, _created = get_or_create_permission("my_perm_name", name="")
         self.assertEqual(unnamed_perm.name, "")
 
         perm, _created = get_or_create_permission("my_perm_name")
         self.assertEqual(unnamed_perm, perm)
```

### Comparing `django-role-permissions-3.1.1/rolepermissions/tests/test_permissions.py` & `django-role-permissions-3.2.0/tests/test_permissions.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,25 +27,25 @@
             pass
 
         PermissionsManager.register_checker('func_name', func)
 
         self.assertEquals(PermissionsManager.retrieve_checker('func_name'), func)
 
     def test_restore_unregistered_function(self):
-        
+
         with self.assertRaises(CheckerNotRegistered):
             PermissionsManager.retrieve_checker('func_name')
 
 
 class RegisterObjectCheckerDecoratorTests(TestCase):
 
     def setUp(self):
         PermissionsManager._checkers = {}
 
-    def test_resgisters_function(self):
+    def test_registers_function(self):
         @register_object_checker()
         def function_name(a, b, c):
             return True
 
         self.assertIn('function_name', PermissionsManager.get_checkers())
 
         restore_function = PermissionsManager.retrieve_checker('function_name')
@@ -58,7 +58,14 @@
             return True
 
         self.assertIn('new_name', PermissionsManager.get_checkers())
 
         restore_function = PermissionsManager.retrieve_checker('new_name')
 
         self.assertTrue(restore_function('', '', ''))
+
+    def test_register_function_call(self):
+        @register_object_checker()
+        def function_name(a, b, c):
+            return True
+
+        self.assertTrue(function_name('', '', ''))
```

### Comparing `django-role-permissions-3.1.1/rolepermissions/management/commands/sync_roles.py` & `django-role-permissions-3.2.0/rolepermissions/management/commands/sync_roles.py`

 * *Files identical despite different names*

### Comparing `django-role-permissions-3.1.1/rolepermissions/admin.py` & `django-role-permissions-3.2.0/rolepermissions/admin.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from django.conf import settings
 from django.contrib import admin, auth
 from django.contrib.auth.models import Group
 from django.contrib.auth.admin import UserAdmin
+from django.contrib.admin.sites import NotRegistered
 from rolepermissions import roles
 
 ROLEPERMISSIONS_REGISTER_ADMIN = getattr(settings, 'ROLEPERMISSIONS_REGISTER_ADMIN', False)
 UserModel = auth.get_user_model()
 
 
 class RolePermissionsUserAdminMixin(object):
@@ -33,9 +34,12 @@
 
 
 class RolePermissionsUserAdmin(RolePermissionsUserAdminMixin, UserAdmin):
     pass
 
 
 if ROLEPERMISSIONS_REGISTER_ADMIN:
-    admin.site.unregister(UserModel)
+    try:
+        admin.site.unregister(UserModel)
+    except NotRegistered:
+        pass
     admin.site.register(UserModel, RolePermissionsUserAdmin)
```

### Comparing `django-role-permissions-3.1.1/rolepermissions/utils.py` & `django-role-permissions-3.2.0/rolepermissions/utils.py`

 * *Files identical despite different names*

### Comparing `django-role-permissions-3.1.1/rolepermissions/loader.py` & `django-role-permissions-3.2.0/rolepermissions/loader.py`

 * *Files identical despite different names*

### Comparing `django-role-permissions-3.1.1/rolepermissions/permissions.py` & `django-role-permissions-3.2.0/rolepermissions/permissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         raise CheckerNotRegistered('Checker with name %s was not registered' % checker_name)
 
 
 def register_object_checker(name=None):
     def fuction_decorator(func):
         checker_name = name if name else func.__name__
         PermissionsManager.register_checker(checker_name, func)
+        return func
     return fuction_decorator
 
 
 def get_permission(permission_name):
     """Get a Permission object from a permission name."""
     permission, created = get_or_create_permission(permission_name)
```

### Comparing `django-role-permissions-3.1.1/rolepermissions/decorators.py` & `django-role-permissions-3.2.0/rolepermissions/decorators.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,50 +1,42 @@
 from __future__ import unicode_literals
 
 from functools import wraps
 
 from django.conf import settings
 from django.contrib.auth.views import redirect_to_login as dj_redirect_to_login
 from django.core.exceptions import PermissionDenied
+from django.shortcuts import redirect as dj_redirect
 
 from rolepermissions.checkers import has_role, has_permission
 from rolepermissions.utils import user_is_authenticated
 
 
-def has_role_decorator(role, redirect_to_login=None):
+def _role_permission_checker(function, subject, redirect_to_login, redirect_url):
     def request_decorator(dispatch):
         @wraps(dispatch)
         def wrapper(request, *args, **kwargs):
             user = request.user
             if user_is_authenticated(user):
-                if has_role(user, role):
+                if function(user, subject):
                     return dispatch(request, *args, **kwargs)
 
+            if redirect_url:
+                return dj_redirect(redirect_url)
+
             redirect = redirect_to_login
             if redirect is None:
                 redirect = getattr(
                     settings, 'ROLEPERMISSIONS_REDIRECT_TO_LOGIN', False)
             if redirect:
                 return dj_redirect_to_login(request.get_full_path())
             raise PermissionDenied
         return wrapper
     return request_decorator
 
 
-def has_permission_decorator(permission_name, redirect_to_login=None):
-    def request_decorator(dispatch):
-        @wraps(dispatch)
-        def wrapper(request, *args, **kwargs):
-            user = request.user
-            if user_is_authenticated(user):
-                if has_permission(user, permission_name):
-                    return dispatch(request, *args, **kwargs)
+def has_role_decorator(role, redirect_to_login=None, redirect_url=None):
+    return _role_permission_checker(has_role, role, redirect_to_login, redirect_url)
 
-            redirect = redirect_to_login
-            if redirect is None:
-                redirect = getattr(
-                    settings, 'ROLEPERMISSIONS_REDIRECT_TO_LOGIN', False)
-            if redirect:
-                return dj_redirect_to_login(request.get_full_path())
-            raise PermissionDenied
-        return wrapper
-    return request_decorator
+
+def has_permission_decorator(permission_name, redirect_to_login=None, redirect_url=None):
+    return _role_permission_checker(has_permission, permission_name, redirect_to_login, redirect_url)
```

