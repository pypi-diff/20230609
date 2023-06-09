# Comparing `tmp/openrepos-webclient-1.5.0.tar.gz` & `tmp/openrepos-webclient-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openrepos-webclient-1.5.0.tar", last modified: Fri Jun  9 15:41:59 2023, max compression
+gzip compressed data, was "openrepos-webclient-1.5.1.tar", last modified: Fri Jun  9 16:01:30 2023, max compression
```

## Comparing `openrepos-webclient-1.5.0.tar` & `openrepos-webclient-1.5.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:41:58.991646 openrepos-webclient-1.5.0/
--rw-rw-rw-   0 root         (0) root         (0)    35048 2023-06-09 15:41:57.000000 openrepos-webclient-1.5.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       16 2023-06-09 15:41:57.000000 openrepos-webclient-1.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4578 2023-06-09 15:41:58.991646 openrepos-webclient-1.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3917 2023-06-09 15:41:57.000000 openrepos-webclient-1.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:41:58.989646 openrepos-webclient-1.5.0/openrepos/
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-06-09 15:41:57.000000 openrepos-webclient-1.5.0/openrepos/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      171 2023-06-09 15:41:57.000000 openrepos-webclient-1.5.0/openrepos/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:41:58.989646 openrepos-webclient-1.5.0/openrepos/cli/
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-06-09 15:41:57.000000 openrepos-webclient-1.5.0/openrepos/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      176 2023-06-09 15:41:57.000000 openrepos-webclient-1.5.0/openrepos/cli/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:41:58.990646 openrepos-webclient-1.5.0/openrepos/cli/commands/
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-06-09 15:41:57.000000 openrepos-webclient-1.5.0/openrepos/cli/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3373 2023-06-09 15:41:57.000000 openrepos-webclient-1.5.0/openrepos/cli/commands/main.py
--rw-rw-rw-   0 root         (0) root         (0)     3594 2023-06-09 15:41:57.000000 openrepos-webclient-1.5.0/openrepos/cli/commands/navigation.py
--rw-rw-rw-   0 root         (0) root         (0)    26027 2023-06-09 15:41:57.000000 openrepos-webclient-1.5.0/openrepos/client.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-09 15:41:57.000000 openrepos-webclient-1.5.0/openrepos/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:41:58.990646 openrepos-webclient-1.5.0/openrepos_webclient.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4578 2023-06-09 15:41:58.000000 openrepos-webclient-1.5.0/openrepos_webclient.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      563 2023-06-09 15:41:58.000000 openrepos-webclient-1.5.0/openrepos_webclient.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 15:41:58.000000 openrepos-webclient-1.5.0/openrepos_webclient.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-06-09 15:41:58.000000 openrepos-webclient-1.5.0/openrepos_webclient.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-06-09 15:41:58.000000 openrepos-webclient-1.5.0/openrepos_webclient.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-09 15:41:58.000000 openrepos-webclient-1.5.0/openrepos_webclient.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-06-09 15:41:57.000000 openrepos-webclient-1.5.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1050 2023-06-09 15:41:58.991646 openrepos-webclient-1.5.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)       61 2023-06-09 15:41:57.000000 openrepos-webclient-1.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 16:01:30.894070 openrepos-webclient-1.5.1/
+-rw-rw-rw-   0 root         (0) root         (0)    35048 2023-06-09 16:01:29.000000 openrepos-webclient-1.5.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       16 2023-06-09 16:01:29.000000 openrepos-webclient-1.5.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4578 2023-06-09 16:01:30.894070 openrepos-webclient-1.5.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3917 2023-06-09 16:01:29.000000 openrepos-webclient-1.5.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 16:01:30.892070 openrepos-webclient-1.5.1/openrepos/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-06-09 16:01:29.000000 openrepos-webclient-1.5.1/openrepos/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      171 2023-06-09 16:01:29.000000 openrepos-webclient-1.5.1/openrepos/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 16:01:30.892070 openrepos-webclient-1.5.1/openrepos/cli/
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-06-09 16:01:29.000000 openrepos-webclient-1.5.1/openrepos/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      176 2023-06-09 16:01:29.000000 openrepos-webclient-1.5.1/openrepos/cli/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 16:01:30.893070 openrepos-webclient-1.5.1/openrepos/cli/commands/
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-06-09 16:01:29.000000 openrepos-webclient-1.5.1/openrepos/cli/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3373 2023-06-09 16:01:29.000000 openrepos-webclient-1.5.1/openrepos/cli/commands/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     3594 2023-06-09 16:01:29.000000 openrepos-webclient-1.5.1/openrepos/cli/commands/navigation.py
+-rw-rw-rw-   0 root         (0) root         (0)    26210 2023-06-09 16:01:29.000000 openrepos-webclient-1.5.1/openrepos/client.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-09 16:01:29.000000 openrepos-webclient-1.5.1/openrepos/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 16:01:30.894070 openrepos-webclient-1.5.1/openrepos_webclient.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4578 2023-06-09 16:01:30.000000 openrepos-webclient-1.5.1/openrepos_webclient.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      563 2023-06-09 16:01:30.000000 openrepos-webclient-1.5.1/openrepos_webclient.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 16:01:30.000000 openrepos-webclient-1.5.1/openrepos_webclient.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-06-09 16:01:30.000000 openrepos-webclient-1.5.1/openrepos_webclient.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-06-09 16:01:30.000000 openrepos-webclient-1.5.1/openrepos_webclient.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-09 16:01:30.000000 openrepos-webclient-1.5.1/openrepos_webclient.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-06-09 16:01:29.000000 openrepos-webclient-1.5.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1050 2023-06-09 16:01:30.894070 openrepos-webclient-1.5.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)       61 2023-06-09 16:01:29.000000 openrepos-webclient-1.5.1/setup.py
```

### Comparing `openrepos-webclient-1.5.0/LICENSE` & `openrepos-webclient-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openrepos-webclient-1.5.0/PKG-INFO` & `openrepos-webclient-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openrepos-webclient
-Version: 1.5.0
+Version: 1.5.1
 Summary: OpenRepos.net web client
 Home-page: https://gitlab.com/nobodyinperson/python3-openrepos-webclient
 Author: Yann Buechau
 Author-email: nobodyinperson@posteo.de
 License: GPLv3
 Keywords: openrepos,openrepos.net,sailfish,sailfishos,selenium,firefox,xvfb
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `openrepos-webclient-1.5.0/README.md` & `openrepos-webclient-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `openrepos-webclient-1.5.0/openrepos/cli/commands/main.py` & `openrepos-webclient-1.5.1/openrepos/cli/commands/main.py`

 * *Files identical despite different names*

### Comparing `openrepos-webclient-1.5.0/openrepos/cli/commands/navigation.py` & `openrepos-webclient-1.5.1/openrepos/cli/commands/navigation.py`

 * *Files identical despite different names*

### Comparing `openrepos-webclient-1.5.0/openrepos/client.py` & `openrepos-webclient-1.5.1/openrepos/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,29 +169,34 @@
         time_before = time.time()
         time_shown_last = time_before
         desc = " ".join(
             itertools.chain(
                 map(repr, args), [f"{k}={v!r}" for k, v in kwargs.items()]
             )
         )
