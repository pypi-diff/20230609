# Comparing `tmp/webhaak-0.5.1.tar.gz` & `tmp/webhaak-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webhaak-0.5.1.tar", last modified: Tue Jun  6 11:52:37 2023, max compression
+gzip compressed data, was "webhaak-0.5.2.tar", last modified: Fri Jun  9 19:54:29 2023, max compression
```

## Comparing `webhaak-0.5.1.tar` & `webhaak-0.5.2.tar`

### file list

```diff
@@ -1,20 +1,58 @@
-drwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)        0 2023-06-06 11:52:37.900978 webhaak-0.5.1/
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)    11357 2021-10-12 17:55:24.000000 webhaak-0.5.1/LICENSE
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     5619 2023-06-06 11:52:37.900978 webhaak-0.5.1/PKG-INFO
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     5002 2023-06-06 09:40:02.000000 webhaak-0.5.1/README.rst
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)      936 2023-06-06 11:45:59.000000 webhaak-0.5.1/pyproject.toml
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)       38 2023-06-06 11:52:37.900978 webhaak-0.5.1/setup.cfg
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)      189 2023-06-06 09:40:02.000000 webhaak-0.5.1/setup.py
-drwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)        0 2023-06-06 11:52:37.900978 webhaak-0.5.1/src/
-drwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)        0 2023-06-06 11:52:37.900978 webhaak-0.5.1/src/webhaak/
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)        0 2023-06-06 09:40:02.000000 webhaak-0.5.1/src/webhaak/__init__.py
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)    10139 2023-06-06 09:40:02.000000 webhaak-0.5.1/src/webhaak/incoming.py
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     9724 2023-06-06 09:40:02.000000 webhaak-0.5.1/src/webhaak/main.py
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)    16526 2023-06-06 11:45:39.000000 webhaak-0.5.1/src/webhaak/tasks.py
-drwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)        0 2023-06-06 11:52:37.900978 webhaak-0.5.1/src/webhaak.egg-info/
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     5619 2023-06-06 11:52:37.000000 webhaak-0.5.1/src/webhaak.egg-info/PKG-INFO
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)      343 2023-06-06 11:52:37.000000 webhaak-0.5.1/src/webhaak.egg-info/SOURCES.txt
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)        1 2023-06-06 11:52:37.000000 webhaak-0.5.1/src/webhaak.egg-info/dependency_links.txt
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)       38 2023-06-06 11:52:37.000000 webhaak-0.5.1/src/webhaak.egg-info/entry_points.txt
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)       92 2023-06-06 11:52:37.000000 webhaak-0.5.1/src/webhaak.egg-info/requires.txt
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)        8 2023-06-06 11:52:37.000000 webhaak-0.5.1/src/webhaak.egg-info/top_level.txt
+drwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)        0 2023-06-09 19:54:29.182563 webhaak-0.5.2/
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)      936 2023-04-06 07:21:19.000000 webhaak-0.5.2/.gitignore
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     4810 2023-06-09 19:53:46.000000 webhaak-0.5.2/CHANGELOG.md
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)    11357 2021-07-07 08:00:19.000000 webhaak-0.5.2/LICENSE
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     5651 2023-06-09 19:54:29.178563 webhaak-0.5.2/PKG-INFO
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     5034 2023-06-09 18:11:07.000000 webhaak-0.5.2/README.rst
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)        0 2021-07-07 08:00:19.000000 webhaak-0.5.2/__init__.py
+drwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)        0 2023-06-09 19:54:29.174564 webhaak-0.5.2/docs/
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)      707 2023-04-29 18:49:36.000000 webhaak-0.5.2/docs/Makefile
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)      791 2021-07-07 08:00:19.000000 webhaak-0.5.2/docs/make.bat
+drwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)        0 2023-06-09 19:54:29.178563 webhaak-0.5.2/docs/source/
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     4810 2023-06-09 19:53:46.000000 webhaak-0.5.2/docs/source/CHANGELOG.md
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     5034 2023-06-09 18:11:07.000000 webhaak-0.5.2/docs/source/README.rst
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     6219 2023-04-29 18:49:36.000000 webhaak-0.5.2/docs/source/conf.py
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     2218 2023-04-29 18:49:36.000000 webhaak-0.5.2/docs/source/exampleconfig.rst
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)      514 2021-07-07 08:00:19.000000 webhaak-0.5.2/docs/source/index.rst
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)       58 2021-07-07 08:00:19.000000 webhaak-0.5.2/docs/source/modules.rst
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)      557 2023-04-29 18:49:36.000000 webhaak-0.5.2/docs/source/webhaak.rst
+drwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)        0 2023-06-09 19:54:29.178563 webhaak-0.5.2/example_config/
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     3351 2023-04-06 07:21:19.000000 webhaak-0.5.2/example_config/examples.yaml
+-rwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)      824 2023-04-29 18:49:36.000000 webhaak-0.5.2/example_config/flake8diff.sh
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)      293 2023-04-06 07:21:19.000000 webhaak-0.5.2/example_config/gunicorn_webhaak_conf.py
+drwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)        0 2023-06-09 19:54:29.178563 webhaak-0.5.2/example_config/nginx/
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     1049 2023-03-31 18:46:56.000000 webhaak-0.5.2/example_config/nginx/hook.example.com.conf
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)      593 2023-04-06 07:21:19.000000 webhaak-0.5.2/example_config/rq_settings.example.py
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     1237 2021-07-07 08:00:19.000000 webhaak-0.5.2/example_config/sentry_to_telegram.sh
+drwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)        0 2023-06-09 19:54:29.178563 webhaak-0.5.2/example_config/supervisord/
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     1112 2023-04-28 07:25:54.000000 webhaak-0.5.2/example_config/supervisord/webhaak_rq_worker.conf
+drwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)        0 2023-06-09 19:54:29.178563 webhaak-0.5.2/example_config/systemd/
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)      887 2023-04-29 18:49:36.000000 webhaak-0.5.2/example_config/systemd/webhaak.service
+-rwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)      631 2021-07-07 08:00:19.000000 webhaak-0.5.2/example_config/update_flask.sh
+-rwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)      987 2021-07-07 08:00:19.000000 webhaak-0.5.2/example_config/update_virtualenv.sh
+-rwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)      628 2023-03-31 18:46:56.000000 webhaak-0.5.2/example_config/update_webapp.sh
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)      353 2023-04-06 07:21:19.000000 webhaak-0.5.2/pylintrc
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)      936 2023-06-09 19:43:45.000000 webhaak-0.5.2/pyproject.toml
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)       98 2023-06-06 16:20:17.000000 webhaak-0.5.2/requirements-dev.in
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     4809 2023-06-06 16:20:17.000000 webhaak-0.5.2/requirements-dev.txt
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)       29 2023-03-31 18:46:56.000000 webhaak-0.5.2/requirements-server.in
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     1972 2023-06-06 16:20:17.000000 webhaak-0.5.2/requirements-server.txt
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)      175 2023-06-06 16:20:17.000000 webhaak-0.5.2/requirements.in
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     1859 2023-06-06 16:20:17.000000 webhaak-0.5.2/requirements.txt
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)       38 2023-06-09 19:54:29.182563 webhaak-0.5.2/setup.cfg
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)      189 2023-04-06 07:21:19.000000 webhaak-0.5.2/setup.py
+drwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)        0 2023-06-09 19:54:29.178563 webhaak-0.5.2/src/
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)      346 2018-10-03 09:36:45.000000 webhaak-0.5.2/src/settings.py
+drwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)        0 2023-06-09 19:54:29.178563 webhaak-0.5.2/src/webhaak/
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)        0 2023-04-06 09:50:43.000000 webhaak-0.5.2/src/webhaak/__init__.py
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)    10139 2023-03-31 18:46:56.000000 webhaak-0.5.2/src/webhaak/incoming.py
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     9724 2023-04-28 07:25:54.000000 webhaak-0.5.2/src/webhaak/main.py
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)    16655 2023-06-09 18:58:03.000000 webhaak-0.5.2/src/webhaak/tasks.py
+drwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)        0 2023-06-09 19:54:29.178563 webhaak-0.5.2/src/webhaak.egg-info/
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     5651 2023-06-09 19:54:29.000000 webhaak-0.5.2/src/webhaak.egg-info/PKG-INFO
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     1133 2023-06-09 19:54:29.000000 webhaak-0.5.2/src/webhaak.egg-info/SOURCES.txt
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)        1 2023-06-09 19:54:29.000000 webhaak-0.5.2/src/webhaak.egg-info/dependency_links.txt
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)       38 2023-06-09 19:54:29.000000 webhaak-0.5.2/src/webhaak.egg-info/entry_points.txt
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)       92 2023-06-09 19:54:29.000000 webhaak-0.5.2/src/webhaak.egg-info/requires.txt
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)       17 2023-06-09 19:54:29.000000 webhaak-0.5.2/src/webhaak.egg-info/top_level.txt
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)      380 2023-04-06 07:21:19.000000 webhaak-0.5.2/tox.ini
```

### Comparing `webhaak-0.5.1/LICENSE` & `webhaak-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `webhaak-0.5.1/PKG-INFO` & `webhaak-0.5.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webhaak
-Version: 0.5.1
+Version: 0.5.2
 Summary: Simple webhook service to update and deploy sites and do other maintenance and automatic tasks
 Author-email: Michiel Scholten <michiel@diginaut.net>
 License: Apache
 Project-URL: Homepage, https://github.com/aquatix/webhaak
 Project-URL: Bug Tracker, https://github.com/aquatix/webhaak/issues
 Keywords: webhook,api,automation,CI/CD
 Classifier: Framework :: FastAPI
@@ -52,17 +52,16 @@
     mkvirtualenv webhaak # or whatever project you are working on
     pip install -r requirements.txt
 
 
 Usage
 -----
 
-Copy ``settings.py`` from example_config to the parent directory and
-configure to your needs. Create a yaml file with the projects to serve (see
-next section) and refer to this file from the settings.py.
+Copy ``example.yaml`` from example_config to a directory you will use for configuration and
+configure to your needs. This is a yaml file with the projects to serve (see next section).
 
 Run webhaak as a service under nginx or apache and call the appropriate
 url's when wanted (e.g., on push to repository).
 
 webhaak can also be run from the command line: ``uvicorn webhaak:app --reload``
 
 Be sure to export/set the ``SECRETKEY`` environment variable before running, it's needed for some management URI's.
@@ -105,14 +104,20 @@
 
 What's new?
 -----------
 
 See the `Changelog`_.
 
 
+Developing
+----------
+
+Running in PyCharm: tbd :)
+
+
 .. _webhaak: https://github.com/aquatix/webhaak
 .. _webhook: https://en.wikipedia.org/wiki/Webhook
 .. |PyPI version| image:: https://img.shields.io/pypi/v/webhaak.svg
    :target: https://pypi.python.org/pypi/webhaak/
 .. |PyPI downloads| image:: https://img.shields.io/pypi/dm/webhaak.svg
    :target: https://pypi.python.org/pypi/webhaak/
 .. |PyPI license| image:: https://img.shields.io/github/license/aquatix/webhaak.svg
```

