# Comparing `tmp/plone.subrequest-2.0.2.tar.gz` & `tmp/plone.subrequest-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.subrequest-2.0.2.tar", last modified: Tue Feb  7 22:50:40 2023, max compression
+gzip compressed data, was "plone.subrequest-2.0.3.tar", last modified: Tue Mar 14 22:42:09 2023, max compression
```

## Comparing `plone.subrequest-2.0.2.tar` & `plone.subrequest-2.0.3.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 22:50:40.204271 plone.subrequest-2.0.2/
--rw-r--r--   0 maurits    (501) staff       (20)     1019 2023-02-07 22:50:39.000000 plone.subrequest-2.0.2/.editorconfig
--rw-r--r--   0 maurits    (501) staff       (20)      190 2023-02-07 22:50:39.000000 plone.subrequest-2.0.2/.gitignore
--rw-r--r--   0 maurits    (501) staff       (20)      239 2023-02-07 22:50:39.000000 plone.subrequest-2.0.2/.meta.toml
--rw-r--r--   0 maurits    (501) staff       (20)     5693 2023-02-07 22:50:39.000000 plone.subrequest-2.0.2/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-02-07 22:50:39.000000 plone.subrequest-2.0.2/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      145 2023-02-07 22:50:39.000000 plone.subrequest-2.0.2/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    10838 2023-02-07 22:50:40.204485 plone.subrequest-2.0.2/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      279 2023-02-07 22:50:39.000000 plone.subrequest-2.0.2/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)      400 2023-02-07 22:50:39.000000 plone.subrequest-2.0.2/buildout.cfg
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 22:50:40.195732 plone.subrequest-2.0.2/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-02-07 22:50:39.000000 plone.subrequest-2.0.2/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      674 2023-02-07 22:50:39.000000 plone.subrequest-2.0.2/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)      215 2023-02-07 22:50:39.000000 plone.subrequest-2.0.2/lint-requirements.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 22:50:40.196141 plone.subrequest-2.0.2/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-02-07 22:50:39.000000 plone.subrequest-2.0.2/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 22:50:40.203898 plone.subrequest-2.0.2/plone/subrequest/
--rw-r--r--   0 maurits    (501) staff       (20)     6586 2023-02-07 22:50:39.000000 plone.subrequest-2.0.2/plone/subrequest/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)       65 2023-02-07 22:50:39.000000 plone.subrequest-2.0.2/plone/subrequest/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      135 2023-02-07 22:50:39.000000 plone.subrequest-2.0.2/plone/subrequest/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     1641 2023-02-07 22:50:39.000000 plone.subrequest-2.0.2/plone/subrequest/subresponse.py
--rw-r--r--   0 maurits    (501) staff       (20)        4 2023-02-07 22:50:39.000000 plone.subrequest-2.0.2/plone/subrequest/testfile.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4173 2023-02-07 22:50:39.000000 plone.subrequest-2.0.2/plone/subrequest/testing.py
--rw-r--r--   0 maurits    (501) staff       (20)     1886 2023-02-07 22:50:39.000000 plone.subrequest-2.0.2/plone/subrequest/testing.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     7598 2023-02-07 22:50:39.000000 plone.subrequest-2.0.2/plone/subrequest/tests.py
--rw-r--r--   0 maurits    (501) staff       (20)     3857 2023-02-07 22:50:39.000000 plone.subrequest-2.0.2/plone/subrequest/usage.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 22:50:40.199583 plone.subrequest-2.0.2/plone.subrequest.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    10838 2023-02-07 22:50:39.000000 plone.subrequest-2.0.2/plone.subrequest.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      811 2023-02-07 22:50:40.000000 plone.subrequest-2.0.2/plone.subrequest.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-02-07 22:50:39.000000 plone.subrequest-2.0.2/plone.subrequest.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2023-02-07 22:50:39.000000 plone.subrequest-2.0.2/plone.subrequest.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-02-07 22:50:39.000000 plone.subrequest-2.0.2/plone.subrequest.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-02-07 22:50:39.000000 plone.subrequest-2.0.2/plone.subrequest.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      191 2023-02-07 22:50:39.000000 plone.subrequest-2.0.2/plone.subrequest.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-02-07 22:50:39.000000 plone.subrequest-2.0.2/plone.subrequest.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)      902 2023-02-07 22:50:39.000000 plone.subrequest-2.0.2/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      215 2023-02-07 22:50:40.205522 plone.subrequest-2.0.2/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1960 2023-02-07 22:50:39.000000 plone.subrequest-2.0.2/setup.py
--rw-r--r--   0 maurits    (501) staff       (20)     1176 2023-02-07 22:50:39.000000 plone.subrequest-2.0.2/tox.ini
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 22:42:09.149941 plone.subrequest-2.0.3/
+-rw-r--r--   0 maurits    (501) staff       (20)     1019 2023-03-14 22:42:08.000000 plone.subrequest-2.0.3/.editorconfig
+-rw-r--r--   0 maurits    (501) staff       (20)      190 2023-03-14 22:42:08.000000 plone.subrequest-2.0.3/.gitignore
+-rw-r--r--   0 maurits    (501) staff       (20)      239 2023-03-14 22:42:08.000000 plone.subrequest-2.0.3/.meta.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      973 2023-03-14 22:42:08.000000 plone.subrequest-2.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 maurits    (501) staff       (20)     5802 2023-03-14 22:42:08.000000 plone.subrequest-2.0.3/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-03-14 22:42:08.000000 plone.subrequest-2.0.3/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      145 2023-03-14 22:42:08.000000 plone.subrequest-2.0.3/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    10947 2023-03-14 22:42:09.150085 plone.subrequest-2.0.3/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      279 2023-03-14 22:42:08.000000 plone.subrequest-2.0.3/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      400 2023-03-14 22:42:08.000000 plone.subrequest-2.0.3/buildout.cfg
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 22:42:09.143833 plone.subrequest-2.0.3/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-03-14 22:42:08.000000 plone.subrequest-2.0.3/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      674 2023-03-14 22:42:08.000000 plone.subrequest-2.0.3/docs/LICENSE.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      215 2023-03-14 22:42:08.000000 plone.subrequest-2.0.3/lint-requirements.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 22:42:09.144251 plone.subrequest-2.0.3/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-03-14 22:42:08.000000 plone.subrequest-2.0.3/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 22:42:09.149690 plone.subrequest-2.0.3/plone/subrequest/
+-rw-r--r--   0 maurits    (501) staff       (20)     6586 2023-03-14 22:42:08.000000 plone.subrequest-2.0.3/plone/subrequest/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)       65 2023-03-14 22:42:08.000000 plone.subrequest-2.0.3/plone/subrequest/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      135 2023-03-14 22:42:08.000000 plone.subrequest-2.0.3/plone/subrequest/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1641 2023-03-14 22:42:08.000000 plone.subrequest-2.0.3/plone/subrequest/subresponse.py
+-rw-r--r--   0 maurits    (501) staff       (20)        4 2023-03-14 22:42:08.000000 plone.subrequest-2.0.3/plone/subrequest/testfile.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4173 2023-03-14 22:42:08.000000 plone.subrequest-2.0.3/plone/subrequest/testing.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1765 2023-03-14 22:42:08.000000 plone.subrequest-2.0.3/plone/subrequest/testing.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     7598 2023-03-14 22:42:08.000000 plone.subrequest-2.0.3/plone/subrequest/tests.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3857 2023-03-14 22:42:08.000000 plone.subrequest-2.0.3/plone/subrequest/usage.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 22:42:09.146855 plone.subrequest-2.0.3/plone.subrequest.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    10947 2023-03-14 22:42:09.000000 plone.subrequest-2.0.3/plone.subrequest.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      835 2023-03-14 22:42:09.000000 plone.subrequest-2.0.3/plone.subrequest.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-14 22:42:09.000000 plone.subrequest-2.0.3/plone.subrequest.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2023-03-14 22:42:09.000000 plone.subrequest-2.0.3/plone.subrequest.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-03-14 22:42:09.000000 plone.subrequest-2.0.3/plone.subrequest.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-14 22:42:09.000000 plone.subrequest-2.0.3/plone.subrequest.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      191 2023-03-14 22:42:09.000000 plone.subrequest-2.0.3/plone.subrequest.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-03-14 22:42:09.000000 plone.subrequest-2.0.3/plone.subrequest.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      902 2023-03-14 22:42:08.000000 plone.subrequest-2.0.3/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      240 2023-03-14 22:42:09.151404 plone.subrequest-2.0.3/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1960 2023-03-14 22:42:08.000000 plone.subrequest-2.0.3/setup.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1315 2023-03-14 22:42:08.000000 plone.subrequest-2.0.3/tox.ini
```

### Comparing `plone.subrequest-2.0.2/.editorconfig` & `plone.subrequest-2.0.3/.editorconfig`

 * *Files identical despite different names*

### Comparing `plone.subrequest-2.0.2/CHANGES.rst` & `plone.subrequest-2.0.3/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.3 (2023-03-14)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (13d8d6c0)
+
+
 2.0.2 (2023-02-07)
 ------------------
 
 Bug fixes:
 
 
 - Declare dependencies as found by z3c.dependencychecker.
