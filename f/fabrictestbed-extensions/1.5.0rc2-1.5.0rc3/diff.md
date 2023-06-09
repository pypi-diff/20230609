# Comparing `tmp/fabrictestbed-extensions-1.5.0rc2.tar.gz` & `tmp/fabrictestbed-extensions-1.5.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabrictestbed-extensions-1.5.0rc2.tar", last modified: Fri May 12 13:48:12 2023, max compression
+gzip compressed data, was "fabrictestbed-extensions-1.5.0rc3.tar", last modified: Mon May 22 14:08:17 2023, max compression
```

## Comparing `fabrictestbed-extensions-1.5.0rc2.tar` & `fabrictestbed-extensions-1.5.0rc3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1025 2023-05-11 18:23:24.341681 fabrictestbed-extensions-1.5.0rc2/.github/workflows/build.yml
--rw-r--r--   0        0        0     1618 2023-05-11 18:23:24.341808 fabrictestbed-extensions-1.5.0rc2/.github/workflows/checks.yml
--rw-r--r--   0        0        0     2402 2023-05-11 18:23:24.341926 fabrictestbed-extensions-1.5.0rc2/.github/workflows/test.yml
--rw-r--r--   0        0        0     1806 2023-05-12 13:41:06.568624 fabrictestbed-extensions-1.5.0rc2/.gitignore
--rw-r--r--   0        0        0      666 2023-05-11 18:23:24.342134 fabrictestbed-extensions-1.5.0rc2/.readthedocs.yaml
--rw-r--r--   0        0        0     2670 2023-05-11 18:23:24.342247 fabrictestbed-extensions-1.5.0rc2/CHANGELOG.md
--rw-r--r--   0        0        0     1071 2023-05-11 18:23:24.342656 fabrictestbed-extensions-1.5.0rc2/LICENSE
--rw-r--r--   0        0        0     4054 2023-05-11 18:23:24.342855 fabrictestbed-extensions-1.5.0rc2/README.md
--rw-r--r--   0        0        0      638 2023-05-11 18:23:24.343022 fabrictestbed-extensions-1.5.0rc2/docs/Makefile
--rw-r--r--   0        0        0      799 2023-05-11 18:23:24.343131 fabrictestbed-extensions-1.5.0rc2/docs/make.bat
--rw-r--r--   0        0        0     1996 2023-05-11 18:23:24.343312 fabrictestbed-extensions-1.5.0rc2/docs/source/conf.py
--rw-r--r--   0        0        0     8903 2023-05-12 13:41:06.569256 fabrictestbed-extensions-1.5.0rc2/docs/source/fablib.rst
--rw-r--r--   0        0        0     4470 2023-05-11 18:23:24.343613 fabrictestbed-extensions-1.5.0rc2/docs/source/index.rst
--rw-r--r--   0        0        0      150 2023-05-12 13:48:08.068598 fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/__init__.py
--rw-r--r--   0        0        0        2 2023-05-11 18:23:24.344271 fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/editors/__init__.py
--rw-r--r--   0        0        0    18044 2023-05-11 18:23:24.344572 fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/editors/abc_topology_editor.py
--rw-r--r--   0        0        0     6277 2023-05-11 18:23:24.345052 fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/editors/cytoscape_topology_editor.py
--rw-r--r--   0        0        0    68479 2023-05-11 18:23:24.345347 fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/editors/geo_topology_editor.py
--rw-r--r--   0        0        0        1 2023-05-11 18:23:24.345570 fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/fablib/__init__.py
--rw-r--r--   0        0        0     4793 2023-05-11 18:23:24.345738 fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/fablib/abc_fablib.py
--rw-r--r--   0        0        0    21062 2023-05-11 18:23:24.345997 fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/fablib/component.py
--rw-r--r--   0        0        0    76799 2023-05-11 18:23:24.346796 fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/fablib/fablib.py
--rw-r--r--   0        0        0     5807 2023-05-11 18:23:24.347162 fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/fablib/facility_port.py
--rw-r--r--   0        0        0    25967 2023-05-11 18:23:24.347819 fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/fablib/interface.py
--rw-r--r--   0        0        0    40005 2023-05-12 13:41:06.570962 fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/fablib/network_service.py
--rw-r--r--   0        0        0    95919 2023-05-11 18:23:24.348593 fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/fablib/node.py
--rw-r--r--   0        0        0    34672 2023-05-11 18:23:24.349105 fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/fablib/resources.py
--rw-r--r--   0        0        0    81904 2023-05-11 18:23:24.349763 fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/fablib/slice.py
--rw-r--r--   0        0        0        2 2023-05-11 18:23:24.350075 fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/images/__init__.py
--rw-r--r--   0        0        0   199914 2023-05-11 18:23:24.351514 fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/images/fabric_logo.png
--rw-r--r--   0        0        0     1316 2023-05-11 18:23:24.351919 fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/images/server.png
--rw-r--r--   0        0        0    62250 2023-05-11 18:23:24.352243 fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/images/slice_rack.png
--rw-r--r--   0        0        0        2 2023-05-11 18:23:24.352522 fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/tests/__init__.py
--rw-r--r--   0        0        0    14765 2023-05-11 18:23:24.352740 fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/tests/abc_test.py
--rw-r--r--   0        0        0    34231 2023-05-11 18:23:24.353058 fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/tests/component_tests.py
--rw-r--r--   0        0        0       85 2023-05-11 18:23:24.353250 fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/tests/dummy-token.json
--rw-r--r--   0        0        0    13366 2023-05-11 18:23:24.353667 fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/tests/gpu_tesla_t4_benchmark.py
--rw-r--r--   0        0        0    10227 2023-05-11 18:23:24.353942 fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/tests/hello_fabric.py
--rw-r--r--   0        0        0    20659 2023-05-11 18:23:24.354269 fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/tests/link_benchmark.py
--rw-r--r--   0        0        0    20919 2023-05-11 18:23:24.354513 fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/tests/local_network_benchmark.py
--rw-r--r--   0        0        0    44883 2023-05-11 18:23:24.354856 fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/tests/network_benchmark_tests.py
--rw-r--r--   0        0        0    10052 2023-05-11 18:23:24.355043 fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/tests/nvme_benchmark.py
--rw-r--r--   0        0        0     5095 2023-05-11 18:23:24.355416 fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/tests/test_basic.py
--rw-r--r--   0        0        0        2 2023-05-11 18:23:24.355793 fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/utils/__init__.py
--rw-r--r--   0        0        0     3082 2023-05-11 18:23:24.356170 fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/utils/abc_utils.py
--rw-r--r--   0        0        0     3304 2023-05-11 18:23:24.356417 fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/utils/node.py
--rw-r--r--   0        0        0     8436 2023-05-11 18:23:24.356653 fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/utils/slice.py
--rw-r--r--   0        0        0     1329 2023-05-12 13:47:58.788785 fabrictestbed-extensions-1.5.0rc2/pyproject.toml
--rwxr-xr-x   0        0        0      122 2023-05-11 18:23:24.357218 fabrictestbed-extensions-1.5.0rc2/sphinx.sh
--rw-r--r--   0        0        0     5278 1970-01-01 00:00:00.000000 fabrictestbed-extensions-1.5.0rc2/PKG-INFO
+-rw-r--r--   0        0        0     1025 2023-05-11 18:23:24.341681 fabrictestbed-extensions-1.5.0rc3/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1618 2023-05-11 18:23:24.341808 fabrictestbed-extensions-1.5.0rc3/.github/workflows/checks.yml
+-rw-r--r--   0        0        0     2402 2023-05-11 18:23:24.341926 fabrictestbed-extensions-1.5.0rc3/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1806 2023-05-12 13:41:06.568624 fabrictestbed-extensions-1.5.0rc3/.gitignore
+-rw-r--r--   0        0        0      666 2023-05-11 18:23:24.342134 fabrictestbed-extensions-1.5.0rc3/.readthedocs.yaml
+-rw-r--r--   0        0        0     2670 2023-05-11 18:23:24.342247 fabrictestbed-extensions-1.5.0rc3/CHANGELOG.md
+-rw-r--r--   0        0        0     1071 2023-05-11 18:23:24.342656 fabrictestbed-extensions-1.5.0rc3/LICENSE
+-rw-r--r--   0        0        0     4054 2023-05-11 18:23:24.342855 fabrictestbed-extensions-1.5.0rc3/README.md
+-rw-r--r--   0        0        0      638 2023-05-11 18:23:24.343022 fabrictestbed-extensions-1.5.0rc3/docs/Makefile
+-rw-r--r--   0        0        0      799 2023-05-11 18:23:24.343131 fabrictestbed-extensions-1.5.0rc3/docs/make.bat
+-rw-r--r--   0        0        0     1996 2023-05-11 18:23:24.343312 fabrictestbed-extensions-1.5.0rc3/docs/source/conf.py
+-rw-r--r--   0        0        0     8903 2023-05-12 13:41:06.569256 fabrictestbed-extensions-1.5.0rc3/docs/source/fablib.rst
+-rw-r--r--   0        0        0     4470 2023-05-11 18:23:24.343613 fabrictestbed-extensions-1.5.0rc3/docs/source/index.rst
+-rw-r--r--   0        0        0      150 2023-05-22 14:07:41.148032 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/__init__.py
+-rw-r--r--   0        0        0        2 2023-05-11 18:23:24.344271 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/editors/__init__.py
+-rw-r--r--   0        0        0    18044 2023-05-11 18:23:24.344572 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/editors/abc_topology_editor.py
+-rw-r--r--   0        0        0     6277 2023-05-11 18:23:24.345052 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/editors/cytoscape_topology_editor.py
+-rw-r--r--   0        0        0    68479 2023-05-11 18:23:24.345347 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/editors/geo_topology_editor.py
+-rw-r--r--   0        0        0        1 2023-05-11 18:23:24.345570 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/fablib/__init__.py
+-rw-r--r--   0        0        0     4793 2023-05-11 18:23:24.345738 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/fablib/abc_fablib.py
+-rw-r--r--   0        0        0    21062 2023-05-11 18:23:24.345997 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/fablib/component.py
+-rw-r--r--   0        0        0    76799 2023-05-11 18:23:24.346796 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/fablib/fablib.py
+-rw-r--r--   0        0        0     5807 2023-05-11 18:23:24.347162 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/fablib/facility_port.py
+-rw-r--r--   0        0        0    25967 2023-05-11 18:23:24.347819 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/fablib/interface.py
+-rw-r--r--   0        0        0    40005 2023-05-12 13:41:06.570962 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/fablib/network_service.py
+-rw-r--r--   0        0        0    95919 2023-05-11 18:23:24.348593 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/fablib/node.py
+-rw-r--r--   0        0        0    34726 2023-05-22 14:06:53.930637 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/fablib/resources.py
+-rw-r--r--   0        0        0    81904 2023-05-11 18:23:24.349763 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/fablib/slice.py
+-rw-r--r--   0        0        0        2 2023-05-11 18:23:24.350075 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/images/__init__.py
+-rw-r--r--   0        0        0   199914 2023-05-11 18:23:24.351514 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/images/fabric_logo.png
+-rw-r--r--   0        0        0     1316 2023-05-11 18:23:24.351919 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/images/server.png
+-rw-r--r--   0        0        0    62250 2023-05-11 18:23:24.352243 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/images/slice_rack.png
+-rw-r--r--   0        0        0        2 2023-05-11 18:23:24.352522 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/tests/__init__.py
+-rw-r--r--   0        0        0    14765 2023-05-11 18:23:24.352740 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/tests/abc_test.py
+-rw-r--r--   0        0        0    34231 2023-05-11 18:23:24.353058 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/tests/component_tests.py
+-rw-r--r--   0        0        0       85 2023-05-11 18:23:24.353250 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/tests/dummy-token.json
+-rw-r--r--   0        0        0    13366 2023-05-11 18:23:24.353667 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/tests/gpu_tesla_t4_benchmark.py
+-rw-r--r--   0        0        0    10227 2023-05-11 18:23:24.353942 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/tests/hello_fabric.py
+-rw-r--r--   0        0        0    20659 2023-05-11 18:23:24.354269 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/tests/link_benchmark.py
+-rw-r--r--   0        0        0    20919 2023-05-11 18:23:24.354513 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/tests/local_network_benchmark.py
+-rw-r--r--   0        0        0    44883 2023-05-11 18:23:24.354856 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/tests/network_benchmark_tests.py
+-rw-r--r--   0        0        0    10052 2023-05-11 18:23:24.355043 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/tests/nvme_benchmark.py
+-rw-r--r--   0        0        0     5095 2023-05-11 18:23:24.355416 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/tests/test_basic.py
+-rw-r--r--   0        0        0        2 2023-05-11 18:23:24.355793 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/utils/__init__.py
+-rw-r--r--   0        0        0     3082 2023-05-11 18:23:24.356170 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/utils/abc_utils.py
+-rw-r--r--   0        0        0     3304 2023-05-11 18:23:24.356417 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/utils/node.py
+-rw-r--r--   0        0        0     8436 2023-05-11 18:23:24.356653 fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/utils/slice.py
+-rw-r--r--   0        0        0     1329 2023-05-12 13:47:58.788785 fabrictestbed-extensions-1.5.0rc3/pyproject.toml
+-rwxr-xr-x   0        0        0      122 2023-05-11 18:23:24.357218 fabrictestbed-extensions-1.5.0rc3/sphinx.sh
+-rw-r--r--   0        0        0     5278 1970-01-01 00:00:00.000000 fabrictestbed-extensions-1.5.0rc3/PKG-INFO
```

### Comparing `fabrictestbed-extensions-1.5.0rc2/.github/workflows/build.yml` & `fabrictestbed-extensions-1.5.0rc3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc2/.github/workflows/checks.yml` & `fabrictestbed-extensions-1.5.0rc3/.github/workflows/checks.yml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc2/.github/workflows/test.yml` & `fabrictestbed-extensions-1.5.0rc3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc2/.gitignore` & `fabrictestbed-extensions-1.5.0rc3/.gitignore`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc2/.readthedocs.yaml` & `fabrictestbed-extensions-1.5.0rc3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc2/CHANGELOG.md` & `fabrictestbed-extensions-1.5.0rc3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc2/LICENSE` & `fabrictestbed-extensions-1.5.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc2/README.md` & `fabrictestbed-extensions-1.5.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc2/docs/Makefile` & `fabrictestbed-extensions-1.5.0rc3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc2/docs/make.bat` & `fabrictestbed-extensions-1.5.0rc3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc2/docs/source/conf.py` & `fabrictestbed-extensions-1.5.0rc3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc2/docs/source/fablib.rst` & `fabrictestbed-extensions-1.5.0rc3/docs/source/fablib.rst`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc2/docs/source/index.rst` & `fabrictestbed-extensions-1.5.0rc3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/editors/abc_topology_editor.py` & `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/editors/abc_topology_editor.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/editors/cytoscape_topology_editor.py` & `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/editors/cytoscape_topology_editor.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/editors/geo_topology_editor.py` & `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/editors/geo_topology_editor.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/fablib/abc_fablib.py` & `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/fablib/abc_fablib.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/fablib/component.py` & `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/fablib/component.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/fablib/fablib.py` & `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/fablib/fablib.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/fablib/facility_port.py` & `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/fablib/facility_port.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/fablib/interface.py` & `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/fablib/interface.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/fablib/network_service.py` & `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/fablib/network_service.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/fablib/node.py` & `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/fablib/node.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/fablib/resources.py` & `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/fablib/resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,20 +195,19 @@
             return self.topology.sites[site_name]
         except Exception as e:
             logging.warning(f"Failed to get site {site_name}")
             return ""
 
     def get_state(self, site_name: str):
         try:
