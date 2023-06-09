# Comparing `tmp/macedon-0.9.7.tar.gz` & `tmp/macedon-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macedon-0.9.7.tar", last modified: Sun Jan  8 08:31:33 2023, max compression
+gzip compressed data, was "macedon-0.9.9.tar", last modified: Sun Feb  5 21:10:13 2023, max compression
```

## Comparing `macedon-0.9.7.tar` & `macedon-0.9.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-01-08 08:31:33.802821 macedon-0.9.7/
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      464 2023-01-08 08:30:09.000000 macedon-0.9.7/CHANGES.rst
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1075 2022-12-13 19:00:07.000000 macedon-0.9.7/LICENSE
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)       20 2022-12-13 18:57:54.000000 macedon-0.9.7/MANIFEST.in
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     3144 2023-01-08 08:31:33.802821 macedon-0.9.7/PKG-INFO
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     2628 2023-01-07 12:23:18.000000 macedon-0.9.7/README.md
-drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-01-08 08:31:33.798821 macedon-0.9.7/macedon/
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      347 2023-01-07 03:49:37.000000 macedon-0.9.7/macedon/__init__.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      387 2023-01-04 19:01:21.000000 macedon-0.9.7/macedon/__main__.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1347 2023-01-07 12:19:41.000000 macedon-0.9.7/macedon/_common.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      287 2023-01-08 08:25:01.000000 macedon-0.9.7/macedon/_version.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     3253 2023-01-07 12:19:41.000000 macedon-0.9.7/macedon/entrypoint.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     3990 2023-01-07 12:07:25.000000 macedon-0.9.7/macedon/fileparser.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     3238 2023-01-07 03:41:40.000000 macedon-0.9.7/macedon/io.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1999 2023-01-08 08:28:43.000000 macedon-0.9.7/macedon/logger.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    10787 2023-01-08 08:28:43.000000 macedon-0.9.7/macedon/printer.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     2688 2023-01-08 08:28:43.000000 macedon-0.9.7/macedon/synchronizer.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     3831 2023-01-07 12:07:25.000000 macedon-0.9.7/macedon/worker.py
-drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-01-08 08:31:33.798821 macedon-0.9.7/macedon.egg-info/
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     3144 2023-01-08 08:31:33.000000 macedon-0.9.7/macedon.egg-info/PKG-INFO
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      730 2023-01-08 08:31:33.000000 macedon-0.9.7/macedon.egg-info/SOURCES.txt
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)        1 2023-01-08 08:31:33.000000 macedon-0.9.7/macedon.egg-info/dependency_links.txt
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)       50 2023-01-08 08:31:33.000000 macedon-0.9.7/macedon.egg-info/entry_points.txt
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)       15 2023-01-08 08:31:33.000000 macedon-0.9.7/macedon.egg-info/requires.txt
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)       17 2023-01-08 08:31:33.000000 macedon-0.9.7/macedon.egg-info/top_level.txt
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      104 2022-12-13 18:57:54.000000 macedon-0.9.7/pyproject.toml
-drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-01-08 08:31:33.802821 macedon-0.9.7/pytermor/
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     5330 2023-01-07 12:26:38.000000 macedon-0.9.7/pytermor/__init__.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      267 2023-01-07 12:26:38.000000 macedon-0.9.7/pytermor/__main__.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      295 2023-01-07 12:26:38.000000 macedon-0.9.7/pytermor/_version.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    27675 2023-01-07 12:26:38.000000 macedon-0.9.7/pytermor/ansi.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    32737 2023-01-07 12:26:38.000000 macedon-0.9.7/pytermor/color.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     5032 2023-01-07 12:26:38.000000 macedon-0.9.7/pytermor/common.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)   187793 2023-01-07 12:26:38.000000 macedon-0.9.7/pytermor/cval.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    23825 2023-01-07 12:26:38.000000 macedon-0.9.7/pytermor/renderer.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    17094 2023-01-07 12:26:38.000000 macedon-0.9.7/pytermor/style.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    24486 2023-01-07 12:26:38.000000 macedon-0.9.7/pytermor/text.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    15073 2023-01-07 12:26:38.000000 macedon-0.9.7/pytermor/utilmisc.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    40269 2023-01-07 12:26:38.000000 macedon-0.9.7/pytermor/utilnum.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    26174 2023-01-07 12:26:38.000000 macedon-0.9.7/pytermor/utilstr.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      736 2023-01-08 08:31:33.802821 macedon-0.9.7/setup.cfg
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      302 2023-01-04 19:01:21.000000 macedon-0.9.7/setup.py
+drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-02-05 21:10:13.450597 macedon-0.9.9/
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      464 2023-01-08 08:30:09.000000 macedon-0.9.9/CHANGES.rst
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1080 2023-01-08 08:44:30.000000 macedon-0.9.9/LICENSE
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)       20 2022-12-13 18:57:54.000000 macedon-0.9.9/MANIFEST.in
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     2874 2023-02-05 21:10:13.450597 macedon-0.9.9/PKG-INFO
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     2358 2023-01-08 08:41:19.000000 macedon-0.9.9/README.md
+drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-02-05 21:10:13.446597 macedon-0.9.9/macedon/
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      347 2023-01-07 03:49:37.000000 macedon-0.9.9/macedon/__init__.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      387 2023-01-04 19:01:21.000000 macedon-0.9.9/macedon/__main__.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1728 2023-01-25 03:41:14.000000 macedon-0.9.9/macedon/_common.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      287 2023-02-05 21:08:00.000000 macedon-0.9.9/macedon/_version.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     3852 2023-02-04 13:32:19.000000 macedon-0.9.9/macedon/entrypoint.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     3990 2023-01-07 12:07:25.000000 macedon-0.9.9/macedon/fileparser.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     3198 2023-01-25 03:41:14.000000 macedon-0.9.9/macedon/io.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     3335 2023-01-25 04:19:46.000000 macedon-0.9.9/macedon/logger.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    11950 2023-01-25 03:41:14.000000 macedon-0.9.9/macedon/printer.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     2686 2023-02-04 13:30:24.000000 macedon-0.9.9/macedon/synchronizer.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     4188 2023-01-25 04:15:12.000000 macedon-0.9.9/macedon/worker.py
+drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-02-05 21:10:13.446597 macedon-0.9.9/macedon.egg-info/
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     2874 2023-02-05 21:10:13.000000 macedon-0.9.9/macedon.egg-info/PKG-INFO
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      730 2023-02-05 21:10:13.000000 macedon-0.9.9/macedon.egg-info/SOURCES.txt
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)        1 2023-02-05 21:10:13.000000 macedon-0.9.9/macedon.egg-info/dependency_links.txt
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)       50 2023-02-05 21:10:13.000000 macedon-0.9.9/macedon.egg-info/entry_points.txt
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)       15 2023-02-05 21:10:13.000000 macedon-0.9.9/macedon.egg-info/requires.txt
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)       17 2023-02-05 21:10:13.000000 macedon-0.9.9/macedon.egg-info/top_level.txt
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      104 2022-12-13 18:57:54.000000 macedon-0.9.9/pyproject.toml
+drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-02-05 21:10:13.450597 macedon-0.9.9/pytermor/
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     5330 2023-01-07 12:26:38.000000 macedon-0.9.9/pytermor/__init__.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      267 2023-01-07 12:26:38.000000 macedon-0.9.9/pytermor/__main__.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      295 2023-01-07 12:26:38.000000 macedon-0.9.9/pytermor/_version.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    27675 2023-01-07 12:26:38.000000 macedon-0.9.9/pytermor/ansi.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    32737 2023-01-07 12:26:38.000000 macedon-0.9.9/pytermor/color.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     5032 2023-01-07 12:26:38.000000 macedon-0.9.9/pytermor/common.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)   187793 2023-01-07 12:26:38.000000 macedon-0.9.9/pytermor/cval.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    23825 2023-01-07 12:26:38.000000 macedon-0.9.9/pytermor/renderer.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    17094 2023-01-07 12:26:38.000000 macedon-0.9.9/pytermor/style.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    24486 2023-01-07 12:26:38.000000 macedon-0.9.9/pytermor/text.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    15073 2023-01-07 12:26:38.000000 macedon-0.9.9/pytermor/utilmisc.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    40269 2023-01-07 12:26:38.000000 macedon-0.9.9/pytermor/utilnum.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    26174 2023-01-07 12:26:38.000000 macedon-0.9.9/pytermor/utilstr.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      736 2023-02-05 21:10:13.450597 macedon-0.9.9/setup.cfg
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      302 2023-01-04 19:01:21.000000 macedon-0.9.9/setup.py
```

### Comparing `macedon-0.9.7/LICENSE` & `macedon-0.9.9/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Aleksandr Shavykin
+Copyright (c) 2022-2023 Aleksandr Shavykin
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `macedon-0.9.7/PKG-INFO` & `macedon-0.9.9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: macedon
-Version: 0.9.7
-Summary: CLI web service availability verifier
-Home-page: https://github.com/es7s/macedon
-Author: Aleksandr Shavykin
-Author-email: 0.delameter@gmail.com
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <h1 align="center">
   <img src="https://user-images.githubusercontent.com/50381946/211150260-a91aa0c7-f79b-459c-8a37-a92da96a86a2.png">
   <br>
   <code>macedon</code>
   <br>
 </h1>
 
@@ -39,28 +23,15 @@
 
 ## Installation
 
     pipx install macedon
 
 ## Basic usage
 
-    > macedon localhost:5000 -n3
-
-    Threads:         1
-    Requests:        3
-    -------------------------
-    200  1.6kb  6.0ms  GET http://localhost:80
-    200  1.6kb  4.0ms  GET http://localhost:80
-    200  1.6kb  3.7ms  GET http://localhost:80
-    -------------------------
-    Successful:      3
-    Failed:          0  (0.0%)
-    Avg time:    4.0ms
-    Total time:   37ms
-
+![image](https://user-images.githubusercontent.com/50381946/211187585-2e932cde-f8f6-4d91-9769-962b6efdfe07.png)
 
 ## Configuration / Advanced usage
 
     Usage: macedon [OPTIONS] [ENDPOINT_URL]...
 
     Options:
       -T, --threads INTEGER         Number of threads for concurrent request making.  [default: 1]
```

