# Comparing `tmp/sr2t-0bs1d1an-0.0.8.tar.gz` & `tmp/sr2t-0bs1d1an-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sr2t-0bs1d1an-0.0.8.tar", last modified: Mon Dec 16 12:23:16 2019, max compression
+gzip compressed data, was "dist/sr2t-0bs1d1an-0.0.9.tar", last modified: Mon Dec 23 11:46:17 2019, max compression
```

## Comparing `sr2t-0bs1d1an-0.0.8.tar` & `sr2t-0bs1d1an-0.0.9.tar`

### file list

```diff
@@ -1,49 +1,54 @@
-drwxr-xr-x   0 gukroon   (1000) users      (100)        0 2019-12-16 12:23:16.000000 sr2t-0bs1d1an-0.0.8/
-drwxr-xr-x   0 gukroon   (1000) users      (100)        0 2019-12-16 12:23:16.000000 sr2t-0bs1d1an-0.0.8/sr2t/
-drwxr-xr-x   0 gukroon   (1000) users      (100)        0 2019-12-16 12:23:16.000000 sr2t-0bs1d1an-0.0.8/sr2t/parsers/
--rw-r--r--   0 gukroon   (1000) users      (100)     9262 2019-12-16 11:45:44.000000 sr2t-0bs1d1an-0.0.8/sr2t/parsers/testssl.py
--rw-r--r--   0 gukroon   (1000) users      (100)     4649 2019-12-16 11:45:44.000000 sr2t-0bs1d1an-0.0.8/sr2t/parsers/fortify.py
--rw-r--r--   0 gukroon   (1000) users      (100)     2508 2019-12-16 11:45:44.000000 sr2t-0bs1d1an-0.0.8/sr2t/parsers/dirble.py
--rw-r--r--   0 gukroon   (1000) users      (100)        0 2019-12-16 12:08:06.000000 sr2t-0bs1d1an-0.0.8/sr2t/parsers/__init__.py
--rw-r--r--   0 gukroon   (1000) users      (100)    25006 2019-12-16 11:45:44.000000 sr2t-0bs1d1an-0.0.8/sr2t/parsers/nessus.py
--rw-r--r--   0 gukroon   (1000) users      (100)     2271 2019-12-16 11:45:44.000000 sr2t-0bs1d1an-0.0.8/sr2t/parsers/nikto.py
--rw-r--r--   0 gukroon   (1000) users      (100)     2754 2019-12-16 11:45:44.000000 sr2t-0bs1d1an-0.0.8/sr2t/parsers/nmap.py
--rw-r--r--   0 gukroon   (1000) users      (100)        0 2019-12-16 11:45:44.000000 sr2t-0bs1d1an-0.0.8/sr2t/__init__.py
--rwxr-xr-x   0 gukroon   (1000) users      (100)     6567 2019-12-16 12:16:14.000000 sr2t-0bs1d1an-0.0.8/sr2t/sr2t.py
--rw-r--r--   0 gukroon   (1000) users      (100)     1799 2019-12-14 19:28:50.000000 sr2t-0bs1d1an-0.0.8/.gitignore
--rw-r--r--   0 gukroon   (1000) users      (100)      208 2019-12-16 12:16:14.000000 sr2t-0bs1d1an-0.0.8/.gitlab-ci.yml
--rw-r--r--   0 gukroon   (1000) users      (100)    23343 2019-12-16 12:23:16.000000 sr2t-0bs1d1an-0.0.8/PKG-INFO
-drwxr-xr-x   0 gukroon   (1000) users      (100)        0 2019-12-16 12:23:16.000000 sr2t-0bs1d1an-0.0.8/example/
--rw-r--r--   0 gukroon   (1000) users      (100)     6513 2019-12-13 14:19:34.000000 sr2t-0bs1d1an-0.0.8/example/nmap.xlsx
--rw-r--r--   0 gukroon   (1000) users      (100)   111825 2019-12-14 13:49:42.000000 sr2t-0bs1d1an-0.0.8/example/dirble-xlsx.png
--rw-r--r--   0 gukroon   (1000) users      (100)     6779 2019-12-14 12:03:19.000000 sr2t-0bs1d1an-0.0.8/example/dirble.xlsx
--rw-r--r--   0 gukroon   (1000) users      (100)      134 2019-12-14 14:12:00.000000 sr2t-0bs1d1an-0.0.8/example/testssl.csv
--rw-r--r--   0 gukroon   (1000) users      (100)    92856 2019-12-14 13:54:38.000000 sr2t-0bs1d1an-0.0.8/example/nikto-xlsx.png
--rw-r--r--   0 gukroon   (1000) users      (100)    38641 2019-12-14 14:08:32.000000 sr2t-0bs1d1an-0.0.8/example/testssl.json
--rw-r--r--   0 gukroon   (1000) users      (100)    80990 2019-12-13 14:23:18.000000 sr2t-0bs1d1an-0.0.8/example/nmap-xlsx.png
--rwxr-xr-x   0 gukroon   (1000) users      (100)     1853 2019-12-14 13:53:19.000000 sr2t-0bs1d1an-0.0.8/example/nikto.xml
--rw-r--r--   0 gukroon   (1000) users      (100)      508 2019-12-14 13:53:47.000000 sr2t-0bs1d1an-0.0.8/example/nikto.csv
--rw-r--r--   0 gukroon   (1000) users      (100)   152946 2019-12-13 14:44:06.000000 sr2t-0bs1d1an-0.0.8/example/nessus-xlsx-tls.png
--rw-r--r--   0 gukroon   (1000) users      (100)     6668 2019-12-14 14:14:58.000000 sr2t-0bs1d1an-0.0.8/example/testssl.xlsx
--rw-r--r--   0 gukroon   (1000) users      (100)      977 2019-12-14 11:59:41.000000 sr2t-0bs1d1an-0.0.8/example/dirble.xml
--rw-r--r--   0 gukroon   (1000) users      (100)   144709 2019-12-13 14:44:41.000000 sr2t-0bs1d1an-0.0.8/example/nessus-xlsx-x509.png
--rw-r--r--   0 gukroon   (1000) users      (100)   127444 2019-12-13 14:43:12.000000 sr2t-0bs1d1an-0.0.8/example/nessus-xlsx-portscan.png
--rw-r--r--   0 gukroon   (1000) users      (100)   190688 2019-12-13 14:07:30.000000 sr2t-0bs1d1an-0.0.8/example/nessus-xlsx-critical.png
--rw-r--r--   0 gukroon   (1000) users      (100)   271966 2019-12-14 14:20:25.000000 sr2t-0bs1d1an-0.0.8/example/fortify-xlsx.png
--rw-r--r--   0 gukroon   (1000) users      (100)      413 2019-12-14 12:00:09.000000 sr2t-0bs1d1an-0.0.8/example/dirble.csv
--rw-r--r--   0 gukroon   (1000) users      (100)      198 2019-11-22 10:42:12.000000 sr2t-0bs1d1an-0.0.8/example/output.csv
--rw-r--r--   0 gukroon   (1000) users      (100)     6577 2019-12-14 13:54:05.000000 sr2t-0bs1d1an-0.0.8/example/nikto.xlsx
--rw-r--r--   0 gukroon   (1000) users      (100)     9263 2019-11-22 10:42:12.000000 sr2t-0bs1d1an-0.0.8/example/nmap.xml
--rw-r--r--   0 gukroon   (1000) users      (100)    83946 2019-12-14 14:15:29.000000 sr2t-0bs1d1an-0.0.8/example/testssl-xlsx.png
--rw-r--r--   0 gukroon   (1000) users      (100)      720 2019-11-22 10:42:12.000000 sr2t-0bs1d1an-0.0.8/example/output.txt
--rw-r--r--   0 gukroon   (1000) users      (100)    35061 2019-11-22 10:42:12.000000 sr2t-0bs1d1an-0.0.8/LICENSE
--rw-r--r--   0 gukroon   (1000) users      (100)      828 2019-12-16 12:20:06.000000 sr2t-0bs1d1an-0.0.8/setup.py
-drwxr-xr-x   0 gukroon   (1000) users      (100)        0 2019-12-16 12:23:16.000000 sr2t-0bs1d1an-0.0.8/sr2t_0bs1d1an.egg-info/
--rw-r--r--   0 gukroon   (1000) users      (100)      958 2019-12-16 12:23:15.000000 sr2t-0bs1d1an-0.0.8/sr2t_0bs1d1an.egg-info/SOURCES.txt
--rw-r--r--   0 gukroon   (1000) users      (100)    23343 2019-12-16 12:23:15.000000 sr2t-0bs1d1an-0.0.8/sr2t_0bs1d1an.egg-info/PKG-INFO
--rw-r--r--   0 gukroon   (1000) users      (100)        1 2019-12-16 12:23:15.000000 sr2t-0bs1d1an-0.0.8/sr2t_0bs1d1an.egg-info/dependency_links.txt
--rw-r--r--   0 gukroon   (1000) users      (100)       41 2019-12-16 12:23:15.000000 sr2t-0bs1d1an-0.0.8/sr2t_0bs1d1an.egg-info/entry_points.txt
--rw-r--r--   0 gukroon   (1000) users      (100)        5 2019-12-16 12:23:15.000000 sr2t-0bs1d1an-0.0.8/sr2t_0bs1d1an.egg-info/top_level.txt
--rw-r--r--   0 gukroon   (1000) users      (100)       32 2019-12-16 12:23:15.000000 sr2t-0bs1d1an-0.0.8/sr2t_0bs1d1an.egg-info/requires.txt
--rw-r--r--   0 gukroon   (1000) users      (100)    19782 2019-12-16 12:21:39.000000 sr2t-0bs1d1an-0.0.8/README.md
--rw-r--r--   0 gukroon   (1000) users      (100)       38 2019-12-16 12:23:16.000000 sr2t-0bs1d1an-0.0.8/setup.cfg
+drwxr-xr-x   0 gukroon   (1000) users      (100)        0 2019-12-23 11:46:17.000000 sr2t-0bs1d1an-0.0.9/
+drwxr-xr-x   0 gukroon   (1000) users      (100)        0 2019-12-23 11:46:17.000000 sr2t-0bs1d1an-0.0.9/sr2t/
+drwxr-xr-x   0 gukroon   (1000) users      (100)        0 2019-12-23 11:46:17.000000 sr2t-0bs1d1an-0.0.9/sr2t/parsers/
+-rw-r--r--   0 gukroon   (1000) users      (100)     9262 2019-12-16 11:45:44.000000 sr2t-0bs1d1an-0.0.9/sr2t/parsers/testssl.py
+-rw-r--r--   0 gukroon   (1000) users      (100)     4649 2019-12-16 11:45:44.000000 sr2t-0bs1d1an-0.0.9/sr2t/parsers/fortify.py
+-rw-r--r--   0 gukroon   (1000) users      (100)     2508 2019-12-16 11:45:44.000000 sr2t-0bs1d1an-0.0.9/sr2t/parsers/dirble.py
+-rw-r--r--   0 gukroon   (1000) users      (100)        0 2019-12-16 12:08:06.000000 sr2t-0bs1d1an-0.0.9/sr2t/parsers/__init__.py
+-rw-r--r--   0 gukroon   (1000) users      (100)    20720 2019-12-23 11:45:46.000000 sr2t-0bs1d1an-0.0.9/sr2t/parsers/nessus.py
+-rw-r--r--   0 gukroon   (1000) users      (100)     2271 2019-12-16 11:45:44.000000 sr2t-0bs1d1an-0.0.9/sr2t/parsers/nikto.py
+-rw-r--r--   0 gukroon   (1000) users      (100)     2754 2019-12-16 11:45:44.000000 sr2t-0bs1d1an-0.0.9/sr2t/parsers/nmap.py
+-rw-r--r--   0 gukroon   (1000) users      (100)        0 2019-12-16 11:45:44.000000 sr2t-0bs1d1an-0.0.9/sr2t/__init__.py
+-rwxr-xr-x   0 gukroon   (1000) users      (100)     6567 2019-12-16 12:16:14.000000 sr2t-0bs1d1an-0.0.9/sr2t/sr2t.py
+drwxr-xr-x   0 gukroon   (1000) users      (100)        0 2019-12-23 11:46:17.000000 sr2t-0bs1d1an-0.0.9/sr2t/data/
+-rw-r--r--   0 gukroon   (1000) users      (100)      440 2019-12-23 11:34:17.000000 sr2t-0bs1d1an-0.0.9/sr2t/data/tls.yaml
+-rw-r--r--   0 gukroon   (1000) users      (100)     7859 2019-12-23 11:36:54.000000 sr2t-0bs1d1an-0.0.9/sr2t/data/autoclassify.yaml
+-rw-r--r--   0 gukroon   (1000) users      (100)      214 2019-12-23 11:21:59.000000 sr2t-0bs1d1an-0.0.9/sr2t/data/x509.yaml
+-rw-r--r--   0 gukroon   (1000) users      (100)       90 2019-12-23 11:09:56.000000 sr2t-0bs1d1an-0.0.9/sr2t/data/http.yaml
+-rw-r--r--   0 gukroon   (1000) users      (100)     1799 2019-12-14 19:28:50.000000 sr2t-0bs1d1an-0.0.9/.gitignore
+-rw-r--r--   0 gukroon   (1000) users      (100)      208 2019-12-16 12:16:14.000000 sr2t-0bs1d1an-0.0.9/.gitlab-ci.yml
+-rw-r--r--   0 gukroon   (1000) users      (100)    23343 2019-12-23 11:46:17.000000 sr2t-0bs1d1an-0.0.9/PKG-INFO
+drwxr-xr-x   0 gukroon   (1000) users      (100)        0 2019-12-23 11:46:17.000000 sr2t-0bs1d1an-0.0.9/example/
+-rw-r--r--   0 gukroon   (1000) users      (100)     6513 2019-12-13 14:19:34.000000 sr2t-0bs1d1an-0.0.9/example/nmap.xlsx
+-rw-r--r--   0 gukroon   (1000) users      (100)   111825 2019-12-14 13:49:42.000000 sr2t-0bs1d1an-0.0.9/example/dirble-xlsx.png
+-rw-r--r--   0 gukroon   (1000) users      (100)     6779 2019-12-14 12:03:19.000000 sr2t-0bs1d1an-0.0.9/example/dirble.xlsx
+-rw-r--r--   0 gukroon   (1000) users      (100)      134 2019-12-14 14:12:00.000000 sr2t-0bs1d1an-0.0.9/example/testssl.csv
+-rw-r--r--   0 gukroon   (1000) users      (100)    92856 2019-12-14 13:54:38.000000 sr2t-0bs1d1an-0.0.9/example/nikto-xlsx.png
+-rw-r--r--   0 gukroon   (1000) users      (100)    38641 2019-12-14 14:08:32.000000 sr2t-0bs1d1an-0.0.9/example/testssl.json
+-rw-r--r--   0 gukroon   (1000) users      (100)    80990 2019-12-13 14:23:18.000000 sr2t-0bs1d1an-0.0.9/example/nmap-xlsx.png
+-rwxr-xr-x   0 gukroon   (1000) users      (100)     1853 2019-12-14 13:53:19.000000 sr2t-0bs1d1an-0.0.9/example/nikto.xml
+-rw-r--r--   0 gukroon   (1000) users      (100)      508 2019-12-14 13:53:47.000000 sr2t-0bs1d1an-0.0.9/example/nikto.csv
+-rw-r--r--   0 gukroon   (1000) users      (100)   152946 2019-12-13 14:44:06.000000 sr2t-0bs1d1an-0.0.9/example/nessus-xlsx-tls.png
+-rw-r--r--   0 gukroon   (1000) users      (100)     6668 2019-12-14 14:14:58.000000 sr2t-0bs1d1an-0.0.9/example/testssl.xlsx
+-rw-r--r--   0 gukroon   (1000) users      (100)      977 2019-12-14 11:59:41.000000 sr2t-0bs1d1an-0.0.9/example/dirble.xml
+-rw-r--r--   0 gukroon   (1000) users      (100)   144709 2019-12-13 14:44:41.000000 sr2t-0bs1d1an-0.0.9/example/nessus-xlsx-x509.png
+-rw-r--r--   0 gukroon   (1000) users      (100)   127444 2019-12-13 14:43:12.000000 sr2t-0bs1d1an-0.0.9/example/nessus-xlsx-portscan.png
+-rw-r--r--   0 gukroon   (1000) users      (100)   190688 2019-12-13 14:07:30.000000 sr2t-0bs1d1an-0.0.9/example/nessus-xlsx-critical.png
+-rw-r--r--   0 gukroon   (1000) users      (100)   271966 2019-12-14 14:20:25.000000 sr2t-0bs1d1an-0.0.9/example/fortify-xlsx.png
+-rw-r--r--   0 gukroon   (1000) users      (100)      413 2019-12-14 12:00:09.000000 sr2t-0bs1d1an-0.0.9/example/dirble.csv
+-rw-r--r--   0 gukroon   (1000) users      (100)      198 2019-11-22 10:42:12.000000 sr2t-0bs1d1an-0.0.9/example/output.csv
+-rw-r--r--   0 gukroon   (1000) users      (100)     6577 2019-12-14 13:54:05.000000 sr2t-0bs1d1an-0.0.9/example/nikto.xlsx
+-rw-r--r--   0 gukroon   (1000) users      (100)     9263 2019-11-22 10:42:12.000000 sr2t-0bs1d1an-0.0.9/example/nmap.xml
+-rw-r--r--   0 gukroon   (1000) users      (100)    83946 2019-12-14 14:15:29.000000 sr2t-0bs1d1an-0.0.9/example/testssl-xlsx.png
+-rw-r--r--   0 gukroon   (1000) users      (100)      720 2019-11-22 10:42:12.000000 sr2t-0bs1d1an-0.0.9/example/output.txt
+-rw-r--r--   0 gukroon   (1000) users      (100)    35061 2019-11-22 10:42:12.000000 sr2t-0bs1d1an-0.0.9/LICENSE
+-rw-r--r--   0 gukroon   (1000) users      (100)      887 2019-12-23 11:44:57.000000 sr2t-0bs1d1an-0.0.9/setup.py
+drwxr-xr-x   0 gukroon   (1000) users      (100)        0 2019-12-23 11:46:17.000000 sr2t-0bs1d1an-0.0.9/sr2t_0bs1d1an.egg-info/
+-rw-r--r--   0 gukroon   (1000) users      (100)     1045 2019-12-23 11:46:17.000000 sr2t-0bs1d1an-0.0.9/sr2t_0bs1d1an.egg-info/SOURCES.txt
+-rw-r--r--   0 gukroon   (1000) users      (100)    23343 2019-12-23 11:46:17.000000 sr2t-0bs1d1an-0.0.9/sr2t_0bs1d1an.egg-info/PKG-INFO
+-rw-r--r--   0 gukroon   (1000) users      (100)        1 2019-12-23 11:46:17.000000 sr2t-0bs1d1an-0.0.9/sr2t_0bs1d1an.egg-info/dependency_links.txt
+-rw-r--r--   0 gukroon   (1000) users      (100)       41 2019-12-23 11:46:17.000000 sr2t-0bs1d1an-0.0.9/sr2t_0bs1d1an.egg-info/entry_points.txt
+-rw-r--r--   0 gukroon   (1000) users      (100)        5 2019-12-23 11:46:17.000000 sr2t-0bs1d1an-0.0.9/sr2t_0bs1d1an.egg-info/top_level.txt
+-rw-r--r--   0 gukroon   (1000) users      (100)       32 2019-12-23 11:46:17.000000 sr2t-0bs1d1an-0.0.9/sr2t_0bs1d1an.egg-info/requires.txt
+-rw-r--r--   0 gukroon   (1000) users      (100)    19782 2019-12-16 12:21:39.000000 sr2t-0bs1d1an-0.0.9/README.md
+-rw-r--r--   0 gukroon   (1000) users      (100)       38 2019-12-23 11:46:17.000000 sr2t-0bs1d1an-0.0.9/setup.cfg
```

### Comparing `sr2t-0bs1d1an-0.0.8/sr2t/parsers/testssl.py` & `sr2t-0bs1d1an-0.0.9/sr2t/parsers/testssl.py`

 * *Files identical despite different names*

### Comparing `sr2t-0bs1d1an-0.0.8/sr2t/parsers/fortify.py` & `sr2t-0bs1d1an-0.0.9/sr2t/parsers/fortify.py`

 * *Files identical despite different names*

### Comparing `sr2t-0bs1d1an-0.0.8/sr2t/parsers/dirble.py` & `sr2t-0bs1d1an-0.0.9/sr2t/parsers/dirble.py`

 * *Files identical despite different names*

### Comparing `sr2t-0bs1d1an-0.0.8/sr2t/parsers/nikto.py` & `sr2t-0bs1d1an-0.0.9/sr2t/parsers/nikto.py`

 * *Files identical despite different names*

### Comparing `sr2t-0bs1d1an-0.0.8/sr2t/parsers/nmap.py` & `sr2t-0bs1d1an-0.0.9/sr2t/parsers/nmap.py`

 * *Files identical despite different names*

### Comparing `sr2t-0bs1d1an-0.0.8/sr2t/sr2t.py` & `sr2t-0bs1d1an-0.0.9/sr2t/sr2t.py`

 * *Files identical despite different names*

### Comparing `sr2t-0bs1d1an-0.0.8/.gitignore` & `sr2t-0bs1d1an-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `sr2t-0bs1d1an-0.0.8/PKG-INFO` & `sr2t-0bs1d1an-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sr2t-0bs1d1an
-Version: 0.0.8
+Version: 0.0.9
 Summary: Converts scanning reports to a tabular format
 Home-page: https://gitlab.com/0bs1d1an/sr2t
 Author: Guido Kroon
 Author-email: gkroon@maelstrom.ninja
 License: UNKNOWN
 Description: [![pipeline status](https://gitlab.com/0bs1d1an/sr2t/badges/master/pipeline.svg)](https://gitlab.com/0bs1d1an/sr2t/commits/master)
```

