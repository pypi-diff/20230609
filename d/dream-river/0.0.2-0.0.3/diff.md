# Comparing `tmp/dream_river-0.0.2.tar.gz` & `tmp/dream_river-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dream_river-0.0.2.tar", last modified: Fri Jun  9 08:15:09 2023, max compression
+gzip compressed data, was "dream_river-0.0.3.tar", last modified: Fri Jun  9 08:31:03 2023, max compression
```

## Comparing `dream_river-0.0.2.tar` & `dream_river-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 08:15:09.006663 dream_river-0.0.2/
--rw-rw-rw-   0        0        0     1069 2023-06-09 04:31:46.000000 dream_river-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1090 2023-06-09 04:31:50.000000 dream_river-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     1413 2023-06-09 08:15:09.007663 dream_river-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      866 2023-06-09 08:10:52.000000 dream_river-0.0.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-09 08:15:08.978662 dream_river-0.0.2/dream_river/
--rw-rw-rw-   0        0        0     7671 2023-06-09 02:24:47.000000 dream_river-0.0.2/dream_river/ML.py
--rw-rw-rw-   0        0        0      226 2023-06-09 04:57:22.000000 dream_river-0.0.2/dream_river/__init__.py
--rw-rw-rw-   0        0        0     7139 2023-06-09 02:19:03.000000 dream_river-0.0.2/dream_river/convertools.py
--rw-rw-rw-   0        0        0     4967 2023-06-09 04:20:55.000000 dream_river-0.0.2/dream_river/geobox.py
--rw-rw-rw-   0        0        0     7648 2023-06-09 02:19:27.000000 dream_river-0.0.2/dream_river/indices.py
--rw-rw-rw-   0        0        0    15124 2023-06-09 04:21:55.000000 dream_river-0.0.2/dream_river/plotimg.py
-drwxrwxrwx   0        0        0        0 2023-06-09 08:15:09.003661 dream_river-0.0.2/dream_river.egg-info/
--rw-rw-rw-   0        0        0     1413 2023-06-09 08:15:08.000000 dream_river-0.0.2/dream_river.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-06-09 08:15:08.000000 dream_river-0.0.2/dream_river.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 08:15:08.000000 dream_river-0.0.2/dream_river.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      158 2023-06-09 08:15:08.000000 dream_river-0.0.2/dream_river.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-09 08:15:08.000000 dream_river-0.0.2/dream_river.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-09 08:15:09.010664 dream_river-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1810 2023-06-09 08:14:16.000000 dream_river-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 08:31:03.279384 dream_river-0.0.3/
+-rw-rw-rw-   0        0        0     1069 2023-06-09 04:31:46.000000 dream_river-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1090 2023-06-09 04:31:50.000000 dream_river-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     1413 2023-06-09 08:31:03.280383 dream_river-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      866 2023-06-09 08:10:52.000000 dream_river-0.0.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-09 08:31:03.249381 dream_river-0.0.3/dream_river/
+-rw-rw-rw-   0        0        0     7586 2023-06-09 08:30:13.000000 dream_river-0.0.3/dream_river/ML.py
+-rw-rw-rw-   0        0        0      226 2023-06-09 04:57:22.000000 dream_river-0.0.3/dream_river/__init__.py
+-rw-rw-rw-   0        0        0     7139 2023-06-09 02:19:03.000000 dream_river-0.0.3/dream_river/convertools.py
+-rw-rw-rw-   0        0        0     4967 2023-06-09 04:20:55.000000 dream_river-0.0.3/dream_river/geobox.py
+-rw-rw-rw-   0        0        0     7648 2023-06-09 08:30:08.000000 dream_river-0.0.3/dream_river/indices.py
+-rw-rw-rw-   0        0        0    15124 2023-06-09 04:21:55.000000 dream_river-0.0.3/dream_river/plotimg.py
+drwxrwxrwx   0        0        0        0 2023-06-09 08:31:03.278383 dream_river-0.0.3/dream_river.egg-info/
+-rw-rw-rw-   0        0        0     1413 2023-06-09 08:31:03.000000 dream_river-0.0.3/dream_river.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-06-09 08:31:03.000000 dream_river-0.0.3/dream_river.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 08:31:03.000000 dream_river-0.0.3/dream_river.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      147 2023-06-09 08:31:03.000000 dream_river-0.0.3/dream_river.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-09 08:31:03.000000 dream_river-0.0.3/dream_river.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-09 08:31:03.282383 dream_river-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1797 2023-06-09 08:30:29.000000 dream_river-0.0.3/setup.py
```

### Comparing `dream_river-0.0.2/LICENSE` & `dream_river-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dream_river-0.0.2/LICENSE.txt` & `dream_river-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dream_river-0.0.2/PKG-INFO` & `dream_river-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dream_river
-Version: 0.0.2
+Version: 0.0.3
 Summary: This is a library contained rice detection tools and other geospatial tools for jupyter environment on sphere.gistda.or.th in part of Data Cube
 Home-page: https://github.com/Pathakorn40/rice-detection
 Author: Pathakorn Usaha
 Author-email: dreamusaha@gmail.com
 License: MIT
 Download-URL: https://pypi.org/project/dream_river/
 Keywords: geography,geospatiol,gis,rice detection