#### html2text {}

```diff
@@ -1,33 +1,24 @@
-Metadata-Version: 2.1 Name: macedon Version: 0.9.7 Summary: CLI web service
-availability verifier Home-page: https://github.com/es7s/macedon Author:
-Aleksandr Shavykin Author-email: 0.delameter@gmail.com Classifier: Environment
-:: Console Classifier: Intended Audience :: Developers Classifier: Programming
-Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Requires-Python: >=3.10
-Description-Content-Type: text/markdown License-File: LICENSE
 ****** [https://user-images.githubusercontent.com/50381946/211150260-a91aa0c7-
                        f79b-459c-8a37-a92da96a86a2.png]
                                    macedon
                                      ******
                     [PyPI] [Downloads] [Code_style:_black]
 Multi-threaded CLI web service availability verifier. Takes a list of endpoints
 with optional input dataset, performs series of HTTP requests and displays the
 results. ## Motivation Necessity to have a fast and configurable endpoint
 testing tool at fingertips. ## Installation pipx install macedon ## Basic usage
-> macedon localhost:5000 -n3 Threads: 1 Requests: 3 ------------------------
-- 200 1.6kb 6.0ms GET http://localhost:80 200 1.6kb 4.0ms GET http://localhost:
-80 200 1.6kb 3.7ms GET http://localhost:80 ------------------------
-- Successful: 3 Failed: 0 (0.0%) Avg time: 4.0ms Total time: 37ms ##
-Configuration / Advanced usage Usage: macedon [OPTIONS] [ENDPOINT_URL]...
-Options: -T, --threads INTEGER Number of threads for concurrent request making.
-[default: 1] -n, --amount INTEGER How many times each request will be
-performed. [default: 1] -d, --delay FLOAT Seconds to wait between each request.
-[default: 0] -t, --timeout FLOAT Seconds to wait for the response. [default:
-10] -f, --file FILENAME Execute request(s) from a specified file. The file
-should contain a list of endpoints in the format '{method} {url}', one per
-line. Another supported (partially) format is JetBrains HTTP Client format,
-which additionally allows to specify request headers and body. The option can
-be specified multiple times. The ENDPOINT_URL argument(s) are ignored if this
-option is present. -c, --color / -C, --no-color --show-id --show-error -v, --
-verbose Display detailed info on every request. [0<=x<=2] --help Show this
-message and exit. ## Changelog [CHANGES.rst](CHANGES.rst)
+![image](https://user-images.githubusercontent.com/50381946/211187585-2e932cde-
+f8f6-4d91-9769-962b6efdfe07.png) ## Configuration / Advanced usage Usage:
+macedon [OPTIONS] [ENDPOINT_URL]... Options: -T, --threads INTEGER Number of
+threads for concurrent request making. [default: 1] -n, --amount INTEGER How
+many times each request will be performed. [default: 1] -d, --delay FLOAT
+Seconds to wait between each request. [default: 0] -t, --timeout FLOAT Seconds
+to wait for the response. [default: 10] -f, --file FILENAME Execute request(s)
+from a specified file. The file should contain a list of endpoints in the
+format '{method} {url}', one per line. Another supported (partially) format is
+JetBrains HTTP Client format, which additionally allows to specify request
+headers and body. The option can be specified multiple times. The ENDPOINT_URL
+argument(s) are ignored if this option is present. -c, --color / -C, --no-color
+--show-id --show-error -v, --verbose Display detailed info on every request.
+[0<=x<=2] --help Show this message and exit. ## Changelog [CHANGES.rst]
+(CHANGES.rst)
```

