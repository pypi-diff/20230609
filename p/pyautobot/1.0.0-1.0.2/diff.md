# Comparing `tmp/pyautobot-1.0.0.tar.gz` & `tmp/pyautobot-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyautobot-1.0.0.tar", last modified: Fri Jun  9 12:24:21 2023, max compression
+gzip compressed data, was "pyautobot-1.0.2.tar", last modified: Fri Jun  9 12:57:22 2023, max compression
```

## Comparing `pyautobot-1.0.0.tar` & `pyautobot-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 rain       (501) staff       (20)        0 2023-06-09 12:24:21.146043 pyautobot-1.0.0/
--rw-r--r--   0 rain       (501) staff       (20)     1483 2023-06-09 11:37:33.000000 pyautobot-1.0.0/LICENSE
--rw-r--r--   0 rain       (501) staff       (20)     1414 2023-06-09 12:24:21.145911 pyautobot-1.0.0/PKG-INFO
--rw-r--r--   0 rain       (501) staff       (20)    11347 2023-06-09 11:35:50.000000 pyautobot-1.0.0/README.md
-drwxr-xr-x   0 rain       (501) staff       (20)        0 2023-06-09 12:24:21.144391 pyautobot-1.0.0/bin/
--rwxr-xr-x   0 rain       (501) staff       (20)      348 2023-06-09 11:54:04.000000 pyautobot-1.0.0/bin/pyautobot
-drwxr-xr-x   0 rain       (501) staff       (20)        0 2023-06-09 12:24:21.145038 pyautobot-1.0.0/pyautobot/
--rw-r--r--   0 rain       (501) staff       (20)     3182 2023-06-09 11:57:14.000000 pyautobot-1.0.0/pyautobot/__init__.py
--rw-r--r--   0 rain       (501) staff       (20)     6732 2023-06-09 11:56:45.000000 pyautobot-1.0.0/pyautobot/chrome.py
--rw-r--r--   0 rain       (501) staff       (20)     1825 2023-06-09 11:02:12.000000 pyautobot-1.0.0/pyautobot/gui.py
--rw-r--r--   0 rain       (501) staff       (20)     6860 2023-06-09 11:03:20.000000 pyautobot-1.0.0/pyautobot/images.py
--rw-r--r--   0 rain       (501) staff       (20)     2632 2023-06-09 10:57:27.000000 pyautobot-1.0.0/pyautobot/ocr.py
--rw-r--r--   0 rain       (501) staff       (20)      329 2023-06-09 10:57:27.000000 pyautobot-1.0.0/pyautobot/utils.py
-drwxr-xr-x   0 rain       (501) staff       (20)        0 2023-06-09 12:24:21.145732 pyautobot-1.0.0/pyautobot.egg-info/
--rw-r--r--   0 rain       (501) staff       (20)     1414 2023-06-09 12:24:21.000000 pyautobot-1.0.0/pyautobot.egg-info/PKG-INFO
--rw-r--r--   0 rain       (501) staff       (20)      319 2023-06-09 12:24:21.000000 pyautobot-1.0.0/pyautobot.egg-info/SOURCES.txt
--rw-r--r--   0 rain       (501) staff       (20)        1 2023-06-09 12:24:21.000000 pyautobot-1.0.0/pyautobot.egg-info/dependency_links.txt
--rw-r--r--   0 rain       (501) staff       (20)       69 2023-06-09 12:24:21.000000 pyautobot-1.0.0/pyautobot.egg-info/requires.txt
--rw-r--r--   0 rain       (501) staff       (20)       10 2023-06-09 12:24:21.000000 pyautobot-1.0.0/pyautobot.egg-info/top_level.txt
--rw-r--r--   0 rain       (501) staff       (20)       38 2023-06-09 12:24:21.146080 pyautobot-1.0.0/setup.cfg
--rw-r--r--   0 rain       (501) staff       (20)     1812 2023-06-09 11:58:09.000000 pyautobot-1.0.0/setup.py
+drwxr-xr-x   0 rain       (501) staff       (20)        0 2023-06-09 12:57:22.534052 pyautobot-1.0.2/
+-rw-r--r--   0 rain       (501) staff       (20)     1483 2023-06-09 11:37:33.000000 pyautobot-1.0.2/LICENSE
+-rw-r--r--   0 rain       (501) staff       (20)     1414 2023-06-09 12:57:22.533928 pyautobot-1.0.2/PKG-INFO
+-rw-r--r--   0 rain       (501) staff       (20)    12037 2023-06-09 12:50:47.000000 pyautobot-1.0.2/README.md
+drwxr-xr-x   0 rain       (501) staff       (20)        0 2023-06-09 12:57:22.532582 pyautobot-1.0.2/bin/
+-rwxr-xr-x   0 rain       (501) staff       (20)      348 2023-06-09 11:54:04.000000 pyautobot-1.0.2/bin/pyautobot
+drwxr-xr-x   0 rain       (501) staff       (20)        0 2023-06-09 12:57:22.533220 pyautobot-1.0.2/pyautobot/
+-rw-r--r--   0 rain       (501) staff       (20)     3182 2023-06-09 12:28:52.000000 pyautobot-1.0.2/pyautobot/__init__.py
+-rw-r--r--   0 rain       (501) staff       (20)     6969 2023-06-09 12:51:05.000000 pyautobot-1.0.2/pyautobot/chrome.py
+-rw-r--r--   0 rain       (501) staff       (20)     1825 2023-06-09 11:02:12.000000 pyautobot-1.0.2/pyautobot/gui.py
+-rw-r--r--   0 rain       (501) staff       (20)     6860 2023-06-09 11:03:20.000000 pyautobot-1.0.2/pyautobot/images.py
+-rw-r--r--   0 rain       (501) staff       (20)     2632 2023-06-09 10:57:27.000000 pyautobot-1.0.2/pyautobot/ocr.py
+-rw-r--r--   0 rain       (501) staff       (20)      329 2023-06-09 10:57:27.000000 pyautobot-1.0.2/pyautobot/utils.py
+drwxr-xr-x   0 rain       (501) staff       (20)        0 2023-06-09 12:57:22.533771 pyautobot-1.0.2/pyautobot.egg-info/
+-rw-r--r--   0 rain       (501) staff       (20)     1414 2023-06-09 12:57:22.000000 pyautobot-1.0.2/pyautobot.egg-info/PKG-INFO
+-rw-r--r--   0 rain       (501) staff       (20)      319 2023-06-09 12:57:22.000000 pyautobot-1.0.2/pyautobot.egg-info/SOURCES.txt
+-rw-r--r--   0 rain       (501) staff       (20)        1 2023-06-09 12:57:22.000000 pyautobot-1.0.2/pyautobot.egg-info/dependency_links.txt
+-rw-r--r--   0 rain       (501) staff       (20)       69 2023-06-09 12:57:22.000000 pyautobot-1.0.2/pyautobot.egg-info/requires.txt
+-rw-r--r--   0 rain       (501) staff       (20)       10 2023-06-09 12:57:22.000000 pyautobot-1.0.2/pyautobot.egg-info/top_level.txt
+-rw-r--r--   0 rain       (501) staff       (20)       38 2023-06-09 12:57:22.534102 pyautobot-1.0.2/setup.cfg
+-rw-r--r--   0 rain       (501) staff       (20)     1812 2023-06-09 12:57:00.000000 pyautobot-1.0.2/setup.py
```

### Comparing `pyautobot-1.0.0/LICENSE` & `pyautobot-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyautobot-1.0.0/PKG-INFO` & `pyautobot-1.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyautobot
-Version: 1.0.0
+Version: 1.0.2
 Summary: pyautobot is a Python library provide functions that do robotic process automation jobs.
 Home-page: https://github.com/blacktear23/pyautobot
 Author: blacktear23
 Author-email: blacktear23@gmail.com
 License: BSD
 Keywords: automation rpa
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyautobot-1.0.0/README.md` & `pyautobot-1.0.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,20 @@
 
 Before install package you should make sure OpenCV and python-tk is installed. Then install package by:
 
 ```
 python3 setup.py install
 ```
 
