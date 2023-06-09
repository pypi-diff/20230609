# Comparing `tmp/scramjet_client_utils-1.0.1.tar.gz` & `tmp/scramjet-client-utils-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scramjet_client_utils-1.0.1.tar", max compression
+gzip compressed data, was "scramjet-client-utils-1.1.0.tar", last modified: Fri Jun  9 11:33:12 2023, max compression
```

## Comparing `scramjet_client_utils-1.0.1.tar` & `scramjet-client-utils-1.1.0.tar`

### file list

```diff
@@ -1,5 +1,14 @@
--rw-r--r--   0        0        0    23951 2023-01-10 11:56:50.307704 scramjet_client_utils-1.0.1/README.md
--rw-r--r--   0        0        0     2269 2023-01-10 11:54:50.220214 scramjet_client_utils-1.0.1/client_utils/client_utils.py
--rw-r--r--   0        0        0      365 2023-01-10 11:57:05.383639 scramjet_client_utils-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    25424 1970-01-01 00:00:00.000000 scramjet_client_utils-1.0.1/setup.py
--rw-r--r--   0        0        0    24438 1970-01-01 00:00:00.000000 scramjet_client_utils-1.0.1/PKG-INFO
+drwxrwxr-x   0 bob       (1000) bob       (1000)        0 2023-06-09 11:33:12.209360 scramjet-client-utils-1.1.0/
+-rw-rw-r--   0 bob       (1000) bob       (1000)    24181 2023-06-09 11:33:12.209360 scramjet-client-utils-1.1.0/PKG-INFO
+-rw-r--r--   0 bob       (1000) bob       (1000)    23908 2023-04-26 06:19:50.000000 scramjet-client-utils-1.1.0/README.md
+drwxrwxr-x   0 bob       (1000) bob       (1000)        0 2023-06-09 11:33:12.209360 scramjet-client-utils-1.1.0/client_utils/
+-rw-rw-r--   0 bob       (1000) bob       (1000)        0 2023-04-28 10:00:38.000000 scramjet-client-utils-1.1.0/client_utils/__init__.py
+-rw-rw-r--   0 bob       (1000) bob       (1000)     3544 2023-06-09 08:59:04.000000 scramjet-client-utils-1.1.0/client_utils/base_client.py
+drwxrwxr-x   0 bob       (1000) bob       (1000)        0 2023-06-09 11:33:12.209360 scramjet-client-utils-1.1.0/scramjet_client_utils.egg-info/
+-rw-rw-r--   0 bob       (1000) bob       (1000)    24181 2023-06-09 11:33:12.000000 scramjet-client-utils-1.1.0/scramjet_client_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 bob       (1000) bob       (1000)      295 2023-06-09 11:33:12.000000 scramjet-client-utils-1.1.0/scramjet_client_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 bob       (1000) bob       (1000)        1 2023-06-09 11:33:12.000000 scramjet-client-utils-1.1.0/scramjet_client_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 bob       (1000) bob       (1000)       50 2023-06-09 11:33:12.000000 scramjet-client-utils-1.1.0/scramjet_client_utils.egg-info/requires.txt
+-rw-rw-r--   0 bob       (1000) bob       (1000)       13 2023-06-09 11:33:12.000000 scramjet-client-utils-1.1.0/scramjet_client_utils.egg-info/top_level.txt
+-rw-rw-r--   0 bob       (1000) bob       (1000)       38 2023-06-09 11:33:12.209360 scramjet-client-utils-1.1.0/setup.cfg
+-rw-r--r--   0 bob       (1000) bob       (1000)      797 2023-06-09 11:32:54.000000 scramjet-client-utils-1.1.0/setup.py
```

### Comparing `scramjet_client_utils-1.0.1/README.md` & `scramjet-client-utils-1.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,32 +2,30 @@
 
 The package provides utilities for API clients. Each of the API clients make use out of it.
 
 Usage:
 
 ```python
 import asyncio
-import json
 from client.host_client import HostClient
-from client_utils import ClientUtils
+from client_utils.base_client import BaseClient
 
 # your middleware token
 token = ''
 # set the token
-ClientUtils.setDefaultHeaders({'Authorization': f'Bearer {token}'})
+BaseClient.setDefaultHeaders({'Authorization': f'Bearer {token}'})
 
 # middleware url
 api_base ='https://api.scramjet.cloud/api/v1' 
 
-# url = {middlewareURL}/space/{manager_id}/api/v1/{host_id}/api/v1
+# url = {middlewareURL}/space/{manager_id}/api/v1/sth/{host_id}/api/v1
 host = HostClient(f'{api_base}/space/org-aa5bu150-9o5c-489b-83e3-b1yf7e086f3h-manager/api/v1/sth-1/api/v1')
 # get a list of Sequences
 res = asyncio.run(host.list_sequences())
-# convert responose to json
-sequences = json.loads(res)
+print(res)
 ```
 
 ---
 ## More reading
 <p align="center">
     <a href="https://github.com/scramjetorg/transform-hub/blob/HEAD/LICENSE"><img src="https://img.shields.io/github/license/scramjetorg/transform-hub?color=green&style=plastic" alt="GitHub license" /></a>
     <a href="https://npmjs.org/package/@scramjet/sth"><img src="https://img.shields.io/github/v/tag/scramjetorg/transform-hub?label=version&color=blue&style=plastic" alt="STH version" /></a>
```

#### html2text {}

```diff
@@ -1,18 +1,17 @@
            ****** Scramjet Transform Hub API Clients utility ******
 The package provides utilities for API clients. Each of the API clients make
-use out of it. Usage: ```python import asyncio import json from
-client.host_client import HostClient from client_utils import ClientUtils #
-your middleware token token = '' # set the token ClientUtils.setDefaultHeaders(
-{'Authorization': f'Bearer {token}'}) # middleware url api_base ='https://
-api.scramjet.cloud/api/v1' # url = {middlewareURL}/space/{manager_id}/api/v1/
-{host_id}/api/v1 host = HostClient(f'{api_base}/space/org-aa5bu150-9o5c-489b-
-83e3-b1yf7e086f3h-manager/api/v1/sth-1/api/v1') # get a list of Sequences res =
-asyncio.run(host.list_sequences()) # convert responose to json sequences =
-json.loads(res) ``` --- ## More reading
+use out of it. Usage: ```python import asyncio from client.host_client import
+HostClient from client_utils.base_client import BaseClient # your middleware
+token token = '' # set the token BaseClient.setDefaultHeaders({'Authorization':
+f'Bearer {token}'}) # middleware url api_base ='https://api.scramjet.cloud/api/
+v1' # url = {middlewareURL}/space/{manager_id}/api/v1/sth/{host_id}/api/v1 host
+= HostClient(f'{api_base}/space/org-aa5bu150-9o5c-489b-83e3-b1yf7e086f3h-
+manager/api/v1/sth-1/api/v1') # get a list of Sequences res = asyncio.run
+(host.list_sequences()) print(res) ``` --- ## More reading
     [GitHub_license] [STH_version] [GitHub_stars] [npm] [Discord] [Donate]
              â­ Star us on GitHub â it motivates us a lot! ð
                          [Scramjet Transform Hub Logo]
 In the link below you will find more information about our stream protocol and
 API usage. See the code documentation here: [scramjetorg/transform-hub/docs/
 read-more/stream-and-api.md](https://github.com/scramjetorg/transform-hub/tree/
 HEAD/docs/read-more/stream-and-api.md) ## Scramjet Transform Hub This package
```

### Comparing `scramjet_client_utils-1.0.1/setup.py` & `scramjet-client-utils-1.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,789 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: scramjet-client-utils
+Version: 1.1.0
+Home-page: https://github.com/scramjetorg/api-client-python/tree/main/client_utils
+Author: Scramjet
+Author-email: open-source@scramjet.org
+Requires-Python: >=3.9,<4.0
+Description-Content-Type: text/markdown
 
-packages = \
-['client_utils']
+<h1 align="center"><strong>Scramjet Transform Hub API Clients utility</strong></h1>
 
-package_data = \
-{'': ['*']}
+The package provides utilities for API clients. Each of the API clients make use out of it.
 
