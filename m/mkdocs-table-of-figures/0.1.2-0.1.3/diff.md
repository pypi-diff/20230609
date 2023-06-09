# Comparing `tmp/mkdocs-table-of-figures-0.1.2.tar.gz` & `tmp/mkdocs-table-of-figures-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-table-of-figures-0.1.2.tar", last modified: Fri Jun  9 12:52:14 2023, max compression
+gzip compressed data, was "mkdocs-table-of-figures-0.1.3.tar", last modified: Fri Jun  9 13:22:07 2023, max compression
```

## Comparing `mkdocs-table-of-figures-0.1.2.tar` & `mkdocs-table-of-figures-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        0 2023-06-09 12:52:14.461013 mkdocs-table-of-figures-0.1.2/
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       77 2023-05-09 09:20:19.000000 mkdocs-table-of-figures-0.1.2/MANIFEST.in
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     4534 2023-06-09 12:52:14.459012 mkdocs-table-of-figures-0.1.2/PKG-INFO
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)      597 2023-06-09 12:52:02.000000 mkdocs-table-of-figures-0.1.2/changelog.md
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     1075 2023-04-28 08:21:37.000000 mkdocs-table-of-figures-0.1.2/license
-drwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        0 2023-06-09 12:52:14.365013 mkdocs-table-of-figures-0.1.2/mkdocs_table_of_figures/
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        0 2023-05-02 06:14:09.000000 mkdocs-table-of-figures-0.1.2/mkdocs_table_of_figures/__init__.py
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     5137 2023-06-09 12:48:14.000000 mkdocs-table-of-figures-0.1.2/mkdocs_table_of_figures/plugin.py
-drwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        0 2023-06-09 12:52:14.444030 mkdocs-table-of-figures-0.1.2/mkdocs_table_of_figures.egg-info/
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     4534 2023-06-09 12:52:13.000000 mkdocs-table-of-figures-0.1.2/mkdocs_table_of_figures.egg-info/PKG-INFO
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)      417 2023-06-09 12:52:13.000000 mkdocs-table-of-figures-0.1.2/mkdocs_table_of_figures.egg-info/SOURCES.txt
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        1 2023-06-09 12:52:13.000000 mkdocs-table-of-figures-0.1.2/mkdocs_table_of_figures.egg-info/dependency_links.txt
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       83 2023-06-09 12:52:13.000000 mkdocs-table-of-figures-0.1.2/mkdocs_table_of_figures.egg-info/entry_points.txt
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       14 2023-06-09 12:52:13.000000 mkdocs-table-of-figures-0.1.2/mkdocs_table_of_figures.egg-info/requires.txt
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       24 2023-06-09 12:52:13.000000 mkdocs-table-of-figures-0.1.2/mkdocs_table_of_figures.egg-info/top_level.txt
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     3324 2023-06-09 12:02:16.000000 mkdocs-table-of-figures-0.1.2/readme.md
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       38 2023-06-09 12:52:14.462014 mkdocs-table-of-figures-0.1.2/setup.cfg
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     1135 2023-06-09 12:52:06.000000 mkdocs-table-of-figures-0.1.2/setup.py
+drwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        0 2023-06-09 13:22:06.847940 mkdocs-table-of-figures-0.1.3/
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       77 2023-05-09 09:20:19.000000 mkdocs-table-of-figures-0.1.3/MANIFEST.in
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     4627 2023-06-09 13:22:06.845942 mkdocs-table-of-figures-0.1.3/PKG-INFO
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)      718 2023-06-09 13:01:16.000000 mkdocs-table-of-figures-0.1.3/changelog.md
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     1075 2023-04-28 08:21:37.000000 mkdocs-table-of-figures-0.1.3/license
+drwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        0 2023-06-09 13:22:06.729282 mkdocs-table-of-figures-0.1.3/mkdocs_table_of_figures/
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        0 2023-05-02 06:14:09.000000 mkdocs-table-of-figures-0.1.3/mkdocs_table_of_figures/__init__.py
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     5506 2023-06-09 13:21:37.000000 mkdocs-table-of-figures-0.1.3/mkdocs_table_of_figures/plugin.py
+drwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        0 2023-06-09 13:22:06.824941 mkdocs-table-of-figures-0.1.3/mkdocs_table_of_figures.egg-info/
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     4627 2023-06-09 13:22:06.000000 mkdocs-table-of-figures-0.1.3/mkdocs_table_of_figures.egg-info/PKG-INFO
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)      417 2023-06-09 13:22:06.000000 mkdocs-table-of-figures-0.1.3/mkdocs_table_of_figures.egg-info/SOURCES.txt
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        1 2023-06-09 13:22:06.000000 mkdocs-table-of-figures-0.1.3/mkdocs_table_of_figures.egg-info/dependency_links.txt
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       83 2023-06-09 13:22:06.000000 mkdocs-table-of-figures-0.1.3/mkdocs_table_of_figures.egg-info/entry_points.txt
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       14 2023-06-09 13:22:06.000000 mkdocs-table-of-figures-0.1.3/mkdocs_table_of_figures.egg-info/requires.txt
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       24 2023-06-09 13:22:06.000000 mkdocs-table-of-figures-0.1.3/mkdocs_table_of_figures.egg-info/top_level.txt
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     3403 2023-06-09 13:17:03.000000 mkdocs-table-of-figures-0.1.3/readme.md
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       38 2023-06-09 13:22:06.849941 mkdocs-table-of-figures-0.1.3/setup.cfg
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     1135 2023-06-09 13:03:27.000000 mkdocs-table-of-figures-0.1.3/setup.py
```

### Comparing `mkdocs-table-of-figures-0.1.2/PKG-INFO` & `mkdocs-table-of-figures-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-table-of-figures
-Version: 0.1.2
+Version: 0.1.3
 Summary: A MkDocs plugin listing all figures to create a table of figures page
 Home-page: https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-table-of-figures
 Author: Thibaud Briard
 Author-email: thibaud.brrd@eduge.ch
 License: MIT
 Description: # mkdocs-table-of-figures
         
