# Comparing `tmp/robocorp_browser-0.4.4.tar.gz` & `tmp/robocorp_browser-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_browser-0.4.4.tar", max compression
+gzip compressed data, was "robocorp_browser-1.0.0.tar", max compression
```

## Comparing `robocorp_browser-0.4.4.tar` & `robocorp_browser-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,9 @@
--rw-r--r--   0        0        0       94 2023-06-05 13:51:44.046831 robocorp_browser-0.4.4/README.md
--rw-r--r--   0        0        0      638 2023-06-05 13:51:44.046831 robocorp_browser-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     7819 2023-06-05 13:51:44.046831 robocorp_browser-0.4.4/src/robocorp/browser/__init__.py
--rw-r--r--   0        0        0     6898 2023-06-05 13:51:44.046831 robocorp_browser-0.4.4/src/robocorp/browser/_browser_context.py
--rw-r--r--   0        0        0        0 2023-06-05 13:51:44.046831 robocorp_browser-0.4.4/src/robocorp/browser/py.typed
--rw-r--r--   0        0        0      606 1970-01-01 00:00:00.000000 robocorp_browser-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0       94 2023-06-09 12:05:54.414735 robocorp_browser-1.0.0/README.md
+-rw-r--r--   0        0        0      638 2023-06-09 12:05:54.414735 robocorp_browser-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6289 2023-06-09 12:05:54.418735 robocorp_browser-1.0.0/src/robocorp/browser/__init__.py
+-rw-r--r--   0        0        0       81 2023-06-09 12:05:54.418735 robocorp_browser-1.0.0/src/robocorp/browser/__main__.py
+-rw-r--r--   0        0        0     6725 2023-06-09 12:05:54.418735 robocorp_browser-1.0.0/src/robocorp/browser/_browser_context.py
+-rw-r--r--   0        0        0     1890 2023-06-09 12:05:54.418735 robocorp_browser-1.0.0/src/robocorp/browser/_browser_engines.py
+-rw-r--r--   0        0        0      825 2023-06-09 12:05:54.418735 robocorp_browser-1.0.0/src/robocorp/browser/cli.py
+-rw-r--r--   0        0        0        0 2023-06-09 12:05:54.418735 robocorp_browser-1.0.0/src/robocorp/browser/py.typed
+-rw-r--r--   0        0        0      606 1970-01-01 00:00:00.000000 robocorp_browser-1.0.0/PKG-INFO
```

### Comparing `robocorp_browser-0.4.4/pyproject.toml` & `robocorp_browser-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-browser"
-version = "0.4.4"
+version = "1.0.0"
 description = "Robocorp browser automation library"
 authors = [
 	"Fabio Z. <fabio@robocorp.com>",
 	"Kerkko P. <kerkko@robocorp.com>",
 	"Ossi R. <ossi@robocorp.com>",
 ]
 readme = "README.md"
```

### Comparing `robocorp_browser-0.4.4/src/robocorp/browser/__init__.py` & `robocorp_browser-1.0.0/src/robocorp/browser/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,43 +5,45 @@
     BrowserContext,
     ElementHandle,
     Locator,
     Page,
     Playwright,
 )
 
-__version__ = "0.4.4"
+from ._browser_engines import BrowserEngine
+
+__version__ = "1.0.0"
 version_info = [int(x) for x in __version__.split(".")]
 
 
 def configure(**kwargs) -> None:
     """
     May be called before any other method to configure the browser settings.
 
     Calling this method is optional (if not called a default configuration will
     be used -- note that calling this method after the browser is already
     initialized will have no effect).
 
     Args:
         browser_engine:
             help="Browser engine which should be used",
-            choices=["chrome", "firefox"],
+            choices=[chromium", "chrome", "chrome-beta", "msedge", "msedge-beta", "msedge-dev", "firefox", "webkit"]
 
         headless: If set to False the browser UI will be shown. If set to True
             the browser UI will be kept hidden. If unset or set to None it'll
             show the browser UI only if a debugger is detected.
 
         slowmo:
             Run interactions in slow motion.
 
         screenshot:
             default="only-on-failure",
             choices=["on", "off", "only-on-failure"],
             help="Whether to automatically capture a screenshot after each task.",
-    """
+    """  # noqa
     from ._browser_context import _browser_config
 
     config = _browser_config()
 
     for key, value in kwargs.items():
         if not hasattr(config, key):
             raise ValueError(f"Invalid configuration: {key}.")
@@ -127,86 +129,25 @@
         automatically closed when the task run session finishes.
     """
     from . import _browser_context
 
     return _browser_context.context()
 
 
