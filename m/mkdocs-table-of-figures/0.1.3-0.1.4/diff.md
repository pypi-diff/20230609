# Comparing `tmp/mkdocs-table-of-figures-0.1.3.tar.gz` & `tmp/mkdocs-table-of-figures-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-table-of-figures-0.1.3.tar", last modified: Fri Jun  9 13:22:07 2023, max compression
+gzip compressed data, was "mkdocs-table-of-figures-0.1.4.tar", last modified: Fri Jun  9 15:40:58 2023, max compression
```

## Comparing `mkdocs-table-of-figures-0.1.3.tar` & `mkdocs-table-of-figures-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        0 2023-06-09 13:22:06.847940 mkdocs-table-of-figures-0.1.3/
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       77 2023-05-09 09:20:19.000000 mkdocs-table-of-figures-0.1.3/MANIFEST.in
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     4627 2023-06-09 13:22:06.845942 mkdocs-table-of-figures-0.1.3/PKG-INFO
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)      718 2023-06-09 13:01:16.000000 mkdocs-table-of-figures-0.1.3/changelog.md
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     1075 2023-04-28 08:21:37.000000 mkdocs-table-of-figures-0.1.3/license
-drwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        0 2023-06-09 13:22:06.729282 mkdocs-table-of-figures-0.1.3/mkdocs_table_of_figures/
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        0 2023-05-02 06:14:09.000000 mkdocs-table-of-figures-0.1.3/mkdocs_table_of_figures/__init__.py
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     5506 2023-06-09 13:21:37.000000 mkdocs-table-of-figures-0.1.3/mkdocs_table_of_figures/plugin.py
-drwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        0 2023-06-09 13:22:06.824941 mkdocs-table-of-figures-0.1.3/mkdocs_table_of_figures.egg-info/
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     4627 2023-06-09 13:22:06.000000 mkdocs-table-of-figures-0.1.3/mkdocs_table_of_figures.egg-info/PKG-INFO
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)      417 2023-06-09 13:22:06.000000 mkdocs-table-of-figures-0.1.3/mkdocs_table_of_figures.egg-info/SOURCES.txt
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        1 2023-06-09 13:22:06.000000 mkdocs-table-of-figures-0.1.3/mkdocs_table_of_figures.egg-info/dependency_links.txt
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       83 2023-06-09 13:22:06.000000 mkdocs-table-of-figures-0.1.3/mkdocs_table_of_figures.egg-info/entry_points.txt
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       14 2023-06-09 13:22:06.000000 mkdocs-table-of-figures-0.1.3/mkdocs_table_of_figures.egg-info/requires.txt
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       24 2023-06-09 13:22:06.000000 mkdocs-table-of-figures-0.1.3/mkdocs_table_of_figures.egg-info/top_level.txt
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     3403 2023-06-09 13:17:03.000000 mkdocs-table-of-figures-0.1.3/readme.md
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       38 2023-06-09 13:22:06.849941 mkdocs-table-of-figures-0.1.3/setup.cfg
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     1135 2023-06-09 13:03:27.000000 mkdocs-table-of-figures-0.1.3/setup.py
+drwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        0 2023-06-09 15:40:58.459045 mkdocs-table-of-figures-0.1.4/
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       77 2023-05-09 09:20:19.000000 mkdocs-table-of-figures-0.1.4/MANIFEST.in
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     5439 2023-06-09 15:40:58.457044 mkdocs-table-of-figures-0.1.4/PKG-INFO
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)      824 2023-06-09 15:40:31.000000 mkdocs-table-of-figures-0.1.4/changelog.md
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     1075 2023-04-28 08:21:37.000000 mkdocs-table-of-figures-0.1.4/license
+drwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        0 2023-06-09 15:40:58.362122 mkdocs-table-of-figures-0.1.4/mkdocs_table_of_figures/
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        0 2023-05-02 06:14:09.000000 mkdocs-table-of-figures-0.1.4/mkdocs_table_of_figures/__init__.py
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     6482 2023-06-09 15:40:47.000000 mkdocs-table-of-figures-0.1.4/mkdocs_table_of_figures/plugin.py
+drwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        0 2023-06-09 15:40:58.441491 mkdocs-table-of-figures-0.1.4/mkdocs_table_of_figures.egg-info/
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     5439 2023-06-09 15:40:57.000000 mkdocs-table-of-figures-0.1.4/mkdocs_table_of_figures.egg-info/PKG-INFO
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)      417 2023-06-09 15:40:57.000000 mkdocs-table-of-figures-0.1.4/mkdocs_table_of_figures.egg-info/SOURCES.txt
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        1 2023-06-09 15:40:57.000000 mkdocs-table-of-figures-0.1.4/mkdocs_table_of_figures.egg-info/dependency_links.txt
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       83 2023-06-09 15:40:57.000000 mkdocs-table-of-figures-0.1.4/mkdocs_table_of_figures.egg-info/entry_points.txt
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       14 2023-06-09 15:40:57.000000 mkdocs-table-of-figures-0.1.4/mkdocs_table_of_figures.egg-info/requires.txt
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       24 2023-06-09 15:40:57.000000 mkdocs-table-of-figures-0.1.4/mkdocs_table_of_figures.egg-info/top_level.txt
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     4117 2023-06-09 15:39:23.000000 mkdocs-table-of-figures-0.1.4/readme.md
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       38 2023-06-09 15:40:58.460045 mkdocs-table-of-figures-0.1.4/setup.cfg
+-rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     1135 2023-06-09 15:40:33.000000 mkdocs-table-of-figures-0.1.4/setup.py
```

### Comparing `mkdocs-table-of-figures-0.1.3/PKG-INFO` & `mkdocs-table-of-figures-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: mkdocs-table-of-figures
-Version: 0.1.3
+Version: 0.1.4
 Summary: A MkDocs plugin listing all figures to create a table of figures page
 Home-page: https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-table-of-figures
 Author: Thibaud Briard
 Author-email: thibaud.brrd@eduge.ch
 License: MIT
 Description: # mkdocs-table-of-figures
         
