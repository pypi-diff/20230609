# Comparing `tmp/mkdocs_iolanta-0.1.5.tar.gz` & `tmp/mkdocs_iolanta-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_iolanta-0.1.5.tar", max compression
+gzip compressed data, was "mkdocs_iolanta-0.1.6.tar", max compression
```

## Comparing `mkdocs_iolanta-0.1.5.tar` & `mkdocs_iolanta-0.1.6.tar`

### file list

```diff
@@ -1,36 +1,24 @@
--rw-r--r--   0        0        0        0 2023-02-11 14:16:23.494652 mkdocs_iolanta-0.1.5/README.md
--rw-r--r--   0        0        0       56 2023-03-04 13:58:27.408724 mkdocs_iolanta-0.1.5/mkdocs_iolanta/__init__.py
--rw-r--r--   0        0        0    73713 2022-04-18 14:16:56.445484 mkdocs_iolanta-0.1.5/mkdocs_iolanta/_data/foaf/foaf.json
--rw-r--r--   0        0        0     1777 2022-04-18 14:16:57.465499 mkdocs_iolanta-0.1.5/mkdocs_iolanta/_data/foaf/named-context.json
--rw-r--r--   0        0        0       63 2022-03-16 16:07:28.993380 mkdocs_iolanta-0.1.5/mkdocs_iolanta/_data/iolanta/named-context.json
--rw-r--r--   0        0        0       21 2022-04-17 16:30:40.516368 mkdocs_iolanta-0.1.5/mkdocs_iolanta/_data/octa/named-context.json
--rw-r--r--   0        0        0     2322 2022-04-18 12:18:38.419069 mkdocs_iolanta-0.1.5/mkdocs_iolanta/_data/owl/named-context.json
--rw-r--r--   0        0        0    80510 2022-04-18 12:18:32.447038 mkdocs_iolanta-0.1.5/mkdocs_iolanta/_data/owl/owl.json
--rw-r--r--   0        0        0      479 2022-04-10 18:15:30.974720 mkdocs_iolanta-0.1.5/mkdocs_iolanta/_data/rdf/named-context.json
--rw-r--r--   0        0        0    17573 2022-04-10 18:15:30.854720 mkdocs_iolanta-0.1.5/mkdocs_iolanta/_data/rdf/rdf.json
--rw-r--r--   0        0        0      522 2022-04-10 17:42:34.623897 mkdocs_iolanta-0.1.5/mkdocs_iolanta/_data/rdfs/named-context.json
--rw-r--r--   0        0        0    11693 2022-04-10 17:42:34.603897 mkdocs_iolanta-0.1.5/mkdocs_iolanta/_data/rdfs/rdfs.json
--rw-r--r--   0        0        0      459 2022-04-12 17:42:43.238139 mkdocs_iolanta-0.1.5/mkdocs_iolanta/_data/skos/named-context.json
--rw-r--r--   0        0        0    37125 2022-04-12 17:42:43.214139 mkdocs_iolanta-0.1.5/mkdocs_iolanta/_data/skos/skos.json
--rw-r--r--   0        0        0        0 2023-04-06 17:30:14.538918 mkdocs_iolanta-0.1.5/mkdocs_iolanta/cli/__init__.py
--rw-r--r--   0        0        0      240 2023-01-02 21:08:12.691702 mkdocs_iolanta-0.1.5/mkdocs_iolanta/cli/context.py
--rw-r--r--   0        0        0      572 2023-04-06 17:30:48.967161 mkdocs_iolanta-0.1.5/mkdocs_iolanta/cli/main.py
--rw-r--r--   0        0        0     1099 2023-04-06 17:31:30.131446 mkdocs_iolanta-0.1.5/mkdocs_iolanta/cli/show.py
--rw-r--r--   0        0        0       52 2023-01-02 21:08:12.695701 mkdocs_iolanta-0.1.5/mkdocs_iolanta/cli/sparql.py
--rw-r--r--   0        0        0      710 2022-12-26 16:18:11.976523 mkdocs_iolanta-0.1.5/mkdocs_iolanta/conversions.py
--rw-r--r--   0        0        0      280 2023-04-06 20:11:16.401845 mkdocs_iolanta-0.1.5/mkdocs_iolanta/data/context.yaml
--rw-r--r--   0        0        0      294 2023-04-06 17:16:48.515576 mkdocs_iolanta-0.1.5/mkdocs_iolanta/data/material.yaml
--rw-r--r--   0        0        0     2756 2023-04-06 17:16:48.535576 mkdocs_iolanta-0.1.5/mkdocs_iolanta/data/mkdocs.yaml
--rw-r--r--   0        0        0     1197 2022-12-26 16:18:12.524526 mkdocs_iolanta-0.1.5/mkdocs_iolanta/describe_documentation_page.py
--rw-r--r--   0        0        0      397 2022-12-26 16:18:11.928523 mkdocs_iolanta-0.1.5/mkdocs_iolanta/environment.py
--rw-r--r--   0        0        0       58 2023-04-06 17:17:05.331641 mkdocs_iolanta-0.1.5/mkdocs_iolanta/facets/__init__.py
--rw-r--r--   0        0        0     1049 2023-04-06 20:14:58.483785 mkdocs_iolanta-0.1.5/mkdocs_iolanta/facets/icon.py
--rw-r--r--   0        0        0      124 2023-01-28 19:41:01.565102 mkdocs_iolanta-0.1.5/mkdocs_iolanta/iolanta_plugin.py
--rw-r--r--   0        0        0      219 2022-05-07 18:17:11.544234 mkdocs_iolanta-0.1.5/mkdocs_iolanta/language_from_config.py
--rw-r--r--   0        0        0     1124 2023-03-02 21:09:44.932579 mkdocs_iolanta-0.1.5/mkdocs_iolanta/plugin.py
--rw-r--r--   0        0        0      676 2022-03-16 16:07:28.993380 mkdocs_iolanta-0.1.5/mkdocs_iolanta/storage.py
--rw-r--r--   0        0        0     1701 2022-12-26 16:18:11.880522 mkdocs_iolanta-0.1.5/mkdocs_iolanta/stored_query.py
--rw-r--r--   0        0        0     2041 2023-02-11 18:28:26.627607 mkdocs_iolanta-0.1.5/mkdocs_iolanta/types.py
--rw-r--r--   0        0        0      867 2023-04-06 20:17:59.261162 mkdocs_iolanta-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1286 1970-01-01 00:00:00.000000 mkdocs_iolanta-0.1.5/setup.py
--rw-r--r--   0        0        0      657 1970-01-01 00:00:00.000000 mkdocs_iolanta-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-02-11 14:16:23.494652 mkdocs_iolanta-0.1.6/README.md
+-rw-r--r--   0        0        0       56 2023-03-04 13:58:27.408724 mkdocs_iolanta-0.1.6/mkdocs_iolanta/__init__.py
+-rw-r--r--   0        0        0    73713 2022-04-18 14:16:56.445484 mkdocs_iolanta-0.1.6/mkdocs_iolanta/_data/foaf/foaf.json
+-rw-r--r--   0        0        0     1777 2022-04-18 14:16:57.465499 mkdocs_iolanta-0.1.6/mkdocs_iolanta/_data/foaf/named-context.json
+-rw-r--r--   0        0        0       63 2022-03-16 16:07:28.993380 mkdocs_iolanta-0.1.6/mkdocs_iolanta/_data/iolanta/named-context.json
+-rw-r--r--   0        0        0       21 2022-04-17 16:30:40.516368 mkdocs_iolanta-0.1.6/mkdocs_iolanta/_data/octa/named-context.json
+-rw-r--r--   0        0        0     2322 2022-04-18 12:18:38.419069 mkdocs_iolanta-0.1.6/mkdocs_iolanta/_data/owl/named-context.json
+-rw-r--r--   0        0        0    80510 2022-04-18 12:18:32.447038 mkdocs_iolanta-0.1.6/mkdocs_iolanta/_data/owl/owl.json
+-rw-r--r--   0        0        0      479 2022-04-10 18:15:30.974720 mkdocs_iolanta-0.1.6/mkdocs_iolanta/_data/rdf/named-context.json
+-rw-r--r--   0        0        0    17573 2022-04-10 18:15:30.854720 mkdocs_iolanta-0.1.6/mkdocs_iolanta/_data/rdf/rdf.json
+-rw-r--r--   0        0        0      522 2022-04-10 17:42:34.623897 mkdocs_iolanta-0.1.6/mkdocs_iolanta/_data/rdfs/named-context.json
+-rw-r--r--   0        0        0    11693 2022-04-10 17:42:34.603897 mkdocs_iolanta-0.1.6/mkdocs_iolanta/_data/rdfs/rdfs.json
+-rw-r--r--   0        0        0      459 2022-04-12 17:42:43.238139 mkdocs_iolanta-0.1.6/mkdocs_iolanta/_data/skos/named-context.json
+-rw-r--r--   0        0        0    37125 2022-04-12 17:42:43.214139 mkdocs_iolanta-0.1.6/mkdocs_iolanta/_data/skos/skos.json
+-rw-r--r--   0        0        0      280 2023-04-06 20:11:16.401845 mkdocs_iolanta-0.1.6/mkdocs_iolanta/data/context.yaml
+-rw-r--r--   0        0        0      294 2023-04-06 17:16:48.515576 mkdocs_iolanta-0.1.6/mkdocs_iolanta/data/material.yaml
+-rw-r--r--   0        0        0     2803 2023-06-09 17:58:41.820413 mkdocs_iolanta-0.1.6/mkdocs_iolanta/data/mkdocs.yaml
+-rw-r--r--   0        0        0       58 2023-04-06 17:17:05.331641 mkdocs_iolanta-0.1.6/mkdocs_iolanta/facets/__init__.py
+-rw-r--r--   0        0        0     1178 2023-04-06 20:30:59.062070 mkdocs_iolanta-0.1.6/mkdocs_iolanta/facets/icon.py
+-rw-r--r--   0        0        0      124 2023-01-28 19:41:01.565102 mkdocs_iolanta-0.1.6/mkdocs_iolanta/iolanta_plugin.py
+-rw-r--r--   0        0        0     1617 2023-06-09 19:09:14.898696 mkdocs_iolanta-0.1.6/mkdocs_iolanta/plugin.py
+-rw-r--r--   0        0        0      867 2023-06-09 18:03:10.209984 mkdocs_iolanta-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1264 1970-01-01 00:00:00.000000 mkdocs_iolanta-0.1.6/setup.py
+-rw-r--r--   0        0        0      657 1970-01-01 00:00:00.000000 mkdocs_iolanta-0.1.6/PKG-INFO
```

### Comparing `mkdocs_iolanta-0.1.5/mkdocs_iolanta/_data/foaf/foaf.json` & `mkdocs_iolanta-0.1.6/mkdocs_iolanta/_data/foaf/foaf.json`

 * *Files identical despite different names*

### Comparing `mkdocs_iolanta-0.1.5/mkdocs_iolanta/_data/foaf/named-context.json` & `mkdocs_iolanta-0.1.6/mkdocs_iolanta/_data/foaf/named-context.json`

 * *Files identical despite different names*

### Comparing `mkdocs_iolanta-0.1.5/mkdocs_iolanta/_data/owl/named-context.json` & `mkdocs_iolanta-0.1.6/mkdocs_iolanta/_data/owl/named-context.json`

 * *Files identical despite different names*

### Comparing `mkdocs_iolanta-0.1.5/mkdocs_iolanta/_data/owl/owl.json` & `mkdocs_iolanta-0.1.6/mkdocs_iolanta/_data/owl/owl.json`

 * *Files identical despite different names*

### Comparing `mkdocs_iolanta-0.1.5/mkdocs_iolanta/_data/rdf/rdf.json` & `mkdocs_iolanta-0.1.6/mkdocs_iolanta/_data/rdf/rdf.json`

 * *Files identical despite different names*

### Comparing `mkdocs_iolanta-0.1.5/mkdocs_iolanta/_data/rdfs/named-context.json` & `mkdocs_iolanta-0.1.6/mkdocs_iolanta/_data/rdfs/named-context.json`

 * *Files identical despite different names*

### Comparing `mkdocs_iolanta-0.1.5/mkdocs_iolanta/_data/rdfs/rdfs.json` & `mkdocs_iolanta-0.1.6/mkdocs_iolanta/_data/rdfs/rdfs.json`

 * *Files identical despite different names*

### Comparing `mkdocs_iolanta-0.1.5/mkdocs_iolanta/_data/skos/skos.json` & `mkdocs_iolanta-0.1.6/mkdocs_iolanta/_data/skos/skos.json`

 * *Files identical despite different names*

### Comparing `mkdocs_iolanta-0.1.5/mkdocs_iolanta/data/mkdocs.yaml` & `mkdocs_iolanta-0.1.6/mkdocs_iolanta/data/mkdocs.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -95,11 +95,11 @@
     $id: python://mkdocs_iolanta.facets.bool_literal.BoolLiteral
     iolanta:supports:
       $id: iolanta:html
 
 - $id: owl:propertyChainAxiom
   domain: owl:ObjectProperty
 
