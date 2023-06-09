# Comparing `tmp/architector-0.0.8.tar.gz` & `tmp/architector-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "architector-0.0.8.tar", last modified: Tue Jun  6 16:25:27 2023, max compression
+gzip compressed data, was "architector-0.0.9.tar", last modified: Fri Jun  9 06:37:08 2023, max compression
```

## Comparing `architector-0.0.8.tar` & `architector-0.0.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:25:27.165297 architector-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-06 16:25:23.000000 architector-0.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-06 16:25:23.000000 architector-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14542 2023-06-06 16:25:27.165297 architector-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14077 2023-06-06 16:25:23.000000 architector-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:25:27.165297 architector-0.0.8/architector/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-06 16:25:23.000000 architector-0.0.8/architector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 16:25:23.000000 architector-0.0.8/architector/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-06 16:25:27.165297 architector-0.0.8/architector/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-06 16:25:23.000000 architector-0.0.8/architector/arch_context_manage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-06-06 16:25:23.000000 architector-0.0.8/architector/ase_db_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    42356 2023-06-06 16:25:23.000000 architector-0.0.8/architector/complex_construction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:25:27.165297 architector-0.0.8/architector/data/
--rw-r--r--   0 runner    (1001) docker     (123) 27596793 2023-06-06 16:25:23.000000 architector-0.0.8/architector/data/angle_stats_datasource.csv
--rw-r--r--   0 runner    (1001) docker     (123)    18350 2023-06-06 16:25:23.000000 architector-0.0.8/architector/data/ligtype_angle_reference.csv
--rw-r--r--   0 runner    (1001) docker     (123)    13997 2023-06-06 16:25:23.000000 architector-0.0.8/architector/geometries.py
--rw-r--r--   0 runner    (1001) docker     (123)    20628 2023-06-06 16:25:23.000000 architector-0.0.8/architector/io_align_mol.py
--rw-r--r--   0 runner    (1001) docker     (123)    16875 2023-06-06 16:25:23.000000 architector-0.0.8/architector/io_calc.py
--rw-r--r--   0 runner    (1001) docker     (123)    18848 2023-06-06 16:25:23.000000 architector-0.0.8/architector/io_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    16427 2023-06-06 16:25:23.000000 architector-0.0.8/architector/io_crest.py
--rw-r--r--   0 runner    (1001) docker     (123)    79274 2023-06-06 16:25:23.000000 architector-0.0.8/architector/io_lig.py
--rw-r--r--   0 runner    (1001) docker     (123)    44449 2023-06-06 16:25:23.000000 architector-0.0.8/architector/io_molecule.py
--rw-r--r--   0 runner    (1001) docker     (123)    31158 2023-06-06 16:25:23.000000 architector-0.0.8/architector/io_obabel.py
--rw-r--r--   0 runner    (1001) docker     (123)    68735 2023-06-06 16:25:23.000000 architector-0.0.8/architector/io_process_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    39950 2023-06-06 16:25:23.000000 architector-0.0.8/architector/io_ptable.py
--rw-r--r--   0 runner    (1001) docker     (123)    14894 2023-06-06 16:25:23.000000 architector-0.0.8/architector/io_symmetry.py
--rw-r--r--   0 runner    (1001) docker     (123)    20602 2023-06-06 16:25:23.000000 architector-0.0.8/architector/io_xtb_calc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-06 16:25:23.000000 architector-0.0.8/architector/vibrations_free_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-06-06 16:25:23.000000 architector-0.0.8/architector/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:25:27.117297 architector-0.0.8/architector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14542 2023-06-06 16:25:27.000000 architector-0.0.8/architector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-06 16:25:27.000000 architector-0.0.8/architector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 16:25:27.000000 architector-0.0.8/architector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-06 16:25:27.000000 architector-0.0.8/architector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-06 16:25:27.000000 architector-0.0.8/architector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-06 16:25:27.165297 architector-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-06 16:25:23.000000 architector-0.0.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-06-06 16:25:23.000000 architector-0.0.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:37:08.830800 architector-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-09 06:37:03.000000 architector-0.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-09 06:37:03.000000 architector-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14542 2023-06-09 06:37:08.830800 architector-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14077 2023-06-09 06:37:03.000000 architector-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:37:08.830800 architector-0.0.9/architector/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-09 06:37:03.000000 architector-0.0.9/architector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 06:37:03.000000 architector-0.0.9/architector/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-09 06:37:08.834800 architector-0.0.9/architector/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-09 06:37:03.000000 architector-0.0.9/architector/arch_context_manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-06-09 06:37:03.000000 architector-0.0.9/architector/ase_db_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42356 2023-06-09 06:37:03.000000 architector-0.0.9/architector/complex_construction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:37:08.830800 architector-0.0.9/architector/data/
+-rw-r--r--   0 runner    (1001) docker     (123) 27596793 2023-06-09 06:37:03.000000 architector-0.0.9/architector/data/angle_stats_datasource.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    18350 2023-06-09 06:37:03.000000 architector-0.0.9/architector/data/ligtype_angle_reference.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13997 2023-06-09 06:37:03.000000 architector-0.0.9/architector/geometries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20628 2023-06-09 06:37:03.000000 architector-0.0.9/architector/io_align_mol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16875 2023-06-09 06:37:03.000000 architector-0.0.9/architector/io_calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18848 2023-06-09 06:37:03.000000 architector-0.0.9/architector/io_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16427 2023-06-09 06:37:03.000000 architector-0.0.9/architector/io_crest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79274 2023-06-09 06:37:03.000000 architector-0.0.9/architector/io_lig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44449 2023-06-09 06:37:03.000000 architector-0.0.9/architector/io_molecule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31158 2023-06-09 06:37:03.000000 architector-0.0.9/architector/io_obabel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68735 2023-06-09 06:37:03.000000 architector-0.0.9/architector/io_process_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39950 2023-06-09 06:37:03.000000 architector-0.0.9/architector/io_ptable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14894 2023-06-09 06:37:03.000000 architector-0.0.9/architector/io_symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20602 2023-06-09 06:37:03.000000 architector-0.0.9/architector/io_xtb_calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-09 06:37:03.000000 architector-0.0.9/architector/vibrations_free_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-06-09 06:37:03.000000 architector-0.0.9/architector/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:37:08.806800 architector-0.0.9/architector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14542 2023-06-09 06:37:08.000000 architector-0.0.9/architector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-09 06:37:08.000000 architector-0.0.9/architector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 06:37:08.000000 architector-0.0.9/architector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-09 06:37:08.000000 architector-0.0.9/architector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-09 06:37:08.000000 architector-0.0.9/architector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-09 06:37:08.830800 architector-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-09 06:37:03.000000 architector-0.0.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-06-09 06:37:03.000000 architector-0.0.9/versioneer.py
```

### Comparing `architector-0.0.8/LICENSE.txt` & `architector-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `architector-0.0.8/PKG-INFO` & `architector-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: architector
-Version: 0.0.8
+Version: 0.0.9
 Summary: The architector python package - for 3D inorganometallic complex design.
 Author: Michael G. Taylor et al.
 License: BSD 3-Clause License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Chemistry
```