-            return str(
-                self.get_topology_site(site_name)
-                .get_property("maintenance_info")
-                .get(site_name)
-                .state
-            )
+            maint_info = self.get_topology_site(site_name).get_property("maintenance_info")
+            if maint_info.get(site_name) is None:
+                return "Active"
+            else:
+                return maint_info.get(site_name).state
         except Exception as e:
             logging.warning(f"Failed to get site state {site_name}")
             return ""
 
     def get_component_capacity(self, site_name: str, component_model_name: str) -> int:
         """
         Gets gets the total site capacity of a component by model name.
```

### Comparing `fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/fablib/slice.py` & `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/fablib/slice.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/images/fabric_logo.png` & `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/images/fabric_logo.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/images/server.png` & `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/images/server.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/images/slice_rack.png` & `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/images/slice_rack.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/tests/abc_test.py` & `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/tests/abc_test.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/tests/component_tests.py` & `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/tests/component_tests.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/tests/gpu_tesla_t4_benchmark.py` & `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/tests/gpu_tesla_t4_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/tests/hello_fabric.py` & `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/tests/hello_fabric.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/tests/link_benchmark.py` & `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/tests/link_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/tests/local_network_benchmark.py` & `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/tests/local_network_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/tests/network_benchmark_tests.py` & `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/tests/network_benchmark_tests.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/tests/nvme_benchmark.py` & `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/tests/nvme_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/tests/test_basic.py` & `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/utils/abc_utils.py` & `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/utils/abc_utils.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/utils/node.py` & `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/utils/node.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc2/fabrictestbed_extensions/utils/slice.py` & `fabrictestbed-extensions-1.5.0rc3/fabrictestbed_extensions/utils/slice.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc2/pyproject.toml` & `fabrictestbed-extensions-1.5.0rc3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc2/PKG-INFO` & `fabrictestbed-extensions-1.5.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabrictestbed-extensions
-Version: 1.5.0rc2
+Version: 1.5.0rc3
 Summary: FABRIC Python Client Library and CLI Extensions
 Author-email: Paul Ruth <pruth@renci.org>, Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

