# Comparing `tmp/liveandletdie-0.0.8.tar.gz` & `tmp/liveandletdie-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/liveandletdie/liveandletdie/dist/tmpbrfjk8mc/liveandletdie-0.0.8.tar", last modified: Mon Aug  9 15:37:45 2021, max compression
+gzip compressed data, was "liveandletdie-0.0.9.tar", last modified: Fri Jun  9 12:15:07 2023, max compression
```

## Comparing `liveandletdie-0.0.8.tar` & `liveandletdie-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 15:37:45.000000 liveandletdie-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)        3 2021-08-09 15:36:55.000000 liveandletdie-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1618 2021-08-09 15:36:55.000000 liveandletdie-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 15:37:45.000000 liveandletdie-0.0.8/liveandletdie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)       20 2021-08-09 15:37:45.000000 liveandletdie-0.0.8/liveandletdie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-08-09 15:37:45.000000 liveandletdie-0.0.8/liveandletdie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6943 2021-08-09 15:37:45.000000 liveandletdie-0.0.8/liveandletdie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-09 15:37:45.000000 liveandletdie-0.0.8/liveandletdie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      294 2021-08-09 15:37:45.000000 liveandletdie-0.0.8/liveandletdie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)       42 2021-08-09 15:36:55.000000 liveandletdie-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      897 2021-08-09 15:36:55.000000 liveandletdie-0.0.8/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6943 2021-08-09 15:37:45.000000 liveandletdie-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1076 2021-08-09 15:36:55.000000 liveandletdie-0.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5673 2021-08-09 15:36:55.000000 liveandletdie-0.0.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 15:37:45.000000 liveandletdie-0.0.8/liveandletdie/
--rw-r--r--   0 runner    (1001) docker     (121)    17463 2021-08-09 15:36:55.000000 liveandletdie-0.0.8/liveandletdie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       67 2021-08-09 15:37:45.000000 liveandletdie-0.0.8/setup.cfg
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-09 12:15:07.114973 liveandletdie-0.0.9/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1180 2023-06-09 12:14:56.000000 liveandletdie-0.0.9/CHANGELOG.rst
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1076 2023-06-09 11:32:00.000000 liveandletdie-0.0.9/LICENSE.txt
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      256 2023-06-09 12:07:14.000000 liveandletdie-0.0.9/MANIFEST.in
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     6954 2023-06-09 12:15:07.114973 liveandletdie-0.0.9/PKG-INFO
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     5673 2023-06-09 11:32:00.000000 liveandletdie-0.0.9/README.rst
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-09 12:15:07.114973 liveandletdie-0.0.9/bootstrap/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     2173 2023-06-09 11:32:00.000000 liveandletdie-0.0.9/bootstrap/bootstrapsrc.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      331 2023-06-09 11:32:00.000000 liveandletdie-0.0.9/bootstrap/makebootstrap.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)       29 2023-06-09 11:32:00.000000 liveandletdie-0.0.9/bootstrap-and-test.sh
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      132 2023-06-09 11:32:00.000000 liveandletdie-0.0.9/bootstrap.sh
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-09 12:15:07.114973 liveandletdie-0.0.9/liveandletdie/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)    17522 2023-06-09 12:04:10.000000 liveandletdie-0.0.9/liveandletdie/__init__.py
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-09 12:15:07.114973 liveandletdie-0.0.9/liveandletdie.egg-info/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     6954 2023-06-09 12:15:07.000000 liveandletdie-0.0.9/liveandletdie.egg-info/PKG-INFO
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1020 2023-06-09 12:15:07.000000 liveandletdie-0.0.9/liveandletdie.egg-info/SOURCES.txt
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)        1 2023-06-09 12:15:07.000000 liveandletdie-0.0.9/liveandletdie.egg-info/dependency_links.txt
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)       18 2023-06-09 12:15:07.000000 liveandletdie-0.0.9/liveandletdie.egg-info/requires.txt
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)       20 2023-06-09 12:15:07.000000 liveandletdie-0.0.9/liveandletdie.egg-info/top_level.txt
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)        3 2023-06-09 11:32:00.000000 liveandletdie-0.0.9/requirements.txt
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      222 2023-06-09 11:32:00.000000 liveandletdie-0.0.9/run-all.sh
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)       51 2023-06-09 11:32:00.000000 liveandletdie-0.0.9/run-lettuce.sh
+-rwxrwxr-x   0 jensens   (1000) jensens   (1000)       61 2023-06-09 11:32:00.000000 liveandletdie-0.0.9/run-pytest.sh
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)       63 2023-06-09 11:32:00.000000 liveandletdie-0.0.9/run-unittest.sh
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-09 12:15:07.110973 liveandletdie-0.0.9/sample_apps/
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-09 12:15:07.110973 liveandletdie-0.0.9/sample_apps/django/
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-09 12:15:07.114973 liveandletdie-0.0.9/sample_apps/django/example/
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-09 12:15:07.114973 liveandletdie-0.0.9/sample_apps/django/example/example/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)        0 2023-06-09 11:32:00.000000 liveandletdie-0.0.9/sample_apps/django/example/example/__init__.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     5211 2023-06-09 11:32:00.000000 liveandletdie-0.0.9/sample_apps/django/example/example/settings.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      130 2023-06-09 12:04:10.000000 liveandletdie-0.0.9/sample_apps/django/example/example/urls.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)       96 2023-06-09 11:32:00.000000 liveandletdie-0.0.9/sample_apps/django/example/example/views.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1136 2023-06-09 11:32:00.000000 liveandletdie-0.0.9/sample_apps/django/example/example/wsgi.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      250 2023-06-09 11:32:00.000000 liveandletdie-0.0.9/sample_apps/django/example/manage.py
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-09 12:15:07.114973 liveandletdie-0.0.9/sample_apps/fastapi/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      229 2023-06-09 12:04:10.000000 liveandletdie-0.0.9/sample_apps/fastapi/main.py
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-09 12:15:07.114973 liveandletdie-0.0.9/sample_apps/flask/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      516 2023-06-09 11:32:00.000000 liveandletdie-0.0.9/sample_apps/flask/main.py
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-09 12:15:07.114973 liveandletdie-0.0.9/sample_apps/gae/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      150 2023-06-09 11:32:00.000000 liveandletdie-0.0.9/sample_apps/gae/app.yaml
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      202 2023-06-09 11:32:00.000000 liveandletdie-0.0.9/sample_apps/gae/main.py
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-09 12:15:07.114973 liveandletdie-0.0.9/sample_apps/pyramid/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      665 2023-06-09 11:32:00.000000 liveandletdie-0.0.9/sample_apps/pyramid/main.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)       67 2023-06-09 12:15:07.118973 liveandletdie-0.0.9/setup.cfg
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1648 2023-06-09 12:14:56.000000 liveandletdie-0.0.9/setup.py
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-09 12:15:07.110973 liveandletdie-0.0.9/test_examples/
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-09 12:15:07.110973 liveandletdie-0.0.9/test_examples/lettuce_example/
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-09 12:15:07.114973 liveandletdie-0.0.9/test_examples/lettuce_example/features/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      765 2023-06-09 11:32:00.000000 liveandletdie-0.0.9/test_examples/lettuce_example/features/homepage.feature
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1932 2023-06-09 11:32:00.000000 liveandletdie-0.0.9/test_examples/lettuce_example/features/steps.py
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-09 12:15:07.114973 liveandletdie-0.0.9/test_examples/pytest_example/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1864 2023-06-09 12:04:10.000000 liveandletdie-0.0.9/test_examples/pytest_example/tests.py
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-09 12:15:07.114973 liveandletdie-0.0.9/test_examples/unittest_example/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     2518 2023-06-09 12:04:10.000000 liveandletdie-0.0.9/test_examples/unittest_example/tests.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      338 2023-06-09 12:04:10.000000 liveandletdie-0.0.9/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `liveandletdie-0.0.8/setup.py` & `liveandletdie-0.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 NAME = 'liveandletdie'
 HERE = os.path.dirname(__file__)
 
 
 setup(
     name=NAME,
-    version='0.0.8',
+    version='0.0.9',
     packages=find_packages(),
     install_requires=['requests', 'werkzeug'],
     package_data={'': ['*.txt', '*.rst']},
     author='Peter Hudec',
     author_email='peterhudec@peterhudec.com',
     maintainer='Authomatic Project Community',
     maintainer_email='authomaticproject@protonmail.com',
@@ -25,19 +25,20 @@
     license = 'MIT',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
-        'Programming Language :: Python :: 2.6',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: JavaScript',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content :: '
             'CGI Tools/Libraries',
-        'Topic :: Software Development :: Libraries :: Python Modules',
         'Topic :: Software Development :: Libraries',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ]
 )
```