### Comparing `macedon-0.9.7/README.md` & `macedon-0.9.9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: macedon
+Version: 0.9.9
+Summary: CLI web service availability verifier
+Home-page: https://github.com/es7s/macedon
+Author: Aleksandr Shavykin
+Author-email: 0.delameter@gmail.com
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <h1 align="center">
   <img src="https://user-images.githubusercontent.com/50381946/211150260-a91aa0c7-f79b-459c-8a37-a92da96a86a2.png">
   <br>
   <code>macedon</code>
   <br>
 </h1>
 
@@ -23,28 +39,15 @@
 
 ## Installation
 
     pipx install macedon
 
 ## Basic usage
 
-    > macedon localhost:5000 -n3
-
-    Threads:         1
-    Requests:        3
-    -------------------------
-    200  1.6kb  6.0ms  GET http://localhost:80
-    200  1.6kb  4.0ms  GET http://localhost:80
-    200  1.6kb  3.7ms  GET http://localhost:80
-    -------------------------
-    Successful:      3
-    Failed:          0  (0.0%)
-    Avg time:    4.0ms
-    Total time:   37ms
-
+![image](https://user-images.githubusercontent.com/50381946/211187585-2e932cde-f8f6-4d91-9769-962b6efdfe07.png)
 
 ## Configuration / Advanced usage
 
     Usage: macedon [OPTIONS] [ENDPOINT_URL]...
 
     Options:
       -T, --threads INTEGER         Number of threads for concurrent request making.  [default: 1]
```

#### html2text {}

```diff
@@ -1,26 +1,31 @@
+Metadata-Version: 2.1 Name: macedon Version: 0.9.9 Summary: CLI web service
+availability verifier Home-page: https://github.com/es7s/macedon Author:
+Aleksandr Shavykin Author-email: 0.delameter@gmail.com Classifier: Environment
+:: Console Classifier: Intended Audience :: Developers Classifier: Programming
+Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent Requires-Python: >=3.10
+Description-Content-Type: text/markdown License-File: LICENSE
 ****** [https://user-images.githubusercontent.com/50381946/211150260-a91aa0c7-
                        f79b-459c-8a37-a92da96a86a2.png]
                                    macedon
                                      ******
                     [PyPI] [Downloads] [Code_style:_black]
 Multi-threaded CLI web service availability verifier. Takes a list of endpoints
 with optional input dataset, performs series of HTTP requests and displays the
 results. ## Motivation Necessity to have a fast and configurable endpoint
 testing tool at fingertips. ## Installation pipx install macedon ## Basic usage
-> macedon localhost:5000 -n3 Threads: 1 Requests: 3 ------------------------
-- 200 1.6kb 6.0ms GET http://localhost:80 200 1.6kb 4.0ms GET http://localhost:
-80 200 1.6kb 3.7ms GET http://localhost:80 ------------------------
-- Successful: 3 Failed: 0 (0.0%) Avg time: 4.0ms Total time: 37ms ##
-Configuration / Advanced usage Usage: macedon [OPTIONS] [ENDPOINT_URL]...
-Options: -T, --threads INTEGER Number of threads for concurrent request making.
-[default: 1] -n, --amount INTEGER How many times each request will be
-performed. [default: 1] -d, --delay FLOAT Seconds to wait between each request.
-[default: 0] -t, --timeout FLOAT Seconds to wait for the response. [default:
-10] -f, --file FILENAME Execute request(s) from a specified file. The file
-should contain a list of endpoints in the format '{method} {url}', one per
-line. Another supported (partially) format is JetBrains HTTP Client format,
-which additionally allows to specify request headers and body. The option can
-be specified multiple times. The ENDPOINT_URL argument(s) are ignored if this
-option is present. -c, --color / -C, --no-color --show-id --show-error -v, --
-verbose Display detailed info on every request. [0<=x<=2] --help Show this
-message and exit. ## Changelog [CHANGES.rst](CHANGES.rst)
+![image](https://user-images.githubusercontent.com/50381946/211187585-2e932cde-
+f8f6-4d91-9769-962b6efdfe07.png) ## Configuration / Advanced usage Usage:
+macedon [OPTIONS] [ENDPOINT_URL]... Options: -T, --threads INTEGER Number of
+threads for concurrent request making. [default: 1] -n, --amount INTEGER How
+many times each request will be performed. [default: 1] -d, --delay FLOAT
+Seconds to wait between each request. [default: 0] -t, --timeout FLOAT Seconds
+to wait for the response. [default: 10] -f, --file FILENAME Execute request(s)
+from a specified file. The file should contain a list of endpoints in the
+format '{method} {url}', one per line. Another supported (partially) format is
+JetBrains HTTP Client format, which additionally allows to specify request
+headers and body. The option can be specified multiple times. The ENDPOINT_URL
+argument(s) are ignored if this option is present. -c, --color / -C, --no-color
+--show-id --show-error -v, --verbose Display detailed info on every request.
+[0<=x<=2] --help Show this message and exit. ## Changelog [CHANGES.rst]
+(CHANGES.rst)
```

### Comparing `macedon-0.9.7/macedon/_common.py` & `macedon-0.9.9/macedon/_common.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,31 @@
 # -----------------------------------------------------------------------------
 #  macedon [CLI web service availability verifier]
 #  (c) 2023 A. Shavykin <0.delameter@gmail.com>
 # -----------------------------------------------------------------------------
+from __future__ import annotations
+from threading import Lock, Event
 from dataclasses import dataclass, field
-from threading import Lock
 
 from requests.structures import CaseInsensitiveDict
 
+_state: State|None = None
+
+
+def get_state() -> State:
+    if _state is None:
+        raise Exception("State is not initialized")
+    return _state
+
+
+def init_state(options: Options):
+    global _state
+    _state = State(options)
+    return _state
+
 
 class ThreadSafeCounter:
     def __init__(self):
         self._value = 0
         self._lock = Lock()
 
     def next(self) -> int:
@@ -19,14 +34,28 @@
             return self._value
 
     @property
     def value(self) -> int:
         return self._value
 
 
+@dataclass
+class State:
+    options: Options
+    last_request_id = ThreadSafeCounter()
+    requests_total = ThreadSafeCounter()
+    requests_printed = ThreadSafeCounter()
+    requests_success = ThreadSafeCounter()
+    requests_failed = ThreadSafeCounter()
+    requests_latency: list[float] = field(default_factory=list)
+    used_methods: set[str] = field(default_factory=set[str])
+    worker_states: list[str] = None
+    shutdown_flag: Event = Event()
+
+
 @dataclass(frozen=True)
 class Options:
     color: bool
     threads: int
     amount: int
     delay: float
     timeout: float
@@ -34,22 +63,10 @@
     show_id: bool
     show_error: bool
 
 
 @dataclass(frozen=True)
 class Task:
     url: str
-    method: str = 'GET'
+    method: str = "GET"
     headers: CaseInsensitiveDict = None
     body: str = None
-
-
-@dataclass
-class SharedState:
-    last_request_id = ThreadSafeCounter()
-    requests_total = ThreadSafeCounter()
-    requests_printed = ThreadSafeCounter()
-    requests_success = ThreadSafeCounter()
-    requests_failed = ThreadSafeCounter()
-    requests_latency: list[float] = field(default_factory=list)
-    methods = set()
-    worker_states: list[str] = None
```

### Comparing `macedon-0.9.7/macedon/entrypoint.py` & `macedon-0.9.9/macedon/entrypoint.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,69 @@
 # -----------------------------------------------------------------------------
 #  macedon [CLI web service availability verifier]
 #  (c) 2022-2023 A. Shavykin <0.delameter@gmail.com>
 # -----------------------------------------------------------------------------
 import os
+import signal
 import sys
 
 import click
-import pytermor as pt
 import urllib3
-from click import Context, HelpFormatter
 from urllib3.exceptions import InsecureRequestWarning
 
+import pytermor as pt
 from . import APP_NAME, APP_VERSION
-from ._common import Options, SharedState
+from ._common import Options, init_state, get_state
 from .fileparser import init_parser
 from .io import init_io
 from .logger import init_loggers, get_logger
-from .printer import init_printer
-from .synchronizer import Synchronizer
+from .printer import init_printer, get_printer
+from .synchronizer import Synchronizer, get_default_thread_num
+
+_shutdown_started = False
 
 
 def invoke():
+    signal.signal(signal.SIGINT, exit_gracefully)
+    signal.signal(signal.SIGTERM, exit_gracefully)
     callback()
 
 
+def shutdown():
+    global _shutdown_started
+    _shutdown_started = True
+    get_state().shutdown_flag.set()
+    get_printer().print_shutdown()
+
+def exit_gracefully(signal_code: int, *args):
+    get_logger().debug(f"{signal.Signals(signal_code).name} ({signal_code}) received")
+    if not _shutdown_started:
+        shutdown()
+        return
+    os._exit(0)
+
+
 class ClickCommand(click.Command):
     pass
 
+
 @click.command(
     cls=ClickCommand,
     no_args_is_help=True,
     context_settings=dict(max_content_width=pt.get_preferable_wrap_width()),
 )
 @click.argument("ENDPOINT_URL", type=str, nargs=-1)
 @click.option(
     "-T",
     "--threads",
     type=int,
-    default=1,
+    default=get_default_thread_num(),
     show_default=True,
-    help="Number of threads for concurrent request making.",
+    help="Number of threads for concurrent request making. Default value depends "
+         "on number of CPU cores available in the system.",
 )
 @click.option(
     "-n",
     "--amount",
     type=int,
     default=1,
     show_default=True,
@@ -51,15 +71,15 @@
 )
 @click.option(
     "-d",
     "--delay",
     type=float,
     default=0,
     show_default=True,
-    help="Seconds to wait between each request.",
+    help="Seconds to wait between requests.",
 )
 @click.option(
     "-t",
     "--timeout",
     type=float,
     default=10,
     show_default=True,
@@ -93,33 +113,31 @@
     is_flag=True,
     help="",
 )
 @click.option(
     "-v",
     "--verbose",
     count=True,
-    type=click.types.IntRange(min=0, max=2, clamp=True),
+    type=click.types.IntRange(min=0, max=3, clamp=True),
     default=0,
-    help="Display detailed info on every request.",
+    help="Increase details level: -v for request info, -vv for debugging worker "
+         "threads debugging, -vvv for response tracing",
 )
-@click.pass_context
-def callback(
-    ctx: click.Context, endpoint_url: tuple[str], file: tuple[click.File], **kwargs
-):
+def callback(endpoint_url: tuple[str], file: tuple[click.File], **kwargs):
     options = Options(**kwargs)
-    shared_state = SharedState()
     urllib3.disable_warnings(InsecureRequestWarning)
 
+    init_state(options)
     init_io(options)
     init_loggers(options)
     _log_init_info(options)
 
     init_parser()
-    init_printer(options, shared_state)
-    sync = Synchronizer(endpoint_url, file, options, shared_state)
+    init_printer()
+    sync = Synchronizer(endpoint_url, file)
     sync.run()
 
 
 def _log_init_info(options: Options):
     logger = get_logger()
     logger.debug(
         f"{APP_NAME} {APP_VERSION} "
```

### Comparing `macedon-0.9.7/macedon/fileparser.py` & `macedon-0.9.9/macedon/fileparser.py`

 * *Files identical despite different names*

### Comparing `macedon-0.9.7/macedon/io.py` & `macedon-0.9.9/macedon/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,27 +12,25 @@
 from ._common import Options
 
 _stdout: IoProxy | None = None
 _stderr: IoProxy | None = None
 
 
 def get_stdout(require=True) -> IoProxy | None:
-    global _stdout
     if not _stdout:
         if require:
-            raise RuntimeError("Stdout proxy is uninitialized")
+            raise Exception("Stdout proxy is not initialized")
         return None
     return _stdout
 
 
 def get_stderr(require=True) -> IoProxy | None:
-    global _stderr
     if not _stderr:
         if require:
-            raise RuntimeError("Stderr proxy is uninitialized")
+            raise Exception("Stderr proxy is not initialized")
         return None
     return _stderr
 
 
 def init_io(options: Options) -> tuple[IoProxy, IoProxy]:
     global _stdout, _stderr
     if _stdout:
```

### Comparing `macedon-0.9.7/macedon/printer.py` & `macedon-0.9.9/macedon/printer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,108 +1,142 @@
 # -----------------------------------------------------------------------------
 #  macedon [CLI web service availability verifier]
 #  (c) 2023 A. Shavykin <0.delameter@gmail.com>
 # -----------------------------------------------------------------------------
+from __future__ import annotations
+
 import re
-import sys
-import threading
+import typing
 from datetime import timedelta
+import threading as th
 
-import pytermor as pt
 import requests
-from pytermor import RT, Fragment
 
-from ._common import Task, SharedState, Options
+import pytermor as pt
+from pytermor import RT, Fragment
+from ._common import Task, get_state, State
 from .io import get_stdout
 from .logger import get_logger
 
+_printer: Printer | None = None
+
+
+def get_printer() -> Printer:
+    if _printer is None:
+        raise Exception("Printer should be initialized")
+    return _printer
+
+
+def init_printer() -> Printer:
+    global _printer
+    _printer = Printer()
+    return _printer
+
 
 class Printer:
     COLUMN_PAD = 2
     CW_STATUS = 4
     CW_SIZE = 7
     CW_ELAPSED = 7
 
     SUCCESS_ST = pt.Style(fg=pt.cv.GREEN, bold=True)
     FAILURE_ST = pt.Style(fg=pt.cv.RED, bold=True)
-    ERROR_ST = pt.Style(fg=pt.cv.RED, dim=True)
-    REQUEST_ID_ST = pt.Style(fg=pt.cv.YELLOW)
+    ERROR_ST = pt.Style(fg=pt.cv.RED)
+    REQUEST_ID_ST = pt.Style(fg=pt.cv.YELLOW, bold=True)
+    REQUEST_ID_LABEL_ST = pt.Style(fg=pt.cv.YELLOW, dim=True)
     NO_VAL_ST = pt.Style(fg=pt.cv.GRAY_23)
-    METHOD_ST = pt.Style(bold=True)
-
-    def __init__(self, options: Options, shared_state: SharedState):
-        self._options = options
-        self._shared_state = shared_state
-        self._lock = threading.Lock()
-        self._request_table = pt.SimpleTable(sep=pt.pad(self.COLUMN_PAD))
-        self._progress_table = pt.SimpleTable(sep="")
-
-        self._size_formatter = None
-        self._elapsed_formatter = None
-        self._request_id_formatter = None
-        self._progress_formatter = None
+    METHOD_OK_ST = pt.Style(bold=True)
+    METHOD_NOK_ST = pt.Style(METHOD_OK_ST, fg=pt.cv.GRAY_23)
+    URL_OK_ST = pt.NOOP_STYLE
+    URL_NOK_ST = pt.Style(URL_OK_ST, fg=pt.cv.GRAY_23)
+
+    def __init__(self):
+        self._state: State = get_state()
+        self._lock: th.Lock = th.Lock()
+        self._request_table: pt.SimpleTable = pt.SimpleTable(
+            sep=pt.pad(self.COLUMN_PAD)
+        )
+        self._progress_table: pt.SimpleTable = pt.SimpleTable(sep="")
+
+        self._size_formatter: pt.StaticBaseFormatter | None = None
+        self._elapsed_formatter: pt.StaticBaseFormatter | None = None
+        self._progress_formatter: pt.StaticBaseFormatter | None = None
 
     def print_prolog(self):
-        req_total = self._shared_state.requests_total.value
-        threads = self._options.threads
+        req_total = self._state.requests_total.value
+        threads = self._state.options.threads
         self._print_row(
             pt.Text(width=2),
             pt.Text(f"Threads:", width=12),
             pt.Text(str(threads), pt.Style(bold=True), width=6, align="right"),
         )
         self._print_row(
             pt.Text(width=2),
             pt.Text(f"Requests:", width=12),
             pt.Text(str(req_total), pt.Style(bold=True), width=6, align="right"),
         )
         self._print_separator()
         self._print_progress(True)
 
-    def print_response(self, task: Task, response: requests.Response, request_id: int):
+    def print_completed_request(
+        self, task: Task, response: requests.Response, request_id: int
+    ):
         size = 0
         try:
             size = len(response.content)
         except Exception:
             pass
 
         self._lock.acquire()
         self._print_request_result(
             self._format_status_code(response),
             self._format_size(size),
             self._format_elapsed(response.elapsed),
             self._format_request_id(request_id),
-            self._format_url(task.url, task.method, None),
+            self._format_url(task.url, task.method, response.ok),
         )
         self._print_progress()
-        self._shared_state.requests_printed.next()
+        self._state.requests_printed.next()
         self._lock.release()
 
     def print_failed_request(
-        self, task: Task, time_ns: int | float, request_id: int, exception: Exception
+        self,
+        task: Task,
+        time_ns: int | float,
+        request_id: int,
+        exception: Exception,
     ):
         self._lock.acquire()
         self._print_request_result(
             self._format_error(exception),
             self._format_elapsed(time_ns),
             self._format_request_id(request_id),
-            self._format_url(task.url, task.method, exception),
+            self._format_url(task.url, task.method, False, exception),
         )
         self._print_progress()
-        self._shared_state.requests_printed.next()
+        self._state.requests_printed.next()
+        self._lock.release()
+
+    def print_shutdown(self):
+        msg = pt.Text(
+            "Shutting threads down (Ctrl+C again to force)", pt.Styles.WARNING
+        )
+        self._lock.acquire()
+        self._print_row(msg)
         self._lock.release()
 
     def print_epilog(self, time_delta_ns: int):
-        req_total = self._shared_state.requests_total.value
-        req_success = self._shared_state.requests_success.value
-        req_failed = self._shared_state.requests_failed.value
+        req_total = self._state.requests_total.value
+        req_success = self._state.requests_success.value
+        req_failed = self._state.requests_failed.value
         success_st = self.SUCCESS_ST if req_success == req_total else None
         failed_st = self.FAILURE_ST if req_failed > 0 else None
         avg_latency_fmtd = pt.Text("---", self.NO_VAL_ST, width=5, align="right")
-        if self._shared_state.requests_latency:
-            avg_latency = pt.utilmisc.median(self._shared_state.requests_latency)
+        if self._state.requests_latency:
+            avg_latency = pt.utilmisc.median(self._state.requests_latency)
             avg_latency_fmtd = self._format_elapsed(timedelta(seconds=avg_latency))
 
         self._reset_cursor_x()
         self._print_separator()
         self._print_row(
             pt.Text(width=2),
             pt.Text(f"Successful:", width=12),
@@ -112,15 +146,15 @@
             pt.Text(width=2),
             pt.Text(f"Failed:", width=12),
             pt.Text(str(req_failed), failed_st, width=6, align="right"),
             pt.Fragment(f"  ({100*req_failed/req_total:.1f}%)"),
         )
         self._print_row(
             pt.Text(width=2),
-            pt.Text(f"Avg time:", width=12),
+            pt.Text(f"Avg (p50):", width=12),
             pt.Text(width=1),
             avg_latency_fmtd,
         )
         self._print_row(
             pt.Text(width=2),
             pt.Text(f"Total time:", width=12),
             pt.Text(width=1),
@@ -140,22 +174,22 @@
             pt.Text("[", width=3, align="center"),
             self._format_progress(pre),
             self._format_request_count(pre),
             pt.Text("]", width=3, align="center"),
             newline=False,
         )
 
+    def _print_separator(self):
+        self._print_row(pt.Text(width=25, fill="-"))
+
     def _print_row(self, *vals: pt.IRenderable, newline: bool = True):
         stdout = get_stdout()
         result = self._progress_table.pass_row(*vals)
         stdout.echo(stdout.render(result), newline=newline)
 
-    def _print_separator(self):
-        self._print_row(pt.Text(width=25, fill="-"))
-
     def _reset_cursor_x(self):
         if not self._is_format_allowed:
             return
         get_stdout().echo(pt.ansi.make_set_cursor_x_abs(1).assemble(), newline=False)
 
     def _get_output_mode(self, opt_color: bool | None) -> pt.OutputMode:
         if opt_color is None:
@@ -165,15 +199,15 @@
         return pt.OutputMode.NO_ANSI
 
     @property
     def _is_format_allowed(self) -> bool:
         return get_stdout().renderer.is_format_allowed
 
     def _get_max_req_id_length(self) -> int:
-        return len(str(self._shared_state.requests_total.value))
+        return len(str(self._state.requests_total.value))
 
     def _format_no_val(self, width: int) -> pt.Text:
         return pt.Text("---", self.NO_VAL_ST, width=width, align="center")
 
     def _format_status_code(self, response: requests.Response) -> pt.Text:
         string = str(response.status_code)
         fmt = self.SUCCESS_ST if response.ok else self.FAILURE_ST
@@ -216,18 +250,18 @@
             seconds = elapsed.total_seconds()
         else:
             get_logger().error(f"Invalid type of 'elazpsed' metric: {elapsed!r}")
             return self._format_no_val(width=self.CW_ELAPSED)
         return self._elapsed_formatter.format(seconds)
 
     def _format_request_id(self, request_id: int) -> pt.Text:
-        if not self._options.show_id:
+        if not self._state.options.show_id:
             return pt.Text(width=0)
 
-        label = Fragment("#")
+        label = Fragment("#", self.REQUEST_ID_LABEL_ST)
         result = Fragment(f"{request_id:>d}", self.REQUEST_ID_ST)
         max_width = self._get_max_req_id_length() + len(str(label.string))
         return pt.Text(label, result, width=max_width, align="right")
 
     def _format_progress(self, pre: bool = False) -> pt.Text:
         if not self._progress_formatter:
             self._progress_formatter = pt.StaticBaseFormatter(
@@ -238,62 +272,60 @@
                 unit="%",
                 pad=True,
                 prefixes=[None, ""],
                 color=self._is_format_allowed,
             )
         original_val = (
             100
-            * (self._shared_state.requests_printed.value + (0 if pre else 1))
-            / self._shared_state.requests_total.value
+            * (self._state.requests_printed.value + (0 if pre else 1))
+            / self._state.requests_total.value
         )
         if original_val <= 1:
             original_val = 0.00
         result = self._progress_formatter.format(original_val)
         return result
 
     def _format_request_count(self, pre: bool = False) -> pt.Text:
-        current = self._shared_state.requests_printed.value + (0 if pre else 1)
-        total = self._shared_state.requests_total.value
+        current = self._state.requests_printed.value + (0 if pre else 1)
+        total = self._state.requests_total.value
         max_id_width = self._get_max_req_id_length()
         label = " "
         result = f"{label}{current:>{max_id_width}d}/{total:<{max_id_width}d}"
         return pt.Text(result, width=max_id_width * 2 + len(str(label)) + 1)
 
     def _format_url(
-        self, url: str, method: str, exception: Exception | None
+        self, url: str, method: str, ok: bool, exception: Exception = None
     ) -> pt.Text:
-        method_len = max(len(m) for m in self._shared_state.methods)
+        method_len = max(len(m) for m in self._state.used_methods)
         error = pt.Fragment(self._get_error_msg(exception), self.ERROR_ST)
+        method_st = self.METHOD_OK_ST if ok else self.METHOD_NOK_ST
+        url_st = self.URL_OK_ST if ok else self.URL_NOK_ST
         result = [
-            pt.Fragment(f"{method:>{method_len}.{method_len}s} ", self.METHOD_ST),
-            pt.Fragment(url + pt.pad(2)),
+            pt.Fragment(f"{method:>{method_len}.{method_len}s} ", method_st),
+            pt.Fragment(url + pt.pad(2), url_st),
             error,
         ]
         return pt.Text(*result)
 
     def _get_error_type(self, exception: Exception | None) -> str:
         if not exception:
             return ""
         return str(exception.__class__.__qualname__)
 
     def _get_error_msg(self, exception: Exception | None) -> str:
-        if not self._options.show_error:
+        if not self._state.options.show_error:
             return ""
         if not exception:
             return ""
         if "Errno" in (exception_str := str(exception)):
             return re.search(r"\[Errno -?\d+][^)\']+", exception_str).group() or ""
-        return ""
-
-
-def get_printer() -> Printer:
-    return _printer
-
-
-def init_printer(options: Options, shared_state: SharedState) -> Printer:
-    global _printer
-    _printer = Printer(options, shared_state)
-
-    return _printer
-
-
-_printer: Printer | None = None
+        if (
+            hasattr(exception, "args")
+            and isinstance(exception.args, typing.Sequence)
+            and len(exception.args) > 0
+        ):
+            if isinstance(subexception := exception.args[0], Exception):
+                return self._get_error_msg(subexception)
+            if hasattr(exception, "reason") and (reason := exception.reason):
+                return str(reason)
+            return str(subexception)
+        return exception.__class__.__qualname__
```

### Comparing `macedon-0.9.7/macedon/synchronizer.py` & `macedon-0.9.9/macedon/synchronizer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,32 @@
 # -----------------------------------------------------------------------------
 #  macedon [CLI web service availability verifier]
 #  (c) 2022-2023 A. Shavykin <0.delameter@gmail.com>
 # -----------------------------------------------------------------------------
-import threading
 import time
 from queue import Queue
 
 import click
-import pytermor as pt
+import psutil
 
-from ._common import Options, Task, SharedState
+from ._common import Options, Task, State, get_state
 from .fileparser import get_parser
 from .logger import get_logger
 from .printer import get_printer
 from .worker import Worker
 
 
 class Synchronizer:
     def __init__(
         self,
         url_args: tuple[str],
         file: tuple[click.File],
-        options: Options,
-        shared_state: SharedState,
     ):
-        self._options = options
-        self._shared_state = shared_state
-        self._task_pool = Queue[Task]()
-        self._workers = []
+        self._task_pool: Queue[Task] = Queue[Task]()
+        self._workers: list[Worker] = []
 
         try:
             self._init_task_queue(url_args, file)
             self._init_workers()
         except Exception as e:
             get_logger().critical(e)
             exit(1)
@@ -44,40 +39,52 @@
         for worker in self._workers:
             get_logger().debug(f"Starting worker {worker}")
             worker.start()
         for worker in self._workers:
             worker.join()
 
         time_after = time.time_ns()
-        self._shared_state.requests_latency.sort()
+        get_state().requests_latency.sort()
         printer.print_epilog(time_after - time_before)
 
     def _init_task_queue(self, url_args: tuple[str], file: tuple[click.File]):
         for file_inst in file:
             try:
                 for task in get_parser().parse(file_inst):
                     self._append_task(task)
             except Exception as e:
                 get_logger().error(f"Failed to parse the file '{file}': {e}")
-        if self._shared_state.requests_total.value > 0:
+        if get_state().requests_total.value > 0:
             return
 
         for url in url_args:
             if not url.startswith("http"):
                 url = f"http://{url}"
             self._append_task(Task(url))
 
-        if self._shared_state.requests_total.value == 0:
+        if get_state().requests_total.value == 0:
             raise ValueError("No urls provided")
 
     def _append_task(self, task: Task):
-        self._shared_state.methods.add(task.method)
-        for _ in range(self._options.amount):
+        state = get_state()
+
+        state.used_methods.add(task.method)
+        for _ in range(state.options.amount):
             self._task_pool.put_nowait(task)
-            self._shared_state.requests_total.next()
+            state.requests_total.next()
 
     def _init_workers(self):
-        self._shared_state.worker_states = ["init"] * self._options.threads
-        for idx in range(self._options.threads):
-            self._workers.append(
-                Worker(self._options, self._task_pool, idx, self._shared_state)
-            )
+        state = get_state()
+        threads = state.options.threads
+
+        state.worker_states = ["init"] * threads
+        for idx in range(threads):
+            self._workers.append(Worker(self._task_pool, idx))
+
+
+def get_default_thread_num() -> int:
+    cores = psutil.cpu_count()
+    if not cores:
+        return 1
+    if cores <= 4:
+        return cores
+    return min(16, cores // 2)
```

### Comparing `macedon-0.9.7/macedon/worker.py` & `macedon-0.9.9/macedon/worker.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,62 +2,66 @@
 #  macedon [CLI web service availability verifier]
 #  (c) 2022-2023 A. Shavykin <0.delameter@gmail.com>
 # -----------------------------------------------------------------------------
 import threading as t
 import time
 from queue import Queue, Empty
 
-import pytermor as pt
 import requests
 import urllib3.exceptions
 from requests import Response
 
-from ._common import Options, Task, SharedState
-from .logger import get_logger
+import pytermor as pt
+from ._common import Options, Task, get_state, State
+from .logger import get_logger, TRACE
 from .printer import get_printer
 
 
 class Worker(t.Thread):
     def __init__(
         self,
-        options: Options,
         task_pool: Queue[Task],
         idx: int,
-        shared_state: SharedState,
     ):
-        self._options = options
-        self._task_pool = task_pool
-        self._idx = idx
-        self._shared_state = shared_state
+        self._state: State = get_state()
+        self._task_pool: Queue[Task] = task_pool
+        self._idx: int = idx
         super().__init__(target=self.run, name=f"#{idx}")
 
     def run(self):
         logger = get_logger()
         printer = get_printer()
 
         while True:
+            if self._shutdown_on_flag():
+                return
             try:
                 task = self._task_pool.get_nowait()
             except Empty:
                 logger.debug(f"Empty queue, terminating")
                 self._update_state("dead")
                 return
             if not task:
                 continue
-            if (delay := self._options.delay) > 0:
-                self._update_state("sleep")
-                time.sleep(delay)
+
+            delay = self._state.options.delay
+            self._update_state("sleep")
+            while delay > 0:
+                if self._shutdown_on_flag():
+                    return
+                time.sleep(1)
+                delay -= 1
 
             response = None
-            request_id = self._shared_state.last_request_id.next()
+            request_id = self._state.last_request_id.next()
             request_params = dict(
                 headers=task.headers,
                 data=task.body,
                 allow_redirects=True,
-                timeout=self._options.timeout,
+                timeout=(self._state.options.timeout/2, self._state.options.timeout/2),
                 verify=task.url.startswith("https"),
             )
             logger.info(
                 f"Performing request #{request_id}: {task.method} {task.url} {request_params}"
             )
             exception = None
             self._update_state("request")
@@ -69,39 +73,46 @@
             except requests.exceptions.RequestException as e:
                 time_after = time.time_ns()
                 logger.exception(e, exc_info=False)
                 exception = e
 
             if response is not None:
                 if response.ok:
-                    self._shared_state.requests_success.next()
+                    self._state.requests_success.next()
                 else:
-                    self._shared_state.requests_failed.next()
+                    self._state.requests_failed.next()
 
-                self._shared_state.requests_latency.append(response.elapsed.total_seconds())
-                printer.print_response(task, response, request_id)
+                self._state.requests_latency.append(response.elapsed.total_seconds())
+                printer.print_completed_request(task, response, request_id)
                 self._dump_response(response, request_id)
             else:
-                self._shared_state.requests_failed.next()
-                printer.print_failed_request(task, time_after - time_before, request_id, exception)
+                self._state.requests_failed.next()
+                printer.print_failed_request(
+                    task, time_after - time_before, request_id, exception
+                )
                 logger.info(f"No response for #{request_id}")
 
     def _update_state(self, state: str):
         get_logger().debug(f"State -> {state}")
-        self._shared_state.worker_states[self._idx] = state
+        self._state.worker_states[self._idx] = state
+
+    def _shutdown_on_flag(self) -> bool:
+        if get_state().shutdown_flag.is_set():
+            self._update_state("dead")
+            return True
+        return False
 
     def _dump_response(self, response: Response, request_id: int):
+        label = f"Response #{request_id} %s:"
+        info_parts = [label % "metadata", str(response.status_code), str(response.headers)]
+
         logger = get_logger()
-        logger.info(
-            f"Response #{request_id} metadata: {response.status_code} {response.headers}"
-        )
+        logger.info(" ".join(info_parts))
         try:
-            logger.debug(
-                pt.dump(response.content.decode(), f"Response #{request_id} content")
-            )
+            decoded = response.content.decode()
+            logger.log(TRACE, pt.dump(decoded, label % "content"))
         except UnicodeError:
-            logger.debug(
-                pt.BytesTracer().apply(
-                    response.content,
-                    pt.TracerExtra(f"Response #{request_id} raw content"),
-                )
+            trace = pt.BytesTracer().apply(
+                response.content,
+                pt.TracerExtra(label % "raw content"),
             )
+            logger.log(TRACE, trace)
```

### Comparing `macedon-0.9.7/macedon.egg-info/PKG-INFO` & `macedon-0.9.9/macedon.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macedon
-Version: 0.9.7
+Version: 0.9.9
 Summary: CLI web service availability verifier
 Home-page: https://github.com/es7s/macedon
 Author: Aleksandr Shavykin
 Author-email: 0.delameter@gmail.com
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -39,28 +39,15 @@
 
 ## Installation
 
     pipx install macedon
 
 ## Basic usage
 
-    > macedon localhost:5000 -n3
-
-    Threads:         1
-    Requests:        3
-    -------------------------
-    200  1.6kb  6.0ms  GET http://localhost:80
-    200  1.6kb  4.0ms  GET http://localhost:80
-    200  1.6kb  3.7ms  GET http://localhost:80
-    -------------------------
-    Successful:      3
-    Failed:          0  (0.0%)
-    Avg time:    4.0ms
-    Total time:   37ms
-
+![image](https://user-images.githubusercontent.com/50381946/211187585-2e932cde-f8f6-4d91-9769-962b6efdfe07.png)
 
 ## Configuration / Advanced usage
 
     Usage: macedon [OPTIONS] [ENDPOINT_URL]...
 
     Options:
       -T, --threads INTEGER         Number of threads for concurrent request making.  [default: 1]
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: macedon Version: 0.9.7 Summary: CLI web service
+Metadata-Version: 2.1 Name: macedon Version: 0.9.9 Summary: CLI web service
 availability verifier Home-page: https://github.com/es7s/macedon Author:
 Aleksandr Shavykin Author-email: 0.delameter@gmail.com Classifier: Environment
 :: Console Classifier: Intended Audience :: Developers Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE
 ****** [https://user-images.githubusercontent.com/50381946/211150260-a91aa0c7-
@@ -10,24 +10,22 @@
                                    macedon
                                      ******
                     [PyPI] [Downloads] [Code_style:_black]
 Multi-threaded CLI web service availability verifier. Takes a list of endpoints
 with optional input dataset, performs series of HTTP requests and displays the
 results. ## Motivation Necessity to have a fast and configurable endpoint
 testing tool at fingertips. ## Installation pipx install macedon ## Basic usage
-> macedon localhost:5000 -n3 Threads: 1 Requests: 3 ------------------------
-- 200 1.6kb 6.0ms GET http://localhost:80 200 1.6kb 4.0ms GET http://localhost:
-80 200 1.6kb 3.7ms GET http://localhost:80 ------------------------
-- Successful: 3 Failed: 0 (0.0%) Avg time: 4.0ms Total time: 37ms ##
-Configuration / Advanced usage Usage: macedon [OPTIONS] [ENDPOINT_URL]...
-Options: -T, --threads INTEGER Number of threads for concurrent request making.
-[default: 1] -n, --amount INTEGER How many times each request will be
-performed. [default: 1] -d, --delay FLOAT Seconds to wait between each request.
-[default: 0] -t, --timeout FLOAT Seconds to wait for the response. [default:
-10] -f, --file FILENAME Execute request(s) from a specified file. The file
-should contain a list of endpoints in the format '{method} {url}', one per
-line. Another supported (partially) format is JetBrains HTTP Client format,
-which additionally allows to specify request headers and body. The option can
-be specified multiple times. The ENDPOINT_URL argument(s) are ignored if this
-option is present. -c, --color / -C, --no-color --show-id --show-error -v, --
-verbose Display detailed info on every request. [0<=x<=2] --help Show this
-message and exit. ## Changelog [CHANGES.rst](CHANGES.rst)
+![image](https://user-images.githubusercontent.com/50381946/211187585-2e932cde-
+f8f6-4d91-9769-962b6efdfe07.png) ## Configuration / Advanced usage Usage:
+macedon [OPTIONS] [ENDPOINT_URL]... Options: -T, --threads INTEGER Number of
+threads for concurrent request making. [default: 1] -n, --amount INTEGER How
+many times each request will be performed. [default: 1] -d, --delay FLOAT
+Seconds to wait between each request. [default: 0] -t, --timeout FLOAT Seconds
+to wait for the response. [default: 10] -f, --file FILENAME Execute request(s)
+from a specified file. The file should contain a list of endpoints in the
+format '{method} {url}', one per line. Another supported (partially) format is
+JetBrains HTTP Client format, which additionally allows to specify request
+headers and body. The option can be specified multiple times. The ENDPOINT_URL
+argument(s) are ignored if this option is present. -c, --color / -C, --no-color
+--show-id --show-error -v, --verbose Display detailed info on every request.
+[0<=x<=2] --help Show this message and exit. ## Changelog [CHANGES.rst]
+(CHANGES.rst)
```

### Comparing `macedon-0.9.7/macedon.egg-info/SOURCES.txt` & `macedon-0.9.9/macedon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `macedon-0.9.7/pytermor/__init__.py` & `macedon-0.9.9/pytermor/__init__.py`

 * *Files identical despite different names*

### Comparing `macedon-0.9.7/pytermor/ansi.py` & `macedon-0.9.9/pytermor/ansi.py`

 * *Files identical despite different names*

### Comparing `macedon-0.9.7/pytermor/color.py` & `macedon-0.9.9/pytermor/color.py`

 * *Files identical despite different names*

### Comparing `macedon-0.9.7/pytermor/common.py` & `macedon-0.9.9/pytermor/common.py`

 * *Files identical despite different names*

### Comparing `macedon-0.9.7/pytermor/cval.py` & `macedon-0.9.9/pytermor/cval.py`

 * *Files identical despite different names*

### Comparing `macedon-0.9.7/pytermor/renderer.py` & `macedon-0.9.9/pytermor/renderer.py`

 * *Files identical despite different names*

### Comparing `macedon-0.9.7/pytermor/style.py` & `macedon-0.9.9/pytermor/style.py`

 * *Files identical despite different names*

### Comparing `macedon-0.9.7/pytermor/text.py` & `macedon-0.9.9/pytermor/text.py`

 * *Files identical despite different names*

### Comparing `macedon-0.9.7/pytermor/utilmisc.py` & `macedon-0.9.9/pytermor/utilmisc.py`

 * *Files identical despite different names*

### Comparing `macedon-0.9.7/pytermor/utilnum.py` & `macedon-0.9.9/pytermor/utilnum.py`

 * *Files identical despite different names*

### Comparing `macedon-0.9.7/pytermor/utilstr.py` & `macedon-0.9.9/pytermor/utilstr.py`

 * *Files identical despite different names*

### Comparing `macedon-0.9.7/setup.cfg` & `macedon-0.9.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = macedon
-version = 0.9.7
+version = 0.9.9
 author = Aleksandr Shavykin
 author_email = 0.delameter@gmail.com
 description = CLI web service availability verifier
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/es7s/macedon
 project_urls =
```

