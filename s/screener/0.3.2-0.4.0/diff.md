# Comparing `tmp/screener-0.3.2.tar.gz` & `tmp/screener-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screener-0.3.2.tar", max compression
+gzip compressed data, was "screener-0.4.0.tar", max compression
```

## Comparing `screener-0.3.2.tar` & `screener-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1919 2023-06-07 19:00:57.528329 screener-0.3.2/README.md
--rw-r--r--   0        0        0     2514 2023-06-07 19:35:11.668394 screener-0.3.2/pyproject.toml
--rw-r--r--   0        0        0       25 2023-05-21 15:27:52.900285 screener-0.3.2/screener/__init__.py
--rw-r--r--   0        0        0     2614 2023-06-07 19:35:11.668394 screener-0.3.2/screener/__main__.py
--rw-r--r--   0        0        0      554 2023-06-07 19:00:57.535328 screener-0.3.2/screener/diagnostic.py
--rw-r--r--   0        0        0      157 2023-05-21 15:59:46.200712 screener-0.3.2/screener/parser/__init__.py
--rw-r--r--   0        0        0      935 2023-06-07 19:00:57.535328 screener-0.3.2/screener/parser/epub.py
--rw-r--r--   0        0        0     1332 2023-06-07 19:00:57.535328 screener-0.3.2/screener/parser/kindle.py
--rw-r--r--   0        0        0      150 2023-05-21 15:59:46.200712 screener-0.3.2/screener/reader/__init__.py
--rw-r--r--   0        0        0      819 2023-05-21 15:27:52.900285 screener-0.3.2/screener/reader/abstract.py
--rw-r--r--   0        0        0      796 2023-06-07 19:00:57.535328 screener-0.3.2/screener/reader/epub.py
--rw-r--r--   0        0        0     1379 2023-05-23 18:36:01.147752 screener-0.3.2/screener/reader/kindle.py
--rw-r--r--   0        0        0      675 2023-05-22 10:19:24.693693 screener-0.3.2/screener/utils.py
--rw-r--r--   0        0        0     2848 1970-01-01 00:00:00.000000 screener-0.3.2/setup.py
--rw-r--r--   0        0        0     2693 1970-01-01 00:00:00.000000 screener-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1808 2023-06-09 12:49:06.826100 screener-0.4.0/README.md
+-rw-r--r--   0        0        0     2514 2023-06-09 12:49:06.826100 screener-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       25 2023-05-21 15:27:52.900285 screener-0.4.0/screener/__init__.py
+-rw-r--r--   0        0        0     1987 2023-06-09 12:49:06.826100 screener-0.4.0/screener/__main__.py
+-rw-r--r--   0        0        0      313 2023-06-09 12:49:06.826100 screener-0.4.0/screener/checker.py
+-rw-r--r--   0        0        0      859 2023-06-09 12:49:06.827100 screener-0.4.0/screener/diagnostic.py
+-rw-r--r--   0        0        0      157 2023-05-21 15:59:46.200712 screener-0.4.0/screener/parser/__init__.py
+-rw-r--r--   0        0        0      960 2023-06-09 12:49:06.827100 screener-0.4.0/screener/parser/epub.py
+-rw-r--r--   0        0        0      902 2023-06-09 12:49:06.827100 screener-0.4.0/screener/parser/kindle.py
+-rw-r--r--   0        0        0      150 2023-05-21 15:59:46.200712 screener-0.4.0/screener/reader/__init__.py
+-rw-r--r--   0        0        0      819 2023-05-21 15:27:52.900285 screener-0.4.0/screener/reader/abstract.py
+-rw-r--r--   0        0        0      796 2023-06-07 19:00:57.535328 screener-0.4.0/screener/reader/epub.py
+-rw-r--r--   0        0        0     1379 2023-05-23 18:36:01.147752 screener-0.4.0/screener/reader/kindle.py
+-rw-r--r--   0        0        0     1040 2023-06-09 12:49:06.827100 screener-0.4.0/screener/utils.py
+-rw-r--r--   0        0        0     2737 1970-01-01 00:00:00.000000 screener-0.4.0/setup.py
+-rw-r--r--   0        0        0     2584 1970-01-01 00:00:00.000000 screener-0.4.0/PKG-INFO
```

### Comparing `screener-0.3.2/README.md` & `screener-0.4.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # Screener
 
 Check e-book files for security and privacy issues.
 
