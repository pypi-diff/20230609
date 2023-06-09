# Comparing `tmp/pipen_board-0.4.0.tar.gz` & `tmp/pipen_board-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipen_board-0.4.0.tar", max compression
+gzip compressed data, was "pipen_board-0.5.0.tar", max compression
```

## Comparing `pipen_board-0.4.0.tar` & `pipen_board-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     6281 2023-06-08 19:05:38.669493 pipen_board-0.4.0/README.md
--rw-r--r--   0        0        0      268 2023-06-08 19:05:38.669493 pipen_board-0.4.0/pipen_board/__init__.py
--rw-r--r--   0        0        0     8985 2023-06-08 19:05:38.669493 pipen_board-0.4.0/pipen_board/apis.py
--rw-r--r--   0        0        0     4367 2023-06-08 19:05:38.669493 pipen_board-0.4.0/pipen_board/cli.py
--rw-r--r--   0        0        0    26842 2023-06-08 19:05:38.673493 pipen_board-0.4.0/pipen_board/data_manager.py
--rw-r--r--   0        0        0     6243 2023-06-08 19:05:38.673493 pipen_board-0.4.0/pipen_board/defaults.py
--rw-r--r--   0        0        0    23628 2023-06-08 19:05:38.673493 pipen_board-0.4.0/pipen_board/frontend/build/assets/favicon.png
--rw-r--r--   0        0        0   624885 2023-06-08 19:05:38.673493 pipen_board-0.4.0/pipen_board/frontend/build/assets/index.css
--rw-r--r--   0        0        0   750650 2023-06-08 19:05:38.677493 pipen_board-0.4.0/pipen_board/frontend/build/assets/index.js
--rw-r--r--   0        0        0     4128 2023-06-08 19:05:38.677493 pipen_board-0.4.0/pipen_board/frontend/build/assets/schema.json
--rw-r--r--   0        0        0      406 2023-06-08 19:05:38.677493 pipen_board-0.4.0/pipen_board/frontend/build/index.html
--rw-r--r--   0        0        0     7562 2023-06-08 19:05:38.681493 pipen_board-0.4.0/pipen_board/plugin.py
--rw-r--r--   0        0        0     3974 2023-06-08 19:05:38.681493 pipen_board-0.4.0/pipen_board/quart_app.py
--rw-r--r--   0        0        0       22 2023-06-08 19:05:38.681493 pipen_board-0.4.0/pipen_board/version.py
--rw-r--r--   0        0        0      732 2023-06-08 19:05:38.681493 pipen_board-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     7427 1970-01-01 00:00:00.000000 pipen_board-0.4.0/setup.py
--rw-r--r--   0        0        0     7058 1970-01-01 00:00:00.000000 pipen_board-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     6281 2023-06-09 07:00:34.741802 pipen_board-0.5.0/README.md
+-rw-r--r--   0        0        0      268 2023-06-09 07:00:34.741802 pipen_board-0.5.0/pipen_board/__init__.py
+-rw-r--r--   0        0        0     8985 2023-06-09 07:00:34.741802 pipen_board-0.5.0/pipen_board/apis.py
+-rw-r--r--   0        0        0     4367 2023-06-09 07:00:34.741802 pipen_board-0.5.0/pipen_board/cli.py
+-rw-r--r--   0        0        0    26842 2023-06-09 07:00:34.741802 pipen_board-0.5.0/pipen_board/data_manager.py
+-rw-r--r--   0        0        0     6243 2023-06-09 07:00:34.741802 pipen_board-0.5.0/pipen_board/defaults.py
+-rw-r--r--   0        0        0    23628 2023-06-09 07:00:34.741802 pipen_board-0.5.0/pipen_board/frontend/build/assets/favicon.png
+-rw-r--r--   0        0        0   624885 2023-06-09 07:00:34.745802 pipen_board-0.5.0/pipen_board/frontend/build/assets/index.css
+-rw-r--r--   0        0        0   750650 2023-06-09 07:00:34.749802 pipen_board-0.5.0/pipen_board/frontend/build/assets/index.js
+-rw-r--r--   0        0        0     4128 2023-06-09 07:00:34.749802 pipen_board-0.5.0/pipen_board/frontend/build/assets/schema.json
+-rw-r--r--   0        0        0      406 2023-06-09 07:00:34.749802 pipen_board-0.5.0/pipen_board/frontend/build/index.html
+-rw-r--r--   0        0        0     7562 2023-06-09 07:00:34.753802 pipen_board-0.5.0/pipen_board/plugin.py
+-rw-r--r--   0        0        0     3974 2023-06-09 07:00:34.753802 pipen_board-0.5.0/pipen_board/quart_app.py
+-rw-r--r--   0        0        0       22 2023-06-09 07:00:34.753802 pipen_board-0.5.0/pipen_board/version.py
+-rw-r--r--   0        0        0      732 2023-06-09 07:00:34.753802 pipen_board-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7427 1970-01-01 00:00:00.000000 pipen_board-0.5.0/setup.py
+-rw-r--r--   0        0        0     7058 1970-01-01 00:00:00.000000 pipen_board-0.5.0/PKG-INFO
```

### Comparing `pipen_board-0.4.0/README.md` & `pipen_board-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pipen_board-0.4.0/pipen_board/apis.py` & `pipen_board-0.5.0/pipen_board/apis.py`

 * *Files identical despite different names*

### Comparing `pipen_board-0.4.0/pipen_board/cli.py` & `pipen_board-0.5.0/pipen_board/cli.py`

 * *Files identical despite different names*

### Comparing `pipen_board-0.4.0/pipen_board/data_manager.py` & `pipen_board-0.5.0/pipen_board/data_manager.py`

 * *Files identical despite different names*

### Comparing `pipen_board-0.4.0/pipen_board/defaults.py` & `pipen_board-0.5.0/pipen_board/defaults.py`

 * *Files identical despite different names*

### Comparing `pipen_board-0.4.0/pipen_board/frontend/build/assets/favicon.png` & `pipen_board-0.5.0/pipen_board/frontend/build/assets/favicon.png`

 * *Files identical despite different names*

### Comparing `pipen_board-0.4.0/pipen_board/frontend/build/assets/index.css` & `pipen_board-0.5.0/pipen_board/frontend/build/assets/index.css`

 * *Files identical despite different names*

### Comparing `pipen_board-0.4.0/pipen_board/frontend/build/assets/index.js` & `pipen_board-0.5.0/pipen_board/frontend/build/assets/index.js`

 * *Files identical despite different names*

### Comparing `pipen_board-0.4.0/pipen_board/frontend/build/assets/schema.json` & `pipen_board-0.5.0/pipen_board/frontend/build/assets/schema.json`

 * *Files identical despite different names*

### Comparing `pipen_board-0.4.0/pipen_board/plugin.py` & `pipen_board-0.5.0/pipen_board/plugin.py`

 * *Files identical despite different names*

### Comparing `pipen_board-0.4.0/pipen_board/quart_app.py` & `pipen_board-0.5.0/pipen_board/quart_app.py`

 * *Files identical despite different names*

### Comparing `pipen_board-0.4.0/setup.py` & `pipen_board-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 packages = \
 ['pipen_board']
 
 package_data = \
 {'': ['*'], 'pipen_board': ['frontend/build/*', 'frontend/build/assets/*']}
 
 install_requires = \
