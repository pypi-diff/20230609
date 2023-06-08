# Comparing `tmp/pipen_diagram-0.5.0.tar.gz` & `tmp/pipen_diagram-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipen_diagram-0.5.0.tar", max compression
+gzip compressed data, was "pipen_diagram-0.6.0.tar", max compression
```

## Comparing `pipen_diagram-0.5.0.tar` & `pipen_diagram-0.6.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rwxr-xr-x   0        0        0     1980 2023-04-16 00:08:10.887365 pipen_diagram-0.5.0/README.md
--rw-r--r--   0        0        0      147 2023-04-16 00:08:10.887365 pipen_diagram-0.5.0/pipen_diagram/__init__.py
--rw-r--r--   0        0        0     8716 2023-04-16 00:08:10.887365 pipen_diagram-0.5.0/pipen_diagram/diagram.py
--rw-r--r--   0        0        0     3553 2023-04-16 00:08:10.887365 pipen_diagram-0.5.0/pipen_diagram/entry.py
--rwxr-xr-x   0        0        0     1178 2023-04-16 00:08:10.887365 pipen_diagram-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2865 1970-01-01 00:00:00.000000 pipen_diagram-0.5.0/setup.py
--rw-r--r--   0        0        0     2701 1970-01-01 00:00:00.000000 pipen_diagram-0.5.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1979 2023-06-08 23:29:35.424049 pipen_diagram-0.6.0/README.md
+-rw-r--r--   0        0        0      147 2023-06-08 23:29:35.424049 pipen_diagram-0.6.0/pipen_diagram/__init__.py
+-rw-r--r--   0        0        0     8716 2023-06-08 23:29:35.424049 pipen_diagram-0.6.0/pipen_diagram/diagram.py
+-rw-r--r--   0        0        0     3553 2023-06-08 23:29:35.424049 pipen_diagram-0.6.0/pipen_diagram/entry.py
+-rwxr-xr-x   0        0        0     1179 2023-06-08 23:29:35.424049 pipen_diagram-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2865 1970-01-01 00:00:00.000000 pipen_diagram-0.6.0/setup.py
+-rw-r--r--   0        0        0     2701 1970-01-01 00:00:00.000000 pipen_diagram-0.6.0/PKG-INFO
```

### Comparing `pipen_diagram-0.5.0/README.md` & `pipen_diagram-0.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
 
 Pipen("MyPipeline").set_start(A).run()
 # Dark theme
 # Pipen("MyPipeline", plugin_opts={"diagram_theme": "dark"}).set_start(A).run()
 ```
 
-Running `python example.py` will generate `mypipeline_results/diagram.png`:
+Running `python example.py` will generate `MyPipeline-output/diagram.png`:
 
 | Default theme | Dark theme |
 | ----------- | ---------- |
 | ![diagram](./diagram.png) | ![diagram](./diagram_dark.png) |
 
 [1]: https://github.com/pwwang/pipen
 [2]: https://graphviz.org/
```

### Comparing `pipen_diagram-0.5.0/pipen_diagram/diagram.py` & `pipen_diagram-0.6.0/pipen_diagram/diagram.py`

 * *Files identical despite different names*

### Comparing `pipen_diagram-0.5.0/pipen_diagram/entry.py` & `pipen_diagram-0.6.0/pipen_diagram/entry.py`

 * *Files identical despite different names*

### Comparing `pipen_diagram-0.5.0/pyproject.toml` & `pipen_diagram-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "pipen-diagram"
-version = "0.5.0"
+version = "0.6.0"
 description = "Draw pipeline diagrams for pipen."
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pwwang/pipen-diagram"
 repository = "https://github.com/pwwang/pipen-diagram"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pipen = "^0.9"
+pipen = "^0.10"
 graphviz = "^0.20"
 
 [tool.poetry.build]
 generate-setup-file = true
 
 [tool.poetry.dev-dependencies]
 pytest = "^7"
```

### Comparing `pipen_diagram-0.5.0/setup.py` & `pipen_diagram-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 packages = \
 ['pipen_diagram']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['graphviz>=0.20,<0.21', 'pipen>=0.9,<0.10']
