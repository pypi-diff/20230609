# Comparing `tmp/get-chrome-driver-1.3.8.tar.gz` & `tmp/get-chrome-driver-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "get-chrome-driver-1.3.8.tar", last modified: Tue Oct  4 05:48:37 2022, max compression
+gzip compressed data, was "get-chrome-driver-1.3.9.tar", last modified: Tue Oct  4 06:20:40 2022, max compression
```

## Comparing `get-chrome-driver-1.3.8.tar` & `get-chrome-driver-1.3.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2022-10-04 05:48:37.260450 get-chrome-driver-1.3.8/
--rw-rw-rw-   0        0        0     1091 2022-09-28 01:58:24.000000 get-chrome-driver-1.3.8/LICENSE
--rw-rw-rw-   0        0        0     5229 2022-10-04 05:48:37.261449 get-chrome-driver-1.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     4440 2022-10-03 03:05:14.000000 get-chrome-driver-1.3.8/README.md
-drwxrwxrwx   0        0        0        0 2022-10-04 05:48:37.219454 get-chrome-driver-1.3.8/get_chrome_driver/
--rw-rw-rw-   0        0        0       66 2022-10-04 03:39:08.000000 get-chrome-driver-1.3.8/get_chrome_driver/__init__.py
--rw-rw-rw-   0        0        0     7599 2022-10-04 03:42:08.000000 get-chrome-driver-1.3.8/get_chrome_driver/app.py
--rw-rw-rw-   0        0        0      278 2022-09-28 01:52:24.000000 get-chrome-driver-1.3.8/get_chrome_driver/constants.py
--rw-rw-rw-   0        0        0     2492 2022-10-04 03:48:42.000000 get-chrome-driver-1.3.8/get_chrome_driver/downloader.py
-drwxrwxrwx   0        0        0        0 2022-10-04 05:48:37.257475 get-chrome-driver-1.3.8/get_chrome_driver/enums/
--rw-rw-rw-   0        0        0       58 2022-09-19 07:56:53.000000 get-chrome-driver-1.3.8/get_chrome_driver/enums/__init__.py
--rw-rw-rw-   0        0        0       94 2022-09-19 07:56:53.000000 get-chrome-driver-1.3.8/get_chrome_driver/enums/phase.py
--rw-rw-rw-   0        0        0      244 2022-09-19 07:56:53.000000 get-chrome-driver-1.3.8/get_chrome_driver/enums/platform.py
--rw-rw-rw-   0        0        0      354 2022-09-19 07:21:46.000000 get-chrome-driver-1.3.8/get_chrome_driver/exceptions.py
--rw-rw-rw-   0        0        0    12720 2022-10-04 03:43:52.000000 get-chrome-driver-1.3.8/get_chrome_driver/get_driver.py
-drwxrwxrwx   0        0        0        0 2022-10-04 05:48:37.259455 get-chrome-driver-1.3.8/get_chrome_driver/test/
--rw-rw-rw-   0        0        0        0 2022-09-19 07:21:46.000000 get-chrome-driver-1.3.8/get_chrome_driver/test/__init__.py
--rw-rw-rw-   0        0        0     6837 2022-10-03 02:53:57.000000 get-chrome-driver-1.3.8/get_chrome_driver/test/test_app.py
-drwxrwxrwx   0        0        0        0 2022-10-04 05:48:37.239450 get-chrome-driver-1.3.8/get_chrome_driver.egg-info/
--rw-rw-rw-   0        0        0     5229 2022-10-04 05:48:37.000000 get-chrome-driver-1.3.8/get_chrome_driver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      641 2022-10-04 05:48:37.000000 get-chrome-driver-1.3.8/get_chrome_driver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-04 05:48:37.000000 get-chrome-driver-1.3.8/get_chrome_driver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2022-10-04 05:48:37.000000 get-chrome-driver-1.3.8/get_chrome_driver.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       58 2022-10-04 05:48:37.000000 get-chrome-driver-1.3.8/get_chrome_driver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2022-10-04 05:48:37.000000 get-chrome-driver-1.3.8/get_chrome_driver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      133 2022-10-04 05:48:37.262446 get-chrome-driver-1.3.8/setup.cfg
--rw-rw-rw-   0        0        0     1296 2022-10-04 03:39:08.000000 get-chrome-driver-1.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-10-04 06:20:40.018454 get-chrome-driver-1.3.9/
+-rw-rw-rw-   0        0        0     1091 2022-09-28 01:58:24.000000 get-chrome-driver-1.3.9/LICENSE
+-rw-rw-rw-   0        0        0     5229 2022-10-04 06:20:40.018454 get-chrome-driver-1.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4440 2022-10-03 03:05:14.000000 get-chrome-driver-1.3.9/README.md
+drwxrwxrwx   0        0        0        0 2022-10-04 06:20:39.993457 get-chrome-driver-1.3.9/get_chrome_driver/
+-rw-rw-rw-   0        0        0       66 2022-10-04 06:20:18.000000 get-chrome-driver-1.3.9/get_chrome_driver/__init__.py
+-rw-rw-rw-   0        0        0     7599 2022-10-04 03:42:08.000000 get-chrome-driver-1.3.9/get_chrome_driver/app.py
+-rw-rw-rw-   0        0        0      278 2022-09-28 01:52:24.000000 get-chrome-driver-1.3.9/get_chrome_driver/constants.py
+-rw-rw-rw-   0        0        0     2478 2022-10-04 06:20:18.000000 get-chrome-driver-1.3.9/get_chrome_driver/downloader.py
+drwxrwxrwx   0        0        0        0 2022-10-04 06:20:40.015455 get-chrome-driver-1.3.9/get_chrome_driver/enums/
+-rw-rw-rw-   0        0        0       58 2022-09-19 07:56:53.000000 get-chrome-driver-1.3.9/get_chrome_driver/enums/__init__.py
+-rw-rw-rw-   0        0        0       94 2022-09-19 07:56:53.000000 get-chrome-driver-1.3.9/get_chrome_driver/enums/phase.py
+-rw-rw-rw-   0        0        0      244 2022-09-19 07:56:53.000000 get-chrome-driver-1.3.9/get_chrome_driver/enums/platform.py
+-rw-rw-rw-   0        0        0      354 2022-09-19 07:21:46.000000 get-chrome-driver-1.3.9/get_chrome_driver/exceptions.py
+-rw-rw-rw-   0        0        0    12685 2022-10-04 06:20:18.000000 get-chrome-driver-1.3.9/get_chrome_driver/get_driver.py
+drwxrwxrwx   0        0        0        0 2022-10-04 06:20:40.017454 get-chrome-driver-1.3.9/get_chrome_driver/test/
+-rw-rw-rw-   0        0        0        0 2022-09-19 07:21:46.000000 get-chrome-driver-1.3.9/get_chrome_driver/test/__init__.py
+-rw-rw-rw-   0        0        0     6837 2022-10-03 02:53:57.000000 get-chrome-driver-1.3.9/get_chrome_driver/test/test_app.py
+drwxrwxrwx   0        0        0        0 2022-10-04 06:20:40.011450 get-chrome-driver-1.3.9/get_chrome_driver.egg-info/
+-rw-rw-rw-   0        0        0     5229 2022-10-04 06:20:39.000000 get-chrome-driver-1.3.9/get_chrome_driver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      641 2022-10-04 06:20:39.000000 get-chrome-driver-1.3.9/get_chrome_driver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-10-04 06:20:39.000000 get-chrome-driver-1.3.9/get_chrome_driver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2022-10-04 06:20:39.000000 get-chrome-driver-1.3.9/get_chrome_driver.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       58 2022-10-04 06:20:39.000000 get-chrome-driver-1.3.9/get_chrome_driver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2022-10-04 06:20:39.000000 get-chrome-driver-1.3.9/get_chrome_driver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      133 2022-10-04 06:20:40.023455 get-chrome-driver-1.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     1296 2022-10-04 06:20:18.000000 get-chrome-driver-1.3.9/setup.py
```

### Comparing `get-chrome-driver-1.3.8/LICENSE` & `get-chrome-driver-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `get-chrome-driver-1.3.8/PKG-INFO` & `get-chrome-driver-1.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: get-chrome-driver
-Version: 1.3.8
+Version: 1.3.9
 Summary: A tool to download and install ChromeDriver.
 Home-page: https://github.com/zaironjacobs/get-chrome-driver
-Download-URL: https://github.com/zaironjacobs/get-chrome-driver/archive/v1.3.8.tar.gz
+Download-URL: https://github.com/zaironjacobs/get-chrome-driver/archive/v1.3.9.tar.gz
 Author: Zairon Jacobs
 Author-email: zaironjacobs@gmail.com
 License: MIT
 Keywords: chrome,chromedriver,download,install,web,driver,tool
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `get-chrome-driver-1.3.8/README.md` & `get-chrome-driver-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `get-chrome-driver-1.3.8/get_chrome_driver/app.py` & `get-chrome-driver-1.3.9/get_chrome_driver/app.py`

 * *Files identical despite different names*