-['pipen-args>=0.9.11,<0.10.0',
- 'pipen-log2file>=0.2.1,<0.3.0',
+['pipen-args>=0.10.0,<0.11.0',
+ 'pipen-log2file>=0.3.0,<0.4.0',
  'psutil>=5.9.5,<6.0.0',
  'quart>=0.18,<0.19',
  'websocket-client>=1.5,<2.0']
 
 entry_points = \
 {'pipen': ['board = pipen_board:pipen_board_plugin'],
  'pipen_cli': ['cli-board = pipen_board:PipenCliBoardPlugin']}
 
 setup_kwargs = {
     'name': 'pipen-board',
-    'version': '0.4.0',
+    'version': '0.5.0',
     'description': 'Visualization configuration and running of pipen pipelines on the web',
     'long_description': '# pipen-board\n\nVisualize configuration and running of [pipen][1] pipelines on the web.\n\n## Installation\n\n```bash\npip install pipen-board\n```\n\n## Usage\n\n```bash\n$ pipen board --help\nUsage: pipen board [options] <pipeline> -- [pipeline options]\n\nVisualize configuration and running of pipen pipelines on the web\n\nRequired Arguments:\n  pipeline              The pipeline and the CLI arguments to run the pipeline. For the\n                        pipeline either `/path/to/pipeline.py:<pipeline>` or\n                        `<module.submodule>:<pipeline>` `<pipeline>` must be an instance of\n                        `Pipen` and running the pipeline should be called under `__name__ ==\n                        \'__main__\'.\n\nOptions:\n  -h, --help            show help message and exit\n  --port PORT           Port to serve the UI wizard [default: 18521]\n  --name NAME           The name of the pipeline. Default to the pipeline class name. You\n                        can use a different name to associate with a different set of\n                        configurations.\n  --additional FILE     Additional arguments for the pipeline, in YAML, INI, JSON or TOML\n                        format. Can have sections `ADDITIONAL_OPTIONS` and `RUNNING_OPTIONS`\n  --dev                 Run the pipeline in development mode. This will print verbosal\n                        logging information and reload the pipeline if a new instantce\n                        starts when page reloads.\n  --root ROOT           The root directory of the pipeline. [default: .]\n  --loglevel {auto,debug,info,warning,error,critical}\n                        Logging level. If `auto`, set to `debug` if `--dev` is set,\n                        otherwise `info` [default: auto]\n```\n\n## Describing arguments in docstring\n\n### Docstring schema\n\n```python\nclass ProcessOrProcessGroup:\n    """Short summary\n\n    Long description\n    Long description\n\n    Args:\n        arg1 (<metadata>): description\n            - subarg1 (<metadata>): description\n            - subarg2 (<metadata>): description\n        arg2 (<metadata>): description\n\n    <Other Sections>:\n        <content>\n    """\n```\n\nThe metadata can have multiple attributes, separated by semicolon (`;`). For example:\n\n```\narg1 (action=ns;required): description\n```\n\n### Marks\n\nYou can mark a process using `pipen.utils.mark(<mark>=<value>)` as a decorator to decorate a process. For example:\n\n```python\nfrom pipen import Proc\nfrom pipen.utils import mark\n\n@mark(board_config_no_input=True)\nclass MyProc(Proc):\n    pass\n```\n\nAvailable marks:\n\n- `board_config_no_input`: Whether to show the input section for the process in configuation page. Only affects the start processes. Default to `False`.\n- `board_config_hidden`: Whether to hide the process options in the configuration page. Note that the process is still visible in the process list. Default to `False`.\n\n### Metadata for arguments\n\n\n| Name     | Description | Allowed values |\n| -------- | ----------- | -------------- |\n| `action` | Like the `action` argument in [`argx`][2]*. | `store_true`, `store_false`, `ns`, `namespace`, `append`, `extend`, `clear_append`, `clear_extend` (other values are allowed but ignore, they may be effective for CLI use) |\n| `btype`  | Board type (option type specified directly). If specified, `action` will be ignored | `ns`, `choice`, `mchoice`, `array`, `list`, `json`, `int`, `float`, `bool`, `str`, `text`, `auto`* |\n| `type` | Fallback for `action` and `btype` | Same as `btype` |\n| `flag` | Fallback for `action=store_true` | No values needed |\n| `text`/`mline`/`mlines` | Shortcut for `btype=text` | No values needed |\n| `ns`/`namespace` | Shortcut for `btype=ns` | No values needed |\n| `choices`/`choice` | Shortcut for `btype=choice` | No values needed |\n| `mchoices`/`mchoice` | Shortcut for `btype=mchoice` | No values needed |\n| `array`/`list` | Shortcut for `btype=array`/`btype=list` | No values needed |\n| `choices`/`choice` | Shortcut for `btype=choice` | No values needed |\n| `mchoices`/`mchoice` | Shortcut for `btype=mchoice` | No values needed |\n| `order` | The order of the argument in the UI. | Any integer |\n| `readonly` | Whether the argument is readonly. | No values needed (True if specified, otherwise False) |\n| `required` | Whether the argument is required. | No values needed (True if specified, otherwise False) |\n| `placeholder` | The placeholder in the UI for the argument. | Any string |\n| `bitype` | The type of the elements in an array or list. | `int`, `float`, `bool`, `str`, `json`, `auto`* |\n| `itype` | Fallback for `bitype` | Same as `bitype` |\n\n- `argx*`: An argument parser for Python, compatible with `argparse`.\n- `auto*`: Automatically infer the type from a string value.\n  - Any of `True`, `TRUE`, `true`, `False`, `FALSE`, `false` will be inferred as a `bool` value.\n  - Any of `None`, `NONE`, `none`, `null`, `NULL` will be inferred as `None`.\n  - Any integers will be inferred as `int`.\n  - Any floats will be inferred as `float`.\n  - Try to parse the value as JSON. If succeed, the value will be inferred as `json`.\n  - Otherwise, the value will be inferred as `str`.\n\n### Types of options in the UI\n\nThe type of an option in the UI is determined by the `btype`, `action` or `type` metadata. If neither is specified, a `PlainText` will be used.\n\n- `BoolOption`: Shown as a switch\n- `TextOption`: Shown as a textarea (allow multiple lines)\n- `ChoiceOption`: Shown as a dropdown list (`subarg1` and `subarg2` in the example above are used as the choices)\n- `MChoiceOption`: Shown as a multiple choice list (`subarg1` and `subarg2` in the example above are used as the choices)\n- `JsonOption`: Shown as a textarea, but the value will be validated and parsed as JSON\n- `ArrayOption`: Shown as a tag input. Items can be added or removed.\n- `AutoOption`: Shown as a 1-row textarea, and the value will be parsed automatically\n- `PlainText`: Shown as a plain text. No validation or parsing will be performed.\n- `MoreLikeOption`: Show as a box with buttons to add or remove sub-options. It\'s usally used together with `ns` type. If there is a sub-option under the option in the docstring wrapped by `<...>`, it indicates that we may have more sub-options.\n\n\n[1]: https://github.com/pwwang/pipen\n[2]: https://github.com/pwwang/argx\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pipen_board-0.4.0/PKG-INFO` & `pipen_board-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pipen-board
-Version: 0.4.0
+Version: 0.5.0
 Summary: Visualization configuration and running of pipen pipelines on the web
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
-Requires-Dist: pipen-args (>=0.9.11,<0.10.0)
-Requires-Dist: pipen-log2file (>=0.2.1,<0.3.0)
+Requires-Dist: pipen-args (>=0.10.0,<0.11.0)
+Requires-Dist: pipen-log2file (>=0.3.0,<0.4.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: quart (>=0.18,<0.19)
 Requires-Dist: websocket-client (>=1.5,<2.0)
 Description-Content-Type: text/markdown
 
 # pipen-board
```