```

### Comparing `plone.subrequest-2.0.2/PKG-INFO` & `plone.subrequest-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.subrequest
-Version: 2.0.2
+Version: 2.0.3
 Summary: Subrequests for Zope2
 Home-page: https://github.com/plone/plone.subrequest
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone
 Platform: Any
@@ -215,14 +215,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.3 (2023-03-14)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (13d8d6c0)
+
+
 2.0.2 (2023-02-07)
 ------------------
 
 Bug fixes:
 
 
 - Declare dependencies as found by z3c.dependencychecker.
```

### Comparing `plone.subrequest-2.0.2/docs/LICENSE.GPL` & `plone.subrequest-2.0.3/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.subrequest-2.0.2/docs/LICENSE.txt` & `plone.subrequest-2.0.3/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.subrequest-2.0.2/plone/subrequest/__init__.py` & `plone.subrequest-2.0.3/plone/subrequest/__init__.py`

 * *Files identical despite different names*

### Comparing `plone.subrequest-2.0.2/plone/subrequest/subresponse.py` & `plone.subrequest-2.0.3/plone/subrequest/subresponse.py`

 * *Files identical despite different names*

### Comparing `plone.subrequest-2.0.2/plone/subrequest/testing.py` & `plone.subrequest-2.0.3/plone/subrequest/testing.py`

 * *Files identical despite different names*

### Comparing `plone.subrequest-2.0.2/plone/subrequest/testing.zcml` & `plone.subrequest-2.0.3/plone/subrequest/testing.zcml`

 * *Files 3% similar despite different names*

```diff
@@ -1,81 +1,82 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:browser="http://namespaces.zope.org/browser"
-    xmlns:zcml="http://namespaces.zope.org/zcml">
+    xmlns:zcml="http://namespaces.zope.org/zcml"
+    >
 
