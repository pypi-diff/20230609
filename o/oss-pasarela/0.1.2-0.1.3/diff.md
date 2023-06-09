# Comparing `tmp/oss_pasarela-0.1.2.tar.gz` & `tmp/oss_pasarela-0.1.3.tar.gz`

## Comparing `oss_pasarela-0.1.2.tar` & `oss_pasarela-0.1.3.tar`

### file list

```diff
@@ -1,40 +1,49 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 oss_pasarela-0.1.2/.eslintignore
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 oss_pasarela-0.1.2/.eslintrc.js
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 oss_pasarela-0.1.2/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 oss_pasarela-0.1.2/.prettierrc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 oss_pasarela-0.1.2/.stylelintrc
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 oss_pasarela-0.1.2/CHANGELOG.md
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 oss_pasarela-0.1.2/RELEASE.md
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 oss_pasarela-0.1.2/USAGE.md
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 oss_pasarela-0.1.2/install.json
--rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 oss_pasarela-0.1.2/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 oss_pasarela-0.1.2/setup.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 oss_pasarela-0.1.2/tsconfig.json
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 oss_pasarela-0.1.2/jupyter-config/nb-config/oss_pasarela.json
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 oss_pasarela-0.1.2/jupyter-config/server-config/oss_pasarela.json
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 oss_pasarela-0.1.2/oss_pasarela/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 oss_pasarela-0.1.2/oss_pasarela/_version.py
--rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 oss_pasarela-0.1.2/oss_pasarela/handlers.py
--rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 oss_pasarela-0.1.2/oss_pasarela/labextension/package.json
--rw-r--r--   0        0        0   105882 2020-02-02 00:00:00.000000 oss_pasarela-0.1.2/oss_pasarela/labextension/static/256.3bc65f51567c52dd84cc.js
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 oss_pasarela-0.1.2/oss_pasarela/labextension/static/256.3bc65f51567c52dd84cc.js.LICENSE.txt
--rw-r--r--   0        0        0   198316 2020-02-02 00:00:00.000000 oss_pasarela-0.1.2/oss_pasarela/labextension/static/39.eb3dd569082abc6284c6.js
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 oss_pasarela-0.1.2/oss_pasarela/labextension/static/530.11e38960dba7be4ca2d6.js
--rw-r--r--   0        0        0    30403 2020-02-02 00:00:00.000000 oss_pasarela-0.1.2/oss_pasarela/labextension/static/666.01432931f78fbf9614d0.js
--rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 oss_pasarela-0.1.2/oss_pasarela/labextension/static/747.2a887d57da0d13137f7d.js
--rw-r--r--   0        0        0     5795 2020-02-02 00:00:00.000000 oss_pasarela-0.1.2/oss_pasarela/labextension/static/917.3cf585ce9cf5a3493da9.js
--rw-r--r--   0        0        0     7589 2020-02-02 00:00:00.000000 oss_pasarela-0.1.2/oss_pasarela/labextension/static/remoteEntry.1a34d27663654f3abb01.js
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 oss_pasarela-0.1.2/oss_pasarela/labextension/static/style.js
--rw-r--r--   0        0        0    66612 2020-02-02 00:00:00.000000 oss_pasarela-0.1.2/oss_pasarela/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 oss_pasarela-0.1.2/src/handler.ts
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 oss_pasarela-0.1.2/src/index.ts
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 oss_pasarela-0.1.2/src/components/PasarelaHelpComponent.tsx
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 oss_pasarela-0.1.2/src/widgets/PasarelaHelpWidget.tsx
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 oss_pasarela-0.1.2/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 oss_pasarela-0.1.2/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 oss_pasarela-0.1.2/style/index.js
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 oss_pasarela-0.1.2/.gitignore
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 oss_pasarela-0.1.2/LICENSE
--rw-r--r--   0        0        0     4747 2020-02-02 00:00:00.000000 oss_pasarela-0.1.2/README.md
--rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 oss_pasarela-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     7721 2020-02-02 00:00:00.000000 oss_pasarela-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/.eslintignore
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/.eslintrc.js
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/.stylelintrc
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/CHANGELOG.md
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/RELEASE.md
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/USAGE.md
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/install.json
+-rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/setup.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/tsconfig.json
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/.vscode/settings.json
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/jupyter-config/nb-config/oss_pasarela.json
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/jupyter-config/server-config/oss_pasarela.json
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/oss_pasarela/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/oss_pasarela/_version.py
+-rw-r--r--   0        0        0     5107 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/oss_pasarela/handlers.py
+-rw-r--r--   0        0        0    22054 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/oss_pasarela/labextension/build_log.json
+-rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/oss_pasarela/labextension/package.json
+-rw-r--r--   0        0        0    10053 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/oss_pasarela/labextension/static/lib_index_js.b045879f4211d8fd6b3e.js
+-rw-r--r--   0        0        0     6724 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/oss_pasarela/labextension/static/lib_index_js.b045879f4211d8fd6b3e.js.map
+-rw-r--r--   0        0        0    31909 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/oss_pasarela/labextension/static/remoteEntry.3ae843e9c3ab50fa734d.js
+-rw-r--r--   0        0        0    30696 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/oss_pasarela/labextension/static/remoteEntry.3ae843e9c3ab50fa734d.js.map
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/oss_pasarela/labextension/static/style.js
+-rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/oss_pasarela/labextension/static/style_index_js.d864bbcd3d7a42abcce5.js
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/oss_pasarela/labextension/static/style_index_js.d864bbcd3d7a42abcce5.js.map
+-rw-r--r--   0        0        0   912162 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/oss_pasarela/labextension/static/vendors-node_modules_bootstrap_dist_css_bootstrap_min_css.bd408c9a32d8e876e4ae.js
+-rw-r--r--   0        0        0  1128492 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/oss_pasarela/labextension/static/vendors-node_modules_bootstrap_dist_css_bootstrap_min_css.bd408c9a32d8e876e4ae.js.map
+-rw-r--r--   0        0        0    12054 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/oss_pasarela/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.986066191fbefa152f6c.js
+-rw-r--r--   0        0        0    13784 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/oss_pasarela/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.986066191fbefa152f6c.js.map
+-rw-r--r--   0        0        0   154588 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/oss_pasarela/labextension/static/vendors-node_modules_micromark-core-commonmark_dev_lib_blank-line_js-node_modules_micromark-u-3f9d00.8f075f2566e91b2d223e.js
+-rw-r--r--   0        0        0   161413 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/oss_pasarela/labextension/static/vendors-node_modules_micromark-core-commonmark_dev_lib_blank-line_js-node_modules_micromark-u-3f9d00.8f075f2566e91b2d223e.js.map
+-rw-r--r--   0        0        0   653123 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/oss_pasarela/labextension/static/vendors-node_modules_react-markdown_index_js.3657b2fafb8eeb7c6282.js
+-rw-r--r--   0        0        0   604082 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/oss_pasarela/labextension/static/vendors-node_modules_react-markdown_index_js.3657b2fafb8eeb7c6282.js.map
+-rw-r--r--   0        0        0   186120 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/oss_pasarela/labextension/static/vendors-node_modules_remark-gfm_index_js.abde0ccba3771f12d03f.js
+-rw-r--r--   0        0        0   178523 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/oss_pasarela/labextension/static/vendors-node_modules_remark-gfm_index_js.abde0ccba3771f12d03f.js.map
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/src/handler.ts
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/src/index.ts
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/src/components/PasarelaHelpComponent.tsx
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/src/widgets/PasarelaHelpWidget.tsx
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/style/index.js
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/LICENSE
+-rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/README.md
+-rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     7685 2020-02-02 00:00:00.000000 oss_pasarela-0.1.3/PKG-INFO
```

