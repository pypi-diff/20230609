# Comparing `tmp/nso-oc-2.65.0.tar.gz` & `tmp/nso-oc-2.66.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nso-oc-2.65.0.tar", last modified: Tue Jun  6 18:11:55 2023, max compression
+gzip compressed data, was "nso-oc-2.66.1.tar", last modified: Thu Jun  8 18:33:07 2023, max compression
```

## Comparing `nso-oc-2.65.0.tar` & `nso-oc-2.66.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:11:55.506501 nso-oc-2.65.0/
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-06-06 18:11:27.000000 nso-oc-2.65.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-06 18:11:27.000000 nso-oc-2.65.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-06 18:11:55.506501 nso-oc-2.65.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-06 18:11:27.000000 nso-oc-2.65.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:11:55.502501 nso-oc-2.65.0/nso_oc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-06 18:11:55.000000 nso-oc-2.65.0/nso_oc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-06 18:11:55.000000 nso-oc-2.65.0/nso_oc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 18:11:55.000000 nso-oc-2.65.0/nso_oc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-06 18:11:55.000000 nso-oc-2.65.0/nso_oc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 18:11:55.000000 nso-oc-2.65.0/nso_oc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-06 18:11:55.000000 nso-oc-2.65.0/nso_oc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:11:55.502501 nso-oc-2.65.0/package_nso_to_oc/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-06 18:11:27.000000 nso-oc-2.65.0/package_nso_to_oc/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-06 18:11:27.000000 nso-oc-2.65.0/package_nso_to_oc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-06-06 18:11:27.000000 nso-oc-2.65.0/package_nso_to_oc/common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3569 2023-06-06 18:11:27.000000 nso-oc-2.65.0/package_nso_to_oc/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:11:55.506501 nso-oc-2.65.0/package_nso_to_oc/xe/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-06 18:11:27.000000 nso-oc-2.65.0/package_nso_to_oc/xe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-06-06 18:11:27.000000 nso-oc-2.65.0/package_nso_to_oc/xe/common_xe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-06-06 18:11:27.000000 nso-oc-2.65.0/package_nso_to_oc/xe/main_xe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30058 2023-06-06 18:11:27.000000 nso-oc-2.65.0/package_nso_to_oc/xe/xe_acls.py
--rw-r--r--   0 runner    (1001) docker     (123)    36678 2023-06-06 18:11:27.000000 nso-oc-2.65.0/package_nso_to_oc/xe/xe_bgp.py
--rw-r--r--   0 runner    (1001) docker     (123)    63537 2023-06-06 18:11:27.000000 nso-oc-2.65.0/package_nso_to_oc/xe/xe_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     8801 2023-06-06 18:11:27.000000 nso-oc-2.65.0/package_nso_to_oc/xe/xe_mpls.py
--rw-r--r--   0 runner    (1001) docker     (123)    42335 2023-06-06 18:11:27.000000 nso-oc-2.65.0/package_nso_to_oc/xe/xe_network_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)    40463 2023-06-06 18:11:27.000000 nso-oc-2.65.0/package_nso_to_oc/xe/xe_ospfv2.py
--rw-r--r--   0 runner    (1001) docker     (123)    29881 2023-06-06 18:11:27.000000 nso-oc-2.65.0/package_nso_to_oc/xe/xe_routing_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8996 2023-06-06 18:11:27.000000 nso-oc-2.65.0/package_nso_to_oc/xe/xe_static_route.py
--rw-r--r--   0 runner    (1001) docker     (123)    32957 2023-06-06 18:11:27.000000 nso-oc-2.65.0/package_nso_to_oc/xe/xe_stp.py
--rw-r--r--   0 runner    (1001) docker     (123)   105916 2023-06-06 18:11:27.000000 nso-oc-2.65.0/package_nso_to_oc/xe/xe_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-06-06 18:11:27.000000 nso-oc-2.65.0/package_nso_to_oc/xe/xe_vlans.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:11:55.506501 nso-oc-2.65.0/package_nso_to_oc/xr/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-06 18:11:27.000000 nso-oc-2.65.0/package_nso_to_oc/xr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-06 18:11:27.000000 nso-oc-2.65.0/package_nso_to_oc/xr/common_xr.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-06 18:11:27.000000 nso-oc-2.65.0/package_nso_to_oc/xr/main_xr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23665 2023-06-06 18:11:27.000000 nso-oc-2.65.0/package_nso_to_oc/xr/xr_acls.py
--rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-06-06 18:11:27.000000 nso-oc-2.65.0/package_nso_to_oc/xr/xr_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-06-06 18:11:27.000000 nso-oc-2.65.0/package_nso_to_oc/xr/xr_system.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-06 18:11:27.000000 nso-oc-2.65.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-06 18:11:55.506501 nso-oc-2.65.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-06 18:11:27.000000 nso-oc-2.65.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:33:07.480641 nso-oc-2.66.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-06-08 18:32:39.000000 nso-oc-2.66.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-08 18:32:39.000000 nso-oc-2.66.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-08 18:33:07.480641 nso-oc-2.66.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-08 18:32:39.000000 nso-oc-2.66.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:33:07.476642 nso-oc-2.66.1/nso_oc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-08 18:33:07.000000 nso-oc-2.66.1/nso_oc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-08 18:33:07.000000 nso-oc-2.66.1/nso_oc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 18:33:07.000000 nso-oc-2.66.1/nso_oc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-08 18:33:07.000000 nso-oc-2.66.1/nso_oc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-08 18:33:07.000000 nso-oc-2.66.1/nso_oc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-08 18:33:07.000000 nso-oc-2.66.1/nso_oc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:33:07.480641 nso-oc-2.66.1/package_nso_to_oc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-08 18:32:39.000000 nso-oc-2.66.1/package_nso_to_oc/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-08 18:32:39.000000 nso-oc-2.66.1/package_nso_to_oc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-06-08 18:32:39.000000 nso-oc-2.66.1/package_nso_to_oc/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3569 2023-06-08 18:32:39.000000 nso-oc-2.66.1/package_nso_to_oc/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:33:07.480641 nso-oc-2.66.1/package_nso_to_oc/xe/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 18:32:39.000000 nso-oc-2.66.1/package_nso_to_oc/xe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-06-08 18:32:39.000000 nso-oc-2.66.1/package_nso_to_oc/xe/common_xe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-06-08 18:32:39.000000 nso-oc-2.66.1/package_nso_to_oc/xe/main_xe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30058 2023-06-08 18:32:39.000000 nso-oc-2.66.1/package_nso_to_oc/xe/xe_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36678 2023-06-08 18:32:39.000000 nso-oc-2.66.1/package_nso_to_oc/xe/xe_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63537 2023-06-08 18:32:39.000000 nso-oc-2.66.1/package_nso_to_oc/xe/xe_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-06-08 18:32:39.000000 nso-oc-2.66.1/package_nso_to_oc/xe/xe_mpls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42337 2023-06-08 18:32:39.000000 nso-oc-2.66.1/package_nso_to_oc/xe/xe_network_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40463 2023-06-08 18:32:39.000000 nso-oc-2.66.1/package_nso_to_oc/xe/xe_ospfv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29881 2023-06-08 18:32:39.000000 nso-oc-2.66.1/package_nso_to_oc/xe/xe_routing_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8996 2023-06-08 18:32:39.000000 nso-oc-2.66.1/package_nso_to_oc/xe/xe_static_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32957 2023-06-08 18:32:39.000000 nso-oc-2.66.1/package_nso_to_oc/xe/xe_stp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105916 2023-06-08 18:32:39.000000 nso-oc-2.66.1/package_nso_to_oc/xe/xe_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-06-08 18:32:39.000000 nso-oc-2.66.1/package_nso_to_oc/xe/xe_vlans.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:33:07.480641 nso-oc-2.66.1/package_nso_to_oc/xr/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 18:32:39.000000 nso-oc-2.66.1/package_nso_to_oc/xr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-08 18:32:39.000000 nso-oc-2.66.1/package_nso_to_oc/xr/common_xr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-08 18:32:39.000000 nso-oc-2.66.1/package_nso_to_oc/xr/main_xr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23665 2023-06-08 18:32:39.000000 nso-oc-2.66.1/package_nso_to_oc/xr/xr_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-06-08 18:32:39.000000 nso-oc-2.66.1/package_nso_to_oc/xr/xr_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-06-08 18:32:39.000000 nso-oc-2.66.1/package_nso_to_oc/xr/xr_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-08 18:32:39.000000 nso-oc-2.66.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-08 18:33:07.480641 nso-oc-2.66.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-08 18:32:39.000000 nso-oc-2.66.1/setup.py
```

### Comparing `nso-oc-2.65.0/LICENSE` & `nso-oc-2.66.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nso-oc-2.65.0/PKG-INFO` & `nso-oc-2.66.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nso-oc
-Version: 2.65.0
+Version: 2.66.1
 Summary: Cisco NSO OpenConfig Tools
 Home-page: https://github.com/model-driven-devops/nso-oc-services
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## NSO NED device configuration to OpenConfig
```

### Comparing `nso-oc-2.65.0/README.md` & `nso-oc-2.66.1/README.md`

 * *Files identical despite different names*

### Comparing `nso-oc-2.65.0/nso_oc.egg-info/PKG-INFO` & `nso-oc-2.66.1/nso_oc.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nso-oc
-Version: 2.65.0
+Version: 2.66.1
 Summary: Cisco NSO OpenConfig Tools
 Home-page: https://github.com/model-driven-devops/nso-oc-services
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## NSO NED device configuration to OpenConfig
```

### Comparing `nso-oc-2.65.0/nso_oc.egg-info/SOURCES.txt` & `nso-oc-2.66.1/nso_oc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nso-oc-2.65.0/package_nso_to_oc/README.md` & `nso-oc-2.66.1/package_nso_to_oc/README.md`

 * *Files identical despite different names*

### Comparing `nso-oc-2.65.0/package_nso_to_oc/common.py` & `nso-oc-2.66.1/package_nso_to_oc/common.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.65.0/package_nso_to_oc/main.py` & `nso-oc-2.66.1/package_nso_to_oc/main.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.65.0/package_nso_to_oc/xe/common_xe.py` & `nso-oc-2.66.1/package_nso_to_oc/xe/common_xe.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.65.0/package_nso_to_oc/xe/main_xe.py` & `nso-oc-2.66.1/package_nso_to_oc/xe/main_xe.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.65.0/package_nso_to_oc/xe/xe_acls.py` & `nso-oc-2.66.1/package_nso_to_oc/xe/xe_acls.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.65.0/package_nso_to_oc/xe/xe_bgp.py` & `nso-oc-2.66.1/package_nso_to_oc/xe/xe_bgp.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.65.0/package_nso_to_oc/xe/xe_interfaces.py` & `nso-oc-2.66.1/package_nso_to_oc/xe/xe_interfaces.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.65.0/package_nso_to_oc/xe/xe_mpls.py` & `nso-oc-2.66.1/package_nso_to_oc/xe/xe_mpls.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 else:
     import common
 
 mpls_notes = []
 
 
 def configure_xe_mpls(net_inst, config_before, config_leftover, network_instances_notes):
