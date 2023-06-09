# Comparing `tmp/ilastik-napari-0.2.2.tar.gz` & `tmp/ilastik-napari-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ilastik-napari-0.2.2.tar", last modified: Tue Jun  6 13:05:43 2023, max compression
+gzip compressed data, was "ilastik-napari-0.2.3.tar", last modified: Fri Jun  9 11:12:54 2023, max compression
```

## Comparing `ilastik-napari-0.2.2.tar` & `ilastik-napari-0.2.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:05:43.250475 ilastik-napari-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-06 13:05:33.000000 ilastik-napari-0.2.2/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:05:43.246475 ilastik-napari-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:05:43.246475 ilastik-napari-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-06 13:05:33.000000 ilastik-napari-0.2.2/.github/workflows/build-upload.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-06 13:05:33.000000 ilastik-napari-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-06 13:05:33.000000 ilastik-napari-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-06-06 13:05:43.250475 ilastik-napari-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-06-06 13:05:33.000000 ilastik-napari-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:05:43.246475 ilastik-napari-0.2.2/conda-recipe/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-06 13:05:33.000000 ilastik-napari-0.2.2/conda-recipe/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:05:43.246475 ilastik-napari-0.2.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-06 13:05:33.000000 ilastik-napari-0.2.2/examples/simple_labeling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-06 13:05:33.000000 ilastik-napari-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 13:05:43.250475 ilastik-napari-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-06 13:05:33.000000 ilastik-napari-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:05:43.246475 ilastik-napari-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:05:43.246475 ilastik-napari-0.2.2/src/ilastik/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:05:43.250475 ilastik-napari-0.2.2/src/ilastik/napari/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-06 13:05:33.000000 ilastik-napari-0.2.2/src/ilastik/napari/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-06 13:05:33.000000 ilastik-napari-0.2.2/src/ilastik/napari/classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-06-06 13:05:33.000000 ilastik-napari-0.2.2/src/ilastik/napari/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-06 13:05:33.000000 ilastik-napari-0.2.2/src/ilastik/napari/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-06-06 13:05:33.000000 ilastik-napari-0.2.2/src/ilastik/napari/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-06 13:05:33.000000 ilastik-napari-0.2.2/src/ilastik/napari/plugin.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:05:43.250475 ilastik-napari-0.2.2/src/ilastik_napari.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-06-06 13:05:43.000000 ilastik-napari-0.2.2/src/ilastik_napari.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-06 13:05:43.000000 ilastik-napari-0.2.2/src/ilastik_napari.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 13:05:43.000000 ilastik-napari-0.2.2/src/ilastik_napari.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-06 13:05:43.000000 ilastik-napari-0.2.2/src/ilastik_napari.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-06 13:05:43.000000 ilastik-napari-0.2.2/src/ilastik_napari.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 13:05:43.000000 ilastik-napari-0.2.2/src/ilastik_napari.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:12:54.704064 ilastik-napari-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-09 11:12:43.000000 ilastik-napari-0.2.3/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:12:54.696064 ilastik-napari-0.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:12:54.700064 ilastik-napari-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-09 11:12:43.000000 ilastik-napari-0.2.3/.github/workflows/build-upload.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-09 11:12:43.000000 ilastik-napari-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-09 11:12:43.000000 ilastik-napari-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-06-09 11:12:54.700064 ilastik-napari-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-06-09 11:12:43.000000 ilastik-napari-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:12:54.700064 ilastik-napari-0.2.3/conda-recipe/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-09 11:12:43.000000 ilastik-napari-0.2.3/conda-recipe/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:12:54.700064 ilastik-napari-0.2.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-09 11:12:43.000000 ilastik-napari-0.2.3/examples/simple_labeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-09 11:12:43.000000 ilastik-napari-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 11:12:54.704064 ilastik-napari-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-09 11:12:43.000000 ilastik-napari-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:12:54.696064 ilastik-napari-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:12:54.696064 ilastik-napari-0.2.3/src/ilastik/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:12:54.700064 ilastik-napari-0.2.3/src/ilastik/napari/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-09 11:12:43.000000 ilastik-napari-0.2.3/src/ilastik/napari/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-09 11:12:43.000000 ilastik-napari-0.2.3/src/ilastik/napari/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-06-09 11:12:43.000000 ilastik-napari-0.2.3/src/ilastik/napari/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-09 11:12:43.000000 ilastik-napari-0.2.3/src/ilastik/napari/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-06-09 11:12:43.000000 ilastik-napari-0.2.3/src/ilastik/napari/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-09 11:12:43.000000 ilastik-napari-0.2.3/src/ilastik/napari/plugin.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:12:54.700064 ilastik-napari-0.2.3/src/ilastik_napari.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-06-09 11:12:54.000000 ilastik-napari-0.2.3/src/ilastik_napari.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-09 11:12:54.000000 ilastik-napari-0.2.3/src/ilastik_napari.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 11:12:54.000000 ilastik-napari-0.2.3/src/ilastik_napari.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-09 11:12:54.000000 ilastik-napari-0.2.3/src/ilastik_napari.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-09 11:12:54.000000 ilastik-napari-0.2.3/src/ilastik_napari.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-09 11:12:54.000000 ilastik-napari-0.2.3/src/ilastik_napari.egg-info/top_level.txt
```

### Comparing `ilastik-napari-0.2.2/.github/workflows/build-upload.yaml` & `ilastik-napari-0.2.3/.github/workflows/build-upload.yaml`

 * *Files identical despite different names*

### Comparing `ilastik-napari-0.2.2/LICENSE` & `ilastik-napari-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ilastik-napari-0.2.2/PKG-INFO` & `ilastik-napari-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ilastik-napari
-Version: 0.2.2
+Version: 0.2.3
 Summary: ilastik plugin for napari
 Author-email: Emil Melnikov <emilmelnikov@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/ilastik/ilastik-napari
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: End Users/Desktop
@@ -33,26 +33,30 @@
 ## Installation
 
 This plugin requires you to use a _conda_ environment. The environment manager conda comes in a few different forms.
 If you haven't used conda before, you can find more information in the [conda user guide][conda-user-guide].
 You can use whichever variant you prefer, as the resulting environment should be the same, but we recommend the [_mambaforge_][mambaforge] variant as it is usually the fastest.
 When using mambaforge, the `mamba` command usually replaces the `conda` command one would otherwise use.
 
