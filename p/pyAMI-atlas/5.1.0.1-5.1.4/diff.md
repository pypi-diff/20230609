# Comparing `tmp/pyAMI_atlas-5.1.0.1.tar.gz` & `tmp/pyAMI_atlas-5.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyAMI_atlas-5.1.0.1.tar", last modified: Wed Jan 29 13:55:32 2020, max compression
+gzip compressed data, was "pyAMI_atlas-5.1.4.tar", last modified: Fri Jun  9 12:58:12 2023, max compression
```

## Comparing `pyAMI_atlas-5.1.0.1.tar` & `pyAMI_atlas-5.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jodier     (502) staff       (20)        0 2020-01-29 13:55:32.000000 pyAMI_atlas-5.1.0.1/
--rw-r--r--   0 jodier     (502) staff       (20)      257 2020-01-29 13:55:32.000000 pyAMI_atlas-5.1.0.1/PKG-INFO
--rw-r--r--   0 jodier     (502) staff       (20)     2905 2020-01-24 15:25:27.000000 pyAMI_atlas-5.1.0.1/ami_atlas_post_install
-drwxr-xr-x   0 jodier     (502) staff       (20)        0 2020-01-29 13:55:32.000000 pyAMI_atlas-5.1.0.1/pyAMI_atlas/
--rw-r--r--   0 jodier     (502) staff       (20)      774 2020-01-29 13:47:32.000000 pyAMI_atlas-5.1.0.1/pyAMI_atlas/config.py
--rw-r--r--   0 jodier     (502) staff       (20)     7194 2020-01-29 13:49:42.000000 pyAMI_atlas-5.1.0.1/pyAMI_atlas/__init__.py
--rw-r--r--   0 jodier     (502) staff       (20)    27841 2020-01-23 14:38:29.000000 pyAMI_atlas-5.1.0.1/pyAMI_atlas/api.py
--rw-r--r--   0 jodier     (502) staff       (20)     5881 2020-01-23 14:31:09.000000 pyAMI_atlas-5.1.0.1/pyAMI_atlas/utils.py
--rw-r--r--   0 jodier     (502) staff       (20)    21862 2019-02-15 10:57:44.000000 pyAMI_atlas-5.1.0.1/pyAMI_atlas/license.txt
--rw-r--r--   0 jodier     (502) staff       (20)     4925 2019-10-29 09:56:37.000000 pyAMI_atlas-5.1.0.1/README
--rw-r--r--   0 jodier     (502) staff       (20)     1623 2020-01-24 14:27:33.000000 pyAMI_atlas-5.1.0.1/setup.py
-drwxr-xr-x   0 jodier     (502) staff       (20)        0 2020-01-29 13:55:32.000000 pyAMI_atlas-5.1.0.1/pyAMI_atlas.egg-info/
--rw-r--r--   0 jodier     (502) staff       (20)      257 2020-01-29 13:55:32.000000 pyAMI_atlas-5.1.0.1/pyAMI_atlas.egg-info/PKG-INFO
--rw-r--r--   0 jodier     (502) staff       (20)        1 2020-01-29 13:55:24.000000 pyAMI_atlas-5.1.0.1/pyAMI_atlas.egg-info/not-zip-safe
--rw-r--r--   0 jodier     (502) staff       (20)      376 2020-01-29 13:55:32.000000 pyAMI_atlas-5.1.0.1/pyAMI_atlas.egg-info/SOURCES.txt
--rw-r--r--   0 jodier     (502) staff       (20)       11 2020-01-29 13:55:32.000000 pyAMI_atlas-5.1.0.1/pyAMI_atlas.egg-info/requires.txt
--rw-r--r--   0 jodier     (502) staff       (20)       12 2020-01-29 13:55:32.000000 pyAMI_atlas-5.1.0.1/pyAMI_atlas.egg-info/top_level.txt
--rw-r--r--   0 jodier     (502) staff       (20)        1 2020-01-29 13:55:32.000000 pyAMI_atlas-5.1.0.1/pyAMI_atlas.egg-info/dependency_links.txt
--rw-r--r--   0 jodier     (502) staff       (20)       38 2020-01-29 13:55:32.000000 pyAMI_atlas-5.1.0.1/setup.cfg
--rwxr-xr-x   0 jodier     (502) staff       (20)    11471 2020-01-21 13:11:02.000000 pyAMI_atlas-5.1.0.1/ami_atlas
+drwxr-xr-x   0 jodier     (501) staff       (20)        0 2023-06-09 12:58:12.723831 pyAMI_atlas-5.1.4/
+-rw-r--r--   0 jodier     (501) staff       (20)      234 2023-06-09 12:58:12.722678 pyAMI_atlas-5.1.4/PKG-INFO
+-rw-r--r--   0 jodier     (501) staff       (20)     4774 2023-06-09 12:50:52.000000 pyAMI_atlas-5.1.4/README
+-rwxr-xr-x   0 jodier     (501) staff       (20)    11471 2023-06-09 12:50:52.000000 pyAMI_atlas-5.1.4/ami_atlas
+-rw-r--r--   0 jodier     (501) staff       (20)     2905 2023-06-09 12:50:52.000000 pyAMI_atlas-5.1.4/ami_atlas_post_install
+drwxr-xr-x   0 jodier     (501) staff       (20)        0 2023-06-09 12:58:12.719396 pyAMI_atlas-5.1.4/pyAMI_atlas/
+-rw-r--r--   0 jodier     (501) staff       (20)    21862 2023-06-09 12:50:52.000000 pyAMI_atlas-5.1.4/pyAMI_atlas/LICENSE.txt
+-rw-r--r--   0 jodier     (501) staff       (20)     5751 2023-06-09 12:50:52.000000 pyAMI_atlas-5.1.4/pyAMI_atlas/__init__.py
+-rw-r--r--   0 jodier     (501) staff       (20)    27841 2023-06-09 12:50:52.000000 pyAMI_atlas-5.1.4/pyAMI_atlas/api.py
+-rw-r--r--   0 jodier     (501) staff       (20)      772 2023-06-09 12:50:52.000000 pyAMI_atlas-5.1.4/pyAMI_atlas/config.py
+-rw-r--r--   0 jodier     (501) staff       (20)     5881 2023-06-09 12:50:52.000000 pyAMI_atlas-5.1.4/pyAMI_atlas/utils.py
+drwxr-xr-x   0 jodier     (501) staff       (20)        0 2023-06-09 12:58:12.722114 pyAMI_atlas-5.1.4/pyAMI_atlas.egg-info/
+-rw-r--r--   0 jodier     (501) staff       (20)      234 2023-06-09 12:58:12.000000 pyAMI_atlas-5.1.4/pyAMI_atlas.egg-info/PKG-INFO
+-rw-r--r--   0 jodier     (501) staff       (20)      390 2023-06-09 12:58:12.000000 pyAMI_atlas-5.1.4/pyAMI_atlas.egg-info/SOURCES.txt
+-rw-r--r--   0 jodier     (501) staff       (20)        1 2023-06-09 12:58:12.000000 pyAMI_atlas-5.1.4/pyAMI_atlas.egg-info/dependency_links.txt
+-rw-r--r--   0 jodier     (501) staff       (20)        1 2023-06-09 12:58:12.000000 pyAMI_atlas-5.1.4/pyAMI_atlas.egg-info/not-zip-safe
+-rw-r--r--   0 jodier     (501) staff       (20)       11 2023-06-09 12:58:12.000000 pyAMI_atlas-5.1.4/pyAMI_atlas.egg-info/requires.txt
+-rw-r--r--   0 jodier     (501) staff       (20)       12 2023-06-09 12:58:12.000000 pyAMI_atlas-5.1.4/pyAMI_atlas.egg-info/top_level.txt
+-rw-r--r--   0 jodier     (501) staff       (20)       38 2023-06-09 12:58:12.723960 pyAMI_atlas-5.1.4/setup.cfg
+-rwxr-xr-x   0 jodier     (501) staff       (20)     1623 2023-06-09 12:50:52.000000 pyAMI_atlas-5.1.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyAMI_atlas-5.1.0.1/ami_atlas_post_install` & `pyAMI_atlas-5.1.4/ami_atlas_post_install`

 * *Files identical despite different names*

### Comparing `pyAMI_atlas-5.1.0.1/pyAMI_atlas/config.py` & `pyAMI_atlas-5.1.4/pyAMI_atlas/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,14 @@
 #           fabian.lambert@lpsc.in2p3.fr
 #           solveig.albrand@lpsc.in2p3.fr
 #
 # Version : 5.X.X (2014)
 #
 #############################################################################
 