@@ -43,15 +43,17 @@
         
         ## Usage
         
         Using the command `mkdocs build` or `mkdocs serve` will trigger the plugin if it has been set correctly in the config file.
         
         ## Support
         
-        This plugin currently supports the inclusion of `mermaid` diagrams.
+        This plugin currently supports markdown images and `mermaid` diagrams.
+        
+        If you don't set any alt text for the markdown image it will be ignored.
         
         To make a `mermaid` diagram detectable by this plugin, you need to give it a title just below the end of the code block like this:
         
         ``` markdown
             ``` mermaid
             sequenceDiagram
                 participant Alice
```

### Comparing `mkdocs-table-of-figures-0.1.2/changelog.md` & `mkdocs-table-of-figures-0.1.3/changelog.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on Keep a Changelog, and this project adheres to Semantic Versioning.
 
+## [0.1.3] - 2023-06-09
+
+### Fixed
+
+- integration of unwanted mermaid diagrams when title is empty in `plugin.py`
+
 ## [0.1.2] - 2023-06-09
 
 ### Fixed
 
 - relative path to local image transformed to absolute path using site_url in `plugin.py`
 
 ## [0.1.1] - 2023-06-09
@@ -20,8 +26,8 @@
 
 ### Added
 
 - `readme.md`
 - `plugin.py`
 - Support for `Mermaid` diagrams
 
-[0.1.2]: https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-table-of-figures/-/releases/v0.1.2
+[0.1.3]: https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-table-of-figures/-/releases/v0.1.3
```

### Comparing `mkdocs-table-of-figures-0.1.2/license` & `mkdocs-table-of-figures-0.1.3/license`

 * *Files identical despite different names*

### Comparing `mkdocs-table-of-figures-0.1.2/mkdocs_table_of_figures/plugin.py` & `mkdocs-table-of-figures-0.1.3/mkdocs_table_of_figures/plugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def __init__(self):
         self._logger = logging.getLogger('mkdocs.table-of-figures')
         self._logger.setLevel(logging.INFO)
 
         self.enabled = True
         self.total_time = 0
 
-        self.counter = 0
+        self.counter = 1
         self.figures = []
         self.page = None
 
     def on_files(self, files, config):
         tof = os.path.join(self.config.temp_dir, self.config.file)
 
         # Create directory if it don't exist
@@ -67,26 +67,30 @@
             matches = sorted(matches, key=lambda x: x.start())
 
             position_offset = 0
             for match in matches:
                 save = markdown
 
                 try:
-                    self.counter += 1
                     link = f'{page.abs_url}#figure-{self.counter}'
-                    if match.re.pattern == pattern_img:
+                    replacement = match.group(0)
+                    if match.re.pattern == pattern_img and match.group(1):
                         self.figures.append({"number": self.counter, "description": match.group(1), "link": link})
                         replacement = f'<figure id="figure-{self.counter}" class="figure-image">\n  <img src="{config.site_url + match.group(2)[1:] if match.group(2).startswith("/") else match.group(2)}" alt="{match.group(1)}">\n  <figcaption>{self.config.figure_label} {self.counter} - {match.group(1)}</figcaption>\n</figure>'
-                    elif match.re.pattern == pattern_mermaid:
+                    elif match.re.pattern == pattern_mermaid and match.group(2):
                         self.figures.append({"number": self.counter, "description": match.group(2), "link": link})
                         replacement = f'<figure id="figure-{self.counter}" class="figure-image">\n{match.group(1)}\n  <figcaption>{self.config.figure_label} {self.counter} - {match.group(2)}</figcaption>\n</figure>'
                     
-                    markdown = markdown[:match.start() + position_offset] + replacement + markdown[match.end() + position_offset:]
-
-                    position_offset += len(replacement) - len(match.group(0))
+                    if replacement == match.group(0):
+                        self._logger.debug(f'Ignoring image/diagram at {page.abs_url}')
+                    else:
+                        self._logger.debug(f'Formating image/diagram as figure at {page.abs_url}')
+                        self.counter += 1
+                        markdown = markdown[:match.start() + position_offset] + replacement + markdown[match.end() + position_offset:]
+                        position_offset += len(replacement) - len(match.group(0))
                 except:
                     markdown = save
                     
         except:
             markdown = original
         
         if self.page == page.file:
```

### Comparing `mkdocs-table-of-figures-0.1.2/mkdocs_table_of_figures.egg-info/PKG-INFO` & `mkdocs-table-of-figures-0.1.3/mkdocs_table_of_figures.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-table-of-figures
-Version: 0.1.2
+Version: 0.1.3
 Summary: A MkDocs plugin listing all figures to create a table of figures page
 Home-page: https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-table-of-figures
 Author: Thibaud Briard
 Author-email: thibaud.brrd@eduge.ch
 License: MIT
 Description: # mkdocs-table-of-figures
         
@@ -43,15 +43,17 @@
         
         ## Usage
         
         Using the command `mkdocs build` or `mkdocs serve` will trigger the plugin if it has been set correctly in the config file.
         
         ## Support
         
-        This plugin currently supports the inclusion of `mermaid` diagrams.
+        This plugin currently supports markdown images and `mermaid` diagrams.
+        
+        If you don't set any alt text for the markdown image it will be ignored.
         
         To make a `mermaid` diagram detectable by this plugin, you need to give it a title just below the end of the code block like this:
         
         ``` markdown
             ``` mermaid
             sequenceDiagram
                 participant Alice
```

### Comparing `mkdocs-table-of-figures-0.1.2/readme.md` & `mkdocs-table-of-figures-0.1.3/readme.md`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,17 @@
 
 ## Usage
 
 Using the command `mkdocs build` or `mkdocs serve` will trigger the plugin if it has been set correctly in the config file.
 
 ## Support
 
-This plugin currently supports the inclusion of `mermaid` diagrams.
+This plugin currently supports markdown images and `mermaid` diagrams.
+
+If you don't set any alt text for the markdown image it will be ignored.
 
 To make a `mermaid` diagram detectable by this plugin, you need to give it a title just below the end of the code block like this:
 
 ``` markdown
     ``` mermaid
     sequenceDiagram
         participant Alice
```

### Comparing `mkdocs-table-of-figures-0.1.2/setup.py` & `mkdocs-table-of-figures-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import io
 
 from setuptools import setup, find_packages
 
 setup(
     name='mkdocs-table-of-figures',
-    version='0.1.2',
+    version='0.1.3',
     description='A MkDocs plugin listing all figures to create a table of figures page',
     long_description=io.open('readme.md', encoding='utf8').read(),
     long_description_content_type='text/markdown',
     keywords='mkdocs',
     url='https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-table-of-figures',
     author='Thibaud Briard',
     author_email='thibaud.brrd@eduge.ch',
```