-- $id: mkdocs:url
-  ∘:
-    - mkdocs:subjectOf
-    - mkdocs:url
+- $id: mkdocs:position
+  rdfs:label: Page position in navigation
+  rdfs:subPropertyOf:
+    $id: schema:position
```

### Comparing `mkdocs_iolanta-0.1.5/mkdocs_iolanta/facets/icon.py` & `mkdocs_iolanta-0.1.6/mkdocs_iolanta/facets/icon.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 class MkdocsMaterialIcon(HTMLFacet):
     """
     Render a mkdocs-material icon.
 
     `<… markdown="1">` can be used to render markdown emoji inside HTML but that
     is complicated. This attribute must be set for **each** of the nested
     HTML tags.
+
+    # FIXME This is undocumented because user must find the path to the icon
+        file themselves, which is… kind of ugly.
     """
 
     def show(self) -> html_tag:
         icon_name = self.iri.removeprefix(
             'https://github.com/squidfunk/mkdocs-material/blob/master/material/.icons/',
         )
```

### Comparing `mkdocs_iolanta-0.1.5/mkdocs_iolanta/plugin.py` & `mkdocs_iolanta-0.1.6/mkdocs_iolanta/plugin.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,34 +5,51 @@
 from iolanta.iolanta import Iolanta
 from iolanta.namespaces import IOLANTA
 from iolanta_jinja2.macros import template_render
 from mkdocs.config import Config
 from mkdocs.config.defaults import MkDocsConfig
 from mkdocs.plugins import BasePlugin
 from mkdocs.structure.files import Files
