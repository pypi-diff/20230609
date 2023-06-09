# Comparing `tmp/succulent-0.2.2.tar.gz` & `tmp/succulent-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "succulent-0.2.2.tar", max compression
+gzip compressed data, was "succulent-0.2.3.tar", max compression
```

## Comparing `succulent-0.2.2.tar` & `succulent-0.2.3.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-06-05 11:01:01.351753 succulent-0.2.2/LICENSE
--rw-r--r--   0        0        0     7105 2023-06-05 11:01:01.351753 succulent-0.2.2/README.md
--rw-r--r--   0        0        0      669 2023-06-05 11:01:01.351753 succulent-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      107 2023-06-05 11:01:01.351753 succulent-0.2.2/succulent/__init__.py
--rw-r--r--   0        0        0     1663 2023-06-05 11:01:01.351753 succulent-0.2.2/succulent/api.py
--rw-r--r--   0        0        0      349 2023-06-05 11:01:01.351753 succulent-0.2.2/succulent/configuration.py
--rw-r--r--   0        0        0     3682 2023-06-05 11:01:01.351753 succulent-0.2.2/succulent/processing.py
--rw-r--r--   0        0        0     7949 2023-06-05 11:01:13.482198 succulent-0.2.2/setup.py
--rw-r--r--   0        0        0     7882 2023-06-05 11:01:13.482468 succulent-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1094 2023-04-18 11:02:21.268343 succulent-0.2.3/LICENSE
+-rw-r--r--   0        0        0      693 2023-06-09 08:05:28.302397 succulent-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     7409 2023-06-09 07:49:54.909125 succulent-0.2.3/README.md
+-rw-r--r--   0        0        0      113 2023-06-09 08:05:33.530717 succulent-0.2.3/succulent/__init__.py
+-rw-r--r--   0        0        0     1716 2023-06-08 12:14:03.927866 succulent-0.2.3/succulent/api.py
+-rw-r--r--   0        0        0      362 2023-05-24 09:55:47.296058 succulent-0.2.3/succulent/configuration.py
+-rw-r--r--   0        0        0     4664 2023-06-09 07:59:43.240467 succulent-0.2.3/succulent/processing.py
+-rw-r--r--   0        0        0     8099 1970-01-01 00:00:00.000000 succulent-0.2.3/PKG-INFO
```

### Comparing `succulent-0.2.2/LICENSE` & `succulent-0.2.3/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Iztok Fister Jr.
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Iztok Fister Jr.
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `succulent-0.2.2/README.md` & `succulent-0.2.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: succulent
+Version: 0.2.3
+Summary: Collect POST requests easily
+Home-page: https://github.com/firefly-cpp/succulent
+License: MIT
+Keywords: data collection,data science,sensor measurements
+Author: Iztok Fister Jr.
+Author-email: iztok@iztok-jr-fister.eu
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: flask (>=2.3.2,<3.0.0)
+Requires-Dist: pandas (>=2.0.1,<3.0.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Project-URL: Repository, https://github.com/firefly-cpp/succulent
+Description-Content-Type: text/markdown
+
 ---
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 [![All Contributors](https://img.shields.io/badge/all_contributors-5-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 <p align="center">
   <img alt="logo" width="300" src=".github/images/logo.png">
@@ -25,15 +47,15 @@
 Sending sensor measurements, data, or GPS positions from embedded devices, microcontrollers, and [smartwatches](https://github.com/firefly-cpp/AST-Monitor) to the central server is sometimes complicated and tricky. Setting up the primary data collection scripts can be time-consuming (selecting a protocol, framework, API, testing it, etc.). Usually, scripts are written for a specific task; thus, they are not easily adaptive to other tasks. succulent is a pure Python framework that simplifies the configuration, management, collection, and preprocessing of data collected via POST requests. The inspiration for the framework comes from the practical data collection challenges in [smart agriculture](https://github.com/firefly-cpp/smart-agriculture-datasets/tree/main/plant-monitoring-esp32). The main idea of the framework was to speed up the process of configuring different collected parameters and providing several useful functions for data transformations. The framework allows users to configure the whole endpoint for data collection in several minutes and thus not spend time on server-side scripts.
 
 ## Detailed insights
 The current version includes (but is not limited to) the following functions:
 
 - Request URL generation for data collection
 - Data collection from POST requests
-- Storing data in different formats (CSV, JSON, SQLite)
+- Storing data in different formats (CSV, JSON, SQLite, images)
 - Defining boundaries for collected data (min, max)
 
 ## Installation
 
 ### pip
 
 Install succulent with pip:
@@ -93,14 +115,20 @@
 ```yml
 data:
   - name: # Measure name
     min: # Minimum value (optional)
     max: # Maximum value (optional)
 ```
 
+To collect images, create a file named ``configuration.yml`` in the root directory and define the following:
+```yml
+data:
+  - key: # Key in POST request
+```
+
 ## License
 
 This package is distributed under the MIT License. This license can be found online at <http://www.opensource.org/licenses/MIT>.
 
 ## Disclaimer
 
 This framework is provided as-is, and there are no guarantees that it fits your purposes or that it is bug-free. Use it at your own risk!
@@ -126,7 +154,8 @@
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 
 This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
+
```