-def open_browser(
-    browser_engine: Optional[Literal["chrome", "firefox"]] = None,
-    headless: Optional[bool] = None,
-    **kwargs,
-) -> Browser:
-    """Shortcut to configure and launch a browser instance (using Playwright).
-
-    Note that if the browser was already previously launched the previous
-    instance will be returned and any configuration passed will be ignored.
-
-    Args:
-        browser_engine: Specifies which browser to use. Supported browsers are:
-            ``chrome`` and ``firefox``.
-
-        headless: If set to False the browser UI will be shown. If set to True
-            the browser UI will be kept hidden. If unset or set to None it'll
-            show the browser UI only if a debugger is detected.
-
-    Note:
-        The arguments related to browser initialization will only be used
-        if this is the first call, on subsequent calls the same browser instance
-        will be used and the current page will open the given url.
-
-    Returns:
-        The browser instance.
-    """
-    if browser_engine is not None:
-        kwargs["browser_engine"] = browser_engine
-    if headless is not None:
-        kwargs["headless"] = headless
-    if kwargs:
-        configure(**kwargs)
-    return browser()
-
-
-def open_url(
-    url: str,
-    browser_engine: Optional[Literal["chrome", "firefox"]] = None,
-    headless: Optional[bool] = None,
-    **kwargs,
-) -> Page:
+def goto(url: str) -> Page:
     """
     Changes the url of the current page (creating a page if needed).
 
     Args:
         url: Navigates to the provided URL.
 
-        browser: Specifies which browser to use. Supported browsers are:
-            ``chrome`` and ``firefox``.
-
-        headless: If set to False the browser UI will be shown. If set to True
-            the browser UI will be kept hidden. If unset or set to None it'll
-            show the browser UI only if a debugger is detected.
-
-        kwargs: Other keyword arguments to be passed to the
-            `configure` function (besides `browser` and `headless`).
-
-    Note:
-        The arguments related to browser initialization will only be used
-        if this is the first call, on subsequent calls the same browser instance
-        will be used and the current page will open the given url.
-
     Returns:
         The page instance managed by the robocorp.tasks framework
         (it will be automatically closed when the task finishes).
     """