### Comparing `oss_pasarela-0.1.2/.eslintrc.js` & `oss_pasarela-0.1.3/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `oss_pasarela-0.1.2/RELEASE.md` & `oss_pasarela-0.1.3/RELEASE.md`

 * *Files identical despite different names*

### Comparing `oss_pasarela-0.1.2/USAGE.md` & `oss_pasarela-0.1.3/USAGE.md`

 * *Files identical despite different names*

### Comparing `oss_pasarela-0.1.2/package.json` & `oss_pasarela-0.1.3/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'0.1.3'"}*

```diff
@@ -102,9 +102,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.2"
+    "version": "0.1.3"
 }
```

### Comparing `oss_pasarela-0.1.2/tsconfig.json` & `oss_pasarela-0.1.3/tsconfig.json`

 * *Files identical despite different names*

### Comparing `oss_pasarela-0.1.2/oss_pasarela/__init__.py` & `oss_pasarela-0.1.3/oss_pasarela/__init__.py`

 * *Files identical despite different names*

### Comparing `oss_pasarela-0.1.2/oss_pasarela/handlers.py` & `oss_pasarela-0.1.3/oss_pasarela/handlers.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,108 +1,143 @@
-import re
-import json
 import base64
 import binascii
+import json
+import nbformat as nbf
+import re
 import requests
