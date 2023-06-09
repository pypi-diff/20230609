# Comparing `tmp/orbit_component_vcheck-1.0.2.tar.gz` & `tmp/orbit_component_vcheck-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orbit_component_vcheck-1.0.2.tar", max compression
+gzip compressed data, was "orbit_component_vcheck-1.0.9.tar", max compression
```

## Comparing `orbit_component_vcheck-1.0.2.tar` & `orbit_component_vcheck-1.0.9.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1099 2023-05-30 15:19:46.404293 orbit_component_vcheck-1.0.2/LICENSE.md
--rw-r--r--   0        0        0      332 2023-05-30 15:19:46.404293 orbit_component_vcheck-1.0.2/README.md
--rw-r--r--   0        0        0       81 2023-05-30 15:19:46.404293 orbit_component_vcheck-1.0.2/orbit_component_vcheck/__init__.py
--rw-r--r--   0        0        0     2749 2023-05-30 15:19:46.404293 orbit_component_vcheck-1.0.2/orbit_component_vcheck/plugin.py
--rw-r--r--   0        0        0      810 2023-05-30 15:19:46.404293 orbit_component_vcheck-1.0.2/orbit_component_vcheck/schema/Sessions.py
--rw-r--r--   0        0        0      554 2023-05-30 15:19:46.404293 orbit_component_vcheck-1.0.2/orbit_component_vcheck/schema/Users.py
--rw-r--r--   0        0        0     1841 2023-05-30 15:19:46.404293 orbit_component_vcheck-1.0.2/orbit_component_vcheck/schema/Versions.py
--rw-r--r--   0        0        0      206 2023-05-30 15:19:46.404293 orbit_component_vcheck-1.0.2/orbit_component_vcheck/src/cli_base.py
--rw-r--r--   0        0        0     1577 2023-05-30 15:19:46.404293 orbit_component_vcheck-1.0.2/orbit_component_vcheck/src/sessions.py
--rw-r--r--   0        0        0     2002 2023-05-30 15:19:46.404293 orbit_component_vcheck-1.0.2/orbit_component_vcheck/src/users.py
--rw-r--r--   0        0        0     1779 2023-05-30 15:19:46.404293 orbit_component_vcheck-1.0.2/orbit_component_vcheck/src/versions.py
--rw-r--r--   0        0        0     1159 2023-05-31 13:07:32.771860 orbit_component_vcheck-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1316 1970-01-01 00:00:00.000000 orbit_component_vcheck-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-05-30 15:19:46.404293 orbit_component_vcheck-1.0.9/LICENSE.md
+-rw-r--r--   0        0        0      332 2023-05-30 15:19:46.404293 orbit_component_vcheck-1.0.9/README.md
+-rw-r--r--   0        0        0       81 2023-05-30 15:19:46.404293 orbit_component_vcheck-1.0.9/orbit_component_vcheck/__init__.py
+-rw-r--r--   0        0        0     2575 2023-06-07 22:19:03.697435 orbit_component_vcheck-1.0.9/orbit_component_vcheck/plugin.py
+-rw-r--r--   0        0        0      810 2023-05-30 15:19:46.404293 orbit_component_vcheck-1.0.9/orbit_component_vcheck/schema/Sessions.py
+-rw-r--r--   0        0        0      554 2023-05-30 15:19:46.404293 orbit_component_vcheck-1.0.9/orbit_component_vcheck/schema/Users.py
+-rw-r--r--   0        0        0      270 2023-06-07 22:27:15.258913 orbit_component_vcheck-1.0.9/orbit_component_vcheck/schema/Versions.py
+-rw-r--r--   0        0        0      206 2023-05-30 15:19:46.404293 orbit_component_vcheck-1.0.9/orbit_component_vcheck/src/cli_base.py
+-rw-r--r--   0        0        0     1690 2023-06-08 10:19:55.986025 orbit_component_vcheck-1.0.9/orbit_component_vcheck/src/sessions.py
+-rw-r--r--   0        0        0     2002 2023-05-30 15:19:46.404293 orbit_component_vcheck-1.0.9/orbit_component_vcheck/src/users.py
+-rw-r--r--   0        0        0     1782 2023-06-07 15:29:05.900778 orbit_component_vcheck-1.0.9/orbit_component_vcheck/src/versions.py
+-rw-r--r--   0        0        0        0 2023-06-08 17:29:42.673123 orbit_component_vcheck-1.0.9/orbit_component_vcheck/version.py
+-rw-r--r--   0        0        0     1159 2023-06-08 17:29:42.673123 orbit_component_vcheck-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1316 1970-01-01 00:00:00.000000 orbit_component_vcheck-1.0.9/PKG-INFO
```

### Comparing `orbit_component_vcheck-1.0.2/LICENSE.md` & `orbit_component_vcheck-1.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `orbit_component_vcheck-1.0.2/orbit_component_vcheck/plugin.py` & `orbit_component_vcheck-1.0.9/orbit_component_vcheck/plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from orbit_component_base.src.orbit_plugin import PluginBase, ArgsBase
-from orbit_component_vcheck.schema.Versions import VersionsCollection
+from orbit_component_base.schema.OrbitVersions import VersionsCollection
 from orbit_component_vcheck.schema.Sessions import SessionsCollection
 from orbit_component_vcheck.schema.Users import UsersCollection
 from orbit_component_vcheck.src.users import Users
 from orbit_component_vcheck.src.versions import Versions
 from orbit_component_vcheck.src.sessions import Sessions
 
 
@@ -12,17 +12,14 @@
     NAMESPACE = 'vcheck'
     COLLECTIONS = [
         VersionsCollection,
         UsersCollection,
         SessionsCollection
     ]
 
-    async def on_get_version (self, sid, product, version):
-        return await VersionsCollection(sid=sid, session=await self.get_session(sid)).get_version(product, version)
-
 
 class Args (ArgsBase):
         
     def setup (self):
         self._parser.add_argument("--vc-users", action='store_true', help="List version check users")
         self._parser.add_argument("--vc-versions", action='store_true', help="List version check versions")
         self._parser.add_argument("--vc-sessions", action='store_true', help="List version check sessions")
```