### Comparing `get-chrome-driver-1.3.8/get_chrome_driver/downloader.py` & `get-chrome-driver-1.3.9/get_chrome_driver/downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from urllib3.util.retry import Retry
 from requests.adapters import HTTPAdapter
 from urllib.parse import urlparse
 from requests.exceptions import RequestException
 from requests.exceptions import HTTPError
 
 
-def download(url: str, output_path: str | None = None, file_name: str | None = None):
+def download(url: str, output_path: str = None, file_name: str = None):
     """
     Download a file from url
     If output_path is None, the file will be downloaded directly at the current directory
     If file_name is None, the file name from the url will be used
     """
 
     session = __retry_session(retries=3,
```

### Comparing `get-chrome-driver-1.3.8/get_chrome_driver/get_driver.py` & `get-chrome-driver-1.3.9/get_chrome_driver/get_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from .enums import Platform, Phase
 from .exceptions import GetChromeDriverError, UnknownPlatformError, VersionUrlError, UnknownVersionError, \
     DownloadError, VersionError
 
 
 class GetChromeDriver:
 
-    def __init__(self, platform: Platform | None = None):
+    def __init__(self, platform: Platform = None):
         if not platform:
             if pl.system() == 'Windows':
                 self.__platform = self.__check_platform(Platform.win)
             elif pl.system() == 'Linux':
                 self.__platform = self.__check_platform(Platform.linux)
             elif pl.system() == 'Darwin':
                 self.__platform = self.__check_platform(Platform.mac)
@@ -135,37 +135,37 @@
                     # No 64 bit, get 32 bit
                     pass
             # 32bit
             url = f'{constants.url_chromedriver_storage}/{version}/{chromedriver}_{Platform.mac32}{zip_ext}'
             self.__check_if_url_is_valid(url)
             return url
 
-    def download_stable_version(self, output_path: str | None = None, extract: bool = False):
+    def download_stable_version(self, output_path: str = None, extract: bool = False):
         """
         Download the latest stable chromedriver version
 
         :param output_path: Path to download the driver to
         :param extract: Extract the downloaded driver or not
         """
 
         version = self.__latest_version_by_phase(Phase.stable)
         self.download_version(version=version, output_path=output_path, extract=extract)
 
-    def download_beta_version(self, output_path: str | None = None, extract: bool = False):
+    def download_beta_version(self, output_path: str = None, extract: bool = False):
         """
         Download the latest beta chromedriver version
 
         :param output_path: Path to download the driver to
         :param extract: Extract the downloaded driver or not
         """
 
         version = self.__latest_version_by_phase(Phase.beta)
         self.download_version(version=version, output_path=output_path, extract=extract)
 
-    def download_version(self, version, output_path: str | None = None, extract: bool = False) -> str:
+    def download_version(self, version, output_path: str = None, extract: bool = False) -> str:
         """
         Download a chromedriver version
 
         :param version: Chromedriver version
         :param output_path: Path to download the driver to
         :param extract: Extract the downloaded driver or not
         """
@@ -236,15 +236,15 @@
 
         all_chromedriver_versions = self.__get_all_chromedriver_versions()
         installed_chrome_version = self.__get_installed_chrome_version()
         for chromedriver_version in reversed(all_chromedriver_versions):
             if '.'.join(installed_chrome_version.split('.')[:-1]) == '.'.join(chromedriver_version.split('.')[:-1]):
                 return chromedriver_version
 
-    def auto_download(self, output_path: str | None = None, extract: bool = False) -> str:
+    def auto_download(self, output_path: str = None, extract: bool = False) -> str:
         """
         Download ChromeDriver for the installed Chrome version on machine
 
         :param output_path: Path to download the driver to
         :param extract: Extract the downloaded driver or not
         """
```

### Comparing `get-chrome-driver-1.3.8/get_chrome_driver/test/test_app.py` & `get-chrome-driver-1.3.9/get_chrome_driver/test/test_app.py`

 * *Files identical despite different names*

### Comparing `get-chrome-driver-1.3.8/get_chrome_driver.egg-info/PKG-INFO` & `get-chrome-driver-1.3.9/get_chrome_driver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: get-chrome-driver
-Version: 1.3.8
+Version: 1.3.9
 Summary: A tool to download and install ChromeDriver.
 Home-page: https://github.com/zaironjacobs/get-chrome-driver
-Download-URL: https://github.com/zaironjacobs/get-chrome-driver/archive/v1.3.8.tar.gz
+Download-URL: https://github.com/zaironjacobs/get-chrome-driver/archive/v1.3.9.tar.gz
 Author: Zairon Jacobs
 Author-email: zaironjacobs@gmail.com
 License: MIT
 Keywords: chrome,chromedriver,download,install,web,driver,tool
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `get-chrome-driver-1.3.8/get_chrome_driver.egg-info/SOURCES.txt` & `get-chrome-driver-1.3.9/get_chrome_driver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `get-chrome-driver-1.3.8/setup.py` & `get-chrome-driver-1.3.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 from setuptools import find_packages
 
 name = 'get-chrome-driver'
-version = '1.3.8'
+version = '1.3.9'
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 requires = [
     'bs4>=0.0.1',
     'requests>=2.28.1',
```

