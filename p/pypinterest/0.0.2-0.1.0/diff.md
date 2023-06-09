# Comparing `tmp/pypinterest-0.0.2.tar.gz` & `tmp/pypinterest-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypinterest-0.0.2.tar", last modified: Fri Jun  9 03:49:18 2023, max compression
+gzip compressed data, was "dist\pypinterest-0.1.0.tar", last modified: Fri Jun  9 04:14:44 2023, max compression
```

## Comparing `pypinterest-0.0.2.tar` & `pypinterest-0.1.0.tar`

### file list

```diff
@@ -1,12 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 03:49:18.621223 pypinterest-0.0.2/
--rw-rw-rw-   0        0        0    11553 2023-06-04 07:18:01.000000 pypinterest-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      283 2023-06-09 03:49:18.621223 pypinterest-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-04 07:24:30.000000 pypinterest-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 03:49:18.612769 pypinterest-0.0.2/pypinterest.egg-info/
--rw-rw-rw-   0        0        0      283 2023-06-09 03:49:18.000000 pypinterest-0.0.2/pypinterest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2023-06-09 03:49:18.000000 pypinterest-0.0.2/pypinterest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 03:49:18.000000 pypinterest-0.0.2/pypinterest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      101 2023-06-09 03:49:18.000000 pypinterest-0.0.2/pypinterest.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 03:49:18.000000 pypinterest-0.0.2/pypinterest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 03:49:18.621223 pypinterest-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1819 2023-06-04 07:25:38.000000 pypinterest-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 04:14:44.000000 pypinterest-0.1.0/
+-rw-rw-rw-   0        0        0    11553 2023-06-04 07:18:01.000000 pypinterest-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      315 2023-06-09 04:14:44.000000 pypinterest-0.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-09 04:14:44.000000 pypinterest-0.1.0/pypinterest.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-09 04:14:44.000000 pypinterest-0.1.0/pypinterest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      315 2023-06-09 04:14:44.000000 pypinterest-0.1.0/pypinterest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      166 2023-06-09 04:14:44.000000 pypinterest-0.1.0/pypinterest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 04:14:44.000000 pypinterest-0.1.0/pypinterest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-06-04 07:24:30.000000 pypinterest-0.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-09 04:14:44.000000 pypinterest-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1684 2023-06-09 04:10:50.000000 pypinterest-0.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pypinterest-0.0.2/LICENSE` & `pypinterest-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pypinterest-0.0.2/setup.py` & `pypinterest-0.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,47 +9,41 @@
 
 def _get_test_version():
     return datetime.today().strftime('%m%d%Y%H%M%S')
 
 
 def _get_prod_version():
     module = {}
-    with open(os.path.join(package_root, "utils/version.py"), encoding='UTF-8') as fp:
+    with open(os.path.join(package_root, "pypinterest/utils/version.py"), encoding='UTF-8') as fp:
         exec(fp.read(), module)  # pylint: disable=exec-used
     return module.get("__version__")
 
 
 _IS_TEST_BUILD = os.environ.get("IS_TEST_BUILD", 0)
 
-REQUIRES = [
-  "urllib3==1.26.12",
-  "python-dateutil",
-  "python-dotenv==0.20.0",
-  "six==1.16.0",
-  "Pinterest-Generated-Client==0.1.7"
-]
+REQUIRES = []
 
 long_description = (Path(__file__).parent / "README.md").read_text()
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 __version__ = None
 
 if _IS_TEST_BUILD:
     print("* Test build enable")
     __version__ = _get_test_version()
 else:
-    __version__ = _get_prod_version()
+    __version__ = "0.0.3"
 
 if __version__ is None:
     raise ValueError("Version is not defined")
 
 setup(
     name="pypinterest",
     description="Pinterest API",
-    version=__version__,
+    version= "0.1.0",
     author="Techfarm",
     author_email="tamilcomway@gmail.com",
     url="https://github.com/piriyaraj/pypinterest",
     install_requires=REQUIRES,
     include_package_data=True,
     packages=find_namespace_packages(
         include=['pinterest.*', 'pinterest', 'pinterest.version', 'pinterest.config'],
```