### Comparing `orbit_component_vcheck-1.0.2/orbit_component_vcheck/schema/Sessions.py` & `orbit_component_vcheck-1.0.9/orbit_component_vcheck/schema/Sessions.py`

 * *Files identical despite different names*

### Comparing `orbit_component_vcheck-1.0.2/orbit_component_vcheck/schema/Users.py` & `orbit_component_vcheck-1.0.9/orbit_component_vcheck/schema/Users.py`

 * *Files identical despite different names*

### Comparing `orbit_component_vcheck-1.0.2/orbit_component_vcheck/src/sessions.py` & `orbit_component_vcheck-1.0.9/orbit_component_vcheck/src/sessions.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,24 +15,26 @@
             title_style='bold green',
             caption=f'authentication="{world.conf.authentication}"',
             caption_style='bold magenta'
         )
         rstyle = 'cyan'
         hstyle = 'deep_sky_blue4'
         table.add_column('Session Id', style=rstyle, header_style=hstyle, no_wrap=True)
+        table.add_column('Namespace',  style=rstyle, header_style=hstyle, no_wrap=True)
         table.add_column('Host Id',    style=rstyle, header_style=hstyle, no_wrap=True)
         table.add_column('Start Time', style=rstyle, header_style=hstyle, no_wrap=True)
         table.add_column('Vendor',     style=rstyle, header_style=hstyle, no_wrap=True)
         table.add_column('Platform',   style=rstyle, header_style=hstyle, no_wrap=True)
         table.add_column('Language',   style=rstyle, header_style=hstyle, no_wrap=True)
         table.add_column('Client',     style=rstyle, header_style=hstyle, no_wrap=True)
         for result in SessionsCollection():
             doc = result.doc
             table.add_row(
                 doc._sid,
+                doc._ns,
                 doc._host_id,
                 doc.when,
                 doc._vendor,
                 doc._platform,
                 doc._language,
                 doc._product)
         Console().print(table)
```

### Comparing `orbit_component_vcheck-1.0.2/orbit_component_vcheck/src/users.py` & `orbit_component_vcheck-1.0.9/orbit_component_vcheck/src/users.py`

 * *Files identical despite different names*

### Comparing `orbit_component_vcheck-1.0.2/orbit_component_vcheck/src/versions.py` & `orbit_component_vcheck-1.0.9/orbit_component_vcheck/src/versions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from orbit_component_vcheck.schema.Versions import VersionsCollection, VersionsTable
+from orbit_component_base.schema.OrbitVersions import VersionsCollection, VersionsTable
 from orbit_component_vcheck.src.cli_base import CliBase
 from rich.console import Console
 from rich.table import Table
 from datetime import datetime
 
 
 class Versions (CliBase):
```

### Comparing `orbit_component_vcheck-1.0.2/pyproject.toml` & `orbit_component_vcheck-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "orbit-component-vcheck"
-version = "1.0.2"
+version = "1.0.9"
 description = "Orbit Component to track product versions"
 authors = ["Gareth Bult <gareth@madpenguin.uk>"]
 license = "MIT"
 readme = "README.md"
 include = ['README.md', 'LICENSE.md']
 packages = [{include = "orbit_component_vcheck"}]
 classifiers = [
```

### Comparing `orbit_component_vcheck-1.0.2/PKG-INFO` & `orbit_component_vcheck-1.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbit-component-vcheck
-Version: 1.0.2
+Version: 1.0.9
 Summary: Orbit Component to track product versions
 Home-page: https://gitlab.com/madpenguin/orbit-component-vcheck
 License: MIT
 Author: Gareth Bult
 Author-email: gareth@madpenguin.uk
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

