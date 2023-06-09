# Comparing `tmp/pytorch_speech_features-0.0.1.tar.gz` & `tmp/pytorch_speech_features-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch_speech_features-0.0.1.tar", last modified: Fri Jun  9 16:38:00 2023, max compression
+gzip compressed data, was "pytorch_speech_features-0.0.2.tar", last modified: Fri Jun  9 18:32:24 2023, max compression
```

## Comparing `pytorch_speech_features-0.0.1.tar` & `pytorch_speech_features-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 debjoy    (1000) debjoy    (1000)        0 2023-06-09 16:38:00.193040 pytorch_speech_features-0.0.1/
--rwxrwxrwx   0 debjoy    (1000) debjoy    (1000)     1068 2023-05-17 04:17:30.000000 pytorch_speech_features-0.0.1/LICENSE
--rwxrwxrwx   0 debjoy    (1000) debjoy    (1000)      265 2023-06-09 16:38:00.194042 pytorch_speech_features-0.0.1/PKG-INFO
--rwxrwxrwx   0 debjoy    (1000) debjoy    (1000)     1533 2023-06-09 15:55:38.000000 pytorch_speech_features-0.0.1/README.md
--rwxrwxrwx   0 debjoy    (1000) debjoy    (1000)     1715 2023-06-09 16:18:48.000000 pytorch_speech_features-0.0.1/README.rst
-drwxrwxrwx   0 debjoy    (1000) debjoy    (1000)        0 2023-06-09 16:38:00.036906 pytorch_speech_features-0.0.1/pytorch_speech_features/
--rwxrwxrwx   0 debjoy    (1000) debjoy    (1000)       19 2023-05-17 04:17:30.000000 pytorch_speech_features-0.0.1/pytorch_speech_features/__init__.py
--rwxrwxrwx   0 debjoy    (1000) debjoy    (1000)    13000 2023-06-09 14:07:54.000000 pytorch_speech_features-0.0.1/pytorch_speech_features/base.py
--rwxrwxrwx   0 debjoy    (1000) debjoy    (1000)     6292 2023-06-09 14:07:59.000000 pytorch_speech_features-0.0.1/pytorch_speech_features/sigproc.py
-drwxrwxrwx   0 debjoy    (1000) debjoy    (1000)        0 2023-06-09 16:38:00.166057 pytorch_speech_features-0.0.1/pytorch_speech_features.egg-info/
--rwxrwxrwx   0 debjoy    (1000) debjoy    (1000)      265 2023-06-09 16:37:59.000000 pytorch_speech_features-0.0.1/pytorch_speech_features.egg-info/PKG-INFO
--rwxrwxrwx   0 debjoy    (1000) debjoy    (1000)      384 2023-06-09 16:37:59.000000 pytorch_speech_features-0.0.1/pytorch_speech_features.egg-info/SOURCES.txt
--rwxrwxrwx   0 debjoy    (1000) debjoy    (1000)        1 2023-06-09 16:37:59.000000 pytorch_speech_features-0.0.1/pytorch_speech_features.egg-info/dependency_links.txt
--rwxrwxrwx   0 debjoy    (1000) debjoy    (1000)       18 2023-06-09 16:37:59.000000 pytorch_speech_features-0.0.1/pytorch_speech_features.egg-info/requires.txt
--rwxrwxrwx   0 debjoy    (1000) debjoy    (1000)       24 2023-06-09 16:37:59.000000 pytorch_speech_features-0.0.1/pytorch_speech_features.egg-info/top_level.txt
--rwxrwxrwx   0 debjoy    (1000) debjoy    (1000)      104 2023-06-09 16:38:00.202041 pytorch_speech_features-0.0.1/setup.cfg
--rwxrwxrwx   0 debjoy    (1000) debjoy    (1000)      521 2023-05-17 04:17:30.000000 pytorch_speech_features-0.0.1/setup.py
+drwxrwxrwx   0 debjoy    (1000) debjoy    (1000)        0 2023-06-09 18:32:24.776725 pytorch_speech_features-0.0.2/
+-rwxrwxrwx   0 debjoy    (1000) debjoy    (1000)     1068 2023-05-17 04:17:30.000000 pytorch_speech_features-0.0.2/LICENSE
+-rwxrwxrwx   0 debjoy    (1000) debjoy    (1000)      265 2023-06-09 18:32:24.778725 pytorch_speech_features-0.0.2/PKG-INFO
+-rwxrwxrwx   0 debjoy    (1000) debjoy    (1000)     2117 2023-06-09 18:26:41.000000 pytorch_speech_features-0.0.2/README.md
+-rwxrwxrwx   0 debjoy    (1000) debjoy    (1000)     1924 2023-06-09 17:55:30.000000 pytorch_speech_features-0.0.2/README.rst
+drwxrwxrwx   0 debjoy    (1000) debjoy    (1000)        0 2023-06-09 18:32:24.624930 pytorch_speech_features-0.0.2/pytorch_speech_features/
+-rwxrwxrwx   0 debjoy    (1000) debjoy    (1000)       19 2023-05-17 04:17:30.000000 pytorch_speech_features-0.0.2/pytorch_speech_features/__init__.py
+-rwxrwxrwx   0 debjoy    (1000) debjoy    (1000)    13000 2023-06-09 14:07:54.000000 pytorch_speech_features-0.0.2/pytorch_speech_features/base.py
+-rwxrwxrwx   0 debjoy    (1000) debjoy    (1000)     6292 2023-06-09 14:07:59.000000 pytorch_speech_features-0.0.2/pytorch_speech_features/sigproc.py
+drwxrwxrwx   0 debjoy    (1000) debjoy    (1000)        0 2023-06-09 18:32:24.748838 pytorch_speech_features-0.0.2/pytorch_speech_features.egg-info/
+-rwxrwxrwx   0 debjoy    (1000) debjoy    (1000)      265 2023-06-09 18:32:24.000000 pytorch_speech_features-0.0.2/pytorch_speech_features.egg-info/PKG-INFO
+-rwxrwxrwx   0 debjoy    (1000) debjoy    (1000)      384 2023-06-09 18:32:24.000000 pytorch_speech_features-0.0.2/pytorch_speech_features.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debjoy    (1000) debjoy    (1000)        1 2023-06-09 18:32:24.000000 pytorch_speech_features-0.0.2/pytorch_speech_features.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debjoy    (1000) debjoy    (1000)       18 2023-06-09 18:32:24.000000 pytorch_speech_features-0.0.2/pytorch_speech_features.egg-info/requires.txt
+-rwxrwxrwx   0 debjoy    (1000) debjoy    (1000)       24 2023-06-09 18:32:24.000000 pytorch_speech_features-0.0.2/pytorch_speech_features.egg-info/top_level.txt
+-rwxrwxrwx   0 debjoy    (1000) debjoy    (1000)      104 2023-06-09 18:32:24.786049 pytorch_speech_features-0.0.2/setup.cfg
+-rwxrwxrwx   0 debjoy    (1000) debjoy    (1000)      521 2023-06-09 18:31:23.000000 pytorch_speech_features-0.0.2/setup.py
```

### Comparing `pytorch_speech_features-0.0.1/LICENSE` & `pytorch_speech_features-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch_speech_features-0.0.1/README.md` & `pytorch_speech_features-0.0.2/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,82 @@
-# pytorch_speech_features
+pytorch_speech_features
+=======================
 