+from mkdocs.structure.nav import Navigation
 
 
 class IolantaPlugin(BasePlugin):   # type: ignore
     """Integrate MkDocs + iolanta."""
 
     iolanta: Iolanta
 
-    def on_files(    # type: ignore
+    def on_files(
         self,
         files: Files,
         *,
         config: MkDocsConfig,
     ) -> Optional[Files]:
         """Construct the local iolanta instance and load files."""
         self.iolanta.add(source=Path(config.docs_dir))
+        return files
 
     def on_config(self, config: MkDocsConfig) -> Optional[Config]:
         """Expose configuration & template variables."""
         self.iolanta = Iolanta()
 
         config.extra['iolanta'] = self.iolanta
         config.extra['render'] = functools.partial(
             template_render,
             iolanta=self.iolanta,
             environments=[IOLANTA.html],
         )
         return config
+
+    def on_nav(
+        self, nav: Navigation, *, config: MkDocsConfig, files: Files,
+    ) -> Optional[Navigation]:
+        """Assign schema:url to pages."""
+        self.iolanta.add({
+            '$included': [
+                {
+                    '$id': f'file://{page.file.abs_src_path}',
+                    'mkdocs:url': f'/{page.url}',
+                }
+                for page in nav.pages
+            ],
+        })
+        return nav
```

### Comparing `mkdocs_iolanta-0.1.5/pyproject.toml` & `mkdocs_iolanta-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mkdocs-iolanta"
-version = "0.1.5"
+version = "0.1.6"
 description = "MkDocs plugin to integrate with Iolanta semantic web framework."
 authors = ["Anatoly Scherbakov <altaisoft@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "mkdocs_iolanta"}]
 
 [tool.poetry.dependencies]
```

### Comparing `mkdocs_iolanta-0.1.5/setup.py` & `mkdocs_iolanta-0.1.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['mkdocs_iolanta', 'mkdocs_iolanta.cli', 'mkdocs_iolanta.facets']
+['mkdocs_iolanta', 'mkdocs_iolanta.facets']
 
 package_data = \
 {'': ['*'],
  'mkdocs_iolanta': ['_data/foaf/*',
                     '_data/iolanta/*',
                     '_data/octa/*',
                     '_data/owl/*',
@@ -23,15 +23,15 @@
 
 entry_points = \
 {'iolanta.plugins': ['mkdocs = mkdocs_iolanta:MkdocsIolanta'],
  'mkdocs.plugins': ['iolanta = mkdocs_iolanta.plugin:IolantaPlugin']}
 
 setup_kwargs = {
     'name': 'mkdocs-iolanta',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': 'MkDocs plugin to integrate with Iolanta semantic web framework.',
     'long_description': '',
     'author': 'Anatoly Scherbakov',
     'author_email': 'altaisoft@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mkdocs_iolanta-0.1.5/PKG-INFO` & `mkdocs_iolanta-0.1.6/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-iolanta
-Version: 0.1.5
+Version: 0.1.6
 Summary: MkDocs plugin to integrate with Iolanta semantic web framework.
 License: MIT
 Author: Anatoly Scherbakov
 Author-email: altaisoft@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