+import tornado
 import validators
-from subprocess import check_output
-import nbformat as nbf
-from nbconvert.preprocessors import ExecutePreprocessor
-from nbconvert.preprocessors import CellExecutionError
-
 from jupyter_server.base.handlers import APIHandler
 from jupyter_server.utils import url_path_join
-import tornado
+from subprocess import check_output
 
-def _get_pasarela_usage():
-    response = requests.get('https://api.github.com/repos/navteca/oss-pasarela/contents/USAGE.md')
-    data = response.json()
-    base64_content = data['content']
-    bytes_content = base64.b64decode(base64_content)
-    help_content = bytes_content.decode()
+NOTEBOOK_NAME = 'Untitled.ipynb'
 
-    return help_content
-class RouteHandler(APIHandler):
-    @tornado.web.authenticated
-    def get(self):
-        code = self.get_argument("code", None)
-        url = self.get_argument("url", None)
-        kernel_name = self.get_argument("kernel_name", None)   
 
-        err = None
-        if code:
-            try:
-                base64_bytes = code.encode('ascii')
-                message_bytes = base64.b64decode(base64_bytes)
-                notebook_content = message_bytes.decode('ascii')
-            except binascii.Error:
-                err = 'Invalid base64 string.'
-        elif url:
-            if validators.url(url):
-                try:
-                    response = requests.get(url)
-                    response.raise_for_status()
-                except requests.exceptions.HTTPError as e:
-                    err = e.response.reason
-                except requests.exceptions.RequestException as e:
-                    err = e.response.reason
-
-                if not err:
-                    try:
-                        notebook_content = json.loads(response.text)
-                    except json.JSONDecodeError as e:
-                        err = "Invalid JSON format."
+class CustomError(Exception):
+    pass
 
-                    if not err and ('metadata' not in notebook_content or 'nbformat' not in notebook_content or 'cells' not in notebook_content):
-                        err = f'The Url {url} does not contains a valid Notebook format'
-            else:
-                err = f'{url} is not a valid url.'
-        else:        
-            err = 'Missing code or url argument.'
 
-        nb = nbf.v4.new_notebook()
-        NOTEBOOK_NAME = 'Untitled.ipynb'
+def _get_pasarela_usage() -> str:
+    help_content = ""
+    try:
+        response = requests.get('https://api.github.com/repos/navteca/oss-pasarela/contents/USAGE.md')
+        response.raise_for_status()
+        data = response.json()
+        base64_content = data['content']
+        bytes_content = base64.b64decode(base64_content)
+        help_content = bytes_content.decode()
+    except requests.exceptions.HTTPError as e:
+        raise CustomError(e.response.reason)
+    except requests.exceptions.RequestException as e:
+        raise CustomError(e.response.reason)
+    except binascii.Error:
+        raise CustomError('Invalid base64 string.')
+    else:
+        return help_content
+
+
+def _decode_base64_string(code: str) -> str:
+    content = None
+    try:
+        message_bytes = base64.b64decode(code)
+        content = message_bytes.decode()
+    except binascii.Error:
+        raise CustomError('Invalid base64 string.')
+    except Exception as e:
+        raise CustomError(e)
+    else:
+        return content
+
+
+def _get_notebook_from_url(url: str) -> str:
+    try:
+        if validators.url(url):
+            response = requests.get(url)
+            response.raise_for_status()
+        else:
+            raise CustomError(f'{url} is not a valid url.')
+        notebook_content = json.loads(response.text)
+        if not isinstance(notebook_content, dict):
+            raise nbf.ValidationError('')
+        nbf.validate(notebook_content)
+    except requests.exceptions.HTTPError as e:
+        raise CustomError(e.response.reason)
+    except requests.exceptions.RequestException as e:
+        raise CustomError(e.response.reason)
+    except json.JSONDecodeError as e:
+        raise CustomError("Invalid JSON format.")
+    except nbf.ValidationError:
+        raise CustomError(f'The Url {url} does not contains a valid Notebook format')
+    else:
+        return notebook_content
+
+
+def _create_notebook(host: str, code: str, url: str, notebook_content: dict, kernel_name: str, note_book_name: str, err: str) -> None:
+    header = None
+    kernelspec = check_output('jupyter kernelspec list --json', shell=True).decode("utf-8")
+    nb = nbf.v4.new_notebook()
 