### Comparing `sr2t-0bs1d1an-0.0.8/example/nmap.xlsx` & `sr2t-0bs1d1an-0.0.9/example/nmap.xlsx`

 * *Files identical despite different names*

### Comparing `sr2t-0bs1d1an-0.0.8/example/dirble-xlsx.png` & `sr2t-0bs1d1an-0.0.9/example/dirble-xlsx.png`

 * *Files identical despite different names*

### Comparing `sr2t-0bs1d1an-0.0.8/example/dirble.xlsx` & `sr2t-0bs1d1an-0.0.9/example/dirble.xlsx`

 * *Files identical despite different names*

### Comparing `sr2t-0bs1d1an-0.0.8/example/nikto-xlsx.png` & `sr2t-0bs1d1an-0.0.9/example/nikto-xlsx.png`

 * *Files identical despite different names*

### Comparing `sr2t-0bs1d1an-0.0.8/example/testssl.json` & `sr2t-0bs1d1an-0.0.9/example/testssl.json`

 * *Files identical despite different names*

### Comparing `sr2t-0bs1d1an-0.0.8/example/nmap-xlsx.png` & `sr2t-0bs1d1an-0.0.9/example/nmap-xlsx.png`

 * *Files identical despite different names*

### Comparing `sr2t-0bs1d1an-0.0.8/example/nikto.xml` & `sr2t-0bs1d1an-0.0.9/example/nikto.xml`

 * *Files identical despite different names*

