# Comparing `tmp/mkdocs-table-of-figures-0.1.0.tar.gz` & `tmp/mkdocs-table-of-figures-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-table-of-figures-0.1.0.tar", last modified: Fri Jun  9 12:04:15 2023, max compression
+gzip compressed data, was "mkdocs-table-of-figures-0.1.1.tar", last modified: Fri Jun  9 12:08:41 2023, max compression
```

## Comparing `mkdocs-table-of-figures-0.1.0.tar` & `mkdocs-table-of-figures-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        0 2023-06-09 12:04:15.143259 mkdocs-table-of-figures-0.1.0/
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       77 2023-05-09 09:20:19.000000 mkdocs-table-of-figures-0.1.0/MANIFEST.in
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     4534 2023-06-09 12:04:15.141247 mkdocs-table-of-figures-0.1.0/PKG-INFO
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)      375 2023-06-09 12:02:43.000000 mkdocs-table-of-figures-0.1.0/changelog.md
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     1075 2023-04-28 08:21:37.000000 mkdocs-table-of-figures-0.1.0/license
-drwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        0 2023-06-09 12:04:15.063250 mkdocs-table-of-figures-0.1.0/mkdocs_table_of_figures/
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        0 2023-05-02 06:14:09.000000 mkdocs-table-of-figures-0.1.0/mkdocs_table_of_figures/__init__.py
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     5093 2023-06-09 11:31:50.000000 mkdocs-table-of-figures-0.1.0/mkdocs_table_of_figures/plugin.py
-drwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        0 2023-06-09 12:04:15.130246 mkdocs-table-of-figures-0.1.0/mkdocs_table_of_figures.egg-info/
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     4534 2023-06-09 12:04:14.000000 mkdocs-table-of-figures-0.1.0/mkdocs_table_of_figures.egg-info/PKG-INFO
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)      417 2023-06-09 12:04:14.000000 mkdocs-table-of-figures-0.1.0/mkdocs_table_of_figures.egg-info/SOURCES.txt
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        1 2023-06-09 12:04:14.000000 mkdocs-table-of-figures-0.1.0/mkdocs_table_of_figures.egg-info/dependency_links.txt
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       83 2023-06-09 12:04:14.000000 mkdocs-table-of-figures-0.1.0/mkdocs_table_of_figures.egg-info/entry_points.txt
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       14 2023-06-09 12:04:14.000000 mkdocs-table-of-figures-0.1.0/mkdocs_table_of_figures.egg-info/requires.txt
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       24 2023-06-09 12:04:14.000000 mkdocs-table-of-figures-0.1.0/mkdocs_table_of_figures.egg-info/top_level.txt
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     3324 2023-06-09 12:02:16.000000 mkdocs-table-of-figures-0.1.0/readme.md
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       38 2023-06-09 12:04:15.144250 mkdocs-table-of-figures-0.1.0/setup.cfg
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     1135 2023-05-10 13:33:31.000000 mkdocs-table-of-figures-0.1.0/setup.py
+drwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        0 2023-06-09 12:08:41.437518 mkdocs-table-of-figures-0.1.1/
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       77 2023-05-09 09:20:19.000000 mkdocs-table-of-figures-0.1.1/MANIFEST.in
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     4534 2023-06-09 12:08:41.435524 mkdocs-table-of-figures-0.1.1/PKG-INFO
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)      464 2023-06-09 12:08:25.000000 mkdocs-table-of-figures-0.1.1/changelog.md
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     1075 2023-04-28 08:21:37.000000 mkdocs-table-of-figures-0.1.1/license
+drwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        0 2023-06-09 12:08:41.325594 mkdocs-table-of-figures-0.1.1/mkdocs_table_of_figures/
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        0 2023-05-02 06:14:09.000000 mkdocs-table-of-figures-0.1.1/mkdocs_table_of_figures/__init__.py
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     5062 2023-06-09 12:07:08.000000 mkdocs-table-of-figures-0.1.1/mkdocs_table_of_figures/plugin.py
+drwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        0 2023-06-09 12:08:41.420528 mkdocs-table-of-figures-0.1.1/mkdocs_table_of_figures.egg-info/
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     4534 2023-06-09 12:08:40.000000 mkdocs-table-of-figures-0.1.1/mkdocs_table_of_figures.egg-info/PKG-INFO
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)      417 2023-06-09 12:08:40.000000 mkdocs-table-of-figures-0.1.1/mkdocs_table_of_figures.egg-info/SOURCES.txt
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        1 2023-06-09 12:08:40.000000 mkdocs-table-of-figures-0.1.1/mkdocs_table_of_figures.egg-info/dependency_links.txt
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       83 2023-06-09 12:08:40.000000 mkdocs-table-of-figures-0.1.1/mkdocs_table_of_figures.egg-info/entry_points.txt
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       14 2023-06-09 12:08:40.000000 mkdocs-table-of-figures-0.1.1/mkdocs_table_of_figures.egg-info/requires.txt
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       24 2023-06-09 12:08:40.000000 mkdocs-table-of-figures-0.1.1/mkdocs_table_of_figures.egg-info/top_level.txt
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     3324 2023-06-09 12:02:16.000000 mkdocs-table-of-figures-0.1.1/readme.md
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       38 2023-06-09 12:08:41.438525 mkdocs-table-of-figures-0.1.1/setup.cfg
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     1135 2023-06-09 12:07:19.000000 mkdocs-table-of-figures-0.1.1/setup.py
```

### Comparing `mkdocs-table-of-figures-0.1.0/PKG-INFO` & `mkdocs-table-of-figures-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-table-of-figures
-Version: 0.1.0
+Version: 0.1.1
 Summary: A MkDocs plugin listing all figures to create a table of figures page
 Home-page: https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-table-of-figures
 Author: Thibaud Briard
 Author-email: thibaud.brrd@eduge.ch
 License: MIT
 Description: # mkdocs-table-of-figures
