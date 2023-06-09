# Comparing `tmp/steam-pysigma-2023.6.3.tar.gz` & `tmp/steam-pysigma-2023.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\steam-pysigma-2023.6.3.tar", last modified: Mon Jun  5 09:31:51 2023, max compression
+gzip compressed data, was "dist\steam-pysigma-2023.6.4.tar", last modified: Fri Jun  9 08:42:11 2023, max compression
```

## Comparing `steam-pysigma-2023.6.3.tar` & `steam-pysigma-2023.6.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 09:31:51.734510 steam-pysigma-2023.6.3/
--rw-rw-rw-   0        0        0     1030 2023-06-05 09:31:51.734434 steam-pysigma-2023.6.3/PKG-INFO
--rw-rw-rw-   0        0        0      616 2023-02-22 13:16:40.000000 steam-pysigma-2023.6.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-05 09:31:51.734510 steam-pysigma-2023.6.3/setup.cfg
--rw-rw-rw-   0        0        0      897 2023-06-05 09:30:46.000000 steam-pysigma-2023.6.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:31:51.695944 steam-pysigma-2023.6.3/steam_pysigma/
--rw-rw-rw-   0        0        0     2861 2023-05-23 07:10:27.000000 steam-pysigma-2023.6.3/steam_pysigma/MainSIGMA.py
--rw-rw-rw-   0        0        0        0 2023-02-02 13:16:25.000000 steam-pysigma-2023.6.3/steam_pysigma/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:31:51.709087 steam-pysigma-2023.6.3/steam_pysigma/comsol/
--rw-rw-rw-   0        0        0    17427 2023-06-05 09:30:46.000000 steam-pysigma-2023.6.3/steam_pysigma/comsol/BuildComsolModel.py
--rw-rw-rw-   0        0        0    15166 2023-05-24 08:17:29.000000 steam-pysigma-2023.6.3/steam_pysigma/comsol/BuildGlobalVariables.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.3/steam_pysigma/comsol/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:31:51.713087 steam-pysigma-2023.6.3/steam_pysigma/data/
--rw-rw-rw-   0        0        0     8068 2023-05-25 12:15:47.000000 steam-pysigma-2023.6.3/steam_pysigma/data/DataRoxieParser.py
--rw-rw-rw-   0        0        0     7220 2023-06-01 09:48:39.000000 steam-pysigma-2023.6.3/steam_pysigma/data/DataSIGMA.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.3/steam_pysigma/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:31:51.717198 steam-pysigma-2023.6.3/steam_pysigma/domain_generator/
--rw-rw-rw-   0        0        0    17229 2023-05-25 12:09:39.000000 steam-pysigma-2023.6.3/steam_pysigma/domain_generator/GeometryMultipole.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.3/steam_pysigma/domain_generator/__init__.py
--rw-rw-rw-   0        0        0    12500 2023-04-21 07:21:40.000000 steam-pysigma-2023.6.3/steam_pysigma/helpers.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:31:51.720199 steam-pysigma-2023.6.3/steam_pysigma/parsers/
--rw-rw-rw-   0        0        0     1975 2023-05-25 12:04:31.000000 steam-pysigma-2023.6.3/steam_pysigma/parsers/ParserRoxie.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.3/steam_pysigma/parsers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:31:51.724328 steam-pysigma-2023.6.3/steam_pysigma/plotters/
--rw-rw-rw-   0        0        0    17437 2023-05-08 12:35:29.000000 steam-pysigma-2023.6.3/steam_pysigma/plotters/PlotterPysigma.py
--rw-rw-rw-   0        0        0     8879 2023-05-22 07:52:03.000000 steam-pysigma-2023.6.3/steam_pysigma/plotters/PlotterRoxie.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.3/steam_pysigma/plotters/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:31:51.727329 steam-pysigma-2023.6.3/steam_pysigma/postprocessing/
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.3/steam_pysigma/postprocessing/__init__.py
--rw-rw-rw-   0        0        0     3077 2023-05-08 12:18:35.000000 steam-pysigma-2023.6.3/steam_pysigma/postprocessing/postprocessing.py
--rw-rw-rw-   0        0        0    10147 2023-04-27 07:07:05.000000 steam-pysigma-2023.6.3/steam_pysigma/pysigma.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:31:51.732328 steam-pysigma-2023.6.3/steam_pysigma/utils/
--rw-rw-rw-   0        0        0     1945 2023-05-08 12:45:36.000000 steam-pysigma-2023.6.3/steam_pysigma/utils/Util.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.3/steam_pysigma/utils/__init__.py
--rw-rw-rw-   0        0        0      299 2022-11-02 10:29:42.000000 steam-pysigma-2023.6.3/steam_pysigma/utils/make_folder_if_not_existing.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:31:51.703944 steam-pysigma-2023.6.3/steam_pysigma.egg-info/
--rw-rw-rw-   0        0        0     1030 2023-06-05 09:31:47.000000 steam-pysigma-2023.6.3/steam_pysigma.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1005 2023-06-05 09:31:47.000000 steam-pysigma-2023.6.3/steam_pysigma.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 09:31:47.000000 steam-pysigma-2023.6.3/steam_pysigma.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      315 2023-06-05 09:31:47.000000 steam-pysigma-2023.6.3/steam_pysigma.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-05 09:31:47.000000 steam-pysigma-2023.6.3/steam_pysigma.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 08:42:11.635981 steam-pysigma-2023.6.4/
+-rw-rw-rw-   0        0        0     1030 2023-06-09 08:42:11.634982 steam-pysigma-2023.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0      616 2023-02-22 13:16:40.000000 steam-pysigma-2023.6.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-09 08:42:11.635981 steam-pysigma-2023.6.4/setup.cfg
+-rw-rw-rw-   0        0        0      897 2023-06-09 08:38:29.000000 steam-pysigma-2023.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 08:42:11.592982 steam-pysigma-2023.6.4/steam_pysigma/
+-rw-rw-rw-   0        0        0     2861 2023-05-23 07:10:27.000000 steam-pysigma-2023.6.4/steam_pysigma/MainSIGMA.py
+-rw-rw-rw-   0        0        0        0 2023-02-02 13:16:25.000000 steam-pysigma-2023.6.4/steam_pysigma/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 08:42:11.605982 steam-pysigma-2023.6.4/steam_pysigma/comsol/
+-rw-rw-rw-   0        0        0    17425 2023-06-09 08:39:51.000000 steam-pysigma-2023.6.4/steam_pysigma/comsol/BuildComsolModel.py
+-rw-rw-rw-   0        0        0    15166 2023-05-24 08:17:29.000000 steam-pysigma-2023.6.4/steam_pysigma/comsol/BuildGlobalVariables.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.4/steam_pysigma/comsol/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 08:42:11.610982 steam-pysigma-2023.6.4/steam_pysigma/data/
+-rw-rw-rw-   0        0        0     8068 2023-05-25 12:15:47.000000 steam-pysigma-2023.6.4/steam_pysigma/data/DataRoxieParser.py
+-rw-rw-rw-   0        0        0     7220 2023-06-01 09:48:39.000000 steam-pysigma-2023.6.4/steam_pysigma/data/DataSIGMA.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.4/steam_pysigma/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 08:42:11.613984 steam-pysigma-2023.6.4/steam_pysigma/domain_generator/
+-rw-rw-rw-   0        0        0    17563 2023-06-09 08:16:54.000000 steam-pysigma-2023.6.4/steam_pysigma/domain_generator/GeometryMultipole.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.4/steam_pysigma/domain_generator/__init__.py
+-rw-rw-rw-   0        0        0    12500 2023-04-21 07:21:40.000000 steam-pysigma-2023.6.4/steam_pysigma/helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-09 08:42:11.617982 steam-pysigma-2023.6.4/steam_pysigma/parsers/
+-rw-rw-rw-   0        0        0     1975 2023-05-25 12:04:31.000000 steam-pysigma-2023.6.4/steam_pysigma/parsers/ParserRoxie.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.4/steam_pysigma/parsers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 08:42:11.623982 steam-pysigma-2023.6.4/steam_pysigma/plotters/
+-rw-rw-rw-   0        0        0    17437 2023-05-08 12:35:29.000000 steam-pysigma-2023.6.4/steam_pysigma/plotters/PlotterPysigma.py
+-rw-rw-rw-   0        0        0     8879 2023-05-22 07:52:03.000000 steam-pysigma-2023.6.4/steam_pysigma/plotters/PlotterRoxie.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.4/steam_pysigma/plotters/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 08:42:11.626990 steam-pysigma-2023.6.4/steam_pysigma/postprocessing/
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.4/steam_pysigma/postprocessing/__init__.py
+-rw-rw-rw-   0        0        0     3077 2023-05-08 12:18:35.000000 steam-pysigma-2023.6.4/steam_pysigma/postprocessing/postprocessing.py
+-rw-rw-rw-   0        0        0    10147 2023-04-27 07:07:05.000000 steam-pysigma-2023.6.4/steam_pysigma/pysigma.py
+drwxrwxrwx   0        0        0        0 2023-06-09 08:42:11.631981 steam-pysigma-2023.6.4/steam_pysigma/utils/
+-rw-rw-rw-   0        0        0     1945 2023-05-08 12:45:36.000000 steam-pysigma-2023.6.4/steam_pysigma/utils/Util.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.4/steam_pysigma/utils/__init__.py
+-rw-rw-rw-   0        0        0      299 2022-11-02 10:29:42.000000 steam-pysigma-2023.6.4/steam_pysigma/utils/make_folder_if_not_existing.py
+drwxrwxrwx   0        0        0        0 2023-06-09 08:42:11.600982 steam-pysigma-2023.6.4/steam_pysigma.egg-info/
+-rw-rw-rw-   0        0        0     1030 2023-06-09 08:42:07.000000 steam-pysigma-2023.6.4/steam_pysigma.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1005 2023-06-09 08:42:07.000000 steam-pysigma-2023.6.4/steam_pysigma.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 08:42:07.000000 steam-pysigma-2023.6.4/steam_pysigma.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      315 2023-06-09 08:42:07.000000 steam-pysigma-2023.6.4/steam_pysigma.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-09 08:42:07.000000 steam-pysigma-2023.6.4/steam_pysigma.egg-info/top_level.txt
```

### Comparing `steam-pysigma-2023.6.3/PKG-INFO` & `steam-pysigma-2023.6.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-pysigma
-Version: 2023.6.3
+Version: 2023.6.4
 Summary: This is python wrapper of STEAM SIGMA code
 Home-page: https://gitlab.cern.ch/steam/steam_pysigma
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: SIGMA,CERN,STEAM
+Keywords: CERN,SIGMA,STEAM
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM PySIGMA
```

### Comparing `steam-pysigma-2023.6.3/README.md` & `steam-pysigma-2023.6.4/README.md`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.3/setup.py` & `steam-pysigma-2023.6.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='steam-pysigma',
-    version="2023.6.3",
+    version="2023.6.4",
     author="STEAM Team",
     author_email="steam-team@cern.ch",
     description="This is python wrapper of STEAM SIGMA code",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://gitlab.cern.ch/steam/steam_pysigma",
     keywords={'STEAM', 'SIGMA', 'CERN'},
```

