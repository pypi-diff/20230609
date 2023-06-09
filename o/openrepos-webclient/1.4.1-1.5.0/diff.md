# Comparing `tmp/openrepos-webclient-1.4.1.tar.gz` & `tmp/openrepos-webclient-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openrepos-webclient-1.4.1.tar", last modified: Fri Aug 26 09:57:55 2022, max compression
+gzip compressed data, was "openrepos-webclient-1.5.0.tar", last modified: Fri Jun  9 15:41:59 2023, max compression
```

## Comparing `openrepos-webclient-1.4.1.tar` & `openrepos-webclient-1.5.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 09:57:55.021593 openrepos-webclient-1.4.1/
--rw-rw-rw-   0 root         (0) root         (0)    35048 2022-08-26 09:57:53.000000 openrepos-webclient-1.4.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       16 2022-08-26 09:57:53.000000 openrepos-webclient-1.4.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4344 2022-08-26 09:57:55.021593 openrepos-webclient-1.4.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3683 2022-08-26 09:57:53.000000 openrepos-webclient-1.4.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 09:57:55.018593 openrepos-webclient-1.4.1/openrepos/
--rw-rw-rw-   0 root         (0) root         (0)      123 2022-08-26 09:57:53.000000 openrepos-webclient-1.4.1/openrepos/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      171 2022-08-26 09:57:53.000000 openrepos-webclient-1.4.1/openrepos/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 09:57:55.019593 openrepos-webclient-1.4.1/openrepos/cli/
--rw-rw-rw-   0 root         (0) root         (0)       87 2022-08-26 09:57:53.000000 openrepos-webclient-1.4.1/openrepos/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      176 2022-08-26 09:57:53.000000 openrepos-webclient-1.4.1/openrepos/cli/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 09:57:55.019593 openrepos-webclient-1.4.1/openrepos/cli/commands/
--rw-rw-rw-   0 root         (0) root         (0)      133 2022-08-26 09:57:53.000000 openrepos-webclient-1.4.1/openrepos/cli/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3412 2022-08-26 09:57:53.000000 openrepos-webclient-1.4.1/openrepos/cli/commands/main.py
--rw-rw-rw-   0 root         (0) root         (0)     3329 2022-08-26 09:57:53.000000 openrepos-webclient-1.4.1/openrepos/cli/commands/navigation.py
--rw-rw-rw-   0 root         (0) root         (0)    23761 2022-08-26 09:57:53.000000 openrepos-webclient-1.4.1/openrepos/client.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-08-26 09:57:53.000000 openrepos-webclient-1.4.1/openrepos/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 09:57:55.021593 openrepos-webclient-1.4.1/openrepos_webclient.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4344 2022-08-26 09:57:54.000000 openrepos-webclient-1.4.1/openrepos_webclient.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      563 2022-08-26 09:57:55.000000 openrepos-webclient-1.4.1/openrepos_webclient.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 09:57:54.000000 openrepos-webclient-1.4.1/openrepos_webclient.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2022-08-26 09:57:54.000000 openrepos-webclient-1.4.1/openrepos_webclient.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       63 2022-08-26 09:57:54.000000 openrepos-webclient-1.4.1/openrepos_webclient.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2022-08-26 09:57:54.000000 openrepos-webclient-1.4.1/openrepos_webclient.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       30 2022-08-26 09:57:53.000000 openrepos-webclient-1.4.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      991 2022-08-26 09:57:55.022593 openrepos-webclient-1.4.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)       61 2022-08-26 09:57:53.000000 openrepos-webclient-1.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:41:58.991646 openrepos-webclient-1.5.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35048 2023-06-09 15:41:57.000000 openrepos-webclient-1.5.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       16 2023-06-09 15:41:57.000000 openrepos-webclient-1.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4578 2023-06-09 15:41:58.991646 openrepos-webclient-1.5.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3917 2023-06-09 15:41:57.000000 openrepos-webclient-1.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:41:58.989646 openrepos-webclient-1.5.0/openrepos/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-06-09 15:41:57.000000 openrepos-webclient-1.5.0/openrepos/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      171 2023-06-09 15:41:57.000000 openrepos-webclient-1.5.0/openrepos/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:41:58.989646 openrepos-webclient-1.5.0/openrepos/cli/
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-06-09 15:41:57.000000 openrepos-webclient-1.5.0/openrepos/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      176 2023-06-09 15:41:57.000000 openrepos-webclient-1.5.0/openrepos/cli/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:41:58.990646 openrepos-webclient-1.5.0/openrepos/cli/commands/
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-06-09 15:41:57.000000 openrepos-webclient-1.5.0/openrepos/cli/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3373 2023-06-09 15:41:57.000000 openrepos-webclient-1.5.0/openrepos/cli/commands/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     3594 2023-06-09 15:41:57.000000 openrepos-webclient-1.5.0/openrepos/cli/commands/navigation.py
+-rw-rw-rw-   0 root         (0) root         (0)    26027 2023-06-09 15:41:57.000000 openrepos-webclient-1.5.0/openrepos/client.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-09 15:41:57.000000 openrepos-webclient-1.5.0/openrepos/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:41:58.990646 openrepos-webclient-1.5.0/openrepos_webclient.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4578 2023-06-09 15:41:58.000000 openrepos-webclient-1.5.0/openrepos_webclient.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      563 2023-06-09 15:41:58.000000 openrepos-webclient-1.5.0/openrepos_webclient.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 15:41:58.000000 openrepos-webclient-1.5.0/openrepos_webclient.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-06-09 15:41:58.000000 openrepos-webclient-1.5.0/openrepos_webclient.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-06-09 15:41:58.000000 openrepos-webclient-1.5.0/openrepos_webclient.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-09 15:41:58.000000 openrepos-webclient-1.5.0/openrepos_webclient.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-06-09 15:41:57.000000 openrepos-webclient-1.5.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1050 2023-06-09 15:41:58.991646 openrepos-webclient-1.5.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)       61 2023-06-09 15:41:57.000000 openrepos-webclient-1.5.0/setup.py
```

### Comparing `openrepos-webclient-1.4.1/LICENSE` & `openrepos-webclient-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openrepos-webclient-1.4.1/PKG-INFO` & `openrepos-webclient-1.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openrepos-webclient
-Version: 1.4.1
+Version: 1.5.0
 Summary: OpenRepos.net web client
 Home-page: https://gitlab.com/nobodyinperson/python3-openrepos-webclient
 Author: Yann Buechau
 Author-email: nobodyinperson@posteo.de
 License: GPLv3
 Keywords: openrepos,openrepos.net,sailfish,sailfishos,selenium,firefox,xvfb
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -85,14 +85,22 @@
 
 If you want to create the app if it doesn't exist yet, you have to provide the same metadata as above for `new-app`:
 
 ```bash
 openrepos upload-rpm -n TestApp -p SailfishOS -c Libraries *.rpm
 ```
 