```

### Comparing `mkdocs-table-of-figures-0.1.0/license` & `mkdocs-table-of-figures-0.1.1/license`

 * *Files identical despite different names*

### Comparing `mkdocs-table-of-figures-0.1.0/mkdocs_table_of_figures/plugin.py` & `mkdocs-table-of-figures-0.1.1/mkdocs_table_of_figures/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,14 @@
             markdown = original
         
         if self.page == page.file:
             self._logger.info(f'Populating table of figure file {self.config.file} with {self.counter} figure{"s" if self.counter else ...} ')
             markdown += f'| {self.config.figure_label} | {self.config.description_label} |\n'
             markdown += f'| -------------------------- | ------------------------------- |\n'
             for figure in self.figures:
-                print(figure)
                 markdown += f'| [{self.config.figure_label} {figure["number"]}]({figure["link"]}) | {figure["description"]} |\n'
         
         return markdown
     
     
     def on_post_build(self, config):
         # Removing temp_dir directory
```

### Comparing `mkdocs-table-of-figures-0.1.0/mkdocs_table_of_figures.egg-info/PKG-INFO` & `mkdocs-table-of-figures-0.1.1/mkdocs_table_of_figures.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-table-of-figures
-Version: 0.1.0
+Version: 0.1.1
 Summary: A MkDocs plugin listing all figures to create a table of figures page
 Home-page: https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-table-of-figures
 Author: Thibaud Briard
 Author-email: thibaud.brrd@eduge.ch
 License: MIT
 Description: # mkdocs-table-of-figures
```

### Comparing `mkdocs-table-of-figures-0.1.0/readme.md` & `mkdocs-table-of-figures-0.1.1/readme.md`

 * *Files identical despite different names*

### Comparing `mkdocs-table-of-figures-0.1.0/setup.py` & `mkdocs-table-of-figures-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import io
 
 from setuptools import setup, find_packages
 
 setup(
     name='mkdocs-table-of-figures',
-    version='0.1.0',
+    version='0.1.1',
     description='A MkDocs plugin listing all figures to create a table of figures page',
     long_description=io.open('readme.md', encoding='utf8').read(),
     long_description_content_type='text/markdown',
     keywords='mkdocs',
     url='https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-table-of-figures',
     author='Thibaud Briard',
     author_email='thibaud.brrd@eduge.ch',
```