-install_requires = \
-['aiohttp>=3.8.3,<4.0.0', 'url_normalize>=1.4.3,<2.0.0']
-
-setup_kwargs = {
-    'name': 'scramjet-client-utils',
-    'version': '1.0.1',
-    'description': '',
-    'long_description': '<h1 align="center"><strong>Scramjet Transform Hub API Clients utility</strong></h1>\n\nThe package provides utilities for API clients. Each of the API clients make use out of it.\n\nUsage:\n\n```python\nimport asyncio\nimport json\nfrom client.host_client import HostClient\nfrom client_utils import ClientUtils\n\n# your middleware token\ntoken = \'\'\n# set the token\nClientUtils.setDefaultHeaders({\'Authorization\': f\'Bearer {token}\'})\n\n# middleware url\napi_base =\'https://api.scramjet.cloud/api/v1\' \n\n# url = {middlewareURL}/space/{manager_id}/api/v1/{host_id}/api/v1\nhost = HostClient(f\'{api_base}/space/org-aa5bu150-9o5c-489b-83e3-b1yf7e086f3h-manager/api/v1/sth-1/api/v1\')\n# get a list of Sequences\nres = asyncio.run(host.list_sequences())\n# convert responose to json\nsequences = json.loads(res)\n```\n\n---\n## More reading\n<p align="center">\n    <a href="https://github.com/scramjetorg/transform-hub/blob/HEAD/LICENSE"><img src="https://img.shields.io/github/license/scramjetorg/transform-hub?color=green&style=plastic" alt="GitHub license" /></a>\n    <a href="https://npmjs.org/package/@scramjet/sth"><img src="https://img.shields.io/github/v/tag/scramjetorg/transform-hub?label=version&color=blue&style=plastic" alt="STH version" /></a>\n    <a href="https://github.com/scramjetorg/transform-hub"><img src="https://img.shields.io/github/stars/scramjetorg/transform-hub?color=pink&style=plastic" alt="GitHub stars" /></a>\n    <a href="https://npmjs.org/package/@scramjet/sth"><img src="https://img.shields.io/npm/dt/@scramjet/sth?color=orange&style=plastic" alt="npm" /></a>\n    <a href="https://scr.je/join-community-mg1"><img alt="Discord" src="https://img.shields.io/discord/925384545342201896?label=discord&style=plastic"></a>\n    <a href="https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=7F7V65C43EBMW">\n        <img src="https://img.shields.io/badge/Donate-PayPal-green.svg?color=yellow&style=plastic" alt="Donate" />\n    </a>\n</p>\n<p align="center">⭐ Star us on GitHub — it motivates us a lot! 🚀 </p>\n\n<p align="center">\n    <img src="https://assets.scramjet.org/sth-logo.svg" alt="Scramjet Transform Hub Logo">\n</p>\n\nIn the link below you will find more information about our stream protocol and API usage.\n\nSee the code documentation here: [scramjetorg/transform-hub/docs/read-more/stream-and-api.md](https://github.com/scramjetorg/transform-hub/tree/HEAD/docs/read-more/stream-and-api.md)\n\n## Scramjet Transform Hub\n\nThis package is part of [Scramjet Transform Hub](https://www.npmjs.org/package/@scramjet/sth).\n\nScramjet Transform Hub is a deployment and execution platform. Once installed on a server, it will allow you to start your programs and keep them running on a remote machine. You will be able to start programs in the background or connect to them and see their output directly on your terminal. You will be able to pipe your local data to the program, as if it was running from your terminal. You can start your server in AWS, Google Cloud or Azure, start it on your local machine, install it on a Raspberry Pi or wherever else you\'d like.\n\n## Use cases\n\nThere\'s no limit what you can use it for. You want a stock checker? A chat bot? Maybe you\'d like to automate your home? Retrieve sensor data? Maybe you have a lot of data and want to transfer and wrangle it? You have a database of cities and you\'d like to enrich your data? You do machine learning and you want to train your set while the data is fetched in real time? Hey, you want to use it for something else and ask us if that\'s a good use? Ask us [via email](mailto:get@scramjet.org) or hop on our [Scramjet Discord](https://scr.je/join-community-mg1)!\n___\n\n### Host operations\n\n<details>\n<summary>\n    <strong class="get">[ GET ]</strong>  <code>/api/v1/version</code> <small>- show the Host version</small>\n</summary>\n\n<br> <strong>Parameters</strong>\n\n<small>No parameters</small>\n\n<strong>Responses</strong>\n\n<small>Successful operation code: `200`</small>\n\n```json\n{ "version" : "0.12.2" }\n```\n\n</details>\n\n<details>\n<summary>\n    <strong class="get">[ GET ]</strong>  <code>/api/v1/sequences</code> <small>- show all Sequences saved on the Host</small>\n</summary>\n\n<br> <strong>Parameters</strong>\n\n<small>No parameters</small>\n\n<strong>Responses</strong>\n\n<small>Successful operation code: `200`</small>\n\n```json\n[\n  {\n    "instances": [], // a list of all running Instances of this Sequence\n    "id": "eea8bc33-440f-4a17-8931-eb22a17d5d56", // Sequence ID\n    "config": {\n      "container": {\n        "image": "scramjetorg/runner:0.12.2",\n        "maxMem": 512,\n        "exposePortsRange": [\n          30000,\n          32767\n        ],\n        "hostIp": "0.0.0.0"\n      },\n      "name": "@scramjet/hello-alice-out",\n      "version": "0.12.2",\n      "engines": {\n        "node": ">=10"\n      },\n      "config": {},\n      "sequencePath": "index", // a path to file with a main function\n      "packageVolumeId": "eea8bc33-440f-4a17-8931-eb22a17d5d56"\n    }\n  },\n  {\n    "instances": [\n      "02381acf-cb16-4cff-aa9b-f22f04ada94f"\n    ],\n    "id": "3ec02b93-4ca9-4d23-baab-048dab5ffda4",\n    "config": {\n      "container": {\n        "image": "scramjetorg/runner:0.12.2",\n        "maxMem": 512,\n        "exposePortsRange": [\n          30000,\n          32767\n        ],\n        "hostIp": "0.0.0.0"\n      },\n      "name": "@scramjet/checksum-sequence",\n      "version": "0.12.2",\n      "engines": {},\n      "config": {},\n      "sequencePath": "index.js",\n      "packageVolumeId": "3ec02b93-4ca9-4d23-baab-048dab5ffda4"\n    }\n  }\n]\n```\n\n</details>\n\n<details>\n<summary>\n    <strong class="get">[ GET ]</strong>  <code>/api/v1/instances</code> <small>- show all Instances running on the Host</small>\n</summary>\n\n<br> <strong>Parameters</strong>\n\n<small>No parameters</small>\n\n<strong>Responses</strong>\n\n<small>Successful operation code: `200`</small>\n\n```json\n[\n  {\n    "id": "02381acf-cb16-4cff-aa9b-f22f04ada94f", // Instance ID\n    "sequence": "3ec02b93-4ca9-4d23-baab-048dab5ffda4" // Sequence ID\n  },\n  {\n    "id": "ab0272d8-c9b0-43f7-9e7e-bcac9ec0f21f",\n    "sequence": "e4ca555c-ced1-4a13-b531-f43016eaf4ed"\n  }\n]\n```\n\n</details>\n\n<details>\n<summary>\n    <strong class="get">[ GET ]</strong>  <code>/api/v1/load-check</code> <small>- monitor CPU, memory and disk usage metrics on the Host machine</small>\n</summary>\n\n<br> <strong>Parameters</strong>\n\n<small>No parameters</small>\n\n<strong>Responses</strong>\n\n<small>Successful operation code: `200`</small>\n\n```json\n{\n  "avgLoad": 0.08,\n  "currentLoad": 5.190776257704936,\n  "memFree": 4634816512,\n  "memUsed": 8050364416,\n  "fsSize": [\n    {\n      "fs": "/dev/sda1",\n      "type": "ext4",\n      "size": 20838993920,\n      "used": 14939455488,\n      "available": 5882761216,\n      "use": 71.75,\n      "mount": "/"\n    },\n    {\n      "fs": "/dev/sda15",\n      "type": "vfat",\n      "size": 109422592,\n      "used": 9621504,\n      "available": 99801088,\n      "use": 8.79,\n      "mount": "/boot/efi"\n    }\n  ]\n}\n\n```\n\n</details>\n\n<details>\n<summary>\n    <strong class="get">[ GET ]</strong>  <code>/api/v1/log</code> <small>- monitor CPU, memory and disk usage metrics on the Host machine</small>\n</summary>\n\n<br> <strong>Parameters</strong>\n\n<small>No parameters</small>\n\n<strong>Responses</strong>\n\n<small>Content-type: `application/octet-stream`</small>\n\n<small>Successful operation code: `200`</small>\n\n```bash\n2021-11-19T16:04:47.094Z log (object:Host) Host main called.\n2021-11-19T16:04:47.100Z info (object:SocketServer) Server on: /tmp/scramjet-socket-server-path\n2021-11-19T16:04:47.104Z info (object:Host) API listening on: 127.0.0.1:8000\n2021-11-19T16:05:08.228Z info (object:Host) New sequence incoming...\n2021-11-19T16:05:08.229Z log (object:LifecycleDockerAdapterSequence) Docker sequence adapter init.\n2021-11-19T16:05:08.229Z log (object:DockerodeDockerHelper) Checking image scramjetorg/pre-runner:0.12.2\n2021-11-19T16:05:12.234Z info (object:LifecycleDockerAdapterSequence) Docker sequence adapter done.\n2021-11-19T16:05:12.246Z log (object:LifecycleDockerAdapterSequence) Volume created. Id:  c50fe4d3-89cc-4685-a82a-16cbc744733d\n2021-11-19T16:05:12.246Z log (object:LifecycleDockerAdapterSequence) Starting PreRunner { image: \'scramjetorg/pre-runner:0.12.2\', maxMem: 128 }\n2021-11-19T16:05:13.536Z log (object:DockerodeDockerHelper) Checking image scramjetorg/runner:0.12.2\n2021-11-19T16:05:16.670Z info (object:SequenceStore) New sequence added: c50fe4d3-89cc-4685-a82a-16cbc744733d\n2021-11-19T16:05:16.672Z info (object:Host) Sequence identified: {\n  container: {\n    image: \'scramjetorg/runner:0.12.2\',\n    maxMem: 512,\n    exposePortsRange: [ 30000, 32767 ],\n    hostIp: \'0.0.0.0\'\n  },\n  name: \'@scramjet/multi-outputs\',\n  version: \'0.12.2\',\n  engines: {},\n  config: {},\n  sequencePath: \'index.js\',\n  packageVolumeId: \'c50fe4d3-89cc-4685-a82a-16cbc744733d\'\n}\n2021-11-19T16:05:16.691Z debug (object:Host) Request date: 2021-11-19T16:05:08.239Z, method: POST, url: /api/v1/sequence, status: 202\n```\n\n</details>\n\n___\n\n### Sequence operations\n\n<details>\n<summary>\n    <strong class="post">[ POST ]</strong> <code>/api/v1/sequence</code> <small>- add new sequence</small>\n</summary>\n\n<br><strong>Parameters</strong>\n\n| Name        | Type     | Description                         | Required |\n| ----------- | -------- | ----------------------------------- | -------- |\n| `file`      | `binary` | compressed package in tar.gz format | yes      |\n| `appConfig` | `json`   | additional package.json config file | no       |\n\n<strong>Responses</strong>\n\n<small>Accepted operation code: `202`</small>\n\n```json\n{\n  "id": "2c3068e5-7c74-45bb-a017-1979c41fc6d0" // sequence id\n}\n```\n\n</details>\n\n<details>\n<summary>\n    <strong class="get">[ GET ]</strong>  <code>/api/v1/sequences</code> <small>- show list of sequences</small>\n</summary>\n\n<br> <strong>Parameters</strong>\n\n<small>No parameters</small>\n\n<strong>Responses</strong>\n\n<small>Successful operation code: `200`</small>\n\n```json\n[\n  {\n    "instances": [\n      "742d2713-7ab6-4cde-82f3-a7beabdd4e98"       // list of sequence instances\n    ],\n    "id": "bdef63db-d3a0-45c8-85db-e94ebb96097f",  // sequence id\n    "config": {\n      "container": {\n        "image": "scramjetorg/runner:0.12.2",\n        "maxMem": 512\n      },\n      "name": "@scramjet/transform-hub",\n      "version": "0.12.2",\n      "engines": {},\n      "config": {},\n      "sequencePath": "index.js",\n      "packageVolumeId": "bdef63db-d3a0-45c8-85db-e94ebb96097f"\n    }\n  }\n]\n```\n\n</details>\n\n<details>\n<summary>\n    <strong class="post">[ POST ]</strong> <code>/api/v1/sequence/:id/start</code> <small>- start chosen sequence</small>\n</summary>\n\n<br> <strong>Parameters</strong>\n\n| Name        | Type   | Description                                           | Required |\n| ----------- | ------ | ----------------------------------------------------- | -------- |\n| `appConfig` | `json` | additional package.json config file                   | no       |\n| `args`      | `json` | additional arguments that instance should starts with | no       |\n\n<strong>Responses</strong>\n\n<small>Successful operation code: `200`</small>\n\n```json\n{\n  "id": "681c856e-dfa4-46a1-951d-47b27345552e"\n}\n```\n\n</details>\n\n<details>\n<summary>\n    <strong class="delete">[ DELETE ]</strong> <code>/api/v1/sequence/:id</code> <small>- delete a sequence by id</small>\n</summary>\n\n<br> <strong>Parameters</strong>\n\n<small>No parameters</small>\n\n<strong>Responses</strong>\n\n<small>Successful operation code: `200`</small>\n\n```json\n{\n  "id": "2c3068e5-7c74-45bb-a017-1979c41fc6d0"\n}\n```\n\n<small>Conflict operation code: `409` - the instance is still running</small>\n\n```json\n{\n  "error": "Can\'t remove sequence in use."\n}\n```\n\n</details>\n\n___\n\n### Instance basic operations\n\n<details>\n<summary>\n    <strong class="get">[ GET ]</strong> <code>/api/v1/instances</code> <small>- list all instances</small>\n</summary>\n\n<br> <strong>Parameters</strong>\n\n<small>No parameters</small>\n\n<strong>Responses</strong>\n\n<small>Successful operation code: `200`</small>\n\n```json\n[\n  {\n    "id": "742d2713-7ab6-4cde-82f3-a7beabdd4e98",\n    "sequence": "bdef63db-d3a0-45c8-85db-e94ebb96097f"\n  },\n  {\n    "id": "681c856e-dfa4-46a1-951d-47b27345552e",\n    "sequence": "bdef63db-d3a0-45c8-85db-e94ebb96097f"\n  },\n  {\n    "id": "21f787ed-6b9e-4e9f-828e-afe428d84833",\n    "sequence": "bdef63db-d3a0-45c8-85db-e94ebb96097f"\n  }\n]\n```\n\n</details>\n\n<details>\n<summary>\n    <strong class="get">[ GET ]</strong> <code>/api/v1/instance/:id</code> <small>- show data of chosen instance</small>\n</summary>\n\n<br> <strong>Parameters</strong>\n\n<small>No parameters</small>\n\n<strong>Responses</strong>\n\n| Name                 | Code  | Description                                 |\n| :------------------- | :---- | :------------------------------------------ |\n| Successful operation | `200` | Returns JSON data                           |\n| Not Found operation  | `404` | For example if instance was already stopped |\n\n```json\n{\n  "created": "2021-10-29T16:08:36.524Z",\n  "started": "2021-10-29T16:08:38.701Z",\n  "sequenceId": "b0c02fdc-b05f-4f26-9d68-43a702eb7b44"\n}\n```\n\n</details>\n\n<details>\n<summary>\n    <strong class="post">[ POST ]</strong> <code>/api/v1/instance/:id/_stop</code> <small>- end instance gracefully and prolong operations or not for task completion\u200b</small>\n</summary>\n\n<br> <strong>Parameters</strong>\n\n| Name               | Type      | Description                                                                     | Required |\n| ------------------ | --------- | ------------------------------------------------------------------------------- | -------- |\n| `timeout`          | `number`  | The number of milliseconds before the Instance will be killed. Default: 7000ms. | no       |\n| `canCallKeepalive` | `boolean` | If set to true, the instance will prolong the running. Default: false.          | no       |\n\n<strong>Responses</strong>\n\n<small>Successful operation code: `200`</small>\n\n```json\n{\n   "code": 0,\n   "type": "string",\n   "message": "string"\n}\n```\n\n</details>\n\n<details>\n<summary>\n    <strong class="post">[ POST ]</strong>  <code>api/v1/instance/:id/_kill</code> <small>- end instance gracefully waiting for unfinished tasks</small>\n</summary>\n\n<br> <strong>Parameters</strong>\n\n<small>No parameters</small>\n\n<strong>Responses</strong>\n\n<small>Accepted operation code: `202`</small>\n\n```text\nNo body returned\n```\n\n</details>\n\n<details>\n<summary>\n    <strong class="get">[ GET ]</strong>  <code>/api/v1/instance/:id/health</code> <small>- check status about instance health</small>\n</summary>\n\n<br> <strong>Parameters</strong>\n\n<small>No parameters</small>\n\n<strong>Responses</strong>\n\n<small>Successful operation code: `200`</small>\n\n```json\n{\n  "cpuTotalUsage": 529325247,\n  "healthy": true,\n  "limit": 536870912,\n  "memoryMaxUsage": 16117760,\n  "memoryUsage": 14155776,\n  "networkRx": 1086,\n  "networkTx": 0,\n  "containerId": "1c993c4ff774fac06185aa9554cf40c23b03e1479a7e0d14827708161b08ae51"\n}\n```\n\n</details>\n\n___\n\n### Instance advanced operation\n\n<details>\n<summary>\n    <strong class="post">[ POST ]</strong>  <code>/api/v1/instance/:id/_event</code> <small>- send event to the Instance</small>\n</summary>\n\n<br> <strong>Parameters</strong>\n\n| Name        | Type     | Description                  | Required |\n| :---------- | :------- | ---------------------------- | -------- |\n| `eventName` | `string` | Name of an event             | true     |\n| `message`   | `string` | JSON formatted event payload | false    |\n\n<strong>Responses</strong>\n\n<small>Content-type: `application/octet-stream`</small>\n\n</details>\n\n<details>\n<summary>\n    <strong class="get">[ GET ]</strong>  <code>/api/v1/instance/:id/event</code> <small>- get the data stream with the events from the Instance</small>\n</summary>\n\n<br> <strong>Parameters</strong>\n\n<small>No parameters</small>\n\n<strong>Responses</strong>\n\n<small>Content-type: `application/octet-stream`</small>\n\n</details>\n\n<details>\n<summary>\n    <strong class="get">[ GET ]</strong>  <code>/api/v1/instance/:id/once</code> <small>- get the last event sent by the Instance</small>\n</summary>\n\n<br> <strong>Parameters</strong>\n\n<small>No parameters</small>\n\n<strong>Responses</strong>\n\n<small>Content-type: `application/octet-stream`</small>\n\n</details>\n\n<details>\n<summary>\n    <strong class="post">[ POST ]</strong>  <code>/api/v1/instance/:id/input</code> <small>- send data to the input stream of the Instance to consume it</small>\n</summary>\n\n<br> <strong>Parameters</strong>\n\n<small>No parameters</small>\n\n<strong>Responses</strong>\n\n| Name                     | Code  | Description                                                  |\n| :----------------------- | :---- | :----------------------------------------------------------- |\n| Successful operation     | `200` | -                                                            |\n| Not Acceptable operation | `406` | Instance expects the input to be provided from the Topic API |\n\n</details>\n\n<details>\n<summary>\n    <strong class="get">[ GET ]</strong>  <code>/api/v1/instance/:id/output</code> <small>- get stream data from an instance and consume it through the endpoint</small>\n</summary>\n\n<br> <strong>Parameters</strong>\n\n<small>No parameters</small>\n\n<strong>Responses</strong>\n\n<small>Content-type: `application/octet-stream`</small>\n\n</details>\n\n<details>\n<summary>\n    <strong class="post">[ POST ]</strong>  <code>/api/v1/instance/:id/stdin\u200b</code> <small>- process.stdin</small>\n</summary>\n\n<br> <strong>Parameters</strong>\n\n<small>No parameters</small>\n\n<strong>Responses</strong>\n\n<small>Successful operation code: `200`</small>\n\n</details>\n\n<details>\n<summary>\n    <strong class="get">[ GET ]</strong>  <code>/api/v1/instance/:id/stdout</code> <small>- process.stdout</small>\n</summary>\n\n<br> <strong>Parameters</strong>\n\n<small>No parameters</small>\n\n<strong>Responses</strong>\n\n<small>Content-type: `application/octet-stream`</small>\n\n</details>\n\n<details>\n<summary>\n    <strong class="get">[ GET ]</strong>  <code>/api/v1/instance/:id/stderr</code> <small>- process.stderr</small>\n</summary>\n\n<br> <strong>Parameters</strong>\n\n<small>No parameters</small>\n\n<strong>Responses</strong>\n\n<small>Content-type: `application/octet-stream`</small>\n\n</details>\n\n<details>\n<summary>\n    <strong class="get">[ GET ]</strong>  <code>/api/v1/instance/:id/log</code> <small>- stream all instance logs</small>\n</summary>\n\n<br> <strong>Parameters</strong>\n\n<small>No parameters</small>\n\n<strong>Responses</strong>\n\n<small>Content-type: `application/octet-stream`</small>\n\n<small>Successful operation code: `200`</small>\n\n```bash\n2021-11-19T16:12:22.948Z log (Sequence) 42\n2021-11-19T16:12:23.949Z log (Sequence) 41\n2021-11-19T16:12:24.950Z log (Sequence) 40\n2021-11-19T16:12:25.951Z log (Sequence) 39\n2021-11-19T16:12:26.952Z log (Sequence) 38\n2021-11-19T16:12:27.952Z log (Sequence) 37\n2021-11-19T16:12:28.953Z log (Sequence) 36\n2021-11-19T16:12:29.953Z log (Sequence) 35\n```\n\n</details>\n\n___\n\n### Service Discovery: Topics\n\nIf a given topic does not exist, Transform-Hub creates it and stores the sent data in the newly created topic. The data is stored in the topic until the data is not consumed (either by the Topic API or by the Instances subscribing to this topic). When the data are sent to the topic they are written to the returned stream.\n\n<details>\n<summary>\n    <strong class="post">[ POST ]</strong>  <code>/api/v1/topics/:name\u200b</code> <small>- sends data to the topic</small>\n</summary>\n\n<br> <strong>Parameters</strong>\n\n<small><small>No parameters</small></small>\n\n<strong>Request Headers</strong>\n\n| Header         | Type                  | Description                                                             | Default                | Required |\n| -------------- | --------------------- | ----------------------------------------------------------------------- | ---------------------- | -------- |\n| `x-end-stream` | `boolean`             | If set to `true`, then close topic stream after processing the request. | false                  | no       |\n| `content-type` | `text`, `application` | Specifies data type of this topic                                       | `application/x-ndjson` | no       |\n\n<small> Supported types: `text/x-ndjson`, `application/x-ndjson`, `application/x-ndjson`, `text/plain`, `application/octet-stream`</small>\n\n<strong>Responses</strong>\n\n| Name                 | Code  | Description                                                           |\n| :------------------- | :---- | :-------------------------------------------------------------------- |\n| Successful operation | `200` | data was sent with the header indicating the end of data              |\n| Successful operation | `202` | data was sent without the header indicating the end of data (default) |\n\n</details>\n\n<details>\n<summary>\n    <strong class="get">[ GET ]</strong>  <code>/api/v1/topics/:name\u200b</code> <small>- get data from the topic</small>\n</summary>\n\n<br> <strong>Parameters</strong>\n\n<small>No parameters</small>\n\n<strong>Responses</strong>\n\n<small>Topic data stream.</small>\n\n<small>Successful operation code: `200`</small>\n\n```json\n{\n  "source": "Twitter",\n  "id": "850006245121695778",\n  "content": "Natural wetlands make up ~30% of global total CH4 emissions",\n  "user": {\n    "id": 1234994945,\n    "name": "Climate Change Conference",\n    "screen_name": "Climate Change",\n  }\n}\n```\n\n</details>\n\n___\n\n## Some important links\n\n* Scramjet, the company behind [Transform Hub](https://scramjet.org)\n* The [Scramjet Framework - functional reactive stream processing framework](https://framework.scramjet.org)\n* The [Transform Hub repo on github](https://github.com/scramjetorg/transform-hub)\n* You can see the [Scramjet Transform Hub API docs here](https://github.com/scramjetorg/transform-hub/tree/HEAD/docs/api-client/README.md)\n* You can see the [CLI documentation here](https://github.com/scramjetorg/transform-hub/tree/HEAD/packages/cli/README.md), but `si help` should also be quite effective.\n* Don\'t forget to ⭐ this repo if you like it, `subscribe` to releases and keep visiting us for new versions and updates.\n* You can [open an issue - file a bug report or a feature request here](https://github.com/scramjetorg/transform-hub/issues/new/choose)\n\n## License and contributions\n\nThis module is licensed under AGPL-3.0 license.\n\nThe Scramjet Transform Hub project is dual-licensed under the AGPL-3.0 and MIT licenses. Parts of the project that are linked with your programs are MIT licensed, the rest is AGPL.\n\n## Contributions\n\nWe accept valid contributions and we will be publishing a more specific project roadmap so contributors can propose features and also help us implement them. We kindly ask you that contributed commits are Signed-Off `git commit --sign-off`.\n\nWe provide support for contributors via test cases. If you expect a certain type of workflow to be officially supported, please specify and implement a test case in `Gherkin` format in `bdd` directory and include it in your pull request. More info about our BDD test you will find [here](https://github.com/scramjetorg/transform-hub/tree/HEAD/bdd/README.md).\n\n### Help wanted 👩\u200d🎓🧑👱\u200d♀️\n\nThe project need\'s your help! There\'s lots of work to do and we have a lot of plans. If you want to help and be part of the Scramjet team, please reach out to us, [on discord](https://scr.je/join-community-mg1) or email us: [opensource@scramjet.org](mailto:opensource@scramjet.org).\n\n### Donation 💸\n\nDo you like this project? It helped you to reduce time spent on delivering your solution? You are welcome to buy us a coffee ☕ Thanks a lot! 😉\n\n[You can sponsor us on github](https://github.com/sponsors/scramjetorg)\n\n* There\'s also a Paypal donation link if you prefer that:\n\n[![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=7F7V65C43EBMW)\n\n\n\n',
-    'author': 'Scramjet',
-    'author_email': 'open-source@scramjet.org',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
+Usage:
+
+```python
+import asyncio
+from client.host_client import HostClient
+from client_utils.base_client import BaseClient
+
+# your middleware token
+token = ''
+# set the token
+BaseClient.setDefaultHeaders({'Authorization': f'Bearer {token}'})
+
+# middleware url
+api_base ='https://api.scramjet.cloud/api/v1' 
+
+# url = {middlewareURL}/space/{manager_id}/api/v1/sth/{host_id}/api/v1
+host = HostClient(f'{api_base}/space/org-aa5bu150-9o5c-489b-83e3-b1yf7e086f3h-manager/api/v1/sth-1/api/v1')
+# get a list of Sequences
+res = asyncio.run(host.list_sequences())
+print(res)
+```
+
+---
+## More reading
+<p align="center">
+    <a href="https://github.com/scramjetorg/transform-hub/blob/HEAD/LICENSE"><img src="https://img.shields.io/github/license/scramjetorg/transform-hub?color=green&style=plastic" alt="GitHub license" /></a>
+    <a href="https://npmjs.org/package/@scramjet/sth"><img src="https://img.shields.io/github/v/tag/scramjetorg/transform-hub?label=version&color=blue&style=plastic" alt="STH version" /></a>
+    <a href="https://github.com/scramjetorg/transform-hub"><img src="https://img.shields.io/github/stars/scramjetorg/transform-hub?color=pink&style=plastic" alt="GitHub stars" /></a>
+    <a href="https://npmjs.org/package/@scramjet/sth"><img src="https://img.shields.io/npm/dt/@scramjet/sth?color=orange&style=plastic" alt="npm" /></a>
+    <a href="https://scr.je/join-community-mg1"><img alt="Discord" src="https://img.shields.io/discord/925384545342201896?label=discord&style=plastic"></a>
+    <a href="https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=7F7V65C43EBMW">
+        <img src="https://img.shields.io/badge/Donate-PayPal-green.svg?color=yellow&style=plastic" alt="Donate" />
+    </a>
+</p>
+<p align="center">⭐ Star us on GitHub — it motivates us a lot! 🚀 </p>
+
+<p align="center">
+    <img src="https://assets.scramjet.org/sth-logo.svg" alt="Scramjet Transform Hub Logo">
+</p>
+
+In the link below you will find more information about our stream protocol and API usage.
+
+See the code documentation here: [scramjetorg/transform-hub/docs/read-more/stream-and-api.md](https://github.com/scramjetorg/transform-hub/tree/HEAD/docs/read-more/stream-and-api.md)
+
+## Scramjet Transform Hub
+
+This package is part of [Scramjet Transform Hub](https://www.npmjs.org/package/@scramjet/sth).
+
+Scramjet Transform Hub is a deployment and execution platform. Once installed on a server, it will allow you to start your programs and keep them running on a remote machine. You will be able to start programs in the background or connect to them and see their output directly on your terminal. You will be able to pipe your local data to the program, as if it was running from your terminal. You can start your server in AWS, Google Cloud or Azure, start it on your local machine, install it on a Raspberry Pi or wherever else you'd like.
+
+## Use cases
+
+There's no limit what you can use it for. You want a stock checker? A chat bot? Maybe you'd like to automate your home? Retrieve sensor data? Maybe you have a lot of data and want to transfer and wrangle it? You have a database of cities and you'd like to enrich your data? You do machine learning and you want to train your set while the data is fetched in real time? Hey, you want to use it for something else and ask us if that's a good use? Ask us [via email](mailto:get@scramjet.org) or hop on our [Scramjet Discord](https://scr.je/join-community-mg1)!
+___
+
+### Host operations
+
+<details>
+<summary>
+    <strong class="get">[ GET ]</strong>  <code>/api/v1/version</code> <small>- show the Host version</small>
+</summary>
+
+<br> <strong>Parameters</strong>
+
+<small>No parameters</small>
+
+<strong>Responses</strong>
+
+<small>Successful operation code: `200`</small>
+
+```json
+{ "version" : "0.12.2" }
+```
+
+</details>
+
+<details>
+<summary>
+    <strong class="get">[ GET ]</strong>  <code>/api/v1/sequences</code> <small>- show all Sequences saved on the Host</small>
+</summary>
+
+<br> <strong>Parameters</strong>
+
+<small>No parameters</small>
+
+<strong>Responses</strong>
+
+<small>Successful operation code: `200`</small>
+
+```json
+[
+  {
+    "instances": [], // a list of all running Instances of this Sequence
+    "id": "eea8bc33-440f-4a17-8931-eb22a17d5d56", // Sequence ID
+    "config": {
+      "container": {
+        "image": "scramjetorg/runner:0.12.2",
+        "maxMem": 512,
+        "exposePortsRange": [
+          30000,
+          32767
+        ],
+        "hostIp": "0.0.0.0"
+      },
+      "name": "@scramjet/hello-alice-out",
+      "version": "0.12.2",
+      "engines": {
+        "node": ">=10"
+      },
+      "config": {},
+      "sequencePath": "index", // a path to file with a main function
+      "packageVolumeId": "eea8bc33-440f-4a17-8931-eb22a17d5d56"
+    }
+  },
+  {
+    "instances": [
+      "02381acf-cb16-4cff-aa9b-f22f04ada94f"
+    ],
+    "id": "3ec02b93-4ca9-4d23-baab-048dab5ffda4",
+    "config": {
+      "container": {
+        "image": "scramjetorg/runner:0.12.2",
+        "maxMem": 512,
+        "exposePortsRange": [
+          30000,
+          32767
+        ],
+        "hostIp": "0.0.0.0"
+      },
+      "name": "@scramjet/checksum-sequence",
+      "version": "0.12.2",
+      "engines": {},
+      "config": {},
+      "sequencePath": "index.js",
+      "packageVolumeId": "3ec02b93-4ca9-4d23-baab-048dab5ffda4"
+    }
+  }
+]
+```
+
+</details>
+
+<details>
+<summary>
+    <strong class="get">[ GET ]</strong>  <code>/api/v1/instances</code> <small>- show all Instances running on the Host</small>
+</summary>
+
+<br> <strong>Parameters</strong>
+
+<small>No parameters</small>
+
+<strong>Responses</strong>
+
+<small>Successful operation code: `200`</small>
+
+```json
+[
+  {
+    "id": "02381acf-cb16-4cff-aa9b-f22f04ada94f", // Instance ID
+    "sequence": "3ec02b93-4ca9-4d23-baab-048dab5ffda4" // Sequence ID
+  },
+  {
+    "id": "ab0272d8-c9b0-43f7-9e7e-bcac9ec0f21f",
+    "sequence": "e4ca555c-ced1-4a13-b531-f43016eaf4ed"
+  }
+]
+```
+
+</details>
+
+<details>
+<summary>
+    <strong class="get">[ GET ]</strong>  <code>/api/v1/load-check</code> <small>- monitor CPU, memory and disk usage metrics on the Host machine</small>
+</summary>
+
+<br> <strong>Parameters</strong>
+
+<small>No parameters</small>
+
+<strong>Responses</strong>
+
+<small>Successful operation code: `200`</small>
+
+```json
+{
+  "avgLoad": 0.08,
+  "currentLoad": 5.190776257704936,
+  "memFree": 4634816512,
+  "memUsed": 8050364416,
+  "fsSize": [
+    {
+      "fs": "/dev/sda1",
+      "type": "ext4",
+      "size": 20838993920,
+      "used": 14939455488,
+      "available": 5882761216,
+      "use": 71.75,
+      "mount": "/"
+    },
+    {
+      "fs": "/dev/sda15",
+      "type": "vfat",
+      "size": 109422592,
+      "used": 9621504,
+      "available": 99801088,
+      "use": 8.79,
+      "mount": "/boot/efi"
+    }
+  ]
+}
+
+```
+
+</details>
+
+<details>
+<summary>
+    <strong class="get">[ GET ]</strong>  <code>/api/v1/log</code> <small>- monitor CPU, memory and disk usage metrics on the Host machine</small>
+</summary>
+
+<br> <strong>Parameters</strong>
+
+<small>No parameters</small>
+
+<strong>Responses</strong>
+
+<small>Content-type: `application/octet-stream`</small>
+
+<small>Successful operation code: `200`</small>
+
+```bash
+2021-11-19T16:04:47.094Z log (object:Host) Host main called.
+2021-11-19T16:04:47.100Z info (object:SocketServer) Server on: /tmp/scramjet-socket-server-path
+2021-11-19T16:04:47.104Z info (object:Host) API listening on: 127.0.0.1:8000
+2021-11-19T16:05:08.228Z info (object:Host) New sequence incoming...
+2021-11-19T16:05:08.229Z log (object:LifecycleDockerAdapterSequence) Docker sequence adapter init.
+2021-11-19T16:05:08.229Z log (object:DockerodeDockerHelper) Checking image scramjetorg/pre-runner:0.12.2
+2021-11-19T16:05:12.234Z info (object:LifecycleDockerAdapterSequence) Docker sequence adapter done.
+2021-11-19T16:05:12.246Z log (object:LifecycleDockerAdapterSequence) Volume created. Id:  c50fe4d3-89cc-4685-a82a-16cbc744733d
+2021-11-19T16:05:12.246Z log (object:LifecycleDockerAdapterSequence) Starting PreRunner { image: 'scramjetorg/pre-runner:0.12.2', maxMem: 128 }
+2021-11-19T16:05:13.536Z log (object:DockerodeDockerHelper) Checking image scramjetorg/runner:0.12.2
+2021-11-19T16:05:16.670Z info (object:SequenceStore) New sequence added: c50fe4d3-89cc-4685-a82a-16cbc744733d
+2021-11-19T16:05:16.672Z info (object:Host) Sequence identified: {
+  container: {
+    image: 'scramjetorg/runner:0.12.2',
+    maxMem: 512,
+    exposePortsRange: [ 30000, 32767 ],
+    hostIp: '0.0.0.0'
+  },
+  name: '@scramjet/multi-outputs',
+  version: '0.12.2',
+  engines: {},
+  config: {},
+  sequencePath: 'index.js',
+  packageVolumeId: 'c50fe4d3-89cc-4685-a82a-16cbc744733d'
+}
+2021-11-19T16:05:16.691Z debug (object:Host) Request date: 2021-11-19T16:05:08.239Z, method: POST, url: /api/v1/sequence, status: 202
+```
+
+</details>
+
+___
+
+### Sequence operations
+
+<details>
+<summary>
+    <strong class="post">[ POST ]</strong> <code>/api/v1/sequence</code> <small>- add new sequence</small>
+</summary>
+
+<br><strong>Parameters</strong>
+
+| Name        | Type     | Description                         | Required |
+| ----------- | -------- | ----------------------------------- | -------- |
+| `file`      | `binary` | compressed package in tar.gz format | yes      |
+| `appConfig` | `json`   | additional package.json config file | no       |
+
+<strong>Responses</strong>
+
+<small>Accepted operation code: `202`</small>
+
+```json
+{
+  "id": "2c3068e5-7c74-45bb-a017-1979c41fc6d0" // sequence id
+}
+```
+
+</details>
+
+<details>
+<summary>
+    <strong class="get">[ GET ]</strong>  <code>/api/v1/sequences</code> <small>- show list of sequences</small>
+</summary>
+
+<br> <strong>Parameters</strong>
+
+<small>No parameters</small>
+
+<strong>Responses</strong>
+
+<small>Successful operation code: `200`</small>
+
+```json
+[
+  {
+    "instances": [
+      "742d2713-7ab6-4cde-82f3-a7beabdd4e98"       // list of sequence instances
+    ],
+    "id": "bdef63db-d3a0-45c8-85db-e94ebb96097f",  // sequence id
+    "config": {
+      "container": {
+        "image": "scramjetorg/runner:0.12.2",
+        "maxMem": 512
+      },
+      "name": "@scramjet/transform-hub",
+      "version": "0.12.2",
+      "engines": {},
+      "config": {},
+      "sequencePath": "index.js",
+      "packageVolumeId": "bdef63db-d3a0-45c8-85db-e94ebb96097f"
+    }
+  }
+]
+```
+
+</details>
+
+<details>
+<summary>
+    <strong class="post">[ POST ]</strong> <code>/api/v1/sequence/:id/start</code> <small>- start chosen sequence</small>
+</summary>
+
+<br> <strong>Parameters</strong>
+
+| Name        | Type   | Description                                           | Required |
+| ----------- | ------ | ----------------------------------------------------- | -------- |
+| `appConfig` | `json` | additional package.json config file                   | no       |
+| `args`      | `json` | additional arguments that instance should starts with | no       |
+
+<strong>Responses</strong>
+
+<small>Successful operation code: `200`</small>
+
+```json
+{
+  "id": "681c856e-dfa4-46a1-951d-47b27345552e"
+}
+```
+
+</details>
+
+<details>
+<summary>
+    <strong class="delete">[ DELETE ]</strong> <code>/api/v1/sequence/:id</code> <small>- delete a sequence by id</small>
+</summary>
+
+<br> <strong>Parameters</strong>
+
+<small>No parameters</small>
+
+<strong>Responses</strong>
+
+<small>Successful operation code: `200`</small>
+
+```json
+{
+  "id": "2c3068e5-7c74-45bb-a017-1979c41fc6d0"
+}
+```
+
+<small>Conflict operation code: `409` - the instance is still running</small>
+
+```json
+{
+  "error": "Can't remove sequence in use."
+}
+```
+
+</details>
+
+___
+
+### Instance basic operations
+
+<details>
+<summary>
+    <strong class="get">[ GET ]</strong> <code>/api/v1/instances</code> <small>- list all instances</small>
+</summary>
+
+<br> <strong>Parameters</strong>
+
+<small>No parameters</small>
+
+<strong>Responses</strong>
+
+<small>Successful operation code: `200`</small>
+
+```json
+[
+  {
+    "id": "742d2713-7ab6-4cde-82f3-a7beabdd4e98",
+    "sequence": "bdef63db-d3a0-45c8-85db-e94ebb96097f"
+  },
+  {
+    "id": "681c856e-dfa4-46a1-951d-47b27345552e",
+    "sequence": "bdef63db-d3a0-45c8-85db-e94ebb96097f"
+  },
+  {
+    "id": "21f787ed-6b9e-4e9f-828e-afe428d84833",
+    "sequence": "bdef63db-d3a0-45c8-85db-e94ebb96097f"
+  }
+]
+```
+
+</details>
+
+<details>
+<summary>
+    <strong class="get">[ GET ]</strong> <code>/api/v1/instance/:id</code> <small>- show data of chosen instance</small>
+</summary>
+
+<br> <strong>Parameters</strong>
+
+<small>No parameters</small>
+
+<strong>Responses</strong>
+
+| Name                 | Code  | Description                                 |
+| :------------------- | :---- | :------------------------------------------ |
+| Successful operation | `200` | Returns JSON data                           |
+| Not Found operation  | `404` | For example if instance was already stopped |
+
+```json
+{
+  "created": "2021-10-29T16:08:36.524Z",
+  "started": "2021-10-29T16:08:38.701Z",
+  "sequenceId": "b0c02fdc-b05f-4f26-9d68-43a702eb7b44"
+}
+```
+
+</details>
+
+<details>
+<summary>
+    <strong class="post">[ POST ]</strong> <code>/api/v1/instance/:id/_stop</code> <small>- end instance gracefully and prolong operations or not for task completion​</small>
+</summary>
+
+<br> <strong>Parameters</strong>
+
+| Name               | Type      | Description                                                                     | Required |
+| ------------------ | --------- | ------------------------------------------------------------------------------- | -------- |
+| `timeout`          | `number`  | The number of milliseconds before the Instance will be killed. Default: 7000ms. | no       |
+| `canCallKeepalive` | `boolean` | If set to true, the instance will prolong the running. Default: false.          | no       |
+
+<strong>Responses</strong>
+
+<small>Successful operation code: `200`</small>
+
+```json
+{
+   "code": 0,
+   "type": "string",
+   "message": "string"
 }
+```
+
+</details>
+
+<details>
+<summary>
+    <strong class="post">[ POST ]</strong>  <code>api/v1/instance/:id/_kill</code> <small>- end instance gracefully waiting for unfinished tasks</small>
+</summary>
+
+<br> <strong>Parameters</strong>
+
+<small>No parameters</small>
+
+<strong>Responses</strong>
+
+<small>Accepted operation code: `202`</small>
+
+```text
+No body returned
+```
+
+</details>
+
+<details>
+<summary>
+    <strong class="get">[ GET ]</strong>  <code>/api/v1/instance/:id/health</code> <small>- check status about instance health</small>
+</summary>
+
+<br> <strong>Parameters</strong>
+
+<small>No parameters</small>
+
+<strong>Responses</strong>
+
+<small>Successful operation code: `200`</small>
+
+```json
+{
+  "cpuTotalUsage": 529325247,
+  "healthy": true,
+  "limit": 536870912,
+  "memoryMaxUsage": 16117760,
+  "memoryUsage": 14155776,
+  "networkRx": 1086,
+  "networkTx": 0,
+  "containerId": "1c993c4ff774fac06185aa9554cf40c23b03e1479a7e0d14827708161b08ae51"
+}
+```
+
+</details>
+
+___
+
+### Instance advanced operation
+
+<details>
+<summary>
+    <strong class="post">[ POST ]</strong>  <code>/api/v1/instance/:id/_event</code> <small>- send event to the Instance</small>
+</summary>
+
+<br> <strong>Parameters</strong>
+
+| Name        | Type     | Description                  | Required |
+| :---------- | :------- | ---------------------------- | -------- |
+| `eventName` | `string` | Name of an event             | true     |
+| `message`   | `string` | JSON formatted event payload | false    |
+
+<strong>Responses</strong>
+
+<small>Content-type: `application/octet-stream`</small>
+
+</details>
+
+<details>
+<summary>
+    <strong class="get">[ GET ]</strong>  <code>/api/v1/instance/:id/event</code> <small>- get the data stream with the events from the Instance</small>
+</summary>
+
+<br> <strong>Parameters</strong>
+
+<small>No parameters</small>
+
+<strong>Responses</strong>
+
+<small>Content-type: `application/octet-stream`</small>
+
+</details>
+
+<details>
+<summary>
+    <strong class="get">[ GET ]</strong>  <code>/api/v1/instance/:id/once</code> <small>- get the last event sent by the Instance</small>
+</summary>
+
+<br> <strong>Parameters</strong>
+
+<small>No parameters</small>
+
+<strong>Responses</strong>
+
+<small>Content-type: `application/octet-stream`</small>
+
+</details>
+
+<details>
+<summary>
+    <strong class="post">[ POST ]</strong>  <code>/api/v1/instance/:id/input</code> <small>- send data to the input stream of the Instance to consume it</small>
+</summary>
+
+<br> <strong>Parameters</strong>
+
+<small>No parameters</small>
+
+<strong>Responses</strong>
+
+| Name                     | Code  | Description                                                  |
+| :----------------------- | :---- | :----------------------------------------------------------- |
+| Successful operation     | `200` | -                                                            |
+| Not Acceptable operation | `406` | Instance expects the input to be provided from the Topic API |
+
+</details>
+
+<details>
+<summary>
+    <strong class="get">[ GET ]</strong>  <code>/api/v1/instance/:id/output</code> <small>- get stream data from an instance and consume it through the endpoint</small>
+</summary>
+
+<br> <strong>Parameters</strong>
+
+<small>No parameters</small>
+
+<strong>Responses</strong>
+
+<small>Content-type: `application/octet-stream`</small>
+
+</details>
+
+<details>
+<summary>
+    <strong class="post">[ POST ]</strong>  <code>/api/v1/instance/:id/stdin​</code> <small>- process.stdin</small>
+</summary>
+
+<br> <strong>Parameters</strong>
+
+<small>No parameters</small>
+
+<strong>Responses</strong>
+
+<small>Successful operation code: `200`</small>
+
+</details>
+
+<details>
+<summary>
+    <strong class="get">[ GET ]</strong>  <code>/api/v1/instance/:id/stdout</code> <small>- process.stdout</small>
+</summary>
+
+<br> <strong>Parameters</strong>
+
+<small>No parameters</small>
+
+<strong>Responses</strong>
+
+<small>Content-type: `application/octet-stream`</small>
+
+</details>
+
+<details>
+<summary>
+    <strong class="get">[ GET ]</strong>  <code>/api/v1/instance/:id/stderr</code> <small>- process.stderr</small>
+</summary>
+
+<br> <strong>Parameters</strong>
+
+<small>No parameters</small>
+
+<strong>Responses</strong>
+
+<small>Content-type: `application/octet-stream`</small>
+
+</details>
+
+<details>
+<summary>
+    <strong class="get">[ GET ]</strong>  <code>/api/v1/instance/:id/log</code> <small>- stream all instance logs</small>
+</summary>
+
+<br> <strong>Parameters</strong>
+
+<small>No parameters</small>
+
+<strong>Responses</strong>
+
+<small>Content-type: `application/octet-stream`</small>
+
+<small>Successful operation code: `200`</small>
+
+```bash
+2021-11-19T16:12:22.948Z log (Sequence) 42
+2021-11-19T16:12:23.949Z log (Sequence) 41
+2021-11-19T16:12:24.950Z log (Sequence) 40
+2021-11-19T16:12:25.951Z log (Sequence) 39
+2021-11-19T16:12:26.952Z log (Sequence) 38
+2021-11-19T16:12:27.952Z log (Sequence) 37
+2021-11-19T16:12:28.953Z log (Sequence) 36
+2021-11-19T16:12:29.953Z log (Sequence) 35
+```
+
+</details>
+
+___
+
+### Service Discovery: Topics
+
+If a given topic does not exist, Transform-Hub creates it and stores the sent data in the newly created topic. The data is stored in the topic until the data is not consumed (either by the Topic API or by the Instances subscribing to this topic). When the data are sent to the topic they are written to the returned stream.
+
+<details>
+<summary>
+    <strong class="post">[ POST ]</strong>  <code>/api/v1/topics/:name​</code> <small>- sends data to the topic</small>
+</summary>
+
+<br> <strong>Parameters</strong>
+
+<small><small>No parameters</small></small>
+
+<strong>Request Headers</strong>
+
+| Header         | Type                  | Description                                                             | Default                | Required |
+| -------------- | --------------------- | ----------------------------------------------------------------------- | ---------------------- | -------- |
+| `x-end-stream` | `boolean`             | If set to `true`, then close topic stream after processing the request. | false                  | no       |
+| `content-type` | `text`, `application` | Specifies data type of this topic                                       | `application/x-ndjson` | no       |
+
+<small> Supported types: `text/x-ndjson`, `application/x-ndjson`, `application/x-ndjson`, `text/plain`, `application/octet-stream`</small>
+
+<strong>Responses</strong>
+
+| Name                 | Code  | Description                                                           |
+| :------------------- | :---- | :-------------------------------------------------------------------- |
+| Successful operation | `200` | data was sent with the header indicating the end of data              |
+| Successful operation | `202` | data was sent without the header indicating the end of data (default) |
+
+</details>
+
+<details>
+<summary>
+    <strong class="get">[ GET ]</strong>  <code>/api/v1/topics/:name​</code> <small>- get data from the topic</small>
+</summary>
+
+<br> <strong>Parameters</strong>
+
+<small>No parameters</small>
+
+<strong>Responses</strong>
+
+<small>Topic data stream.</small>
+
+<small>Successful operation code: `200`</small>
+
+```json
+{
+  "source": "Twitter",
+  "id": "850006245121695778",
+  "content": "Natural wetlands make up ~30% of global total CH4 emissions",
+  "user": {
+    "id": 1234994945,
+    "name": "Climate Change Conference",
+    "screen_name": "Climate Change",
+  }
+}
+```
+
+</details>
+
+___
+
+## Some important links
+
+* Scramjet, the company behind [Transform Hub](https://scramjet.org)
+* The [Scramjet Framework - functional reactive stream processing framework](https://framework.scramjet.org)
+* The [Transform Hub repo on github](https://github.com/scramjetorg/transform-hub)
+* You can see the [Scramjet Transform Hub API docs here](https://github.com/scramjetorg/transform-hub/tree/HEAD/docs/api-client/README.md)
+* You can see the [CLI documentation here](https://github.com/scramjetorg/transform-hub/tree/HEAD/packages/cli/README.md), but `si help` should also be quite effective.
+* Don't forget to ⭐ this repo if you like it, `subscribe` to releases and keep visiting us for new versions and updates.
+* You can [open an issue - file a bug report or a feature request here](https://github.com/scramjetorg/transform-hub/issues/new/choose)
+
+## License and contributions
+
+This module is licensed under AGPL-3.0 license.
+
+The Scramjet Transform Hub project is dual-licensed under the AGPL-3.0 and MIT licenses. Parts of the project that are linked with your programs are MIT licensed, the rest is AGPL.
+
+## Contributions
+
+We accept valid contributions and we will be publishing a more specific project roadmap so contributors can propose features and also help us implement them. We kindly ask you that contributed commits are Signed-Off `git commit --sign-off`.
+
+We provide support for contributors via test cases. If you expect a certain type of workflow to be officially supported, please specify and implement a test case in `Gherkin` format in `bdd` directory and include it in your pull request. More info about our BDD test you will find [here](https://github.com/scramjetorg/transform-hub/tree/HEAD/bdd/README.md).
+
+### Help wanted 👩‍🎓🧑👱‍♀️
+
+The project need's your help! There's lots of work to do and we have a lot of plans. If you want to help and be part of the Scramjet team, please reach out to us, [on discord](https://scr.je/join-community-mg1) or email us: [opensource@scramjet.org](mailto:opensource@scramjet.org).
+
+### Donation 💸
+
+Do you like this project? It helped you to reduce time spent on delivering your solution? You are welcome to buy us a coffee ☕ Thanks a lot! 😉
+
+[You can sponsor us on github](https://github.com/sponsors/scramjetorg)
+
+* There's also a Paypal donation link if you prefer that:
+
+[![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=7F7V65C43EBMW)
+
 
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,267 +1,239 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \
-['client_utils'] package_data = \ {'': ['*']} install_requires = \
-['aiohttp>=3.8.3,<4.0.0', 'url_normalize>=1.4.3,<2.0.0'] setup_kwargs =
-{ 'name': 'scramjet-client-utils', 'version': '1.0.1', 'description': '',
-'long_description': '
+Metadata-Version: 2.1 Name: scramjet-client-utils Version: 1.1.0 Home-page:
+https://github.com/scramjetorg/api-client-python/tree/main/client_utils Author:
+Scramjet Author-email: open-source@scramjet.org Requires-Python: >=3.9,<4.0
+Description-Content-Type: text/markdown
            ****** Scramjet Transform Hub API Clients utility ******
-\n\nThe package provides utilities for API clients. Each of the API clients
-make use out of it.\n\nUsage:\n\n```python\nimport asyncio\nimport json\nfrom
-client.host_client import HostClient\nfrom client_utils import ClientUtils\n\n#
-your middleware token\ntoken = \'\'\n# set the
-token\nClientUtils.setDefaultHeaders({\'Authorization\': f\'Bearer
-{token}\'})\n\n# middleware url\napi_base =\'https://api.scramjet.cloud/api/
-v1\' \n\n# url = {middlewareURL}/space/{manager_id}/api/v1/{host_id}/api/
-v1\nhost = HostClient(f\'{api_base}/space/org-aa5bu150-9o5c-489b-83e3-
-b1yf7e086f3h-manager/api/v1/sth-1/api/v1\')\n# get a list of Sequences\nres =
-asyncio.run(host.list_sequences())\n# convert responose to json\nsequences =
-json.loads(res)\n```\n\n---\n## More reading\n
-\n [GitHub_license]\n [STH_version]\n [GitHub_stars]\n [npm]\n [Discord]\n \n_
-                                 [Donate]\n\n
-\n
+The package provides utilities for API clients. Each of the API clients make
+use out of it. Usage: ```python import asyncio from client.host_client import
+HostClient from client_utils.base_client import BaseClient # your middleware
+token token = '' # set the token BaseClient.setDefaultHeaders({'Authorization':
+f'Bearer {token}'}) # middleware url api_base ='https://api.scramjet.cloud/api/
+v1' # url = {middlewareURL}/space/{manager_id}/api/v1/sth/{host_id}/api/v1 host
+= HostClient(f'{api_base}/space/org-aa5bu150-9o5c-489b-83e3-b1yf7e086f3h-
+manager/api/v1/sth-1/api/v1') # get a list of Sequences res = asyncio.run
+(host.list_sequences()) print(res) ``` --- ## More reading
+    [GitHub_license] [STH_version] [GitHub_stars] [npm] [Discord] [Donate]
              â­ Star us on GitHub â it motivates us a lot! ð
-\n\n
-                      \n [Scramjet Transform Hub Logo]\n
-\n\nIn the link below you will find more information about our stream protocol
-and API usage.\n\nSee the code documentation here: [scramjetorg/transform-hub/
-docs/read-more/stream-and-api.md](https://github.com/scramjetorg/transform-hub/
-tree/HEAD/docs/read-more/stream-and-api.md)\n\n## Scramjet Transform
-Hub\n\nThis package is part of [Scramjet Transform Hub](https://www.npmjs.org/
-package/@scramjet/sth).\n\nScramjet Transform Hub is a deployment and execution
-platform. Once installed on a server, it will allow you to start your programs
-and keep them running on a remote machine. You will be able to start programs
-in the background or connect to them and see their output directly on your
-terminal. You will be able to pipe your local data to the program, as if it was
-running from your terminal. You can start your server in AWS, Google Cloud or
-Azure, start it on your local machine, install it on a Raspberry Pi or wherever
-else you\'d like.\n\n## Use cases\n\nThere\'s no limit what you can use it for.
-You want a stock checker? A chat bot? Maybe you\'d like to automate your home?
-Retrieve sensor data? Maybe you have a lot of data and want to transfer and
-wrangle it? You have a database of cities and you\'d like to enrich your data?
-You do machine learning and you want to train your set while the data is
-fetched in real time? Hey, you want to use it for something else and ask us if
-that\'s a good use? Ask us [via email](mailto:get@scramjet.org) or hop on our
-[Scramjet Discord](https://scr.je/join-community-mg1)!\n___\n\n### Host
-operations\n\n\n\n [ GET ] /api/v1/version - show the Host version\n\n\n
-Parameters\n\nNo parameters\n\nResponses\n\nSuccessful operation code:
-`200`\n\n```json\n{ "version" : "0.12.2" }\n```\n\n\n\n\n\n [ GET ] /api/v1/
-sequences - show all Sequences saved on the Host\n\n\n
-Parameters\n\nNo parameters\n\nResponses\n\nSuccessful operation code:
-`200`\n\n```json\n[\n {\n "instances": [], // a list of all running Instances
-of this Sequence\n "id": "eea8bc33-440f-4a17-8931-eb22a17d5d56", // Sequence
-ID\n "config": {\n "container": {\n "image": "scramjetorg/runner:0.12.2",\n
-"maxMem": 512,\n "exposePortsRange": [\n 30000,\n 32767\n ],\n "hostIp":
-"0.0.0.0"\n },\n "name": "@scramjet/hello-alice-out",\n "version": "0.12.2",\n
-"engines": {\n "node": ">=10"\n },\n "config": {},\n "sequencePath": "index", /
-/ a path to file with a main function\n "packageVolumeId": "eea8bc33-440f-4a17-
-8931-eb22a17d5d56"\n }\n },\n {\n "instances": [\n "02381acf-cb16-4cff-aa9b-
-f22f04ada94f"\n ],\n "id": "3ec02b93-4ca9-4d23-baab-048dab5ffda4",\n "config":
-{\n "container": {\n "image": "scramjetorg/runner:0.12.2",\n "maxMem": 512,\n
-"exposePortsRange": [\n 30000,\n 32767\n ],\n "hostIp": "0.0.0.0"\n },\n
-"name": "@scramjet/checksum-sequence",\n "version": "0.12.2",\n "engines":
-{},\n "config": {},\n "sequencePath": "index.js",\n "packageVolumeId":
-"3ec02b93-4ca9-4d23-baab-048dab5ffda4"\n }\n }\n]\n```\n\n\n\n\n\n [ GET ] /
-api/v1/instances - show all Instances running on the Host\n\n\n
-Parameters\n\nNo parameters\n\nResponses\n\nSuccessful operation code:
-`200`\n\n```json\n[\n {\n "id": "02381acf-cb16-4cff-aa9b-f22f04ada94f", /
-/ Instance ID\n "sequence": "3ec02b93-4ca9-4d23-baab-048dab5ffda4" // Sequence
-ID\n },\n {\n "id": "ab0272d8-c9b0-43f7-9e7e-bcac9ec0f21f",\n "sequence":
-"e4ca555c-ced1-4a13-b531-f43016eaf4ed"\n }\n]\n```\n\n\n\n\n\n [ GET ] /api/v1/
-load-check - monitor CPU, memory and disk usage metrics on the Host
-machine\n\n\n
-Parameters\n\nNo parameters\n\nResponses\n\nSuccessful operation code:
-`200`\n\n```json\n{\n "avgLoad": 0.08,\n "currentLoad": 5.190776257704936,\n
-"memFree": 4634816512,\n "memUsed": 8050364416,\n "fsSize": [\n {\n "fs": "/
-dev/sda1",\n "type": "ext4",\n "size": 20838993920,\n "used": 14939455488,\n
-"available": 5882761216,\n "use": 71.75,\n "mount": "/"\n },\n {\n "fs": "/dev/
-sda15",\n "type": "vfat",\n "size": 109422592,\n "used": 9621504,\n
-"available": 99801088,\n "use": 8.79,\n "mount": "/boot/efi"\n }\n
-]\n}\n\n```\n\n\n\n\n\n [ GET ] /api/v1/log - monitor CPU, memory and disk
-usage metrics on the Host machine\n\n\n
-Parameters\n\nNo parameters\n\nResponses\n\nContent-type: `application/octet-
-stream`\n\nSuccessful operation code: `200`\n\n```bash\n2021-11-19T16:04:
-47.094Z log (object:Host) Host main called.\n2021-11-19T16:04:47.100Z info
-(object:SocketServer) Server on: /tmp/scramjet-socket-server-path\n2021-11-
-19T16:04:47.104Z info (object:Host) API listening on: 127.0.0.1:8000\n2021-11-
-19T16:05:08.228Z info (object:Host) New sequence incoming...\n2021-11-19T16:05:
-08.229Z log (object:LifecycleDockerAdapterSequence) Docker sequence adapter
-init.\n2021-11-19T16:05:08.229Z log (object:DockerodeDockerHelper) Checking
-image scramjetorg/pre-runner:0.12.2\n2021-11-19T16:05:12.234Z info (object:
-LifecycleDockerAdapterSequence) Docker sequence adapter done.\n2021-11-19T16:
-05:12.246Z log (object:LifecycleDockerAdapterSequence) Volume created. Id:
-c50fe4d3-89cc-4685-a82a-16cbc744733d\n2021-11-19T16:05:12.246Z log (object:
-LifecycleDockerAdapterSequence) Starting PreRunner { image: \'scramjetorg/pre-
-runner:0.12.2\', maxMem: 128 }\n2021-11-19T16:05:13.536Z log (object:
-DockerodeDockerHelper) Checking image scramjetorg/runner:0.12.2\n2021-11-19T16:
+                         [Scramjet Transform Hub Logo]
+In the link below you will find more information about our stream protocol and
+API usage. See the code documentation here: [scramjetorg/transform-hub/docs/
+read-more/stream-and-api.md](https://github.com/scramjetorg/transform-hub/tree/
+HEAD/docs/read-more/stream-and-api.md) ## Scramjet Transform Hub This package
+is part of [Scramjet Transform Hub](https://www.npmjs.org/package/@scramjet/
+sth). Scramjet Transform Hub is a deployment and execution platform. Once
+installed on a server, it will allow you to start your programs and keep them
+running on a remote machine. You will be able to start programs in the
+background or connect to them and see their output directly on your terminal.
+You will be able to pipe your local data to the program, as if it was running
+from your terminal. You can start your server in AWS, Google Cloud or Azure,
+start it on your local machine, install it on a Raspberry Pi or wherever else
+you'd like. ## Use cases There's no limit what you can use it for. You want a
+stock checker? A chat bot? Maybe you'd like to automate your home? Retrieve
+sensor data? Maybe you have a lot of data and want to transfer and wrangle it?
+You have a database of cities and you'd like to enrich your data? You do
+machine learning and you want to train your set while the data is fetched in
+real time? Hey, you want to use it for something else and ask us if that's a
+good use? Ask us [via email](mailto:get@scramjet.org) or hop on our [Scramjet
+Discord](https://scr.je/join-community-mg1)! ___ ### Host operations   [ GET ]
+/api/v1/version - show the Host version
+Parameters No parameters Responses Successful operation code: `200` ```json
+{ "version" : "0.12.2" } ```    [ GET ] /api/v1/sequences - show all Sequences
+saved on the Host
+Parameters No parameters Responses Successful operation code: `200` ```json [
+{ "instances": [], // a list of all running Instances of this Sequence "id":
+"eea8bc33-440f-4a17-8931-eb22a17d5d56", // Sequence ID "config": { "container":
+{ "image": "scramjetorg/runner:0.12.2", "maxMem": 512, "exposePortsRange":
+[ 30000, 32767 ], "hostIp": "0.0.0.0" }, "name": "@scramjet/hello-alice-out",
+"version": "0.12.2", "engines": { "node": ">=10" }, "config": {},
+"sequencePath": "index", // a path to file with a main function
+"packageVolumeId": "eea8bc33-440f-4a17-8931-eb22a17d5d56" } }, { "instances":
+[ "02381acf-cb16-4cff-aa9b-f22f04ada94f" ], "id": "3ec02b93-4ca9-4d23-baab-
+048dab5ffda4", "config": { "container": { "image": "scramjetorg/runner:0.12.2",
+"maxMem": 512, "exposePortsRange": [ 30000, 32767 ], "hostIp": "0.0.0.0" },
+"name": "@scramjet/checksum-sequence", "version": "0.12.2", "engines": {},
+"config": {}, "sequencePath": "index.js", "packageVolumeId": "3ec02b93-4ca9-
+4d23-baab-048dab5ffda4" } } ] ```    [ GET ] /api/v1/instances - show all
+Instances running on the Host
+Parameters No parameters Responses Successful operation code: `200` ```json [
+{ "id": "02381acf-cb16-4cff-aa9b-f22f04ada94f", // Instance ID "sequence":
+"3ec02b93-4ca9-4d23-baab-048dab5ffda4" // Sequence ID }, { "id": "ab0272d8-
+c9b0-43f7-9e7e-bcac9ec0f21f", "sequence": "e4ca555c-ced1-4a13-b531-
+f43016eaf4ed" } ] ```    [ GET ] /api/v1/load-check - monitor CPU, memory and
+disk usage metrics on the Host machine
+Parameters No parameters Responses Successful operation code: `200` ```json
+{ "avgLoad": 0.08, "currentLoad": 5.190776257704936, "memFree": 4634816512,
+"memUsed": 8050364416, "fsSize": [ { "fs": "/dev/sda1", "type": "ext4", "size":
+20838993920, "used": 14939455488, "available": 5882761216, "use": 71.75,
+"mount": "/" }, { "fs": "/dev/sda15", "type": "vfat", "size": 109422592,
+"used": 9621504, "available": 99801088, "use": 8.79, "mount": "/boot/efi" } ] }
+```    [ GET ] /api/v1/log - monitor CPU, memory and disk usage metrics on the
+Host machine
+Parameters No parameters Responses Content-type: `application/octet-stream`
+Successful operation code: `200` ```bash 2021-11-19T16:04:47.094Z log (object:
+Host) Host main called. 2021-11-19T16:04:47.100Z info (object:SocketServer)
+Server on: /tmp/scramjet-socket-server-path 2021-11-19T16:04:47.104Z info
+(object:Host) API listening on: 127.0.0.1:8000 2021-11-19T16:05:08.228Z info
+(object:Host) New sequence incoming... 2021-11-19T16:05:08.229Z log (object:
+LifecycleDockerAdapterSequence) Docker sequence adapter init. 2021-11-19T16:05:
+08.229Z log (object:DockerodeDockerHelper) Checking image scramjetorg/pre-
+runner:0.12.2 2021-11-19T16:05:12.234Z info (object:
+LifecycleDockerAdapterSequence) Docker sequence adapter done. 2021-11-19T16:05:
+12.246Z log (object:LifecycleDockerAdapterSequence) Volume created. Id:
+c50fe4d3-89cc-4685-a82a-16cbc744733d 2021-11-19T16:05:12.246Z log (object:
+LifecycleDockerAdapterSequence) Starting PreRunner { image: 'scramjetorg/pre-
+runner:0.12.2', maxMem: 128 } 2021-11-19T16:05:13.536Z log (object:
+DockerodeDockerHelper) Checking image scramjetorg/runner:0.12.2 2021-11-19T16:
 05:16.670Z info (object:SequenceStore) New sequence added: c50fe4d3-89cc-4685-
-a82a-16cbc744733d\n2021-11-19T16:05:16.672Z info (object:Host) Sequence
-identified: {\n container: {\n image: \'scramjetorg/runner:0.12.2\',\n maxMem:
-512,\n exposePortsRange: [ 30000, 32767 ],\n hostIp: \'0.0.0.0\'\n },\n name:
-\'@scramjet/multi-outputs\',\n version: \'0.12.2\',\n engines: {},\n config:
-{},\n sequencePath: \'index.js\',\n packageVolumeId: \'c50fe4d3-89cc-4685-a82a-
-16cbc744733d\'\n}\n2021-11-19T16:05:16.691Z debug (object:Host) Request date:
-2021-11-19T16:05:08.239Z, method: POST, url: /api/v1/sequence, status:
-202\n```\n\n\n\n___\n\n### Sequence operations\n\n\n\n [ POST ] /api/v1/
-sequence - add new sequence\n\n\n
-Parameters\n\n| Name | Type | Description | Required |\n| ----------- | -------
-- | ----------------------------------- | -------- |\n| `file` | `binary` |
-compressed package in tar.gz format | yes |\n| `appConfig` | `json` |
-additional package.json config file | no |\n\nResponses\n\nAccepted operation
-code: `202`\n\n```json\n{\n "id": "2c3068e5-7c74-45bb-a017-1979c41fc6d0" /
-/ sequence id\n}\n```\n\n\n\n\n\n [ GET ] /api/v1/sequences - show list of
-sequences\n\n\n
-Parameters\n\nNo parameters\n\nResponses\n\nSuccessful operation code:
-`200`\n\n```json\n[\n {\n "instances": [\n "742d2713-7ab6-4cde-82f3-
-a7beabdd4e98" // list of sequence instances\n ],\n "id": "bdef63db-d3a0-45c8-
-85db-e94ebb96097f", // sequence id\n "config": {\n "container": {\n "image":
-"scramjetorg/runner:0.12.2",\n "maxMem": 512\n },\n "name": "@scramjet/
-transform-hub",\n "version": "0.12.2",\n "engines": {},\n "config": {},\n
-"sequencePath": "index.js",\n "packageVolumeId": "bdef63db-d3a0-45c8-85db-
-e94ebb96097f"\n }\n }\n]\n```\n\n\n\n\n\n [ POST ] /api/v1/sequence/:id/start -
-start chosen sequence\n\n\n
-Parameters\n\n| Name | Type | Description | Required |\n| ----------- | -----
-- | ----------------------------------------------------- | -------- |\n|
-`appConfig` | `json` | additional package.json config file | no |\n| `args` |
-`json` | additional arguments that instance should starts with | no
-|\n\nResponses\n\nSuccessful operation code: `200`\n\n```json\n{\n "id":
-"681c856e-dfa4-46a1-951d-47b27345552e"\n}\n```\n\n\n\n\n\n [ DELETE ] /api/v1/
-sequence/:id - delete a sequence by id\n\n\n
-Parameters\n\nNo parameters\n\nResponses\n\nSuccessful operation code:
-`200`\n\n```json\n{\n "id": "2c3068e5-7c74-45bb-a017-
-1979c41fc6d0"\n}\n```\n\nConflict operation code: `409` - the instance is still
-running\n\n```json\n{\n "error": "Can\'t remove sequence in
-use."\n}\n```\n\n\n\n___\n\n### Instance basic operations\n\n\n\n [ GET ] /api/
-v1/instances - list all instances\n\n\n
-Parameters\n\nNo parameters\n\nResponses\n\nSuccessful operation code:
-`200`\n\n```json\n[\n {\n "id": "742d2713-7ab6-4cde-82f3-a7beabdd4e98",\n
-"sequence": "bdef63db-d3a0-45c8-85db-e94ebb96097f"\n },\n {\n "id": "681c856e-
-dfa4-46a1-951d-47b27345552e",\n "sequence": "bdef63db-d3a0-45c8-85db-
-e94ebb96097f"\n },\n {\n "id": "21f787ed-6b9e-4e9f-828e-afe428d84833",\n
-"sequence": "bdef63db-d3a0-45c8-85db-e94ebb96097f"\n }\n]\n```\n\n\n\n\n\n
-[ GET ] /api/v1/instance/:id - show data of chosen instance\n\n\n
-Parameters\n\nNo parameters\n\nResponses\n\n| Name | Code | Description |\n| :-
------------------- | :---- | :------------------------------------------ |\n|
-Successful operation | `200` | Returns JSON data |\n| Not Found operation |
-`404` | For example if instance was already stopped |\n\n```json\n{\n
-"created": "2021-10-29T16:08:36.524Z",\n "started": "2021-10-29T16:08:
-38.701Z",\n "sequenceId": "b0c02fdc-b05f-4f26-9d68-
-43a702eb7b44"\n}\n```\n\n\n\n\n\n [ POST ] /api/v1/instance/:id/_stop - end
-instance gracefully and prolong operations or not for task
-completion\u200b\n\n\n
-Parameters\n\n| Name | Type | Description | Required |\n| ------------------ |
---------- | -------------------------------------------------------------------
------------- | -------- |\n| `timeout` | `number` | The number of milliseconds
-before the Instance will be killed. Default: 7000ms. | no |\n|
+a82a-16cbc744733d 2021-11-19T16:05:16.672Z info (object:Host) Sequence
+identified: { container: { image: 'scramjetorg/runner:0.12.2', maxMem: 512,
+exposePortsRange: [ 30000, 32767 ], hostIp: '0.0.0.0' }, name: '@scramjet/
+multi-outputs', version: '0.12.2', engines: {}, config: {}, sequencePath:
+'index.js', packageVolumeId: 'c50fe4d3-89cc-4685-a82a-16cbc744733d' } 2021-11-
+19T16:05:16.691Z debug (object:Host) Request date: 2021-11-19T16:05:08.239Z,
+method: POST, url: /api/v1/sequence, status: 202 ```  ___ ### Sequence
+operations   [ POST ] /api/v1/sequence - add new sequence
+Parameters | Name | Type | Description | Required | | ----------- | -------- |
+----------------------------------- | -------- | | `file` | `binary` |
+compressed package in tar.gz format | yes | | `appConfig` | `json` | additional
+package.json config file | no | Responses Accepted operation code: `202`
+```json { "id": "2c3068e5-7c74-45bb-a017-1979c41fc6d0" // sequence id } ```
+[ GET ] /api/v1/sequences - show list of sequences
+Parameters No parameters Responses Successful operation code: `200` ```json [
+{ "instances": [ "742d2713-7ab6-4cde-82f3-a7beabdd4e98" // list of sequence
+instances ], "id": "bdef63db-d3a0-45c8-85db-e94ebb96097f", // sequence id
+"config": { "container": { "image": "scramjetorg/runner:0.12.2", "maxMem": 512
+}, "name": "@scramjet/transform-hub", "version": "0.12.2", "engines": {},
+"config": {}, "sequencePath": "index.js", "packageVolumeId": "bdef63db-d3a0-
+45c8-85db-e94ebb96097f" } } ] ```    [ POST ] /api/v1/sequence/:id/start -
+start chosen sequence
+Parameters | Name | Type | Description | Required | | ----------- | ------ | --
+--------------------------------------------------- | -------- | | `appConfig`
+| `json` | additional package.json config file | no | | `args` | `json` |
+additional arguments that instance should starts with | no | Responses
+Successful operation code: `200` ```json { "id": "681c856e-dfa4-46a1-951d-
+47b27345552e" } ```    [ DELETE ] /api/v1/sequence/:id - delete a sequence by
+id
+Parameters No parameters Responses Successful operation code: `200` ```json
+{ "id": "2c3068e5-7c74-45bb-a017-1979c41fc6d0" } ``` Conflict operation code:
+`409` - the instance is still running ```json { "error": "Can't remove sequence
+in use." } ```  ___ ### Instance basic operations   [ GET ] /api/v1/instances -
+list all instances
+Parameters No parameters Responses Successful operation code: `200` ```json [
+{ "id": "742d2713-7ab6-4cde-82f3-a7beabdd4e98", "sequence": "bdef63db-d3a0-
+45c8-85db-e94ebb96097f" }, { "id": "681c856e-dfa4-46a1-951d-47b27345552e",
+"sequence": "bdef63db-d3a0-45c8-85db-e94ebb96097f" }, { "id": "21f787ed-6b9e-
+4e9f-828e-afe428d84833", "sequence": "bdef63db-d3a0-45c8-85db-e94ebb96097f" } ]
+```    [ GET ] /api/v1/instance/:id - show data of chosen instance
+Parameters No parameters Responses | Name | Code | Description | | :-----------
+-------- | :---- | :------------------------------------------ | | Successful
+operation | `200` | Returns JSON data | | Not Found operation | `404` | For
+example if instance was already stopped | ```json { "created": "2021-10-29T16:
+08:36.524Z", "started": "2021-10-29T16:08:38.701Z", "sequenceId": "b0c02fdc-
+b05f-4f26-9d68-43a702eb7b44" } ```    [ POST ] /api/v1/instance/:id/_stop - end
+instance gracefully and prolong operations or not for task completionâ
+Parameters | Name | Type | Description | Required | | ------------------ | ----
+----- | -----------------------------------------------------------------------
+-------- | -------- | | `timeout` | `number` | The number of milliseconds
+before the Instance will be killed. Default: 7000ms. | no | |
 `canCallKeepalive` | `boolean` | If set to true, the instance will prolong the
-running. Default: false. | no |\n\nResponses\n\nSuccessful operation code:
-`200`\n\n```json\n{\n "code": 0,\n "type": "string",\n "message":
-"string"\n}\n```\n\n\n\n\n\n [ POST ] api/v1/instance/:id/_kill - end instance
-gracefully waiting for unfinished tasks\n\n\n
-Parameters\n\nNo parameters\n\nResponses\n\nAccepted operation code:
-`202`\n\n```text\nNo body returned\n```\n\n\n\n\n\n [ GET ] /api/v1/instance/:
-id/health - check status about instance health\n\n\n
-Parameters\n\nNo parameters\n\nResponses\n\nSuccessful operation code:
-`200`\n\n```json\n{\n "cpuTotalUsage": 529325247,\n "healthy": true,\n "limit":
-536870912,\n "memoryMaxUsage": 16117760,\n "memoryUsage": 14155776,\n
-"networkRx": 1086,\n "networkTx": 0,\n "containerId":
-"1c993c4ff774fac06185aa9554cf40c23b03e1479a7e0d14827708161b08ae51"\n}\n```\n\n\n\n___\n\n###
-Instance advanced operation\n\n\n\n [ POST ] /api/v1/instance/:id/_event - send
-event to the Instance\n\n\n
-Parameters\n\n| Name | Type | Description | Required |\n| :---------- | :------
-- | ---------------------------- | -------- |\n| `eventName` | `string` | Name
-of an event | true |\n| `message` | `string` | JSON formatted event payload |
-false |\n\nResponses\n\nContent-type: `application/octet-stream`\n\n\n\n\n\n
-[ GET ] /api/v1/instance/:id/event - get the data stream with the events from
-the Instance\n\n\n
-Parameters\n\nNo parameters\n\nResponses\n\nContent-type: `application/octet-
-stream`\n\n\n\n\n\n [ GET ] /api/v1/instance/:id/once - get the last event sent
-by the Instance\n\n\n
-Parameters\n\nNo parameters\n\nResponses\n\nContent-type: `application/octet-
-stream`\n\n\n\n\n\n [ POST ] /api/v1/instance/:id/input - send data to the
-input stream of the Instance to consume it\n\n\n
-Parameters\n\nNo parameters\n\nResponses\n\n| Name | Code | Description |\n| :-
----------------------- | :---- | :---------------------------------------------
--------------- |\n| Successful operation | `200` | - |\n| Not Acceptable
-operation | `406` | Instance expects the input to be provided from the Topic
-API |\n\n\n\n\n\n [ GET ] /api/v1/instance/:id/output - get stream data from an
-instance and consume it through the endpoint\n\n\n
-Parameters\n\nNo parameters\n\nResponses\n\nContent-type: `application/octet-
-stream`\n\n\n\n\n\n [ POST ] /api/v1/instance/:id/stdin\u200b -
-process.stdin\n\n\n
-Parameters\n\nNo parameters\n\nResponses\n\nSuccessful operation code:
-`200`\n\n\n\n\n\n [ GET ] /api/v1/instance/:id/stdout - process.stdout\n\n\n
-Parameters\n\nNo parameters\n\nResponses\n\nContent-type: `application/octet-
-stream`\n\n\n\n\n\n [ GET ] /api/v1/instance/:id/stderr - process.stderr\n\n\n
-Parameters\n\nNo parameters\n\nResponses\n\nContent-type: `application/octet-
-stream`\n\n\n\n\n\n [ GET ] /api/v1/instance/:id/log - stream all instance
-logs\n\n\n
-Parameters\n\nNo parameters\n\nResponses\n\nContent-type: `application/octet-
-stream`\n\nSuccessful operation code: `200`\n\n```bash\n2021-11-19T16:12:
-22.948Z log (Sequence) 42\n2021-11-19T16:12:23.949Z log (Sequence) 41\n2021-11-
-19T16:12:24.950Z log (Sequence) 40\n2021-11-19T16:12:25.951Z log (Sequence)
-39\n2021-11-19T16:12:26.952Z log (Sequence) 38\n2021-11-19T16:12:27.952Z log
-(Sequence) 37\n2021-11-19T16:12:28.953Z log (Sequence) 36\n2021-11-19T16:12:
-29.953Z log (Sequence) 35\n```\n\n\n\n___\n\n### Service Discovery:
-Topics\n\nIf a given topic does not exist, Transform-Hub creates it and stores
-the sent data in the newly created topic. The data is stored in the topic until
-the data is not consumed (either by the Topic API or by the Instances
-subscribing to this topic). When the data are sent to the topic they are
-written to the returned stream.\n\n\n\n [ POST ] /api/v1/topics/:name\u200b -
-sends data to the topic\n\n\n
-Parameters\n\nNo parameters\n\nRequest Headers\n\n| Header | Type | Description
-| Default | Required |\n| -------------- | --------------------- | ------------
------------------------------------------------------------ | -----------------
------ | -------- |\n| `x-end-stream` | `boolean` | If set to `true`, then close
-topic stream after processing the request. | false | no |\n| `content-type` |
+running. Default: false. | no | Responses Successful operation code: `200`
+```json { "code": 0, "type": "string", "message": "string" } ```    [ POST ]
+api/v1/instance/:id/_kill - end instance gracefully waiting for unfinished
+tasks
+Parameters No parameters Responses Accepted operation code: `202` ```text No
+body returned ```    [ GET ] /api/v1/instance/:id/health - check status about
+instance health
+Parameters No parameters Responses Successful operation code: `200` ```json
+{ "cpuTotalUsage": 529325247, "healthy": true, "limit": 536870912,
+"memoryMaxUsage": 16117760, "memoryUsage": 14155776, "networkRx": 1086,
+"networkTx": 0, "containerId":
+"1c993c4ff774fac06185aa9554cf40c23b03e1479a7e0d14827708161b08ae51" } ```  ___
+### Instance advanced operation   [ POST ] /api/v1/instance/:id/_event - send
+event to the Instance
+Parameters | Name | Type | Description | Required | | :---------- | :------- |
+---------------------------- | -------- | | `eventName` | `string` | Name of an
+event | true | | `message` | `string` | JSON formatted event payload | false |
+Responses Content-type: `application/octet-stream`    [ GET ] /api/v1/
+instance/:id/event - get the data stream with the events from the Instance
+Parameters No parameters Responses Content-type: `application/octet-stream`
+[ GET ] /api/v1/instance/:id/once - get the last event sent by the Instance
+Parameters No parameters Responses Content-type: `application/octet-stream`
+[ POST ] /api/v1/instance/:id/input - send data to the input stream of the
+Instance to consume it
+Parameters No parameters Responses | Name | Code | Description | | :-----------
+------------ | :---- | :-------------------------------------------------------
+---- | | Successful operation | `200` | - | | Not Acceptable operation | `406`
+| Instance expects the input to be provided from the Topic API |    [ GET ] /
+api/v1/instance/:id/output - get stream data from an instance and consume it
+through the endpoint
+Parameters No parameters Responses Content-type: `application/octet-stream`
+[ POST ] /api/v1/instance/:id/stdinâ - process.stdin
+Parameters No parameters Responses Successful operation code: `200`    [ GET ]
+/api/v1/instance/:id/stdout - process.stdout
+Parameters No parameters Responses Content-type: `application/octet-stream`
+[ GET ] /api/v1/instance/:id/stderr - process.stderr
+Parameters No parameters Responses Content-type: `application/octet-stream`
+[ GET ] /api/v1/instance/:id/log - stream all instance logs
+Parameters No parameters Responses Content-type: `application/octet-stream`
+Successful operation code: `200` ```bash 2021-11-19T16:12:22.948Z log
+(Sequence) 42 2021-11-19T16:12:23.949Z log (Sequence) 41 2021-11-19T16:12:
+24.950Z log (Sequence) 40 2021-11-19T16:12:25.951Z log (Sequence) 39 2021-11-
+19T16:12:26.952Z log (Sequence) 38 2021-11-19T16:12:27.952Z log (Sequence) 37
+2021-11-19T16:12:28.953Z log (Sequence) 36 2021-11-19T16:12:29.953Z log
+(Sequence) 35 ```  ___ ### Service Discovery: Topics If a given topic does not
+exist, Transform-Hub creates it and stores the sent data in the newly created
+topic. The data is stored in the topic until the data is not consumed (either
+by the Topic API or by the Instances subscribing to this topic). When the data
+are sent to the topic they are written to the returned stream.   [ POST ] /api/
+v1/topics/:nameâ - sends data to the topic
+Parameters No parameters Request Headers | Header | Type | Description |
+Default | Required | | -------------- | --------------------- | ---------------
+-------------------------------------------------------- | --------------------
+-- | -------- | | `x-end-stream` | `boolean` | If set to `true`, then close
+topic stream after processing the request. | false | no | | `content-type` |
 `text`, `application` | Specifies data type of this topic | `application/x-
-ndjson` | no |\n\nSupported types: `text/x-ndjson`, `application/x-ndjson`,
-`application/x-ndjson`, `text/plain`, `application/octet-
-stream`\n\nResponses\n\n| Name | Code | Description |\n| :------------------- |
-:---- | :-------------------------------------------------------------------
-- |\n| Successful operation | `200` | data was sent with the header indicating
-the end of data |\n| Successful operation | `202` | data was sent without the
-header indicating the end of data (default) |\n\n\n\n\n\n [ GET ] /api/v1/
-topics/:name\u200b - get data from the topic\n\n\n
-Parameters\n\nNo parameters\n\nResponses\n\nTopic data stream.\n\nSuccessful
-operation code: `200`\n\n```json\n{\n "source": "Twitter",\n "id":
-"850006245121695778",\n "content": "Natural wetlands make up ~30% of global
-total CH4 emissions",\n "user": {\n "id": 1234994945,\n "name": "Climate Change
-Conference",\n "screen_name": "Climate Change",\n }\n}\n```\n\n\n\n___\n\n##
-Some important links\n\n* Scramjet, the company behind [Transform Hub](https://
-scramjet.org)\n* The [Scramjet Framework - functional reactive stream
-processing framework](https://framework.scramjet.org)\n* The [Transform Hub
-repo on github](https://github.com/scramjetorg/transform-hub)\n* You can see
-the [Scramjet Transform Hub API docs here](https://github.com/scramjetorg/
-transform-hub/tree/HEAD/docs/api-client/README.md)\n* You can see the [CLI
-documentation here](https://github.com/scramjetorg/transform-hub/tree/HEAD/
-packages/cli/README.md), but `si help` should also be quite effective.\n*
-Don\'t forget to â­ this repo if you like it, `subscribe` to releases and keep
-visiting us for new versions and updates.\n* You can [open an issue - file a
-bug report or a feature request here](https://github.com/scramjetorg/transform-
-hub/issues/new/choose)\n\n## License and contributions\n\nThis module is
-licensed under AGPL-3.0 license.\n\nThe Scramjet Transform Hub project is dual-
-licensed under the AGPL-3.0 and MIT licenses. Parts of the project that are
-linked with your programs are MIT licensed, the rest is AGPL.\n\n##
-Contributions\n\nWe accept valid contributions and we will be publishing a more
-specific project roadmap so contributors can propose features and also help us
-implement them. We kindly ask you that contributed commits are Signed-Off `git
-commit --sign-off`.\n\nWe provide support for contributors via test cases. If
-you expect a certain type of workflow to be officially supported, please
-specify and implement a test case in `Gherkin` format in `bdd` directory and
-include it in your pull request. More info about our BDD test you will find
-[here](https://github.com/scramjetorg/transform-hub/tree/HEAD/bdd/
-README.md).\n\n### Help wanted ð©\u200dðð§ð±\u200dâï¸\n\nThe
-project need\'s your help! There\'s lots of work to do and we have a lot of
+ndjson` | no | Supported types: `text/x-ndjson`, `application/x-ndjson`,
+`application/x-ndjson`, `text/plain`, `application/octet-stream` Responses |
+Name | Code | Description | | :------------------- | :---- | :-----------------
+--------------------------------------------------- | | Successful operation |
+`200` | data was sent with the header indicating the end of data | | Successful
+operation | `202` | data was sent without the header indicating the end of data
+(default) |    [ GET ] /api/v1/topics/:nameâ - get data from the topic
+Parameters No parameters Responses Topic data stream. Successful operation
+code: `200` ```json { "source": "Twitter", "id": "850006245121695778",
+"content": "Natural wetlands make up ~30% of global total CH4 emissions",
+"user": { "id": 1234994945, "name": "Climate Change Conference", "screen_name":
+"Climate Change", } } ```  ___ ## Some important links * Scramjet, the company
+behind [Transform Hub](https://scramjet.org) * The [Scramjet Framework -
+functional reactive stream processing framework](https://
+framework.scramjet.org) * The [Transform Hub repo on github](https://
+github.com/scramjetorg/transform-hub) * You can see the [Scramjet Transform Hub
+API docs here](https://github.com/scramjetorg/transform-hub/tree/HEAD/docs/api-
+client/README.md) * You can see the [CLI documentation here](https://
+github.com/scramjetorg/transform-hub/tree/HEAD/packages/cli/README.md), but `si
+help` should also be quite effective. * Don't forget to â­ this repo if you
+like it, `subscribe` to releases and keep visiting us for new versions and
+updates. * You can [open an issue - file a bug report or a feature request
+here](https://github.com/scramjetorg/transform-hub/issues/new/choose) ##
+License and contributions This module is licensed under AGPL-3.0 license. The
+Scramjet Transform Hub project is dual-licensed under the AGPL-3.0 and MIT
+licenses. Parts of the project that are linked with your programs are MIT
+licensed, the rest is AGPL. ## Contributions We accept valid contributions and
+we will be publishing a more specific project roadmap so contributors can
+propose features and also help us implement them. We kindly ask you that
+contributed commits are Signed-Off `git commit --sign-off`. We provide support
+for contributors via test cases. If you expect a certain type of workflow to be
+officially supported, please specify and implement a test case in `Gherkin`
+format in `bdd` directory and include it in your pull request. More info about
+our BDD test you will find [here](https://github.com/scramjetorg/transform-hub/
+tree/HEAD/bdd/README.md). ### Help wanted ð©âðð§ð±ââï¸ The
+project need's your help! There's lots of work to do and we have a lot of
 plans. If you want to help and be part of the Scramjet team, please reach out
 to us, [on discord](https://scr.je/join-community-mg1) or email us:
-[opensource@scramjet.org](mailto:opensource@scramjet.org).\n\n### Donation
-ð¸\n\nDo you like this project? It helped you to reduce time spent on
-delivering your solution? You are welcome to buy us a coffee â Thanks a lot!
-ð\n\n[You can sponsor us on github](https://github.com/sponsors/
-scramjetorg)\n\n* There\'s also a Paypal donation link if you prefer that:\n\n
-[![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)]
-(https://www.paypal.com/cgi-bin/webscr?cmd=_s-
-xclick&hosted_button_id=7F7V65C43EBMW)\n\n\n\n', 'author': 'Scramjet',
-'author_email': 'open-source@scramjet.org', 'maintainer': 'None',
-'maintainer_email': 'None', 'url': 'None', 'packages': packages,
-'package_data': package_data, 'install_requires': install_requires,
-'python_requires': '>=3.9,<4.0', } setup(**setup_kwargs)
+[opensource@scramjet.org](mailto:opensource@scramjet.org). ### Donation ð¸ Do
+you like this project? It helped you to reduce time spent on delivering your
+solution? You are welcome to buy us a coffee â Thanks a lot! ð [You can
+sponsor us on github](https://github.com/sponsors/scramjetorg) * There's also a
+Paypal donation link if you prefer that: [![paypal](https://
+www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/
+cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=7F7V65C43EBMW)
```

### Comparing `scramjet_client_utils-1.0.1/PKG-INFO` & `scramjet-client-utils-1.1.0/scramjet_client_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,40 @@
 Metadata-Version: 2.1
 Name: scramjet-client-utils
-Version: 1.0.1
-Summary: 
+Version: 1.1.0
+Home-page: https://github.com/scramjetorg/api-client-python/tree/main/client_utils
 Author: Scramjet
 Author-email: open-source@scramjet.org
 Requires-Python: >=3.9,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
-Requires-Dist: url_normalize (>=1.4.3,<2.0.0)
 Description-Content-Type: text/markdown
 
 <h1 align="center"><strong>Scramjet Transform Hub API Clients utility</strong></h1>
 
 The package provides utilities for API clients. Each of the API clients make use out of it.
 
 Usage:
 
 ```python
 import asyncio
-import json
 from client.host_client import HostClient
-from client_utils import ClientUtils
+from client_utils.base_client import BaseClient
 
 # your middleware token
 token = ''
 # set the token
-ClientUtils.setDefaultHeaders({'Authorization': f'Bearer {token}'})
+BaseClient.setDefaultHeaders({'Authorization': f'Bearer {token}'})
 
 # middleware url
 api_base ='https://api.scramjet.cloud/api/v1' 
 
-# url = {middlewareURL}/space/{manager_id}/api/v1/{host_id}/api/v1
+# url = {middlewareURL}/space/{manager_id}/api/v1/sth/{host_id}/api/v1
 host = HostClient(f'{api_base}/space/org-aa5bu150-9o5c-489b-83e3-b1yf7e086f3h-manager/api/v1/sth-1/api/v1')
 # get a list of Sequences
 res = asyncio.run(host.list_sequences())
-# convert responose to json
-sequences = json.loads(res)
+print(res)
 ```
 
 ---
 ## More reading
 <p align="center">
     <a href="https://github.com/scramjetorg/transform-hub/blob/HEAD/LICENSE"><img src="https://img.shields.io/github/license/scramjetorg/transform-hub?color=green&style=plastic" alt="GitHub license" /></a>
     <a href="https://npmjs.org/package/@scramjet/sth"><img src="https://img.shields.io/github/v/tag/scramjetorg/transform-hub?label=version&color=blue&style=plastic" alt="STH version" /></a>
@@ -791,8 +783,7 @@
 
 * There's also a Paypal donation link if you prefer that:
 
 [![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=7F7V65C43EBMW)
 
 
 
-
```

#### html2text {}

```diff
@@ -1,25 +1,21 @@
-Metadata-Version: 2.1 Name: scramjet-client-utils Version: 1.0.1 Summary:
-Author: Scramjet Author-email: open-source@scramjet.org Requires-Python:
->=3.9,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
-Dist: aiohttp (>=3.8.3,<4.0.0) Requires-Dist: url_normalize (>=1.4.3,<2.0.0)
+Metadata-Version: 2.1 Name: scramjet-client-utils Version: 1.1.0 Home-page:
+https://github.com/scramjetorg/api-client-python/tree/main/client_utils Author:
+Scramjet Author-email: open-source@scramjet.org Requires-Python: >=3.9,<4.0
 Description-Content-Type: text/markdown
            ****** Scramjet Transform Hub API Clients utility ******
 The package provides utilities for API clients. Each of the API clients make
-use out of it. Usage: ```python import asyncio import json from
-client.host_client import HostClient from client_utils import ClientUtils #
-your middleware token token = '' # set the token ClientUtils.setDefaultHeaders(
-{'Authorization': f'Bearer {token}'}) # middleware url api_base ='https://
-api.scramjet.cloud/api/v1' # url = {middlewareURL}/space/{manager_id}/api/v1/
-{host_id}/api/v1 host = HostClient(f'{api_base}/space/org-aa5bu150-9o5c-489b-
-83e3-b1yf7e086f3h-manager/api/v1/sth-1/api/v1') # get a list of Sequences res =
-asyncio.run(host.list_sequences()) # convert responose to json sequences =
-json.loads(res) ``` --- ## More reading
+use out of it. Usage: ```python import asyncio from client.host_client import
+HostClient from client_utils.base_client import BaseClient # your middleware
+token token = '' # set the token BaseClient.setDefaultHeaders({'Authorization':
+f'Bearer {token}'}) # middleware url api_base ='https://api.scramjet.cloud/api/
+v1' # url = {middlewareURL}/space/{manager_id}/api/v1/sth/{host_id}/api/v1 host
+= HostClient(f'{api_base}/space/org-aa5bu150-9o5c-489b-83e3-b1yf7e086f3h-
+manager/api/v1/sth-1/api/v1') # get a list of Sequences res = asyncio.run
+(host.list_sequences()) print(res) ``` --- ## More reading
     [GitHub_license] [STH_version] [GitHub_stars] [npm] [Discord] [Donate]
              â­ Star us on GitHub â it motivates us a lot! ð
                          [Scramjet Transform Hub Logo]
 In the link below you will find more information about our stream protocol and
 API usage. See the code documentation here: [scramjetorg/transform-hub/docs/
 read-more/stream-and-api.md](https://github.com/scramjetorg/transform-hub/tree/
 HEAD/docs/read-more/stream-and-api.md) ## Scramjet Transform Hub This package
```