+['graphviz>=0.20,<0.21', 'pipen>=0.10,<0.11']
 
 entry_points = \
 {'pipen': ['diagram = pipen_diagram:PipenDiagram']}
 
 setup_kwargs = {
     'name': 'pipen-diagram',
-    'version': '0.5.0',
+    'version': '0.6.0',
     'description': 'Draw pipeline diagrams for pipen.',
-    'long_description': '# pipen-diagram\n\nDraw pipeline diagrams for [pipen][1].\n\n## Features\n\n- Diagram theming\n- Hiding processes from diagram\n\n## Configurations\n\n- `diagram_theme`: The name of the theme to use, or a dict of a custom theme.\n  - See `pipen_diagram/diagram.py` for the a theme definition\n  - See [https://graphviz.org/][2] for theme items\n- `diagram_savedot`: Whhether to save the dot file (for debugging purpose)\n- `diagram_hide`: Process-level item, whether to hide current process from the diagram\n\n## Installation\n\n```shell\npip install -U pipen-diagram\n```\n\n## Enabling/Disabling the plugin\n\nThe plugin is registered via entrypoints. It\'s by default enabled. To disable it:\n`plugins=[..., "no:diagram"]`, or uninstall this plugin.\n\n## Usage\n\n`example.py`\n\n```python\nfrom pipen import Proc, Pipen, ProcGroup\n\n\nclass A(Proc):\n    """Process A"""\n\n\nclass B(Proc):\n    """Process B"""\n    requires = A\n    plugin_opts = {"diagram_hide": True}\n\n\nclass PG(ProcGroup):\n    """Process Group"""\n    @ProcGroup.add_proc\n    def c(self):\n        """Process C"""\n        class C(Proc):\n            ...\n\n        return C\n\n    @ProcGroup.add_proc\n    def c1(self):\n        """Process C1"""\n        class C1(Proc):\n            requires = self.c\n            plugin_opts = {"diagram_hide": True}\n\n        return C1\n\n    @ProcGroup.add_proc\n    def d(self):\n        """Process D"""\n        class D(Proc):\n            requires = self.c1\n\n        return D\n\n\npg = PG()\npg.c.requires = B\n\n\nclass E(Proc):\n    """Process E"""\n    requires = pg.d, A\n\n\nclass F(Proc):\n    """Process F"""\n    requires = E\n\n\nPipen("MyPipeline").set_start(A).run()\n# Dark theme\n# Pipen("MyPipeline", plugin_opts={"diagram_theme": "dark"}).set_start(A).run()\n```\n\nRunning `python example.py` will generate `mypipeline_results/diagram.png`:\n\n| Default theme | Dark theme |\n| ----------- | ---------- |\n| ![diagram](./diagram.png) | ![diagram](./diagram_dark.png) |\n\n[1]: https://github.com/pwwang/pipen\n[2]: https://graphviz.org/\n',
+    'long_description': '# pipen-diagram\n\nDraw pipeline diagrams for [pipen][1].\n\n## Features\n\n- Diagram theming\n- Hiding processes from diagram\n\n## Configurations\n\n- `diagram_theme`: The name of the theme to use, or a dict of a custom theme.\n  - See `pipen_diagram/diagram.py` for the a theme definition\n  - See [https://graphviz.org/][2] for theme items\n- `diagram_savedot`: Whhether to save the dot file (for debugging purpose)\n- `diagram_hide`: Process-level item, whether to hide current process from the diagram\n\n## Installation\n\n```shell\npip install -U pipen-diagram\n```\n\n## Enabling/Disabling the plugin\n\nThe plugin is registered via entrypoints. It\'s by default enabled. To disable it:\n`plugins=[..., "no:diagram"]`, or uninstall this plugin.\n\n## Usage\n\n`example.py`\n\n```python\nfrom pipen import Proc, Pipen, ProcGroup\n\n\nclass A(Proc):\n    """Process A"""\n\n\nclass B(Proc):\n    """Process B"""\n    requires = A\n    plugin_opts = {"diagram_hide": True}\n\n\nclass PG(ProcGroup):\n    """Process Group"""\n    @ProcGroup.add_proc\n    def c(self):\n        """Process C"""\n        class C(Proc):\n            ...\n\n        return C\n\n    @ProcGroup.add_proc\n    def c1(self):\n        """Process C1"""\n        class C1(Proc):\n            requires = self.c\n            plugin_opts = {"diagram_hide": True}\n\n        return C1\n\n    @ProcGroup.add_proc\n    def d(self):\n        """Process D"""\n        class D(Proc):\n            requires = self.c1\n\n        return D\n\n\npg = PG()\npg.c.requires = B\n\n\nclass E(Proc):\n    """Process E"""\n    requires = pg.d, A\n\n\nclass F(Proc):\n    """Process F"""\n    requires = E\n\n\nPipen("MyPipeline").set_start(A).run()\n# Dark theme\n# Pipen("MyPipeline", plugin_opts={"diagram_theme": "dark"}).set_start(A).run()\n```\n\nRunning `python example.py` will generate `MyPipeline-output/diagram.png`:\n\n| Default theme | Dark theme |\n| ----------- | ---------- |\n| ![diagram](./diagram.png) | ![diagram](./diagram_dark.png) |\n\n[1]: https://github.com/pwwang/pipen\n[2]: https://graphviz.org/\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/pwwang/pipen-diagram',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pipen_diagram-0.5.0/PKG-INFO` & `pipen_diagram-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pipen-diagram
-Version: 0.5.0
+Version: 0.6.0
 Summary: Draw pipeline diagrams for pipen.
 Home-page: https://github.com/pwwang/pipen-diagram
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: graphviz (>=0.20,<0.21)
-Requires-Dist: pipen (>=0.9,<0.10)
+Requires-Dist: pipen (>=0.10,<0.11)
 Project-URL: Repository, https://github.com/pwwang/pipen-diagram
 Description-Content-Type: text/markdown
 
 # pipen-diagram
 
 Draw pipeline diagrams for [pipen][1].
 
@@ -107,15 +107,15 @@
 
 
 Pipen("MyPipeline").set_start(A).run()
 # Dark theme
 # Pipen("MyPipeline", plugin_opts={"diagram_theme": "dark"}).set_start(A).run()
 ```
 
-Running `python example.py` will generate `mypipeline_results/diagram.png`:
+Running `python example.py` will generate `MyPipeline-output/diagram.png`:
 
 | Default theme | Dark theme |
 | ----------- | ---------- |
 | ![diagram](./diagram.png) | ![diagram](./diagram_dark.png) |
 
 [1]: https://github.com/pwwang/pipen
 [2]: https://graphviz.org/
```