+Or install from pip
+
+```
+pip3 install pyautobot
+```
+
 
 ### MacOS
 
 You should install OpenCV and make sure python-tk is installed (for message box support).
 
 
 Install OpenCV
@@ -92,16 +98,16 @@
 | -------- | ------ | ----------- |
 | chrome(profile\_dir=None, socks5\_proxy=None, size=(1266, 800), position=(0, 0), user\_agent=None, mobile\_emulation=None, timeout=None) | Driver Object | Start Chrome browser and return Selenium driver object. profile\_dir: Chrome user data path; socks5\_proxy: socks5 proxy address; size: window size; position: window position; user\_agent: set User-Agent header; mobile\_emulation: set mobile browser emulation, require a dict; timeout: Selenium Chrome driver timeout, None will use default 60 seconds. |
 | switch\_tab(driver, idx=None, name='', url='', mode='contains') | None | Switch current tab. driver: Selenium driver object; idx: tab index; name: page title query; url: page url query; mode: query match mode, `contains` means name or url contains query, `equals` means name or url equals query. |
 | new\_tab(driver, url='') | None | Create new tab and switch it to current. url: URL for new tab, empty means new blank tab. |
 | tabs(driver) | List | List Chrome tabs info list |
 | get\_new\_tabs(driver, origin\_tabs\_info) | List | Calculate new opened tabs different from `origin_tabs_info` |
 | snap\_page(driver, fname=None) | bool / bytes | Take screen shot from browser page and save to a file when `fname` provided. |