### Comparing `sr2t-0bs1d1an-0.0.8/example/nessus-xlsx-tls.png` & `sr2t-0bs1d1an-0.0.9/example/nessus-xlsx-tls.png`

 * *Files identical despite different names*

### Comparing `sr2t-0bs1d1an-0.0.8/example/testssl.xlsx` & `sr2t-0bs1d1an-0.0.9/example/testssl.xlsx`

 * *Files identical despite different names*

### Comparing `sr2t-0bs1d1an-0.0.8/example/dirble.xml` & `sr2t-0bs1d1an-0.0.9/example/dirble.xml`

 * *Files identical despite different names*

### Comparing `sr2t-0bs1d1an-0.0.8/example/nessus-xlsx-x509.png` & `sr2t-0bs1d1an-0.0.9/example/nessus-xlsx-x509.png`

 * *Files identical despite different names*

### Comparing `sr2t-0bs1d1an-0.0.8/example/nessus-xlsx-portscan.png` & `sr2t-0bs1d1an-0.0.9/example/nessus-xlsx-portscan.png`

 * *Files identical despite different names*

### Comparing `sr2t-0bs1d1an-0.0.8/example/nessus-xlsx-critical.png` & `sr2t-0bs1d1an-0.0.9/example/nessus-xlsx-critical.png`

 * *Files identical despite different names*

