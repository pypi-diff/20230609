# Comparing `tmp/datalad_osf-0.2.3.1.tar.gz` & `tmp/datalad_osf-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datalad_osf-0.2.3.1.tar", last modified: Tue Mar  2 08:20:28 2021, max compression
+gzip compressed data, was "datalad_osf-0.3.0.tar", last modified: Fri Jun  9 09:45:33 2023, max compression
```

## Comparing `datalad_osf-0.2.3.1.tar` & `datalad_osf-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2021-03-02 08:20:28.845440 datalad_osf-0.2.3.1/
--rw-rw-r--   0 mih       (1000) mih       (1000)       92 2020-06-17 18:11:34.000000 datalad_osf-0.2.3.1/MANIFEST.in
--rw-rw-r--   0 mih       (1000) mih       (1000)     9431 2021-03-02 08:20:28.845440 datalad_osf-0.2.3.1/PKG-INFO
--rw-rw-r--   0 mih       (1000) mih       (1000)     8342 2021-02-10 14:30:29.000000 datalad_osf-0.2.3.1/README.md
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2021-03-02 08:20:28.845440 datalad_osf-0.2.3.1/datalad_osf/
--rw-rw-r--   0 mih       (1000) mih       (1000)     1543 2020-06-27 11:21:22.000000 datalad_osf-0.2.3.1/datalad_osf/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      499 2021-03-02 08:20:28.845440 datalad_osf-0.2.3.1/datalad_osf/_version.py
--rwxrwxr-x   0 mih       (1000) mih       (1000)    11160 2021-02-10 14:24:36.000000 datalad_osf-0.2.3.1/datalad_osf/annex_remote.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    13844 2021-02-10 14:24:36.000000 datalad_osf-0.2.3.1/datalad_osf/create_sibling_osf.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     4356 2021-02-10 14:24:36.000000 datalad_osf-0.2.3.1/datalad_osf/credentials.py
--rwxrwxr-x   0 mih       (1000) mih       (1000)    17921 2021-02-10 14:24:36.000000 datalad_osf-0.2.3.1/datalad_osf/git_remote.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2021-03-02 08:20:28.845440 datalad_osf-0.2.3.1/datalad_osf/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)      393 2020-06-20 10:47:58.000000 datalad_osf-0.2.3.1/datalad_osf/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     3863 2021-02-10 14:24:36.000000 datalad_osf-0.2.3.1/datalad_osf/tests/test_create_sibling_osf.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2982 2021-02-01 19:06:08.000000 datalad_osf-0.2.3.1/datalad_osf/tests/test_public.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      491 2020-06-20 10:47:58.000000 datalad_osf-0.2.3.1/datalad_osf/tests/test_register.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1895 2021-02-01 19:06:08.000000 datalad_osf-0.2.3.1/datalad_osf/tests/test_remote.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1224 2021-02-10 14:24:36.000000 datalad_osf-0.2.3.1/datalad_osf/tests/utils.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     6046 2021-02-01 19:06:08.000000 datalad_osf-0.2.3.1/datalad_osf/utils.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2021-03-02 08:20:28.841440 datalad_osf-0.2.3.1/datalad_osf.egg-info/
--rw-rw-r--   0 mih       (1000) mih       (1000)     9431 2021-03-02 08:20:28.000000 datalad_osf-0.2.3.1/datalad_osf.egg-info/PKG-INFO
--rw-rw-r--   0 mih       (1000) mih       (1000)      668 2021-03-02 08:20:28.000000 datalad_osf-0.2.3.1/datalad_osf.egg-info/SOURCES.txt
--rw-rw-r--   0 mih       (1000) mih       (1000)        1 2021-03-02 08:20:28.000000 datalad_osf-0.2.3.1/datalad_osf.egg-info/dependency_links.txt
--rw-rw-r--   0 mih       (1000) mih       (1000)      171 2021-03-02 08:20:28.000000 datalad_osf-0.2.3.1/datalad_osf.egg-info/entry_points.txt
--rw-rw-r--   0 mih       (1000) mih       (1000)       75 2021-03-02 08:20:28.000000 datalad_osf-0.2.3.1/datalad_osf.egg-info/requires.txt
--rw-rw-r--   0 mih       (1000) mih       (1000)       12 2021-03-02 08:20:28.000000 datalad_osf-0.2.3.1/datalad_osf.egg-info/top_level.txt
--rw-rw-r--   0 mih       (1000) mih       (1000)       60 2020-06-16 11:35:01.000000 datalad_osf-0.2.3.1/pyproject.toml
--rw-rw-r--   0 mih       (1000) mih       (1000)     1025 2021-03-02 08:20:28.845440 datalad_osf-0.2.3.1/setup.cfg
--rwxrwxr-x   0 mih       (1000) mih       (1000)     1778 2020-07-15 06:19:37.000000 datalad_osf-0.2.3.1/setup.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    68611 2020-06-16 11:35:01.000000 datalad_osf-0.2.3.1/versioneer.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 09:45:33.720361 datalad_osf-0.3.0/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3215 2023-06-09 09:45:29.000000 datalad_osf-0.3.0/LICENSE
+-rw-rw-r--   0 mih       (1000) mih       (1000)       92 2023-06-09 09:45:29.000000 datalad_osf-0.3.0/MANIFEST.in
+-rw-rw-r--   0 mih       (1000) mih       (1000)     9449 2023-06-09 09:45:33.720361 datalad_osf-0.3.0/PKG-INFO
+-rw-rw-r--   0 mih       (1000) mih       (1000)     8915 2023-06-09 09:45:29.000000 datalad_osf-0.3.0/README.md
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 09:45:33.720361 datalad_osf-0.3.0/datalad_osf/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1451 2023-06-09 09:45:29.000000 datalad_osf-0.3.0/datalad_osf/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      497 2023-06-09 09:45:33.720361 datalad_osf-0.3.0/datalad_osf/_version.py
+-rwxrwxr-x   0 mih       (1000) mih       (1000)    11435 2023-06-09 09:45:29.000000 datalad_osf-0.3.0/datalad_osf/annex_remote.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      637 2023-06-09 09:45:29.000000 datalad_osf-0.3.0/datalad_osf/conftest.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    13865 2023-06-09 09:45:29.000000 datalad_osf-0.3.0/datalad_osf/create_sibling_osf.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     4355 2023-06-09 09:45:29.000000 datalad_osf-0.3.0/datalad_osf/credentials.py
+-rwxrwxr-x   0 mih       (1000) mih       (1000)     2257 2023-06-09 09:45:29.000000 datalad_osf-0.3.0/datalad_osf/git_remote.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 09:45:33.720361 datalad_osf-0.3.0/datalad_osf/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      393 2023-06-09 09:45:29.000000 datalad_osf-0.3.0/datalad_osf/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1264 2023-06-09 09:45:29.000000 datalad_osf-0.3.0/datalad_osf/tests/fixtures.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3139 2023-06-09 09:45:29.000000 datalad_osf-0.3.0/datalad_osf/tests/test_create_sibling_osf.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3431 2023-06-09 09:45:29.000000 datalad_osf-0.3.0/datalad_osf/tests/test_public.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      490 2023-06-09 09:45:29.000000 datalad_osf-0.3.0/datalad_osf/tests/test_register.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1309 2023-06-09 09:45:29.000000 datalad_osf-0.3.0/datalad_osf/tests/test_remote.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1224 2023-06-09 09:45:29.000000 datalad_osf-0.3.0/datalad_osf/tests/utils.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     6046 2023-06-09 09:45:29.000000 datalad_osf-0.3.0/datalad_osf/utils.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 09:45:33.720361 datalad_osf-0.3.0/datalad_osf.egg-info/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     9449 2023-06-09 09:45:33.000000 datalad_osf-0.3.0/datalad_osf.egg-info/PKG-INFO
+-rw-rw-r--   0 mih       (1000) mih       (1000)      730 2023-06-09 09:45:33.000000 datalad_osf-0.3.0/datalad_osf.egg-info/SOURCES.txt
+-rw-rw-r--   0 mih       (1000) mih       (1000)        1 2023-06-09 09:45:33.000000 datalad_osf-0.3.0/datalad_osf.egg-info/dependency_links.txt
+-rw-rw-r--   0 mih       (1000) mih       (1000)      170 2023-06-09 09:45:33.000000 datalad_osf-0.3.0/datalad_osf.egg-info/entry_points.txt
+-rw-rw-r--   0 mih       (1000) mih       (1000)      110 2023-06-09 09:45:33.000000 datalad_osf-0.3.0/datalad_osf.egg-info/requires.txt
+-rw-rw-r--   0 mih       (1000) mih       (1000)       12 2023-06-09 09:45:33.000000 datalad_osf-0.3.0/datalad_osf.egg-info/top_level.txt
+-rw-rw-r--   0 mih       (1000) mih       (1000)       60 2023-06-09 09:45:29.000000 datalad_osf-0.3.0/pyproject.toml
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1031 2023-06-09 09:45:33.720361 datalad_osf-0.3.0/setup.cfg
+-rwxrwxr-x   0 mih       (1000) mih       (1000)     1778 2023-06-09 09:45:29.000000 datalad_osf-0.3.0/setup.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    83607 2023-06-09 09:45:29.000000 datalad_osf-0.3.0/versioneer.py
```

### Comparing `datalad_osf-0.2.3.1/PKG-INFO` & `datalad_osf-0.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,84 +1,76 @@
-Metadata-Version: 2.1
-Name: datalad_osf
-Version: 0.2.3.1
-Summary: DataLad extension to interface with the Open Science Framework (OSF)
-Home-page: https://github.com/datalad/datalad-osf
-Author: The DataLad Team and Contributors
-Author-email: team@datalad.org
-License: MIT
-Description: # DataLad-OSF: Opening up the Open Science Framework for DataLad 
-        <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-        [![All Contributors](https://img.shields.io/badge/all_contributors-10-orange.svg?style=flat-square)](#contributors-)
-        <!-- ALL-CONTRIBUTORS-BADGE:END -->
-        
-        [![GitHub release](https://img.shields.io/github/release/datalad/datalad-osf.svg)](https://GitHub.com/datalad/datalad-osf/releases/) [![PyPI version fury.io](https://badge.fury.io/py/datalad-osf.svg)](https://pypi.python.org/pypi/datalad-osf/) [![Build status](https://ci.appveyor.com/api/projects/status/298n91oo1mla276t/branch/master?svg=true)](https://ci.appveyor.com/project/mih/datalad-osf/branch/master) [![codecov.io](https://codecov.io/github/datalad/datalad-osf/coverage.svg?branch=master)](https://codecov.io/github/datalad/datalad-osf?branch=master) [![docs](https://github.com/datalad/datalad-osf/workflows/docs/badge.svg)](https://github.com/datalad/datalad-osf/actions?query=workflow%3Adocs) [![Documentation Status](https://readthedocs.org/projects/datalad-osf/badge/?version=latest)](http://docs.datalad.org/projects/osf/en/latest/?badge=latest) [![DOI](https://zenodo.org/badge/272689400.svg)](https://zenodo.org/badge/latestdoi/272689400)
-        
-        
-        Welcome! This repository contains a [DataLad](http://datalad.org) extension that enables DataLad to work with the Open Science Framework (OSF). Use it to share, retrieve and collaborate on DataLad datasets via the OSF.
-        
-        The development of this tool started at [OHBM Brainhack 2020](https://github.com/ohbm/hackathon2020/issues/156) in June 2020, coordinated in [this repository](https://github.com/adswa/git-annex-remote-osf). See our [documentation](http://docs.datalad.org/projects/osf) for more extensive information.
-        
-        ## Requirements
-        
-        - Datalad: relies on [git-annex](http://docs.datalad.org/projects/osf/en/latest/git-annex.branchable.com/), [Git](http://docs.datalad.org/projects/osf/en/latest/git-scm.com/) and Python. If you don’t have DataLad installed yet, please follow the instructions [here](http://handbook.datalad.org/en/latest/intro/installation.html).
-        - Account on the [Open Science Framework (OSF)](https://osf.io/register)
-        
-        ## Installation
-        
-        ```
-        # create and enter a new virtual environment (optional)
-        $ virtualenv --python=python3 ~/env/dl-osf
-        $ . ~/env/dl-osf/bin/activate
-        # install from PyPi
-        $ pip install datalad-osf
-        ```
-        
-        ## How to use
-        
-        See our [documentation](http://docs.datalad.org/projects/osf/) for more info on how to use this tool and a tutorial on major use cases.
-        
-        ## How to contribute
-        You are very welcome to help out developing this tool further. You can contribute by:
-        
-        - Creating an issue for bugs or tips for further development
-        - Making a pull request for any changes suggested by yourself
-        - Testing out the software and communicating your feedback to us
-        
-        Please see our contributing guidelines for more information.
-        
-        ## Contributors ✨
-        
-        Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
-        <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
-        <!-- prettier-ignore-start -->
-        <!-- markdownlint-disable -->
-        <table>
-          <tr>
-            <td align="center"><a href="http://psychoinformatics.de"><img src="https://avatars1.githubusercontent.com/u/136479?v=4" width="100px;" alt=""/><br /><sub><b>Michael Hanke</b></sub></a><br /><a href="#maintenance-mih" title="Maintenance">🚧</a> <a href="https://github.com/datalad/datalad-osf/commits?author=mih" title="Code">💻</a> <a href="https://github.com/datalad/datalad-osf/issues?q=author%3Amih" title="Bug reports">🐛</a> <a href="#ideas-mih" title="Ideas, Planning, & Feedback">🤔</a></td>
-            <td align="center"><a href="https://github.com/DorienHuijser"><img src="https://avatars1.githubusercontent.com/u/58177697?v=4" width="100px;" alt=""/><br /><sub><b>Dorien Huijser</b></sub></a><br /><a href="https://github.com/datalad/datalad-osf/commits?author=DorienHuijser" title="Documentation">📖</a> <a href="#projectManagement-DorienHuijser" title="Project Management">📆</a> <a href="#ideas-DorienHuijser" title="Ideas, Planning, & Feedback">🤔</a> <a href="#userTesting-DorienHuijser" title="User Testing">📓</a></td>
-            <td align="center"><a href="https://github.com/TheDragon246"><img src="https://avatars2.githubusercontent.com/u/63247401?v=4" width="100px;" alt=""/><br /><sub><b>Ashish Sahoo</b></sub></a><br /><a href="https://github.com/datalad/datalad-osf/commits?author=TheDragon246" title="Documentation">📖</a> <a href="#maintenance-TheDragon246" title="Maintenance">🚧</a></td>
-            <td align="center"><a href="https://github.com/SRSteinkamp"><img src="https://avatars2.githubusercontent.com/u/17494653?v=4" width="100px;" alt=""/><br /><sub><b>Simon Steinkamp</b></sub></a><br /><a href="https://github.com/datalad/datalad-osf/commits?author=SRSteinkamp" title="Tests">⚠️</a> <a href="https://github.com/datalad/datalad-osf/commits?author=SRSteinkamp" title="Documentation">📖</a> <a href="#projectManagement-SRSteinkamp" title="Project Management">📆</a> <a href="#ideas-SRSteinkamp" title="Ideas, Planning, & Feedback">🤔</a> <a href="#userTesting-SRSteinkamp" title="User Testing">📓</a> <a href="#maintenance-SRSteinkamp" title="Maintenance">🚧</a></td>
-            <td align="center"><a href="https://github.com/bpoldrack"><img src="https://avatars2.githubusercontent.com/u/10498301?v=4" width="100px;" alt=""/><br /><sub><b>Benjamin Poldrack</b></sub></a><br /><a href="#projectManagement-bpoldrack" title="Project Management">📆</a> <a href="#ideas-bpoldrack" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/datalad/datalad-osf/commits?author=bpoldrack" title="Code">💻</a> <a href="#maintenance-bpoldrack" title="Maintenance">🚧</a></td>
-            <td align="center"><a href="https://gitlab.com/kousu"><img src="https://avatars2.githubusercontent.com/u/987487?v=4" width="100px;" alt=""/><br /><sub><b>Nick</b></sub></a><br /><a href="#projectManagement-kousu" title="Project Management">📆</a> <a href="#ideas-kousu" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/datalad/datalad-osf/commits?author=kousu" title="Code">💻</a> <a href="#maintenance-kousu" title="Maintenance">🚧</a></td>
-            <td align="center"><a href="https://github.com/nbeliy"><img src="https://avatars0.githubusercontent.com/u/44231332?v=4" width="100px;" alt=""/><br /><sub><b>Nikita Beliy</b></sub></a><br /><a href="#ideas-nbeliy" title="Ideas, Planning, & Feedback">🤔</a> <a href="#userTesting-nbeliy" title="User Testing">📓</a></td>
-          </tr>
-          <tr>
-            <td align="center"><a href="https://github.com/mjboos"><img src="https://avatars0.githubusercontent.com/u/7125006?v=4" width="100px;" alt=""/><br /><sub><b>Moritz J. Boos</b></sub></a><br /><a href="https://github.com/datalad/datalad-osf/commits?author=mjboos" title="Code">💻</a> <a href="#userTesting-mjboos" title="User Testing">📓</a> <a href="#ideas-mjboos" title="Ideas, Planning, & Feedback">🤔</a> <a href="#maintenance-mjboos" title="Maintenance">🚧</a></td>
-            <td align="center"><a href="http://www.adina-wagner.com"><img src="https://avatars1.githubusercontent.com/u/29738718?v=4" width="100px;" alt=""/><br /><sub><b>Adina Wagner</b></sub></a><br /><a href="#projectManagement-adswa" title="Project Management">📆</a> <a href="#ideas-adswa" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/datalad/datalad-osf/commits?author=adswa" title="Code">💻</a> <a href="https://github.com/datalad/datalad-osf/commits?author=adswa" title="Documentation">📖</a> <a href="#maintenance-adswa" title="Maintenance">🚧</a></td>
-            <td align="center"><a href="https://www.stefanappelhoff.com"><img src="https://avatars1.githubusercontent.com/u/9084751?v=4" width="100px;" alt=""/><br /><sub><b>Stefan Appelhoff</b></sub></a><br /><a href="https://github.com/datalad/datalad-osf/commits?author=sappelhoff" title="Documentation">📖</a> <a href="#userTesting-sappelhoff" title="User Testing">📓</a></td>
-          </tr>
-        </table>
-        
-        <!-- markdownlint-enable -->
-        <!-- prettier-ignore-end -->
-        <!-- ALL-CONTRIBUTORS-LIST:END -->
-        
-        This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown; charset=UTF-8
-Provides-Extra: devel
+# DataLad-OSF: Opening up the Open Science Framework for DataLad 
+<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
+[![All Contributors](https://img.shields.io/badge/all_contributors-11-orange.svg?style=flat-square)](#contributors-)
+<!-- ALL-CONTRIBUTORS-BADGE:END -->
+
+[![GitHub release](https://img.shields.io/github/release/datalad/datalad-osf.svg)](https://GitHub.com/datalad/datalad-osf/releases/) [![PyPI version fury.io](https://badge.fury.io/py/datalad-osf.svg)](https://pypi.python.org/pypi/datalad-osf/) [![Build status](https://ci.appveyor.com/api/projects/status/298n91oo1mla276t/branch/master?svg=true)](https://ci.appveyor.com/project/mih/datalad-osf/branch/master) [![codecov.io](https://codecov.io/github/datalad/datalad-osf/coverage.svg?branch=master)](https://codecov.io/github/datalad/datalad-osf?branch=master) [![docs](https://github.com/datalad/datalad-osf/workflows/docs/badge.svg)](https://github.com/datalad/datalad-osf/actions?query=workflow%3Adocs) [![Documentation Status](https://readthedocs.org/projects/datalad-osf/badge/?version=latest)](http://docs.datalad.org/projects/osf/en/latest/?badge=latest) [![DOI](https://zenodo.org/badge/272689400.svg)](https://zenodo.org/badge/latestdoi/272689400)
+
+
+Welcome! This repository contains a [DataLad](http://datalad.org) extension that enables DataLad to work with the Open Science Framework (OSF). Use it to share, retrieve and collaborate on DataLad datasets via the OSF.
+
+The development of this tool started at [OHBM Brainhack 2020](https://github.com/ohbm/hackathon2020/issues/156) in June 2020, coordinated in [this repository](https://github.com/adswa/git-annex-remote-osf). See our [documentation](http://docs.datalad.org/projects/osf) for more extensive information.
+
+## Requirements
+
+- Datalad: relies on [git-annex](http://docs.datalad.org/projects/osf/en/latest/git-annex.branchable.com/), [Git](http://docs.datalad.org/projects/osf/en/latest/git-scm.com/) and Python. If you don’t have DataLad installed yet, please follow the instructions [here](http://handbook.datalad.org/en/latest/intro/installation.html).
+- Account on the [Open Science Framework (OSF)](https://osf.io/register)
+
+## Installation
+
+```
+# create and enter a new virtual environment (optional)
+$ virtualenv --python=python3 ~/env/dl-osf
+$ . ~/env/dl-osf/bin/activate
+# install from PyPi
+$ pip install datalad-osf
+```
+
+## How to use
+
+See our [documentation](http://docs.datalad.org/projects/osf/) for more info on how to use this tool and a tutorial on major use cases.
+
+## How to contribute
+You are very welcome to help out developing this tool further. You can contribute by:
+
+- Creating an issue for bugs or tips for further development
+- Making a pull request for any changes suggested by yourself
+- Testing out the software and communicating your feedback to us
+
+Please see our contributing guidelines for more information.
+
+## Contributors ✨
+
+Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable -->
+<table>
+  <tr>
+    <td align="center"><a href="http://psychoinformatics.de"><img src="https://avatars1.githubusercontent.com/u/136479?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Michael Hanke</b></sub></a><br /><a href="#maintenance-mih" title="Maintenance">🚧</a> <a href="https://github.com/datalad/datalad-osf/commits?author=mih" title="Code">💻</a> <a href="https://github.com/datalad/datalad-osf/issues?q=author%3Amih" title="Bug reports">🐛</a> <a href="#ideas-mih" title="Ideas, Planning, & Feedback">🤔</a></td>
+    <td align="center"><a href="https://github.com/DorienHuijser"><img src="https://avatars1.githubusercontent.com/u/58177697?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Dorien Huijser</b></sub></a><br /><a href="https://github.com/datalad/datalad-osf/commits?author=DorienHuijser" title="Documentation">📖</a> <a href="#projectManagement-DorienHuijser" title="Project Management">📆</a> <a href="#ideas-DorienHuijser" title="Ideas, Planning, & Feedback">🤔</a> <a href="#userTesting-DorienHuijser" title="User Testing">📓</a></td>
+    <td align="center"><a href="https://github.com/TheDragon246"><img src="https://avatars2.githubusercontent.com/u/63247401?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Ashish Sahoo</b></sub></a><br /><a href="https://github.com/datalad/datalad-osf/commits?author=TheDragon246" title="Documentation">📖</a> <a href="#maintenance-TheDragon246" title="Maintenance">🚧</a></td>
+    <td align="center"><a href="https://github.com/SRSteinkamp"><img src="https://avatars2.githubusercontent.com/u/17494653?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Simon Steinkamp</b></sub></a><br /><a href="https://github.com/datalad/datalad-osf/commits?author=SRSteinkamp" title="Tests">⚠️</a> <a href="https://github.com/datalad/datalad-osf/commits?author=SRSteinkamp" title="Documentation">📖</a> <a href="#projectManagement-SRSteinkamp" title="Project Management">📆</a> <a href="#ideas-SRSteinkamp" title="Ideas, Planning, & Feedback">🤔</a> <a href="#userTesting-SRSteinkamp" title="User Testing">📓</a> <a href="#maintenance-SRSteinkamp" title="Maintenance">🚧</a></td>
+    <td align="center"><a href="https://github.com/bpoldrack"><img src="https://avatars2.githubusercontent.com/u/10498301?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Benjamin Poldrack</b></sub></a><br /><a href="#projectManagement-bpoldrack" title="Project Management">📆</a> <a href="#ideas-bpoldrack" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/datalad/datalad-osf/commits?author=bpoldrack" title="Code">💻</a> <a href="#maintenance-bpoldrack" title="Maintenance">🚧</a></td>
+    <td align="center"><a href="https://gitlab.com/kousu"><img src="https://avatars2.githubusercontent.com/u/987487?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Nick</b></sub></a><br /><a href="#projectManagement-kousu" title="Project Management">📆</a> <a href="#ideas-kousu" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/datalad/datalad-osf/commits?author=kousu" title="Code">💻</a> <a href="#maintenance-kousu" title="Maintenance">🚧</a></td>
+    <td align="center"><a href="https://github.com/nbeliy"><img src="https://avatars0.githubusercontent.com/u/44231332?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Nikita Beliy</b></sub></a><br /><a href="#ideas-nbeliy" title="Ideas, Planning, & Feedback">🤔</a> <a href="#userTesting-nbeliy" title="User Testing">📓</a></td>
+  </tr>
+  <tr>
+    <td align="center"><a href="https://github.com/mjboos"><img src="https://avatars0.githubusercontent.com/u/7125006?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Moritz J. Boos</b></sub></a><br /><a href="https://github.com/datalad/datalad-osf/commits?author=mjboos" title="Code">💻</a> <a href="#userTesting-mjboos" title="User Testing">📓</a> <a href="#ideas-mjboos" title="Ideas, Planning, & Feedback">🤔</a> <a href="#maintenance-mjboos" title="Maintenance">🚧</a></td>
+    <td align="center"><a href="http://www.adina-wagner.com"><img src="https://avatars1.githubusercontent.com/u/29738718?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Adina Wagner</b></sub></a><br /><a href="#projectManagement-adswa" title="Project Management">📆</a> <a href="#ideas-adswa" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/datalad/datalad-osf/commits?author=adswa" title="Code">💻</a> <a href="https://github.com/datalad/datalad-osf/commits?author=adswa" title="Documentation">📖</a> <a href="#maintenance-adswa" title="Maintenance">🚧</a></td>
+    <td align="center"><a href="https://www.stefanappelhoff.com"><img src="https://avatars1.githubusercontent.com/u/9084751?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Stefan Appelhoff</b></sub></a><br /><a href="https://github.com/datalad/datalad-osf/commits?author=sappelhoff" title="Documentation">📖</a> <a href="#userTesting-sappelhoff" title="User Testing">📓</a></td>
+    <td align="center"><a href="https://github.com/thomasrockhu-codecov"><img src="https://avatars.githubusercontent.com/u/88201630?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Tom Hu</b></sub></a><br /><a href="#infra-thomasrockhu-codecov" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a></td>
+  </tr>
+</table>
+
+<!-- markdownlint-restore -->
+<!-- prettier-ignore-end -->
+
+<!-- ALL-CONTRIBUTORS-LIST:END -->
+
+This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
+
+## Acknowledgements
+
+This DataLad extension was developed with support from the German Federal
+Ministry of Education and Research (BMBF 01GQ1905), and the US National Science
+Foundation (NSF 1912266).
```

#### html2text {}

```diff
@@ -1,24 +1,21 @@
-Metadata-Version: 2.1 Name: datalad_osf Version: 0.2.3.1 Summary: DataLad
-extension to interface with the Open Science Framework (OSF) Home-page: https:/
-/github.com/datalad/datalad-osf Author: The DataLad Team and Contributors
-Author-email: team@datalad.org License: MIT Description: # DataLad-OSF: Opening
-up the Open Science Framework for DataLad  [![All Contributors](https://
-img.shields.io/badge/all_contributors-10-orange.svg?style=flat-square)]
-(#contributors-)  [![GitHub release](https://img.shields.io/github/release/
-datalad/datalad-osf.svg)](https://GitHub.com/datalad/datalad-osf/releases/) [!
-[PyPI version fury.io](https://badge.fury.io/py/datalad-osf.svg)](https://
-pypi.python.org/pypi/datalad-osf/) [![Build status](https://ci.appveyor.com/
-api/projects/status/298n91oo1mla276t/branch/master?svg=true)](https://
-ci.appveyor.com/project/mih/datalad-osf/branch/master) [![codecov.io](https://
-codecov.io/github/datalad/datalad-osf/coverage.svg?branch=master)](https://
-codecov.io/github/datalad/datalad-osf?branch=master) [![docs](https://
-github.com/datalad/datalad-osf/workflows/docs/badge.svg)](https://github.com/
-datalad/datalad-osf/actions?query=workflow%3Adocs) [![Documentation Status]
-(https://readthedocs.org/projects/datalad-osf/badge/?version=latest)](http://
+# DataLad-OSF: Opening up the Open Science Framework for DataLad  [![All
+Contributors](https://img.shields.io/badge/all_contributors-11-
+orange.svg?style=flat-square)](#contributors-)  [![GitHub release](https://
+img.shields.io/github/release/datalad/datalad-osf.svg)](https://GitHub.com/
+datalad/datalad-osf/releases/) [![PyPI version fury.io](https://badge.fury.io/
+py/datalad-osf.svg)](https://pypi.python.org/pypi/datalad-osf/) [![Build
+status](https://ci.appveyor.com/api/projects/status/298n91oo1mla276t/branch/
+master?svg=true)](https://ci.appveyor.com/project/mih/datalad-osf/branch/
+master) [![codecov.io](https://codecov.io/github/datalad/datalad-osf/
+coverage.svg?branch=master)](https://codecov.io/github/datalad/datalad-
+osf?branch=master) [![docs](https://github.com/datalad/datalad-osf/workflows/
+docs/badge.svg)](https://github.com/datalad/datalad-osf/
+actions?query=workflow%3Adocs) [![Documentation Status](https://
+readthedocs.org/projects/datalad-osf/badge/?version=latest)](http://
 docs.datalad.org/projects/osf/en/latest/?badge=latest) [![DOI](https://
 zenodo.org/badge/272689400.svg)](https://zenodo.org/badge/latestdoi/272689400)
 Welcome! This repository contains a [DataLad](http://datalad.org) extension
 that enables DataLad to work with the Open Science Framework (OSF). Use it to
 share, retrieve and collaborate on DataLad datasets via the OSF. The
 development of this tool started at [OHBM Brainhack 2020](https://github.com/
 ohbm/hackathon2020/issues/156) in June 2020, coordinated in [this repository]
@@ -41,16 +38,15 @@
 guidelines for more information. ## Contributors â¨ Thanks goes to these
 wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
            Michael_Hanke                           Dorien_Huijser                  Ashish_Sahoo                         Simon_Steinkamp                               Benjamin_Poldrack                         Nick                   Nikita_Beliy
 
         ð§ ð» ð �            ð ð ð¤ ð    ð ð�             â ï¸ ð ð ð¤ ð�        ð ð¤ ð» �        ð ð¤ ð» �    ð¤ ð
 
-          Moritz_J._Boos                            Adina_Wagner                 Stefan_Appelhoff
+          Moritz_J._Boos                            Adina_Wagner                 Stefan_Appelhoff                                      Tom_Hu
 
-        ð» ð ð¤ �          ð ð¤ ð» ð    ð ð
+        ð» ð ð¤ �          ð ð¤ ð» ð    ð ð                                  ð
    This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
-welcome! Platform: UNKNOWN Classifier: Programming Language :: Python
-Classifier: License :: OSI Approved :: BSD License Classifier: Programming
-Language :: Python :: 3 Requires-Python: >=3.5 Description-Content-Type: text/
-markdown; charset=UTF-8 Provides-Extra: devel
+welcome! ## Acknowledgements This DataLad extension was developed with support
+from the German Federal Ministry of Education and Research (BMBF 01GQ1905), and
+the US National Science Foundation (NSF 1912266).
```

### Comparing `datalad_osf-0.2.3.1/README.md` & `datalad_osf-0.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,26 @@
+Metadata-Version: 2.1
+Name: datalad_osf
+Version: 0.3.0
+Summary: DataLad extension to interface with the Open Science Framework (OSF)
+Home-page: https://github.com/datalad/datalad-osf
+Author: The DataLad Team and Contributors
+Author-email: team@datalad.org
+License: MIT
+Classifier: Programming Language :: Python
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown; charset=UTF-8
+Provides-Extra: devel
+License-File: LICENSE
+
 # DataLad-OSF: Opening up the Open Science Framework for DataLad 
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-10-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-11-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 [![GitHub release](https://img.shields.io/github/release/datalad/datalad-osf.svg)](https://GitHub.com/datalad/datalad-osf/releases/) [![PyPI version fury.io](https://badge.fury.io/py/datalad-osf.svg)](https://pypi.python.org/pypi/datalad-osf/) [![Build status](https://ci.appveyor.com/api/projects/status/298n91oo1mla276t/branch/master?svg=true)](https://ci.appveyor.com/project/mih/datalad-osf/branch/master) [![codecov.io](https://codecov.io/github/datalad/datalad-osf/coverage.svg?branch=master)](https://codecov.io/github/datalad/datalad-osf?branch=master) [![docs](https://github.com/datalad/datalad-osf/workflows/docs/badge.svg)](https://github.com/datalad/datalad-osf/actions?query=workflow%3Adocs) [![Documentation Status](https://readthedocs.org/projects/datalad-osf/badge/?version=latest)](http://docs.datalad.org/projects/osf/en/latest/?badge=latest) [![DOI](https://zenodo.org/badge/272689400.svg)](https://zenodo.org/badge/latestdoi/272689400)
 
 
 Welcome! This repository contains a [DataLad](http://datalad.org) extension that enables DataLad to work with the Open Science Framework (OSF). Use it to share, retrieve and collaborate on DataLad datasets via the OSF.
 
@@ -42,27 +58,35 @@
 
 Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
   <tr>
-    <td align="center"><a href="http://psychoinformatics.de"><img src="https://avatars1.githubusercontent.com/u/136479?v=4" width="100px;" alt=""/><br /><sub><b>Michael Hanke</b></sub></a><br /><a href="#maintenance-mih" title="Maintenance">🚧</a> <a href="https://github.com/datalad/datalad-osf/commits?author=mih" title="Code">💻</a> <a href="https://github.com/datalad/datalad-osf/issues?q=author%3Amih" title="Bug reports">🐛</a> <a href="#ideas-mih" title="Ideas, Planning, & Feedback">🤔</a></td>
-    <td align="center"><a href="https://github.com/DorienHuijser"><img src="https://avatars1.githubusercontent.com/u/58177697?v=4" width="100px;" alt=""/><br /><sub><b>Dorien Huijser</b></sub></a><br /><a href="https://github.com/datalad/datalad-osf/commits?author=DorienHuijser" title="Documentation">📖</a> <a href="#projectManagement-DorienHuijser" title="Project Management">📆</a> <a href="#ideas-DorienHuijser" title="Ideas, Planning, & Feedback">🤔</a> <a href="#userTesting-DorienHuijser" title="User Testing">📓</a></td>
-    <td align="center"><a href="https://github.com/TheDragon246"><img src="https://avatars2.githubusercontent.com/u/63247401?v=4" width="100px;" alt=""/><br /><sub><b>Ashish Sahoo</b></sub></a><br /><a href="https://github.com/datalad/datalad-osf/commits?author=TheDragon246" title="Documentation">📖</a> <a href="#maintenance-TheDragon246" title="Maintenance">🚧</a></td>
-    <td align="center"><a href="https://github.com/SRSteinkamp"><img src="https://avatars2.githubusercontent.com/u/17494653?v=4" width="100px;" alt=""/><br /><sub><b>Simon Steinkamp</b></sub></a><br /><a href="https://github.com/datalad/datalad-osf/commits?author=SRSteinkamp" title="Tests">⚠️</a> <a href="https://github.com/datalad/datalad-osf/commits?author=SRSteinkamp" title="Documentation">📖</a> <a href="#projectManagement-SRSteinkamp" title="Project Management">📆</a> <a href="#ideas-SRSteinkamp" title="Ideas, Planning, & Feedback">🤔</a> <a href="#userTesting-SRSteinkamp" title="User Testing">📓</a> <a href="#maintenance-SRSteinkamp" title="Maintenance">🚧</a></td>
-    <td align="center"><a href="https://github.com/bpoldrack"><img src="https://avatars2.githubusercontent.com/u/10498301?v=4" width="100px;" alt=""/><br /><sub><b>Benjamin Poldrack</b></sub></a><br /><a href="#projectManagement-bpoldrack" title="Project Management">📆</a> <a href="#ideas-bpoldrack" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/datalad/datalad-osf/commits?author=bpoldrack" title="Code">💻</a> <a href="#maintenance-bpoldrack" title="Maintenance">🚧</a></td>
-    <td align="center"><a href="https://gitlab.com/kousu"><img src="https://avatars2.githubusercontent.com/u/987487?v=4" width="100px;" alt=""/><br /><sub><b>Nick</b></sub></a><br /><a href="#projectManagement-kousu" title="Project Management">📆</a> <a href="#ideas-kousu" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/datalad/datalad-osf/commits?author=kousu" title="Code">💻</a> <a href="#maintenance-kousu" title="Maintenance">🚧</a></td>
-    <td align="center"><a href="https://github.com/nbeliy"><img src="https://avatars0.githubusercontent.com/u/44231332?v=4" width="100px;" alt=""/><br /><sub><b>Nikita Beliy</b></sub></a><br /><a href="#ideas-nbeliy" title="Ideas, Planning, & Feedback">🤔</a> <a href="#userTesting-nbeliy" title="User Testing">📓</a></td>
+    <td align="center"><a href="http://psychoinformatics.de"><img src="https://avatars1.githubusercontent.com/u/136479?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Michael Hanke</b></sub></a><br /><a href="#maintenance-mih" title="Maintenance">🚧</a> <a href="https://github.com/datalad/datalad-osf/commits?author=mih" title="Code">💻</a> <a href="https://github.com/datalad/datalad-osf/issues?q=author%3Amih" title="Bug reports">🐛</a> <a href="#ideas-mih" title="Ideas, Planning, & Feedback">🤔</a></td>
+    <td align="center"><a href="https://github.com/DorienHuijser"><img src="https://avatars1.githubusercontent.com/u/58177697?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Dorien Huijser</b></sub></a><br /><a href="https://github.com/datalad/datalad-osf/commits?author=DorienHuijser" title="Documentation">📖</a> <a href="#projectManagement-DorienHuijser" title="Project Management">📆</a> <a href="#ideas-DorienHuijser" title="Ideas, Planning, & Feedback">🤔</a> <a href="#userTesting-DorienHuijser" title="User Testing">📓</a></td>
+    <td align="center"><a href="https://github.com/TheDragon246"><img src="https://avatars2.githubusercontent.com/u/63247401?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Ashish Sahoo</b></sub></a><br /><a href="https://github.com/datalad/datalad-osf/commits?author=TheDragon246" title="Documentation">📖</a> <a href="#maintenance-TheDragon246" title="Maintenance">🚧</a></td>
+    <td align="center"><a href="https://github.com/SRSteinkamp"><img src="https://avatars2.githubusercontent.com/u/17494653?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Simon Steinkamp</b></sub></a><br /><a href="https://github.com/datalad/datalad-osf/commits?author=SRSteinkamp" title="Tests">⚠️</a> <a href="https://github.com/datalad/datalad-osf/commits?author=SRSteinkamp" title="Documentation">📖</a> <a href="#projectManagement-SRSteinkamp" title="Project Management">📆</a> <a href="#ideas-SRSteinkamp" title="Ideas, Planning, & Feedback">🤔</a> <a href="#userTesting-SRSteinkamp" title="User Testing">📓</a> <a href="#maintenance-SRSteinkamp" title="Maintenance">🚧</a></td>
+    <td align="center"><a href="https://github.com/bpoldrack"><img src="https://avatars2.githubusercontent.com/u/10498301?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Benjamin Poldrack</b></sub></a><br /><a href="#projectManagement-bpoldrack" title="Project Management">📆</a> <a href="#ideas-bpoldrack" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/datalad/datalad-osf/commits?author=bpoldrack" title="Code">💻</a> <a href="#maintenance-bpoldrack" title="Maintenance">🚧</a></td>
+    <td align="center"><a href="https://gitlab.com/kousu"><img src="https://avatars2.githubusercontent.com/u/987487?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Nick</b></sub></a><br /><a href="#projectManagement-kousu" title="Project Management">📆</a> <a href="#ideas-kousu" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/datalad/datalad-osf/commits?author=kousu" title="Code">💻</a> <a href="#maintenance-kousu" title="Maintenance">🚧</a></td>
+    <td align="center"><a href="https://github.com/nbeliy"><img src="https://avatars0.githubusercontent.com/u/44231332?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Nikita Beliy</b></sub></a><br /><a href="#ideas-nbeliy" title="Ideas, Planning, & Feedback">🤔</a> <a href="#userTesting-nbeliy" title="User Testing">📓</a></td>
   </tr>
   <tr>
-    <td align="center"><a href="https://github.com/mjboos"><img src="https://avatars0.githubusercontent.com/u/7125006?v=4" width="100px;" alt=""/><br /><sub><b>Moritz J. Boos</b></sub></a><br /><a href="https://github.com/datalad/datalad-osf/commits?author=mjboos" title="Code">💻</a> <a href="#userTesting-mjboos" title="User Testing">📓</a> <a href="#ideas-mjboos" title="Ideas, Planning, & Feedback">🤔</a> <a href="#maintenance-mjboos" title="Maintenance">🚧</a></td>
-    <td align="center"><a href="http://www.adina-wagner.com"><img src="https://avatars1.githubusercontent.com/u/29738718?v=4" width="100px;" alt=""/><br /><sub><b>Adina Wagner</b></sub></a><br /><a href="#projectManagement-adswa" title="Project Management">📆</a> <a href="#ideas-adswa" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/datalad/datalad-osf/commits?author=adswa" title="Code">💻</a> <a href="https://github.com/datalad/datalad-osf/commits?author=adswa" title="Documentation">📖</a> <a href="#maintenance-adswa" title="Maintenance">🚧</a></td>
-    <td align="center"><a href="https://www.stefanappelhoff.com"><img src="https://avatars1.githubusercontent.com/u/9084751?v=4" width="100px;" alt=""/><br /><sub><b>Stefan Appelhoff</b></sub></a><br /><a href="https://github.com/datalad/datalad-osf/commits?author=sappelhoff" title="Documentation">📖</a> <a href="#userTesting-sappelhoff" title="User Testing">📓</a></td>
+    <td align="center"><a href="https://github.com/mjboos"><img src="https://avatars0.githubusercontent.com/u/7125006?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Moritz J. Boos</b></sub></a><br /><a href="https://github.com/datalad/datalad-osf/commits?author=mjboos" title="Code">💻</a> <a href="#userTesting-mjboos" title="User Testing">📓</a> <a href="#ideas-mjboos" title="Ideas, Planning, & Feedback">🤔</a> <a href="#maintenance-mjboos" title="Maintenance">🚧</a></td>
+    <td align="center"><a href="http://www.adina-wagner.com"><img src="https://avatars1.githubusercontent.com/u/29738718?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Adina Wagner</b></sub></a><br /><a href="#projectManagement-adswa" title="Project Management">📆</a> <a href="#ideas-adswa" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/datalad/datalad-osf/commits?author=adswa" title="Code">💻</a> <a href="https://github.com/datalad/datalad-osf/commits?author=adswa" title="Documentation">📖</a> <a href="#maintenance-adswa" title="Maintenance">🚧</a></td>
+    <td align="center"><a href="https://www.stefanappelhoff.com"><img src="https://avatars1.githubusercontent.com/u/9084751?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Stefan Appelhoff</b></sub></a><br /><a href="https://github.com/datalad/datalad-osf/commits?author=sappelhoff" title="Documentation">📖</a> <a href="#userTesting-sappelhoff" title="User Testing">📓</a></td>
+    <td align="center"><a href="https://github.com/thomasrockhu-codecov"><img src="https://avatars.githubusercontent.com/u/88201630?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Tom Hu</b></sub></a><br /><a href="#infra-thomasrockhu-codecov" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a></td>
   </tr>
 </table>
 
-<!-- markdownlint-enable -->
+<!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
+
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 
 This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
+
+## Acknowledgements
+
+This DataLad extension was developed with support from the German Federal
+Ministry of Education and Research (BMBF 01GQ1905), and the US National Science
+Foundation (NSF 1912266).
```

#### html2text {}

```diff
@@ -1,9 +1,16 @@
+Metadata-Version: 2.1 Name: datalad_osf Version: 0.3.0 Summary: DataLad
+extension to interface with the Open Science Framework (OSF) Home-page: https:/
+/github.com/datalad/datalad-osf Author: The DataLad Team and Contributors
+Author-email: team@datalad.org License: MIT Classifier: Programming Language ::
+Python Classifier: License :: OSI Approved :: BSD License Classifier:
+Programming Language :: Python :: 3 Requires-Python: >=3.7 Description-Content-
+Type: text/markdown; charset=UTF-8 Provides-Extra: devel License-File: LICENSE
 # DataLad-OSF: Opening up the Open Science Framework for DataLad  [![All
-Contributors](https://img.shields.io/badge/all_contributors-10-
+Contributors](https://img.shields.io/badge/all_contributors-11-
 orange.svg?style=flat-square)](#contributors-)  [![GitHub release](https://
 img.shields.io/github/release/datalad/datalad-osf.svg)](https://GitHub.com/
 datalad/datalad-osf/releases/) [![PyPI version fury.io](https://badge.fury.io/
 py/datalad-osf.svg)](https://pypi.python.org/pypi/datalad-osf/) [![Build
 status](https://ci.appveyor.com/api/projects/status/298n91oo1mla276t/branch/
 master?svg=true)](https://ci.appveyor.com/project/mih/datalad-osf/branch/
 master) [![codecov.io](https://codecov.io/github/datalad/datalad-osf/
@@ -38,13 +45,15 @@
 guidelines for more information. ## Contributors â¨ Thanks goes to these
 wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
            Michael_Hanke                           Dorien_Huijser                  Ashish_Sahoo                         Simon_Steinkamp                               Benjamin_Poldrack                         Nick                   Nikita_Beliy
 
         ð§ ð» ð �            ð ð ð¤ ð    ð ð�             â ï¸ ð ð ð¤ ð�        ð ð¤ ð» �        ð ð¤ ð» �    ð¤ ð
 
-          Moritz_J._Boos                            Adina_Wagner                 Stefan_Appelhoff
+          Moritz_J._Boos                            Adina_Wagner                 Stefan_Appelhoff                                      Tom_Hu
 
-        ð» ð ð¤ �          ð ð¤ ð» ð    ð ð
+        ð» ð ð¤ �          ð ð¤ ð» ð    ð ð                                  ð
    This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
-welcome!
+welcome! ## Acknowledgements This DataLad extension was developed with support
+from the German Federal Ministry of Education and Research (BMBF 01GQ1905), and
+the US National Science Foundation (NSF 1912266).
```

### Comparing `datalad_osf-0.2.3.1/datalad_osf/__init__.py` & `datalad_osf-0.3.0/datalad_osf/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,13 +33,9 @@
             # optional name of the command in the Python API
             'create_sibling_osf'
         ),
     ]
 )
 
 
-from datalad import setup_package
-from datalad import teardown_package
-
-from ._version import get_versions
-__version__ = get_versions()['version']
-del get_versions
+from . import _version
+__version__ = _version.get_versions()['version']
```

### Comparing `datalad_osf-0.2.3.1/datalad_osf/annex_remote.py` & `datalad_osf-0.3.0/datalad_osf/annex_remote.py`

 * *Files 4% similar despite different names*

```diff
@@ -249,14 +249,21 @@
             # faster to get all at once
             self._files = {
                 # strip leading prefix to be directly indexable with ani
                 # annex key
                 f.path.lstrip(posixpath.sep): f
                 for f in self.storage.files
             }
+            for p, key in (
+                ('.git/refs', 'XDLRA--refs'),
+                ('.git/repo.zip', 'XDLRA--repo-export'),
+            ):
+                handle = self._files.get(p)
+                if handle is not None:
+                    self._files[key] = handle
         return self._files
 
     def removeexportdirectory(self, remote_directory):
         """Remove the directory `remote_directory` from the remote"""
         try:
             folder = [f for f in self.storage.folders
                       if '{sep}{path}{sep}'.format(
```

### Comparing `datalad_osf-0.2.3.1/datalad_osf/create_sibling_osf.py` & `datalad_osf-0.3.0/datalad_osf/create_sibling_osf.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,25 +15,23 @@
 from datalad.support.annexrepo import AnnexRepo
 from datalad.support.param import Parameter
 from datalad.distribution.dataset import (
     datasetmethod,
     EnsureDataset,
     require_dataset
 )
-from datalad.interface.utils import (
-    ac,
-    eval_results,
-)
+from datalad.interface.base import eval_results
 from datalad.support.constraints import (
     EnsureChoice,
     EnsureNone,
     EnsureStr,
     EnsureBool,
 )
 from datalad.interface.results import get_status_dict
+from datalad.interface.utils import ac
 from osfclient import OSF
 from datalad_osf.utils import (
     create_node,
     update_node,
     get_credentials,
 )
 from datalad.utils import ensure_list
```

### Comparing `datalad_osf-0.2.3.1/datalad_osf/credentials.py` & `datalad_osf-0.3.0/datalad_osf/credentials.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 )
 from datalad.dochelpers import exc_str
 from datalad.support.param import Parameter
 from datalad.distribution.dataset import (
     datasetmethod,
     EnsureDataset,
 )
-from datalad.interface.utils import (
+from datalad.interface.base import (
     eval_results,
 )
 from datalad.support.constraints import (
     EnsureChoice,
     EnsureNone,
 )
 from datalad.downloaders.credentials import (
```

### Comparing `datalad_osf-0.2.3.1/datalad_osf/tests/test_public.py` & `datalad_osf-0.3.0/datalad_osf/tests/test_public.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,39 +3,40 @@
 # ## ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ##
 #
 #   See LICENSE file distributed along with the datalad_osf package for the
 #   copyright and license terms.
 #
 # ## ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ##
 
-from mock import patch
-
 from datalad.api import clone
-from datalad.support.exceptions import IncompleteResultsError
-from datalad.tests.utils import (
+from datalad_next.exceptions import IncompleteResultsError
+from datalad_next.tests.utils import (
     assert_in,
     assert_raises,
     eq_,
     skip_if_on_windows,
-    with_tempfile,
 )
+import datalad_osf.utils as dlosf_utils
 
 
 def no_credentials(*args, **kwargs):
     return dict(token=None, username=None, password=None)
 
 
-@with_tempfile
-# make sure that even with locally configured credentials
-# none actually reach the special remote
-@patch('datalad_osf.utils.get_credentials', no_credentials)
-def test_readonly_access(path):
+def test_readonly_access(tmp_path, monkeypatch):
     # obtain a prepared minimal dataset with pre-configured
     # OSF remotes and prestaged data
-    ds = clone('https://github.com/datalad/testrepo--minimalds-osf.git', path)
+    # make sure that even with locally configured credentials
+    # none actually reach the special remote
+    with monkeypatch.context() as m:
+        m.setattr(dlosf_utils, 'get_credentials', no_credentials)
+        ds = clone(
+            'https://github.com/datalad/testrepo--minimalds-osf.git',
+            tmp_path,
+        )
     # check that both OSF remotes were enabled
     assert_in('osfannex', ds.repo.get_remotes())
     assert_in('osftree', ds.repo.get_remotes())
     test_file = ds.repo.pathobj / 'inannex' / 'animated.gif'
     test_file_status = ds.repo.annexstatus([test_file])[test_file]
     eq_(test_file_status['has_content'], False)
     # git-annex reports annexed file to be available on osf remote
@@ -50,27 +51,33 @@
     eq_(ds.repo.annexstatus([test_file])[test_file]['has_content'], True)
 
 
 # git remote helper does not work on windows, due to some unclear
 # line-ending(?) issue
 # https://github.com/datalad/datalad-osf/pull/106#issuecomment-653772696
 @skip_if_on_windows
-@with_tempfile
-@patch('datalad_osf.utils.get_credentials', no_credentials)
-def test_readonly_dataset_access(path):
+def test_readonly_dataset_access(tmp_path, monkeypatch):
     # clone from OSF; ds is self-contained at OSF
-    ds = clone('osf://q8xnk', path)
+    # make sure that even with locally configured credentials
+    # none actually reach the special remote
+    with monkeypatch.context() as m:
+        m.setattr(dlosf_utils, 'get_credentials', no_credentials)
+        ds = clone('osf://q8xnk', tmp_path)
     # standard name storage remote
     assert_in('osf-storage', ds.repo.get_remotes())
     for avail in ds.repo.whereis('inannex'):
         assert_in('7784367b-69c6-483d-9564-67f840715890', avail)
     test_file = ds.repo.pathobj / 'inannex' / 'animated.gif'
     eq_(ds.repo.annexstatus([test_file])[test_file]['has_content'], False)
     ds.repo.call_git(['annex', 'copy', str(test_file), '-f', 'osf-storage'])
     eq_(ds.repo.annexstatus([test_file])[test_file]['has_content'], True)
 
 
-@with_tempfile
-@patch('datalad_osf.utils.get_credentials', no_credentials)
-def test_invalid_url(path):
-
-    assert_raises(IncompleteResultsError, clone, 'osf://q8xnk/somepath', path)
+def test_invalid_url(tmp_path, monkeypatch):
+    # make sure that even with locally configured credentials
+    # none actually reach the special remote
+    with monkeypatch.context() as m:
+        m.setattr(dlosf_utils, 'get_credentials', no_credentials)
+        assert_raises(
+            IncompleteResultsError,
+            clone, 'osf://q8xnk/somepath', tmp_path,
+        )
```

### Comparing `datalad_osf-0.2.3.1/datalad_osf/tests/utils.py` & `datalad_osf-0.3.0/datalad_osf/tests/utils.py`

 * *Files identical despite different names*

### Comparing `datalad_osf-0.2.3.1/datalad_osf/utils.py` & `datalad_osf-0.3.0/datalad_osf/utils.py`

 * *Files identical despite different names*

### Comparing `datalad_osf-0.2.3.1/datalad_osf.egg-info/PKG-INFO` & `datalad_osf-0.3.0/datalad_osf.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,84 +1,92 @@
 Metadata-Version: 2.1
 Name: datalad-osf
-Version: 0.2.3.1
+Version: 0.3.0
 Summary: DataLad extension to interface with the Open Science Framework (OSF)
 Home-page: https://github.com/datalad/datalad-osf
 Author: The DataLad Team and Contributors
 Author-email: team@datalad.org
 License: MIT
-Description: # DataLad-OSF: Opening up the Open Science Framework for DataLad 
-        <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-        [![All Contributors](https://img.shields.io/badge/all_contributors-10-orange.svg?style=flat-square)](#contributors-)
-        <!-- ALL-CONTRIBUTORS-BADGE:END -->
-        
-        [![GitHub release](https://img.shields.io/github/release/datalad/datalad-osf.svg)](https://GitHub.com/datalad/datalad-osf/releases/) [![PyPI version fury.io](https://badge.fury.io/py/datalad-osf.svg)](https://pypi.python.org/pypi/datalad-osf/) [![Build status](https://ci.appveyor.com/api/projects/status/298n91oo1mla276t/branch/master?svg=true)](https://ci.appveyor.com/project/mih/datalad-osf/branch/master) [![codecov.io](https://codecov.io/github/datalad/datalad-osf/coverage.svg?branch=master)](https://codecov.io/github/datalad/datalad-osf?branch=master) [![docs](https://github.com/datalad/datalad-osf/workflows/docs/badge.svg)](https://github.com/datalad/datalad-osf/actions?query=workflow%3Adocs) [![Documentation Status](https://readthedocs.org/projects/datalad-osf/badge/?version=latest)](http://docs.datalad.org/projects/osf/en/latest/?badge=latest) [![DOI](https://zenodo.org/badge/272689400.svg)](https://zenodo.org/badge/latestdoi/272689400)
-        
-        
-        Welcome! This repository contains a [DataLad](http://datalad.org) extension that enables DataLad to work with the Open Science Framework (OSF). Use it to share, retrieve and collaborate on DataLad datasets via the OSF.
-        
-        The development of this tool started at [OHBM Brainhack 2020](https://github.com/ohbm/hackathon2020/issues/156) in June 2020, coordinated in [this repository](https://github.com/adswa/git-annex-remote-osf). See our [documentation](http://docs.datalad.org/projects/osf) for more extensive information.
-        
-        ## Requirements
-        
-        - Datalad: relies on [git-annex](http://docs.datalad.org/projects/osf/en/latest/git-annex.branchable.com/), [Git](http://docs.datalad.org/projects/osf/en/latest/git-scm.com/) and Python. If you don’t have DataLad installed yet, please follow the instructions [here](http://handbook.datalad.org/en/latest/intro/installation.html).
-        - Account on the [Open Science Framework (OSF)](https://osf.io/register)
-        
-        ## Installation
-        
-        ```
-        # create and enter a new virtual environment (optional)
-        $ virtualenv --python=python3 ~/env/dl-osf
-        $ . ~/env/dl-osf/bin/activate
-        # install from PyPi
-        $ pip install datalad-osf
-        ```
-        
-        ## How to use
-        
-        See our [documentation](http://docs.datalad.org/projects/osf/) for more info on how to use this tool and a tutorial on major use cases.
-        
-        ## How to contribute
-        You are very welcome to help out developing this tool further. You can contribute by:
-        
-        - Creating an issue for bugs or tips for further development
-        - Making a pull request for any changes suggested by yourself
-        - Testing out the software and communicating your feedback to us
-        
-        Please see our contributing guidelines for more information.
-        
-        ## Contributors ✨
-        
-        Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
-        <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
-        <!-- prettier-ignore-start -->
-        <!-- markdownlint-disable -->
-        <table>
-          <tr>
-            <td align="center"><a href="http://psychoinformatics.de"><img src="https://avatars1.githubusercontent.com/u/136479?v=4" width="100px;" alt=""/><br /><sub><b>Michael Hanke</b></sub></a><br /><a href="#maintenance-mih" title="Maintenance">🚧</a> <a href="https://github.com/datalad/datalad-osf/commits?author=mih" title="Code">💻</a> <a href="https://github.com/datalad/datalad-osf/issues?q=author%3Amih" title="Bug reports">🐛</a> <a href="#ideas-mih" title="Ideas, Planning, & Feedback">🤔</a></td>
-            <td align="center"><a href="https://github.com/DorienHuijser"><img src="https://avatars1.githubusercontent.com/u/58177697?v=4" width="100px;" alt=""/><br /><sub><b>Dorien Huijser</b></sub></a><br /><a href="https://github.com/datalad/datalad-osf/commits?author=DorienHuijser" title="Documentation">📖</a> <a href="#projectManagement-DorienHuijser" title="Project Management">📆</a> <a href="#ideas-DorienHuijser" title="Ideas, Planning, & Feedback">🤔</a> <a href="#userTesting-DorienHuijser" title="User Testing">📓</a></td>
-            <td align="center"><a href="https://github.com/TheDragon246"><img src="https://avatars2.githubusercontent.com/u/63247401?v=4" width="100px;" alt=""/><br /><sub><b>Ashish Sahoo</b></sub></a><br /><a href="https://github.com/datalad/datalad-osf/commits?author=TheDragon246" title="Documentation">📖</a> <a href="#maintenance-TheDragon246" title="Maintenance">🚧</a></td>
-            <td align="center"><a href="https://github.com/SRSteinkamp"><img src="https://avatars2.githubusercontent.com/u/17494653?v=4" width="100px;" alt=""/><br /><sub><b>Simon Steinkamp</b></sub></a><br /><a href="https://github.com/datalad/datalad-osf/commits?author=SRSteinkamp" title="Tests">⚠️</a> <a href="https://github.com/datalad/datalad-osf/commits?author=SRSteinkamp" title="Documentation">📖</a> <a href="#projectManagement-SRSteinkamp" title="Project Management">📆</a> <a href="#ideas-SRSteinkamp" title="Ideas, Planning, & Feedback">🤔</a> <a href="#userTesting-SRSteinkamp" title="User Testing">📓</a> <a href="#maintenance-SRSteinkamp" title="Maintenance">🚧</a></td>
-            <td align="center"><a href="https://github.com/bpoldrack"><img src="https://avatars2.githubusercontent.com/u/10498301?v=4" width="100px;" alt=""/><br /><sub><b>Benjamin Poldrack</b></sub></a><br /><a href="#projectManagement-bpoldrack" title="Project Management">📆</a> <a href="#ideas-bpoldrack" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/datalad/datalad-osf/commits?author=bpoldrack" title="Code">💻</a> <a href="#maintenance-bpoldrack" title="Maintenance">🚧</a></td>
-            <td align="center"><a href="https://gitlab.com/kousu"><img src="https://avatars2.githubusercontent.com/u/987487?v=4" width="100px;" alt=""/><br /><sub><b>Nick</b></sub></a><br /><a href="#projectManagement-kousu" title="Project Management">📆</a> <a href="#ideas-kousu" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/datalad/datalad-osf/commits?author=kousu" title="Code">💻</a> <a href="#maintenance-kousu" title="Maintenance">🚧</a></td>
-            <td align="center"><a href="https://github.com/nbeliy"><img src="https://avatars0.githubusercontent.com/u/44231332?v=4" width="100px;" alt=""/><br /><sub><b>Nikita Beliy</b></sub></a><br /><a href="#ideas-nbeliy" title="Ideas, Planning, & Feedback">🤔</a> <a href="#userTesting-nbeliy" title="User Testing">📓</a></td>
-          </tr>
-          <tr>
-            <td align="center"><a href="https://github.com/mjboos"><img src="https://avatars0.githubusercontent.com/u/7125006?v=4" width="100px;" alt=""/><br /><sub><b>Moritz J. Boos</b></sub></a><br /><a href="https://github.com/datalad/datalad-osf/commits?author=mjboos" title="Code">💻</a> <a href="#userTesting-mjboos" title="User Testing">📓</a> <a href="#ideas-mjboos" title="Ideas, Planning, & Feedback">🤔</a> <a href="#maintenance-mjboos" title="Maintenance">🚧</a></td>
-            <td align="center"><a href="http://www.adina-wagner.com"><img src="https://avatars1.githubusercontent.com/u/29738718?v=4" width="100px;" alt=""/><br /><sub><b>Adina Wagner</b></sub></a><br /><a href="#projectManagement-adswa" title="Project Management">📆</a> <a href="#ideas-adswa" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/datalad/datalad-osf/commits?author=adswa" title="Code">💻</a> <a href="https://github.com/datalad/datalad-osf/commits?author=adswa" title="Documentation">📖</a> <a href="#maintenance-adswa" title="Maintenance">🚧</a></td>
-            <td align="center"><a href="https://www.stefanappelhoff.com"><img src="https://avatars1.githubusercontent.com/u/9084751?v=4" width="100px;" alt=""/><br /><sub><b>Stefan Appelhoff</b></sub></a><br /><a href="https://github.com/datalad/datalad-osf/commits?author=sappelhoff" title="Documentation">📖</a> <a href="#userTesting-sappelhoff" title="User Testing">📓</a></td>
-          </tr>
-        </table>
-        
-        <!-- markdownlint-enable -->
-        <!-- prettier-ignore-end -->
-        <!-- ALL-CONTRIBUTORS-LIST:END -->
-        
-        This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.5
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: devel
+License-File: LICENSE
+
+# DataLad-OSF: Opening up the Open Science Framework for DataLad 
+<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
+[![All Contributors](https://img.shields.io/badge/all_contributors-11-orange.svg?style=flat-square)](#contributors-)
+<!-- ALL-CONTRIBUTORS-BADGE:END -->
+
+[![GitHub release](https://img.shields.io/github/release/datalad/datalad-osf.svg)](https://GitHub.com/datalad/datalad-osf/releases/) [![PyPI version fury.io](https://badge.fury.io/py/datalad-osf.svg)](https://pypi.python.org/pypi/datalad-osf/) [![Build status](https://ci.appveyor.com/api/projects/status/298n91oo1mla276t/branch/master?svg=true)](https://ci.appveyor.com/project/mih/datalad-osf/branch/master) [![codecov.io](https://codecov.io/github/datalad/datalad-osf/coverage.svg?branch=master)](https://codecov.io/github/datalad/datalad-osf?branch=master) [![docs](https://github.com/datalad/datalad-osf/workflows/docs/badge.svg)](https://github.com/datalad/datalad-osf/actions?query=workflow%3Adocs) [![Documentation Status](https://readthedocs.org/projects/datalad-osf/badge/?version=latest)](http://docs.datalad.org/projects/osf/en/latest/?badge=latest) [![DOI](https://zenodo.org/badge/272689400.svg)](https://zenodo.org/badge/latestdoi/272689400)
+
+
+Welcome! This repository contains a [DataLad](http://datalad.org) extension that enables DataLad to work with the Open Science Framework (OSF). Use it to share, retrieve and collaborate on DataLad datasets via the OSF.
+
+The development of this tool started at [OHBM Brainhack 2020](https://github.com/ohbm/hackathon2020/issues/156) in June 2020, coordinated in [this repository](https://github.com/adswa/git-annex-remote-osf). See our [documentation](http://docs.datalad.org/projects/osf) for more extensive information.
+
+## Requirements
+
+- Datalad: relies on [git-annex](http://docs.datalad.org/projects/osf/en/latest/git-annex.branchable.com/), [Git](http://docs.datalad.org/projects/osf/en/latest/git-scm.com/) and Python. If you don’t have DataLad installed yet, please follow the instructions [here](http://handbook.datalad.org/en/latest/intro/installation.html).
+- Account on the [Open Science Framework (OSF)](https://osf.io/register)
+
+## Installation
+
+```
+# create and enter a new virtual environment (optional)
+$ virtualenv --python=python3 ~/env/dl-osf
+$ . ~/env/dl-osf/bin/activate
+# install from PyPi
+$ pip install datalad-osf
+```
+
+## How to use
+
+See our [documentation](http://docs.datalad.org/projects/osf/) for more info on how to use this tool and a tutorial on major use cases.
+
+## How to contribute
+You are very welcome to help out developing this tool further. You can contribute by:
+
+- Creating an issue for bugs or tips for further development
+- Making a pull request for any changes suggested by yourself
+- Testing out the software and communicating your feedback to us
+
+Please see our contributing guidelines for more information.
+
+## Contributors ✨
+
+Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable -->
+<table>
+  <tr>
+    <td align="center"><a href="http://psychoinformatics.de"><img src="https://avatars1.githubusercontent.com/u/136479?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Michael Hanke</b></sub></a><br /><a href="#maintenance-mih" title="Maintenance">🚧</a> <a href="https://github.com/datalad/datalad-osf/commits?author=mih" title="Code">💻</a> <a href="https://github.com/datalad/datalad-osf/issues?q=author%3Amih" title="Bug reports">🐛</a> <a href="#ideas-mih" title="Ideas, Planning, & Feedback">🤔</a></td>
+    <td align="center"><a href="https://github.com/DorienHuijser"><img src="https://avatars1.githubusercontent.com/u/58177697?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Dorien Huijser</b></sub></a><br /><a href="https://github.com/datalad/datalad-osf/commits?author=DorienHuijser" title="Documentation">📖</a> <a href="#projectManagement-DorienHuijser" title="Project Management">📆</a> <a href="#ideas-DorienHuijser" title="Ideas, Planning, & Feedback">🤔</a> <a href="#userTesting-DorienHuijser" title="User Testing">📓</a></td>
+    <td align="center"><a href="https://github.com/TheDragon246"><img src="https://avatars2.githubusercontent.com/u/63247401?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Ashish Sahoo</b></sub></a><br /><a href="https://github.com/datalad/datalad-osf/commits?author=TheDragon246" title="Documentation">📖</a> <a href="#maintenance-TheDragon246" title="Maintenance">🚧</a></td>
+    <td align="center"><a href="https://github.com/SRSteinkamp"><img src="https://avatars2.githubusercontent.com/u/17494653?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Simon Steinkamp</b></sub></a><br /><a href="https://github.com/datalad/datalad-osf/commits?author=SRSteinkamp" title="Tests">⚠️</a> <a href="https://github.com/datalad/datalad-osf/commits?author=SRSteinkamp" title="Documentation">📖</a> <a href="#projectManagement-SRSteinkamp" title="Project Management">📆</a> <a href="#ideas-SRSteinkamp" title="Ideas, Planning, & Feedback">🤔</a> <a href="#userTesting-SRSteinkamp" title="User Testing">📓</a> <a href="#maintenance-SRSteinkamp" title="Maintenance">🚧</a></td>
+    <td align="center"><a href="https://github.com/bpoldrack"><img src="https://avatars2.githubusercontent.com/u/10498301?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Benjamin Poldrack</b></sub></a><br /><a href="#projectManagement-bpoldrack" title="Project Management">📆</a> <a href="#ideas-bpoldrack" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/datalad/datalad-osf/commits?author=bpoldrack" title="Code">💻</a> <a href="#maintenance-bpoldrack" title="Maintenance">🚧</a></td>
+    <td align="center"><a href="https://gitlab.com/kousu"><img src="https://avatars2.githubusercontent.com/u/987487?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Nick</b></sub></a><br /><a href="#projectManagement-kousu" title="Project Management">📆</a> <a href="#ideas-kousu" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/datalad/datalad-osf/commits?author=kousu" title="Code">💻</a> <a href="#maintenance-kousu" title="Maintenance">🚧</a></td>
+    <td align="center"><a href="https://github.com/nbeliy"><img src="https://avatars0.githubusercontent.com/u/44231332?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Nikita Beliy</b></sub></a><br /><a href="#ideas-nbeliy" title="Ideas, Planning, & Feedback">🤔</a> <a href="#userTesting-nbeliy" title="User Testing">📓</a></td>
+  </tr>
+  <tr>
+    <td align="center"><a href="https://github.com/mjboos"><img src="https://avatars0.githubusercontent.com/u/7125006?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Moritz J. Boos</b></sub></a><br /><a href="https://github.com/datalad/datalad-osf/commits?author=mjboos" title="Code">💻</a> <a href="#userTesting-mjboos" title="User Testing">📓</a> <a href="#ideas-mjboos" title="Ideas, Planning, & Feedback">🤔</a> <a href="#maintenance-mjboos" title="Maintenance">🚧</a></td>
+    <td align="center"><a href="http://www.adina-wagner.com"><img src="https://avatars1.githubusercontent.com/u/29738718?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Adina Wagner</b></sub></a><br /><a href="#projectManagement-adswa" title="Project Management">📆</a> <a href="#ideas-adswa" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/datalad/datalad-osf/commits?author=adswa" title="Code">💻</a> <a href="https://github.com/datalad/datalad-osf/commits?author=adswa" title="Documentation">📖</a> <a href="#maintenance-adswa" title="Maintenance">🚧</a></td>
+    <td align="center"><a href="https://www.stefanappelhoff.com"><img src="https://avatars1.githubusercontent.com/u/9084751?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Stefan Appelhoff</b></sub></a><br /><a href="https://github.com/datalad/datalad-osf/commits?author=sappelhoff" title="Documentation">📖</a> <a href="#userTesting-sappelhoff" title="User Testing">📓</a></td>
+    <td align="center"><a href="https://github.com/thomasrockhu-codecov"><img src="https://avatars.githubusercontent.com/u/88201630?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Tom Hu</b></sub></a><br /><a href="#infra-thomasrockhu-codecov" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a></td>
+  </tr>
+</table>
+
+<!-- markdownlint-restore -->
+<!-- prettier-ignore-end -->
+
+<!-- ALL-CONTRIBUTORS-LIST:END -->
+
+This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
+
+## Acknowledgements
+
+This DataLad extension was developed with support from the German Federal
+Ministry of Education and Research (BMBF 01GQ1905), and the US National Science
+Foundation (NSF 1912266).
```

#### html2text {}

```diff
@@ -1,24 +1,28 @@
-Metadata-Version: 2.1 Name: datalad-osf Version: 0.2.3.1 Summary: DataLad
+Metadata-Version: 2.1 Name: datalad-osf Version: 0.3.0 Summary: DataLad
 extension to interface with the Open Science Framework (OSF) Home-page: https:/
 /github.com/datalad/datalad-osf Author: The DataLad Team and Contributors
-Author-email: team@datalad.org License: MIT Description: # DataLad-OSF: Opening
-up the Open Science Framework for DataLad  [![All Contributors](https://
-img.shields.io/badge/all_contributors-10-orange.svg?style=flat-square)]
-(#contributors-)  [![GitHub release](https://img.shields.io/github/release/
-datalad/datalad-osf.svg)](https://GitHub.com/datalad/datalad-osf/releases/) [!
-[PyPI version fury.io](https://badge.fury.io/py/datalad-osf.svg)](https://
-pypi.python.org/pypi/datalad-osf/) [![Build status](https://ci.appveyor.com/
-api/projects/status/298n91oo1mla276t/branch/master?svg=true)](https://
-ci.appveyor.com/project/mih/datalad-osf/branch/master) [![codecov.io](https://
-codecov.io/github/datalad/datalad-osf/coverage.svg?branch=master)](https://
-codecov.io/github/datalad/datalad-osf?branch=master) [![docs](https://
-github.com/datalad/datalad-osf/workflows/docs/badge.svg)](https://github.com/
-datalad/datalad-osf/actions?query=workflow%3Adocs) [![Documentation Status]
-(https://readthedocs.org/projects/datalad-osf/badge/?version=latest)](http://
+Author-email: team@datalad.org License: MIT Classifier: Programming Language ::
+Python Classifier: License :: OSI Approved :: BSD License Classifier:
+Programming Language :: Python :: 3 Requires-Python: >=3.7 Description-Content-
+Type: text/markdown; charset=UTF-8 Provides-Extra: devel License-File: LICENSE
+# DataLad-OSF: Opening up the Open Science Framework for DataLad  [![All
+Contributors](https://img.shields.io/badge/all_contributors-11-
+orange.svg?style=flat-square)](#contributors-)  [![GitHub release](https://
+img.shields.io/github/release/datalad/datalad-osf.svg)](https://GitHub.com/
+datalad/datalad-osf/releases/) [![PyPI version fury.io](https://badge.fury.io/
+py/datalad-osf.svg)](https://pypi.python.org/pypi/datalad-osf/) [![Build
+status](https://ci.appveyor.com/api/projects/status/298n91oo1mla276t/branch/
+master?svg=true)](https://ci.appveyor.com/project/mih/datalad-osf/branch/
+master) [![codecov.io](https://codecov.io/github/datalad/datalad-osf/
+coverage.svg?branch=master)](https://codecov.io/github/datalad/datalad-
+osf?branch=master) [![docs](https://github.com/datalad/datalad-osf/workflows/
+docs/badge.svg)](https://github.com/datalad/datalad-osf/
+actions?query=workflow%3Adocs) [![Documentation Status](https://
+readthedocs.org/projects/datalad-osf/badge/?version=latest)](http://
 docs.datalad.org/projects/osf/en/latest/?badge=latest) [![DOI](https://
 zenodo.org/badge/272689400.svg)](https://zenodo.org/badge/latestdoi/272689400)
 Welcome! This repository contains a [DataLad](http://datalad.org) extension
 that enables DataLad to work with the Open Science Framework (OSF). Use it to
 share, retrieve and collaborate on DataLad datasets via the OSF. The
 development of this tool started at [OHBM Brainhack 2020](https://github.com/
 ohbm/hackathon2020/issues/156) in June 2020, coordinated in [this repository]
@@ -41,16 +45,15 @@
 guidelines for more information. ## Contributors â¨ Thanks goes to these
 wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
            Michael_Hanke                           Dorien_Huijser                  Ashish_Sahoo                         Simon_Steinkamp                               Benjamin_Poldrack                         Nick                   Nikita_Beliy
 
         ð§ ð» ð �            ð ð ð¤ ð    ð ð�             â ï¸ ð ð ð¤ ð�        ð ð¤ ð» �        ð ð¤ ð» �    ð¤ ð
 
-          Moritz_J._Boos                            Adina_Wagner                 Stefan_Appelhoff
+          Moritz_J._Boos                            Adina_Wagner                 Stefan_Appelhoff                                      Tom_Hu
 
-        ð» ð ð¤ �          ð ð¤ ð» ð    ð ð
+        ð» ð ð¤ �          ð ð¤ ð» ð    ð ð                                  ð
    This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
-welcome! Platform: UNKNOWN Classifier: Programming Language :: Python
-Classifier: License :: OSI Approved :: BSD License Classifier: Programming
-Language :: Python :: 3 Requires-Python: >=3.5 Description-Content-Type: text/
-markdown; charset=UTF-8 Provides-Extra: devel
+welcome! ## Acknowledgements This DataLad extension was developed with support
+from the German Federal Ministry of Education and Research (BMBF 01GQ1905), and
+the US National Science Foundation (NSF 1912266).
```

### Comparing `datalad_osf-0.2.3.1/datalad_osf.egg-info/SOURCES.txt` & `datalad_osf-0.3.0/datalad_osf.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,28 @@
+LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 versioneer.py
 datalad_osf/__init__.py
 datalad_osf/_version.py
 datalad_osf/annex_remote.py
+datalad_osf/conftest.py
 datalad_osf/create_sibling_osf.py
 datalad_osf/credentials.py
 datalad_osf/git_remote.py
 datalad_osf/utils.py
 datalad_osf.egg-info/PKG-INFO
 datalad_osf.egg-info/SOURCES.txt
 datalad_osf.egg-info/dependency_links.txt
 datalad_osf.egg-info/entry_points.txt
 datalad_osf.egg-info/requires.txt
 datalad_osf.egg-info/top_level.txt
 datalad_osf/tests/__init__.py
+datalad_osf/tests/fixtures.py
 datalad_osf/tests/test_create_sibling_osf.py
 datalad_osf/tests/test_public.py
 datalad_osf/tests/test_register.py
 datalad_osf/tests/test_remote.py
 datalad_osf/tests/utils.py
```

### Comparing `datalad_osf-0.2.3.1/setup.cfg` & `datalad_osf-0.3.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -8,36 +8,35 @@
 license = MIT
 classifiers = 
 	Programming Language :: Python
 	License :: OSI Approved :: BSD License
 	Programming Language :: Python :: 3
 
 [options]
-python_requires = >= 3.5
+python_requires = >= 3.7
 install_requires = 
-	datalad >= 0.13.0
-	annexremote >= 1.4.0
+	datalad >= 0.18.4
+	datalad_next >= 1.0.0b3
+	annexremote >= 1.5.0
 	osfclient >= 0.0.5
-test_requires = 
-	nose
-	coverage
 packages = find:
 include_package_data = True
 
 [options.extras_require]
 devel = 
-	nose
+	pytest
+	pytest-cov
 	coverage
 
 [options.packages.find]
 exclude = 
 	_datalad_buildsupport
 
 [versioneer]
-vcs = git
+VCS = git
 style = pep440
 versionfile_source = datalad_osf/_version.py
 versionfile_build = datalad_osf/_version.py
 tag_prefix = 
 parentdir_prefix = 
 
 [coverage:report]
```

### Comparing `datalad_osf-0.2.3.1/setup.py` & `datalad_osf-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `datalad_osf-0.2.3.1/versioneer.py` & `datalad_osf-0.3.0/versioneer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,64 @@
 
-# Version: 0.18
+# Version: 0.28
 
 """The Versioneer - like a rocketeer, but for versions.
 
 The Versioneer
 ==============
 
 * like a rocketeer, but for versions!
-* https://github.com/warner/python-versioneer
+* https://github.com/python-versioneer/python-versioneer
 * Brian Warner
-* License: Public Domain
-* Compatible With: python2.6, 2.7, 3.2, 3.3, 3.4, 3.5, 3.6, and pypy
-* [![Latest Version]
-(https://pypip.in/version/versioneer/badge.svg?style=flat)
-](https://pypi.python.org/pypi/versioneer/)
-* [![Build Status]
-(https://travis-ci.org/warner/python-versioneer.png?branch=master)
-](https://travis-ci.org/warner/python-versioneer)
+* License: Public Domain (Unlicense)
+* Compatible with: Python 3.7, 3.8, 3.9, 3.10 and pypy3
+* [![Latest Version][pypi-image]][pypi-url]
+* [![Build Status][travis-image]][travis-url]
 
-This is a tool for managing a recorded version number in distutils-based
+This is a tool for managing a recorded version number in setuptools-based
 python projects. The goal is to remove the tedious and error-prone "update
 the embedded version string" step from your release process. Making a new
 release should be as easy as recording a new tag in your version-control
 system, and maybe making new tarballs.
 
 
 ## Quick Install
 
-* `pip install versioneer` to somewhere to your $PATH
-* add a `[versioneer]` section to your setup.cfg (see below)
-* run `versioneer install` in your source tree, commit the results
+Versioneer provides two installation modes. The "classic" vendored mode installs
+a copy of versioneer into your repository. The experimental build-time dependency mode
+is intended to allow you to skip this step and simplify the process of upgrading.
+
+### Vendored mode
+
+* `pip install versioneer` to somewhere in your $PATH
+   * A [conda-forge recipe](https://github.com/conda-forge/versioneer-feedstock) is
+     available, so you can also use `conda install -c conda-forge versioneer`
+* add a `[tool.versioneer]` section to your `pyproject.toml` or a
+  `[versioneer]` section to your `setup.cfg` (see [Install](INSTALL.md))
+   * Note that you will need to add `tomli; python_version < "3.11"` to your
+     build-time dependencies if you use `pyproject.toml`
+* run `versioneer install --vendor` in your source tree, commit the results
+* verify version information with `python setup.py version`
+
+### Build-time dependency mode
+
+* `pip install versioneer` to somewhere in your $PATH
+   * A [conda-forge recipe](https://github.com/conda-forge/versioneer-feedstock) is
+     available, so you can also use `conda install -c conda-forge versioneer`
+* add a `[tool.versioneer]` section to your `pyproject.toml` or a
+  `[versioneer]` section to your `setup.cfg` (see [Install](INSTALL.md))
+* add `versioneer` (with `[toml]` extra, if configuring in `pyproject.toml`)
+  to the `requires` key of the `build-system` table in `pyproject.toml`:
+  ```toml
+  [build-system]
+  requires = ["setuptools", "versioneer[toml]"]
+  build-backend = "setuptools.build_meta"
+  ```
+* run `versioneer install --no-vendor` in your source tree, commit the results
+* verify version information with `python setup.py version`
 
 ## Version Identifiers
 
 Source trees come from a variety of places:
 
 * a version-control system checkout (mostly used by developers)
 * a nightly tarball, produced by build automation
@@ -57,15 +82,15 @@
 unreleased software (between tags), the version identifier should provide
 enough information to help developers recreate the same tree, while also
 giving them an idea of roughly how old the tree is (after version 1.2, before
 version 1.3). Many VCS systems can report a description that captures this,
 for example `git describe --tags --dirty --always` reports things like
 "0.7-1-g574ab98-dirty" to indicate that the checkout is one revision past the
 0.7 tag, has a unique revision id of "574ab98", and is "dirty" (it has
-uncommitted changes.
+uncommitted changes).
 
 The version identifier is used for multiple purposes:
 
 * to allow the module to self-identify its version: `myproject.__version__`
 * to choose a name and prefix for a 'setup.py sdist' tarball
 
 ## Theory of Operation
@@ -162,45 +187,45 @@
 display the full contents of `get_versions()` (including the `error` string,
 which may help identify what went wrong).
 
 ## Known Limitations
 
 Some situations are known to cause problems for Versioneer. This details the
 most significant ones. More can be found on Github
-[issues page](https://github.com/warner/python-versioneer/issues).
+[issues page](https://github.com/python-versioneer/python-versioneer/issues).
 
 ### Subprojects
 
 Versioneer has limited support for source trees in which `setup.py` is not in
 the root directory (e.g. `setup.py` and `.git/` are *not* siblings). The are
 two common reasons why `setup.py` might not be in the root:
 
 * Source trees which contain multiple subprojects, such as
   [Buildbot](https://github.com/buildbot/buildbot), which contains both
   "master" and "slave" subprojects, each with their own `setup.py`,
   `setup.cfg`, and `tox.ini`. Projects like these produce multiple PyPI
   distributions (and upload multiple independently-installable tarballs).
 * Source trees whose main purpose is to contain a C library, but which also
-  provide bindings to Python (and perhaps other langauges) in subdirectories.
+  provide bindings to Python (and perhaps other languages) in subdirectories.
 
 Versioneer will look for `.git` in parent directories, and most operations
 should get the right version string. However `pip` and `setuptools` have bugs
 and implementation details which frequently cause `pip install .` from a
 subproject directory to fail to find a correct version string (so it usually
 defaults to `0+unknown`).
 
 `pip install --editable .` should work correctly. `setup.py install` might
 work too.
 
 Pip-8.1.1 is known to have this problem, but hopefully it will get fixed in
 some later version.
 
-[Bug #38](https://github.com/warner/python-versioneer/issues/38) is tracking
+[Bug #38](https://github.com/python-versioneer/python-versioneer/issues/38) is tracking
 this issue. The discussion in
-[PR #61](https://github.com/warner/python-versioneer/pull/61) describes the
+[PR #61](https://github.com/python-versioneer/python-versioneer/pull/61) describes the
 issue from the Versioneer side in more detail.
 [pip PR#3176](https://github.com/pypa/pip/pull/3176) and
 [pip PR#3615](https://github.com/pypa/pip/pull/3615) contain work to improve
 pip to let Versioneer work correctly.
 
 Versioneer-0.16 and earlier only looked for a `.git` directory next to the
 `setup.cfg`, so subprojects were completely unsupported with those releases.
@@ -220,39 +245,28 @@
 `pkg_resources.DistributionNotFound` errors when running the entrypoint
 script, which must be resolved by re-installing the package. This happens
 when the install happens with one version, then the egg_info data is
 regenerated while a different version is checked out. Many setup.py commands
 cause egg_info to be rebuilt (including `sdist`, `wheel`, and installing into
 a different virtualenv), so this can be surprising.
 
-[Bug #83](https://github.com/warner/python-versioneer/issues/83) describes
+[Bug #83](https://github.com/python-versioneer/python-versioneer/issues/83) describes
 this one, but upgrading to a newer version of setuptools should probably
 resolve it.
 
-### Unicode version strings
-
-While Versioneer works (and is continually tested) with both Python 2 and
-Python 3, it is not entirely consistent with bytes-vs-unicode distinctions.
-Newer releases probably generate unicode version strings on py2. It's not
-clear that this is wrong, but it may be surprising for applications when then
-write these strings to a network connection or include them in bytes-oriented
-APIs like cryptographic checksums.
-
-[Bug #71](https://github.com/warner/python-versioneer/issues/71) investigates
-this question.
-
 
 ## Updating Versioneer
 
 To upgrade your project to a new release of Versioneer, do the following:
 
 * install the new Versioneer (`pip install -U versioneer` or equivalent)
-* edit `setup.cfg`, if necessary, to include any new configuration settings
-  indicated by the release notes. See [UPGRADING](./UPGRADING.md) for details.
-* re-run `versioneer install` in your source tree, to replace
+* edit `setup.cfg` and `pyproject.toml`, if necessary,
+  to include any new configuration settings indicated by the release notes.
+  See [UPGRADING](./UPGRADING.md) for details.
+* re-run `versioneer install --[no-]vendor` in your source tree, to replace
   `SRC/_version.py`
 * commit any changed files
 
 ## Future Directions
 
 This tool is designed to make it easily extended to other version-control
 systems: all VCS-specific components are in separate directories like
@@ -261,36 +275,62 @@
 will take a VCS name as an argument, and will construct a version of
 `versioneer.py` that is specific to the given VCS. It might also take the
 configuration arguments that are currently provided manually during
 installation by editing setup.py . Alternatively, it might go the other
 direction and include code from all supported VCS systems, reducing the
 number of intermediate scripts.
 
+## Similar projects
+
+* [setuptools_scm](https://github.com/pypa/setuptools_scm/) - a non-vendored build-time
+  dependency
+* [minver](https://github.com/jbweston/miniver) - a lightweight reimplementation of
+  versioneer
+* [versioningit](https://github.com/jwodder/versioningit) - a PEP 518-based setuptools
+  plugin
 
 ## License
 
 To make Versioneer easier to embed, all its code is dedicated to the public
 domain. The `_version.py` that it creates is also in the public domain.
-Specifically, both are released under the Creative Commons "Public Domain
-Dedication" license (CC0-1.0), as described in
-https://creativecommons.org/publicdomain/zero/1.0/ .
+Specifically, both are released under the "Unlicense", as described in
+https://unlicense.org/.
+
+[pypi-image]: https://img.shields.io/pypi/v/versioneer.svg
+[pypi-url]: https://pypi.python.org/pypi/versioneer/
+[travis-image]:
+https://img.shields.io/travis/com/python-versioneer/python-versioneer.svg
+[travis-url]: https://travis-ci.com/github/python-versioneer/python-versioneer
 
 """
+# pylint:disable=invalid-name,import-outside-toplevel,missing-function-docstring
+# pylint:disable=missing-class-docstring,too-many-branches,too-many-statements
+# pylint:disable=raise-missing-from,too-many-lines,too-many-locals,import-error
+# pylint:disable=too-few-public-methods,redefined-outer-name,consider-using-with
+# pylint:disable=attribute-defined-outside-init,too-many-arguments
 
-from __future__ import print_function
-try:
-    import configparser
-except ImportError:
-    import ConfigParser as configparser
+import configparser
 import errno
 import json
 import os
 import re
 import subprocess
 import sys
+from pathlib import Path
+from typing import Callable, Dict
+import functools
+
+have_tomllib = True
+if sys.version_info >= (3, 11):
+    import tomllib
+else:
+    try:
+        import tomli as tomllib
+    except ImportError:
+        have_tomllib = False
 
 
 class VersioneerConfig:
     """Container for Versioneer configuration parameters."""
 
 
 def get_root():
@@ -317,128 +357,144 @@
     try:
         # Certain runtime workflows (setup.py install/develop in a setuptools
         # tree) execute all dependencies in a single python process, so
         # "versioneer" may be imported multiple times, and python's shared
         # module-import table will cache the first one. So we can't use
         # os.path.dirname(__file__), as that will find whichever
         # versioneer.py was first imported, even in later projects.
-        me = os.path.realpath(os.path.abspath(__file__))
-        me_dir = os.path.normcase(os.path.splitext(me)[0])
+        my_path = os.path.realpath(os.path.abspath(__file__))
+        me_dir = os.path.normcase(os.path.splitext(my_path)[0])
         vsr_dir = os.path.normcase(os.path.splitext(versioneer_py)[0])
-        if me_dir != vsr_dir:
+        if me_dir != vsr_dir and "VERSIONEER_PEP518" not in globals():
             print("Warning: build in %s is using versioneer.py from %s"
-                  % (os.path.dirname(me), versioneer_py))
+                  % (os.path.dirname(my_path), versioneer_py))
     except NameError:
         pass
     return root
 
 
 def get_config_from_root(root):
     """Read the project setup.cfg file to determine Versioneer config."""
-    # This might raise EnvironmentError (if setup.cfg is missing), or
+    # This might raise OSError (if setup.cfg is missing), or
     # configparser.NoSectionError (if it lacks a [versioneer] section), or
     # configparser.NoOptionError (if it lacks "VCS="). See the docstring at
     # the top of versioneer.py for instructions on writing your setup.cfg .
-    setup_cfg = os.path.join(root, "setup.cfg")
-    parser = configparser.SafeConfigParser()
-    with open(setup_cfg, "r") as f:
-        parser.readfp(f)
-    VCS = parser.get("versioneer", "VCS")  # mandatory
-
-    def get(parser, name):
-        if parser.has_option("versioneer", name):
-            return parser.get("versioneer", name)
-        return None
+    root = Path(root)
+    pyproject_toml = root / "pyproject.toml"
+    setup_cfg = root / "setup.cfg"
+    section = None
+    if pyproject_toml.exists() and have_tomllib:
+        try:
+            with open(pyproject_toml, 'rb') as fobj:
+                pp = tomllib.load(fobj)
+            section = pp['tool']['versioneer']
+        except (tomllib.TOMLDecodeError, KeyError):
+            pass
+    if not section:
+        parser = configparser.ConfigParser()
+        with open(setup_cfg) as cfg_file:
+            parser.read_file(cfg_file)
+        parser.get("versioneer", "VCS")  # raise error if missing
+
+        section = parser["versioneer"]
+
     cfg = VersioneerConfig()
-    cfg.VCS = VCS
-    cfg.style = get(parser, "style") or ""
-    cfg.versionfile_source = get(parser, "versionfile_source")
-    cfg.versionfile_build = get(parser, "versionfile_build")
-    cfg.tag_prefix = get(parser, "tag_prefix")
-    if cfg.tag_prefix in ("''", '""'):
+    cfg.VCS = section['VCS']
+    cfg.style = section.get("style", "")
+    cfg.versionfile_source = section.get("versionfile_source")
+    cfg.versionfile_build = section.get("versionfile_build")
+    cfg.tag_prefix = section.get("tag_prefix")
+    if cfg.tag_prefix in ("''", '""', None):
         cfg.tag_prefix = ""
-    cfg.parentdir_prefix = get(parser, "parentdir_prefix")
-    cfg.verbose = get(parser, "verbose")
+    cfg.parentdir_prefix = section.get("parentdir_prefix")
+    cfg.verbose = section.get("verbose")
     return cfg
 
 
 class NotThisMethod(Exception):
     """Exception raised if a method is not valid for the current scenario."""
 
 
 # these dictionaries contain VCS-specific tools
-LONG_VERSION_PY = {}
-HANDLERS = {}
+LONG_VERSION_PY: Dict[str, str] = {}
+HANDLERS: Dict[str, Dict[str, Callable]] = {}
 
 
 def register_vcs_handler(vcs, method):  # decorator
-    """Decorator to mark a method as the handler for a particular VCS."""
+    """Create decorator to mark a method as the handler of a VCS."""
     def decorate(f):
         """Store f in HANDLERS[vcs][method]."""
-        if vcs not in HANDLERS:
-            HANDLERS[vcs] = {}
-        HANDLERS[vcs][method] = f
+        HANDLERS.setdefault(vcs, {})[method] = f
         return f
     return decorate
 
 
 def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
                 env=None):
     """Call the given command(s)."""
     assert isinstance(commands, list)
-    p = None
-    for c in commands:
+    process = None
+
+    popen_kwargs = {}
+    if sys.platform == "win32":
+        # This hides the console window if pythonw.exe is used
+        startupinfo = subprocess.STARTUPINFO()
+        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+        popen_kwargs["startupinfo"] = startupinfo
+
+    for command in commands:
         try:
-            dispcmd = str([c] + args)
+            dispcmd = str([command] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            p = subprocess.Popen([c] + args, cwd=cwd, env=env,
-                                 stdout=subprocess.PIPE,
-                                 stderr=(subprocess.PIPE if hide_stderr
-                                         else None))
+            process = subprocess.Popen([command] + args, cwd=cwd, env=env,
+                                       stdout=subprocess.PIPE,
+                                       stderr=(subprocess.PIPE if hide_stderr
+                                               else None), **popen_kwargs)
             break
-        except EnvironmentError:
+        except OSError:
             e = sys.exc_info()[1]
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %s" % dispcmd)
                 print(e)
             return None, None
     else:
         if verbose:
             print("unable to find command, tried %s" % (commands,))
         return None, None
-    stdout = p.communicate()[0].strip()
-    if sys.version_info[0] >= 3:
-        stdout = stdout.decode()
-    if p.returncode != 0:
+    stdout = process.communicate()[0].strip().decode()
+    if process.returncode != 0:
         if verbose:
             print("unable to run %s (error)" % dispcmd)
             print("stdout was %s" % stdout)
-        return None, p.returncode
-    return stdout, p.returncode
+        return None, process.returncode
+    return stdout, process.returncode
 
 
-LONG_VERSION_PY['git'] = '''
+LONG_VERSION_PY['git'] = r'''
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by githubs download-from-tag
 # feature). Distribution tarballs (built by setup.py sdist) and build
 # directories (produced by setup.py build) will contain a much shorter file
 # that just contains the computed version number.
 
-# This file is released into the public domain. Generated by
-# versioneer-0.18 (https://github.com/warner/python-versioneer)
+# This file is released into the public domain.
+# Generated by versioneer-0.28
+# https://github.com/python-versioneer/python-versioneer
 
 """Git implementation of _version.py."""
 
 import errno
 import os
 import re
 import subprocess
 import sys
+from typing import Callable, Dict
+import functools
 
 
 def get_keywords():
     """Get the keywords needed to look up the version information."""
     # these strings will be replaced by git during git-archive.
     # setup.py/versioneer.py will grep for the variable names, so they must
     # each be defined on a line of their own. _version.py will just call
@@ -468,84 +524,89 @@
     return cfg
 
 
 class NotThisMethod(Exception):
     """Exception raised if a method is not valid for the current scenario."""
 
 
-LONG_VERSION_PY = {}
-HANDLERS = {}
+LONG_VERSION_PY: Dict[str, str] = {}
+HANDLERS: Dict[str, Dict[str, Callable]] = {}
 
 
 def register_vcs_handler(vcs, method):  # decorator
-    """Decorator to mark a method as the handler for a particular VCS."""
+    """Create decorator to mark a method as the handler of a VCS."""
     def decorate(f):
         """Store f in HANDLERS[vcs][method]."""
         if vcs not in HANDLERS:
             HANDLERS[vcs] = {}
         HANDLERS[vcs][method] = f
         return f
     return decorate
 
 
 def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
                 env=None):
     """Call the given command(s)."""
     assert isinstance(commands, list)
-    p = None
-    for c in commands:
+    process = None
+
+    popen_kwargs = {}
+    if sys.platform == "win32":
+        # This hides the console window if pythonw.exe is used
+        startupinfo = subprocess.STARTUPINFO()
+        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+        popen_kwargs["startupinfo"] = startupinfo
+
+    for command in commands:
         try:
-            dispcmd = str([c] + args)
+            dispcmd = str([command] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            p = subprocess.Popen([c] + args, cwd=cwd, env=env,
-                                 stdout=subprocess.PIPE,
-                                 stderr=(subprocess.PIPE if hide_stderr
-                                         else None))
+            process = subprocess.Popen([command] + args, cwd=cwd, env=env,
+                                       stdout=subprocess.PIPE,
+                                       stderr=(subprocess.PIPE if hide_stderr
+                                               else None), **popen_kwargs)
             break
-        except EnvironmentError:
+        except OSError:
             e = sys.exc_info()[1]
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %%s" %% dispcmd)
                 print(e)
             return None, None
     else:
         if verbose:
             print("unable to find command, tried %%s" %% (commands,))
         return None, None
-    stdout = p.communicate()[0].strip()
-    if sys.version_info[0] >= 3:
-        stdout = stdout.decode()
-    if p.returncode != 0:
+    stdout = process.communicate()[0].strip().decode()
+    if process.returncode != 0:
         if verbose:
             print("unable to run %%s (error)" %% dispcmd)
             print("stdout was %%s" %% stdout)
-        return None, p.returncode
-    return stdout, p.returncode
+        return None, process.returncode
+    return stdout, process.returncode
 
 
 def versions_from_parentdir(parentdir_prefix, root, verbose):
     """Try to determine the version from the parent directory name.
 
     Source tarballs conventionally unpack into a directory that includes both
     the project name and a version string. We will also support searching up
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
 
-    for i in range(3):
+    for _ in range(3):
         dirname = os.path.basename(root)
         if dirname.startswith(parentdir_prefix):
             return {"version": dirname[len(parentdir_prefix):],
                     "full-revisionid": None,
                     "dirty": False, "error": None, "date": None}
-        else:
-            rootdirs.append(root)
-            root = os.path.dirname(root)  # up a level
+        rootdirs.append(root)
+        root = os.path.dirname(root)  # up a level
 
     if verbose:
         print("Tried directories %%s but none started with prefix %%s" %%
               (str(rootdirs), parentdir_prefix))
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
@@ -554,75 +615,83 @@
     """Extract version information from the given file."""
     # the code embedded in _version.py can just fetch the value of these
     # keywords. When used from setup.py, we don't want to import _version.py,
     # so we do it with a regexp instead. This function is not used from
     # _version.py.
     keywords = {}
     try:
-        f = open(versionfile_abs, "r")
-        for line in f.readlines():
-            if line.strip().startswith("git_refnames ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["refnames"] = mo.group(1)
-            if line.strip().startswith("git_full ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["full"] = mo.group(1)
-            if line.strip().startswith("git_date ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["date"] = mo.group(1)
-        f.close()
-    except EnvironmentError:
+        with open(versionfile_abs, "r") as fobj:
+            for line in fobj:
+                if line.strip().startswith("git_refnames ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["refnames"] = mo.group(1)
+                if line.strip().startswith("git_full ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["full"] = mo.group(1)
+                if line.strip().startswith("git_date ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["date"] = mo.group(1)
+    except OSError:
         pass
     return keywords
 
 
 @register_vcs_handler("git", "keywords")
 def git_versions_from_keywords(keywords, tag_prefix, verbose):
     """Get version information from git keywords."""
-    if not keywords:
-        raise NotThisMethod("no keywords at all, weird")
+    if "refnames" not in keywords:
+        raise NotThisMethod("Short version file found")
     date = keywords.get("date")
     if date is not None:
+        # Use only the last line.  Previous lines may contain GPG signature
+        # information.
+        date = date.splitlines()[-1]
+
         # git-2.2.0 added "%%cI", which expands to an ISO-8601 -compliant
         # datestamp. However we prefer "%%ci" (which expands to an "ISO-8601
         # -like" string, which we must then edit to make compliant), because
         # it's been around since git-1.5.3, and it's too difficult to
         # discover which version we're using, or to work around using an
         # older one.
         date = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
     refnames = keywords["refnames"].strip()
     if refnames.startswith("$Format"):
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
-    refs = set([r.strip() for r in refnames.strip("()").split(",")])
+    refs = {r.strip() for r in refnames.strip("()").split(",")}
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = set([r[len(TAG):] for r in refs if r.startswith(TAG)])
+    tags = {r[len(TAG):] for r in refs if r.startswith(TAG)}
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %%d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = set([r for r in refs if re.search(r'\d', r)])
+        tags = {r for r in refs if re.search(r'\d', r)}
         if verbose:
             print("discarding '%%s', no digits" %% ",".join(refs - tags))
     if verbose:
         print("likely tags: %%s" %% ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
             r = ref[len(tag_prefix):]
+            # Filter out refs that exactly match prefix or that don't start
+            # with a number once the prefix is stripped (mostly a concern
+            # when prefix is '')
+            if not re.match(r'\d', r):
+                continue
             if verbose:
                 print("picking %%s" %% r)
             return {"version": r,
                     "full-revisionid": keywords["full"].strip(),
                     "dirty": False, "error": None,
                     "date": date}
     # no suitable tags, so version is "0+unknown", but full hex is still there
@@ -630,52 +699,92 @@
         print("no suitable tags, using unknown + full revision id")
     return {"version": "0+unknown",
             "full-revisionid": keywords["full"].strip(),
             "dirty": False, "error": "no suitable tags", "date": None}
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
-def git_pieces_from_vcs(tag_prefix, root, verbose, run_command=run_command):
+def git_pieces_from_vcs(tag_prefix, root, verbose, runner=run_command):
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
 
-    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                          hide_stderr=True)
+    # GIT_DIR can interfere with correct operation of Versioneer.
+    # It may be intended to be passed to the Versioneer-versioned project,
+    # but that should not change where we get our version from.
+    env = os.environ.copy()
+    env.pop("GIT_DIR", None)
+    runner = functools.partial(runner, env=env)
+
+    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
+                   hide_stderr=not verbose)
     if rc != 0:
         if verbose:
             print("Directory %%s not under git control" %% root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = run_command(GITS, ["describe", "--tags", "--dirty",
-                                          "--always", "--long",
-                                          "--match", "%%s*" %% tag_prefix],
-                                   cwd=root)
+    describe_out, rc = runner(GITS, [
+        "describe", "--tags", "--dirty", "--always", "--long",
+        "--match", f"{tag_prefix}[[:digit:]]*"
+    ], cwd=root)
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
-    full_out, rc = run_command(GITS, ["rev-parse", "HEAD"], cwd=root)
+    full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
     full_out = full_out.strip()
 
     pieces = {}
     pieces["long"] = full_out
     pieces["short"] = full_out[:7]  # maybe improved later
     pieces["error"] = None
 
+    branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"],
+                             cwd=root)
+    # --abbrev-ref was added in git-1.6.3
+    if rc != 0 or branch_name is None:
+        raise NotThisMethod("'git rev-parse --abbrev-ref' returned error")
+    branch_name = branch_name.strip()
+
+    if branch_name == "HEAD":
+        # If we aren't exactly on a branch, pick a branch which represents
+        # the current commit. If all else fails, we are on a branchless
+        # commit.
+        branches, rc = runner(GITS, ["branch", "--contains"], cwd=root)
+        # --contains was added in git-1.5.4
+        if rc != 0 or branches is None:
+            raise NotThisMethod("'git branch --contains' returned error")
+        branches = branches.split("\n")
+
+        # Remove the first line if we're running detached
+        if "(" in branches[0]:
+            branches.pop(0)
+
+        # Strip off the leading "* " from the list of branches.
+        branches = [branch[2:] for branch in branches]
+        if "master" in branches:
+            branch_name = "master"
+        elif not branches:
+            branch_name = None
+        else:
+            # Pick the first branch that is returned. Good or bad.
+            branch_name = branches[0]
+
+    pieces["branch"] = branch_name
+
     # parse describe_out. It will be like TAG-NUM-gHEX[-dirty] or HEX[-dirty]
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
@@ -684,15 +793,15 @@
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
         mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
         if not mo:
-            # unparseable. Maybe git-describe is misbehaving?
+            # unparsable. Maybe git-describe is misbehaving?
             pieces["error"] = ("unable to parse git-describe output: '%%s'"
                                %% describe_out)
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
@@ -709,21 +818,22 @@
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"],
-                                    cwd=root)
-        pieces["distance"] = int(count_out)  # total number of commits
+        out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
+        pieces["distance"] = len(out.split())  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
-    date = run_command(GITS, ["show", "-s", "--format=%%ci", "HEAD"],
-                       cwd=root)[0].strip()
+    date = runner(GITS, ["show", "-s", "--format=%%ci", "HEAD"], cwd=root)[0].strip()
+    # Use only the last line.  Previous lines may contain GPG signature
+    # information.
+    date = date.splitlines()[-1]
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
 def plus_or_dot(pieces):
     """Return a + if we don't already have one, else return a ."""
@@ -753,27 +863,75 @@
         rendered = "0+untagged.%%d.g%%s" %% (pieces["distance"],
                                           pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_pre(pieces):
-    """TAG[.post.devDISTANCE] -- No -dirty.
+def render_pep440_branch(pieces):
+    """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
+
+    The ".dev0" means not master branch. Note that .dev0 sorts backwards
+    (a feature branch will appear "older" than the master branch).
 
     Exceptions:
-    1: no tags. 0.post.devDISTANCE
+    1: no tags. 0[.dev0]+untagged.DISTANCE.gHEX[.dirty]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "%%d.g%%s" %% (pieces["distance"], pieces["short"])
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0"
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+untagged.%%d.g%%s" %% (pieces["distance"],
+                                          pieces["short"])
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
+def pep440_split_post(ver):
+    """Split pep440 version string at the post-release segment.
+
+    Returns the release segments before the post-release and the
+    post-release version number (or -1 if no post-release segment is present).
+    """
+    vc = str.split(ver, ".post")
+    return vc[0], int(vc[1] or 0) if len(vc) == 2 else None
+
+
+def render_pep440_pre(pieces):
+    """TAG[.postN.devDISTANCE] -- No -dirty.
+
+    Exceptions:
+    1: no tags. 0.post0.devDISTANCE
+    """
+    if pieces["closest-tag"]:
         if pieces["distance"]:
-            rendered += ".post.dev%%d" %% pieces["distance"]
+            # update the post release segment
+            tag_version, post_version = pep440_split_post(pieces["closest-tag"])
+            rendered = tag_version
+            if post_version is not None:
+                rendered += ".post%%d.dev%%d" %% (post_version + 1, pieces["distance"])
+            else:
+                rendered += ".post0.dev%%d" %% (pieces["distance"])
+        else:
+            # no commits, use the tag as the version
+            rendered = pieces["closest-tag"]
     else:
         # exception #1
-        rendered = "0.post.dev%%d" %% pieces["distance"]
+        rendered = "0.post0.dev%%d" %% pieces["distance"]
     return rendered
 
 
 def render_pep440_post(pieces):
     """TAG[.postDISTANCE[.dev0]+gHEX] .
 
     The ".dev0" means dirty. Note that .dev0 sorts backwards
@@ -796,20 +954,49 @@
         rendered = "0.post%%d" %% pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
         rendered += "+g%%s" %% pieces["short"]
     return rendered
 
 
+def render_pep440_post_branch(pieces):
+    """TAG[.postDISTANCE[.dev0]+gHEX[.dirty]] .
+
+    The ".dev0" means not master branch.
+
+    Exceptions:
+    1: no tags. 0.postDISTANCE[.dev0]+gHEX[.dirty]
+    """
+    if pieces["closest-tag"]:
+        rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            rendered += ".post%%d" %% pieces["distance"]
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "g%%s" %% pieces["short"]
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0.post%%d" %% pieces["distance"]
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+g%%s" %% pieces["short"]
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
 def render_pep440_old(pieces):
     """TAG[.postDISTANCE[.dev0]] .
 
     The ".dev0" means dirty.
 
-    Eexceptions:
+    Exceptions:
     1: no tags. 0.postDISTANCE[.dev0]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
         if pieces["distance"] or pieces["dirty"]:
             rendered += ".post%%d" %% pieces["distance"]
             if pieces["dirty"]:
@@ -872,18 +1059,22 @@
                 "date": None}
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
+    elif style == "pep440-branch":
+        rendered = render_pep440_branch(pieces)
     elif style == "pep440-pre":
         rendered = render_pep440_pre(pieces)
     elif style == "pep440-post":
         rendered = render_pep440_post(pieces)
+    elif style == "pep440-post-branch":
+        rendered = render_pep440_post_branch(pieces)
     elif style == "pep440-old":
         rendered = render_pep440_old(pieces)
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
@@ -911,15 +1102,15 @@
         pass
 
     try:
         root = os.path.realpath(__file__)
         # versionfile_source is the relative path from the top of the source
         # tree (where the .git directory might live) to this file. Invert
         # this to find the root from __file__.
-        for i in cfg.versionfile_source.split('/'):
+        for _ in cfg.versionfile_source.split('/'):
             root = os.path.dirname(root)
     except NameError:
         return {"version": "0+unknown", "full-revisionid": None,
                 "dirty": None,
                 "error": "unable to find root of source tree",
                 "date": None}
 
@@ -946,75 +1137,83 @@
     """Extract version information from the given file."""
     # the code embedded in _version.py can just fetch the value of these
     # keywords. When used from setup.py, we don't want to import _version.py,
     # so we do it with a regexp instead. This function is not used from
     # _version.py.
     keywords = {}
     try:
-        f = open(versionfile_abs, "r")
-        for line in f.readlines():
-            if line.strip().startswith("git_refnames ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["refnames"] = mo.group(1)
-            if line.strip().startswith("git_full ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["full"] = mo.group(1)
-            if line.strip().startswith("git_date ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["date"] = mo.group(1)
-        f.close()
-    except EnvironmentError:
+        with open(versionfile_abs, "r") as fobj:
+            for line in fobj:
+                if line.strip().startswith("git_refnames ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["refnames"] = mo.group(1)
+                if line.strip().startswith("git_full ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["full"] = mo.group(1)
+                if line.strip().startswith("git_date ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["date"] = mo.group(1)
+    except OSError:
         pass
     return keywords
 
 
 @register_vcs_handler("git", "keywords")
 def git_versions_from_keywords(keywords, tag_prefix, verbose):
     """Get version information from git keywords."""
-    if not keywords:
-        raise NotThisMethod("no keywords at all, weird")
+    if "refnames" not in keywords:
+        raise NotThisMethod("Short version file found")
     date = keywords.get("date")
     if date is not None:
+        # Use only the last line.  Previous lines may contain GPG signature
+        # information.
+        date = date.splitlines()[-1]
+
         # git-2.2.0 added "%cI", which expands to an ISO-8601 -compliant
         # datestamp. However we prefer "%ci" (which expands to an "ISO-8601
         # -like" string, which we must then edit to make compliant), because
         # it's been around since git-1.5.3, and it's too difficult to
         # discover which version we're using, or to work around using an
         # older one.
         date = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
     refnames = keywords["refnames"].strip()
     if refnames.startswith("$Format"):
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
-    refs = set([r.strip() for r in refnames.strip("()").split(",")])
+    refs = {r.strip() for r in refnames.strip("()").split(",")}
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = set([r[len(TAG):] for r in refs if r.startswith(TAG)])
+    tags = {r[len(TAG):] for r in refs if r.startswith(TAG)}
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = set([r for r in refs if re.search(r'\d', r)])
+        tags = {r for r in refs if re.search(r'\d', r)}
         if verbose:
             print("discarding '%s', no digits" % ",".join(refs - tags))
     if verbose:
         print("likely tags: %s" % ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
             r = ref[len(tag_prefix):]
+            # Filter out refs that exactly match prefix or that don't start
+            # with a number once the prefix is stripped (mostly a concern
+            # when prefix is '')
+            if not re.match(r'\d', r):
+                continue
             if verbose:
                 print("picking %s" % r)
             return {"version": r,
                     "full-revisionid": keywords["full"].strip(),
                     "dirty": False, "error": None,
                     "date": date}
     # no suitable tags, so version is "0+unknown", but full hex is still there
@@ -1022,52 +1221,92 @@
         print("no suitable tags, using unknown + full revision id")
     return {"version": "0+unknown",
             "full-revisionid": keywords["full"].strip(),
             "dirty": False, "error": "no suitable tags", "date": None}
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
-def git_pieces_from_vcs(tag_prefix, root, verbose, run_command=run_command):
+def git_pieces_from_vcs(tag_prefix, root, verbose, runner=run_command):
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
 
-    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                          hide_stderr=True)
+    # GIT_DIR can interfere with correct operation of Versioneer.
+    # It may be intended to be passed to the Versioneer-versioned project,
+    # but that should not change where we get our version from.
+    env = os.environ.copy()
+    env.pop("GIT_DIR", None)
+    runner = functools.partial(runner, env=env)
+
+    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
+                   hide_stderr=not verbose)
     if rc != 0:
         if verbose:
             print("Directory %s not under git control" % root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = run_command(GITS, ["describe", "--tags", "--dirty",
-                                          "--always", "--long",
-                                          "--match", "%s*" % tag_prefix],
-                                   cwd=root)
+    describe_out, rc = runner(GITS, [
+        "describe", "--tags", "--dirty", "--always", "--long",
+        "--match", f"{tag_prefix}[[:digit:]]*"
+    ], cwd=root)
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
-    full_out, rc = run_command(GITS, ["rev-parse", "HEAD"], cwd=root)
+    full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
     full_out = full_out.strip()
 
     pieces = {}
     pieces["long"] = full_out
     pieces["short"] = full_out[:7]  # maybe improved later
     pieces["error"] = None
 
+    branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"],
+                             cwd=root)
+    # --abbrev-ref was added in git-1.6.3
+    if rc != 0 or branch_name is None:
+        raise NotThisMethod("'git rev-parse --abbrev-ref' returned error")
+    branch_name = branch_name.strip()
+
+    if branch_name == "HEAD":
+        # If we aren't exactly on a branch, pick a branch which represents
+        # the current commit. If all else fails, we are on a branchless
+        # commit.
+        branches, rc = runner(GITS, ["branch", "--contains"], cwd=root)
+        # --contains was added in git-1.5.4
+        if rc != 0 or branches is None:
+            raise NotThisMethod("'git branch --contains' returned error")
+        branches = branches.split("\n")
+
+        # Remove the first line if we're running detached
+        if "(" in branches[0]:
+            branches.pop(0)
+
+        # Strip off the leading "* " from the list of branches.
+        branches = [branch[2:] for branch in branches]
+        if "master" in branches:
+            branch_name = "master"
+        elif not branches:
+            branch_name = None
+        else:
+            # Pick the first branch that is returned. Good or bad.
+            branch_name = branches[0]
+
+    pieces["branch"] = branch_name
+
     # parse describe_out. It will be like TAG-NUM-gHEX[-dirty] or HEX[-dirty]
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
@@ -1076,15 +1315,15 @@
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
         mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
         if not mo:
-            # unparseable. Maybe git-describe is misbehaving?
+            # unparsable. Maybe git-describe is misbehaving?
             pieces["error"] = ("unable to parse git-describe output: '%s'"
                                % describe_out)
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
@@ -1101,91 +1340,91 @@
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"],
-                                    cwd=root)
-        pieces["distance"] = int(count_out)  # total number of commits
+        out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
+        pieces["distance"] = len(out.split())  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
-    date = run_command(GITS, ["show", "-s", "--format=%ci", "HEAD"],
-                       cwd=root)[0].strip()
+    date = runner(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[0].strip()
+    # Use only the last line.  Previous lines may contain GPG signature
+    # information.
+    date = date.splitlines()[-1]
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
-def do_vcs_install(manifest_in, versionfile_source, ipy):
+def do_vcs_install(versionfile_source, ipy):
     """Git-specific installation logic for Versioneer.
 
     For Git, this means creating/changing .gitattributes to mark _version.py
     for export-subst keyword substitution.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
-    files = [manifest_in, versionfile_source]
+    files = [versionfile_source]
     if ipy:
         files.append(ipy)
-    try:
-        me = __file__
-        if me.endswith(".pyc") or me.endswith(".pyo"):
-            me = os.path.splitext(me)[0] + ".py"
-        versioneer_file = os.path.relpath(me)
-    except NameError:
-        versioneer_file = "versioneer.py"
-    files.append(versioneer_file)
+    if "VERSIONEER_PEP518" not in globals():
+        try:
+            my_path = __file__
+            if my_path.endswith((".pyc", ".pyo")):
+                my_path = os.path.splitext(my_path)[0] + ".py"
+            versioneer_file = os.path.relpath(my_path)
+        except NameError:
+            versioneer_file = "versioneer.py"
+        files.append(versioneer_file)
     present = False
     try:
-        f = open(".gitattributes", "r")
-        for line in f.readlines():
-            if line.strip().startswith(versionfile_source):
-                if "export-subst" in line.strip().split()[1:]:
-                    present = True
-        f.close()
-    except EnvironmentError:
+        with open(".gitattributes", "r") as fobj:
+            for line in fobj:
+                if line.strip().startswith(versionfile_source):
+                    if "export-subst" in line.strip().split()[1:]:
+                        present = True
+                        break
+    except OSError:
         pass
     if not present:
-        f = open(".gitattributes", "a+")
-        f.write("%s export-subst\n" % versionfile_source)
-        f.close()
+        with open(".gitattributes", "a+") as fobj:
+            fobj.write(f"{versionfile_source} export-subst\n")
         files.append(".gitattributes")
     run_command(GITS, ["add", "--"] + files)
 
 
 def versions_from_parentdir(parentdir_prefix, root, verbose):
     """Try to determine the version from the parent directory name.
 
     Source tarballs conventionally unpack into a directory that includes both
     the project name and a version string. We will also support searching up
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
 
-    for i in range(3):
+    for _ in range(3):
         dirname = os.path.basename(root)
         if dirname.startswith(parentdir_prefix):
             return {"version": dirname[len(parentdir_prefix):],
                     "full-revisionid": None,
                     "dirty": False, "error": None, "date": None}
-        else:
-            rootdirs.append(root)
-            root = os.path.dirname(root)  # up a level
+        rootdirs.append(root)
+        root = os.path.dirname(root)  # up a level
 
     if verbose:
         print("Tried directories %s but none started with prefix %s" %
               (str(rootdirs), parentdir_prefix))
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 SHORT_VERSION_PY = """
-# This file was generated by 'versioneer.py' (0.18) from
+# This file was generated by 'versioneer.py' (0.28) from
 # revision-control system data, or from the parent directory name of an
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
@@ -1199,15 +1438,15 @@
 
 
 def versions_from_file(filename):
     """Try to determine the version from _version.py if present."""
     try:
         with open(filename) as f:
             contents = f.read()
-    except EnvironmentError:
+    except OSError:
         raise NotThisMethod("unable to read _version.py")
     mo = re.search(r"version_json = '''\n(.*)'''  # END VERSION_JSON",
                    contents, re.M | re.S)
     if not mo:
         mo = re.search(r"version_json = '''\r\n(.*)'''  # END VERSION_JSON",
                        contents, re.M | re.S)
     if not mo:
@@ -1254,27 +1493,75 @@
         rendered = "0+untagged.%d.g%s" % (pieces["distance"],
                                           pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_pre(pieces):
-    """TAG[.post.devDISTANCE] -- No -dirty.
+def render_pep440_branch(pieces):
+    """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
+
+    The ".dev0" means not master branch. Note that .dev0 sorts backwards
+    (a feature branch will appear "older" than the master branch).
 
     Exceptions:
-    1: no tags. 0.post.devDISTANCE
+    1: no tags. 0[.dev0]+untagged.DISTANCE.gHEX[.dirty]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "%d.g%s" % (pieces["distance"], pieces["short"])
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0"
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+untagged.%d.g%s" % (pieces["distance"],
+                                          pieces["short"])
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
+def pep440_split_post(ver):
+    """Split pep440 version string at the post-release segment.
+
+    Returns the release segments before the post-release and the
+    post-release version number (or -1 if no post-release segment is present).
+    """
+    vc = str.split(ver, ".post")
+    return vc[0], int(vc[1] or 0) if len(vc) == 2 else None
+
+
+def render_pep440_pre(pieces):
+    """TAG[.postN.devDISTANCE] -- No -dirty.
+
+    Exceptions:
+    1: no tags. 0.post0.devDISTANCE
+    """
+    if pieces["closest-tag"]:
         if pieces["distance"]:
-            rendered += ".post.dev%d" % pieces["distance"]
+            # update the post release segment
+            tag_version, post_version = pep440_split_post(pieces["closest-tag"])
+            rendered = tag_version
+            if post_version is not None:
+                rendered += ".post%d.dev%d" % (post_version + 1, pieces["distance"])
+            else:
+                rendered += ".post0.dev%d" % (pieces["distance"])
+        else:
+            # no commits, use the tag as the version
+            rendered = pieces["closest-tag"]
     else:
         # exception #1
-        rendered = "0.post.dev%d" % pieces["distance"]
+        rendered = "0.post0.dev%d" % pieces["distance"]
     return rendered
 
 
 def render_pep440_post(pieces):
     """TAG[.postDISTANCE[.dev0]+gHEX] .
 
     The ".dev0" means dirty. Note that .dev0 sorts backwards
@@ -1297,20 +1584,49 @@
         rendered = "0.post%d" % pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
         rendered += "+g%s" % pieces["short"]
     return rendered
 
 
+def render_pep440_post_branch(pieces):
+    """TAG[.postDISTANCE[.dev0]+gHEX[.dirty]] .
+
+    The ".dev0" means not master branch.
+
+    Exceptions:
+    1: no tags. 0.postDISTANCE[.dev0]+gHEX[.dirty]
+    """
+    if pieces["closest-tag"]:
+        rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            rendered += ".post%d" % pieces["distance"]
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "g%s" % pieces["short"]
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0.post%d" % pieces["distance"]
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+g%s" % pieces["short"]
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
 def render_pep440_old(pieces):
     """TAG[.postDISTANCE[.dev0]] .
 
     The ".dev0" means dirty.
 
-    Eexceptions:
+    Exceptions:
     1: no tags. 0.postDISTANCE[.dev0]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
         if pieces["distance"] or pieces["dirty"]:
             rendered += ".post%d" % pieces["distance"]
             if pieces["dirty"]:
@@ -1373,18 +1689,22 @@
                 "date": None}
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
+    elif style == "pep440-branch":
+        rendered = render_pep440_branch(pieces)
     elif style == "pep440-pre":
         rendered = render_pep440_pre(pieces)
     elif style == "pep440-post":
         rendered = render_pep440_post(pieces)
+    elif style == "pep440-post-branch":
+        rendered = render_pep440_post_branch(pieces)
     elif style == "pep440-old":
         rendered = render_pep440_old(pieces)
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
@@ -1476,35 +1796,39 @@
 
 
 def get_version():
     """Get the short version string for this project."""
     return get_versions()["version"]
 
 
-def get_cmdclass():
-    """Get the custom setuptools/distutils subclasses used by Versioneer."""
+def get_cmdclass(cmdclass=None):
+    """Get the custom setuptools subclasses used by Versioneer.
+
+    If the package uses a different cmdclass (e.g. one from numpy), it
+    should be provide as an argument.
+    """
     if "versioneer" in sys.modules:
         del sys.modules["versioneer"]
         # this fixes the "python setup.py develop" case (also 'install' and
         # 'easy_install .'), in which subdependencies of the main project are
         # built (using setup.py bdist_egg) in the same python process. Assume
         # a main project A and a dependency B, which use different versions
         # of Versioneer. A's setup.py imports A's Versioneer, leaving it in
         # sys.modules by the time B's setup.py is executed, causing B to run
         # with the wrong versioneer. Setuptools wraps the sub-dep builds in a
         # sandbox that restores sys.modules to it's pre-build state, so the
         # parent is protected against the child's "import versioneer". By
         # removing ourselves from sys.modules here, before the child build
         # happens, we protect the child from the parent's versioneer too.
-        # Also see https://github.com/warner/python-versioneer/issues/52
+        # Also see https://github.com/python-versioneer/python-versioneer/issues/52
 
-    cmds = {}
+    cmds = {} if cmdclass is None else cmdclass.copy()
 
-    # we add "version" to both distutils and setuptools
-    from distutils.core import Command
+    # we add "version" to setuptools
+    from setuptools import Command
 
     class cmd_version(Command):
         description = "report generated version string"
         user_options = []
         boolean_options = []
 
         def initialize_options(self):
@@ -1519,50 +1843,89 @@
             print(" full-revisionid: %s" % vers.get("full-revisionid"))
             print(" dirty: %s" % vers.get("dirty"))
             print(" date: %s" % vers.get("date"))
             if vers["error"]:
                 print(" error: %s" % vers["error"])
     cmds["version"] = cmd_version
 
-    # we override "build_py" in both distutils and setuptools
+    # we override "build_py" in setuptools
     #
     # most invocation pathways end up running build_py:
     #  distutils/build -> build_py
     #  distutils/install -> distutils/build ->..
     #  setuptools/bdist_wheel -> distutils/install ->..
     #  setuptools/bdist_egg -> distutils/install_lib -> build_py
     #  setuptools/install -> bdist_egg ->..
     #  setuptools/develop -> ?
     #  pip install:
     #   copies source tree to a tempdir before running egg_info/etc
     #   if .git isn't copied too, 'git describe' will fail
     #   then does setup.py bdist_wheel, or sometimes setup.py install
     #  setup.py egg_info -> ?
 
+    # pip install -e . and setuptool/editable_wheel will invoke build_py
+    # but the build_py command is not expected to copy any files.
+
     # we override different "build_py" commands for both environments
-    if "setuptools" in sys.modules:
-        from setuptools.command.build_py import build_py as _build_py
+    if 'build_py' in cmds:
+        _build_py = cmds['build_py']
     else:
-        from distutils.command.build_py import build_py as _build_py
+        from setuptools.command.build_py import build_py as _build_py
 
     class cmd_build_py(_build_py):
         def run(self):
             root = get_root()
             cfg = get_config_from_root(root)
             versions = get_versions()
             _build_py.run(self)
+            if getattr(self, "editable_mode", False):
+                # During editable installs `.py` and data files are
+                # not copied to build_lib
+                return
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
             if cfg.versionfile_build:
                 target_versionfile = os.path.join(self.build_lib,
                                                   cfg.versionfile_build)
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
     cmds["build_py"] = cmd_build_py
 
+    if 'build_ext' in cmds:
+        _build_ext = cmds['build_ext']
+    else:
+        from setuptools.command.build_ext import build_ext as _build_ext
+
+    class cmd_build_ext(_build_ext):
+        def run(self):
+            root = get_root()
+            cfg = get_config_from_root(root)
+            versions = get_versions()
+            _build_ext.run(self)
+            if self.inplace:
+                # build_ext --inplace will only build extensions in
+                # build/lib<..> dir with no _version.py to write to.
+                # As in place builds will already have a _version.py
+                # in the module dir, we do not need to write one.
+                return
+            # now locate _version.py in the new build/ directory and replace
+            # it with an updated value
+            if not cfg.versionfile_build:
+                return
+            target_versionfile = os.path.join(self.build_lib,
+                                              cfg.versionfile_build)
+            if not os.path.exists(target_versionfile):
+                print(f"Warning: {target_versionfile} does not exist, skipping "
+                      "version update. This can happen if you are running build_ext "
+                      "without first running build_py.")
+                return
+            print("UPDATING %s" % target_versionfile)
+            write_to_version_file(target_versionfile, versions)
+    cmds["build_ext"] = cmd_build_ext
+
     if "cx_Freeze" in sys.modules:  # cx_freeze enabled?
         from cx_Freeze.dist import build_exe as _build_exe
         # nczeczulin reports that py2exe won't like the pep440-style string
         # as FILEVERSION, but it can be used for PRODUCTVERSION, e.g.
         # setup(console=[{
         #   "version": versioneer.get_version().split("+", 1)[0], # FILEVERSION
         #   "product_version": versioneer.get_version(),
@@ -1589,17 +1952,17 @@
                              "VERSIONFILE_SOURCE": cfg.versionfile_source,
                              })
         cmds["build_exe"] = cmd_build_exe
         del cmds["build_py"]
 
     if 'py2exe' in sys.modules:  # py2exe enabled?
         try:
-            from py2exe.distutils_buildexe import py2exe as _py2exe  # py3
+            from py2exe.setuptools_buildexe import py2exe as _py2exe
         except ImportError:
-            from py2exe.build_exe import py2exe as _py2exe  # py2
+            from py2exe.distutils_buildexe import py2exe as _py2exe
 
         class cmd_py2exe(_py2exe):
             def run(self):
                 root = get_root()
                 cfg = get_config_from_root(root)
                 versions = get_versions()
                 target_versionfile = cfg.versionfile_source
@@ -1615,19 +1978,56 @@
                              "STYLE": cfg.style,
                              "TAG_PREFIX": cfg.tag_prefix,
                              "PARENTDIR_PREFIX": cfg.parentdir_prefix,
                              "VERSIONFILE_SOURCE": cfg.versionfile_source,
                              })
         cmds["py2exe"] = cmd_py2exe
 
+    # sdist farms its file list building out to egg_info
+    if 'egg_info' in cmds:
+        _egg_info = cmds['egg_info']
+    else:
+        from setuptools.command.egg_info import egg_info as _egg_info
+
+    class cmd_egg_info(_egg_info):
+        def find_sources(self):
+            # egg_info.find_sources builds the manifest list and writes it
+            # in one shot
+            super().find_sources()
+
+            # Modify the filelist and normalize it
+            root = get_root()
+            cfg = get_config_from_root(root)
+            self.filelist.append('versioneer.py')
+            if cfg.versionfile_source:
+                # There are rare cases where versionfile_source might not be
+                # included by default, so we must be explicit
+                self.filelist.append(cfg.versionfile_source)
+            self.filelist.sort()
+            self.filelist.remove_duplicates()
+
+            # The write method is hidden in the manifest_maker instance that
+            # generated the filelist and was thrown away
+            # We will instead replicate their final normalization (to unicode,
+            # and POSIX-style paths)
+            from setuptools import unicode_utils
+            normalized = [unicode_utils.filesys_decode(f).replace(os.sep, '/')
+                          for f in self.filelist.files]
+
+            manifest_filename = os.path.join(self.egg_info, 'SOURCES.txt')
+            with open(manifest_filename, 'w') as fobj:
+                fobj.write('\n'.join(normalized))
+
+    cmds['egg_info'] = cmd_egg_info
+
     # we override different "sdist" commands for both environments
-    if "setuptools" in sys.modules:
-        from setuptools.command.sdist import sdist as _sdist
+    if 'sdist' in cmds:
+        _sdist = cmds['sdist']
     else:
-        from distutils.command.sdist import sdist as _sdist
+        from setuptools.command.sdist import sdist as _sdist
 
     class cmd_sdist(_sdist):
         def run(self):
             versions = get_versions()
             self._versioneer_generated_versions = versions
             # unless we update this, the command will keep using the old
             # version
@@ -1683,29 +2083,34 @@
 #versionfile_source =
 #versionfile_build =
 #tag_prefix =
 #parentdir_prefix =
 
 """
 
-INIT_PY_SNIPPET = """
+OLD_SNIPPET = """
 from ._version import get_versions
 __version__ = get_versions()['version']
 del get_versions
 """
 
+INIT_PY_SNIPPET = """
+from . import {0}
+__version__ = {0}.get_versions()['version']
+"""
+
 
 def do_setup():
-    """Main VCS-independent setup function for installing Versioneer."""
+    """Do main VCS-independent setup function for installing Versioneer."""
     root = get_root()
     try:
         cfg = get_config_from_root(root)
-    except (EnvironmentError, configparser.NoSectionError,
+    except (OSError, configparser.NoSectionError,
             configparser.NoOptionError) as e:
-        if isinstance(e, (EnvironmentError, configparser.NoSectionError)):
+        if isinstance(e, (OSError, configparser.NoSectionError)):
             print("Adding sample versioneer config to setup.cfg",
                   file=sys.stderr)
             with open(os.path.join(root, "setup.cfg"), "a") as f:
                 f.write(SAMPLE_CONFIG)
         print(CONFIG_ERROR, file=sys.stderr)
         return 1
 
@@ -1721,62 +2126,36 @@
 
     ipy = os.path.join(os.path.dirname(cfg.versionfile_source),
                        "__init__.py")
     if os.path.exists(ipy):
         try:
             with open(ipy, "r") as f:
                 old = f.read()
-        except EnvironmentError:
+        except OSError:
             old = ""
-        if INIT_PY_SNIPPET not in old:
+        module = os.path.splitext(os.path.basename(cfg.versionfile_source))[0]
+        snippet = INIT_PY_SNIPPET.format(module)
+        if OLD_SNIPPET in old:
+            print(" replacing boilerplate in %s" % ipy)
+            with open(ipy, "w") as f:
+                f.write(old.replace(OLD_SNIPPET, snippet))
+        elif snippet not in old:
             print(" appending to %s" % ipy)
             with open(ipy, "a") as f:
-                f.write(INIT_PY_SNIPPET)
+                f.write(snippet)
         else:
             print(" %s unmodified" % ipy)
     else:
         print(" %s doesn't exist, ok" % ipy)
         ipy = None
 
-    # Make sure both the top-level "versioneer.py" and versionfile_source
-    # (PKG/_version.py, used by runtime code) are in MANIFEST.in, so
-    # they'll be copied into source distributions. Pip won't be able to
-    # install the package without this.
-    manifest_in = os.path.join(root, "MANIFEST.in")
-    simple_includes = set()
-    try:
-        with open(manifest_in, "r") as f:
-            for line in f:
-                if line.startswith("include "):
-                    for include in line.split()[1:]:
-                        simple_includes.add(include)
-    except EnvironmentError:
-        pass
-    # That doesn't cover everything MANIFEST.in can do
-    # (http://docs.python.org/2/distutils/sourcedist.html#commands), so
-    # it might give some false negatives. Appending redundant 'include'
-    # lines is safe, though.
-    if "versioneer.py" not in simple_includes:
-        print(" appending 'versioneer.py' to MANIFEST.in")
-        with open(manifest_in, "a") as f:
-            f.write("include versioneer.py\n")
-    else:
-        print(" 'versioneer.py' already in MANIFEST.in")
-    if cfg.versionfile_source not in simple_includes:
-        print(" appending versionfile_source ('%s') to MANIFEST.in" %
-              cfg.versionfile_source)
-        with open(manifest_in, "a") as f:
-            f.write("include %s\n" % cfg.versionfile_source)
-    else:
-        print(" versionfile_source already in MANIFEST.in")
-
     # Make VCS-specific changes. For git, this means creating/changing
     # .gitattributes to mark _version.py for export-subst keyword
     # substitution.
-    do_vcs_install(manifest_in, cfg.versionfile_source, ipy)
+    do_vcs_install(cfg.versionfile_source, ipy)
     return 0
 
 
 def scan_setup_py():
     """Validate the contents of setup.py against Versioneer's expectations."""
     found = set()
     setters = False
@@ -1809,14 +2188,18 @@
         print("'versioneer.versionfile_source = ' . This configuration")
         print("now lives in setup.cfg, and should be removed from setup.py")
         print("")
         errors += 1
     return errors
 
 
+def setup_command():
+    """Set up Versioneer and exit with appropriate error code."""
+    errors = do_setup()
+    errors += scan_setup_py()
+    sys.exit(1 if errors else 0)
+
+
 if __name__ == "__main__":
     cmd = sys.argv[1]
     if cmd == "setup":
-        errors = do_setup()
-        errors += scan_setup_py()
-        if errors:
-            sys.exit(1)
+        setup_command()
```

