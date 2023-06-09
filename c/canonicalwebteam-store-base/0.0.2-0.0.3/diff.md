# Comparing `tmp/canonicalwebteam_store_base-0.0.2.tar.gz` & `tmp/canonicalwebteam_store_base-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canonicalwebteam_store_base-0.0.2.tar", max compression
+gzip compressed data, was "canonicalwebteam_store_base-0.0.3.tar", max compression
```

## Comparing `canonicalwebteam_store_base-0.0.2.tar` & `canonicalwebteam_store_base-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    35149 2023-06-06 07:55:51.048541 canonicalwebteam_store_base-0.0.2/LICENSE
--rw-r--r--   0        0        0     1304 2023-06-06 07:55:51.048541 canonicalwebteam_store_base-0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-06-06 07:55:51.052541 canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/__init__.py
--rw-r--r--   0        0        0     1424 2023-06-06 07:55:51.052541 canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/app.py
--rw-r--r--   0        0        0        0 2023-06-06 07:55:51.052541 canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/auth/__init__.py
--rw-r--r--   0        0        0      385 2023-06-06 07:55:51.052541 canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/auth/authentication.py
--rw-r--r--   0        0        0     1656 2023-06-06 07:55:51.052541 canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/auth/logic.py
--rw-r--r--   0        0        0     3723 2023-06-06 07:55:51.052541 canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/auth/views.py
--rw-r--r--   0        0        0    27069 2023-06-06 07:55:51.052541 canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/data/licenses.json
--rw-r--r--   0        0        0     2745 2023-06-06 07:55:51.052541 canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/handlers.py
--rw-r--r--   0        0        0        0 2023-06-06 07:55:51.052541 canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/packages/__init__.py
--rw-r--r--   0        0        0     9736 2023-06-06 07:55:51.052541 canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/packages/logic.py
--rw-r--r--   0        0        0     2568 2023-06-06 07:55:51.052541 canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/packages/views.py
--rw-r--r--   0        0        0      201 2023-06-06 07:55:51.052541 canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/sample_blueprint/views.py
--rw-r--r--   0        0        0        0 2023-06-06 07:55:51.052541 canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/utils/__init__.py
--rw-r--r--   0        0        0     1089 2023-06-06 07:55:51.052541 canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/utils/config.py
--rw-r--r--   0        0        0      166 2023-06-06 07:55:51.052541 canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/utils/constants.py
--rw-r--r--   0        0        0      434 2023-06-06 07:55:51.052541 canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/utils/decorators.py
--rw-r--r--   0        0        0       61 2023-06-06 07:55:51.052541 canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/utils/extensions.py
--rw-r--r--   0        0        0     4608 2023-06-06 07:55:51.052541 canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/utils/helpers.py
--rw-r--r--   0        0        0       25 2023-06-06 07:55:51.052541 canonicalwebteam_store_base-0.0.2/canonicalwebteam/templates/storebase.html
--rw-r--r--   0        0        0     1050 2023-06-06 07:55:51.056541 canonicalwebteam_store_base-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2728 1970-01-01 00:00:00.000000 canonicalwebteam_store_base-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-09 08:20:07.747096 canonicalwebteam_store_base-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1304 2023-06-09 08:20:07.747096 canonicalwebteam_store_base-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-06-09 08:20:07.747096 canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/__init__.py
+-rw-r--r--   0        0        0     1424 2023-06-09 08:20:07.747096 canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/app.py
+-rw-r--r--   0        0        0        0 2023-06-09 08:20:07.747096 canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/auth/__init__.py
+-rw-r--r--   0        0        0      385 2023-06-09 08:20:07.747096 canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/auth/authentication.py
+-rw-r--r--   0        0        0     1656 2023-06-09 08:20:07.747096 canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/auth/logic.py
+-rw-r--r--   0        0        0     3723 2023-06-09 08:20:07.747096 canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/auth/views.py
+-rw-r--r--   0        0        0    27069 2023-06-09 08:20:07.747096 canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/data/licenses.json
+-rw-r--r--   0        0        0     2745 2023-06-09 08:20:07.747096 canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/handlers.py
+-rw-r--r--   0        0        0        0 2023-06-09 08:20:07.747096 canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/packages/__init__.py
+-rw-r--r--   0        0        0    10405 2023-06-09 08:20:07.747096 canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/packages/logic.py
+-rw-r--r--   0        0        0     2665 2023-06-09 08:20:07.747096 canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/packages/views.py
+-rw-r--r--   0        0        0      201 2023-06-09 08:20:07.747096 canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/sample_blueprint/views.py
+-rw-r--r--   0        0        0        0 2023-06-09 08:20:07.747096 canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/utils/__init__.py
+-rw-r--r--   0        0        0     1094 2023-06-09 08:20:07.747096 canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/utils/config.py
+-rw-r--r--   0        0        0      166 2023-06-09 08:20:07.747096 canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/utils/constants.py
+-rw-r--r--   0        0        0      434 2023-06-09 08:20:07.747096 canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/utils/decorators.py
+-rw-r--r--   0        0        0       61 2023-06-09 08:20:07.747096 canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/utils/extensions.py
+-rw-r--r--   0        0        0     4608 2023-06-09 08:20:07.747096 canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/utils/helpers.py
+-rw-r--r--   0        0        0       25 2023-06-09 08:20:07.747096 canonicalwebteam_store_base-0.0.3/canonicalwebteam/templates/storebase.html
+-rw-r--r--   0        0        0     1050 2023-06-09 08:20:07.751096 canonicalwebteam_store_base-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2728 1970-01-01 00:00:00.000000 canonicalwebteam_store_base-0.0.3/PKG-INFO
```

### Comparing `canonicalwebteam_store_base-0.0.2/LICENSE` & `canonicalwebteam_store_base-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_base-0.0.2/README.md` & `canonicalwebteam_store_base-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/app.py` & `canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/app.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/auth/logic.py` & `canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/auth/logic.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/auth/views.py` & `canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/auth/views.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/data/licenses.json` & `canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/data/licenses.json`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/handlers.py` & `canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/handlers.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/packages/logic.py` & `canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/packages/logic.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         "packages": List[
             Dict[str, Dict[str, str or List[str]] or List[Dict[str, str]]]
         ]
     },
 )
 
 
-def fetch_packages(store_api, fields: List[str]):
+def fetch_packages(store_api, fields: List[str]) -> Package:
     """
     Fetches packages from the store API based on the specified fields.
 
     :param: store_api: The specific store API object.
     :param: fields (List[str]): A list of fields to include in the package
     data.
 
@@ -34,29 +34,29 @@
     store = store_api(talisker.requests.get_session())
     packages = store.find(fields=fields).get("results", [])
     response = make_response({"packages": packages})
     response.cache_control.max_age = 3600
     return response.json
 
 
-def parse_package_for_card(package: Dict[str, Any]) -> Package:
+def parse_package_for_card(
+    package: Dict[str, Any], store_name: str
+) -> Package:
     """
     Parses a package (snap, charm, or bundle) and returns the formatted package
     based on the given card schema.
 
     :param: package (Dict[str, Any]): The package to be parsed.
     :returns: a dictionary containing the formatted package.
 
     note:
         - This function has to be refactored to be more generic,
         so we won't have to check for the package type before parsing.
 
     """
-
-    package_type = package.get("type", "")
     resp = {
         "package": {
             "description": "",
             "display_name": "",
             "icon_url": "",
             "name": "",
             "platforms": [],
@@ -64,15 +64,15 @@
         },
         "publisher": {"display_name": "", "name": "", "validation": ""},
         "categories": [],
         # hardcoded temporarily until we have this data from the API
         "ratings": {"value": "0", "count": "0"},
     }
 
-    if package_type == "charm" or package_type == "bundle":
+    if store_name.startswith("charmhub"):
         result = package.get("result", {})
         publisher = result.get("publisher", {})
 
         resp["package"]["type"] = package.get("type", "")
         resp["package"]["name"] = package.get("name", "")
         resp["package"]["description"] = result.get("summary", "")
         resp["package"]["display_name"] = result.get(
@@ -80,15 +80,16 @@
         )
         resp["package"]["platforms"] = result.get("deployable-on", [])
         resp["publisher"]["display_name"] = publisher.get("display-name", "")
         resp["publisher"]["validation"] = publisher.get("validation", "")
         resp["categories"] = result.get("categories", [])
         resp["package"]["icon_url"] = helpers.get_icon(result.get("media", []))
 
-    else:
+    if store_name.startswith("snapcraft"):
+        # pprint({package_type: package})
         snap = package.get("snap", {})
         publisher = snap.get("publisher", {})
         resp["package"]["description"] = snap.get("summary", "")
         resp["package"]["display_name"] = snap.get("title", "")
         resp["package"]["type"] = "snap"
         resp["package"]["name"] = package.get("name", "")
         # platform to be fetched
@@ -131,39 +132,54 @@
     if end > len(packages):
         end = len(packages)
 
     return packages[start:end]
 
 
 def get_packages(
-    store, fields: List[str], size: int = 10, page: int = 1
+    store,
+    store_name: str,
+    fields: List[str],
+    size: int = 10,
+    page: int = 1,
+    filters: Dict = {},
 ) -> List[Dict[str, Any]]:
     """
     Retrieves a list of packages from the store based on the specified
     parameters.The returned packages are paginated and parsed using the
     card schema.
 
     :param: store: The store object.
     :param: fields (List[str]): A list of fields to include in the
             package data.
     :param: size (int, optional): The number of packages to include
             in each page. Defaults to 10.
     :param: page (int, optional): The current page number. Defaults to 1.
+    :param: filters (Dict, optional): The filter parameters. Defaults to {}.
     :returns: a dictionary containing the list of parsed packages and
             the total pages
     """
 
     packages = fetch_packages(store, fields).get("packages", [])
     total_pages = -(len(packages) // -size)
-    packages_per_page = paginate(packages, page, size, total_pages)
-    parsed_packages = []
-    for package in packages_per_page:
-        parsed_packages.append(parse_package_for_card(package))
 
-    return {"packages": parsed_packages, "total_pages": total_pages}
+    if filters:
+        parsed_packages = []
+        for package in packages:
+            parsed_packages.append(parse_package_for_card(package, store_name))
+        filtered_packages = filter_packages(parsed_packages, filters)
+        res = paginate(filtered_packages, page, size, total_pages)
+    else:
+        packages_per_page = paginate(packages, page, size, total_pages)
+        parsed_packages = []
+        for package in packages_per_page:
+            parsed_packages.append(parse_package_for_card(package, store_name))
+        res = parsed_packages
+
+    return {"packages": res, "total_pages": total_pages}
 
 
 def filter_packages(
     packages: List[Package], filter_params: Dict[str, List[str]]
 ):
     """
     Filters the list of packages based on the specified filter parameters.
@@ -186,27 +202,30 @@
                         ]
                     )
                     != 0,
                     result,
                 )
             )
         if (key == "platforms" or key == "architectures") and "all" not in val:
+            platform = "platforms" if key == "platforms" else "architectures"
             result = list(
                 filter(
                     lambda package: len(
-                        [p for p in package["platforms"] if p in val]
+                        [p for p in package["package"][platform] if p in val]
                     )
                     != 0,
                     result,
                 )
             )
 
         if key == "type" and "all" not in val:
             result = list(
-                filter(lambda package: package["type"] in val, result)
+                filter(
+                    lambda package: package["package"]["type"] in val, result
+                )
             )
 
     return result
 
 
 def format_slug(slug):
     """Format category name into a standard title format
```

