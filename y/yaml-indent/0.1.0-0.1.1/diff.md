# Comparing `tmp/yaml_indent-0.1.0.tar.gz` & `tmp/yaml_indent-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaml_indent-0.1.0.tar", max compression
+gzip compressed data, was "yaml_indent-0.1.1.tar", max compression
```

## Comparing `yaml_indent-0.1.0.tar` & `yaml_indent-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-06-08 11:39:30.751856 yaml_indent-0.1.0/LICENSE
--rw-r--r--   0        0        0     1347 2023-06-08 11:48:25.689424 yaml_indent-0.1.0/README.md
--rw-r--r--   0        0        0      357 2023-06-09 08:13:19.420470 yaml_indent-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-08 11:19:16.282076 yaml_indent-0.1.0/yaml_indent/__init__.py
--rwxr-xr-x   0        0        0     1130 2023-06-09 08:13:23.082536 yaml_indent-0.1.0/yaml_indent/yaml_indent.py
--rw-r--r--   0        0        0     2112 1970-01-01 00:00:00.000000 yaml_indent-0.1.0/setup.py
--rw-r--r--   0        0        0     1725 1970-01-01 00:00:00.000000 yaml_indent-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-08 11:39:30.751856 yaml_indent-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1525 2023-06-09 08:19:25.573057 yaml_indent-0.1.1/README.md
+-rw-r--r--   0        0        0      410 2023-06-09 14:29:30.292178 yaml_indent-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-08 11:19:16.282076 yaml_indent-0.1.1/yaml_indent/__init__.py
+-rwxr-xr-x   0        0        0     2611 2023-06-09 14:41:45.327691 yaml_indent-0.1.1/yaml_indent/yaml_indent.py
+-rw-r--r--   0        0        0     2367 1970-01-01 00:00:00.000000 yaml_indent-0.1.1/setup.py
+-rw-r--r--   0        0        0     2001 1970-01-01 00:00:00.000000 yaml_indent-0.1.1/PKG-INFO
```

### Comparing `yaml_indent-0.1.0/LICENSE` & `yaml_indent-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yaml_indent-0.1.0/README.md` & `yaml_indent-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # YAML Indent
+
+
 ## Overview
 
 yaml-indent is a Python utility for formatting YAML files with correct
 indentation. It reads in a YAML file, processes it, and outputs a new
 YAML file with proper indentation, making the file more readable and
 manageable.
 
@@ -28,24 +30,29 @@
 
 To use this utility, you need to run the Python script yaml_indent.py
 with two arguments: the input YAML file and the output YAML file. 
 
 Here is an example:
 
 ``` sh
-python input.yaml output.yaml
+yaml-indent input.yaml output.yaml
 ```
 
 In this command, input.yaml is the YAML file you want to format and
 output.yaml is the file where the formatted YAML will be written. If
 output.yaml already exists, it will be overwritten.
 
 ## Contributing
 
 Contributions to this project are welcome. If you find a bug or think
 of a feature that this utility could benefit from, please open an
 issue or submit a pull request.
 