-Once you have installed mambaforge, set up a conda environment with the _fastfilters_ package, and then use pip to install _ilastik-napari_:
+Once you have installed mambaforge, set up a conda environment with napari and the _fastfilters_ package, and then use pip to install _ilastik-napari_:
 ```shell
-mamba create -y -c ilastik-forge -c conda-forge -n my-napari-env fastfilters
+mamba create -y -c ilastik-forge -c conda-forge -n my-napari-env napari fastfilters
 mamba activate my-napari-env
 pip install ilastik-napari
 ```
 
 Finally, run napari:
 ```shell
 napari
 ```
-You should be able to find the ilastik-napari plugin in the Plugins menu.
+That's it! You should be able to find the ilastik-napari plugin in the Plugins menu.
+
+If you prefer to __install napari using pip__ instead of conda:
+Make sure to install `napari[all]`.
+Unless you want to [choose a PyQt implementation other than _PyQt5_][napari-pyqt], in which case you should leave out the `[all]` extra.
 
 ## Usage
 
 As a prerequisite, make sure you understand the [napari basics][napari-quickstart].
 
 1. Open your image, or use a sample in _File - Open Sample_.
 
@@ -116,7 +120,8 @@
 
 [napari]: https://napari.org/
 [ilastik]: https://www.ilastik.org/
 [conda-user-guide]: https://docs.conda.io/projects/conda/en/latest/user-guide/index.html
 [miniconda]: https://docs.conda.io/en/latest/miniconda.html
 [mambaforge]: https://github.com/conda-forge/miniforge#mambaforge
 [napari-quickstart]: https://napari.org/tutorials/fundamentals/quick_start.html
+[napari-pyqt]: https://napari.org/stable/plugins/best_practices.html#don-t-include-pyside2-or-pyqt5-in-your-plugin-s-dependencies
```

### Comparing `ilastik-napari-0.2.2/README.md` & `ilastik-napari-0.2.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -6,26 +6,30 @@
 ## Installation
 
 This plugin requires you to use a _conda_ environment. The environment manager conda comes in a few different forms.
 If you haven't used conda before, you can find more information in the [conda user guide][conda-user-guide].
 You can use whichever variant you prefer, as the resulting environment should be the same, but we recommend the [_mambaforge_][mambaforge] variant as it is usually the fastest.
 When using mambaforge, the `mamba` command usually replaces the `conda` command one would otherwise use.
 
-Once you have installed mambaforge, set up a conda environment with the _fastfilters_ package, and then use pip to install _ilastik-napari_:
+Once you have installed mambaforge, set up a conda environment with napari and the _fastfilters_ package, and then use pip to install _ilastik-napari_:
 ```shell
-mamba create -y -c ilastik-forge -c conda-forge -n my-napari-env fastfilters
+mamba create -y -c ilastik-forge -c conda-forge -n my-napari-env napari fastfilters
 mamba activate my-napari-env
 pip install ilastik-napari
 ```
 
 Finally, run napari:
 ```shell
 napari
 ```
-You should be able to find the ilastik-napari plugin in the Plugins menu.
+That's it! You should be able to find the ilastik-napari plugin in the Plugins menu.
+
+If you prefer to __install napari using pip__ instead of conda:
+Make sure to install `napari[all]`.
+Unless you want to [choose a PyQt implementation other than _PyQt5_][napari-pyqt], in which case you should leave out the `[all]` extra.
 
 ## Usage
 
 As a prerequisite, make sure you understand the [napari basics][napari-quickstart].
 
 1. Open your image, or use a sample in _File - Open Sample_.
 
