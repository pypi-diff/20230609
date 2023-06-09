# Comparing `tmp/betfairutil-0.6.1.tar.gz` & `tmp/betfairutil-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betfairutil-0.6.1.tar", last modified: Tue Jun  6 06:37:50 2023, max compression
+gzip compressed data, was "betfairutil-0.6.2.tar", last modified: Fri Jun  9 13:37:23 2023, max compression
```

## Comparing `betfairutil-0.6.1.tar` & `betfairutil-0.6.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 mberk     (1000) mberk     (1000)        0 2023-06-06 06:37:50.944822 betfairutil-0.6.1/
--rw-r--r--   0 mberk     (1000) mberk     (1000)     1062 2021-07-12 09:03:49.000000 betfairutil-0.6.1/LICENSE
--rw-rw-r--   0 mberk     (1000) mberk     (1000)     7231 2023-06-06 06:37:50.944822 betfairutil-0.6.1/PKG-INFO
--rw-rw-r--   0 mberk     (1000) mberk     (1000)     6693 2023-01-13 07:10:05.000000 betfairutil-0.6.1/README.md
-drwxrwxr-x   0 mberk     (1000) mberk     (1000)        0 2023-06-06 06:37:50.940822 betfairutil-0.6.1/betfairutil/
--rw-rw-r--   0 mberk     (1000) mberk     (1000)    95978 2023-06-06 06:23:54.000000 betfairutil-0.6.1/betfairutil/__init__.py
-drwxrwxr-x   0 mberk     (1000) mberk     (1000)        0 2023-06-06 06:37:50.944822 betfairutil-0.6.1/betfairutil.egg-info/
--rw-r--r--   0 mberk     (1000) mberk     (1000)     7231 2023-06-06 06:37:50.000000 betfairutil-0.6.1/betfairutil.egg-info/PKG-INFO
--rw-r--r--   0 mberk     (1000) mberk     (1000)      224 2023-06-06 06:37:50.000000 betfairutil-0.6.1/betfairutil.egg-info/SOURCES.txt
--rw-r--r--   0 mberk     (1000) mberk     (1000)        1 2023-06-06 06:37:50.000000 betfairutil-0.6.1/betfairutil.egg-info/dependency_links.txt
--rw-r--r--   0 mberk     (1000) mberk     (1000)       95 2023-06-06 06:37:50.000000 betfairutil-0.6.1/betfairutil.egg-info/requires.txt
--rw-r--r--   0 mberk     (1000) mberk     (1000)       12 2023-06-06 06:37:50.000000 betfairutil-0.6.1/betfairutil.egg-info/top_level.txt
--rw-rw-r--   0 mberk     (1000) mberk     (1000)       38 2023-06-06 06:37:50.944822 betfairutil-0.6.1/setup.cfg
--rw-r--r--   0 mberk     (1000) mberk     (1000)      916 2023-06-06 06:34:28.000000 betfairutil-0.6.1/setup.py
+drwxrwxr-x   0 mberk     (1000) mberk     (1000)        0 2023-06-09 13:37:23.897948 betfairutil-0.6.2/
+-rw-r--r--   0 mberk     (1000) mberk     (1000)     1062 2021-07-12 09:03:49.000000 betfairutil-0.6.2/LICENSE
+-rw-rw-r--   0 mberk     (1000) mberk     (1000)     7231 2023-06-09 13:37:23.897948 betfairutil-0.6.2/PKG-INFO
+-rw-rw-r--   0 mberk     (1000) mberk     (1000)     6693 2023-01-13 07:10:05.000000 betfairutil-0.6.2/README.md
+drwxrwxr-x   0 mberk     (1000) mberk     (1000)        0 2023-06-09 13:37:23.897948 betfairutil-0.6.2/betfairutil/
+-rw-rw-r--   0 mberk     (1000) mberk     (1000)    96147 2023-06-09 12:09:39.000000 betfairutil-0.6.2/betfairutil/__init__.py
+drwxrwxr-x   0 mberk     (1000) mberk     (1000)        0 2023-06-09 13:37:23.897948 betfairutil-0.6.2/betfairutil.egg-info/
+-rw-r--r--   0 mberk     (1000) mberk     (1000)     7231 2023-06-09 13:37:23.000000 betfairutil-0.6.2/betfairutil.egg-info/PKG-INFO
+-rw-r--r--   0 mberk     (1000) mberk     (1000)      224 2023-06-09 13:37:23.000000 betfairutil-0.6.2/betfairutil.egg-info/SOURCES.txt
+-rw-r--r--   0 mberk     (1000) mberk     (1000)        1 2023-06-09 13:37:23.000000 betfairutil-0.6.2/betfairutil.egg-info/dependency_links.txt
+-rw-r--r--   0 mberk     (1000) mberk     (1000)       95 2023-06-09 13:37:23.000000 betfairutil-0.6.2/betfairutil.egg-info/requires.txt
+-rw-r--r--   0 mberk     (1000) mberk     (1000)       12 2023-06-09 13:37:23.000000 betfairutil-0.6.2/betfairutil.egg-info/top_level.txt
+-rw-rw-r--   0 mberk     (1000) mberk     (1000)       38 2023-06-09 13:37:23.897948 betfairutil-0.6.2/setup.cfg
+-rw-r--r--   0 mberk     (1000) mberk     (1000)      916 2023-06-09 12:47:00.000000 betfairutil-0.6.2/setup.py
```

### Comparing `betfairutil-0.6.1/LICENSE` & `betfairutil-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `betfairutil-0.6.1/PKG-INFO` & `betfairutil-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betfairutil
-Version: 0.6.1
+Version: 0.6.2
 Summary: Utility functions for working with Betfair data
 Home-page: https://github.com/mberk/betfairutil
 Author: Maurice Berk
 Author-email: maurice@mauriceberk.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `betfairutil-0.6.1/README.md` & `betfairutil-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `betfairutil-0.6.1/betfairutil/__init__.py` & `betfairutil-0.6.2/betfairutil/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2744,19 +2744,23 @@
             df["depth"] = df["depth"].astype(int)
         return df
 
 
 def publish_time_to_datetime(
     publish_time: Optional[int],
 ) -> Optional[datetime.datetime]:
-    if publish_time is None:
-        return
-    return datetime.datetime.utcfromtimestamp(publish_time / 1000).replace(
-        tzinfo=datetime.timezone.utc
-    )
+    if publish_time is not None:
+        return datetime.datetime.utcfromtimestamp(publish_time / 1000).replace(
+            tzinfo=datetime.timezone.utc
+        )
+
+
+def datetime_to_publish_time(_datetime: Optional[datetime.datetime]) -> Optional[int]:
+    if _datetime is not None:
+        return int(_datetime.timestamp() * 1000)
 
 
 def create_market_book_generator_from_prices_file(
     path_to_prices_file: Union[str, Path],
     lightweight: bool = True,
     market_type_filter: Optional[Sequence[str]] = None,
     **kwargs,
```

### Comparing `betfairutil-0.6.1/betfairutil.egg-info/PKG-INFO` & `betfairutil-0.6.2/betfairutil.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betfairutil
-Version: 0.6.1
+Version: 0.6.2
 Summary: Utility functions for working with Betfair data
 Home-page: https://github.com/mberk/betfairutil
 Author: Maurice Berk
 Author-email: maurice@mauriceberk.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `betfairutil-0.6.1/setup.py` & `betfairutil-0.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 requires = ["betfairlightweight"]
 tests_require = ["pytest"]
 
 setup(
     name="betfairutil",
-    version="0.6.1",
+    version="0.6.2",
     description="Utility functions for working with Betfair data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Maurice Berk",
     author_email="maurice@mauriceberk.com",
     url="https://github.com/mberk/betfairutil",
     packages=["betfairutil"],
```