### Comparing `succulent-0.2.2/succulent/api.py` & `succulent-0.2.3/succulent/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-from flask import Flask, jsonify, request
-from succulent.configuration import Configuration
-from succulent.processing import Processing
-from datetime import datetime
-
-class SucculentAPI:
-    def __init__(self, host, port, config, format='csv'):
-        self.host = host
-        self.port = port
-        self.format = format
-
-        # Configuration file
-        conf = Configuration(config)
-        self.config = conf.load_config()
-
-        # Initialise processing
-        self.processing = Processing(self.config['data'], self.format)
-
-        # Initialise Flask
-        self.app = Flask(__name__)
-        self.app.add_url_rule('/measure', 'url', self.url, methods=['GET'])
-        self.app.add_url_rule('/measure', 'measure', self.measure, methods=['POST'])
-
-    def url(self):
-        # Generate URL
-        parameters = self.processing.parameters()
-
-        # Send response
-        return jsonify({'url': f'{self.host}:{self.port}/measure?{parameters}'}), 200
-
-    def measure(self):
-        try:
-            # Process request
-            self.processing.process(request)
-            
-            # Collect and store timestamp
-            timestamp = datetime.now().strftime('%Y-%m-%d %H:%M:%S')
-            # You can store the timestamp in a database, file, or any other desired storage mechanism.
-            # Example: database.insert_timestamp(timestamp)
-        except ValueError as err:
-            # Invalid file type
-            return jsonify({'message': str(err)}), 400
-
-        # Send response
-        return jsonify({'message': 'Data stored', 'timestamp': timestamp}), 200
-
-    def start(self):
+from flask import Flask, jsonify, request
+from succulent.configuration import Configuration
+from succulent.processing import Processing
+from datetime import datetime
+
+class SucculentAPI:
+    def __init__(self, host, port, config, format='csv'):
+        self.host = host
+        self.port = port
+        self.format = format
+
+        # Configuration file
+        conf = Configuration(config)
+        self.config = conf.load_config()
+
+        # Initialise processing
+        self.processing = Processing(config=self.config, format=self.format)
+
+        # Initialise Flask
+        self.app = Flask(__name__)
+        self.app.add_url_rule('/measure', 'url', self.url, methods=['GET'])
+        self.app.add_url_rule('/measure', 'measure', self.measure, methods=['POST'])
+
+    def url(self):
+        # Generate URL
+        parameters = self.processing.parameters()
+
+        # Send response
+        return jsonify({'url': f'{self.host}:{self.port}/measure?{parameters}'}), 200
+
+    def measure(self):
+        try:
+            # Process request
+            self.processing.process(request)
+            
+            # Collect and store timestamp
+            timestamp = datetime.now().strftime('%Y-%m-%d %H:%M:%S')
+            # You can store the timestamp in a database, file, or any other desired storage mechanism.
+            # Example: database.insert_timestamp(timestamp)
+        except ValueError as err:
+            # Invalid file type
+            return jsonify({'message': str(err)}), 400
+
+        # Send response
+        return jsonify({'message': 'Data stored', 'timestamp': timestamp}), 200
+
+    def start(self):
         self.app.run(host=self.host, port=self.port)