### Comparing `canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/packages/views.py` & `canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/packages/views.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,18 +21,25 @@
     __name__,
 )
 
 
 @store_packages.route("/store.json")
 def get_store_packages():
     app_name = app.name
+
+    filters = dict(request.args)
+    filters.pop("page", {})
     params = PACKAGE_PARAMS[app_name]
     store, fields, size = params["store"], params["fields"], params["size"]
+
     page = int(request.args.get("page", 1))
-    res = make_response(get_packages(store, fields, size, page))
+
+    res = make_response(
+        get_packages(store, app_name, fields, size, page, filters)
+    )
     return res
 
 
 @store_packages.route("/<any(charms, bundles, snaps):package_type>")
 @login_required
 def package(package_type):
     """
```

### Comparing `canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/utils/config.py` & `canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/utils/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,15 +22,15 @@
             "summary",
             "media",
             "publisher",
             "categories",
         ],
         "size": 15,
     },
-    "charmhub": {
+    "charmhub_beta": {
         "store": CharmStore,
         "publisher": CharmPublisher,
         "fields": [
             "result.categories",
             "result.summary",
             "result.media",
             "result.title",
```

### Comparing `canonicalwebteam_store_base-0.0.2/canonicalwebteam/store_base/utils/helpers.py` & `canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_base-0.0.2/pyproject.toml` & `canonicalwebteam_store_base-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "canonicalwebteam-store-base"
-version = "0.0.2"
+version = "0.0.3"
 description = "An application base for all stores"
 authors = ["Canonical Webteam <webteam@canonical.com>"]
 license = "GPL3"
 readme = "README.md"
 packages = [{include = "canonicalwebteam"}]
 
 [tool.poetry.dependencies]
```

### Comparing `canonicalwebteam_store_base-0.0.2/PKG-INFO` & `canonicalwebteam_store_base-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canonicalwebteam-store-base
-Version: 0.0.2
+Version: 0.0.3
 Summary: An application base for all stores
 License: GPL3
 Author: Canonical Webteam
 Author-email: webteam@canonical.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

