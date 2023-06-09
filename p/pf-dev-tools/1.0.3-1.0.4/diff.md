# Comparing `tmp/pf_dev_tools-1.0.3.tar.gz` & `tmp/pf_dev_tools-1.0.4.tar.gz`

## Comparing `pf_dev_tools-1.0.3.tar` & `pf_dev_tools-1.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/.flake8
--rw-r--r--   0        0        0    27037 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/.nova/Artwork
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/.nova/Configuration.json
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/pfDevTools/Exceptions.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/pfDevTools/__about__.py
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/pfDevTools/__init__.py
--rw-r--r--   0        0        0     5906 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/pfDevTools/pfBuildCore.py
--rw-r--r--   0        0        0     4342 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/pfDevTools/pfConfig.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/pfDevTools/pfSconsEnvironment.py
--rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/pfDevTools/pfUtils.py
--rwxr-xr-x   0        0        0     1080 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/pfDevTools/pfCommand/__main__.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfClean.py
--rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfClone.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfCommand.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfConvert.py
--rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfDelete.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfDryRun.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfEject.py
--rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfInstall.py
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfMake.py
--rw-r--r--   0        0        0     9978 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfPackage.py
--rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfQfs.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfReverse.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/LICENSE
--rw-r--r--   0        0        0    10264 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/README.md
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/pyproject.toml
--rw-r--r--   0        0        0    11324 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/.flake8
+-rw-r--r--   0        0        0    27037 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/.nova/Artwork
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/.nova/Configuration.json
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/pfDevTools/Exceptions.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/pfDevTools/__about__.py
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/pfDevTools/__init__.py
+-rw-r--r--   0        0        0     5927 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/pfDevTools/pfBuildCore.py
+-rw-r--r--   0        0        0     4342 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/pfDevTools/pfConfig.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/pfDevTools/pfSconsEnvironment.py
+-rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/pfDevTools/pfUtils.py
+-rwxr-xr-x   0        0        0     1080 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/pfDevTools/pfCommand/__main__.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfClean.py
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfClone.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfCommand.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfConvert.py
+-rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfDelete.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfDryRun.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfEject.py
+-rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfInstall.py
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfMake.py
+-rw-r--r--   0        0        0     9978 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfPackage.py
+-rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfQfs.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfReverse.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/LICENSE
+-rw-r--r--   0        0        0    10264 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/README.md
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0    11324 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/PKG-INFO
```

### Comparing `pf_dev_tools-1.0.3/.nova/Artwork` & `pf_dev_tools-1.0.4/.nova/Artwork`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.3/pfDevTools/__init__.py` & `pf_dev_tools-1.0.4/pfDevTools/__init__.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.3/pfDevTools/pfBuildCore.py` & `pf_dev_tools-1.0.4/pfDevTools/pfBuildCore.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,15 @@
         env.Command(core_input_qsf_file, '', pfBuildCore._cloneRepo)
 
         dest_verilog_files: List[str] = pfBuildCore._searchSourceFiles(env, src_folder, dest_verilog_folder)
         extra_dest_files: List[str] = pfBuildCore._addExtraFiles(env, src_folder, dest_verilog_folder, extra_files)
 
         env.Command(core_output_qsf_file, [core_input_qsf_file] + dest_verilog_files, pfBuildCore._updateQsfFile)
 
-        env.Command(core_output_bitstream_file, [core_output_qsf_file] + extra_dest_files, pfBuildCore._compileBitStream)
+        env.Command(core_output_bitstream_file, [core_output_qsf_file] + dest_verilog_files + extra_dest_files, pfBuildCore._compileBitStream)
 
         build_process: pfDevTools.pfPackage = pfDevTools.pfPackage([config_file, core_output_bitstream_file, build_folder])
         packaged_core = os.path.join(build_folder, build_process.packagedFilename())
         p = env.Command(packaged_core, build_process.dependencies(), pfBuildCore._packageCore)
 
         env.Default(packaged_core)
         env.Clean(packaged_core, build_folder)
```

### Comparing `pf_dev_tools-1.0.3/pfDevTools/pfConfig.py` & `pf_dev_tools-1.0.4/pfDevTools/pfConfig.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.3/pfDevTools/pfUtils.py` & `pf_dev_tools-1.0.4/pfDevTools/pfUtils.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.3/pfDevTools/pfCommand/__main__.py` & `pf_dev_tools-1.0.4/pfDevTools/pfCommand/__main__.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfClean.py` & `pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfClean.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfClone.py` & `pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfClone.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfCommand.py` & `pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfCommand.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfConvert.py` & `pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfConvert.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfDelete.py` & `pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfDelete.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfDryRun.py` & `pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfDryRun.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfEject.py` & `pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfEject.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfInstall.py` & `pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfInstall.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfMake.py` & `pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfMake.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfPackage.py` & `pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfPackage.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfQfs.py` & `pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfQfs.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.3/pfDevTools/pfCommand/pfReverse.py` & `pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfReverse.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.3/LICENSE` & `pf_dev_tools-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.3/README.md` & `pf_dev_tools-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.3/pyproject.toml` & `pf_dev_tools-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.3/PKG-INFO` & `pf_dev_tools-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pf-dev-tools
-Version: 1.0.3
+Version: 1.0.4
 Summary: A collection of tools for Project Freedom projects
 Project-URL: Homepage, https://didier.malenfant.net/ProjectFreedom/
 Project-URL: Documentation, https://github.com/DidierMalenfant/pfDevTools#readme
 Project-URL: Bug Tracker, https://github.com/DidierMalenfant/pfDevTools/issues
 Project-URL: Source Code, https://github.com/DidierMalenfant/pfDevTools
 Author-email: Didier Malenfant <coding@malenfant.net>
 License-Expression: GPL-3.0-or-later
```