-    <include package="plone.subrequest" />
+  <include package="plone.subrequest" />
 
-    <browser:page
-        name="cookie"
-        for="*"
-        class="plone.subrequest.testing.CookieView"
-        permission="zope.Public"
-        />
-
-    <browser:page
-        name="parameter"
-        for="*"
-        class="plone.subrequest.testing.ParameterView"
-        permission="zope.Public"
-        />
-
-    <browser:page
-        name="url"
-        for="*"
-        class="plone.subrequest.testing.URLView"
-        permission="zope.Public"
-        />
-
-    <browser:page
-        name="response-write"
-        for="*"
-        class="plone.subrequest.testing.ResponseWriteView"
-        permission="zope.Public"
-        />
-
-    <browser:page
-        name="error"
-        for="*"
-        class="plone.subrequest.testing.ErrorView"
-        permission="zope.Public"
-        />
-
-    <browser:page
-        name="root"
-        for="OFS.Application.Application"
-        class="plone.subrequest.testing.RootView"
-        permission="zope.Public"
-        />
-
-    <browser:page
-        name="test"
-        for="*"
-        class="plone.subrequest.testing.SubrequestView"
-        permission="zope.Public"
-        />
-
-    <browser:defaultView
-        for="OFS.Folder.Folder"
-        name="test"
-        />
-
-    <browser:defaultView
-        for="OFS.Application.Application"
-        name="root"
-        />
-
-    <browser:page
-        name="custom-error"
-        for="*"
-        class="plone.subrequest.testing.CustomErrorView"
-        permission="zope.Public"
-        />
-
-    <browser:page
-        name="index.html"
-        for="plone.subrequest.testing.CustomException"
-        class="plone.subrequest.testing.CustomExceptionHandler"
-        permission="zope.Public"
-        />
+  <browser:page
+      name="cookie"
+      for="*"
+      class="plone.subrequest.testing.CookieView"
+      permission="zope.Public"
+      />
+
+  <browser:page
+      name="parameter"
+      for="*"
+      class="plone.subrequest.testing.ParameterView"
+      permission="zope.Public"
+      />
+
+  <browser:page
+      name="url"
+      for="*"
+      class="plone.subrequest.testing.URLView"
+      permission="zope.Public"
+      />
+
+  <browser:page
+      name="response-write"
+      for="*"
+      class="plone.subrequest.testing.ResponseWriteView"
+      permission="zope.Public"
+      />
+
+  <browser:page
+      name="error"
+      for="*"
+      class="plone.subrequest.testing.ErrorView"
+      permission="zope.Public"
+      />
+
+  <browser:page
+      name="root"
+      for="OFS.Application.Application"
+      class="plone.subrequest.testing.RootView"
+      permission="zope.Public"
+      />
+
+  <browser:page
+      name="test"
+      for="*"
+      class="plone.subrequest.testing.SubrequestView"
+      permission="zope.Public"
+      />
+
+  <browser:defaultView
+      name="test"
+      for="OFS.Folder.Folder"
+      />
+
+  <browser:defaultView
+      name="root"
+      for="OFS.Application.Application"
+      />
+
+  <browser:page
+      name="custom-error"
+      for="*"
+      class="plone.subrequest.testing.CustomErrorView"
+      permission="zope.Public"
+      />
+
+  <browser:page
+      name="index.html"
+      for="plone.subrequest.testing.CustomException"
+      class="plone.subrequest.testing.CustomExceptionHandler"
+      permission="zope.Public"
+      />
 
 </configure>