### Comparing `liveandletdie-0.0.8/liveandletdie.egg-info/PKG-INFO` & `liveandletdie-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: liveandletdie
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simplifies launching and terminating of web development servers from BDD and functional tests.
 Home-page: http://github.com/peterhudec/liveandletdie
 Author: Peter Hudec
 Author-email: peterhudec@peterhudec.com
 Maintainer: Authomatic Project Community
 Maintainer-email: authomaticproject@protonmail.com
 License: MIT
 Keywords: Flask,Pyramid,Django,Google App Engine,GAE,BDD,TDD,functional testing,live server
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: JavaScript
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: CGI Tools/Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE.txt
 
 ================
 Live and Let Die
 ================
@@ -242,9 +242,7 @@
 Or bootstrap and run tests in one step:
 
 ::
 
     $ sh bootstrap-and-test.sh
 
 Enjoy!
-
-
```

### Comparing `liveandletdie-0.0.8/CHANGELOG.rst` & `liveandletdie-0.0.9/CHANGELOG.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+0.0.9 (2023-06-09)
+------------------
+
+* Fixed Django deprecation
+* Fixed FastAPI code
+* Fixed tests
+* removed support for Python 3.6
+* added support for Python 3.7 to 3.11
+
+
+Version 0.0.8
+-------------
+
+* changes undocumented
+
+
+Version 0.0.8
+-------------
+
+* changes undocumented
+
+
 Version 0.0.6
 -------------
 
 * The ``check()`` method now uses the `requests <python-requests.org>`__ package.
 
 Version 0.0.5
 -------------