-A simple PyTorch reimplementation of library [python_speech_features](https://github.com/jameslyons/python_speech_features). 
+A simple PyTorch reimplementation of library
+`python_speech_features <https://github.com/jameslyons/python_speech_features>`__.
 
-## Uses
+Uses
+----
 
-* **Great for Intepretability experiments** - All audio processing operations can be performed and the results can be backpropagated to the original signal tensor.
-* **Supports Hybrid Model Design** - Parametric operations at different stages of audio processing.  
+-  **Great for Intepretability experiments** - All audio processing
+   operations can be performed and the results can be backpropagated to
+   the original signal tensor.
+-  **Supports Hybrid Model Design** - Parametric operations at different
+   stages of audio processing.
 
-[Example use](https://github.com/Debjoy10/pytorch_speech_features/blob/main/demo.ipynb)
+`Example
+use <https://github.com/Debjoy10/pytorch_speech_features/blob/main/demo.ipynb>`__
 
-## Installation
-> Install from GitHub
-```
-git clone https://github.com/Debjoy10/pytorch_speech_features
-python setup.py develop
-```  
+Installation
+------------
 
-## Usage
-Functions same as python_speech_features ([Refer to its documentation here](https://python-speech-features.readthedocs.io/en/latest/)).  
-> Instead of input signal as list / numpy array, pass tensor (both 'cpu' and 'cuda' supported!!). 
+   Install from PyPI
 
-See example use given above.  
+::
 
-## Testing
-Two things to test for pytorch_speech_features operations - 
-1. Similarity to python_speech_features outputs.
-2. Gradient correctness via Autograd Gradcheck. 
+   pip install pytorch-speech-features
 
-##### Find the testing python notebook here - 
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1Tyizr62YGi5-CR-o-tawV6pu68JT3DOF?usp=sharing)
+..
+
+   Install from GitHub
+
+::
+
+   git clone https://github.com/Debjoy10/pytorch_speech_features
+   python setup.py develop
+
+Usage
+-----
+
+Functions same as python_speech_features (`Refer to its documentation here <https://python-speech-features.readthedocs.io/en/latest/>`__).
+
+
+   Instead of input signal as list / numpy array, pass torch tensor (both ‘cpu’ and ‘cuda’ supported!!).
+
+::
+
+See example use given above.
+
+| Supported features:
+-  Mel Frequency Cepstral Coefficients
+- Filterbank Energies
+- Log Filterbank Energies
+- Spectral Subband Centroids
+
+Testing
+-------
+Two things to test for pytorch_speech_features operations -   
+
+
+-  Similarity to python_speech_features outputs. 
+-  Gradient correctness via Autograd Gradcheck.
+
+Find the testing python notebook here -
+'''''''''''''''''''''''''''''''''''''''
+
+|Open In Colab|
+
+Citation
+--------
 
-## Citation
 *TODO*
 
-## References
-* Python_speech_features library - [Link](https://github.com/jameslyons/python_speech_features)
-* Sample english.wav - [Link](http://voyager.jpl.nasa.gov/spacecraft/audio/english.au)
+References
+----------
+
+-  Python_speech_features library -
+   `Link <https://github.com/jameslyons/python_speech_features>`__
+-  Sample english.wav -
+   `Link <http://voyager.jpl.nasa.gov/spacecraft/audio/english.au>`__
+
+.. |Open In Colab| image:: https://colab.research.google.com/assets/colab-badge.svg
+   :target: https://colab.research.google.com/drive/1Tyizr62YGi5-CR-o-tawV6pu68JT3DOF?usp=sharing
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pytorch_speech_features-0.0.1/README.rst` & `pytorch_speech_features-0.0.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,68 +1,61 @@
-pytorch_speech_features
-=======================
+# pytorch_speech_features
 
-A simple PyTorch reimplementation of library
-`python_speech_features <https://github.com/jameslyons/python_speech_features>`__.
+[![DOI](https://zenodo.org/badge/470451115.svg)](https://zenodo.org/badge/latestdoi/470451115)
 
-Uses
-----
+A simple PyTorch reimplementation of library [python_speech_features](https://github.com/jameslyons/python_speech_features). 
 
--  **Great for Intepretability experiments** - All audio processing
-   operations can be performed and the results can be backpropagated to
-   the original signal tensor.
--  **Supports Hybrid Model Design** - Parametric operations at different
-   stages of audio processing.
+## Uses
 
-`Example
-use <https://github.com/Debjoy10/pytorch_speech_features/blob/main/demo.ipynb>`__
-
-Installation
-------------
-
-   Install from GitHub
-
-::
-
-   git clone https://github.com/Debjoy10/pytorch_speech_features
-   python setup.py develop
-
-Usage
------
-
-Functions same as python_speech_features (`Refer to its documentation here <https://python-speech-features.readthedocs.io/en/latest/>`__).
-
-
-   Instead of input signal as list / numpy array, pass torch tensor (both ‘cpu’ and ‘cuda’ supported!!).
-
-::
-
-See example use given above.
-
-Testing
--------
-Two things to test for pytorch_speech_features operations -   
-
-
--  Similarity to python_speech_features outputs. 
--  Gradient correctness via Autograd Gradcheck.
-
-Find the testing python notebook here -
-'''''''''''''''''''''''''''''''''''''''
-
-|Open In Colab|
-
-Citation
---------
-
-*TODO*
-
-References
-----------
-
--  Python_speech_features library -
-   `Link <https://github.com/jameslyons/python_speech_features>`__
--  Sample english.wav -
-   `Link <http://voyager.jpl.nasa.gov/spacecraft/audio/english.au>`__
-
-.. |Open In Colab| image:: https://colab.research.google.com/assets/colab-badge.svg
-   :target: https://colab.research.google.com/drive/1Tyizr62YGi5-CR-o-tawV6pu68JT3DOF?usp=sharing
+* **Great for Intepretability experiments** - All audio processing operations can be performed and the results can be backpropagated to the original signal tensor.
+* **Supports Hybrid Model Design** - Parametric operations at different stages of audio processing.  
+
+[Example use](https://github.com/Debjoy10/pytorch_speech_features/blob/main/demo.ipynb)
+
+## Installation
+> Install from PyPI
+```
+pip install pytorch-speech-features
+```
+
+> Install from GitHub
+```
+git clone https://github.com/Debjoy10/pytorch_speech_features
+python setup.py develop
+```  
+
+## Usage
+Functions same as python_speech_features ([Refer to its documentation here](https://python-speech-features.readthedocs.io/en/latest/)).  
+> Instead of input signal as list / numpy array, pass tensor (both 'cpu' and 'cuda' supported!!). 
+
+See example use given above.  
+
+Supported features:
+* Mel Frequency Cepstral Coefficients
+* Filterbank Energies
+* Log Filterbank Energies
+* Spectral Subband Centroids
+
+## Testing
+Two things to test for pytorch_speech_features operations - 
+1. Similarity to python_speech_features outputs.
+2. Gradient correctness via Autograd Gradcheck. 
+
+##### Find the testing python notebook here - 
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1Tyizr62YGi5-CR-o-tawV6pu68JT3DOF?usp=sharing)
+
+## Citation
+```
+@misc{https://doi.org/10.5281/zenodo.8021586,
+  doi = {10.5281/ZENODO.8021586},
+  url = {https://zenodo.org/record/8021586},
+  author = {{Debjoy Saha}},
+  title = {Debjoy10/pytorch_speech_features: Release v0.0.1},
+  publisher = {Zenodo},
+  year = {2023},
+  copyright = {Open Access}
+}
+```
+
+## References
+* Python_speech_features library - [Link](https://github.com/jameslyons/python_speech_features)
+* Sample english.wav - [Link](http://voyager.jpl.nasa.gov/spacecraft/audio/english.au)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pytorch_speech_features-0.0.1/pytorch_speech_features/base.py` & `pytorch_speech_features-0.0.2/pytorch_speech_features/base.py`

 * *Files identical despite different names*

### Comparing `pytorch_speech_features-0.0.1/pytorch_speech_features/sigproc.py` & `pytorch_speech_features-0.0.2/pytorch_speech_features/sigproc.py`

 * *Files identical despite different names*

### Comparing `pytorch_speech_features-0.0.1/setup.py` & `pytorch_speech_features-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 try:
     from setuptools import setup #enables develop
 except ImportError:
     from distutils.core import setup
 
 setup(name='pytorch_speech_features',
-      version='0.0.1',
+      version='0.0.2',
       description='PyTorch Speech Feature extraction',
       author='Debjoy Saha',
       author_email='sahadebjoy10@gmail.com',
       license='MIT',
       url='https://github.com/Debjoy10/pytorch_speech_features',
       packages=['pytorch_speech_features'],
       install_requires=[
```