```

### Comparing `plone.subrequest-2.0.2/plone/subrequest/tests.py` & `plone.subrequest-2.0.3/plone/subrequest/tests.py`

 * *Files identical despite different names*

### Comparing `plone.subrequest-2.0.2/plone/subrequest/usage.rst` & `plone.subrequest-2.0.3/plone/subrequest/usage.rst`

 * *Files identical despite different names*

### Comparing `plone.subrequest-2.0.2/plone.subrequest.egg-info/PKG-INFO` & `plone.subrequest-2.0.3/plone.subrequest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.subrequest
-Version: 2.0.2
+Version: 2.0.3
 Summary: Subrequests for Zope2
 Home-page: https://github.com/plone/plone.subrequest
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone
 Platform: Any
@@ -215,14 +215,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.3 (2023-03-14)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (13d8d6c0)
+
+
 2.0.2 (2023-02-07)
 ------------------
 
 Bug fixes:
 
 
 - Declare dependencies as found by z3c.dependencychecker.
```

### Comparing `plone.subrequest-2.0.2/plone.subrequest.egg-info/SOURCES.txt` & `plone.subrequest-2.0.3/plone.subrequest.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 .editorconfig
 .gitignore
 .meta.toml
+.pre-commit-config.yaml
 CHANGES.rst
 CONTRIBUTING.rst
 MANIFEST.in
 README.rst
 buildout.cfg
 lint-requirements.txt
 pyproject.toml
```

### Comparing `plone.subrequest-2.0.2/pyproject.toml` & `plone.subrequest-2.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.subrequest-2.0.2/setup.py` & `plone.subrequest-2.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages
 from setuptools import setup
 
 import os.path
 
 
-version = "2.0.2"
+version = "2.0.3"
 
 setup(
     name="plone.subrequest",
     version=version,
     description="Subrequests for Zope2",
     long_description=(
         open("README.rst").read()
```