+    try:
         if err:
             header = f"""# <span style="color:red">Oops, something went wrong.</span>\n````Reason: {err}````"""
-            help_content = _get_pasarela_usage().replace("[jupyterhub_domain]", self.request.host)
-            nb['cells'] = [nbf.v4.new_markdown_cell(header), nbf.v4.new_markdown_cell(help_content)]
+            help_content = _get_pasarela_usage().replace("[jupyterhub_domain]", host)
+            nb['cells'] = [nbf.v4.new_markdown_cell(help_content)]
+        elif code:
+            nb['cells'] = [nbf.v4.new_code_cell(notebook_content)]
         else:
-            header = f""" This notebook has been generated by OSS Pasarela extension. """
-            if code:
-                nb['cells'] = [nbf.v4.new_code_cell(notebook_content)]
-            else:
-                nb = nbf.from_dict(notebook_content)
+            nb = nbf.from_dict(notebook_content)
             
+        if kernel_name:
+            if kernel_name not in kernelspec:
+                header = f"""# <span style="orange:red">Warning.</span>\n````Reason: Kernel {kernel_name} is not installed````"""
+            else:
+                nb.metadata['kernelspec'] = {'name' : kernel_name, 'display_name': kernel_name}
+
+        if header:
             nb['cells'].insert(0, nbf.v4.new_markdown_cell(header))
+        nbf.write(nb, note_book_name)
+    except Exception as e:
+        raise CustomError(e)
+    else:
+        return None
 
-            kernelspec = check_output('jupyter kernelspec list --json', shell=True).decode("utf-8")
-            if kernel_name:
-                if kernel_name not in kernelspec:
-                    err = f"""# <span style="orange:red">Warning.</span>\n````Reason: Kernel {kernel_name} is not installed````"""
-                else:
-                    nb.metadata['kernelspec'] = {'name' : kernel_name, 'display_name': kernel_name}
 
-            if url and 'kernelspec' in nb.metadata and 'name' in nb.metadata.kernelspec and nb.metadata.kernelspec.name not in kernelspec:
-                err = f"""# <span style="orange:red">Warning.</span>\n````Reason: Kernel {nb.metadata['kernelspec']['name']} is not installed````"""
-            
-            if err:
-                nb['cells'].insert(0, nbf.v4.new_markdown_cell(err))
+class RouteHandler(APIHandler):
+    @tornado.web.authenticated
+    def get(self):
+        code = self.get_argument("code", None)
+        kernel_name = self.get_argument("kernel_name", None)   
+        url = self.get_argument("url", None)                   
+        tree = self.get_argument("tree", None)
+        err = None
+        host = self.request.host
+        notebook_content = {}
+        path = '/notebooks/' if tree == '' else '/lab/tree/'
+        try:
+            if not (code or url):
+                raise CustomError('Missing code or url argument.')
+            notebook_content = _decode_base64_string(code) if code else _get_notebook_from_url(url)            
+        except CustomError as e:
+            err = e
+        finally:
+            _create_notebook(host, code, url, notebook_content, kernel_name, NOTEBOOK_NAME, err)
+            full_url = self.request.full_url()
+            match = re.search("(\/user\/)(.*)(\/pasarela)", full_url)
+
+        # self.redirect('http://' + self.request.host + path + NOTEBOOK_NAME)
+        self.redirect('http://' + self.request.host + '/user/' + match.group(2) + path + NOTEBOOK_NAME)
 
-        nbf.write(nb, NOTEBOOK_NAME)
 
-        full_url = self.request.full_url()
-        match = re.search("(\/user\/)(.*)(\/pasarela)", full_url)
-        self.redirect('http://' + self.request.host + '/user/' + match.group(2) + '/lab/tree/' + NOTEBOOK_NAME)
 class UsageHandler(APIHandler):
     @tornado.web.authenticated
     def get(self):