+## Source Code
+
+The source code for this project is hosted on GitHub. You can access it at [https://github.com/knobo/yaml-indent](https://github.com/knobo/yaml-indent).
+
+
 ## License
 
 This project is open source under the terms of the GPL License.
```

### Comparing `yaml_indent-0.1.0/setup.py` & `yaml_indent-0.1.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,24 +4,26 @@
 packages = \
 ['yaml_indent']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pyyaml>=6.0,<7.0']
+['argparse>=1.4.0,<2.0.0',
+ 'configparser>=5.3.0,<6.0.0',
+ 'ruamel-yaml>=0.17.31,<0.18.0']
 
 entry_points = \
 {'console_scripts': ['yaml-indent = yaml_indent.yaml_indent:main']}
 
 setup_kwargs = {
     'name': 'yaml-indent',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '',
-    'long_description': '# YAML Indent\n## Overview\n\nyaml-indent is a Python utility for formatting YAML files with correct\nindentation. It reads in a YAML file, processes it, and outputs a new\nYAML file with proper indentation, making the file more readable and\nmanageable.\n\n## How it Works\n\nThe utility makes use of the PyYAML library to parse the input YAML\nfile, and re-dumps the YAML data into the output file with correct\nindentation.\n\n## Installation\n\nTo use this utility, you must have Python 3 installed on your\nsystem. Additionally, you need to install the PyYAML library. You can\ninstall it using pip:\n\n``` sh\npip install yaml-indent\n```\n\nYou can then clone this repository to your local machine.\n\n## Usage\n\nTo use this utility, you need to run the Python script yaml_indent.py\nwith two arguments: the input YAML file and the output YAML file. \n\nHere is an example:\n\n``` sh\npython input.yaml output.yaml\n```\n\nIn this command, input.yaml is the YAML file you want to format and\noutput.yaml is the file where the formatted YAML will be written. If\noutput.yaml already exists, it will be overwritten.\n\n## Contributing\n\nContributions to this project are welcome. If you find a bug or think\nof a feature that this utility could benefit from, please open an\nissue or submit a pull request.\n\n## License\n\nThis project is open source under the terms of the GPL License.\n\n',
+    'long_description': '# YAML Indent\n\n\n## Overview\n\nyaml-indent is a Python utility for formatting YAML files with correct\nindentation. It reads in a YAML file, processes it, and outputs a new\nYAML file with proper indentation, making the file more readable and\nmanageable.\n\n## How it Works\n\nThe utility makes use of the PyYAML library to parse the input YAML\nfile, and re-dumps the YAML data into the output file with correct\nindentation.\n\n## Installation\n\nTo use this utility, you must have Python 3 installed on your\nsystem. Additionally, you need to install the PyYAML library. You can\ninstall it using pip:\n\n``` sh\npip install yaml-indent\n```\n\nYou can then clone this repository to your local machine.\n\n## Usage\n\nTo use this utility, you need to run the Python script yaml_indent.py\nwith two arguments: the input YAML file and the output YAML file. \n\nHere is an example:\n\n``` sh\nyaml-indent input.yaml output.yaml\n```\n\nIn this command, input.yaml is the YAML file you want to format and\noutput.yaml is the file where the formatted YAML will be written. If\noutput.yaml already exists, it will be overwritten.\n\n## Contributing\n\nContributions to this project are welcome. If you find a bug or think\nof a feature that this utility could benefit from, please open an\nissue or submit a pull request.\n\n## Source Code\n\nThe source code for this project is hosted on GitHub. You can access it at [https://github.com/knobo/yaml-indent](https://github.com/knobo/yaml-indent).\n\n\n## License\n\nThis project is open source under the terms of the GPL License.\n\n',
     'author': 'Knut Olav Bøhmer',
     'author_email': 'bohmer@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `yaml_indent-0.1.0/PKG-INFO` & `yaml_indent-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: yaml-indent
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Knut Olav Bøhmer
 Author-email: bohmer@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: argparse (>=1.4.0,<2.0.0)
+Requires-Dist: configparser (>=5.3.0,<6.0.0)
+Requires-Dist: ruamel-yaml (>=0.17.31,<0.18.0)
 Description-Content-Type: text/markdown
 
 # YAML Indent
+
+
 ## Overview
 
 yaml-indent is a Python utility for formatting YAML files with correct
 indentation. It reads in a YAML file, processes it, and outputs a new
 YAML file with proper indentation, making the file more readable and
 manageable.
 
@@ -41,25 +45,30 @@
 
 To use this utility, you need to run the Python script yaml_indent.py
 with two arguments: the input YAML file and the output YAML file. 
 
 Here is an example:
 
 ``` sh
-python input.yaml output.yaml
+yaml-indent input.yaml output.yaml
 ```
 
 In this command, input.yaml is the YAML file you want to format and
 output.yaml is the file where the formatted YAML will be written. If
 output.yaml already exists, it will be overwritten.
 
 ## Contributing
 
 Contributions to this project are welcome. If you find a bug or think
 of a feature that this utility could benefit from, please open an
 issue or submit a pull request.
 
+## Source Code
+
+The source code for this project is hosted on GitHub. You can access it at [https://github.com/knobo/yaml-indent](https://github.com/knobo/yaml-indent).
+
+
 ## License
 
 This project is open source under the terms of the GPL License.
```