### Comparing `webhaak-0.5.1/README.rst` & `webhaak-0.5.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -36,17 +36,16 @@
     mkvirtualenv webhaak # or whatever project you are working on
     pip install -r requirements.txt
 
 
 Usage
 -----
 
-Copy ``settings.py`` from example_config to the parent directory and
-configure to your needs. Create a yaml file with the projects to serve (see
-next section) and refer to this file from the settings.py.
+Copy ``example.yaml`` from example_config to a directory you will use for configuration and
+configure to your needs. This is a yaml file with the projects to serve (see next section).
 
 Run webhaak as a service under nginx or apache and call the appropriate
 url's when wanted (e.g., on push to repository).
 
 webhaak can also be run from the command line: ``uvicorn webhaak:app --reload``
 
 Be sure to export/set the ``SECRETKEY`` environment variable before running, it's needed for some management URI's.
@@ -89,14 +88,20 @@
 
 What's new?
 -----------
 
 See the `Changelog`_.
 
 
+Developing
+----------
+
+Running in PyCharm: tbd :)
+
+
 .. _webhaak: https://github.com/aquatix/webhaak
 .. _webhook: https://en.wikipedia.org/wiki/Webhook
 .. |PyPI version| image:: https://img.shields.io/pypi/v/webhaak.svg
    :target: https://pypi.python.org/pypi/webhaak/
 .. |PyPI downloads| image:: https://img.shields.io/pypi/dm/webhaak.svg
    :target: https://pypi.python.org/pypi/webhaak/
 .. |PyPI license| image:: https://img.shields.io/github/license/aquatix/webhaak.svg