+        finder = (
+            self.webdriver.find_elements
+            if multiple
+            else self.webdriver.find_element
+        )
         with self.console.status(f"⏳🔎 Waiting for {desc} to appear..."):
             for n in itertools.count(1):
                 if time.time() - time_before > timeout:
                     logger.warning(
                         f"🤷 Couldn't find {desc} after {n} tries and {time.time() - time_before}s"
                     )
                     return None
                 if time.time() - time_shown_last > 2:
                     logger.info(f"⏳🔎 Still Waiting for {desc} to appear...")
                     time_shown_last = time.time()
-                if element := (
-                    self.webdriver.find_elements
-                    if multiple
-                    else self.webdriver.find_element
-                )(*args, **kwargs):
+                try:
+                    element = finder(*args, **kwargs)
+                except NoSuchElementException as e:
+                    element = None
+                if element:
                     logger.debug(
                         f"✅ Found {len(element) if isinstance(element,(list,tuple)) else 1} "
                         f"matches for {desc} "
                         f"after {n} tries in {time.time() - time_before}s"
                     )
                     return element
                 time.sleep(0.5)
@@ -304,17 +309,20 @@
         self.webdriver.get(self.OPENREPOS_HOMEPAGE)
 
     @action()
     def go_to_my_apps(self):
         """
         Go to the My Applications page
         """
-        try:
-            self.find_element(By.LINK_TEXT, "My Applications").click()
-        except NoSuchElementException:
+        my_apps_link = self.find_element(
+            By.LINK_TEXT, "My Applications", timeout=2
+        )
+        if my_apps_link:
+            my_apps_link.click()
+        else:
             logger.debug(
                 "Can't find 'My Applications' link. Probably not logged in."
             )
             self.login()
             logger.debug("Retrying to go to My Applications")
             self.find_element(By.LINK_TEXT, "My Applications").click()
```

### Comparing `openrepos-webclient-1.5.0/openrepos_webclient.egg-info/PKG-INFO` & `openrepos-webclient-1.5.1/openrepos_webclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openrepos-webclient
-Version: 1.5.0
+Version: 1.5.1
 Summary: OpenRepos.net web client
 Home-page: https://gitlab.com/nobodyinperson/python3-openrepos-webclient
 Author: Yann Buechau
 Author-email: nobodyinperson@posteo.de
 License: GPLv3
 Keywords: openrepos,openrepos.net,sailfish,sailfishos,selenium,firefox,xvfb
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `openrepos-webclient-1.5.0/openrepos_webclient.egg-info/SOURCES.txt` & `openrepos-webclient-1.5.1/openrepos_webclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openrepos-webclient-1.5.0/setup.cfg` & `openrepos-webclient-1.5.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = openrepos-webclient
 author = Yann Buechau
 author_email = nobodyinperson@posteo.de
 keywords = openrepos,openrepos.net,sailfish,sailfishos,selenium,firefox,xvfb
-version = 1.5.0
+version = 1.5.1
 license = GPLv3
 url = https://gitlab.com/nobodyinperson/python3-openrepos-webclient
 description = OpenRepos.net web client
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