### Comparing `sr2t-0bs1d1an-0.0.8/example/fortify-xlsx.png` & `sr2t-0bs1d1an-0.0.9/example/fortify-xlsx.png`

 * *Files identical despite different names*

### Comparing `sr2t-0bs1d1an-0.0.8/example/nikto.xlsx` & `sr2t-0bs1d1an-0.0.9/example/nikto.xlsx`

 * *Files identical despite different names*

### Comparing `sr2t-0bs1d1an-0.0.8/example/nmap.xml` & `sr2t-0bs1d1an-0.0.9/example/nmap.xml`

 * *Files identical despite different names*

### Comparing `sr2t-0bs1d1an-0.0.8/example/testssl-xlsx.png` & `sr2t-0bs1d1an-0.0.9/example/testssl-xlsx.png`

 * *Files identical despite different names*

### Comparing `sr2t-0bs1d1an-0.0.8/example/output.txt` & `sr2t-0bs1d1an-0.0.9/example/output.txt`

 * *Files identical despite different names*

### Comparing `sr2t-0bs1d1an-0.0.8/LICENSE` & `sr2t-0bs1d1an-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sr2t-0bs1d1an-0.0.8/setup.py` & `sr2t-0bs1d1an-0.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sr2t-0bs1d1an",
-    version="0.0.8",
+    version="0.0.9",
     author="Guido Kroon",
     author_email="gkroon@maelstrom.ninja",
     description="Converts scanning reports to a tabular format",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/0bs1d1an/sr2t",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     install_requires=['argparse', 'PrettyTable', 'XlsxWriter'],