-        # self.finish('This is a test')
         self.finish(_get_pasarela_usage().replace("[jupyterhub_domain]", self.request.host))
 
+
 def setup_handlers(web_app):
     host_pattern = ".*$"
 
     base_url = web_app.settings["base_url"]
     handlers = [
         (url_path_join(base_url, "pasarela", "open"), RouteHandler),
         (url_path_join(base_url, "pasarela", "usage"), UsageHandler)
```

### Comparing `oss_pasarela-0.1.2/oss_pasarela/labextension/package.json` & `oss_pasarela-0.1.3/oss_pasarela/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994791666666666%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.3ae843e9c3ab50fa734d.js'}}"}*

```diff
@@ -43,15 +43,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/Navteca/oss-pasarela.git",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.1a34d27663654f3abb01.js",
+            "load": "static/remoteEntry.3ae843e9c3ab50fa734d.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "oss_pasarela"
                 },
```

### Comparing `oss_pasarela-0.1.2/src/handler.ts` & `oss_pasarela-0.1.3/src/handler.ts`

 * *Files identical despite different names*

### Comparing `oss_pasarela-0.1.2/src/index.ts` & `oss_pasarela-0.1.3/src/index.ts`

 * *Files identical despite different names*

### Comparing `oss_pasarela-0.1.2/src/components/PasarelaHelpComponent.tsx` & `oss_pasarela-0.1.3/src/components/PasarelaHelpComponent.tsx`

 * *Files identical despite different names*

### Comparing `oss_pasarela-0.1.2/.gitignore` & `oss_pasarela-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `oss_pasarela-0.1.2/LICENSE` & `oss_pasarela-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `oss_pasarela-0.1.2/README.md` & `oss_pasarela-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -64,17 +64,17 @@
 
 ### Usage
 
 To use the extension on this system, you open a new window with a specially crafted URL as follows:
 
 **Base URL**:
 
-https://[jupyterhub_domain]/user/[username]/pasarela/open
+https://[jupyterhub_domain]/hub/user-redirect/pasarela/open
 
-First, [jupyterhub_domain] with your JupyterHub domain and replace [username] with your JupyterHub username.
+First, replace [jupyterhub_domain] with your JupyterHub domain.
 
 **Required Parameters (use only one):**
 
 **code** - the base64 encoded source code that will pre-populate a cell in a new notebook on this system
 
 -**or**-
 
@@ -83,26 +83,26 @@
 **Optional Parameters**:
 
 **kernel_name** - the specific Notebook kernel on this system to use to open the new Notebook. If unspecified, Jupyterlab will ask you to select a kernel to use when you first open the notebook.
 
 ### Open a Notebook with a base64 string code
 The following URL will open a notebook and it will be pre-populated with the base64 decoded content provided. Jupyterlab will ask which kernel is to be used for the notebook
 
-> https://[jupyterhub_domain]/user/[username]/pasarela/open?code=cHJpbnQoIkhlbGxvIFdvcmxkIik=
+> https://[jupyterhub_domain]/hub/user-redirect/pasarela/open?code=cHJpbnQoIkhlbGxvIFdvcmxkIik=
 
 
 The following URL will open a notebook and it will be pre-populated with the base64 decoded content provided and will use the “python3” kernel.
 
-> https://[jupyterhub_domain]/user/[username]/pasarela/open?code=cHJpbnQoIkhlbGxvIFdvcmxkIik=&kernel_name=python3
+> https://[jupyterhub_domain]/hub/user-redirect/pasarela/open?code=cHJpbnQoIkhlbGxvIFdvcmxkIik=&kernel_name=python3
 
 
 ### Open a Notebook with a URL
 The following URL will open a notebook and it will be pre-populated with contents of the Jupyter notebook file at the specified URL. Jupyterlab will ask which kernel is to be used for the notebook
 
-> https://[jupyterhub_domain]/user/[username]/pasarela/open?url=https://cdaweb.gsfc.nasa.gov/WebServices/REST/jupyter/CdasWsExampleXarray.ipynb
+> https://[jupyterhub_domain]/hub/user-redirect/pasarela/open?url=https://cdaweb.gsfc.nasa.gov/WebServices/REST/jupyter/CdasWsExampleXarray.ipynb
 
 <br/>
 
 ### Current Status
 
 We are in a very early stage in terms of all the features we want to add to the extension to be even with other extensions. Currently you can do the following:
 
@@ -138,7 +138,8 @@
 
 <br/>
 
 ### Notes for your consideration
 
 - This project is in early stage. We are continuously working on it to make it better.
 - This is one of our first extensions we put out there. We are aware we have so much to learn from the FLOSS communities and that is one of the reasons we why decided to publish it.
+
```

### Comparing `oss_pasarela-0.1.2/pyproject.toml` & `oss_pasarela-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oss_pasarela-0.1.2/PKG-INFO` & `oss_pasarela-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oss-pasarela
-Version: 0.1.2
+Version: 0.1.3
 Summary: A JupyterLab extension to open notebooks from websites with just one click.
 Project-URL: Homepage, https://github.com/Navteca/oss-pasarela.git
 Project-URL: Bug Tracker, https://github.com/Navteca/oss-pasarela.git/issues
 Project-URL: Repository, https://github.com/Navteca/oss-pasarela.git.git
 Author-email: Navteca LLC <info@navteca.com>
 License: BSD 3-Clause License
         
@@ -120,17 +120,17 @@
 
 ### Usage
 
 To use the extension on this system, you open a new window with a specially crafted URL as follows:
 
 **Base URL**:
 
-https://[jupyterhub_domain]/user/[username]/pasarela/open
+https://[jupyterhub_domain]/hub/user-redirect/pasarela/open
 
-First, [jupyterhub_domain] with your JupyterHub domain and replace [username] with your JupyterHub username.
+First, replace [jupyterhub_domain] with your JupyterHub domain.
 
 **Required Parameters (use only one):**
 
 **code** - the base64 encoded source code that will pre-populate a cell in a new notebook on this system
 
 -**or**-
 
@@ -139,26 +139,26 @@
 **Optional Parameters**:
 
 **kernel_name** - the specific Notebook kernel on this system to use to open the new Notebook. If unspecified, Jupyterlab will ask you to select a kernel to use when you first open the notebook.
 
 ### Open a Notebook with a base64 string code
 The following URL will open a notebook and it will be pre-populated with the base64 decoded content provided. Jupyterlab will ask which kernel is to be used for the notebook
 
-> https://[jupyterhub_domain]/user/[username]/pasarela/open?code=cHJpbnQoIkhlbGxvIFdvcmxkIik=
+> https://[jupyterhub_domain]/hub/user-redirect/pasarela/open?code=cHJpbnQoIkhlbGxvIFdvcmxkIik=
 
 
 The following URL will open a notebook and it will be pre-populated with the base64 decoded content provided and will use the “python3” kernel.
 
-> https://[jupyterhub_domain]/user/[username]/pasarela/open?code=cHJpbnQoIkhlbGxvIFdvcmxkIik=&kernel_name=python3
+> https://[jupyterhub_domain]/hub/user-redirect/pasarela/open?code=cHJpbnQoIkhlbGxvIFdvcmxkIik=&kernel_name=python3
 
 
 ### Open a Notebook with a URL
 The following URL will open a notebook and it will be pre-populated with contents of the Jupyter notebook file at the specified URL. Jupyterlab will ask which kernel is to be used for the notebook
 
-> https://[jupyterhub_domain]/user/[username]/pasarela/open?url=https://cdaweb.gsfc.nasa.gov/WebServices/REST/jupyter/CdasWsExampleXarray.ipynb
+> https://[jupyterhub_domain]/hub/user-redirect/pasarela/open?url=https://cdaweb.gsfc.nasa.gov/WebServices/REST/jupyter/CdasWsExampleXarray.ipynb
 
 <br/>
 
 ### Current Status
 
 We are in a very early stage in terms of all the features we want to add to the extension to be even with other extensions. Currently you can do the following:
 
@@ -194,7 +194,8 @@
 
 <br/>
 
 ### Notes for your consideration
 
 - This project is in early stage. We are continuously working on it to make it better.
 - This is one of our first extensions we put out there. We are aware we have so much to learn from the FLOSS communities and that is one of the reasons we why decided to publish it.
+
```