-    if browser_engine is not None:
-        kwargs["browser_engine"] = browser_engine
-    if headless is not None:
-        kwargs["headless"] = headless
-    if kwargs:
-        configure(**kwargs)
     p = page()
     p.goto(url)
     return p
 
 
 def screenshot(
     element: Optional[Union[Page, ElementHandle, Locator]] = None,
@@ -246,16 +187,33 @@
     log.html(
         f'<img src="data:image/{image_type};base64,{in_base64}"/>', level=log_level
     )
 
     return in_bytes
 
 
+def install(browser_engine: BrowserEngine):
+    """
+    Downloads and installs the given browser engine.
+
+    Note: Google Chrome or Microsoft Edge installations will be installed
+    at the default global location of your operating system overriding your
+    current browser installation.
+
+    Args:
+        browser_engine:
+            help="Browser engine which should be installed",
+            choices=[chromium", "chrome", "chrome-beta", "msedge", "msedge-beta", "msedge-dev", "firefox", "webkit"]
+    """  # noqa
+    from . import _browser_engines
+
+    _browser_engines.install_browser(browser_engine, force=False)
+
+
 __all__ = [
-    "open_browser",
-    "open_url",
+    "install",
     "configure",
     "page",
     "browser",
     "playwright",
     "context",
 ]
```

### Comparing `robocorp_browser-0.4.4/src/robocorp/browser/_browser_context.py` & `robocorp_browser-1.0.0/src/robocorp/browser/_browser_context.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,110 +1,91 @@
-import platform
+import os
 import sys
-from pathlib import Path
-from typing import Callable, Dict, Iterator, List, Literal, Optional
+from typing import Callable, Dict, Iterator, List, Optional, Union
 
 from playwright.sync_api import (
     Browser,
     BrowserContext,
     BrowserType,
     Error,
     Page,
     Playwright,
     sync_playwright,
 )
 from robocorp.tasks import session_cache, task_cache
 
-EXECUTABLE_PATHS = {
-    "chrome": {
-        "Linux": "/usr/bin/google-chrome",
-        "Darwin": "/Applications/Google Chrome.app/Contents/MacOS/Google Chrome",
-    },
-    "firefox": {
-        "Linux": "/usr/bin/firefox",
-        "Windows": "C:\\Program Files\\Mozilla Firefox\\firefox.exe",
-        "Darwin": "/Applications/Firefox.app/Contents/MacOS/firefox",
-    },
-}
-
-
-def _get_executable_path(browser: Literal["firefox", "chrome"]) -> str:
-    system = platform.system()
-
-    if system == "Windows":
-        return _registry_path(browser)
-
-    if browser not in EXECUTABLE_PATHS:
-        raise ValueError(f"Unsupported browser: {browser}")
-
-    path = EXECUTABLE_PATHS[browser][system]
-    if not Path(path).exists():
-        raise RuntimeError(f"Browser executable not found: {path}")
-
-    return path
-
-
-def _registry_path(browser: Literal["chrome", "firefox"]) -> str:
-    if sys.platform != "win32":
-        raise NotImplementedError("Not implemented for non-Windows")
-
-    import winreg
-
-    parent = winreg.HKEY_LOCAL_MACHINE
-    key = rf"SOFTWARE\Microsoft\Windows\CurrentVersion\App Paths\{browser}.exe"
-
-    handle = winreg.OpenKeyEx(parent, key)
-    path, _ = winreg.QueryValueEx(handle, "")  # Empty string is (Default) value
-
-    if not path:
-        raise RuntimeError(f"Failed to read browser path: {browser}")
-
-    return str(path)
+from ._browser_engines import (
+    ENGINE_TO_ARGS,
+    BrowserEngine,
+    browsers_path,
+    install_browser,
+)
 
 
 class _BrowserConfig:
-    __slots__ = "_browser_engine _headless _slowmo _screenshot __weakref__".split()
+    __slots__ = [
+        "_browser_engine",
+        "_install",
+        "_headless",
+        "_slowmo",
+        "_screenshot",
+        "__weakref__",
+    ]
 
     def __init__(
         self,
-        browser_engine: str = "chrome",
+        browser_engine: BrowserEngine = BrowserEngine.CHROMIUM,
+        install: Optional[bool] = None,
         headless: Optional[bool] = None,
         slowmo: int = 0,
         screenshot: str = "only-on-failure",
     ):
         """
         Args:
             browser_engine:
                 help="Browser engine which should be used",
-                choices=["chrome", "firefox"],
+                choices=[chromium", "chrome", "chrome-beta", "msedge", "msedge-beta", "msedge-dev", "firefox", "webkit"]
+
+            install:
+                Install browser or not. If not defined, download is only
+                attempted if the browser fails to launch.
 
             headless:
                 Run headless or not.
 
             slowmo:
                 Run interactions in slow motion (number in millis).
 
             screenshot:
                 default="only-on-failure",
                 choices=["on", "off", "only-on-failure"],
                 help="Whether to automatically capture a screenshot after each task.",
-        """
+        """  # noqa
         self.browser_engine = browser_engine
+        self.install = install
         self.headless = headless
         self.slowmo = slowmo
         self.screenshot = screenshot
 
     @property
-    def browser_engine(self) -> str:
+    def browser_engine(self) -> BrowserEngine:
         return self._browser_engine
 
     @browser_engine.setter
-    def browser_engine(self, value: str):
-        assert value in ["chrome", "firefox"]
-        self._browser_engine = value
+    def browser_engine(self, value: Union[BrowserEngine, str]):
+        self._browser_engine = BrowserEngine(value)
+
+    @property
+    def install(self) -> Optional[bool]:
+        return self._install
+
+    @install.setter
+    def install(self, value: Optional[bool]):
+        assert value is None or isinstance(value, bool)
+        self._install = value
 
     @property
     def headless(self) -> Optional[bool]:
         return self._headless
 
     @headless.setter
     def headless(self, value: Optional[bool]):
@@ -164,57 +145,73 @@
     if slowmo_option:
         launch_options["slow_mo"] = slowmo_option
     return launch_options
 
 
 @session_cache
 def playwright() -> Iterator[Playwright]:
+    # Make sure playwright searches from robocorp-specific path
+    os.environ["PLAYWRIGHT_BROWSERS_PATH"] = str(browsers_path())
+
     pw = sync_playwright().start()
     yield pw
     # Need to stop when tasks finish running.
     pw.stop()
 
 
 @session_cache
 def _browser_type() -> BrowserType:
     pw = playwright()
 
     engine = _browser_config().browser_engine
-    if engine == "chrome":
-        engine = "chromium"
+    klass, _ = ENGINE_TO_ARGS[engine]
 
-    return getattr(pw, engine)
+    return getattr(pw, klass)
 
 
 @session_cache
 def _browser_launcher() -> Callable[..., Browser]:
     browser_type: BrowserType = _browser_type()
 
     def launch(**kwargs: Dict) -> Browser:
         launch_options = {**browser_type_launch_args(), **kwargs}
 
-        if "executable_path" not in launch_options:
+        if "channel" not in launch_options:
             engine = _browser_config().browser_engine
-            launch_options["executable_path"] = _get_executable_path(engine)
+            _, channel = ENGINE_TO_ARGS[engine]
+            if channel is not None:
+                launch_options["channel"] = channel
 
         browser = browser_type.launch(**launch_options)
         return browser
 
     return launch
 
 
 @session_cache
 def browser(**kwargs) -> Iterator[Browser]:
     """
     The kwargs are passed as additional launch options to the
     BrowserType.launch(**kwargs).
     """
     # Note: one per session (must be tear-down).
+    config = _browser_config()
+    if config.install:
+        install_browser(config.browser_engine)
+
     launcher = _browser_launcher()
-    browser = launcher(**kwargs)
+    try:
+        browser = launcher(**kwargs)
+    except Error:
+        if config.install is None:
+            install_browser(config.browser_engine)
+            browser = launcher(**kwargs)
+        else:
+            raise
+
     yield browser
     browser.close()
 
 
 @task_cache
 def context(**browser_context_kwargs) -> Iterator[BrowserContext]:
     from robocorp.tasks import get_current_task
```

### Comparing `robocorp_browser-0.4.4/PKG-INFO` & `robocorp_browser-1.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robocorp-browser
-Version: 0.4.4
+Version: 1.0.0
 Summary: Robocorp browser automation library
 Author: Fabio Z.
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