```

### Comparing `dream_river-0.0.2/README.rst` & `dream_river-0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `dream_river-0.0.2/dream_river/ML.py` & `dream_river-0.0.3/dream_river/ML.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,19 +9,18 @@
 import geopandas as gpd
 import matplotlib.pyplot as plt
 from io import StringIO
 from odc.io.cgroups import get_cpu_quota
 from sklearn.ensemble import RandomForestClassifier
 from sklearn import model_selection
 from sklearn.metrics import accuracy_score
-from IPython.display import Image
 from datacube.utils import geometry
 from datacube.utils.cog import write_cog
 from dea_tools.classification import collect_training_data, predict_xr
-from dea_tools.bandindices import calculate_indices
+
 from convertools import vectorize
 import warnings
 warnings.filterwarnings("ignore")
 
 def custom_loadband(query):
 
     # Initialise datacube
```

### Comparing `dream_river-0.0.2/dream_river/convertools.py` & `dream_river-0.0.3/dream_river/convertools.py`

 * *Files identical despite different names*

### Comparing `dream_river-0.0.2/dream_river/geobox.py` & `dream_river-0.0.3/dream_river/geobox.py`

 * *Files identical despite different names*

### Comparing `dream_river-0.0.2/dream_river/indices.py` & `dream_river-0.0.3/dream_river/indices.py`

 * *Files identical despite different names*

### Comparing `dream_river-0.0.2/dream_river/plotimg.py` & `dream_river-0.0.3/dream_river/plotimg.py`

 * *Files identical despite different names*

### Comparing `dream_river-0.0.2/dream_river.egg-info/PKG-INFO` & `dream_river-0.0.3/dream_river.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dream-river
-Version: 0.0.2
+Version: 0.0.3
 Summary: This is a library contained rice detection tools and other geospatial tools for jupyter environment on sphere.gistda.or.th in part of Data Cube
 Home-page: https://github.com/Pathakorn40/rice-detection
 Author: Pathakorn Usaha
 Author-email: dreamusaha@gmail.com
 License: MIT
 Download-URL: https://pypi.org/project/dream_river/
 Keywords: geography,geospatiol,gis,rice detection
```

### Comparing `dream_river-0.0.2/setup.py` & `dream_river-0.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup, find_packages
 
 DESC ='This is a library that contain rice cultivated area detection tools and other geospatial tools for jupyter environment on https://sphere.gistda.or.th/ in part of Data Cube. Thus, you needs go to sphere.gistda (https://sphere.gistda.or.th/) and register the account to access jupyter lab environment interactively from a browser.'
 
 setup(
     name='dream_river',
     packages=['dream_river'],
-    version='0.0.2',
+    version='0.0.3',
     license='MIT',
     author_email='dreamusaha@gmail.com',
     description= 'This is a library contained rice detection tools and other geospatial tools for jupyter environment on sphere.gistda.or.th in part of Data Cube',
     long_description= DESC,
     author='Pathakorn Usaha',
     url= 'https://github.com/Pathakorn40/rice-detection',
     download_url= 'https://pypi.org/project/dream_river/',
     keywords= ['geography','geospatiol','gis', 'rice detection'],
     install_requires= ['datacube','shapely','xarray','matplotlib','numpy','geopandas','dea_tools','sklearn',
-                'pydotplus','subprocess','odc','flusstools','skimage','gdal','scipy','math','folium','json','odc.ui','os','odc.io'],
+                'pydotplus','odc','flusstools','skimage','gdal','scipy','math','folium','json','odc.ui','os','odc.io'],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Science/Research',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',  
         'Programming Language :: Python :: 3',      #Specify which pyhton versions that you want to support
         'Programming Language :: Python :: 3.4',
```

