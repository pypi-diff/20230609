# Comparing `tmp/asp_chef_headless-0.1.0.tar.gz` & `tmp/asp_chef_headless-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asp_chef_headless-0.1.0.tar", max compression
+gzip compressed data, was "asp_chef_headless-0.1.1.tar", max compression
```

## Comparing `asp_chef_headless-0.1.0.tar` & `asp_chef_headless-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-06-09 19:16:09.263790 asp_chef_headless-0.1.0/LICENSE
--rw-r--r--   0        0        0        0 2023-06-09 17:38:58.650957 asp_chef_headless-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-09 17:38:58.650957 asp_chef_headless-0.1.0/asp_chef_headless/__init__.py
--rw-r--r--   0        0        0      107 2023-06-09 17:50:50.186917 asp_chef_headless-0.1.0/asp_chef_headless/__main__.py
--rwxr-xr-x   0        0        0     3603 2023-06-09 19:12:13.861697 asp_chef_headless-0.1.0/asp_chef_headless/cli.py
--rw-r--r--   0        0        0      413 2023-06-09 17:51:31.997404 asp_chef_headless-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      704 1970-01-01 00:00:00.000000 asp_chef_headless-0.1.0/setup.py
--rw-r--r--   0        0        0      524 1970-01-01 00:00:00.000000 asp_chef_headless-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-09 19:16:09.263790 asp_chef_headless-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2659 2023-06-09 19:54:33.372517 asp_chef_headless-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-09 17:38:58.650957 asp_chef_headless-0.1.1/asp_chef_headless/__init__.py
+-rw-r--r--   0        0        0      107 2023-06-09 17:50:50.186917 asp_chef_headless-0.1.1/asp_chef_headless/__main__.py
+-rwxr-xr-x   0        0        0     3608 2023-06-09 19:38:01.222043 asp_chef_headless-0.1.1/asp_chef_headless/cli.py
+-rw-r--r--   0        0        0      413 2023-06-09 19:54:33.348518 asp_chef_headless-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3417 1970-01-01 00:00:00.000000 asp_chef_headless-0.1.1/setup.py
+-rw-r--r--   0        0        0     3183 1970-01-01 00:00:00.000000 asp_chef_headless-0.1.1/PKG-INFO
```

### Comparing `asp_chef_headless-0.1.0/LICENSE` & `asp_chef_headless-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asp_chef_headless-0.1.0/asp_chef_headless/cli.py` & `asp_chef_headless-0.1.1/asp_chef_headless/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typer
 from dumbo_utils.console import console
 from dumbo_utils.url import compress_object_for_url
 from dumbo_utils.validation import validate
 from playwright.sync_api import sync_playwright, Playwright
 
 
-class Browser(Enum):
+class Browser(str, Enum):
     CHROMIUM = "chromium"
     # CHROME = "chrome"
     # CHROME_BETA = "chrome-beta"
     # MS_EDGE = "msedge"
     # MS_EDGE_BETA = "msedge-beta"
     # MS_EDGE_DEV = "msedge-dev"
     FIREFOX = "firefox"
```