### Comparing `steam-pysigma-2023.6.3/steam_pysigma/MainSIGMA.py` & `steam-pysigma-2023.6.4/steam_pysigma/MainSIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.3/steam_pysigma/comsol/BuildComsolModel.py` & `steam-pysigma-2023.6.4/steam_pysigma/comsol/BuildComsolModel.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,16 +65,16 @@
         self.time1DConverted = self.postprocessing_data.out_1D_vs_times.time
         self.variables1DvsTimeVector = self.postprocessing_data.out_1D_vs_times.variables
         self.timeRange = ", ".join(["range(" + ", ".join(map(str, lst)) + ")" for lst in
                                     self.model_data.options_sigma.time_vector_solution.time_step])
 
         print(f"Comsol compile path {self.COMSOL_compile_path}")
         print(f"Comsol version {self.COMSOL_version}")
-        #bgv = BuildGlobalVariables(self.g, self.model_data)
-        #bgv.validate_sigma_model_data()
+        bgv = BuildGlobalVariables(self.g, self.model_data)
+        bgv.validate_sigma_model_data()
         self.cfg = self.setup_config_sigma()
         self.srv = self.g.TxtSigmaServer(self.cfg.getOutputModelPath(), self.cfg.getComsolBatchPath(),
                                          self.cfg.getComsolCompilePath())
 
 
         geom_multipole = GeometryMultipole(self.g, self.roxie_data, model_data, self.bh_curve_database, self.input_conductor_params,
                                            self.settings_dict)