-        This is a plugin that creates a `figcaption` with image `alt` and lists all figures in files into a table of figures to be integrated in Markdown pages for MkDocs.
+        This is a plugin that creates a `figcaption` with image `alt` and lists all figures in files into a table of figures to be integrated in `Markdown` pages for MkDocs.
         
         ## Setup
         
         ### Installing using pip:
         
         `pip install mkdocs-table-of-figures`
         
@@ -29,32 +29,46 @@
         
               temp_dir: "folder_name" # Optional --> Default : temp_figures
               file: "file_name" # Optional --> Default : figures.md
         ```
         
         As you can see, every option is optional, but if you want to generate a table of figures in another language than English, you will need to set up label options.
         
-        Set at least one annex to use this plugin. If you don't have any annex, don't add this plugin to the mkdocs plugins list in the config file `mkdocs.yml`.
+        Set at least one annex to use this plugin. If you don't have any annex, don't add this plugin to the `MkDocs` plugins list in the config file `mkdocs.yml`.
         
         - `title_label` - This is the title (heading 1) given to the page that will contain the table of figures.
         - `figure_label` - This is the name given to every figure right before the auto-incremented number.
         - `description_label` - This is the label given to the column containing the description of each figure (alt text).
-        - `temp_dir` - The temporary directory used to store the table of figures markdown file before rendering to HTML. Only set this option if you already have a `temp_figures` folder in the root directory (same as `mkdocs.yml`), which you should not normally have.
-        - `file` - The name of the markdown file containing the table of figures. Only set this option if you already have a `figures.md` file in the `docs` directory.
+        - `temp_dir` - The temporary directory used to store the table of figures `Markdown` file before rendering to HTML. Only set this option if you already have a `temp_figures` folder in the root directory (same as `mkdocs.yml`), which you should not normally have.
+        - `file` - The name of the `Markdown` file containing the table of figures. Only set this option if you already have a `figures.md` file in the `docs` directory.
         
         ## Usage
         
+        The plugin will only look for `Markdown` image composed of alt text. If you don't set any alt text for the `Markdown` image it will be ignored.
+        
+        There is two way of correctly rendering image stored within the docs:
+        
+        - Using url from base: this mean that you give the full path from the docs directory starting with `/` like this `/path/to/image/from/docs/image.png`
+        - With the help of `md_in_html`: there is a `Markdown` extension that you can set in `mkdocs.yml` that allow the plugin to place `Markdown` in `HTML` which allow this plugin to let `MkDocs` set relative link in src attribute properly during `HTML` rendering
+        
+        Concerning external images nothing change.
+        
+        You can set the `md_in_html` option like so :
+        
+        ``` yaml
+        markdown_extensions:
+          - md_in_html
+        ```
+        
         Using the command `mkdocs build` or `mkdocs serve` will trigger the plugin if it has been set correctly in the config file.
         
         ## Support
         
         This plugin currently supports markdown images and `mermaid` diagrams.
         
-        If you don't set any alt text for the markdown image it will be ignored.
-        
         To make a `mermaid` diagram detectable by this plugin, you need to give it a title just below the end of the code block like this:
         
         ``` markdown
             ``` mermaid
             sequenceDiagram
                 participant Alice
                 participant Bob
```