+    if net_inst["openconfig-network-instance:config"]["openconfig-network-instance:name"] == "management":
+        return
+    
     mpls_before = config_before.get("tailf-ned-cisco-ios:mpls", {})
     mpls_leftover = config_leftover.get("tailf-ned-cisco-ios:mpls", {})
     process_propagate_ttl(net_inst, mpls_before, mpls_leftover)
     process_mpls_intf(net_inst, config_before, config_leftover, mpls_before, mpls_leftover)
     process_ldp(net_inst, config_before, mpls_before, mpls_leftover)
     network_instances_notes += mpls_notes
 
@@ -39,23 +42,22 @@
         mpls_global["openconfig-network-instance:config"]["openconfig-network-instance:ttl-propagation"] = True
         
     if len(mpls_leftover.get("mpls-ip-conf", {}).get("ip", {}).get("propagate-ttl-conf", {})) > 0:
         del mpls_leftover["mpls-ip-conf"]
 
 
 def process_mpls_intf(net_inst, config_before, config_leftover, mpls_before, mpls_leftover):
-    if not mpls_before.get("ip"):
-        return
-    
+    if mpls_before.get("ip") == False:
+        raise ValueError("Invalid value of false for global MPLS IP")
     if mpls_leftover.get("ip") != None:
         del mpls_leftover["ip"]