```

### Comparing `steam-pysigma-2023.6.3/steam_pysigma/comsol/BuildGlobalVariables.py` & `steam-pysigma-2023.6.4/steam_pysigma/comsol/BuildGlobalVariables.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.3/steam_pysigma/data/DataRoxieParser.py` & `steam-pysigma-2023.6.4/steam_pysigma/data/DataRoxieParser.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.3/steam_pysigma/data/DataSIGMA.py` & `steam-pysigma-2023.6.4/steam_pysigma/data/DataSIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.3/steam_pysigma/domain_generator/GeometryMultipole.py` & `steam-pysigma-2023.6.4/steam_pysigma/domain_generator/GeometryMultipole.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,17 +123,22 @@
         self.g.cable.setwInsulNarrow(self.cableParameters['cable']['th_insulation_along_height'])
         self.g.cable.setwInsulWide(self.cableParameters['cable']['th_insulation_along_width'])
         self.g.cable.setRc(self.cableParameters['cable']['Rc'])
         self.g.cable.setRa(self.cableParameters['cable']['Ra'])
         self.g.cable.setwBare(self.cableParameters['cable']['bare_cable_width'])
         self.g.cable.sethInBare(self.cableParameters['cable']['bare_cable_height_low'])
         self.g.cable.sethOutBare(self.cableParameters['cable']['bare_cable_height_high'])