```

### Comparing `succulent-0.2.2/setup.py` & `succulent-0.2.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,138 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['succulent']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['flask>=2.3.2,<3.0.0', 'pandas>=2.0.1,<3.0.0', 'pyyaml>=6.0,<7.0']
-
-setup_kwargs = {
-    'name': 'succulent',
-    'version': '0.2.2',
-    'description': 'Collect POST requests easily',
-    'long_description': '---\n<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->\n[![All Contributors](https://img.shields.io/badge/all_contributors-5-orange.svg?style=flat-square)](#contributors-)\n<!-- ALL-CONTRIBUTORS-BADGE:END -->\n\n<p align="center">\n  <img alt="logo" width="300" src=".github/images/logo.png">\n</p>\n\n\n# succulent - Collect POST requests easily\n\n---\n![PyPI Version](https://img.shields.io/pypi/v/succulent.svg)\n![PyPI - Downloads](https://img.shields.io/pypi/dm/succulent.svg)\n[![Downloads](https://pepy.tech/badge/succulent)](https://pepy.tech/project/succulent)\n![GitHub repo size](https://img.shields.io/github/repo-size/firefly-cpp/succulent?style=flat-square)\n[![GitHub license](https://img.shields.io/github/license/firefly-cpp/succulent.svg)](https://github.com/firefly-cpp/succulent/blob/master/LICENSE)\n![GitHub commit activity](https://img.shields.io/github/commit-activity/w/firefly-cpp/succulent.svg)\n[![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/firefly-cpp/succulent.svg)](http://isitmaintained.com/project/firefly-cpp/succulent "Average time to resolve an issue")\n[![Percentage of issues still open](http://isitmaintained.com/badge/open/firefly-cpp/succulent.svg)](http://isitmaintained.com/project/firefly-cpp/succulent "Percentage of issues still open")\n\n## About\n\nSending sensor measurements, data, or GPS positions from embedded devices, microcontrollers, and [smartwatches](https://github.com/firefly-cpp/AST-Monitor) to the central server is sometimes complicated and tricky. Setting up the primary data collection scripts can be time-consuming (selecting a protocol, framework, API, testing it, etc.). Usually, scripts are written for a specific task; thus, they are not easily adaptive to other tasks. succulent is a pure Python framework that simplifies the configuration, management, collection, and preprocessing of data collected via POST requests. The inspiration for the framework comes from the practical data collection challenges in [smart agriculture](https://github.com/firefly-cpp/smart-agriculture-datasets/tree/main/plant-monitoring-esp32). The main idea of the framework was to speed up the process of configuring different collected parameters and providing several useful functions for data transformations. The framework allows users to configure the whole endpoint for data collection in several minutes and thus not spend time on server-side scripts.\n\n## Detailed insights\nThe current version includes (but is not limited to) the following functions:\n\n- Request URL generation for data collection\n- Data collection from POST requests\n- Storing data in different formats (CSV, JSON, SQLite)\n- Defining boundaries for collected data (min, max)\n\n## Installation\n\n### pip\n\nInstall succulent with pip:\n\n```sh\npip install succulent\n```\n### Alpine Linux\n\nTo install succulent on Alpine Linux, please use:\n\n```sh\n$ apk add py3-succulent\n```\n\n## Container\n\n[Basic container for succulent](https://github.com/firefly-cpp/succulent-container)\n\n### Configuration\nFollow the instructions in the [configuration](##configuration) section to define the configuration file.\n\n### Installation\nBuild the container using Docker:\n```bash\ndocker build -t succulent-container .\n```\n\nAlternatively, you can use ``docker-compose``:\n```bash\ndocker compose build\n```\n\n### Usage\nRun the container using Docker:\n```bash\ndocker run -p 8080:8080 succulent-container\n```\n\nAlternatively, you can use ``docker-compose``:\n```bash\ndocker compose up\n```\n\n## Usage\n\n### Example\n\n```python\nfrom succulent.api import SucculentAPI\napi = SucculentAPI(host=\'0.0.0.0\', port=8080, config=\'configuration.yml\', format=\'csv\')\napi.start()\n```\n\n## Configuration\nIn the root directory, create a file named `configuration.yml` and define the following:\n```yml\ndata:\n  - name: # Measure name\n    min: # Minimum value (optional)\n    max: # Maximum value (optional)\n```\n\n## License\n\nThis package is distributed under the MIT License. This license can be found online at <http://www.opensource.org/licenses/MIT>.\n\n## Disclaimer\n\nThis framework is provided as-is, and there are no guarantees that it fits your purposes or that it is bug-free. Use it at your own risk!\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable -->\n<table>\n  <tbody>\n    <tr>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/lahovniktadej"><img src="https://avatars.githubusercontent.com/u/57890734?v=4?s=100" width="100px;" alt="Tadej Lahovnik"/><br /><sub><b>Tadej Lahovnik</b></sub></a><br /><a href="https://github.com/firefly-cpp/succulent/commits?author=lahovniktadej" title="Code">💻</a> <a href="https://github.com/firefly-cpp/succulent/issues?q=author%3Alahovniktadej" title="Bug reports">🐛</a> <a href="#ideas-lahovniktadej" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/firefly-cpp/succulent/commits?author=lahovniktadej" title="Documentation">📖</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/AyanDas348"><img src="https://avatars.githubusercontent.com/u/53610626?v=4?s=100" width="100px;" alt="Ayan Das"/><br /><sub><b>Ayan Das</b></sub></a><br /><a href="https://github.com/firefly-cpp/succulent/commits?author=AyanDas348" title="Code">💻</a> <a href="https://github.com/firefly-cpp/succulent/commits?author=AyanDas348" title="Tests">⚠️</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="http://www.iztok-jr-fister.eu/"><img src="https://avatars.githubusercontent.com/u/1633361?v=4?s=100" width="100px;" alt="Iztok Fister Jr."/><br /><sub><b>Iztok Fister Jr.</b></sub></a><br /><a href="https://github.com/firefly-cpp/succulent/commits?author=firefly-cpp" title="Code">💻</a> <a href="#ideas-firefly-cpp" title="Ideas, Planning, & Feedback">🤔</a> <a href="#mentoring-firefly-cpp" title="Mentoring">🧑\u200d🏫</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="http://carlosal1015.github.io"><img src="https://avatars.githubusercontent.com/u/21283014?v=4?s=100" width="100px;" alt="Oromion"/><br /><sub><b>Oromion</b></sub></a><br /><a href="https://github.com/firefly-cpp/succulent/issues?q=author%3Acarlosal1015" title="Bug reports">🐛</a> <a href="#platform-carlosal1015" title="Packaging/porting to new platform">📦</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/rhododendrom"><img src="https://avatars.githubusercontent.com/u/3198785?v=4?s=100" width="100px;" alt="rhododendrom"/><br /><sub><b>rhododendrom</b></sub></a><br /><a href="#design-rhododendrom" title="Design">🎨</a></td>\n    </tr>\n  </tbody>\n</table>\n\n<!-- markdownlint-restore -->\n<!-- prettier-ignore-end -->\n\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n',
-    'author': 'Iztok Fister Jr.',
-    'author_email': 'iztok@iztok-jr-fister.eu',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/firefly-cpp/succulent',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
+---
+<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
+[![All Contributors](https://img.shields.io/badge/all_contributors-5-orange.svg?style=flat-square)](#contributors-)
+<!-- ALL-CONTRIBUTORS-BADGE:END -->
+
+<p align="center">
+  <img alt="logo" width="300" src=".github/images/logo.png">
+</p>
+
+
+# succulent - Collect POST requests easily
+
+---
+![PyPI Version](https://img.shields.io/pypi/v/succulent.svg)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/succulent.svg)
+[![Downloads](https://pepy.tech/badge/succulent)](https://pepy.tech/project/succulent)
+![GitHub repo size](https://img.shields.io/github/repo-size/firefly-cpp/succulent?style=flat-square)
+[![GitHub license](https://img.shields.io/github/license/firefly-cpp/succulent.svg)](https://github.com/firefly-cpp/succulent/blob/master/LICENSE)
+![GitHub commit activity](https://img.shields.io/github/commit-activity/w/firefly-cpp/succulent.svg)
+[![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/firefly-cpp/succulent.svg)](http://isitmaintained.com/project/firefly-cpp/succulent "Average time to resolve an issue")
+[![Percentage of issues still open](http://isitmaintained.com/badge/open/firefly-cpp/succulent.svg)](http://isitmaintained.com/project/firefly-cpp/succulent "Percentage of issues still open")
+
+## About
+
+Sending sensor measurements, data, or GPS positions from embedded devices, microcontrollers, and [smartwatches](https://github.com/firefly-cpp/AST-Monitor) to the central server is sometimes complicated and tricky. Setting up the primary data collection scripts can be time-consuming (selecting a protocol, framework, API, testing it, etc.). Usually, scripts are written for a specific task; thus, they are not easily adaptive to other tasks. succulent is a pure Python framework that simplifies the configuration, management, collection, and preprocessing of data collected via POST requests. The inspiration for the framework comes from the practical data collection challenges in [smart agriculture](https://github.com/firefly-cpp/smart-agriculture-datasets/tree/main/plant-monitoring-esp32). The main idea of the framework was to speed up the process of configuring different collected parameters and providing several useful functions for data transformations. The framework allows users to configure the whole endpoint for data collection in several minutes and thus not spend time on server-side scripts.
+
+## Detailed insights
+The current version includes (but is not limited to) the following functions:
+
+- Request URL generation for data collection
+- Data collection from POST requests
+- Storing data in different formats (CSV, JSON, SQLite, images)
+- Defining boundaries for collected data (min, max)
+
+## Installation
+
+### pip
+
+Install succulent with pip:
+
+```sh
+pip install succulent
+```
+### Alpine Linux
+
+To install succulent on Alpine Linux, please use:
+
+```sh
+$ apk add py3-succulent
+```
+
+## Container
+
+[Basic container for succulent](https://github.com/firefly-cpp/succulent-container)
+
+### Configuration
+Follow the instructions in the [configuration](##configuration) section to define the configuration file.
+
+### Installation
+Build the container using Docker:
+```bash
+docker build -t succulent-container .
+```
+
+Alternatively, you can use ``docker-compose``:
+```bash
+docker compose build
+```
+
+### Usage
+Run the container using Docker:
+```bash
+docker run -p 8080:8080 succulent-container
+```
+
+Alternatively, you can use ``docker-compose``:
+```bash
+docker compose up
+```
+
+## Usage
+
+### Example
+
+```python
+from succulent.api import SucculentAPI
+api = SucculentAPI(host='0.0.0.0', port=8080, config='configuration.yml', format='csv')
+api.start()
+```
+
+## Configuration
+In the root directory, create a file named `configuration.yml` and define the following:
+```yml
+data:
+  - name: # Measure name
+    min: # Minimum value (optional)
+    max: # Maximum value (optional)
+```
+
+To collect images, create a file named ``configuration.yml`` in the root directory and define the following:
+```yml
+data:
+  - key: # Key in POST request
+```
+
+## License
+
+This package is distributed under the MIT License. This license can be found online at <http://www.opensource.org/licenses/MIT>.
+
+## Disclaimer
+
+This framework is provided as-is, and there are no guarantees that it fits your purposes or that it is bug-free. Use it at your own risk!
+
+## Contributors ✨
+
+Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
+
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable -->
+<table>
+  <tbody>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/lahovniktadej"><img src="https://avatars.githubusercontent.com/u/57890734?v=4?s=100" width="100px;" alt="Tadej Lahovnik"/><br /><sub><b>Tadej Lahovnik</b></sub></a><br /><a href="https://github.com/firefly-cpp/succulent/commits?author=lahovniktadej" title="Code">💻</a> <a href="https://github.com/firefly-cpp/succulent/issues?q=author%3Alahovniktadej" title="Bug reports">🐛</a> <a href="#ideas-lahovniktadej" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/firefly-cpp/succulent/commits?author=lahovniktadej" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/AyanDas348"><img src="https://avatars.githubusercontent.com/u/53610626?v=4?s=100" width="100px;" alt="Ayan Das"/><br /><sub><b>Ayan Das</b></sub></a><br /><a href="https://github.com/firefly-cpp/succulent/commits?author=AyanDas348" title="Code">💻</a> <a href="https://github.com/firefly-cpp/succulent/commits?author=AyanDas348" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="http://www.iztok-jr-fister.eu/"><img src="https://avatars.githubusercontent.com/u/1633361?v=4?s=100" width="100px;" alt="Iztok Fister Jr."/><br /><sub><b>Iztok Fister Jr.</b></sub></a><br /><a href="https://github.com/firefly-cpp/succulent/commits?author=firefly-cpp" title="Code">💻</a> <a href="#ideas-firefly-cpp" title="Ideas, Planning, & Feedback">🤔</a> <a href="#mentoring-firefly-cpp" title="Mentoring">🧑‍🏫</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="http://carlosal1015.github.io"><img src="https://avatars.githubusercontent.com/u/21283014?v=4?s=100" width="100px;" alt="Oromion"/><br /><sub><b>Oromion</b></sub></a><br /><a href="https://github.com/firefly-cpp/succulent/issues?q=author%3Acarlosal1015" title="Bug reports">🐛</a> <a href="#platform-carlosal1015" title="Packaging/porting to new platform">📦</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/rhododendrom"><img src="https://avatars.githubusercontent.com/u/3198785?v=4?s=100" width="100px;" alt="rhododendrom"/><br /><sub><b>rhododendrom</b></sub></a><br /><a href="#design-rhododendrom" title="Design">🎨</a></td>
+    </tr>
+  </tbody>
+</table>
+
+<!-- markdownlint-restore -->
+<!-- prettier-ignore-end -->
+
+<!-- ALL-CONTRIBUTORS-LIST:END -->
+
+This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
```