@@ -89,7 +93,8 @@
 
 [napari]: https://napari.org/
 [ilastik]: https://www.ilastik.org/
 [conda-user-guide]: https://docs.conda.io/projects/conda/en/latest/user-guide/index.html
 [miniconda]: https://docs.conda.io/en/latest/miniconda.html
 [mambaforge]: https://github.com/conda-forge/miniforge#mambaforge
 [napari-quickstart]: https://napari.org/tutorials/fundamentals/quick_start.html
+[napari-pyqt]: https://napari.org/stable/plugins/best_practices.html#don-t-include-pyside2-or-pyqt5-in-your-plugin-s-dependencies
```

### Comparing `ilastik-napari-0.2.2/conda-recipe/meta.yaml` & `ilastik-napari-0.2.3/conda-recipe/meta.yaml`

 * *Files identical despite different names*

### Comparing `ilastik-napari-0.2.2/examples/simple_labeling.py` & `ilastik-napari-0.2.3/examples/simple_labeling.py`

 * *Files identical despite different names*

### Comparing `ilastik-napari-0.2.2/pyproject.toml` & `ilastik-napari-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ilastik-napari-0.2.2/src/ilastik/napari/classifier.py` & `ilastik-napari-0.2.3/src/ilastik/napari/classifier.py`

 * *Files identical despite different names*

### Comparing `ilastik-napari-0.2.2/src/ilastik/napari/filters.py` & `ilastik-napari-0.2.3/src/ilastik/napari/filters.py`

 * *Files identical despite different names*

### Comparing `ilastik-napari-0.2.2/src/ilastik/napari/gui.py` & `ilastik-napari-0.2.3/src/ilastik/napari/gui.py`

 * *Files identical despite different names*

### Comparing `ilastik-napari-0.2.2/src/ilastik/napari/plugin.py` & `ilastik-napari-0.2.3/src/ilastik/napari/plugin.py`

 * *Files identical despite different names*

### Comparing `ilastik-napari-0.2.2/src/ilastik_napari.egg-info/PKG-INFO` & `ilastik-napari-0.2.3/src/ilastik_napari.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ilastik-napari
-Version: 0.2.2
+Version: 0.2.3
 Summary: ilastik plugin for napari
 Author-email: Emil Melnikov <emilmelnikov@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/ilastik/ilastik-napari
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: End Users/Desktop
@@ -33,26 +33,30 @@
 ## Installation
 
 This plugin requires you to use a _conda_ environment. The environment manager conda comes in a few different forms.
 If you haven't used conda before, you can find more information in the [conda user guide][conda-user-guide].
 You can use whichever variant you prefer, as the resulting environment should be the same, but we recommend the [_mambaforge_][mambaforge] variant as it is usually the fastest.
 When using mambaforge, the `mamba` command usually replaces the `conda` command one would otherwise use.
 
-Once you have installed mambaforge, set up a conda environment with the _fastfilters_ package, and then use pip to install _ilastik-napari_:
+Once you have installed mambaforge, set up a conda environment with napari and the _fastfilters_ package, and then use pip to install _ilastik-napari_:
 ```shell
-mamba create -y -c ilastik-forge -c conda-forge -n my-napari-env fastfilters
+mamba create -y -c ilastik-forge -c conda-forge -n my-napari-env napari fastfilters
 mamba activate my-napari-env
 pip install ilastik-napari
 ```
 
 Finally, run napari:
 ```shell
 napari
 ```
-You should be able to find the ilastik-napari plugin in the Plugins menu.
+That's it! You should be able to find the ilastik-napari plugin in the Plugins menu.
+
+If you prefer to __install napari using pip__ instead of conda:
+Make sure to install `napari[all]`.
+Unless you want to [choose a PyQt implementation other than _PyQt5_][napari-pyqt], in which case you should leave out the `[all]` extra.
 
 ## Usage
 
 As a prerequisite, make sure you understand the [napari basics][napari-quickstart].
 
 1. Open your image, or use a sample in _File - Open Sample_.
 
@@ -116,7 +120,8 @@
 
 [napari]: https://napari.org/
 [ilastik]: https://www.ilastik.org/
 [conda-user-guide]: https://docs.conda.io/projects/conda/en/latest/user-guide/index.html
 [miniconda]: https://docs.conda.io/en/latest/miniconda.html
 [mambaforge]: https://github.com/conda-forge/miniforge#mambaforge
 [napari-quickstart]: https://napari.org/tutorials/fundamentals/quick_start.html
+[napari-pyqt]: https://napari.org/stable/plugins/best_practices.html#don-t-include-pyside2-or-pyqt5-in-your-plugin-s-dependencies
```

### Comparing `ilastik-napari-0.2.2/src/ilastik_napari.egg-info/SOURCES.txt` & `ilastik-napari-0.2.3/src/ilastik_napari.egg-info/SOURCES.txt`

 * *Files identical despite different names*