```

### Comparing `webhaak-0.5.1/pyproject.toml` & `webhaak-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "webhaak"
-version = "0.5.1"
+version = "0.5.2"
 authors = [
     {name = "Michiel Scholten", email = "michiel@diginaut.net"},
 ]
 description= "Simple webhook service to update and deploy sites and do other maintenance and automatic tasks"
 readme = "README.rst"
 requires-python = ">=3.7"
 keywords = ["webhook", "api", "automation", "CI/CD"]
```

### Comparing `webhaak-0.5.1/src/webhaak/incoming.py` & `webhaak-0.5.2/src/webhaak/incoming.py`

 * *Files identical despite different names*

### Comparing `webhaak-0.5.1/src/webhaak/main.py` & `webhaak-0.5.2/src/webhaak/main.py`

 * *Files identical despite different names*

### Comparing `webhaak-0.5.1/src/webhaak/tasks.py` & `webhaak-0.5.2/src/webhaak/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,23 +26,23 @@
 
     pushover_userkey: str
     pushover_apptoken: str
 
     debug: bool = False
 
     @validator('jobs_log_dir', pre=True)
-    def apply_root(cls, v, values):
+    def apply_root(cls, value, values):
         """
         Create the actual value for jobs_log_dir, through its validator
         """
         if log_dir := values.get('log_dir'):
             # jobs_log_dir is a subdirectory of log_dir