-_Screener is currently in early development. Please consider contributing if you have the time and know-how!_
-
 ## Motivation
 
 E-books are great, but the common file formats have security and privacy issues. Most use web browser technologies like HTML, CSS, and JavaScript. Therefore, e-books are vulnerable to security and privacy issues that already exist on the web.
 
 Screener aims to check e-book files for these issues so that you can read with peace of mind!
 
 ## Features
@@ -22,15 +20,15 @@
 
 ### Prerequisites
 
 Screener requires [Python](https://www.python.org/about/gettingstarted/) (version 3.10 or newer).
 
 ### Installing
 
-Screen is available on [PyPI](https://pypi.org/project/screener/). To install, run:
+Screener is available on [PyPI](https://pypi.org/project/screener/). To install, run:
 
 ```bash
 pip install screener
 ```
 
 #### Development installation
```

### Comparing `screener-0.3.2/pyproject.toml` & `screener-0.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Screener"
-version = "0.3.2"
+version = "0.4.0"
 description = "Check e-book files for security and privacy issues."
 authors = ["Tom Kuson <mail@tjkuson.me>"]
 license = "LGPL-3.0-only"
 readme = "README.md"
 packages = [
     { include = "screener", from = "." },
 ]
```

### Comparing `screener-0.3.2/screener/parser/epub.py` & `screener-0.4.0/screener/parser/epub.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 """Parse epub file to check that it is safe."""
 
 from pathlib import Path
 
 from ebooklib import ITEM_DOCUMENT
 
-from screener.diagnostic import ExternalImageDiagnostic, JavaScriptDiagnostic
+from screener.checker import Checker
 from screener.reader import EpubFileReader
 from screener.utils import (
     html_contains_images_with_external_sources,
     html_contains_javascript,
 )
 
 
 def parse_epub(
+    checker: Checker,
     path_to_epub: Path,
-) -> JavaScriptDiagnostic | ExternalImageDiagnostic | None:
-    """Parse epub to check that it is safe."""
+) -> None:
+    """Parse epub to check that it is safe.
+
+    Mutates the checker object to add diagnostics.
+    """
     with EpubFileReader(path_to_epub) as epub:
         for item in epub.book.get_items_of_type(ITEM_DOCUMENT):
             content = item.get_content()
-            if html_contains_javascript(content):
-                return JavaScriptDiagnostic(path_to_epub.name)
-            if html_contains_images_with_external_sources(content):
-                return ExternalImageDiagnostic(path_to_epub.name)
-        return None
+            if js := html_contains_javascript(checker, content):
+                checker.diagnostics.extend(js)
+            if external_images := html_contains_images_with_external_sources(
+                checker, content
+            ):
+                checker.diagnostics.extend(external_images)
```

### Comparing `screener-0.3.2/screener/parser/kindle.py` & `screener-0.4.0/screener/parser/kindle.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,28 @@
 """Parse kindle files."""
 
 from pathlib import Path
 
-from screener.diagnostic import (
-    ExternalImageDiagnostic,
-    JavaScriptDiagnostic,
-    ParseErrorDiagnostic,
-)
+from screener.checker import Checker
 from screener.reader.kindle import KindleFileReader
 
 from .epub import parse_epub
 
 
 def parse_kindle(
+    checker: Checker,
     path_to_kindle: Path | None,
-) -> JavaScriptDiagnostic | ExternalImageDiagnostic | ParseErrorDiagnostic | None:
+) -> None:
     """Parse kindle to check that it is safe."""
     if path_to_kindle is None:
         msg = "path_to_kindle cannot be None"
         raise ValueError(msg)
     with KindleFileReader(path_to_kindle) as kindle:
         if kindle.generated_translation is None:
-            return ParseErrorDiagnostic(
-                path_to_kindle.name, "failed to generate translation"
-            )
+            msg = "generated_translation cannot be None"
+            raise FileNotFoundError(msg)
         extension = Path(kindle.generated_translation).suffix
         match extension:
             case ".epub":
                 epub_translation = Path(kindle.generated_translation)
-                if (diagnostic := parse_epub(epub_translation)) is not None:
-                    diagnostic.file_name = path_to_kindle.name
-                    return diagnostic
-                return None
-
-        # If failed to parse, assume it is unsafe.
-        return ParseErrorDiagnostic(path_to_kindle.name, "could not process file")
+                parse_epub(checker, epub_translation)
+                return
```

### Comparing `screener-0.3.2/screener/reader/abstract.py` & `screener-0.4.0/screener/reader/abstract.py`

 * *Files identical despite different names*

### Comparing `screener-0.3.2/screener/reader/epub.py` & `screener-0.4.0/screener/reader/epub.py`

 * *Files identical despite different names*

### Comparing `screener-0.3.2/screener/reader/kindle.py` & `screener-0.4.0/screener/reader/kindle.py`

 * *Files identical despite different names*

### Comparing `screener-0.3.2/screener/utils.py` & `screener-0.4.0/screener/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 """Screener utility functions."""
 
-import logging
 
 from bs4 import BeautifulSoup
 
+from screener.checker import Checker
+from screener.diagnostic import ExternalImageDiagnostic, JavaScriptDiagnostic
 
-def html_contains_javascript(content: bytes) -> bool:
-    """Search for JavaScript in html files."""
+
+def html_contains_javascript(
+    checker: Checker, content: bytes
+) -> list[JavaScriptDiagnostic] | None:
+    """Check if HTML contains JavaScript."""
     soup = BeautifulSoup(content, "html.parser")
     if scripts := soup.find_all("script"):
-        logging.info("scripts detected: %s", scripts)
-        return True
-    return False
+        return [JavaScriptDiagnostic(checker.file_path.name) for _ in scripts]
+    return None
 
 
-def html_contains_images_with_external_sources(content: bytes) -> bool:
-    """Search for images with external sources in html files."""
+def html_contains_images_with_external_sources(
+    checker: Checker, content: bytes
+) -> list[ExternalImageDiagnostic] | None:
+    """Check if HTML contains images with external sources."""
     soup = BeautifulSoup(content, "html.parser")
     images = soup.find_all("img")
-    return any(i for i in images if i["src"].startswith("http"))
+    if external_images := tuple(i for i in images if i["src"].startswith("http")):
+        return [
+            ExternalImageDiagnostic(checker.file_path.name) for _ in external_images
+        ]
+    return None
```

### Comparing `screener-0.3.2/setup.py` & `screener-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 ['EbookLib>=0.18,<0.19', 'beautifulsoup4>=4.12.2,<5.0.0', 'mobi>=0.3.3,<0.4.0']
 
 entry_points = \
 {'console_scripts': ['screener = screener.__main__:main']}
 
 setup_kwargs = {
     'name': 'screener',
-    'version': '0.3.2',
+    'version': '0.4.0',
     'description': 'Check e-book files for security and privacy issues.',
-    'long_description': '# Screener\n\nCheck e-book files for security and privacy issues.\n\n_Screener is currently in early development. Please consider contributing if you have the time and know-how!_\n\n## Motivation\n\nE-books are great, but the common file formats have security and privacy issues. Most use web browser technologies like HTML, CSS, and JavaScript. Therefore, e-books are vulnerable to security and privacy issues that already exist on the web.\n\nScreener aims to check e-book files for these issues so that you can read with peace of mind!\n\n## Features\n\n- Check e-book files for JavaScript tags.\n- Check e-book files for images with external sources to prevent tracking.\n- Supports `.epub`, `.mobi`, and `.azw3` files.\n\n## Get started\n\nThese instructions will get you a copy of the project up and running on your local machine for development and testing purposes.\n\n### Prerequisites\n\nScreener requires [Python](https://www.python.org/about/gettingstarted/) (version 3.10 or newer).\n\n### Installing\n\nScreen is available on [PyPI](https://pypi.org/project/screener/). To install, run:\n\n```bash\npip install screener\n```\n\n#### Development installation\n\nTo install Screener for development, ensure you have [Poetry](https://python-poetry.org/) clone the repository and run:\n\n```bash\npoetry install\n```\n\n## Contributing\n\nPull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.\n\nAt present, this project is in early development and needs extra security and privacy checks and wider file format support more than anything else.\n\nPlease make sure to update tests as appropriate.\n\n## Versioning\n\nThis project uses [SemVer](http://semver.org/) for versioning.\n\n## Authors\n\nScreener was created by Tom Kuson ([@tjkuson](https://github.com/tjkuson)).\n\n## Licence\n\nScreener is released under the [LGPL version 3](LICENCE).\n',
+    'long_description': '# Screener\n\nCheck e-book files for security and privacy issues.\n\n## Motivation\n\nE-books are great, but the common file formats have security and privacy issues. Most use web browser technologies like HTML, CSS, and JavaScript. Therefore, e-books are vulnerable to security and privacy issues that already exist on the web.\n\nScreener aims to check e-book files for these issues so that you can read with peace of mind!\n\n## Features\n\n- Check e-book files for JavaScript tags.\n- Check e-book files for images with external sources to prevent tracking.\n- Supports `.epub`, `.mobi`, and `.azw3` files.\n\n## Get started\n\nThese instructions will get you a copy of the project up and running on your local machine for development and testing purposes.\n\n### Prerequisites\n\nScreener requires [Python](https://www.python.org/about/gettingstarted/) (version 3.10 or newer).\n\n### Installing\n\nScreener is available on [PyPI](https://pypi.org/project/screener/). To install, run:\n\n```bash\npip install screener\n```\n\n#### Development installation\n\nTo install Screener for development, ensure you have [Poetry](https://python-poetry.org/) clone the repository and run:\n\n```bash\npoetry install\n```\n\n## Contributing\n\nPull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.\n\nAt present, this project is in early development and needs extra security and privacy checks and wider file format support more than anything else.\n\nPlease make sure to update tests as appropriate.\n\n## Versioning\n\nThis project uses [SemVer](http://semver.org/) for versioning.\n\n## Authors\n\nScreener was created by Tom Kuson ([@tjkuson](https://github.com/tjkuson)).\n\n## Licence\n\nScreener is released under the [LGPL version 3](LICENCE).\n',
     'author': 'Tom Kuson',
     'author_email': 'mail@tjkuson.me',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/tjkuson/screener/',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `screener-0.3.2/PKG-INFO` & `screener-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screener
-Version: 0.3.2
+Version: 0.4.0
 Summary: Check e-book files for security and privacy issues.
 Home-page: https://github.com/tjkuson/screener/
 License: LGPL-3.0-only
 Keywords: ebook,security,privacy,epub,mobi,kindle
 Author: Tom Kuson
 Author-email: mail@tjkuson.me
 Requires-Python: >=3.10,<4.0
@@ -20,16 +20,14 @@
 Project-URL: Repository, https://github.com/tjkuson/screener/
 Description-Content-Type: text/markdown
 
 # Screener
 
 Check e-book files for security and privacy issues.
 
-_Screener is currently in early development. Please consider contributing if you have the time and know-how!_
-
 ## Motivation
 
 E-books are great, but the common file formats have security and privacy issues. Most use web browser technologies like HTML, CSS, and JavaScript. Therefore, e-books are vulnerable to security and privacy issues that already exist on the web.
 
 Screener aims to check e-book files for these issues so that you can read with peace of mind!
 
 ## Features
@@ -44,15 +42,15 @@
 
 ### Prerequisites
 
 Screener requires [Python](https://www.python.org/about/gettingstarted/) (version 3.10 or newer).
 
 ### Installing
 
-Screen is available on [PyPI](https://pypi.org/project/screener/). To install, run:
+Screener is available on [PyPI](https://pypi.org/project/screener/). To install, run:
 
 ```bash
 pip install screener
 ```
 
 #### Development installation
```