-    
+
     for intf_type in config_before.get("tailf-ned-cisco-ios:interface", {}):
         for intf_num, current_intf in enumerate(config_before["tailf-ned-cisco-ios:interface"].get(intf_type, [])):
-            if (current_intf.get("mpls", {}).get("ip")):
+            if type(current_intf) == dict and current_intf.get("mpls", {}).get("ip"):
                 set_mpls_interface(net_inst, intf_type, current_intf.get("name", ""))
 
                 leftover_intf = common.get_index_or_default(
                     config_leftover.get("tailf-ned-cisco-ios:interface", {}).get(intf_type, {}), intf_num)
                 if leftover_intf.get("mpls", {}).get("ip", None) != None:
                     del leftover_intf["mpls"]
 
@@ -110,15 +112,15 @@
         if not current_ip:
             continue
         if current_intf.get("name", None) == intf_num:
             get_ldp_global(net_inst_mpls_ldp)["openconfig-network-instance:config"] = {
                 "openconfig-network-instance:lsr-id": current_ip
             }
 
-            if mpls_leftover.get("ldp", {}).get("router-id", {}) != None:
+            if mpls_leftover.get("ldp", {}).get("router-id") != None:
                 del mpls_leftover["ldp"]["router-id"]
 
             return
 
 
 def process_graceful_restart(net_inst_mpls_ldp, ldp_before, mpls_leftover):
     if ldp_before.get("graceful-restart-enable", {}).get("graceful-restart"):