-            return log_dir / v
+            return log_dir / value
         # should only happen when there was an error with log_dir
-        return v
+        return value
 
 
 # Read the settings from the environment, based on the above configuration
 settings = Settings()
 print(settings.dict())
 
 logger = logging.getLogger('worker')
@@ -89,28 +89,28 @@
 )
 
 # Load the configuration of the various projects/hooks
 with open(settings.projects_file, 'r', encoding='utf-8') as pf:
     projects = strictyaml.load(pf.read(), schema).data
 
 
-def send_pushover_message(user, api_key, text, **kwargs):
+def send_pushover_message(userkey, apptoken, text, **kwargs):
     """
     Send a message through PushOver
 
     It is possible to specify additional properties of the message by passing keyword
     arguments. The list of valid keywords is ``title, priority, sound,
     callback, timestamp, url, url_title, device, retry, expire and html``
     which are described in the Pushover API documentation.
 
     For convenience, you can simply set ``timestamp=True`` to set the
     timestamp to the current timestamp.
 
-    :param str user: user key in PushOver
-    :param str api_key: app token for PushOver
+    :param str userkey: user key in PushOver
+    :param str apptoken: app token for PushOver
     :param str text: message to send
     """
     message_keywords = [
         "title",
         "priority",
         "sound",
         "callback",
@@ -119,29 +119,29 @@
         "url_title",
         "device",
         "retry",
         "expire",
         "html",
         "attachment",
     ]
