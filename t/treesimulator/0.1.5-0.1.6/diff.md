# Comparing `tmp/treesimulator-0.1.5.tar.gz` & `tmp/treesimulator-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "treesimulator-0.1.5.tar", last modified: Tue May 23 12:48:08 2023, max compression
+gzip compressed data, was "treesimulator-0.1.6.tar", last modified: Fri Jun  9 10:43:30 2023, max compression
```

## Comparing `treesimulator-0.1.5.tar` & `treesimulator-0.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        0 2023-05-23 12:48:08.502782 treesimulator-0.1.5/
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)    35823 2022-12-22 13:30:01.000000 treesimulator-0.1.5/LICENSE
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)     6340 2023-05-23 12:48:08.502782 treesimulator-0.1.5/PKG-INFO
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     5793 2022-12-22 13:30:01.000000 treesimulator-0.1.5/README.md
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)       38 2023-05-23 12:48:08.502782 treesimulator-0.1.5/setup.cfg
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     1302 2023-05-23 12:38:30.000000 treesimulator-0.1.5/setup.py
-drwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        0 2023-05-23 12:48:08.502782 treesimulator-0.1.5/treesimulator/
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)     1281 2023-05-23 12:45:26.000000 treesimulator-0.1.5/treesimulator/__init__.py
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)    17829 2023-05-23 12:47:02.000000 treesimulator-0.1.5/treesimulator/generator.py
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)    10186 2023-05-23 12:38:06.000000 treesimulator-0.1.5/treesimulator/mtbd_models.py
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     4537 2022-12-22 13:30:02.000000 treesimulator-0.1.5/treesimulator/sequence_generator.py
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     5466 2022-12-22 13:30:02.000000 treesimulator-0.1.5/treesimulator/simulate_forest.py
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     3883 2022-12-22 13:30:02.000000 treesimulator-0.1.5/treesimulator/simulate_forest_bd.py
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     4069 2022-12-22 13:30:02.000000 treesimulator-0.1.5/treesimulator/simulate_forest_bdei.py
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     4582 2022-12-22 13:30:02.000000 treesimulator-0.1.5/treesimulator/simulate_forest_bdss.py
-drwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        0 2023-05-23 12:48:08.502782 treesimulator-0.1.5/treesimulator.egg-info/
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     6340 2023-05-23 12:48:08.000000 treesimulator-0.1.5/treesimulator.egg-info/PKG-INFO
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)      513 2023-05-23 12:48:08.000000 treesimulator-0.1.5/treesimulator.egg-info/SOURCES.txt
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        1 2023-05-23 12:48:08.000000 treesimulator-0.1.5/treesimulator.egg-info/dependency_links.txt
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)      233 2023-05-23 12:48:08.000000 treesimulator-0.1.5/treesimulator.egg-info/entry_points.txt
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)       15 2023-05-23 12:48:08.000000 treesimulator-0.1.5/treesimulator.egg-info/requires.txt
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)       14 2023-05-23 12:48:08.000000 treesimulator-0.1.5/treesimulator.egg-info/top_level.txt
+drwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        0 2023-06-09 10:43:30.327995 treesimulator-0.1.6/
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)    35823 2022-12-22 13:30:01.000000 treesimulator-0.1.6/LICENSE
+-rw-rw-r--   0 azhukova  (1000) azhukova  (1000)     6340 2023-06-09 10:43:30.327995 treesimulator-0.1.6/PKG-INFO
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     5793 2022-12-22 13:30:01.000000 treesimulator-0.1.6/README.md
+-rw-rw-r--   0 azhukova  (1000) azhukova  (1000)       38 2023-06-09 10:43:30.327995 treesimulator-0.1.6/setup.cfg
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     1302 2023-06-09 10:42:39.000000 treesimulator-0.1.6/setup.py
+drwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        0 2023-06-09 10:43:30.327995 treesimulator-0.1.6/treesimulator/
+-rw-rw-r--   0 azhukova  (1000) azhukova  (1000)     1281 2023-05-23 12:45:26.000000 treesimulator-0.1.6/treesimulator/__init__.py
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)    17829 2023-05-23 12:47:02.000000 treesimulator-0.1.6/treesimulator/generator.py
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)    10186 2023-05-23 12:38:06.000000 treesimulator-0.1.6/treesimulator/mtbd_models.py
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     4537 2022-12-22 13:30:02.000000 treesimulator-0.1.6/treesimulator/sequence_generator.py
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     5459 2023-06-09 10:42:39.000000 treesimulator-0.1.6/treesimulator/simulate_forest.py
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     3883 2022-12-22 13:30:02.000000 treesimulator-0.1.6/treesimulator/simulate_forest_bd.py
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     4069 2022-12-22 13:30:02.000000 treesimulator-0.1.6/treesimulator/simulate_forest_bdei.py
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     4582 2022-12-22 13:30:02.000000 treesimulator-0.1.6/treesimulator/simulate_forest_bdss.py
+drwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        0 2023-06-09 10:43:30.327995 treesimulator-0.1.6/treesimulator.egg-info/
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     6340 2023-06-09 10:43:30.000000 treesimulator-0.1.6/treesimulator.egg-info/PKG-INFO
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)      513 2023-06-09 10:43:30.000000 treesimulator-0.1.6/treesimulator.egg-info/SOURCES.txt
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        1 2023-06-09 10:43:30.000000 treesimulator-0.1.6/treesimulator.egg-info/dependency_links.txt
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)      233 2023-06-09 10:43:30.000000 treesimulator-0.1.6/treesimulator.egg-info/entry_points.txt
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)       15 2023-06-09 10:43:30.000000 treesimulator-0.1.6/treesimulator.egg-info/requires.txt
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)       14 2023-06-09 10:43:30.000000 treesimulator-0.1.6/treesimulator.egg-info/top_level.txt
```

### Comparing `treesimulator-0.1.5/LICENSE` & `treesimulator-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `treesimulator-0.1.5/PKG-INFO` & `treesimulator-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treesimulator
-Version: 0.1.5
+Version: 0.1.6
 Summary: Simulation of rooted phylogenetic trees under a given Multitype Birth–Death model.
 Home-page: https://github.com/evolbioinfo/treesimulator
 Author: Anna Zhukova
 Author-email: anna.zhukova@pasteur.fr
 Keywords: phylogenetics,tree generator,multitype birth-death model
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `treesimulator-0.1.5/README.md` & `treesimulator-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `treesimulator-0.1.5/setup.py` & `treesimulator-0.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         'Development Status :: 4 - Beta',
         'Environment :: Console',
         'Intended Audience :: Developers',
         'Topic :: Scientific/Engineering :: Bio-Informatics',
         'Topic :: Software Development',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
-    version='0.1.5',
+    version='0.1.6',
     description='Simulation of rooted phylogenetic trees under a given Multitype Birth–Death model.',
     author='Anna Zhukova',
     author_email='anna.zhukova@pasteur.fr',
     url='https://github.com/evolbioinfo/treesimulator',
     keywords=['phylogenetics', 'tree generator', 'multitype birth-death model'],
     install_requires=['six', 'ete3', 'numpy'],
     entry_points={
```