### Comparing `architector-0.0.8/README.md` & `architector-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `architector-0.0.8/architector/arch_context_manage.py` & `architector-0.0.9/architector/arch_context_manage.py`

 * *Files identical despite different names*

### Comparing `architector-0.0.8/architector/ase_db_utilities.py` & `architector-0.0.9/architector/ase_db_utilities.py`

 * *Files identical despite different names*

### Comparing `architector-0.0.8/architector/complex_construction.py` & `architector-0.0.9/architector/complex_construction.py`

 * *Files identical despite different names*

### Comparing `architector-0.0.8/architector/data/angle_stats_datasource.csv` & `architector-0.0.9/architector/data/angle_stats_datasource.csv`

 * *Files identical despite different names*

### Comparing `architector-0.0.8/architector/data/ligtype_angle_reference.csv` & `architector-0.0.9/architector/data/ligtype_angle_reference.csv`

 * *Files identical despite different names*

### Comparing `architector-0.0.8/architector/geometries.py` & `architector-0.0.9/architector/geometries.py`

 * *Files identical despite different names*

### Comparing `architector-0.0.8/architector/io_align_mol.py` & `architector-0.0.9/architector/io_align_mol.py`

 * *Files identical despite different names*

### Comparing `architector-0.0.8/architector/io_calc.py` & `architector-0.0.9/architector/io_calc.py`

 * *Files identical despite different names*

### Comparing `architector-0.0.8/architector/io_core.py` & `architector-0.0.9/architector/io_core.py`

 * *Files identical despite different names*

### Comparing `architector-0.0.8/architector/io_crest.py` & `architector-0.0.9/architector/io_crest.py`

 * *Files identical despite different names*

### Comparing `architector-0.0.8/architector/io_lig.py` & `architector-0.0.9/architector/io_lig.py`

 * *Files identical despite different names*

### Comparing `architector-0.0.8/architector/io_molecule.py` & `architector-0.0.9/architector/io_molecule.py`

 * *Files identical despite different names*

### Comparing `architector-0.0.8/architector/io_obabel.py` & `architector-0.0.9/architector/io_obabel.py`

 * *Files identical despite different names*

### Comparing `architector-0.0.8/architector/io_process_input.py` & `architector-0.0.9/architector/io_process_input.py`

 * *Files identical despite different names*

### Comparing `architector-0.0.8/architector/io_ptable.py` & `architector-0.0.9/architector/io_ptable.py`

 * *Files identical despite different names*

### Comparing `architector-0.0.8/architector/io_symmetry.py` & `architector-0.0.9/architector/io_symmetry.py`

 * *Files identical despite different names*

### Comparing `architector-0.0.8/architector/io_xtb_calc.py` & `architector-0.0.9/architector/io_xtb_calc.py`

 * *Files identical despite different names*

### Comparing `architector-0.0.8/architector/vibrations_free_energy.py` & `architector-0.0.9/architector/vibrations_free_energy.py`

 * *Files identical despite different names*

### Comparing `architector-0.0.8/architector/visualization.py` & `architector-0.0.9/architector/visualization.py`

 * *Files identical despite different names*

### Comparing `architector-0.0.8/architector.egg-info/PKG-INFO` & `architector-0.0.9/architector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: architector
-Version: 0.0.8
+Version: 0.0.9
 Summary: The architector python package - for 3D inorganometallic complex design.
 Author: Michael G. Taylor et al.
 License: BSD 3-Clause License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Chemistry
```

### Comparing `architector-0.0.8/architector.egg-info/SOURCES.txt` & `architector-0.0.9/architector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `architector-0.0.8/setup.py` & `architector-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,16 +13,15 @@
     install_requires=[
         'ase',
         'numpy',
         'py3Dmol',
         'pynauty',
         'scipy',
         'pandas',
-        'mendeleev',
-        'sqlalchemy<2.0.0'
+        'mendeleev'
     ],
     license="BSD 3-Clause License",
     classifiers=["Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "Programming Language :: Python :: 3",
         "Topic :: Scientific/Engineering :: Chemistry"],
     description="The architector python package - for 3D inorganometallic complex design.",
```

### Comparing `architector-0.0.8/versioneer.py` & `architector-0.0.9/versioneer.py`

 * *Files identical despite different names*