-    payload = {"message": text, "user": user, "token": api_key}
+    payload = {"message": text, "user": userkey, "token": apptoken}
     for key, value in kwargs.items():
         if key not in message_keywords:
-            raise ValueError("{0}: invalid message parameter".format(key))
+            raise ValueError(f'{key}: invalid message parameter')
         if key == "timestamp" and value is True:
             payload[key] = int(time.time())
         else:
             payload[key] = value
-    r = requests.post(
+    response = requests.post(
         'https://api.pushover.net/1/messages.json',
         data=payload,
         headers={'User-Agent': 'Python'},
         timeout=60
     )
-    return r
+    return response
 
 
 def make_sentry_message(result):
     """
     # Filter away known things
     if [[ $MESSAGE == *"Het ElementTree object kon niet"* ||
           $MESSAGE == *"The ElementTree object could"* ||
@@ -212,17 +212,22 @@
             with requests.get(
                 f"https://api.telegram.org/bot{telegram_token}/sendMessage?chat_id={telegram_chat_id}&text={msg}",
                 timeout=30
             ) as response:
                 logging.info('Telegram notification sent, result was %s', str(response.status_code))
         else:
             # Use the Pushover default
-            r = send_pushover_message(settings.pushover_userkey, settings.pushover_userkey, message, title=title)
-            if not r.status_code == 200:
-                logging.error(r.text)
+            response = send_pushover_message(
+                settings.pushover_userkey,
+                settings.pushover_apptoken,
+                message,
+                title=title
+            )
+            if not response.status_code == 200:
+                logging.error(response.text)
         logging.info('Notification sent')
     except AttributeError:
         logging.warning('Notification through PushOver failed because of missing configuration')
 
 
 def get_trigger_settings(app_key, trigger_key):
     """Look up the trigger and return the repo and command to be updated and fired
```

### Comparing `webhaak-0.5.1/src/webhaak.egg-info/PKG-INFO` & `webhaak-0.5.2/src/webhaak.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webhaak
-Version: 0.5.1
+Version: 0.5.2
 Summary: Simple webhook service to update and deploy sites and do other maintenance and automatic tasks
 Author-email: Michiel Scholten <michiel@diginaut.net>
 License: Apache
 Project-URL: Homepage, https://github.com/aquatix/webhaak
 Project-URL: Bug Tracker, https://github.com/aquatix/webhaak/issues
 Keywords: webhook,api,automation,CI/CD
 Classifier: Framework :: FastAPI
@@ -52,17 +52,16 @@
     mkvirtualenv webhaak # or whatever project you are working on
     pip install -r requirements.txt
 
 
 Usage
 -----
 
-Copy ``settings.py`` from example_config to the parent directory and
-configure to your needs. Create a yaml file with the projects to serve (see
-next section) and refer to this file from the settings.py.
+Copy ``example.yaml`` from example_config to a directory you will use for configuration and
+configure to your needs. This is a yaml file with the projects to serve (see next section).
 
 Run webhaak as a service under nginx or apache and call the appropriate
 url's when wanted (e.g., on push to repository).
 
 webhaak can also be run from the command line: ``uvicorn webhaak:app --reload``
 
 Be sure to export/set the ``SECRETKEY`` environment variable before running, it's needed for some management URI's.
@@ -105,14 +104,20 @@
 
 What's new?
 -----------
 
 See the `Changelog`_.
 
 
+Developing
+----------
+
+Running in PyCharm: tbd :)
+
+
 .. _webhaak: https://github.com/aquatix/webhaak
 .. _webhook: https://en.wikipedia.org/wiki/Webhook
 .. |PyPI version| image:: https://img.shields.io/pypi/v/webhaak.svg
    :target: https://pypi.python.org/pypi/webhaak/
 .. |PyPI downloads| image:: https://img.shields.io/pypi/dm/webhaak.svg
    :target: https://pypi.python.org/pypi/webhaak/
 .. |PyPI license| image:: https://img.shields.io/github/license/aquatix/webhaak.svg
```