```

### Comparing `nso-oc-2.65.0/package_nso_to_oc/xe/xe_network_instances.py` & `nso-oc-2.66.1/package_nso_to_oc/xe/xe_network_instances.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,15 @@
             vrf_forwarding_list = route_forwarding_list_by_vrf.get(net_inst["openconfig-network-instance:name"])
             xe_static_route.configure_xe_static_routes(net_inst, vrf_forwarding_list, config_leftover,
                                                        network_instances_notes)
         
         xe_ospfv2.configure_xe_ospf_redistribution(net_inst, config_before, config_leftover, router_ospf_by_vrf)
         xe_bgp.configure_xe_bgp(net_inst, config_before, config_leftover, network_instances_notes)
         xe_bgp.configure_xe_bgp_redistribution(net_inst, config_before, config_leftover)
-        xe_mpls.configure_xe_mpls(net_inst, config_before, config_before, network_instances_notes)
+        xe_mpls.configure_xe_mpls(net_inst, config_before, config_leftover, network_instances_notes)
 
 
 def configure_network_interfaces(net_inst, interfaces_by_vrf):
     for interface in interfaces_by_vrf.get(net_inst["openconfig-network-instance:name"], []):
         name_split = interface["name"].split(".")
         primary_interface = name_split[0]
         new_interface = {
```

### Comparing `nso-oc-2.65.0/package_nso_to_oc/xe/xe_ospfv2.py` & `nso-oc-2.66.1/package_nso_to_oc/xe/xe_ospfv2.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.65.0/package_nso_to_oc/xe/xe_routing_policy.py` & `nso-oc-2.66.1/package_nso_to_oc/xe/xe_routing_policy.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.65.0/package_nso_to_oc/xe/xe_static_route.py` & `nso-oc-2.66.1/package_nso_to_oc/xe/xe_static_route.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.65.0/package_nso_to_oc/xe/xe_stp.py` & `nso-oc-2.66.1/package_nso_to_oc/xe/xe_stp.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.65.0/package_nso_to_oc/xe/xe_system.py` & `nso-oc-2.66.1/package_nso_to_oc/xe/xe_system.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.65.0/package_nso_to_oc/xe/xe_vlans.py` & `nso-oc-2.66.1/package_nso_to_oc/xe/xe_vlans.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.65.0/package_nso_to_oc/xr/common_xr.py` & `nso-oc-2.66.1/package_nso_to_oc/xr/common_xr.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.65.0/package_nso_to_oc/xr/main_xr.py` & `nso-oc-2.66.1/package_nso_to_oc/xr/main_xr.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.65.0/package_nso_to_oc/xr/xr_acls.py` & `nso-oc-2.66.1/package_nso_to_oc/xr/xr_acls.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.65.0/package_nso_to_oc/xr/xr_interfaces.py` & `nso-oc-2.66.1/package_nso_to_oc/xr/xr_interfaces.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.65.0/package_nso_to_oc/xr/xr_system.py` & `nso-oc-2.66.1/package_nso_to_oc/xr/xr_system.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.65.0/setup.py` & `nso-oc-2.66.1/setup.py`

 * *Files identical despite different names*