+    package_data={
+        'sr2t': ['data/*.yaml'],
+    },
     entry_points={
         'console_scripts': ['sr2t=sr2t.sr2t:main'],
     }
 )
```

### Comparing `sr2t-0bs1d1an-0.0.8/sr2t_0bs1d1an.egg-info/SOURCES.txt` & `sr2t-0bs1d1an-0.0.9/sr2t_0bs1d1an.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -23,14 +23,18 @@
 example/output.txt
 example/testssl-xlsx.png
 example/testssl.csv
 example/testssl.json
 example/testssl.xlsx
 sr2t/__init__.py
 sr2t/sr2t.py
+sr2t/data/autoclassify.yaml
+sr2t/data/http.yaml
+sr2t/data/tls.yaml
+sr2t/data/x509.yaml
 sr2t/parsers/__init__.py
 sr2t/parsers/dirble.py
 sr2t/parsers/fortify.py
 sr2t/parsers/nessus.py
 sr2t/parsers/nikto.py
 sr2t/parsers/nmap.py
 sr2t/parsers/testssl.py
```

### Comparing `sr2t-0bs1d1an-0.0.8/sr2t_0bs1d1an.egg-info/PKG-INFO` & `sr2t-0bs1d1an-0.0.9/sr2t_0bs1d1an.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sr2t-0bs1d1an
-Version: 0.0.8
+Version: 0.0.9
 Summary: Converts scanning reports to a tabular format
 Home-page: https://gitlab.com/0bs1d1an/sr2t
 Author: Guido Kroon
 Author-email: gkroon@maelstrom.ninja
 License: UNKNOWN
 Description: [![pipeline status](https://gitlab.com/0bs1d1an/sr2t/badges/master/pipeline.svg)](https://gitlab.com/0bs1d1an/sr2t/commits/master)
```

### Comparing `sr2t-0bs1d1an-0.0.8/README.md` & `sr2t-0bs1d1an-0.0.9/README.md`

 * *Files identical despite different names*