```

### Comparing `liveandletdie-0.0.8/PKG-INFO` & `liveandletdie-0.0.9/liveandletdie.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: liveandletdie
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simplifies launching and terminating of web development servers from BDD and functional tests.
 Home-page: http://github.com/peterhudec/liveandletdie
 Author: Peter Hudec
 Author-email: peterhudec@peterhudec.com
 Maintainer: Authomatic Project Community
 Maintainer-email: authomaticproject@protonmail.com
 License: MIT
 Keywords: Flask,Pyramid,Django,Google App Engine,GAE,BDD,TDD,functional testing,live server
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: JavaScript
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: CGI Tools/Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE.txt
 
 ================
 Live and Let Die
 ================
@@ -242,9 +242,7 @@
 Or bootstrap and run tests in one step:
 
 ::
 
     $ sh bootstrap-and-test.sh
 
 Enjoy!
-
-
```

### Comparing `liveandletdie-0.0.8/LICENSE.txt` & `liveandletdie-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `liveandletdie-0.0.8/README.rst` & `liveandletdie-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `liveandletdie-0.0.8/liveandletdie/__init__.py` & `liveandletdie-0.0.9/liveandletdie/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -564,12 +564,17 @@
     def __init__(self, *args, **kwargs):
         kwargs['executable'] = 'uvicorn'
         super().__init__(*args, **kwargs)
 
     def create_command(self):
         return [
             self.executable,
-            '{}:app'.format(self.path),
-            '--host {}'.format(self.host),
-            '--port {}'.format(self.port),
+            '--app-dir',
+            os.path.dirname(self.path),
+            '--host',
+            self.host,
+            '--port',
+            str(self.port),
+            'main:app',
             '--reload',
         ]
+
```