-version = '5.1.0.1'
+version = '5.1.4'
 
 #############################################################################
 
 bug_report = 'Bug reports: ami@lpsc.in2p3.fr, http://ami.in2p3.fr/pyAMI/'
 
 #############################################################################
```

### Comparing `pyAMI_atlas-5.1.0.1/pyAMI_atlas/api.py` & `pyAMI_atlas-5.1.4/pyAMI_atlas/api.py`

 * *Files identical despite different names*

### Comparing `pyAMI_atlas-5.1.0.1/pyAMI_atlas/utils.py` & `pyAMI_atlas-5.1.4/pyAMI_atlas/utils.py`

 * *Files identical despite different names*

### Comparing `pyAMI_atlas-5.1.0.1/pyAMI_atlas/license.txt` & `pyAMI_atlas-5.1.4/pyAMI_atlas/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyAMI_atlas-5.1.0.1/README` & `pyAMI_atlas-5.1.4/README`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,151 +1,151 @@
-===========
-pyAMI.atlas
-===========
-
-pyAMI 5 is a major upgrade of the AMI python client. The command line syntax
-has been rationalized, with improved help functions. The code has been split
-into a core layer and an experiment specific layer. This documentation is
-specific for the ATLAS layer.
-
-pyAMI is available in the ATLAS software release and also installed centrally
-on LXPLUS (CVFMS and AFS). pyAMI can be installed standalone on a laptop.
-Instructions are given below for Linux, OSX and Windows.
-
-.. warning:: All commands are simply subcommands of ``ami_atlas``. On centrally
-    installed versions of pyAMI we have made an alias so that ``ami`` is
-    redirected to ``ami_atlas`` and the instructions below are for this installation.
-
-.. note:: The legacy version of pyAMI (pyAMI 4.1.3) is documented `here <https://ami.in2p3.fr/pyAMI-4.1.3/>`__.
-
-A few examples
-==============
-
-List runs for 2012 in a period or multiple periods::
-
-    ami list runs --year 12 --data-periods A B
-
-List AOD datasets matching a pattern::
-
-    ami list datasets --type AOD data14_cos%
-
-Display dataset information::
-
-    ami show dataset info data13_2p76TeV.00219364.physics_MinBias.merge.NTUP_HI.f519_m1313
-
-Display dataset provenance::
-
-    ami show dataset prov data13_2p76TeV.00219364.physics_MinBias.merge.NTUP_HI.f519_m1313
-
-List the files in a dataset:: 
-
-    ami list files -LHC data13_2p76TeV.00219364.physics_MinBias.merge.NTUP_HI.f519_m1313
-
-.. note:: pyAMI also provides an API allowing you to perform all of the same queries from within your own Python program.
-
-LXPLUS (CVMFS and AFS)
-======================
-
-pyAMI is installed centrally on LXPLUS at CERN. To begin using pyAMI simply::
-
-    export ATLAS_LOCAL_ROOT_BASE=/cvmfs/atlas.cern.ch/repo/ATLASLocalRootBase
-    source $ATLAS_LOCAL_ROOT_BASE/user/atlasLocalSetup.sh
-    localSetupPyAMI
-
-pyAMI is also available through AFS::
-
-    source /afs/cern.ch/atlas/software/tools/pyAMI/setup.sh
-
-Standalone installation
-=======================
-
-pyAMI 5 is compatible with Python 2.6, 2.7 and 3.X.
-
-Automatic installation for LINUX and MAC OSX
---------------------------------------------
-
-.. warning:: If you have an earlier version of pyAMI installed please uninstall it first: ``pip uninstall pyAMI``
-
-Automatically install the latest version of pyAMI with `pip <http://pypi.python.org/pypi/pip>`_::
-
-    pip install --user pyAMI_atlas
-
-or with ``easy_install`` (deprecated)::
-
-    easy_install --user pyAMI_atlas
-
-Omit the ``--user`` for a system-wide installation (requires root privileges).
-Add ``${HOME}/.local/bin`` to your ``${PATH}`` if using ``--user`` and if it
-is not there already (put this in your .bashrc)::
-
-    # For LINUX
-    export PATH=${HOME}/.local/bin${PATH:+:$PATH}
-
-    # For MAC OSX
-    export PATH=${HOME}/Library/Python/2.7/bin${PATH:+:$PATH}
-
-Execute the post-install script::
-
-    ami_atlas_post_install
-
-To upgrade an existing installation with `pip <http://pypi.python.org/pypi/pip>`_::
-
-    pip install --upgrade pyAMI_core
-    pip install --upgrade pyAMI_atlas
-    ami_atlas_post_install
-
-or with ``easy_install`` (deprecated)::
-
-    easy_install --upgrade pyAMI_core
-    easy_install --upgrade pyAMI_atlas
-    ami_atlas_post_install
-
-Automatic installation for WINDOWS
-----------------------------------
-
-.. warning:: If you have an earlier version of pyAMI installed please uninstall it first: ``pip uninstall pyAMI``
-
-1. Install `Python 2.7.X <https://www.python.org/downloads/>`_
-
-2. ``python.exe`` should be in ``C:\Python27``. You must adjust your paths in the
-   Windows environment. If you do not know how to do this follow the instructions
-   here `www.java.com/en/download/help/path.xml <http://www.java.com/en/download/help/path.xml>`__.
-   Add to the path::
-
-    C:\PYTHON27;C:\PYTHON27\Scripts
-
-3. Download and install `pip <https://bootstrap.pypa.io/get-pip.py>`__
-   (for easy installation of dependences)::
-
-    python get-pip.py
-
-4. Install pyAMI::
-
-    pip install pyAMI_atlas
-
-5. Execute the post-install script::
-
-    ami_atlas_post_install
-
-To upgrade an existing installation::
-
-   pip install --upgrade pyAMI_core
-   pip install --upgrade pyAMI_atlas
-   ami_atlas_post_install
-
-Authentication
-==============
-
-VOMS authentication is supported::
-
-    voms-proxy-init -voms atlas
-
-If gLite is not available, the alternative option is to connect with your
-username and password. You can set up an encrypted configuration file by running::
-
-    ami auth
-
-You will only need to do this once since your credentials are stored in
-``~/.pyami/pyami.cfg`` for later use. If your credentials change just run
-``ami auth`` again. If you would like to keep your pyAMI configuration in a
-directory other than ``~/.pyami`` then set the environment variable
-``PYAMI_CONFIG_DIR``.
+===========
+pyAMI.atlas
+===========
+
+pyAMI 5 is a major upgrade of the AMI python client. The command line syntax
+has been rationalized, with improved help functions. The code has been split
+into a core layer and an experiment specific layer. This documentation is
+specific for the ATLAS layer.
+
+pyAMI is available in the ATLAS software release and also installed centrally
+on LXPLUS (CVFMS and AFS). pyAMI can be installed standalone on a laptop.
+Instructions are given below for Linux, OSX and Windows.
+
+.. warning:: All commands are simply subcommands of ``ami_atlas``. On centrally
+    installed versions of pyAMI we have made an alias so that ``ami`` is
+    redirected to ``ami_atlas`` and the instructions below are for this installation.
+
+.. note:: The legacy version of pyAMI (pyAMI 4.1.3) is documented `here <https://ami.in2p3.fr/pyAMI-4.1.3/>`__.
+
+A few examples
+==============
+
+List runs for 2012 in a period or multiple periods::
+
+    ami list runs --year 12 --data-periods A B
+
+List AOD datasets matching a pattern::
+
+    ami list datasets --type AOD data14_cos%
+
+Display dataset information::
+
+    ami show dataset info data13_2p76TeV.00219364.physics_MinBias.merge.NTUP_HI.f519_m1313
+
+Display dataset provenance::
+
+    ami show dataset prov data13_2p76TeV.00219364.physics_MinBias.merge.NTUP_HI.f519_m1313
+
+List the files in a dataset:: 
+
+    ami list files -LHC data13_2p76TeV.00219364.physics_MinBias.merge.NTUP_HI.f519_m1313
+
+.. note:: pyAMI also provides an API allowing you to perform all of the same queries from within your own Python program.
+
+LXPLUS (CVMFS and AFS)
+======================
+
+pyAMI is installed centrally on LXPLUS at CERN. To begin using pyAMI simply::
+
+    export ATLAS_LOCAL_ROOT_BASE=/cvmfs/atlas.cern.ch/repo/ATLASLocalRootBase
+    source $ATLAS_LOCAL_ROOT_BASE/user/atlasLocalSetup.sh
+    localSetupPyAMI
+
+pyAMI is also available through AFS::
+
+    source /afs/cern.ch/atlas/software/tools/pyAMI/setup.sh
+
+Standalone installation
+=======================
+
+pyAMI 5 is compatible with Python 2.6, 2.7 and 3.X.
+
+Automatic installation for LINUX and MAC OSX
+--------------------------------------------
+
+.. warning:: If you have an earlier version of pyAMI installed please uninstall it first: ``pip uninstall pyAMI``
+
+Automatically install the latest version of pyAMI with `pip <http://pypi.python.org/pypi/pip>`_::
+
+    pip install --user pyAMI_atlas
+
+or with ``easy_install`` (deprecated)::
+
+    easy_install --user pyAMI_atlas
+
+Omit the ``--user`` for a system-wide installation (requires root privileges).
+Add ``${HOME}/.local/bin`` to your ``${PATH}`` if using ``--user`` and if it
+is not there already (put this in your .bashrc)::
+
+    # For LINUX
+    export PATH=${HOME}/.local/bin${PATH:+:$PATH}
+
+    # For MAC OSX
+    export PATH=${HOME}/Library/Python/2.7/bin${PATH:+:$PATH}
+
+Execute the post-install script::
+
+    ami_atlas_post_install
+
+To upgrade an existing installation with `pip <http://pypi.python.org/pypi/pip>`_::
+
+    pip install --upgrade pyAMI_core
+    pip install --upgrade pyAMI_atlas
+    ami_atlas_post_install
+
+or with ``easy_install`` (deprecated)::
+
+    easy_install --upgrade pyAMI_core
+    easy_install --upgrade pyAMI_atlas
+    ami_atlas_post_install
+
+Automatic installation for WINDOWS
+----------------------------------
+
+.. warning:: If you have an earlier version of pyAMI installed please uninstall it first: ``pip uninstall pyAMI``
+
+1. Install `Python 2.7.X <https://www.python.org/downloads/>`_
+
+2. ``python.exe`` should be in ``C:\Python27``. You must adjust your paths in the
+   Windows environment. If you do not know how to do this follow the instructions
+   here `www.java.com/en/download/help/path.xml <http://www.java.com/en/download/help/path.xml>`__.
+   Add to the path::
+
+    C:\PYTHON27;C:\PYTHON27\Scripts
+
+3. Download and install `pip <https://bootstrap.pypa.io/get-pip.py>`__
+   (for easy installation of dependences)::
+
+    python get-pip.py
+
+4. Install pyAMI::
+
+    pip install pyAMI_atlas
+
+5. Execute the post-install script::
+
+    ami_atlas_post_install
+
+To upgrade an existing installation::
+
+   pip install --upgrade pyAMI_core
+   pip install --upgrade pyAMI_atlas
+   ami_atlas_post_install
+
+Authentication
+==============
+
+VOMS authentication is supported::
+
+    voms-proxy-init -voms atlas
+
+If gLite is not available, the alternative option is to connect with your
+username and password. You can set up an encrypted configuration file by running::
+
+    ami auth
+
+You will only need to do this once since your credentials are stored in
+``~/.pyami/pyami.cfg`` for later use. If your credentials change just run
+``ami auth`` again. If you would like to keep your pyAMI configuration in a
+directory other than ``~/.pyami`` then set the environment variable
+``PYAMI_CONFIG_DIR``.
```

### Comparing `pyAMI_atlas-5.1.0.1/setup.py` & `pyAMI_atlas-5.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `pyAMI_atlas-5.1.0.1/ami_atlas` & `pyAMI_atlas-5.1.4/ami_atlas`

 * *Files identical despite different names*