+### Delete an App
+
+This delete a `TestApp`:
+
+```bash
+openrepos delete-app -n TestApp
+```
+
 ## Using this to automate uploading RPMs to OpenRepos in GitLab CI
 
 This package was designed to automate RPM upload to [OpenRepos.net](https://openrepos.net).
 To do that in GitLab CI, you can `include` the file [`openrepos-upload-rpm.gitlab-ci.yml`](https://gitlab.com/nobodyinperson/python3-openrepos-webclient/-/blob/master/openrepos-upload-rpm.gitlab-ci.yml) from this repository in your CI config.
 The file contains an example of how to do that.
 
 ## Troubleshooting
@@ -101,13 +109,20 @@
 
 ```bash
 openrepos --interactive -vvv upload-rpm ...
 ```
 
 This will ask you before every step and tell you what's going on.
 
+To run without opening the browser window (like in CI), run it with `--xvfb`:
+
+```bash
+openrepos --xvfb --interactive -vvv upload-rpm ...
+```
+
+
 ## Documentation
 
 Documentation of the `openrepos` package can be found [here on
 GitLab](https://nobodyinperson.gitlab.io/python3-openrepos/).
 
 Also, the command-line help page `openrepos -h` is your friend.
```

### Comparing `openrepos-webclient-1.4.1/README.md` & `openrepos-webclient-1.5.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -68,14 +68,22 @@
 
 If you want to create the app if it doesn't exist yet, you have to provide the same metadata as above for `new-app`:
 
 ```bash
 openrepos upload-rpm -n TestApp -p SailfishOS -c Libraries *.rpm
 ```
 
+### Delete an App
+
+This delete a `TestApp`:
+
+```bash
+openrepos delete-app -n TestApp
+```
+
 ## Using this to automate uploading RPMs to OpenRepos in GitLab CI
 
 This package was designed to automate RPM upload to [OpenRepos.net](https://openrepos.net).
 To do that in GitLab CI, you can `include` the file [`openrepos-upload-rpm.gitlab-ci.yml`](https://gitlab.com/nobodyinperson/python3-openrepos-webclient/-/blob/master/openrepos-upload-rpm.gitlab-ci.yml) from this repository in your CI config.
 The file contains an example of how to do that.
 
 ## Troubleshooting
@@ -84,13 +92,20 @@
 
 ```bash
 openrepos --interactive -vvv upload-rpm ...
 ```
 
 This will ask you before every step and tell you what's going on.
 
+To run without opening the browser window (like in CI), run it with `--xvfb`:
+
+```bash
+openrepos --xvfb --interactive -vvv upload-rpm ...
+```
+
+
 ## Documentation
 
 Documentation of the `openrepos` package can be found [here on
 GitLab](https://nobodyinperson.gitlab.io/python3-openrepos/).
 
 Also, the command-line help page `openrepos -h` is your friend.
```

### Comparing `openrepos-webclient-1.4.1/openrepos/cli/commands/main.py` & `openrepos-webclient-1.5.0/openrepos/cli/commands/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # system modules
+import os
 import logging
 import re
 
 # internal modules
 from openrepos.client import Client
 
 # external modules
 import click
+from rich.logging import RichHandler
+from rich.console import Console
 from xvfbwrapper import Xvfb
 
 logger = logging.getLogger(__name__)
 
 
 @click.group(
     help="OpenRepos.net web client",
@@ -54,14 +57,16 @@
     help="OpenRepos.net password",
     show_envvar=True,
 )
 @click.option(
     "--xvfb/--no-xvfb",
     "use_xvfb",
     help="Whether to execute Xvfb",
+    default=not bool(os.environ.get("DISPLAY")),
+    show_default=True,
     show_envvar=True,
 )
 @click.option(
     "-i/--interactive", "interactive", is_flag=True, help="Ask before "
 )
 @click.option(
     "-w",
@@ -79,64 +84,55 @@
     verbosity,
     username,
     password,
     use_xvfb,
     webdriver,
     interactive,
 ):
+    ctx.ensure_object(dict)
+    ctx.obj["console"] = Console()
     # set up logging
-    loglevel_choices = dict(
-        enumerate(
-            (
-                logging.CRITICAL + 1,
-                logging.CRITICAL,
-                logging.WARNING,
-                logging.INFO,
-                logging.DEBUG,
-            ),
-            -2,
-        )
-    )
-    loglevel = loglevel_choices.get(
-        min(
-            max(loglevel_choices),
-            max(min(loglevel_choices), verbosity - quietness),
-        )
-    )
+    loglevel = logging.INFO + 10 * (-verbosity + quietness)
     logging.basicConfig(
         level=loglevel,
-        format="[%(asctime)s] %(levelname)-8s"
-        + (" (%(name)s)" if verbosity >= 3 else "")
-        + " %(message)s",
+        handlers=[RichHandler(console=ctx.obj["console"])],
+        format="%(message)s",
+        datefmt="[%X]",
     )
     for n, l in logger.manager.loggerDict.items():
         if (
             not re.match(
-                r"openrepos\." if verbosity >= 3 else r"openrepos.cli(?!\w)", n
+                r"openrepos\."
+                if logger.getEffectiveLevel() <= logging.INFO
+                else r"openrepos.cli(?!\w)",
+                n,
             )
             and not verbosity > 4
         ):
             l.propagate = False
             if hasattr(l, "setLevel"):
                 l.setLevel(logging.CRITICAL + 1)
-    ctx.ensure_object(dict)
     if use_xvfb:
         xvfb = Xvfb()
         logger.info("Starting Xvfb...")
         xvfb.start()
         logger.debug("Xvfb is running")
 
         def stop_xvfb():
             logger.info("Stopping Xvfb...")
             xvfb.stop()
             logger.debug("Xvfb stopped")
 
         ctx.obj["xvfb"] = xvfb
     client = Client(
-        username=username, password=password, interactive=interactive
+        username=username,
+        password=password,
+        interactive=interactive,
+        webdriver_name=webdriver,
+        console=ctx.obj["console"],
     )
     ctx.obj["client"] = client
     # explicitly cause the webdriver to be loaded
     logger.info("Opening the webdriver")
     client.webdriver
     # proper teardown order: webdriver needs to be closed before Xvfb
     ctx.call_on_close(client.close)
```

### Comparing `openrepos-webclient-1.4.1/openrepos/cli/commands/navigation.py` & `openrepos-webclient-1.5.0/openrepos/cli/commands/navigation.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,28 @@
     show_envvar=True,
 )
 @click.pass_obj
 def new_app(obj, name, platform, category):
     obj["client"].new_app(name=name, platform=platform, category=category)
 
 
+@cli.command(help="Delete an app")
+@click.option(
+    "-n",
+    "--appname",
+    metavar="APPNAME",
+    help="name of the app",
+    required=True,
+    show_envvar=True,
+)
+@click.pass_obj
+def delete_app(obj, appname):
+    obj["client"].delete_app(appname=appname)
+
+
 @cli.command(help="Upload one or more RPM files to an app")
 @click.option(
     "-n",
     "--appname",
     metavar="APPNAME",
     help="name of the app",
     required=True,
```

### Comparing `openrepos-webclient-1.4.1/openrepos/client.py` & `openrepos-webclient-1.5.0/openrepos/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 # system modules
 import os
+import inspect
 import time
 import logging
 import functools
 import itertools
 import operator
 import types
 import re
+from dataclasses import dataclass
 
 # internal modules
 
 # external modules
+import rich
+from rich.console import Console
 import selenium.webdriver
 from selenium.webdriver.remote.webdriver import WebDriver
 from selenium.common.exceptions import NoSuchElementException
 from selenium.webdriver.support.select import Select
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.expected_conditions import (
     text_to_be_present_in_element,
@@ -112,94 +116,104 @@
 
     return decorator
 
 
 action.depth = 0
 
 
+@dataclass
 class Client:
     """
     OpenRepos.net web client
     """
 
     OPENREPOS_HOMEPAGE = "https://openrepos.net"
 
-    def __init__(self, **kwargs):
-        properties = set(
-            k for k, v in vars(type(self)).items() if isinstance(v, property)
-        )
-        for k, v in kwargs.items():
-            if k not in properties:
-                raise ValueError(
-                    "{} has no property {}".format(
-                        type(self).__name__, repr(k)
-                    )
-                )
-            setattr(self, k, v)
-
-    @property
-    def username(self):
-        return getattr(self, "_username", None)
-
-    @username.setter
-    def username(self, value):
-        setattr(self, "_username", str(value))
-
-    @property
-    def password(self):
-        return getattr(self, "_password", None)
-
-    @password.setter
-    def password(self, value):
-        setattr(self, "_password", str(value))
+    username: str = ""
+    password: str = ""
+    interactive: bool = False
+    webdriver_name: str = os.environ.get("OPENREPOS_WEBCLIENT_WEBDRIVER", "")
+    console: Console = Console()
 
-    @property
-    def webdriver_class(self):
-        return getattr(
-            self,
-            "_webdriver_class",
-            next(self.matching_webdriver(), (WebDriver.__name__, WebDriver))[
-                -1
-            ],
-        )
+    @staticmethod
+    def matching_webdriver(s=""):
+        """
+        Generator yielding matching :any:`WebDriver` classes
+        """
+        for subcls in WebDriver.__subclasses__():
+            for name, v in selenium.webdriver.__dict__.items():
+                if v is subcls:
+                    if s.lower() in name.lower():
+                        yield (name, subcls)
 
-    @property
-    def interactive(self):
-        return getattr(self, "_interactive", False)
+    @action("Open the webdriver")
+    def create_webdriver(self):
+        """
+        Create the webdriver
+        """
+        webdrivers = list(self.matching_webdriver(self.webdriver_name))
+        logger.debug(f"{webdrivers = }")
+        if not webdrivers:
+            raise ValueError(f"No useable webdrivers??")
+        name, webdriver = webdrivers[0]
+        logger.debug(f"Creating {name} webdriver")
+        return webdriver()
 
-    @interactive.setter
-    def interactive(self, value):
-        setattr(self, "_interactive", bool(value))
+    @functools.cached_property
+    def webdriver(self):
+        webdriver = self.create_webdriver()
+        # logger.debug(f"⏳ Waiting 10 seconds for the webdriver to load...")
+        # webdriver.implicitly_wait(10)
+        return webdriver
 
-    @webdriver_class.setter
-    def webdriver_class(self, value):
-        if not issubclass(value, WebDriver):
-            raise ValueError(
-                "webdriver_class needs to be a WebDriver, not {}".format(
-                    type(value).__name__
-                )
+    def find_element(self, *args, timeout=10, multiple=False, **kwargs):
+        time_before = time.time()
+        time_shown_last = time_before
+        desc = " ".join(
+            itertools.chain(
+                map(repr, args), [f"{k}={v!r}" for k, v in kwargs.items()]
             )
-        setattr(self, "_webdriver_class", value)
+        )
+        with self.console.status(f"⏳🔎 Waiting for {desc} to appear..."):
+            for n in itertools.count(1):
+                if time.time() - time_before > timeout:
+                    logger.warning(
+                        f"🤷 Couldn't find {desc} after {n} tries and {time.time() - time_before}s"
+                    )
+                    return None
+                if time.time() - time_shown_last > 2:
+                    logger.info(f"⏳🔎 Still Waiting for {desc} to appear...")
+                    time_shown_last = time.time()
+                if element := (
+                    self.webdriver.find_elements
+                    if multiple
+                    else self.webdriver.find_element
+                )(*args, **kwargs):
+                    logger.debug(
+                        f"✅ Found {len(element) if isinstance(element,(list,tuple)) else 1} "
+                        f"matches for {desc} "
+                        f"after {n} tries in {time.time() - time_before}s"
+                    )
+                    return element
+                time.sleep(0.5)
 
-    @property
-    def webdriver(self):
-        try:
-            return self._webdriver
-        except AttributeError:
-            self._webdriver = self.create_webdriver()
-            self._webdriver.implicitly_wait(10)
-        return self._webdriver
+    def find_elements(self, *args, **kwargs):
+        return (
+            self.find_element(*args, **{**kwargs, **dict(multiple=True)}) or []
+        )
 
     def execute_action(
         self, fun, *args, mask_args=False, description=None, **kwargs
     ):
         decorator = action(description=description)
-        logger.debug("Decorating {} with {}".format(fun, decorator))
+        if logger.getEffectiveLevel() < logging.DEBUG:
+            logger.debug("Decorating {} with {}".format(fun, decorator))
         if not isinstance(getattr(fun, "__self__", object), type(self)):
-            logger.debug("Converting to methodtype")
+            if logger.getEffectiveLevel() < logging.DEBUG:
+                logger.debug("Converting to methodtype")
 
             def wrapper(self, *args, **kwargs):
                 return fun(*args, **kwargs)
 
             decorated_function = decorator(wrapper)
         else:
             decorated_function = decorator(fun)
@@ -209,28 +223,30 @@
             logger.warning(
                 "Weird OPENREPOS_ACTION_DELAY ({})".format(
                     repr(os.environ.get("OPENREPOS_ACTION_DELAY"))
                 )
             )
             delay = None
         if delay:
-            logger.debug(
-                "Waiting {} seconds before calling {} with {}, {}".format(
-                    delay,
-                    decorated_function,
-                    "***" if mask_args else args,
-                    kwargs,
+            if logger.getEffectiveLevel() < logging.DEBUG:
+                logger.debug(
+                    "Waiting {} seconds before calling {} with {}, {}".format(
+                        delay,
+                        decorated_function,
+                        "***" if mask_args else args,
+                        kwargs,
+                    )
                 )
-            )
             time.sleep(delay)
-        logger.debug(
-            "Calling {} with {}, {}".format(
-                decorated_function, "***" if mask_args else args, kwargs
+        if logger.getEffectiveLevel() < logging.DEBUG:
+            logger.debug(
+                "Calling {} with {}, {}".format(
+                    decorated_function, "***" if mask_args else args, kwargs
+                )
             )
-        )
         return decorated_function(self, *args, **kwargs)
 
     def wait(
         self,
         condition=lambda driver: True,
         interval=1,
         timeout=10,
@@ -251,115 +267,90 @@
 
         Raises:
             Timeout : if the waiting timed out
         """
         try_ = itertools.count(0)
         time_before = time.time()
         time_last_check = 0
-        desc = str(getattr(condition, "__doc__", condition)).strip()
-        while True:
-            if next(try_) > tries:
-                raise Timeout(
-                    f"Timeout waiting for {desc!r} after {try_} tries"
-                )
-            if time.time() - time_before > timeout:
-                raise Timeout(
-                    f"Timeout waiting for {desc!r} "
-                    f"after {time.time() - time_before:.1f} seconds"
-                )
-            if time.time() - time_last_check < interval:
-                time.sleep(0.1)
-                continue
-            logger.debug(f"Checking {desc!r}...")
-            if result := condition(self.webdriver):
-                logger.info(f"Condition {desc!r} met!")
-                return
-            else:
-                logger.debug(f"Condition {desc!r} not met yet...")
-                time_last_check = time.time()
-
-    @staticmethod
-    def matching_webdriver(s=""):
-        """
-        Generator yielding matching :any:`WebDriver` classes
-        """
-        for subcls in WebDriver.__subclasses__():
-            for name, v in selenium.webdriver.__dict__.items():
-                if v is subcls:
-                    if s.lower() in v.__name__.lower():
-                        yield (name, subcls)
-
-    @action("Open the webdriver")
-    def create_webdriver(self):
-        """
-        Create the webdriver
-        """
-        logger.debug(
-            "Creating {} webdriver".format(
-                ".".join(
-                    (
-                        self.webdriver_class.__module__,
-                        self.webdriver_class.__name__,
+        desc = str(
+            getattr(condition, "__doc__", inspect.getsource(condition))
+        ).strip()
+        with self.console.status(f"⏳ Waiting for {desc}..."):
+            while True:
+                if next(try_) > tries:
+                    raise Timeout(
+                        f"Timeout waiting for {desc!r} after {try_} tries"
                     )
-                )
-            )
-        )
-        return self.webdriver_class()
+                if time.time() - time_before > timeout:
+                    raise Timeout(
+                        f"Timeout waiting for {desc!r} "
+                        f"after {time.time() - time_before:.1f} seconds"
+                    )
+                if time.time() - time_last_check < interval:
+                    time.sleep(0.1)
+                    continue
+                logger.debug(f"Checking {desc!r}...")
+                if result := condition(self.webdriver):
+                    logger.info(f"Condition {desc!r} met!")
+                    return
+                else:
+                    logger.debug(f"Condition {desc!r} not met yet...")
+                    time_last_check = time.time()
 
     @action()
     def go_to_home_page(self):
         """
         Go to the home page
         """
         self.webdriver.get(self.OPENREPOS_HOMEPAGE)
 
     @action()
     def go_to_my_apps(self):
         """
         Go to the My Applications page
         """
         try:
-            self.webdriver.find_element_by_link_text("My Applications").click()
+            self.find_element(By.LINK_TEXT, "My Applications").click()
         except NoSuchElementException:
             logger.debug(
-                "Can't find My Applications link. Probably not logged in."
+                "Can't find 'My Applications' link. Probably not logged in."
             )
             self.login()
             logger.debug("Retrying to go to My Applications")
-            self.webdriver.find_element_by_link_text("My Applications").click()
+            self.find_element(By.LINK_TEXT, "My Applications").click()
 
     @action()
     def go_to_new_app(self):
         """
         Go to Add Application page
         """
         try:
-            link = self.webdriver.find_element_by_link_text("Add Application")
+            link = self.find_element(By.LINK_TEXT, "Add Application")
             self.execute_action(
                 link.click, description="Click ”Add Application” link"
             )
         except NoSuchElementException:
             logger.debug(
                 "Can't find Add Application link. Probably not logged in."
             )
             self.login()
             logger.debug("Retrying to go to New Application")
-            link = self.webdriver.find_element_by_link_text("Add Application")
+            link = self.find_element(By.LINK_TEXT, "Add Application")
             self.execute_action(
                 link.click, description="Click Add Aplication link"
             )
 
     @action()
     def new_app(self, name, platform, category):
         """
         Create a new app
         """
         self.go_to_new_app()
-        links = self.webdriver.find_elements_by_xpath(
-            "//div[@id='block-system-main']//a"
+        links = self.find_elements(
+            By.XPATH, "//div[@id='block-system-main']//a"
         )
         try:
             link = next(
                 filter(
                     lambda e: re.match(r"(.*?)\s+Application$", e.text)
                     and str(platform).lower() in e.text.lower(),
                     links,
@@ -388,23 +379,23 @@
                         )
                     ),
                 )
             )
         self.execute_action(
             link.click, description="Click {} link".format(repr(link.text))
         )
-        title_field = self.webdriver.find_element_by_id("edit-title")
+        title_field = self.find_element(By.ID, "edit-title")
         self.execute_action(
             title_field.send_keys,
             name,
             description="Enter {} title".format(repr(name)),
         )
         category_menu = Select(
-            self.webdriver.find_element_by_id(
-                "edit-field-category-und-hierarchical-select-selects-0"
+            self.find_element(
+                By.ID, "edit-field-category-und-hierarchical-select-selects-0"
             )
         )
         try:
             index = next(
                 (
                     i
                     for i, e in enumerate(category_menu.options)
@@ -444,66 +435,127 @@
             index,
             description="Select category {}".format(
                 repr(category_menu.options[index].text)
             ),
         )
 
         def save():
-            save_button = self.webdriver.find_element_by_id("edit-submit--2")
+            save_button = self.find_element(By.ID, "edit-submit--2")
             save_button.click()
 
             def wait_for_messages(driver):
                 """
                 Wait for a div with id 'messages' containing 'has been updated'
                 """
                 return any(
                     "has been created" in t
                     for t in [
                         e.text
-                        for e in driver.find_elements_by_xpath(
-                            "//div[@id='messages']"
+                        for e in driver.find_elements(
+                            By.XPATH, "//div[@id='messages']"
                         )
                     ]
                 )
 
             self.wait(wait_for_messages)
             logger.info("Saved!")
 
         self.execute_action(save, description="Click Save button")
 
     @action()
-    def upload_rpm(
-        self,
-        appname=None,
-        rpmfiles=None,
-        create_app=False,
-        platform=None,
-        category=None,
-    ):
+    def find_applink_in_my_apps(self, appname=None):
         """
-        Upload RPM file(s)
+        Find the link to the App in 'My Applications'
         """
         self.go_to_my_apps()
 
-        logger.info("Looking for existing app links...")
-        applinks = self.webdriver.find_elements_by_xpath(
-            "//div[@class='content']//tbody//tr//td[1]//a"
+        logger.info("🔎 Looking for existing app links...")
+        applinks = self.find_elements(
+            By.XPATH, "//div[@class='content']//tbody//tr//td[1]//a"
         )
         logger.info(
-            "Found {} exsiting apps: {}".format(
-                len(applinks), ", ".join(e.text for e in applinks)
-            )
+            f"Found {len(applinks)} exsiting apps: {[e.text for e in applinks]}"
         )
         applink = next(
             itertools.chain(
                 filter(lambda e: e.text.lower() == appname.lower(), applinks),
                 filter(lambda e: e.text.lower() in appname.lower(), applinks),
             ),
             None,
         )
+        return applink
+
+    @action()
+    def delete_app(self, appname=None):
+        """
+        Delete App
+        """
+        applink = self.find_applink_in_my_apps(appname)
+
+        if not applink:
+            logger.error(f"App {appname} doesn't exist, no need to delete it.")
+            return
+
+        self.execute_action(
+            applink.click,
+            description="Click {} link".format(repr(applink.text)),
+        )
+
+        edit_link = self.find_element(By.LINK_TEXT, "Edit")
+        self.execute_action(
+            edit_link.click,
+            description=f"Click {edit_link.text!r} link",
+        )
+
+        delete_button = self.find_element(
+            By.CSS_SELECTOR, "input[value=Delete]"
+        )
+        self.execute_action(
+            delete_button.click,
+            description=f"Click {delete_button.text!r} link",
+        )
+
+        delete_button = self.find_element(
+            By.CSS_SELECTOR, "input[value=Delete]"
+        )
+        self.execute_action(
+            delete_button.click,
+            description=f"Click confirmation {delete_button.text!r} link",
+        )
+
+        def wait_for_messages(driver):
+            """
+            Wait for a div with id 'messages' containing 'has been deleted'
+            """
+            return any(
+                "has been deleted" in t
+                for t in [
+                    e.text
+                    for e in driver.find_elements(
+                        By.XPATH, "//div[@id='messages']"
+                    )
+                ]
+            )
+
+        self.wait(wait_for_messages)
+        logger.info("✅ Successfully deleted! 🗑️")
+
+    @action()
+    def upload_rpm(
+        self,
+        appname=None,
+        rpmfiles=None,
+        create_app=False,
+        platform=None,
+        category=None,
+    ):
+        """
+        Upload RPM file(s)
+        """
+        applink = self.find_applink_in_my_apps(appname)
 
         if not applink:
             logger.info(
                 "It seems the app {} doesn't exist yet.".format(repr(appname))
             )
             if create_app:
                 logger.info("Creating app {}".format(repr(appname)))
@@ -531,16 +583,16 @@
         logger.info("Found matching app link {}".format(repr(applink.text)))
 
         self.execute_action(
             applink.click,
             description="Click {} link".format(repr(applink.text)),
         )
 
-        rpmlinks = self.webdriver.find_elements_by_xpath(
-            "//div[@class='content']//tbody//tr//td[1]//a"
+        rpmlinks = self.find_elements(
+            By.XPATH, "//div[@class='content']//tbody//tr//td[1]//a"
         )
 
         logger.debug("This app has {} RPMs".format(len(rpmlinks)))
 
         rpmfiles_to_upload = []
 
         for rpmfile in rpmfiles:
@@ -551,15 +603,15 @@
             ):
                 logger.warning(
                     f"RPM file {rpmfilename!r} is already present. Skipping!"
                 )
                 continue
             rpmfiles_to_upload.append(rpmfile)
 
-        edit_link = self.webdriver.find_element_by_link_text("Edit")
+        edit_link = self.find_element(By.LINK_TEXT, "Edit")
         self.execute_action(
             edit_link.click,
             description="Click {} link".format(repr(edit_link.text)),
         )
 
         if not rpmfiles_to_upload:
             click.echo("No RPM files to upload that aren't already there.")
@@ -573,17 +625,15 @@
                 )
                 package_upload_selector = next(
                     filter(
                         lambda e: all(
                             w in e.get_attribute("id")
                             for w in ("package", "upload")
                         ),
-                        self.webdriver.find_elements_by_xpath(
-                            "//input[@type='file']"
-                        ),
+                        self.find_elements(By.XPATH, "//input[@type='file']"),
                     ),
                     None,
                 )
                 if not package_upload_selector:
                     raise ValueError(
                         "Don't know where to select the RPM to upload... "
                         "Can't find the button."
@@ -604,16 +654,16 @@
                 logger.info("Uploading RPM file '{}'...".format(rpmfile))
                 package_upload_button = next(
                     filter(
                         lambda e: all(
                             w in e.get_attribute("id")
                             for w in ("package", "upload")
                         ),
-                        self.webdriver.find_elements_by_xpath(
-                            "//input[@type='submit']"
+                        self.find_elements(
+                            By.XPATH, "//input[@type='submit']"
                         ),
                     ),
                     None,
                 )
                 if not package_upload_button:
                     raise ValueError(
                         "Don't know where to click to upload the RPM to... "
@@ -623,16 +673,16 @@
 
                 def wait_for_rpm_in_table(driver):
                     """
                     Wait for the RPM file to appear in the list
                     """
                     return sanitize_rpm(os.path.basename(rpmfile)) in [
                         sanitize_rpm(e.text)
-                        for e in driver.find_elements_by_xpath(
-                            "//table//span[@class='file']"
+                        for e in driver.find_elements(
+                            By.XPATH, "//table//span[@class='file']"
                         )
                     ]
 
                 self.wait(wait_for_rpm_in_table)
                 logger.info(f"RPM file {rpmfile!r} uploaded.")
 
             self.execute_action(
@@ -640,28 +690,26 @@
                 description="Upload RPM file {}".format(repr(rpmfile)),
             )
 
             time.sleep(1)
 
         def save():
             logger.info("Saving...")
-            self.webdriver.find_element_by_css_selector(
-                "input[value=Save]"
-            ).click()
+            self.find_element(By.CSS_SELECTOR, "input[value=Save]").click()
 
             def wait_for_messages(driver):
                 """
                 Wait for a div with id 'messages' containing 'has been updated'
                 """
                 return any(
                     "has been updated" in t
                     for t in [
                         e.text
-                        for e in driver.find_elements_by_xpath(
-                            "//div[@id='messages']"
+                        for e in driver.find_elements(
+                            By.XPATH, "//div[@id='messages']"
                         )
                     ]
                 )
 
             self.wait(wait_for_messages)
             logger.info("Saved!")
 
@@ -679,41 +727,41 @@
             username = self.username
         if not password:
             password = self.password
 
         if not (username and password):
             raise ValueError("Both username and password must be specified!")
 
-        username_field = self.webdriver.find_element_by_id("edit-name")
+        username_field = self.find_element(By.ID, "edit-name")
         self.execute_action(
             username_field.send_keys, username, description="Type username"
         )
 
-        password_field = self.webdriver.find_element_by_id("edit-pass")
+        password_field = self.find_element(By.ID, "edit-pass")
         self.execute_action(
             password_field.send_keys,
             password,
             mask_args=True,
             description="Type password",
         )
 
-        login_button = self.webdriver.find_element_by_id("edit-submit--3")
+        login_button = self.find_element(By.ID, "edit-submit--3")
         self.execute_action(
             login_button.click, description="Click Login Button"
         )
 
     @action()
     def close(self):
         """
         Close the webdriver
         """
-        if getattr(self, "_webdriver", None):
+        if webdriver := self.__dict__.get("webdriver"):
             try:
-                self._webdriver.close()
-                del self._webdriver
+                webdriver.close()
+                del self.webdriver
             except BaseException as e:
                 logger.error(
                     "There was an error closing the webdriver. Oh well... 🤷"
                 )
 
     def __del__(self):
         self.interactive = False
```

### Comparing `openrepos-webclient-1.4.1/openrepos_webclient.egg-info/PKG-INFO` & `openrepos-webclient-1.5.0/openrepos_webclient.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openrepos-webclient
-Version: 1.4.1
+Version: 1.5.0
 Summary: OpenRepos.net web client
 Home-page: https://gitlab.com/nobodyinperson/python3-openrepos-webclient
 Author: Yann Buechau
 Author-email: nobodyinperson@posteo.de
 License: GPLv3
 Keywords: openrepos,openrepos.net,sailfish,sailfishos,selenium,firefox,xvfb
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -85,14 +85,22 @@
 
 If you want to create the app if it doesn't exist yet, you have to provide the same metadata as above for `new-app`:
 
 ```bash
 openrepos upload-rpm -n TestApp -p SailfishOS -c Libraries *.rpm
 ```
 
+### Delete an App
+
+This delete a `TestApp`:
+
+```bash
+openrepos delete-app -n TestApp
+```
+
 ## Using this to automate uploading RPMs to OpenRepos in GitLab CI
 
 This package was designed to automate RPM upload to [OpenRepos.net](https://openrepos.net).
 To do that in GitLab CI, you can `include` the file [`openrepos-upload-rpm.gitlab-ci.yml`](https://gitlab.com/nobodyinperson/python3-openrepos-webclient/-/blob/master/openrepos-upload-rpm.gitlab-ci.yml) from this repository in your CI config.
 The file contains an example of how to do that.
 
 ## Troubleshooting
@@ -101,13 +109,20 @@
 
 ```bash
 openrepos --interactive -vvv upload-rpm ...
 ```
 
 This will ask you before every step and tell you what's going on.
 
+To run without opening the browser window (like in CI), run it with `--xvfb`:
+
+```bash
+openrepos --xvfb --interactive -vvv upload-rpm ...
+```
+
+
 ## Documentation
 
 Documentation of the `openrepos` package can be found [here on
 GitLab](https://nobodyinperson.gitlab.io/python3-openrepos/).
 
 Also, the command-line help page `openrepos -h` is your friend.
```

### Comparing `openrepos-webclient-1.4.1/openrepos_webclient.egg-info/SOURCES.txt` & `openrepos-webclient-1.5.0/openrepos_webclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openrepos-webclient-1.4.1/setup.cfg` & `openrepos-webclient-1.5.0/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = openrepos-webclient
 author = Yann Buechau
 author_email = nobodyinperson@posteo.de
 keywords = openrepos,openrepos.net,sailfish,sailfishos,selenium,firefox,xvfb
-version = 1.4.1
+version = 1.5.0
 license = GPLv3
 url = https://gitlab.com/nobodyinperson/python3-openrepos-webclient
 description = OpenRepos.net web client
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -16,25 +16,30 @@
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.5
 
 [options]
 packages = find:
 include_package_data = True
 install_requires = 
+	rich
 	click >= 7
-	selenium >= 3.141, <= 4.2
+	selenium >= 3.141
 	ipython >= 6.5
 	xvfbwrapper >= 0.2.9
 test_suite = tests
 tests_require = 
 
 [options.packages.find]
 exclude = tests
 
 [options.entry_points]
 console_scripts = 
 	openrepos = openrepos.cli.commands.main:cli
 
+[pycodestyle]
+ignore = E402,W503,E501,E203
+exclude = build/
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

