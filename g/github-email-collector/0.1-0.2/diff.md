# Comparing `tmp/github_email_collector-0.1.tar.gz` & `tmp/github_email_collector-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "github_email_collector-0.1.tar", last modified: Sun May 28 17:45:07 2023, max compression
+gzip compressed data, was "github_email_collector-0.2.tar", last modified: Fri Jun  9 17:43:20 2023, max compression
```

## Comparing `github_email_collector-0.1.tar` & `github_email_collector-0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 17:45:07.474669 github_email_collector-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-28 17:45:07.474669 github_email_collector-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-28 17:45:03.000000 github_email_collector-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 17:45:07.474669 github_email_collector-0.1/github_email_collector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-28 17:45:07.000000 github_email_collector-0.1/github_email_collector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-28 17:45:07.000000 github_email_collector-0.1/github_email_collector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 17:45:07.000000 github_email_collector-0.1/github_email_collector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-28 17:45:07.000000 github_email_collector-0.1/github_email_collector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 17:45:07.000000 github_email_collector-0.1/github_email_collector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 17:45:07.474669 github_email_collector-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-28 17:45:03.000000 github_email_collector-0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:43:20.935842 github_email_collector-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-09 17:43:20.935842 github_email_collector-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-09 17:43:15.000000 github_email_collector-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:43:20.935842 github_email_collector-0.2/github_email_collector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-09 17:43:20.000000 github_email_collector-0.2/github_email_collector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-09 17:43:20.000000 github_email_collector-0.2/github_email_collector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 17:43:20.000000 github_email_collector-0.2/github_email_collector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-09 17:43:20.000000 github_email_collector-0.2/github_email_collector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 17:43:20.000000 github_email_collector-0.2/github_email_collector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 17:43:20.935842 github_email_collector-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-09 17:43:15.000000 github_email_collector-0.2/setup.py
```

### Comparing `github_email_collector-0.1/PKG-INFO` & `github_email_collector-0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 Metadata-Version: 2.1
 Name: github_email_collector
-Version: 0.1
+Version: 0.2
 Summary: Collect email address of users affiliated to a given repository
-Home-page: https://github.com/LucBerge/github-email-collector
+Home-page: https://github.com/LucBerge/github_email_collector
 Author: LucBerge
 Author-email: lucas.bergeron@outlook.fr
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Github Email Collector
 
 Collect the email address of users affiliated to a given repository
 
 ## Installation
+### From PyPi
 
-Download from PyPi:
 ```python
 pip install github-email-collector
 ```
 
+### As a submodule
+
+```
+git submodule add https://github.com/LucBerge/github_email_collector.git
+git submodule update --init
+```
+
 ## Usage
 
 From your python script
 ```python
-from  github_email_collector import EmailCollector
+from github_email_collector import EmailCollector
 
 email_collector = EmailCollector("MY_GITHUB_TOKEN", "owner/repo")
 emails = email_collector.get_emails()
 print(emails)
 ```
```

### Comparing `github_email_collector-0.1/setup.py` & `github_email_collector-0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,17 +10,17 @@
         ] if s != ''
     ]
 
 long_description = open("README.md", "r").read()
 
 setuptools.setup(
     name='github_email_collector',
-    version='0.1',
+    version='0.2',
     author='LucBerge',
     author_email='lucas.bergeron@outlook.fr',
     description="Collect email address of users affiliated to a given repository",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url='https://github.com/LucBerge/github-email-collector',
+    url='https://github.com/LucBerge/github_email_collector',
     packages=setuptools.find_packages(),
     install_requires=requirements
 )
```