### Comparing `mkdocs-table-of-figures-0.1.3/changelog.md` & `mkdocs-table-of-figures-0.1.4/changelog.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on Keep a Changelog, and this project adheres to Semantic Versioning.
 
+## [0.1.4] - 2023-06-09
+
+### Added
+
+- md_in_html support for relative link to image in `plugin.py`
+
 ## [0.1.3] - 2023-06-09
 
 ### Fixed
 
 - integration of unwanted mermaid diagrams when title is empty in `plugin.py`
 
 ## [0.1.2] - 2023-06-09
@@ -26,8 +32,8 @@
 
 ### Added
 
 - `readme.md`
 - `plugin.py`
 - Support for `Mermaid` diagrams
 
-[0.1.3]: https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-table-of-figures/-/releases/v0.1.3
+[0.1.4]: https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-table-of-figures/-/releases/v0.1.4
```

### Comparing `mkdocs-table-of-figures-0.1.3/license` & `mkdocs-table-of-figures-0.1.4/license`

 * *Files identical despite different names*

### Comparing `mkdocs-table-of-figures-0.1.3/mkdocs_table_of_figures/plugin.py` & `mkdocs-table-of-figures-0.1.4/mkdocs_table_of_figures/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 File: mkdocs_table_of_figures/plugin.py
 Desc: This file contain the plugin used by mkdocs create the table of figures
 Author: Thibaud Briard - BRT, <thibaud.brrd@eduge.ch>