-| find\_element(driver, by, query) | None / Element | Find element by query. If exists just return the first element, if not exists return None. `by` is query type, `query` is query text. |
-| find\_elements(driver, by, query) | [Element] | Find elements by query. `by` is query type, `query` is query text. |
+| find\_element(driver, \*\*kwargs) | None / Element | Find element by query. If exists just return the first element, if not exists return None. `kwargs` key is query type and value is query text. |
+| find\_elements(driver, \*\*kwargs) | [Element] | Find elements by query. `kwargs` key is query type and value is query text. |
 | get\_parent(elem) | Element | Get element's parent element |
 
 > You can use `chrome` function returned driver object to perform more operations. For more details please read Selenium documents.
 >
 > `user_agent` can accept string or dict. There has 3 pre-defined User-Agent configuration `WINDOWS_UA`, `LINUX_UA`, `MACOS_UA`.
 >
 > The `user_agent` parameter dict fields:
@@ -119,22 +125,44 @@
 > 		* width: Screen width
 > 		* height: Screen height
 > 		* pixelRatio: Pixel ratio e.g.: 3.0
 > * userAgent: User-Agent header
 > 
 > You can use only `deviceName` to tell browser which phone that used, or use rest parameters to define your device settings.
 > 
-> For the query type parameter `by`, it can use Selenium's `By` class or you can just pass a shorten string:
+> For `kwargs`'s query type, it will map key to a Selenium's `By` class value:
 > 
 >  * `id`: By.ID
 >  * `css`: By.CSS_SELECTOR
->  * `class`: By.CLASS_NAME
+>  * `style`: By.CLASS_NAME
 >  * `tag`: By.TAG_NAME
 >  * `name`: By.NAME
 >  * `xpath`: By.XPATH
+> 
+> For example:
+> 
+> ```
+> # Find by ID
+> find_element(d, id='element-id')
+> 
+> # Find by CSS class name
+> find_element(d, style='css-name')
+> 
+> # Find by tag
+> find_element(d, tag='div')
+> 
+> # Find by CSS selector
+> find_element(d, css='div[class="css-name1"]'
+> 
+> # Find by XPATH
+> find_element(d, xpath='parent::*')
+> 
+> # Find by name
+> find_element(d, name='name')
+> ```
 
 ### OCR functions
 | Function | Return | Description |
 | -------- | ------ | ----------- |
 | init\_ocr(langs=['en'], enable_gpu=False) | None | Initialize OCR system, setup languages and set whether enable CUDA |
 | find\_ocr\_element(text, pmode='center', debug=True, threshold=None) | found: bool, x: int, y: int | Find `text` position at screen, return whether founded and position. pmode: position mode, `'center'` means return center position of text, `'topleft'` means top left position; threshold: confidence threshold for image find, None means use system default (0.8). |
 