-        self.g.cable.setNoOfStrands(self.cableParameters['cable']['n_strands'])
-        self.g.cable.setNoOfStrandsPerLayer(self.cableParameters['cable']['n_strands_per_layers'])
-        self.g.cable.setNoOfLayers(self.cableParameters['cable']['n_strand_layers'])
+        try: self.g.cable.setNoOfStrands(self.cableParameters['cable']['n_strands'])
+        except: print("WARNING! n_strands is set to null, will be set to 0 by default")
+        try: self.g.cable.setNoOfStrandsPerLayer(self.cableParameters['cable']['n_strands_per_layers'])
+        except: print("WARNING! n_strands_per_layers is set to null, will be set to 0 by default")
+        try:
+            self.g.cable.setNoOfStrandsPerLayer(self.cableParameters['cable']['n_strand_layers'])
+        except:
+            print("WARNING! n_strand_layers is set to null, will be set to 0 by default")
         self.g.cable.setlTpStrand(self.cableParameters['cable']['strand_twist_pitch'])
         self.g.cable.setwCore(self.cableParameters['cable']['width_core'])
         self.g.cable.sethCore(self.cableParameters['cable']['height_core'])
         self.g.cable.setThetaTpStrand(self.cableParameters['cable']['strand_twist_pitch_angle'])
         self.g.cable.setFracFillInnerVoids(self.cableParameters['cable']['f_inner_voids'])
         self.g.cable.setFractFillOuterVoids(self.cableParameters['cable']['f_outer_voids'])
```

### Comparing `steam-pysigma-2023.6.3/steam_pysigma/helpers.py` & `steam-pysigma-2023.6.4/steam_pysigma/helpers.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.3/steam_pysigma/parsers/ParserRoxie.py` & `steam-pysigma-2023.6.4/steam_pysigma/parsers/ParserRoxie.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.3/steam_pysigma/plotters/PlotterPysigma.py` & `steam-pysigma-2023.6.4/steam_pysigma/plotters/PlotterPysigma.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.3/steam_pysigma/plotters/PlotterRoxie.py` & `steam-pysigma-2023.6.4/steam_pysigma/plotters/PlotterRoxie.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.3/steam_pysigma/postprocessing/postprocessing.py` & `steam-pysigma-2023.6.4/steam_pysigma/postprocessing/postprocessing.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.3/steam_pysigma/pysigma.py` & `steam-pysigma-2023.6.4/steam_pysigma/pysigma.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.3/steam_pysigma/utils/Util.py` & `steam-pysigma-2023.6.4/steam_pysigma/utils/Util.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.3/steam_pysigma.egg-info/PKG-INFO` & `steam-pysigma-2023.6.4/steam_pysigma.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-pysigma
-Version: 2023.6.3
+Version: 2023.6.4
 Summary: This is python wrapper of STEAM SIGMA code
 Home-page: https://gitlab.cern.ch/steam/steam_pysigma
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: SIGMA,CERN,STEAM
+Keywords: CERN,SIGMA,STEAM
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM PySIGMA
```

### Comparing `steam-pysigma-2023.6.3/steam_pysigma.egg-info/SOURCES.txt` & `steam-pysigma-2023.6.4/steam_pysigma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