-Version: 0.1.3 - 2023-05-10
+Version: 0.1.4 - 2023-05-10
 """
 # Imports...
 import os, shutil # used to create folder and file in documentation
 import re # used to recognize markdown figure pattern
 import logging # used to log warning and errors for MkDocs among other things
 
 from mkdocs.config.base import Config as base_config # used to create an MkDocs config class derived from MkDocs config base
@@ -31,14 +31,22 @@
 
         self.enabled = True
         self.total_time = 0
 
         self.counter = 1
         self.figures = []
         self.page = None
+        self.keep_md_format = False
+        self.listening = True
+
+    def on_config(self, config):
+        if 'markdown_extensions' in config and 'md_in_html' in config.markdown_extensions:
+            self.keep_md_format = True
+        return config
+    
 
     def on_files(self, files, config):
         tof = os.path.join(self.config.temp_dir, self.config.file)
 
         # Create directory if it don't exist
         if not os.path.exists(os.path.dirname(tof)):
             os.makedirs(os.path.dirname(tof))
@@ -50,60 +58,64 @@
         # Add the tof file to the mkdocs files list
         self.page = File(self.config.file, src_dir=self.config.temp_dir, dest_dir=config.site_dir, use_directory_urls=config.use_directory_urls)
         files.append(self.page)
 
         return files
     
     def on_page_markdown(self, markdown, page, config, files):
-        original = markdown
-
-        try:
-            pattern_img = r'!\[(.*?)\]\((.+?)\)'
-            pattern_mermaid = r'^(``` ?mermaid\r?\n.*?```)$\r?\n^(.*?)$'
-            
-            matches = []
-            matches.extend(re.finditer(pattern_img, markdown, flags= re.IGNORECASE))
-            matches.extend(re.finditer(pattern_mermaid, markdown, flags= re.MULTILINE | re.DOTALL))
-
-            matches = sorted(matches, key=lambda x: x.start())
-
-            position_offset = 0
-            for match in matches:
-                save = markdown
-
+        if self.listening:
+            if self.page == page.file:
+                self._logger.info(f'Populating table of figure file {self.config.file} with {self.counter} figure{"s" if self.counter else ""} ')
+                markdown += f'| {self.config.figure_label} | {self.config.description_label} |\n'
+                markdown += f'| -------------------------- | ------------------------------- |\n'
+                for figure in self.figures:
+                    markdown += f'| [{self.config.figure_label} {figure["number"]}]({figure["link"]}) | {figure["description"]} |\n'
+                
+                self.listening = False
+            else:
+                original = markdown
                 try:
-                    link = f'{page.abs_url}#figure-{self.counter}'
-                    replacement = match.group(0)
-                    if match.re.pattern == pattern_img and match.group(1):
-                        self.figures.append({"number": self.counter, "description": match.group(1), "link": link})
-                        replacement = f'<figure id="figure-{self.counter}" class="figure-image">\n  <img src="{config.site_url + match.group(2)[1:] if match.group(2).startswith("/") else match.group(2)}" alt="{match.group(1)}">\n  <figcaption>{self.config.figure_label} {self.counter} - {match.group(1)}</figcaption>\n</figure>'
-                    elif match.re.pattern == pattern_mermaid and match.group(2):
-                        self.figures.append({"number": self.counter, "description": match.group(2), "link": link})
-                        replacement = f'<figure id="figure-{self.counter}" class="figure-image">\n{match.group(1)}\n  <figcaption>{self.config.figure_label} {self.counter} - {match.group(2)}</figcaption>\n</figure>'
+                    pattern_img = r'!\[(.*?)\]\((.+?)\)'
+                    pattern_mermaid = r'^(``` ?mermaid\r?\n.*?```)$\r?\n^(.*?)$'
                     
-                    if replacement == match.group(0):
-                        self._logger.debug(f'Ignoring image/diagram at {page.abs_url}')
-                    else:
-                        self._logger.debug(f'Formating image/diagram as figure at {page.abs_url}')
-                        self.counter += 1
-                        markdown = markdown[:match.start() + position_offset] + replacement + markdown[match.end() + position_offset:]
-                        position_offset += len(replacement) - len(match.group(0))
+                    matches = []
+                    matches.extend(re.finditer(pattern_img, markdown, flags= re.IGNORECASE))
+                    matches.extend(re.finditer(pattern_mermaid, markdown, flags= re.MULTILINE | re.DOTALL))
+
+                    matches = sorted(matches, key=lambda x: x.start())
+
+                    position_offset = 0
+                    for match in matches:
+                        checkpoint = markdown
+
+                        try:
+                            link = f'{page.abs_url}#figure-{self.counter}'
+                            replacement = match.group(0)
+                            if match.re.pattern == pattern_img and match.group(1):
+                                self.figures.append({"number": self.counter, "description": match.group(1), "link": link})
+                                replacement = f'<figure id="figure-{self.counter}" class="figure-image">\n  <img src="{config.site_url + match.group(2)[1:] if match.group(2).startswith("/") else match.group(2)}" alt="{match.group(1)}">\n  <figcaption>{self.config.figure_label} {self.counter} - {match.group(1)}</figcaption>\n</figure>'
+                                if self.keep_md_format:
+                                    replacement = f'<figure id="figure-{self.counter}" class="figure-image" markdown>\n  ![{match.group(1)}]({match.group(2)})\n  <figcaption>{self.config.figure_label} {self.counter} - {match.group(1)}</figcaption>\n</figure>'
+                            elif match.re.pattern == pattern_mermaid and match.group(2):
+                                self.figures.append({"number": self.counter, "description": match.group(2), "link": link})
+                                replacement = f'<figure id="figure-{self.counter}" class="figure-image">\n{match.group(1)}\n  <figcaption>{self.config.figure_label} {self.counter} - {match.group(2)}</figcaption>\n</figure>'
+                            
+                            if replacement == match.group(0):
+                                self._logger.debug(f'Ignoring image/diagram at {page.abs_url}')
+                            else:
+                                self._logger.debug(f'Formating image/diagram as figure at {page.abs_url}')
+                                self.counter += 1
+                                markdown = markdown[:match.start() + position_offset] + replacement + markdown[match.end() + position_offset:]
+                                position_offset += len(replacement) - len(match.group(0))
+                        except:
+                            markdown = checkpoint
+                            
                 except:
-                    markdown = save
-                    
-        except:
-            markdown = original
-        
-        if self.page == page.file:
-            self._logger.info(f'Populating table of figure file {self.config.file} with {self.counter} figure{"s" if self.counter else ""} ')
-            markdown += f'| {self.config.figure_label} | {self.config.description_label} |\n'
-            markdown += f'| -------------------------- | ------------------------------- |\n'
-            for figure in self.figures:
-                markdown += f'| [{self.config.figure_label} {figure["number"]}]({figure["link"]}) | {figure["description"]} |\n'
-        
+                    markdown = original
+
         return markdown
     
     
     def on_post_build(self, config):
         # Removing temp_dir directory
         self._logger.info(f'Removing tables of figure temporary directory {self.config.temp_dir}')
         if os.path.exists(self.config.temp_dir):
```

### Comparing `mkdocs-table-of-figures-0.1.3/mkdocs_table_of_figures.egg-info/PKG-INFO` & `mkdocs-table-of-figures-0.1.4/mkdocs_table_of_figures.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: mkdocs-table-of-figures
-Version: 0.1.3
+Version: 0.1.4
 Summary: A MkDocs plugin listing all figures to create a table of figures page
 Home-page: https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-table-of-figures
 Author: Thibaud Briard
 Author-email: thibaud.brrd@eduge.ch
 License: MIT
 Description: # mkdocs-table-of-figures
         
-        This is a plugin that creates a `figcaption` with image `alt` and lists all figures in files into a table of figures to be integrated in Markdown pages for MkDocs.
+        This is a plugin that creates a `figcaption` with image `alt` and lists all figures in files into a table of figures to be integrated in `Markdown` pages for MkDocs.
         
         ## Setup
         
         ### Installing using pip:
         
         `pip install mkdocs-table-of-figures`
         
@@ -29,32 +29,46 @@
         
               temp_dir: "folder_name" # Optional --> Default : temp_figures
               file: "file_name" # Optional --> Default : figures.md
         ```
         
         As you can see, every option is optional, but if you want to generate a table of figures in another language than English, you will need to set up label options.
         
-        Set at least one annex to use this plugin. If you don't have any annex, don't add this plugin to the mkdocs plugins list in the config file `mkdocs.yml`.
+        Set at least one annex to use this plugin. If you don't have any annex, don't add this plugin to the `MkDocs` plugins list in the config file `mkdocs.yml`.
         
         - `title_label` - This is the title (heading 1) given to the page that will contain the table of figures.
         - `figure_label` - This is the name given to every figure right before the auto-incremented number.
         - `description_label` - This is the label given to the column containing the description of each figure (alt text).
-        - `temp_dir` - The temporary directory used to store the table of figures markdown file before rendering to HTML. Only set this option if you already have a `temp_figures` folder in the root directory (same as `mkdocs.yml`), which you should not normally have.
-        - `file` - The name of the markdown file containing the table of figures. Only set this option if you already have a `figures.md` file in the `docs` directory.
+        - `temp_dir` - The temporary directory used to store the table of figures `Markdown` file before rendering to HTML. Only set this option if you already have a `temp_figures` folder in the root directory (same as `mkdocs.yml`), which you should not normally have.
+        - `file` - The name of the `Markdown` file containing the table of figures. Only set this option if you already have a `figures.md` file in the `docs` directory.
         
         ## Usage
         
+        The plugin will only look for `Markdown` image composed of alt text. If you don't set any alt text for the `Markdown` image it will be ignored.
+        
+        There is two way of correctly rendering image stored within the docs:
+        
+        - Using url from base: this mean that you give the full path from the docs directory starting with `/` like this `/path/to/image/from/docs/image.png`
+        - With the help of `md_in_html`: there is a `Markdown` extension that you can set in `mkdocs.yml` that allow the plugin to place `Markdown` in `HTML` which allow this plugin to let `MkDocs` set relative link in src attribute properly during `HTML` rendering
+        
+        Concerning external images nothing change.
+        
+        You can set the `md_in_html` option like so :
+        
+        ``` yaml
+        markdown_extensions:
+          - md_in_html
+        ```
+        
         Using the command `mkdocs build` or `mkdocs serve` will trigger the plugin if it has been set correctly in the config file.
         
         ## Support
         
         This plugin currently supports markdown images and `mermaid` diagrams.
         
-        If you don't set any alt text for the markdown image it will be ignored.
-        
         To make a `mermaid` diagram detectable by this plugin, you need to give it a title just below the end of the code block like this:
         
         ``` markdown
             ``` mermaid
             sequenceDiagram
                 participant Alice
                 participant Bob
```

### Comparing `mkdocs-table-of-figures-0.1.3/readme.md` & `mkdocs-table-of-figures-0.1.4/readme.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # mkdocs-table-of-figures
 
-This is a plugin that creates a `figcaption` with image `alt` and lists all figures in files into a table of figures to be integrated in Markdown pages for MkDocs.
+This is a plugin that creates a `figcaption` with image `alt` and lists all figures in files into a table of figures to be integrated in `Markdown` pages for MkDocs.
 
 ## Setup
 
 ### Installing using pip:
 
 `pip install mkdocs-table-of-figures`
 
@@ -21,32 +21,46 @@
 
       temp_dir: "folder_name" # Optional --> Default : temp_figures
       file: "file_name" # Optional --> Default : figures.md
 ```
 
 As you can see, every option is optional, but if you want to generate a table of figures in another language than English, you will need to set up label options.
 
-Set at least one annex to use this plugin. If you don't have any annex, don't add this plugin to the mkdocs plugins list in the config file `mkdocs.yml`.
+Set at least one annex to use this plugin. If you don't have any annex, don't add this plugin to the `MkDocs` plugins list in the config file `mkdocs.yml`.
 
 - `title_label` - This is the title (heading 1) given to the page that will contain the table of figures.
 - `figure_label` - This is the name given to every figure right before the auto-incremented number.
 - `description_label` - This is the label given to the column containing the description of each figure (alt text).
-- `temp_dir` - The temporary directory used to store the table of figures markdown file before rendering to HTML. Only set this option if you already have a `temp_figures` folder in the root directory (same as `mkdocs.yml`), which you should not normally have.
-- `file` - The name of the markdown file containing the table of figures. Only set this option if you already have a `figures.md` file in the `docs` directory.
+- `temp_dir` - The temporary directory used to store the table of figures `Markdown` file before rendering to HTML. Only set this option if you already have a `temp_figures` folder in the root directory (same as `mkdocs.yml`), which you should not normally have.
+- `file` - The name of the `Markdown` file containing the table of figures. Only set this option if you already have a `figures.md` file in the `docs` directory.
 
 ## Usage
 
+The plugin will only look for `Markdown` image composed of alt text. If you don't set any alt text for the `Markdown` image it will be ignored.
+
+There is two way of correctly rendering image stored within the docs:
+
+- Using url from base: this mean that you give the full path from the docs directory starting with `/` like this `/path/to/image/from/docs/image.png`
+- With the help of `md_in_html`: there is a `Markdown` extension that you can set in `mkdocs.yml` that allow the plugin to place `Markdown` in `HTML` which allow this plugin to let `MkDocs` set relative link in src attribute properly during `HTML` rendering
+
+Concerning external images nothing change.
+
+You can set the `md_in_html` option like so :
+
+``` yaml
+markdown_extensions:
+  - md_in_html
+```
+
 Using the command `mkdocs build` or `mkdocs serve` will trigger the plugin if it has been set correctly in the config file.
 
 ## Support
 
 This plugin currently supports markdown images and `mermaid` diagrams.
 
-If you don't set any alt text for the markdown image it will be ignored.
-
 To make a `mermaid` diagram detectable by this plugin, you need to give it a title just below the end of the code block like this:
 
 ``` markdown
     ``` mermaid
     sequenceDiagram
         participant Alice
         participant Bob
```

### Comparing `mkdocs-table-of-figures-0.1.3/setup.py` & `mkdocs-table-of-figures-0.1.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import io
 
 from setuptools import setup, find_packages
 
 setup(
     name='mkdocs-table-of-figures',
-    version='0.1.3',
+    version='0.1.4',
     description='A MkDocs plugin listing all figures to create a table of figures page',
     long_description=io.open('readme.md', encoding='utf8').read(),
     long_description_content_type='text/markdown',
     keywords='mkdocs',
     url='https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-table-of-figures',
     author='Thibaud Briard',
     author_email='thibaud.brrd@eduge.ch',
```