@@ -150,7 +178,19 @@
 | is_linux() | bool | Return is Linux |
 | is_macos() | bool | Return is MacOS |
 
 ## Tips
 
 * Input text: If some character cannot input by just type keyboard, please use clipboard to copy and paste to input box. For example, you can use `click_and_paste` function.
 * If button image will present more than one at screen, you can use `find_image_element2` to locate bigger image at screen and then find your element image in location image.
+
+## `pyautobot` Command
+
+After install pyautobot it provide a `pyautobot` command line tool. Run `pyautobot` it will start a Python shell with all provided functions imported.
+
+```
+$ pyautobot
+Screen Ratio: 2.0, 2.0
+Elememt Image Ratio: 1, 1
+PyAutoBot Shell
+>>>
+```
```

### Comparing `pyautobot-1.0.0/pyautobot/__init__.py` & `pyautobot-1.0.2/pyautobot/__init__.py`

 * *Files identical despite different names*

### Comparing `pyautobot-1.0.0/pyautobot/chrome.py` & `pyautobot-1.0.2/pyautobot/chrome.py`

 * *Files 5% similar despite different names*

```diff
@@ -180,34 +180,41 @@
     return driver.get_screenshot_as_file(fname)
 
 
 def get_parent(elem):
     return elem.find_element(By.XPATH, 'parent::*')
 
 
-def __transform_by(by):
+def __transform_by(kwargs):
+    if len(kwargs) != 1:
+        raise Exception('Invalid query argument, require only one query')
+
+    by, query = list(kwargs.items())[0]
     if by.lower() == 'id':
         by = By.ID
-    elif by.lower() == 'css':
-        by = By.CSS_SELECTOR
     elif by.lower() == 'tag':
         by = By.TAG_NAME
-    elif by.lower() == 'class':
+    elif by.lower() == 'style':
         by = By.CLASS_NAME
+    elif by.lower() == 'css':
+        by = By.CSS_SELECTOR
     elif by.lower() == 'name':
         by = By.NAME
     elif by.lower() == 'xpath':
         by = By.XPATH
-    return by
+    else:
+        raise Exception('Invalid query type: %s' % by)
+
+    return by, query
 
 
-def find_element(driver, by, query):
-    by = __transform_by(by)
+def find_element(driver, **kwargs):
+    by, query = __transform_by(kwargs)
     elems = driver.find_elements(by, query)
     if len(elems) == 0:
         return None
     return elems[0]
 
 
-def find_elements(driver, by, query):
-    by = __transform_by(by)
+def find_elements(driver, **kwargs):
+    by, query = __transform_by(kwargs)
     return driver.find_elements(by, query)
```

### Comparing `pyautobot-1.0.0/pyautobot/gui.py` & `pyautobot-1.0.2/pyautobot/gui.py`

 * *Files identical despite different names*

### Comparing `pyautobot-1.0.0/pyautobot/images.py` & `pyautobot-1.0.2/pyautobot/images.py`

 * *Files identical despite different names*

### Comparing `pyautobot-1.0.0/pyautobot/ocr.py` & `pyautobot-1.0.2/pyautobot/ocr.py`

 * *Files identical despite different names*

### Comparing `pyautobot-1.0.0/pyautobot.egg-info/PKG-INFO` & `pyautobot-1.0.2/pyautobot.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyautobot
-Version: 1.0.0
+Version: 1.0.2
 Summary: pyautobot is a Python library provide functions that do robotic process automation jobs.
 Home-page: https://github.com/blacktear23/pyautobot
 Author: blacktear23
 Author-email: blacktear23@gmail.com
 License: BSD
 Keywords: automation rpa
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyautobot-1.0.0/setup.py` & `pyautobot-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 * PyAutoGUI and pyperclip: control clipboard, mouse and keyboard operations.
 * Selenium: control Chrome browser.
 * OpenCV-Python: provide graphic based operation.
 * EasyOCR: provide OCR functions.
 '''
 
-version = '1.0.0'
+version = '1.0.2'
 
 setup(
     name='pyautobot',
     version=version,
     url='https://github.com/blacktear23/pyautobot',
     author='blacktear23',
     author_email='blacktear23@gmail.com',
```