### Comparing `treesimulator-0.1.5/treesimulator/__init__.py` & `treesimulator-0.1.6/treesimulator/__init__.py`

 * *Files identical despite different names*

### Comparing `treesimulator-0.1.5/treesimulator/generator.py` & `treesimulator-0.1.6/treesimulator/generator.py`

 * *Files identical despite different names*

### Comparing `treesimulator-0.1.5/treesimulator/mtbd_models.py` & `treesimulator-0.1.6/treesimulator/mtbd_models.py`

 * *Files identical despite different names*

### Comparing `treesimulator-0.1.5/treesimulator/sequence_generator.py` & `treesimulator-0.1.6/treesimulator/sequence_generator.py`

 * *Files identical despite different names*

### Comparing `treesimulator-0.1.5/treesimulator/simulate_forest.py` & `treesimulator-0.1.6/treesimulator/simulate_forest.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,21 +64,21 @@
     transition_rates = np.array(params.transition_rates).reshape((n_states, n_states))
     transmission_rates = np.array(params.transmission_rates).reshape((n_states, n_states))
 
     logging.info(
         'MTBD model parameters are:\n'
         '\ttransition_rates=\n{}\n'
         '\ttransmission_rates=\n{}\n'
-        '\ttransmission_rates={}\n'
+        '\tremoval_rates={}\n'
         '\tps={}'.format(transition_rates, transmission_rates, params.removal_rates, params.sampling_probabilities))
     logging.info('Total time T={}'.format(params.T))
 
     model = Model(states=params.states,
                   transmission_rates=transition_rates,
-                  transition_rates=transmission_rates,
+                  transition_rates=transition_rates,
                   removal_rates=params.removal_rates, ps=params.sampling_probabilities)
     if params.pn and params.pn > 0:
         model = PNModel(model=model, pn=params.pn, removal_rate=params.partner_psi)
 
     forest, (total_tips, u, T), ltt = generate(model, params.min_tips, params.max_tips, T=params.T)
 
     save_forest(forest, params.nwk)
```

### Comparing `treesimulator-0.1.5/treesimulator/simulate_forest_bd.py` & `treesimulator-0.1.6/treesimulator/simulate_forest_bd.py`

 * *Files identical despite different names*

### Comparing `treesimulator-0.1.5/treesimulator/simulate_forest_bdei.py` & `treesimulator-0.1.6/treesimulator/simulate_forest_bdei.py`

 * *Files identical despite different names*

### Comparing `treesimulator-0.1.5/treesimulator/simulate_forest_bdss.py` & `treesimulator-0.1.6/treesimulator/simulate_forest_bdss.py`

 * *Files identical despite different names*

### Comparing `treesimulator-0.1.5/treesimulator.egg-info/PKG-INFO` & `treesimulator-0.1.6/treesimulator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treesimulator
-Version: 0.1.5
+Version: 0.1.6
 Summary: Simulation of rooted phylogenetic trees under a given Multitype Birth–Death model.
 Home-page: https://github.com/evolbioinfo/treesimulator
 Author: Anna Zhukova
 Author-email: anna.zhukova@pasteur.fr
 Keywords: phylogenetics,tree generator,multitype birth-death model
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `treesimulator-0.1.5/treesimulator.egg-info/SOURCES.txt` & `treesimulator-0.1.6/treesimulator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

