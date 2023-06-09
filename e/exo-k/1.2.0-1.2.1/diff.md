# Comparing `tmp/Exo_k-1.2.0.tar.gz` & `tmp/exo_k-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Exo_k-1.2.0.tar", max compression
+gzip compressed data, was "exo_k-1.2.1.tar", max compression
```

## Comparing `Exo_k-1.2.0.tar` & `exo_k-1.2.1.tar`

### file list

```diff
@@ -1,46 +1,49 @@
--rw-r--r--   0        0        0    35085 2022-07-13 13:37:24.271022 Exo_k-1.2.0/LICENSE
--rw-r--r--   0        0        0     4283 2022-07-13 13:37:24.271022 Exo_k-1.2.0/README.md
--rw-r--r--   0        0        0     1199 2022-07-13 13:37:24.283022 Exo_k-1.2.0/exo_k/__init__.py
--rw-r--r--   0        0        0     8418 2022-07-13 13:37:24.283022 Exo_k-1.2.0/exo_k/adatabase.py
--rw-r--r--   0        0        0     4298 2022-07-13 13:37:24.283022 Exo_k-1.2.0/exo_k/aerosols.py
--rw-r--r--   0        0        0    21061 2022-07-13 13:37:24.283022 Exo_k-1.2.0/exo_k/atable.py
--rw-r--r--   0        0        0    40241 2022-07-13 13:37:24.283022 Exo_k-1.2.0/exo_k/atm.py
--rw-r--r--   0        0        0    14868 2022-07-13 13:37:24.283022 Exo_k-1.2.0/exo_k/atm_2band.py
--rw-r--r--   0        0        0      144 2022-07-13 13:37:24.283022 Exo_k-1.2.0/exo_k/atm_evolution/__init__.py
--rw-r--r--   0        0        0    35420 2022-07-13 13:37:24.283022 Exo_k-1.2.0/exo_k/atm_evolution/atm_evol.py
--rw-r--r--   0        0        0    12126 2022-07-13 13:37:24.283022 Exo_k-1.2.0/exo_k/atm_evolution/condensation.py
--rw-r--r--   0        0        0    26638 2022-07-13 13:37:24.283022 Exo_k-1.2.0/exo_k/atm_evolution/convection.py
--rw-r--r--   0        0        0     3126 2022-07-13 13:37:24.283022 Exo_k-1.2.0/exo_k/atm_evolution/settings.py
--rw-r--r--   0        0        0     7784 2022-07-13 13:37:24.283022 Exo_k-1.2.0/exo_k/atm_evolution/tracers.py
--rw-r--r--   0        0        0    19622 2022-07-13 13:37:24.283022 Exo_k-1.2.0/exo_k/atm_profile.py
--rw-r--r--   0        0        0     8767 2022-07-13 13:37:24.283022 Exo_k-1.2.0/exo_k/chemistry.py
--rw-r--r--   0        0        0    22627 2022-07-13 13:37:24.283022 Exo_k-1.2.0/exo_k/cia_table.py
--rw-r--r--   0        0        0    11264 2022-07-13 13:37:24.283022 Exo_k-1.2.0/exo_k/ciadatabase.py
--rw-r--r--   0        0        0    29503 2022-07-13 13:37:24.287023 Exo_k-1.2.0/exo_k/data_table.py
--rw-r--r--   0        0        0    26443 2022-07-13 13:37:24.287023 Exo_k-1.2.0/exo_k/gas_mix.py
--rw-r--r--   0        0        0    11824 2022-07-13 13:37:24.287023 Exo_k-1.2.0/exo_k/hires_spectrum.py
--rw-r--r--   0        0        0    22130 2022-07-13 13:37:24.287023 Exo_k-1.2.0/exo_k/kdatabase.py
--rw-r--r--   0        0        0    26239 2022-07-13 13:37:24.287023 Exo_k-1.2.0/exo_k/ktable.py
--rw-r--r--   0        0        0    34396 2022-07-13 13:37:24.287023 Exo_k-1.2.0/exo_k/ktable5d.py
--rw-r--r--   0        0        0    22362 2022-07-13 13:37:24.287023 Exo_k-1.2.0/exo_k/ktable_io.py
--rw-r--r--   0        0        0     5591 2022-07-13 13:37:24.287023 Exo_k-1.2.0/exo_k/rayleigh.py
--rw-r--r--   0        0        0    16266 2022-07-13 13:37:24.287023 Exo_k-1.2.0/exo_k/settings.py
--rw-r--r--   0        0        0      160 2022-07-13 13:37:24.287023 Exo_k-1.2.0/exo_k/two_stream/__init__.py
--rw-r--r--   0        0        0    15993 2022-07-13 13:37:24.287023 Exo_k-1.2.0/exo_k/two_stream/two_stream_crisp.py
--rw-r--r--   0        0        0    14348 2022-07-13 13:37:24.287023 Exo_k-1.2.0/exo_k/two_stream/two_stream_lmdz.py
--rw-r--r--   0        0        0    12104 2022-07-13 13:37:24.287023 Exo_k-1.2.0/exo_k/two_stream/two_stream_toon.py
--rw-r--r--   0        0        0      256 2022-07-13 13:37:24.287023 Exo_k-1.2.0/exo_k/util/__init__.py
--rw-r--r--   0        0        0     2480 2022-07-13 13:37:24.287023 Exo_k-1.2.0/exo_k/util/cst.py
--rw-r--r--   0        0        0     7597 2022-07-13 13:37:24.287023 Exo_k-1.2.0/exo_k/util/filenames.py
--rw-r--r--   0        0        0    21016 2022-07-13 13:37:24.287023 Exo_k-1.2.0/exo_k/util/interp.py
--rw-r--r--   0        0        0     2062 2022-07-13 13:37:24.287023 Exo_k-1.2.0/exo_k/util/molar_heat_capacity.py
--rw-r--r--   0        0        0     7020 2022-07-13 13:37:24.287023 Exo_k-1.2.0/exo_k/util/molar_mass.py
--rw-r--r--   0        0        0    13687 2022-07-13 13:37:24.287023 Exo_k-1.2.0/exo_k/util/radiation.py
--rw-r--r--   0        0        0      706 2022-07-13 13:37:24.287023 Exo_k-1.2.0/exo_k/util/singleton.py
--rw-r--r--   0        0        0     2668 2022-07-13 13:37:24.287023 Exo_k-1.2.0/exo_k/util/spectral_object.py
--rw-r--r--   0        0        0    12525 2022-07-13 13:37:24.287023 Exo_k-1.2.0/exo_k/util/spectrum.py
--rw-r--r--   0        0        0    10267 2022-07-13 13:37:24.287023 Exo_k-1.2.0/exo_k/util/user_func.py
--rw-r--r--   0        0        0    19526 2022-07-13 13:37:24.291023 Exo_k-1.2.0/exo_k/xtable.py
--rw-r--r--   0        0        0     2830 2022-07-13 13:53:50.034701 Exo_k-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     5292 1970-01-01 00:00:00.000000 Exo_k-1.2.0/setup.py
--rw-r--r--   0        0        0     6261 1970-01-01 00:00:00.000000 Exo_k-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35085 2022-09-28 14:39:44.393162 exo_k-1.2.1/LICENSE
+-rw-r--r--   0        0        0     4482 2023-06-09 13:11:32.645398 exo_k-1.2.1/README.md
+-rw-r--r--   0        0        0     1348 2023-06-09 13:11:32.649399 exo_k-1.2.1/exo_k/__init__.py
+-rw-r--r--   0        0        0       71 2023-06-09 13:11:32.649399 exo_k-1.2.1/exo_k/__version__.py
+-rw-r--r--   0        0        0     9230 2023-06-09 13:11:32.649399 exo_k-1.2.1/exo_k/adatabase.py
+-rw-r--r--   0        0        0      120 2023-06-09 13:11:32.649399 exo_k-1.2.1/exo_k/aerosol/__init__.py
+-rw-r--r--   0        0        0     1748 2023-06-09 13:11:32.649399 exo_k-1.2.1/exo_k/aerosol/util_aerosol.py
+-rw-r--r--   0        0        0     5912 2023-06-09 13:11:32.649399 exo_k-1.2.1/exo_k/aerosols.py
+-rw-r--r--   0        0        0    23639 2023-06-09 13:11:32.649399 exo_k-1.2.1/exo_k/atable.py
+-rw-r--r--   0        0        0    41280 2023-06-09 13:11:32.649399 exo_k-1.2.1/exo_k/atm.py
+-rw-r--r--   0        0        0    14964 2023-06-09 13:11:32.649399 exo_k-1.2.1/exo_k/atm_2band.py
+-rw-r--r--   0        0        0      144 2022-09-28 14:39:44.397162 exo_k-1.2.1/exo_k/atm_evolution/__init__.py
+-rw-r--r--   0        0        0    37428 2023-06-09 13:11:32.649399 exo_k-1.2.1/exo_k/atm_evolution/atm_evol.py
+-rw-r--r--   0        0        0    12510 2023-06-09 13:11:32.649399 exo_k-1.2.1/exo_k/atm_evolution/condensation.py
+-rw-r--r--   0        0        0    27332 2023-06-09 13:11:32.649399 exo_k-1.2.1/exo_k/atm_evolution/convection.py
+-rw-r--r--   0        0        0     3087 2023-06-09 13:11:32.649399 exo_k-1.2.1/exo_k/atm_evolution/settings.py
+-rw-r--r--   0        0        0     9373 2023-06-09 13:11:32.649399 exo_k-1.2.1/exo_k/atm_evolution/tracers.py
+-rw-r--r--   0        0        0    20286 2023-06-09 13:11:32.649399 exo_k-1.2.1/exo_k/atm_profile.py
+-rw-r--r--   0        0        0     8791 2023-06-09 13:11:32.649399 exo_k-1.2.1/exo_k/chemistry.py
+-rw-r--r--   0        0        0    22592 2023-06-09 13:11:32.649399 exo_k-1.2.1/exo_k/cia_table.py
+-rw-r--r--   0        0        0    11308 2023-06-09 13:11:32.649399 exo_k-1.2.1/exo_k/ciadatabase.py
+-rw-r--r--   0        0        0    28804 2023-06-09 13:11:32.649399 exo_k-1.2.1/exo_k/data_table.py
+-rw-r--r--   0        0        0    12054 2022-09-28 14:39:44.401162 exo_k-1.2.1/exo_k/fit.py
+-rw-r--r--   0        0        0    25744 2023-06-09 13:11:32.649399 exo_k-1.2.1/exo_k/gas_mix.py
+-rw-r--r--   0        0        0    13397 2023-06-09 13:11:32.649399 exo_k-1.2.1/exo_k/hires_spectrum.py
+-rw-r--r--   0        0        0    22157 2023-06-09 13:11:32.649399 exo_k-1.2.1/exo_k/kdatabase.py
+-rw-r--r--   0        0        0    26371 2023-06-09 13:11:32.649399 exo_k-1.2.1/exo_k/ktable.py
+-rw-r--r--   0        0        0    34492 2023-06-09 13:11:32.649399 exo_k-1.2.1/exo_k/ktable5d.py
+-rw-r--r--   0        0        0    22372 2022-09-28 14:39:44.401162 exo_k-1.2.1/exo_k/ktable_io.py
+-rw-r--r--   0        0        0     5639 2023-06-09 13:11:32.653399 exo_k-1.2.1/exo_k/rayleigh.py
+-rw-r--r--   0        0        0    16616 2023-06-09 13:11:32.653399 exo_k-1.2.1/exo_k/settings.py
+-rw-r--r--   0        0        0      160 2022-09-28 14:39:44.401162 exo_k-1.2.1/exo_k/two_stream/__init__.py
+-rw-r--r--   0        0        0    16077 2023-06-09 13:11:32.653399 exo_k-1.2.1/exo_k/two_stream/two_stream_crisp.py
+-rw-r--r--   0        0        0    14348 2022-09-28 14:39:44.401162 exo_k-1.2.1/exo_k/two_stream/two_stream_lmdz.py
+-rw-r--r--   0        0        0    12154 2023-06-09 13:11:32.653399 exo_k-1.2.1/exo_k/two_stream/two_stream_toon.py
+-rw-r--r--   0        0        0      256 2022-09-28 14:39:44.401162 exo_k-1.2.1/exo_k/util/__init__.py
+-rw-r--r--   0        0        0     2567 2022-09-28 14:39:44.401162 exo_k-1.2.1/exo_k/util/cst.py
+-rw-r--r--   0        0        0     7597 2022-09-28 14:39:44.401162 exo_k-1.2.1/exo_k/util/filenames.py
+-rw-r--r--   0        0        0    21508 2023-06-09 13:11:32.653399 exo_k-1.2.1/exo_k/util/interp.py
+-rw-r--r--   0        0        0     2062 2022-09-28 14:39:44.401162 exo_k-1.2.1/exo_k/util/molar_heat_capacity.py
+-rw-r--r--   0        0        0     7020 2022-09-28 14:39:44.401162 exo_k-1.2.1/exo_k/util/molar_mass.py
+-rw-r--r--   0        0        0    13896 2023-06-09 13:11:32.653399 exo_k-1.2.1/exo_k/util/radiation.py
+-rw-r--r--   0        0        0      706 2022-09-28 14:39:44.401162 exo_k-1.2.1/exo_k/util/singleton.py
+-rw-r--r--   0        0        0     5358 2023-06-09 13:11:32.653399 exo_k-1.2.1/exo_k/util/spectral_object.py
+-rw-r--r--   0        0        0    14858 2023-06-09 13:11:32.653399 exo_k-1.2.1/exo_k/util/spectrum.py
+-rw-r--r--   0        0        0     9718 2023-06-09 13:11:32.653399 exo_k-1.2.1/exo_k/util/user_func.py
+-rw-r--r--   0        0        0    19550 2023-06-09 13:11:32.653399 exo_k-1.2.1/exo_k/xtable.py
+-rw-r--r--   0        0        0     3301 2023-06-09 13:22:14.173032 exo_k-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6564 1970-01-01 00:00:00.000000 exo_k-1.2.1/PKG-INFO
```

### Comparing `Exo_k-1.2.0/LICENSE` & `exo_k-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Exo_k-1.2.0/README.md` & `exo_k-1.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 # Exo_k
 
 Author: Jeremy Leconte (CNRS/LAB/Univ. Bordeaux)
 
 `Exo_k` is a Python 3 based library to handle radiative opacities from various sources for atmospheric applications.
+It now comes with a full-fledged 1D atmospheric evolution model.
+
 It enables you to:
 
 * Interpolate efficiently and easily in correlated-k and cross section tables.
 * Convert easily correlated-k and cross section tables from one format to another
   (hdf5, LMDZ GCM, Exomol, Nemesis, PetitCode, TauREx, ExoREM, ARCIS, etc.).
 * Adapt precomputed correlated-k tables to your needs by changing:
 
-  * the resolution and quadrature (g) grid,
+  * the spectral and quadrature (g) grids,
   * the pressure/temperature grid.
 * Create tables for a mix of gases using tables for individual gases.
 * Create your own tables from high-resolution spectra (for example from K-spectrum, Helios-K, etc.).
 * Use your data in an integrated radiative transfer framework to simulate planetary atmospheres.
+* Compute the physical state of planetary atmospheres in radiative-convective equilibrium.
   
 For a complete online documentation, checkout:
 http://perso.astrophy.u-bordeaux.fr/~jleconte/exo_k-doc/index.html
 
-In this repository, you'll find a [tutorial jupyter notebook](https://forge.oasu.u-bordeaux.fr/jleconte/exo_k-public/-/blob/public/tutorial-exo_k.ipynb) that will show you how to do all that
+In this repository, you'll find a [tutorial jupyter notebook](https://forge.oasu.u-bordeaux.fr/jleconte/exo_k-public/-/blob/public/tutorials/tutorial-exo_k.ipynb) that will show you how to do all that
 with concrete examples that you can run on your own machine. Many important concepts and options are
 presented along the way.
 
 Enjoy!
 
 J. Leconte
 
@@ -39,30 +42,24 @@
 (grant agreement n° 679030/WHIPLASH).
 
 The framework for this documentation has been developped by Aurelien Falco using Sphinx.
 The Framework for automatic testing has been developped by Alexandre Mechineau. 
 
 # last release (see past releases below)
 
-v1.2.0 (July 2022): The model for atmospheric evolution is finally stable and documented.
-The atm module has also seen several note worthy additions: surface albedo, oceans. 
-We also added a framework for an automatic test suite. In particular, we can test several python versions. Additional tests should rapidly come along.
-Rosseland and Planck mean opacities can now be computed from radiative tables. 
+v1.2.1 (June 2023): Fixes some minor bugs in the atmospheric evolution module.
+Addition of a contribution function in the atmospheric radiative transfer module. See the atmosphere tutorial for an example.
 
 # Installation
 
 Exo_k can be installed using pip (without cloning the repository;
 dependencies should be downloaded automatically):
 ```
 pip install exo_k
 ```
-Or by running the [setup.py](https://forge.oasu.u-bordeaux.fr/jleconte/exo_k-public/-/blob/public/setup.py) script in the cloned repository:
-```
-python setup.py install
-```
 
 # Usage
 
 To learn how to use `exo_k`, you can follow the [tutorial jupyter notebook](https://forge.oasu.u-bordeaux.fr/jleconte/exo_k-public/-/blob/public/tutorial-exo_k.ipynb).
 
 Have fun!
 
@@ -72,14 +69,19 @@
 * Code repository: https://forge.oasu.u-bordeaux.fr/jleconte/exo_k-public
 * Documentation: http://perso.astrophy.u-bordeaux.fr/~jleconte/exo_k-doc/index.html
 * Contact: jeremy.leconte at u-bordeaux.fr
 
 
 # past releases
 
+v1.2.0 (July 2022): The model for atmospheric evolution is finally stable and documented.
+The atm module has also seen several note worthy additions: surface albedo, oceans. 
+We also added a framework for an automatic test suite. In particular, we can test several python versions. Additional tests should rapidly come along.
+Rosseland and Planck mean opacities can now be computed from radiative tables. 
+
 v1.1.0 (August 2021): New scheme for the computation of atmospheric emission/transmission
 to ensure an improved numerical accuracy. The variable names to instantiate atm objects have
 changed accordingly (see tutorial). 
 
 v1.0.2 (June 2021): Adds a few missing dependencies. Enables computation of thermal
 emission spectra with scattering through the two-stream method (full documentation pending). 
 Enables creating Xtables for a mix of gases (CIA can be added as well). Solves some issues
```

### Comparing `Exo_k-1.2.0/exo_k/__init__.py` & `exo_k-1.2.1/exo_k/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 @author: jeremy leconte
 __init__ module to load the exo_k library
 """
+from .__version__ import __version__
+
 from exo_k.util.user_func import *
 from exo_k.two_stream import two_stream_crisp, two_stream_toon, two_stream_lmdz
 from exo_k.util.radiation import *
 from exo_k.util.interp import gauss_legendre, split_gauss_legendre
 from exo_k.util.cst import *
 from exo_k.util.spectrum import Spectrum
 from exo_k.util.filenames import *
@@ -25,7 +27,9 @@
 from .atm_2band import Atm_2band
 from .chemistry import EquChemTable, InterpolationChemistry
 from .gas_mix import Gas_mix, Known_composite_species
 from .settings import Settings
 from .rayleigh import Rayleigh
 from exo_k.atm_evolution.atm_evol import Atm_evolution
 from exo_k.atm_evolution.condensation import Condensation_Thermodynamical_Parameters, Condensing_species
+from exo_k.aerosol.util_aerosol import mmr_to_number_density, mmr_to_number_density_ratio
+from .fit import Fit
```

### Comparing `Exo_k-1.2.0/exo_k/adatabase.py` & `exo_k-1.2.1/exo_k/adatabase.py`

 * *Files 15% similar despite different names*

```diff
@@ -23,44 +23,53 @@
                 List of names (not full path) of the input cia files. 
                 The files must be in the global search path.
                 
         A local search path can be specified with 'search_path='
 
         See the options of :class:`~exo_k.atable.Atable` __init__ method.
         """
-        self.atables={}
-        self.r_eff_unit=None
-        self.wns=None
-        self.Nw=None
+        super().__init__()
+        self.atables = {}
+        self.r_eff_unit = None
         if filenames is not None:
             for filename in filenames:
-                tmp_atable=Atable(*([filename]+list(str_filters)),
+                tmp_atable = Atable(*([filename]+list(str_filters)),
                     remove_zeros=remove_zeros, **kwargs)
                 self.add_atables(tmp_atable)
     
     def add_atables(self, *atables):
         """Adds new :class:`~exo_k.atable.Atable` objects to a Adatabase.
 
         Parameters
         ----------
             atables: :class:`~exo_k.atable.Atable`
                 As many Atables as you want.
         """
         for atable in atables:
             if self.r_eff_unit is None:
-                self.r_eff_unit=atable.r_eff_unit
-            elif self.r_eff_unit!=atable.r_eff_unit:
+                self.r_eff_unit = atable.r_eff_unit
+            elif self.r_eff_unit != atable.r_eff_unit:
                 print('Adatabase units for r_eff: {k}'.format(k=self.r_eff_unit))
                 print('{aer} units for cia coeff: {k}'.format(\
                     aer=atable.aerosol_name, k=atable.r_eff_unit))
                 raise RuntimeError("""You naughty:
                 all Atables in a database must have the same r_eff units""")
             # should ultimately check for wn_unit as well !
 
-            self.atables[atable.aerosol_name]=atable
+            self.atables[atable.aerosol_name] = atable
+
+            if self.wns is None:
+                self.wns = atable.wns
+                self.Nw = self.wns.size
+            else:
+                if np.any(self.wns != atable.wns):
+                    self.wns = None
+                    self.Nw = None
+
+
 
     @property
     def names(self):
         """Gives the names of the aerosols in the database
         """
         return list(self.atables.keys())
 
@@ -83,18 +92,18 @@
     def __repr__(self):
         """Method to output
         """
         output='The available aerosols are: \n'
         for aer,atab in self.atables.items():
             output+=aer+'->'+atab.filename+'\n'
         if self.wns is not None:
-            output+='All tables share a common spectral grid\n'
+            output += 'All tables share a common spectral grid\n'
         else:
-            output+='All tables do NOT have common spectral grid\n'
-            output+='You will need to run sample before using the database\n'
+            output += 'All tables do NOT have common spectral grid\n'
+            output += 'You will need to run sample before using the database\n'
 
         return output
 
     def sample(self, wngrid, remove_zeros=True, use_grid_filter=True,
             sample_all_vars=True):
         """Samples all the Atables in the database on the same wavenumber grid
         to be able to use them in radiative transfer modules.
@@ -104,98 +113,108 @@
             This ensures that you do not count several contributinns twice when
             you use two different aerosol tables to represent
             the same aerosol type over two different
             spectral window (typically VI and IR)
 
         Parameters
         ----------
-            wngrid : array
+            wngrid : array, np.ndarray
                 new wavenumber grid (cm-1)
 
         .. seealso::
-            See :func:`exo_k.atable.Atable.sample for further details on options.
+            See :func:`exo_k.atable.Atable.sample` for further details on options.
         """
         for atable in self.atables.values():
             atable.sample(wngrid, remove_zeros=remove_zeros, use_grid_filter=use_grid_filter,
                 sample_all_vars=sample_all_vars)
-        self.wns=np.array(wngrid)
-        self.Nw=self.wns.size
+        self.wns = np.array(wngrid)
+        self.Nw = self.wns.size
 
     def convert_to_mks(self):
         """Converts units of all Cia_tables to MKS.
         """
         first=True
         for atable in self.atables.values():
             atable.convert_to_mks()
             if first:
-                self.r_eff_unit=atable.r_eff_unit
+                self.r_eff_unit = atable.r_eff_unit
         
 
     def absorption_coefficient(self, aer_reffs_densities,
             wngrid_limit=None, log_interp=None):
-        """Computes the absorption coefficient in m^-1 for the whole mix specified 
+        """Computes the opacity for the whole mix specified 
         (assumes data in MKS).
 
+        .. warning::
+            The unit and physical meaning of the result may change depending on the
+            quantity provided in aer_reffs_densities.
+            See :func:`exo_k.atable.Atable.absorption_coefficient` for further details.
+
         Parameters
         ----------
             aer_reffs_densities: dict
                 A dictionary with aerosol names as keys and lists containing 2
                 floats (or arrays) as values. The values are the particle effective radii
-                and number densities.
+                and number densities (or ratio of aerosol to gas number density).
 
-            wngrid_limit: array, optional
+            wngrid_limit: array, np.ndarray, optional
                 Smaller and bigger wavenumbers inside which to perform the calculation.
 
         Returns:
             array:
-                The effective cross section coefficient profile for the aerosols (in m^2).
+                The opacity profile for the aerosols.
         """
         first=True
         if self.wns is None: raise RuntimeError("""Atables must be sampled
             on the same grid before calling cross_section.
             Please use the sample() method.""")
         for aer, values in aer_reffs_densities.items():
             if aer in self.atables.keys():
                 if first:
-                    res=self.atables[aer].absorption_coefficient(values[0], values[1],
+                    res = self.atables[aer].absorption_coefficient(values[0], values[1],
                         wngrid_limit=wngrid_limit, log_interp=log_interp)
                     first=False
                 else:
-                    res+=self.atables[aer].absorption_coefficient(values[0], values[1],
+                    res += self.atables[aer].absorption_coefficient(values[0], values[1],
                         wngrid_limit=wngrid_limit, log_interp=log_interp)
         if first: # means that no molecule was in the database, we need to initialize res
             res=np.zeros((1, self.wns.size))
         return res
 
     def optical_properties(self, aer_reffs_densities, wngrid_limit=None,
             log_interp=None, compute_all_opt_prop=True):
         """Computes the optical properties for the mix of aerosols
         (assumes data in MKS).
 
+        .. warning::
+            The unit and physical meaning of the result may change depending on the
+            quantity provided in aer_reffs_densities.
+            See :func:`exo_k.atable.Atable.absorption_coefficient` for further details.
+
         Parameters
         ----------
             aer_reffs_densities: dict
                 A dictionary with aerosol names as keys and lists containing 2
                 floats (or arrays) as values. The values are the particle effective radii
-                and number densities.
+                and number densities (or ratio of aerosol to gas number density).
 
-            wngrid_limit: array, optional
+            wngrid_limit: array, np.ndarray, optional
                 Smaller and bigger wavenumbers inside which to perform the calculation.
 
         Returns:
             array:
-                The effective cross section coefficient profile for the aerosols (in m^2).
+                The optical properties profile for the aerosols (in m^2).
         """
         first=True
         if self.wns is None: raise RuntimeError("""Atables must be sampled
             on the same grid before calling optical_properties.
             Please use the sample() method.""")
         for aer, values in aer_reffs_densities.items():
             if aer in self.atables.keys():
-                [k, kscat, g]=self.atables[aer].optical_properties(values[0], values[1],
+                [k, kscat, g] = self.atables[aer].optical_properties(values[0], values[1],
                         wngrid_limit=wngrid_limit, log_interp=log_interp,
                         compute_all_opt_prop=compute_all_opt_prop)
                 k_scat_g = kscat * g
                 if first:
                     k_tot = k
                     kscat_tot = kscat
                     g_tot = k_scat_g
```

### Comparing `Exo_k-1.2.0/exo_k/aerosols.py` & `exo_k-1.2.1/exo_k/aerosols.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,73 +2,83 @@
 """
 @author: jeremy leconte
 """
 import numpy as np
 from .util.spectral_object import Spectral_object
 
 class Aerosols(Spectral_object):
-    """Dict-like class to handle gas composition (with background gas) and molar mass.
-
-    If `logp_array`, `t_array`, and radiative databases are provided, :any:`cross_section`
-    can be used to compute the opacity of the gas
+    """Dict-like class to handle aerosol composition, reff, and density, and link this to the optical propoerties.
     """
 
-    def __init__(self, aer_reffs_densities={}, a_database=None):
-        """__init__ Instantiates
-        an aerosols object.
+    def __init__(self, aer_reffs_densities=None, a_database=None):
+        """__init__ Instantiates an aerosols object.
         """
+        super().__init__()
         self.set_a_database(a_database=a_database)
         self.set_aer_reffs_densities(aer_reffs_densities=aer_reffs_densities)
         self._wn_range=None
 
-    def set_aer_reffs_densities(self, aer_reffs_densities={}):
-        self.aer_reffs_densities = aer_reffs_densities
+    def set_aer_reffs_densities(self, aer_reffs_densities=None):
+        """Set the dictionary with the arrays of the effective radii and number densities for the aerosols.
 
-    def set_a_database(self, a_database=None):
-        """Change the radiative database attached to the current instance of aerosols
+        .. warning::
+            The unit and physical meaning of the result may change depending on the
+            quantity provided in aer_reffs_densities (number density or ratio of particle to gas number density).
+            See :func:`exo_k.atable.Atable.absorption_coefficient` for further details.
+
+            For use in the amtospheric model, one should provide the particle to gas number density ratio.
 
         Parameters
         ----------
-            a_database: :class:`~exo_k.kdatabase.Kdatabase` object
-                New Adatabase to use.
+            aer_reffs_densities: dict
+                A dictionary with aerosol names as keys and lists containing 2
+                floats (or arrays) as values. The values are the particle effective radii
+                and number densities (or ratio of aerosol to gas number density).
         """
-        self.adatabase=a_database
-        if self.adatabase is not None and self.adatabase.r_eff_unit != 'm' :
-            print("""
-            You're being Bad!!! You are trying *NOT* to use MKS units
-            for the effective radii in the aerosol database!!!""")
-            raise RuntimeError("Bad units in the Adatabase used with aerosols.")
-
-    def _compute_spectral_range(self, wn_range=None, wl_range=None):
-        """Converts an unordered spectral range in either wavenumber or wavelength
-        in an ordered wavenumber range.
+        if aer_reffs_densities is None:
+            self.aer_reffs_densities = {}
+        else:
+            self.aer_reffs_densities = aer_reffs_densities
+
+    def set_a_database(self, a_database=None):
+        """Change the radiative database attached to the current instance of aerosols
 
         Parameters
         ----------
-            wn_range: list or array of size 2
-                Minimum and maximum wavenumber (in cm^-1).
-            wl_range: list or array of size 2
-                Minimum and maximum wavelength (in micron)
+            a_database: :class:`~exo_k.kdatabase.Kdatabase` object
+                New Adatabase to use.
         """
-        if wl_range is not None:
-            if wn_range is not None:
-                print('Cannot specify both wl and wn range!')
-                raise RuntimeError()
-            else:
-                _wn_range=np.sort(10000./np.array(wl_range))
-        else:
-            if wn_range is not None:
-                _wn_range=np.sort(np.array(wn_range))
-            else:
-                _wn_range=self._wn_range
-        return _wn_range
+        self.adatabase = a_database
+        if self.adatabase is not None:
+            if self.adatabase.r_eff_unit != 'm' :
+                print("""
+                You're being Bad!!! You are trying *NOT* to use MKS units
+                for the effective radii in the aerosol database!!!""")
+                raise RuntimeError("Bad units in the Adatabase used with aerosols.")
 
     def optical_properties(self, aer_reffs_densities=None, wl_range=None, wn_range=None,
             log_interp=True, compute_all_opt_prop=True, **kwargs):
-        """bla
+        """Compute the optical properties for the mix.
+
+        Parameters
+        ----------
+            aer_reffs_densities: dict
+                A dictionary with aerosol names as keys and lists containing 2
+                floats (or arrays) as values. The values are the particle effective radii
+                and number densities (or ratio of aerosol to gas number density).
+                See :func:`exo_k.atable.Atable.absorption_coefficient` for further details.
+
+        Other Parameters
+        ----------------
+            wl_range, wn_range: two-value list
+                Wavelength or wavenumber range to consider
+            log_interp: bool, optional
+                Whether the interpolation is linear in kdata or in log(kdata).
+            compute_all_opt_prop: bool, optional
+                Whether to compute all the optical properties or just the extinction.
         """
         if self.adatabase is None: raise RuntimeError("""
             a_database not provided. 
             Use the a_database keyword during initialization or use the set_a_database method.""")
         if self.adatabase.wns is None: raise RuntimeError("""
             All tables in the Adatabase should have the same wavenumber grid to proceed.
             You should probably use sample().""")
@@ -80,15 +90,30 @@
         [k, k_scat, g] = self.adatabase.optical_properties(self.aer_reffs_densities,
             wngrid_limit=local_wn_range, log_interp=log_interp,
             compute_all_opt_prop=compute_all_opt_prop)
         return [k, k_scat, g]
     
     def absorption_coefficient(self, aer_reffs_densities=None, wl_range=None, wn_range=None,
             log_interp=True, **kwargs):
-        """bla
+        """Compute the aerosol opacity for the mix.
+
+        Parameters
+        ----------
+            aer_reffs_densities: dict
+                A dictionary with aerosol names as keys and lists containing 2
+                floats (or arrays) as values. The values are the particle effective radii
+                and number densities (or ratio of aerosol to gas number density).
+                See :func:`exo_k.atable.Atable.absorption_coefficient` for further details.
+
+        Other Parameters
+        ----------------
+            wl_range, wn_range: two-value list
+                Wavelength or wavenumber range to consider
+            log_interp: bool, optional
+                Whether the interpolation is linear in kdata or in log(kdata).
         """
         if self.adatabase is None: raise RuntimeError("""
             a_database not provided. 
             Use the a_database keyword during initialization or use the set_a_database method.""")
         if self.adatabase.wns is None: raise RuntimeError("""
             All tables in the Adatabase should have the same wavenumber grid to proceed.
             You should probably use sample().""")
```

### Comparing `Exo_k-1.2.0/exo_k/atable.py` & `exo_k-1.2.1/exo_k/atable.py`

 * *Files 13% similar despite different names*

```diff
@@ -63,30 +63,27 @@
         if self.ext_coeff is not None:
             if self._settings._convert_to_mks or mks: self.convert_to_mks()
             if remove_zeros: self.remove_zeros()
 
     def _init_empty(self):
         """Initializes attributes to none.
         """
+        super().__init__()
         self.aerosol_name=None
-        self.wns=None
-        self.wnedges=None
-        self.wn_unit='cm^-1'
         self.ext_coeff=None
         self.single_scat_alb=None
         self.asymmetry_factor=None
         self.r_eff_grid=None
         self.r_eff_unit=None
-        self.Nw=None
         self.Nr=None
         self.filename=None
 
 
     def read_LMDZ(self, filename, aerosol_name=None, N_per_line=5):
-        """Reads LMDZ like optical propertt files.
+        """Reads LMDZ like optical properties files.
 
         Parameters
         ----------
             filename: str
                 Name of the file to be read.
         """
         with open(filename, 'r') as file:
@@ -111,15 +108,15 @@
         self.r_eff_unit='m'
         if aerosol_name:
             self.aerosol_name=aerosol_name
         else:
             self.aerosol_name=os.path.basename(filename).split('.')[0]
 
     def _read_arrays(self, file, Nvalue, Narray, N_per_line=5):
-        """Reads an array in a optical property LMDZ file.
+        """Reads an array in an optical property LMDZ file.
         Assumes that the arrays are arranged 5 values per line.
 
         Parameters
         ----------
             file: file stream
                 File to be read.
             Nvalue: int
@@ -157,14 +154,15 @@
                 self.aerosol_name=aerosol_name
             else:
                 self.aerosol_name=f['aerosol_name'][()]
             if isinstance(self.aerosol_name, bytes):
                 self.aerosol_name=self.aerosol_name.decode('UTF-8')
             self.wns=f['bin_centers'][...]
             self.wnedges=np.concatenate(([self.wns[0]],0.5*(self.wns[1:]+self.wns[:-1]),[self.wns[-1]]))
+            self.Nw = self.wns.size
             iw_min, iw_max = self.select_spectral_range(wn_range, wl_range)
             if 'units' in f['bin_centers'].attrs:
                 self.wn_unit=f['bin_centers'].attrs['units']
             self.ext_coeff=f['ext_coeff'][..., iw_min:iw_max]
             self.single_scat_alb=f['single_scat_alb'][..., iw_min:iw_max]
             self.asymmetry_factor=f['asymmetry_factor'][..., iw_min:iw_max]
             self.r_eff_grid=f['r_eff'][...]
@@ -191,19 +189,19 @@
             f.create_dataset("single_scat_alb", data=self.single_scat_alb, compression=compression)
             f.create_dataset("asymmetry_factor", data=self.asymmetry_factor, compression=compression)
             f["bin_centers"].attrs["units"] = self.wn_unit
             f["r_eff"].attrs["units"] = self.r_eff_unit
 
     def sample(self, wngrid, remove_zeros=False, use_grid_filter=False,
             sample_all_vars=True, **kwargs):
-        """Method to re sample a Atable to a new grid of wavenumbers (in place)
+        """Method to re sample an Atable to a new grid of wavenumbers (in place)
 
         Parameters
         ----------
-            wngrid : array
+            wngrid : array, np.ndarray
                 new wavenumber grid (cm-1)
             use_grid_filter: boolean, optional
                 If true, the table is sampled only within the boundaries
                 of its current wavenumber grid. The coefficients are set to zero elswere
                 (except if remove_zeros is set to True).
                 If false, the values at the boundaries are used when sampling outside the grid.
             sample_all_vars: boolean, optional
@@ -261,15 +259,15 @@
                 Effective radius array to interpolate to.
                 If a float is given, it is interpreted as an array of size 1.
             data_id: int
                 type of data to interpolate:
                   * 0 is extinction coefficient
                   * 1 is single scattering albedo
                   * 2 is asymmetry factor
-            wngrid_limit: array, optional
+            wngrid_limit: array, np.ndarray, optional
                 If an array is given, interpolates only within this array.
             log_interp: bool, optional
                 Whether the interpolation is linear in kdata or in log(kdata).
         """
         if hasattr(r_array, "__len__"):
             r_array=np.array(r_array)
         else:
@@ -279,15 +277,15 @@
             wngrid_filter = slice(None)
             Nw=self.Nw
         else:
             wngrid_limit=np.array(wngrid_limit)
             wngrid_filter = np.where((self.wnedges > wngrid_limit.min()) & (
                 self.wnedges <= wngrid_limit.max()))[0][:-1]
             Nw=wngrid_filter.size
-        if log_interp is None: log_interp=self._settings._log_interp
+        if log_interp is None: log_interp=self._settings._log_interp_aerosol
         if var_type == -1:
             return [interp_data(self.ext_coeff, rind, rweight, Nw, wngrid_filter, log_interp),
                 interp_data(self.single_scat_alb, rind, rweight, Nw, wngrid_filter, log_interp),
                 interp_data(self.asymmetry_factor, rind, rweight, Nw, wngrid_filter, log_interp)
                 ]
         if var_type == 0:
             data_to_interp=self.ext_coeff
@@ -305,68 +303,88 @@
         ----------
             r_array: float or array
                 Effective radius array to interpolate to.
                 If a float is given, it is interpreted as an array of size 1.
 
         Other Parameters
         ----------------
-            wngrid_limit: array, optional
+            wngrid_limit: array, np.ndarray, optional
                 If an array is given, interpolates only within this array.
             log_interp: bool, optional
                 Whether the interpolation is linear in kdata or in log(kdata).
         """
         if hasattr(r_array, "__len__"):
             r_array=np.array(r_array)
         else:
             r_array=np.array([r_array])
         area=PI*r_array**2
         return (area*self.interpolate_optical_properties(r_array=r_array,
             wngrid_limit=wngrid_limit, log_interp=log_interp).transpose()).transpose()
 
     def absorption_coefficient(self, r_array, n_density, wngrid_limit=None, log_interp=None):
-        """Computes the absorption coefficient due to the aerosol (in per unit length).
+        """Computes the opacity due to the aerosols.
 
+        .. warning::
+            If n_density is the number density of aerosol particles (in m^-3),
+            then the result is the absorption coefficient in m^-1.
+
+            If n_density is the ratio of the number density of aerosol particles
+            normalized to the number density of gas molecules (dimless), 
+            then the result is a cross section (in m^2) for aerosols normalized "per gas molecule".
+            This latter choice allows us to directly add it to gaseous cross sections later-on without
+            further normalizations. This is what needs to be used when coupling with the atmospheric model.
+            
         Parameters
         ----------
             r_array: float or 1d array
                 Effective radius array to interpolate to.
                 If a float is given, it is interpreted as an array of size 1.
             n_density: float or 1d array (same dim as r_array)
-                Number density of aerosol
+                Number density of aerosol or ratio of aerosol to gas particle number density (see above). 
 
         Other Parameters
         ----------------
-            wngrid_limit: array, optional
+            wngrid_limit: array, np.ndarray, optional
                 If an array is given, interpolates only within this array.
             log_interp: bool, optional
                 Whether the interpolation is linear in kdata or in log(kdata).
         """
         if hasattr(r_array, "__len__"):
             r_array=np.array(r_array)
         else:
             r_array=np.array([r_array])
         factor=np.array(n_density)*PI*r_array**2
         return (factor*self.interpolate_optical_properties(r_array=r_array,
             wngrid_limit=wngrid_limit, log_interp=log_interp).transpose()).transpose()
 
     def optical_properties(self, r_array, n_density, wngrid_limit=None,
             log_interp=None, compute_all_opt_prop=True):
-        """Computes all the optical properties for the aerosol.
+        """Computes all the optical properties for the aerosols.
+
+        .. warning::
+            If n_density is the number density of aerosol particles (in m^-3),
+            then kdata is the absorption coefficient in m^-1.
+
+            If n_density is the ratio of the number density of aerosol particles
+            normalized to the number density of gas molecules (dimless), 
+            then kdata is a cross section (in m^2) for aerosols normalized "per gas molecule".
+            This latter choice allows us to directly add it to gaseous cross sections later-on without
+            further normalizations. This is what needs to be used when coupling with the atmospheric model.
 
         Parameters
         ----------
             r_array: float or 1d array
                 Effective radius array to interpolate to.
                 If a float is given, it is interpreted as an array of size 1.
             n_density: float or 1d array (same dim as r_array)
-                Number density of aerosol
+                Number density of aerosol or ratio of aerosol to gas particle number density (see above). 
 
         Other Parameters
         ----------------
-            wngrid_limit: array, optional
+            wngrid_limit: array, np.ndarray, optional
                 If an array is given, interpolates only within this array.
             log_interp: bool, optional
                 Whether the interpolation is linear in kdata or in log(kdata).
         """
         if hasattr(r_array, "__len__"):
             r_array=np.array(r_array)
         else:
@@ -473,16 +491,41 @@
         res.single_scat_alb = np.copy(self.single_scat_alb)
         res.asymmetry_factor = np.copy(self.asymmetry_factor)
         res.Nr = self.Nr
         res.Nw = self.Nw
         res.filename = self.filename
         return res
 
+    @classmethod
+    def concatenate_spectral_range(cls, atab1, atab2, verbose=False):
+        """Combine the instance of atable with another one for which there is some
+        overlap of the spectral range. 
+        """
+        if atab2.wns[-1] < atab1.wns[-1]:
+            atab1,atab2 = atab2,atab1
+        id_keep_ir = list(map(lambda num: num not in atab2.wns, atab1.wns))
+        new_atab = atab1.copy()
+        if verbose:
+            print(atab2.ext_coeff.shape)
+        new_atab.ext_coeff = np.concatenate( \
+                        (atab1.ext_coeff[:,id_keep_ir], atab2.ext_coeff[...]), axis=1)
+        new_atab.single_scat_alb = np.concatenate( \
+                        (atab1.single_scat_alb[:,id_keep_ir], atab2.single_scat_alb[...]), axis=1)
+        new_atab.asymmetry_factor = np.concatenate( \
+                        (atab1.asymmetry_factor[:,id_keep_ir], atab2.asymmetry_factor[...]), axis=1)
+        new_atab.wns = np.concatenate((atab1.wns[id_keep_ir], atab2.wns))
+        new_atab.Nw = len(new_atab.wns)
+        if verbose:
+            print(atab1.wns, atab2.wns, new_atab.wns)
+        return new_atab
+
 def combine_tables(aerosol_name, *atables):
     """Combine several tables representing the same aerosol type for different wavelength range.
+
+    Deprecated, use concatenate_spectral_range
     """
     r_eff_grid=atables[0].r_eff_grid
     order=np.argsort([atable.wns[0] for atable in atables])
     ordered_atables=np.array(atables)[order]
     #print(ordered_atables)
     res=ordered_atables[0].copy()
     r_eff_grid=res.r_eff_grid
```

### Comparing `Exo_k-1.2.0/exo_k/atm.py` & `exo_k-1.2.1/exo_k/atm.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     - - - - - - - - - -  bottom layer (play[Nlay-1]=psurf, tlay[3], xlay[3])
     ------------------- Surface (plev[Nlev-1=Nlay]=psurf)
     ///////////////////
 
 .. image:: /images/atm_schema.png
 
 
-Tempratures (`tlay`) and volume mixing ratios (`xlay`) are provided at the
+Temperatures (`tlay`) and volume mixing ratios (`xlay`) are provided at the
 *mid layer* point (`play`) (Note that this does not mean
 that this point is the middle of the layer, in general, it is not).
 
 If pressure levels are not specified by the user with `logplevel`,
 they are at the mid point between
 the pressure of the layers directly above and below. The pressure of the
 top and bottom levels are counfounded with the pressure of the
@@ -252,39 +252,36 @@
 
     def spectral_integration(self, spectral_var):
         """Spectrally integrate an array, taking care of whether
         we are dealing with corr-k or xsec data.
 
         Parameters
         ----------
-            spectral_var: array
+            spectral_var: array, np.ndarray
                 array to integrate
 
         Returns
         -------
-            var: array
+            var: array, np.ndarray
                 array integrated over wavenumber (and g-space if relevant)
         """
-        if self.Ng is None:
-            var=np.sum(spectral_var*self.dwnedges,axis=-1)
-        else:
-            var=np.sum(np.sum(spectral_var*self.weights,axis=-1)*self.dwnedges,axis=-1)
-        return var
+
+        return np.sum(self.g_integration(spectral_var) * self.dwnedges, axis=-1)
 
     def g_integration(self, spectral_var):
         """Integrate an array along the g direction (only for corrk)
 
         Parameters
         ----------
-            spectral_var: array
+            spectral_var: array, np.ndarray
                 array to integrate
 
         Returns
         -------
-            var: array
+            var: array, np.ndarray
                 array integrated over g-space if relevant
         """
         if self.Ng is None:
             var = spectral_var
         else:
             var = np.sum(spectral_var * self.k_database.weights, axis=-1)
         return var
@@ -326,15 +323,15 @@
             else:
                 kdata_scat_tot = np.zeros(shape[0:2], dtype=float)
             if self.aerosols.adatabase is not None:
                 kdata_scat_tot += k_scat_aer
                 self.asym_param = np.where(kdata_scat_tot<=0., 0., k_scat_aer * g_aer / kdata_scat_tot)
                 #the line below is for test. Should be removed
                 #self.asym_param = np.zeros(shape[0:2], dtype=float)
-                self.asym_param = np.ones(shape[0:2], dtype=float)
+                #self.asym_param = np.ones(shape[0:2], dtype=float)
             else:
                 self.asym_param = np.zeros(shape[0:2], dtype=float)
 
             if self.Ng is None:
                 self.single_scat_albedo = kdata_scat_tot / self.kdata
             else:
                 self.single_scat_albedo = kdata_scat_tot[:,:,None] / self.kdata
@@ -374,20 +371,21 @@
                     /self.dwnedges
             else:
                 piBatm=PI*Bnu(self.wns[None,:],self.tlay[:,None])
         else:
             piBatm=np.zeros((self.Nlay,self.Nw))
         return piBatm
 
-    def setup_emission_caculation(self, mu_eff = 0.5, rayleigh = None, integral = True,
-            source = True, gas_vmr = None, Mgas = None, **kwargs):
+    def setup_emission_caculation(self, mu_eff=0.5, rayleigh=None, integral=True,
+            source=True, gas_vmr=None, Mgas=None, aer_reffs_densities=None, **kwargs):
         """Computes all necessary quantities for emission calculations
         (opacity, source, etc.)
         """
         if gas_vmr is not None: self.set_gas(gas_vmr, Mgas = Mgas)
+        if aer_reffs_densities is not None: self.aerosols.set_aer_reffs_densities(aer_reffs_densities=aer_reffs_densities)
         self.opacity(rayleigh = rayleigh, **kwargs)
         self.set_surface_albedo(**kwargs)
         self.set_incoming_stellar_flux(**kwargs)
         self.piBatm = self.source_function(integral=integral, source=source)
         self.compute_layer_col_density()
         if self.Ng is None:
             self.tau, self.dtau=rad_prop_xsec(self.dcol_density_rad,
@@ -648,18 +646,18 @@
         ----------
             per_unit_mass: bool
                 If True, the heating rates are normalized by the
                 mass of each layer (result in W/kg).
 
         Returns
         -------
-            H: array
+            H: array, np.ndarray
                 Heating rate in each layer (Difference of the net fluxes). Positive means heating.
                 The last value is the net flux impinging on the surface + the internal flux.
-            net: array
+            net: array, np.ndarray
                 Net fluxes at level surfaces
         """
         if self.flux_net_nu is None:
             raise RuntimeError('should have ran emission_spectrum_2stream.')
         net = self.spectral_integration(self.flux_net_nu)
         H = -np.copy(net)
         H[:-1] -= H[1:]
@@ -677,18 +675,18 @@
             dTmax_use_kernel: float
                 Maximum temperature difference between the current temperature
                 and the temperature of the last kernel computation before
                 a new kernel is recomputed.
 
         Returns
         -------
-            H: array
+            H: array, np.ndarray
                 Heating rate in each layer (Difference of the net fluxes). Positive means heating.
                 The last value is the net flux impinging on the surface + the internal flux.
-            net: array
+            net: array, np.ndarray
                 Net fluxes at level surfaces
         """
         if (not compute_kernel) and (dTmax_use_kernel is not None):
             dT=self.tlay-self.tlay_kernel
             if np.amax(np.abs(dT)) < dTmax_use_kernel:
                 try:
                     H = self.H_kernel + np.dot(dT,self.kernel)
@@ -762,21 +760,21 @@
         ----------
             per_unit_mass: bool
                 If True, the heating rates are normalized by the
                 mass of each layer (result in W/kg).
 
         Returns
         -------
-            up: array
+            up: array, np.ndarray
                 Upward fluxes at level surfaces
-            dw: array
+            dw: array, np.ndarray
                 Downward fluxes at level surfaces
-            net: array
+            net: array, np.ndarray
                 Net fluxes at level surfaces
-            H: array
+            H: array, np.ndarray
                 Heating rate in each layer (Difference of the net fluxes). Positive means heating.
                 The last value is the net flux impinging on the surface + the internal flux.
         """
         H, net = self.flux_divergence(per_unit_mass = per_unit_mass)
         up=self.spectral_integration(self.flux_up_nu)
         dw=self.spectral_integration(self.flux_down_nu)
         return up, dw, net, H
@@ -785,22 +783,22 @@
         """Computes the transmittance profile of an atmosphere,
         i.e. Exp(-tau) for each layer of the model.
         Real work done in the numbafied function path_integral_corrk/xsec
         depending on the type of data.
         """
         self.opacity(**kwargs)
         self.compute_tangent_path()
-        self.compute_density()
+        self.compute_number_density()
         if self.Ng is not None:
             self.weights=self.k_database.weights
             transmittance=path_integral_corrk( \
-                self.Nlay-1,self.Nw,self.Ng,self.tangent_path,self.density,self.kdata,self.weights)
+                self.Nlay-1,self.Nw,self.Ng,self.tangent_path,self.n_density,self.kdata,self.weights)
         else:
             transmittance=path_integral_xsec( \
-                self.Nlay-1,self.Nw,self.tangent_path,self.density,self.kdata)
+                self.Nlay-1,self.Nw,self.tangent_path,self.n_density,self.kdata)
         return transmittance
 
     def transmission_spectrum(self, normalized=False, Rstar=None, **kwargs):
         r"""Computes the transmission spectrum of the atmosphere.
         In general (see options below), the code returns the transit depth:
 
         .. math::
@@ -836,15 +834,15 @@
                     \delta_\nu=\pi R_p^2+\alpha_\nu.
 
         Returns
         -------
             array
                 The transit spectrum (see above for normalization options).
         """
-        self.set_Rstar(Rstar)
+        if Rstar is not None: self.set_Rstar(Rstar)
         transmittance=self.transmittance_profile(**kwargs)
         self.compute_area()
         res=Spectrum((np.dot(self.area,(1.-transmittance))),self.wns,self.wnedges)
         if self.Rstar is not None:
             return (res+(PI*self.Rp**2))/(PI*self.Rstar**2)
         elif normalized:
             return res/(PI*self.Rp**2)+1
@@ -922,7 +920,28 @@
         Returns
         -------
             Spectrum object
                 Spectral flux of a bb at the temperature at the top of atmosphere (in W/m^2/cm^-1)
         """
         return self.blackbody(layer_idx=0, **kwargs)
 
+    def contribution_function(self) -> np.ndarray:
+        r"""
+        Compute the contribution function $Cf(P,\lambda) = B(T,\lambda) \frac{d e^\tau}{d \log P}$.
+
+        $\tau$ and $\log P$ are taken at the mid-layers, the temperature needs to be taken at the level surfaces.
+        For that, we use the computed temperature `t_opac[:-1]`.
+
+        The result is not normalized to allow comparison.
+        Returns
+        -------
+        : np.ndarray
+            Contribution function [W/m^2/str/cm-1].
+            Shape: **(Nlay - 1, Nw)**.
+
+        """
+        B = Bnu_integral_array(self.wnedges, self.t_opac, self.Nw,
+                               self.t_opac.shape[0]) / self.dwnedges
+        dlogP = np.diff(self.logplay)
+        detau = np.diff(self.g_integration(np.exp(-self.tau)), axis=0)
+
+        return - ((B * detau).T / dlogP).T
```

### Comparing `Exo_k-1.2.0/exo_k/atm_2band.py` & `exo_k-1.2.1/exo_k/atm_2band.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,20 +108,20 @@
 
     def spectral_integration_stellar(self, spectral_var):
         """Spectrally integrate an array, taking care of whether
         we are dealing with corr-k or xsec data.
 
         Parameters
         ----------
-            spectral_var: array
+            spectral_var: array, np.ndarray
                 array to integrate
 
         Returns
         -------
-            var: array
+            var: array, np.ndarray
                 array integrated over wavenumber (and g-space if relevant)
         """
         if self.Ng_stellar is None:
             var=np.sum(spectral_var*self.dwnedges_stellar,axis=-1)
         else:
             var=np.sum(np.sum(spectral_var*self.weights_stellar,axis=-1)*self.dwnedges_stellar,axis=-1)
         return var
@@ -266,18 +266,18 @@
         ----------
             per_unit_mass: bool
                 If True, the heating rates are normalized by the
                 mass of each layer (result in W/kg).
 
         Returns
         -------
-            H: array
+            H: array, np.ndarray
                 Heating rate in each layer (Difference of the net fluxes). Positive means heating.
                 The last value is the net flux impinging on the surface.
-            net: array
+            net: array, np.ndarray
                 Net fluxes at level surfaces
         """
         if self.flux_net_nu_stellar is None:
             raise RuntimeError('should have ran reflexion_spectrum_2stream.')
         net=self.spectral_integration_stellar(self.flux_net_nu_stellar)
         H=-np.copy(net)
         #print(H)
@@ -319,21 +319,21 @@
         ----------
             per_unit_mass: bool
                 If True, the heating rates are normalized by the
                 mass of each layer (result in W/kg).
 
         Returns
         -------
-            up: array
+            up: array, np.ndarray
                 Upward fluxes at level surfaces
-            dw: array
+            dw: array, np.ndarray
                 Downward fluxes at level surfaces
-            net: array
+            net: array, np.ndarray
                 Net fluxes at level surfaces
-            H: array
+            H: array, np.ndarray
                 Heating rate in each layer (Difference of the net fluxes). Positive means heating.
                 The last value is the net flux impinging on the surface.
         """
         H, net = self.flux_divergence_stellar(per_unit_mass = per_unit_mass)
         up=self.spectral_integration_stellar(self.flux_up_nu_stellar)
         dw=self.spectral_integration_stellar(self.flux_down_nu_stellar)
         return up, dw, net, H
```

### Comparing `Exo_k-1.2.0/exo_k/atm_evolution/atm_evol.py` & `exo_k-1.2.1/exo_k/atm_evolution/atm_evol.py`

 * *Files 3% similar despite different names*

```diff
@@ -200,15 +200,16 @@
         self.Fnet[0] = self.Fnet_rad
         for ii in range(1,5):
             self.Fnet[ii]=np.concatenate([[0.],
                 np.cumsum(self.H_ave[ii]*self.atm.dmass)[:-1]])
         self.Fnet[-1] = np.sum(self.Fnet, axis=0)
 
 
-    def evolve(self, N_timestep=1, N_kernel=10000, timestep_factor=1., dT_max = 100., verbose = False, **kwargs):
+    def evolve(self, N_timestep=1, N_kernel=10000, timestep_factor=1., dT_max=100.,
+            verbose=False, check_cons=False, **kwargs):
         r"""The time variable used in the model is tau=t/cp. 
         The equation we are solving in each layer is thus
 
         .. math::
             c_p \frac{d T}{d t}= \frac{d T}{d tau} = \sum_i H_i
 
         For a given timestep `dtau`, the physical time elapsed in second can be computed using `dt=dtau*cp`
@@ -238,14 +239,18 @@
             print('Use self.set_options(k_database=, ...)')
             raise RuntimeError('No k_database provided.')
         self.H_ave = np.zeros((6, self.Nlay))
 
         self.tlay_hist = np.zeros((N_timestep,self.Nlay))
         self.Fnet_top = np.zeros((N_timestep))
         self.timestep_hist = np.zeros((N_timestep))
+        if check_cons:
+            self.nrj_cons = np.zeros((N_timestep,self.Nlay))
+            self.vapor_cons = np.zeros((N_timestep,self.Nlay))
+            self.cond_cons = np.zeros((N_timestep,self.Nlay))
         tau0 = self.evol_tau
         self.N_last_ker = 0
         compute_kernel = False
         dTlay_max = 2. * self.settings['dTmax_use_kernel']
         self.tracers.update_gas_composition(update_vmr=True)
         for ii in range(N_timestep):
             if np.amax(np.abs(self.tlay-self.atm.tlay_kernel)) < self.settings['dTmax_use_kernel']:
@@ -264,49 +269,73 @@
                     compute_kernel=True
             self.H_tot=np.zeros(self.Nlay)
             if verbose: print('iter, compute_kernel:', ii, compute_kernel)
             if self.tracers.some_var_gases:
                 gas_vmr_rad = self.tracers.gas_vmr
             else:
                 gas_vmr_rad = None
-            self.H_rad, self.Fnet_rad = self.atm.heating_rate(compute_kernel = compute_kernel,
-                rayleigh = self.settings['rayleigh'], dTmax_use_kernel=self.settings['dTmax_use_kernel'],
-                gas_vmr = gas_vmr_rad, **kwargs)
+            aer_reffs_densities = self.tracers.update_aerosol_properties(self.atm)
+            self.H_rad, self.Fnet_rad = self.atm.heating_rate(compute_kernel=compute_kernel,
+                rayleigh=self.settings['rayleigh'], dTmax_use_kernel=self.settings['dTmax_use_kernel'],
+                gas_vmr=gas_vmr_rad, aer_reffs_densities=aer_reffs_densities, **kwargs)
 #            if verbose and compute_kernel: print('H_rad', self.H_rad)
             self.H_tot += self.H_rad
             self.timestep = timestep_factor * self.atm.tau_rad
             #if verbose: print('tau_rad, dt:', self.atm.tau_rad, self.timestep)
             self.evol_tau += self.timestep
             if self.settings['convection']:
                 self.H_conv = self.tracers.dry_convective_adjustment(self.timestep, self.H_tot, self.atm, verbose = verbose)
                 self.H_tot += self.H_conv
+                if check_cons:
+                    self.nrj_cons[ii] += self.H_conv * self.atm.dmass
             else:
                 self.H_conv = np.zeros(self.Nlay)
             if self.settings['diffusion']:
                 self.tracers.turbulent_diffusion(self.timestep, self.H_tot, self.atm, self.cp)
                 self.tracers.update_gas_composition(update_vmr=False)
             if self.settings['molecular_diffusion']:
                 self.H_diff = self.molecular_diffusion(self.timestep,
                     self.H_tot, self.atm, self.cp)
                 self.H_tot += self.H_diff
             qarray_before_condensation = np.copy(self.tracers.qarray)
             if self.settings['moist_convection']:
+                if check_cons:
+                    self.vapor_cons -= self.tracers['H2O'] * self.atm.dmass
+                    self.cond_cons -= self.tracers['H2O_liq'] * self.atm.dmass
                 self.H_madj = self.moist_convective_adjustment(self.timestep, self.H_tot,
                                     moist_inhibition=self.settings['moist_inhibition'], verbose = verbose)                
                 self.H_tot += self.H_madj
+                if check_cons:
+                    self.nrj_cons[ii] += self.H_madj * self.atm.dmass
+                    self.vapor_cons += self.tracers['H2O'] * self.atm.dmass
+                    self.cond_cons += self.tracers['H2O_liq'] * self.atm.dmass
             else:
                 self.H_madj = np.zeros(self.Nlay)
             if self.settings['condensation']:
+                if check_cons:
+                    self.vapor_cons -= self.tracers['H2O'] * self.atm.dmass
+                    self.cond_cons -= self.tracers['H2O_liq'] * self.atm.dmass
                 self.H_cond = self.condensation(self.timestep, self.H_tot, verbose = verbose)
                 self.H_tot += self.H_cond
+                if check_cons:
+                    self.nrj_cons[ii] += self.H_cond * self.atm.dmass
+                    self.vapor_cons += self.tracers['H2O'] * self.atm.dmass
+                    self.cond_cons += self.tracers['H2O_liq'] * self.atm.dmass
             else:
                 self.H_cond = np.zeros(self.Nlay)
             if self.settings['rain']:
+                if check_cons:
+                    self.vapor_cons -= self.tracers['H2O'] * self.atm.dmass
+                    self.cond_cons -= self.tracers['H2O_liq'] * self.atm.dmass
                 self.H_rain = self.rainout(self.timestep, self.H_tot, verbose = verbose)
                 self.H_tot += self.H_rain
+                if check_cons:
+                    self.nrj_cons[ii] += self.H_rain * self.atm.dmass
+                    self.vapor_cons += self.tracers['H2O'] * self.atm.dmass
+                    self.cond_cons += self.tracers['H2O_liq'] * self.atm.dmass
             else:
                 self.H_rain = np.zeros(self.Nlay)
             if self.settings['mass_redistribution']:
                 self.mass_redistribution(qarray_before_condensation)
             if self.settings['surface_reservoir']:
                 self.tracers.update_surface_reservoir(condensing_pairs_idx = self.condensing_pairs_idx,
                     surf_layer_mass = self.atm.dmass[-1])
@@ -387,21 +416,21 @@
 
         The tracer array in modified in place.
 
         Parameters
         ----------
             timestep: float
                 physical timestep of the current step (in s/cp).
-            Htot: array
+            Htot: array, np.ndarray
                 Total heating rate (in W/kg) of all physical processes
                 already computed
 
         Return
         ------
-            H_madj: array
+            H_madj: array, np.ndarray
                 Heating rate due to large scale condensation (W/kg)
         """
         new_t = self.atm.tlay + timestep * Htot
         H_madj = np.zeros(self.Nlay)
         for i_cond in range(self.Ncond): #careful i_cond is the index of the condensing pair
             # in the list of condensing species, idx_cond is the position of the
             # condensate linked to i_cond in the tracers array.
@@ -422,15 +451,15 @@
         with a constant Dmol parameter (self.Dmol in m^2/s).
 
         Parameters
         ----------
             timestep: float
                 physical timestep of the current step (in s/cp).
                 (needs to be converted before it is sent to `turbulent diffusion)
-            Htot: array
+            Htot: array, np.ndarray
                 Total heating rate (in W/kg) of all physical processes
                 already computed
             atm: :class:`Atm` object
                 The Atm object used in the radiative transfer which
                 contains many state variables. 
         """
         new_t = atm.tlay + timestep * Htot
@@ -446,21 +475,21 @@
 
         The tracer array in modified in place.
 
         Parameters
         ----------
             timestep: float
                 physical timestep of the current step (in s/cp).
-            Htot: array
+            Htot: array, np.ndarray
                 Total heating rate (in W/kg) of all physical processes
                 already computed
 
         Return
         ------
-            H_cond: array
+            H_cond: array, np.ndarray
                 Heating rate due to large scale condensation (W/kg)
         """
         new_t = self.atm.tlay + timestep * Htot
         H_cond = np.zeros(self.Nlay)
         for i_cond in range(self.Ncond): #careful i_cond is a dumy loop index, idx_cond is position of species i_cond in tracers array.
             idx_vap, idx_cond = self.condensing_pairs_idx[i_cond]
             thermo_parameters = self.condensing_species_thermo[i_cond].th_params
@@ -487,32 +516,35 @@
 
         The tracer array is modified in place.
 
         Parameters
         ----------
             timestep: float
                 physical timestep of the current step (in s/cp).
-            Htot: array
+            Htot: array, np.ndarray
                 Total heating rate (in W/kg) of all physical processes
                 already computed
 
         Return
         ------
-            H_rain: array
+            H_rain: array, np.ndarray
                 Heating rate due to re evaporation (W/kg)
         """
         new_t = self.atm.tlay + timestep * Htot
         H_rain=np.zeros(self.Nlay)
         for i_cond in range(self.Ncond):
             idx_vap, idx_cond = self.condensing_pairs_idx[i_cond]
             thermo_parameters = self.condensing_species_thermo[i_cond].th_params
             H_rain += compute_rainout_numba(timestep, self.Nlay, new_t, self.atm.play,
                 self.atm.dmass, self.cp, self.tracers.Mgas, self.tracers.qarray,
                 idx_vap, idx_cond, thermo_parameters,
-                self.settings['evap_coeff'], self.tracers.qdeep[idx_vap], verbose = verbose)
+                self.settings['evap_coeff'], self.tracers.qdeep[idx_vap],
+                q_cloud=self.settings['q_cloud'],
+                latent_heating = self.settings['latent_heating'],
+                verbose = verbose)
 
         return H_rain
 
     def compute_hybrid_coordinates(self):
         """Compute hybrid coordinates as in GCM.
 
         This will be used when surface pressure changes.
@@ -535,15 +567,15 @@
         W[k] is the mass flux between layer k-1 et k.
 
         Parameters
         ----------
             sum_dvapor_mass: float
                 Total mass of vapor added to the atmosphere
                 in the last timestep.
-            dvapor_mass: array
+            dvapor_mass: array, np.ndarray
                 mass of vapor added to each layer.
 
         For the moment, W[0] = W[Nlay]
         """
         W = np.zeros(self.Nlay+1)
         #W[0] = 0. #No mass flux between the top of the atm and space
         W[1:] = np.cumsum(self.dsigma_lev * sum_dvapor_mass - dvapor_mass)
```

### Comparing `Exo_k-1.2.0/exo_k/atm_evolution/condensation.py` & `exo_k-1.2.1/exo_k/atm_evolution/condensation.py`

 * *Files 16% similar despite different names*

```diff
@@ -47,107 +47,107 @@
         self.c2 = self.delta_cp_R * self.T_ref - self.LovR 
  
     def Lvap(self, T):
         """Latent heat at temperature T
 
         Parameters
         ----------
-            T: array
+            T: array, np.ndarray
                 Temperature in layers (K)
         """
         return Lvap_T(T, self.Latent_heat_vaporization, self.T_ref, self.delta_cp)
 
     def Psat(self, T):
         """Saturation vapor pressure for the condensing species
 
         Parameters
         ----------
-            T: array
+            T: array, np.ndarray
                 Temperature in layers (K)
         """
         return Psat_T(T, self.T_ref, self.Psat_ref, self.c1, self.c2, self.delta_cp_R)
 
     def Tsat(self, P):
         """Boiling temperature for the condensing species
 
         NOT EXACT IF DELTA CP != 0.
 
         Parameters
         ----------
-            P: array
+            P: array, np.ndarray
                 Pressure in layers (Pa)
         """
         return Tsat_P(P, self.Psat_ref, self.c1, self.c2)
 
 
     def qsat(self, psat, p, epsilon):
         """Saturation vapor mass mixing ratio for the condensing species
 
         Parameters
         ----------
-            psat: array
+            psat: array, np.ndarray
                 saturation vapor pressure
-            p: array
+            p: array, np.ndarray
                 pressure at the layer center
             epsilon: float or array
                 Ratio of the molar mass of the vapor over the background molar mass
         """
         return Qsat(psat, p, epsilon)
 
     def dPsat_dT(self, T):
         """Saturation vapor pressure derivative for the condensing species 
 
         Parameters
         ----------
-            T: array
+            T: array, np.ndarray
                 Temperature in layers (K)
         """
         return dPsat_dT(T, self.Latent_heat_vaporization, self.T_ref,
             self.Psat_ref, self.Rvap, self.delta_cp, self.delta_cp_R, self.c1, self.c2)
 
 
     def dlnPsat_dlnT(self, T):
         """Saturation vapor pressure for the condensing species and its derivative 
 
         Parameters
         ----------
-            T: array
+            T: array, np.ndarray
                 Temperature in layers (K)
         """
         return dlnPsat_dlnT(T, self.Latent_heat_vaporization, self.T_ref,
             self.delta_cp, self.Rvap)
 
 
     def moist_adiabat(self, T, P, cp, Mgas):
         """Computes the threshold thermal gradient (d ln T / d ln P) for a moist atmosphere.
 
         Parameters
         ----------
-            T: array
+            T: array, np.ndarray
                 Temperature in layers (K)
-            P: array
+            P: array, np.ndarray
                 pressure at the layer center
             cp: float
                 specific heat capacity at constant pressure of the background gas
             Mgas: float or array
                 Molar mass of the background atmosphere
         
         Returns
         -------
             array
                 Moist adiabat lapse rate
-            Lvap: array
+            Lvap: array, np.ndarray
                 Latent heat at temperature T
-            psat: array
+            psat: array, np.ndarray
                 Saturation vapor pressure for the condensing species (Pa)
-            qsat: array
+            qsat: array, np.ndarray
                 Saturation vapor mass mixing ratio for the condensing species
-            dqsat_dt: array
+            dqsat_dt: array, np.ndarray
                 Derivative of qsat with respect to temperature at fixed pressure
-            q_crit: array
+            q_crit: array, np.ndarray
                 Critical mass mixing ratio for the inhibition of moist convection
                 (Eq. 17 of Leconte et al. 2017)
 
         """
         return moist_adiabat(T, P, cp, Mgas, self.cp_vap, self.Mvap, self.Rvap,
             self.Latent_heat_vaporization, self.T_ref, self.Psat_ref,
             self.delta_cp, self.delta_cp_R, self.c1, self.c2)
@@ -155,17 +155,17 @@
 
     def compute_condensation_parameters(self, T, P, Mgas):
         """Computes necessary quantities to compute
         large scale condensation.
 
         Parameters
         ----------
-            T: array
+            T: array, np.ndarray
                 Temperature in layers (K)
-            P: array
+            P: array, np.ndarray
                 pressure at the layer center
             Mgas: float or array
                 Molar mass of the background atmosphere
         """
         return compute_condensation_parameters(T, P, Mgas, self.Mvap,
             self.Rvap, self.Latent_heat_vaporization, self.T_ref,
             self.Psat_ref, self.delta_cp, self.delta_cp_R, self.c1, self.c2)
@@ -222,52 +222,52 @@
 
 @numba.jit(nopython=True, fastmath=True, cache=True)
 def Lvap_T(T, Latent_heat_vaporization, T_ref, delta_cp):
     """Latent heat at temperature T
 
     Parameters
     ----------
-        T: array
+        T: array, np.ndarray
             Temperature in layers (K)
     """
     return Latent_heat_vaporization + delta_cp * (T-T_ref)
 
 @numba.jit(nopython=True, fastmath=True, cache=True)
 def Psat_T(T, T_ref, Psat_ref, c1, c2, delta_cp_R):
     """Saturation vapor pressure for the condensing species
 
     Parameters
     ----------
-        T: array
+        T: array, np.ndarray
             Temperature in layers (K)
     """
     return Psat_ref*np.exp( c1 + c2/T + delta_cp_R*np.log(T/T_ref))
 
 @numba.jit(nopython=True, fastmath=True, cache=True)
 def Tsat_P(P, Psat_ref, c1, c2):
     """Boiling temperature for the condensing species
 
     NOT EXACT IF DELTA CP != 0.
     
     Parameters
     ----------
-        P: array
+        P: array, np.ndarray
             Pressure in layers (Pa)
     """
     return c2/(np.log(P/Psat_ref)-c1)
 
 @numba.jit(nopython=True, fastmath=True, cache=True)
 def Qsat(psat, p, epsilon):
     """Saturation vapor mass mixing ratio for the condensing species
 
     Parameters
     ----------
-        psat: array
+        psat: array, np.ndarray
             saturation vapor pressure
-        p: array
+        p: array, np.ndarray
             pressure at the layer center
         epsilon: float or array
             Ratio of the molar mass of the vapor over the background molar mass
     """
     psat_tmp = np.core.umath.minimum(psat,p)
     fac =  p + (epsilon -1.) * psat_tmp
     qsat = epsilon * psat_tmp / fac
@@ -275,63 +275,63 @@
 
 @numba.jit(nopython=True, fastmath=True, cache=True)
 def dPsat_dT(T, Latent_heat_vaporization, T_ref, Psat_ref, Rvap, delta_cp, delta_cp_R, c1, c2):
     """Saturation vapor pressure derivative for the condensing species 
 
     Parameters
     ----------
-        T: array
+        T: array, np.ndarray
             Temperature in layers (K)
     """
     RT2 = Rvap * T * T
     Lvap = Lvap_T(T, Latent_heat_vaporization, T_ref, delta_cp)
     psat = Psat_T(T, T_ref, Psat_ref, c1, c2, delta_cp_R)
     return psat * Lvap / RT2, psat, Lvap
 
 @numba.jit(nopython=True, fastmath=True, cache=True)
 def dlnPsat_dlnT(T, Latent_heat_vaporization, T_ref, delta_cp, Rvap):
     """Saturation vapor pressure for the condensing species and its derivative
 
     Parameters
     ----------
-        T: array
+        T: array, np.ndarray
             Temperature in layers (K)
     """
     RT = Rvap * T
     Lvap = Lvap_T(T, Latent_heat_vaporization, T_ref, delta_cp)
     return Lvap / RT, Lvap
 
 @numba.jit(nopython=True, fastmath=True, cache=True)
 def moist_adiabat(T, P, cp, Mgas, cp_vap, Mvap, Rvap, Latent_heat_vaporization, T_ref, Psat_ref, delta_cp, delta_cp_R, c1, c2):
     """Computes the threshold thermal gradient (d ln T / d ln P) for a moist atmosphere.
 
     Parameters
     ----------
-        T: array
+        T: array, np.ndarray
             Temperature in layers (K)
-        P: array
+        P: array, np.ndarray
             pressure at the layer center
         cp: float
             specific heat capacity at constant pressure of the background gas
         Mgas: float or array
             Molar mass of the background atmosphere
     
     Returns
     -------
         array
             Moist adiabat lapse rate
-        Lvap: array
+        Lvap: array, np.ndarray
             Latent heat at temperature T
-        psat: array
+        psat: array, np.ndarray
             Saturation vapor pressure for the condensing species (Pa)
-        qsat: array
+        qsat: array, np.ndarray
             Saturation vapor mass mixing ratio for the condensing species
-        dqsat_dt: array
+        dqsat_dt: array, np.ndarray
             Derivative of qsat with respect to temperature at fixed pressure
-        q_crit: array
+        q_crit: array, np.ndarray
             Critical mass mixing ratio for the inhibition of moist convection
             (Eq. 17 of Leconte et al. 2017)
     """
     epsilon = Mvap / Mgas
     psat = Psat_T(T, T_ref, Psat_ref, c1, c2, delta_cp_R)
     qsat = Qsat(psat, P, epsilon)
     dlpsat_dlT, Lvap = dlnPsat_dlnT(T, Latent_heat_vaporization, T_ref, delta_cp, Rvap)
@@ -345,17 +345,17 @@
 @numba.jit(nopython=True, fastmath=True, cache=True)
 def compute_condensation_parameters(T, P, Mgas, Mvap, Rvap, Latent_heat_vaporization, T_ref, Psat_ref, delta_cp, delta_cp_R, c1, c2):
     """Computes necessary quantities to compute
     large scale condensation.
 
     Parameters
     ----------
-        T: array
+        T: array, np.ndarray
             Temperature in layers (K)
-        P: array
+        P: array, np.ndarray
             pressure at the layer center
         Mgas: float or array
             Molar mass of the background atmosphere
     """
     epsilon = Mvap / Mgas
     psat = Psat_T(T, T_ref, Psat_ref, c1, c2, delta_cp_R)
     qsat = Qsat(psat, P, epsilon)
```

### Comparing `Exo_k-1.2.0/exo_k/atm_evolution/convection.py` & `exo_k-1.2.1/exo_k/atm_evolution/convection.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,23 +20,23 @@
         timestep: float
             Duration of the adjustment.
             If given in seconds, H=dT/timestep is in K/s.
             In the current model, timestep is in second over cp.
             This ensures that H=dT/timestep is in W/kg.
         Nlay: int
             Number of atmospheric layers
-        t_lay: array
+        t_lay: array, np.ndarray
             Temperatures of the atmospheric layers (K)
-        exner: array
+        exner: array, np.ndarray
             Exner function computed at the layer centers ((p/psurf)**rcp)
 
             .. math::
               \Pi=(p / p_{s})^{R/c_p}
 
-        dmass: array
+        dmass: array, np.ndarray
             Mass of gas in each layer (kg/m^2)
 
     Returns
     -------
         array
             Heating rate in each atmospheric layer (W/kg).  
     """
@@ -129,24 +129,24 @@
         timestep: float
             Duration of the adjustment.
             If given in seconds, H=dT/timestep is in K/s.
             In the current model, timestep is in second over cp.
             This ensures that H=dT/timestep is in W/kg.
         Nlay: int
             Number of atmospheric layers
-        H_rad: array
+        H_rad: array, np.ndarray
             Radiative heating rate
-        rad_layers: array of bool
+        rad_layers: array, np.ndarray of bool
             Elements in the array are true if layer is purely radiative
-        tau_rad: array
+        tau_rad: array, np.ndarray
             Baseline radiative timescale for the atmosphere. (e.g. the min of tau_rads)
             Should use the same units as timestep.
-        tau_rads: array
+        tau_rads: array, np.ndarray
             Radiative timescale for each layer. Should use the same units as timestep.
-        dmass: array
+        dmass: array, np.ndarray
             Mass of gas in each layer (kg/m^2)
         convective_acceleration_mode: int
             convective_acceleration_mode=0 is the default mode
             =1 emulates an old (and bad) behavior.
 
     Returns
     -------
@@ -213,33 +213,33 @@
 
     Parameters
     ----------
         timestep: float
             Time step in seconds.
         Nlay: int
             Number of atmospheric layers
-        t_lay_ov_mu: array
+        t_lay_ov_mu: array, np.ndarray
             Temperatures of the atmospheric layers divided by the molar_mass in kg/mol
-        p_lay: array
+        p_lay: array, np.ndarray
             Pressure at the layer centers (Pa)
-        p_lev: array
+        p_lev: array, np.ndarray
             Presure at the Nlay+1 level boundaries (Pa)
-        dmass: array
+        dmass: array, np.ndarray
             Mass of gas in each layer (kg/m^2)
         g: float
             Gravity (m/s^2)
         Kzz: float
             Eddy mixing coefficient (m^2/s)
-        tracer_array: array (Ntrac, Nlay)
+        tracer_array: array, np.ndarray (Ntrac, Nlay)
             Array containing the mass mixing ratio of all tracers at each layer
             before the mixing
 
     Returns
     -------
-        new_tracers: array (Ntrac, Nlay)
+        new_tracers: array, np.ndarray (Ntrac, Nlay)
             Array containing the mass mixing ratio of all tracers at each layer
             after the mixing
     """
     mid_density = p_lev[1:-1]*2./(cst.RGP*(t_lay_ov_mu[1:]+t_lay_ov_mu[:-1]))
     mid_factor = - g * g * timestep * mid_density**2 / np.diff(p_lay) * 0.5*(Kzz[1:]+Kzz[:-1])
     if verbose:
         print(mid_factor)
@@ -269,33 +269,33 @@
     regions back to saturation
 
     Parameters
     ----------
         timestep
         Nlay: float
             Number of layers
-        tlay: array
+        tlay: array, np.ndarray
             Layer temperatures
         cp: float
             Specific heat capacity
-        Mgas: array
+        Mgas: array, np.ndarray
             Layer molar mass
-        qarray: array
+        qarray: array, np.ndarray
             Array of tracer specific concentrations
         idx_vap, idx_cond: int
             Indices for condensing species in tracer array
-        thermo_parameters: array
+        thermo_parameters: array, np.ndarray
             Array of thermodynamical paramaters for condensing species.
             See `:class:`~exo_k.atm_evolution.condensation.Condensation_Thermodynamical_Parameters`
         latent_heating: bool
             Whether latent heating should be taken into account
 
     Returns
     -------
-        H_cond: array
+        H_cond: array, np.ndarray
             Heating rate in W/kg
     """
     itermax = 1000
     if condensation_timestep_reducer is None:
         alpha = 1.
     else:
         alpha = condensation_timestep_reducer
@@ -328,14 +328,15 @@
 
     else:
         # here we treat whole arrays at once.
         Lvap, qsat, dqsat_dt = compute_condensation_parameters(tlay, play, Mgas, 
                 thermo_parameters[1], thermo_parameters[2], thermo_parameters[3], thermo_parameters[4],
                 thermo_parameters[5], thermo_parameters[6], thermo_parameters[7], thermo_parameters[8],
                 thermo_parameters[9])
+        qvap = qarray[idx_vap]
         dqvap= np.where(qsat <= qvap, qsat-qvap, 0.)
         qarray[idx_vap] += dqvap
         qarray[idx_cond] -= dqvap
         if verbose: print('in cond, RH, T:', qarray[idx_vap]/qsat, tlay, dqsat_dt)
     return H_cond
 
 @numba.jit(nopython=True, fastmath=True, cache=True)
@@ -346,49 +347,49 @@
     of a given atmosphere to a moist adiabat.
 
     Parameters
     ----------
         timestep
         Nlay: float
             Number of layers
-        tlay: array
+        tlay: array, np.ndarray
             Layer temperatures
         play:array
             Pressure at layer centers
-        dmass: array
+        dmass: array, np.ndarray
             mass of layers in kg/m^2
         cp: float
             specific heat capacity at constant pressure
-        q_array: array
+        q_array: array, np.ndarray
             mass mixing ratio of tracers
         i_vap: int
             index of vapor tracer in qarray
         i_cond: int
             index of condensate tracer in qarray
-        qsat: array
+        qsat: array, np.ndarray
             Saturation mmr for each layer
-        dqsat_dt: array
+        dqsat_dt: array, np.ndarray
             d qsat / dT in each layer
-        Lvap: array
+        Lvap: array, np.ndarray
             Latent heat of vaporization (can have different values
             in each layer if Lvap=f(T))
-        dlnt_dlnp_moist: array
+        dlnt_dlnp_moist: array, np.ndarray
             threshold thermal gradient (d ln T / d ln P) for a moist atmosphere
             computed at the layer centers.
-        q_crit: array
+        q_crit: array, np.ndarray
             Critical mass mixing ratio for the inhibition of moist convection
             (Eq. 17 of Leconte et al. 2017)
 
     Returns
     -------
-        H_madj: array
+        H_madj: array, np.ndarray
             Heating rate in each atmospheric layer (W/kg). 
-        new_q: array
+        new_q: array, np.ndarray
             tracer mmr array after adjustment.
-        new_t: array
+        new_t: array, np.ndarray
             Temperature of layers after adjustment. 
     """
     if verbose: print('enter moist adj')
     H_madj=np.zeros(Nlay)
     new_q = q_array.copy()
     new_t = tlay.copy()
     dp = np.diff(play)
@@ -451,16 +452,16 @@
             int_m_cond = tmp_int_m_cond
             C = tmp_C
             B = tmp_B
             m_cond = tmp_m_cond
             i_bot += 1
             continue
         else:
-            i_bot -= 1
             break
+    i_bot -= 1
     if verbose: print('it,ib=', i_top, i_bot)
     if i_top == i_bot: # need at least 2 layers to convect, so exit
         return H_madj, new_q, new_t
     new_Ttop = B / C
     if verbose: print(new_Ttop, m_cond, dT_moist)
     dT = new_Ttop - new_t[i_top]
     qvap[i_top] = qsat[i_top] + dqsat_dt[i_top] * dT
@@ -485,49 +486,52 @@
     new_q[i_cond, i_top:i_bot+1] += m_cond / m_conv
     if verbose: 
         print('m_cond, m_conv, m_cond2', m_cond, m_conv, m_cond_2)
     return H_madj, new_q, new_t
 
 @numba.jit(nopython=True, fastmath=True, cache=True)
 def compute_rainout_numba(timestep, Nlay, tlay, play, dmass, cp, Mgas, qarray,
-        idx_vap, idx_cond, thermo_parameters, evap_coeff, qvap_deep,
+        idx_vap, idx_cond, thermo_parameters, evap_coeff, qvap_deep, q_cloud=0.,
+        latent_heating=False,
         verbose = False):
     r"""Computes the heating rates needed to adjust unstable regions 
     of a given atmosphere to a moist adiabat.
 
     Parameters
     ----------
         timestep
         Nlay: float
             Number of layers
-        tlay: array
+        tlay: array, np.ndarray
             Layer temperatures
     """
     H_rain=np.zeros(Nlay)
     Lvap, qsat, dqsat_dt = compute_condensation_parameters(tlay, play, Mgas, 
             thermo_parameters[1], thermo_parameters[2], thermo_parameters[3], thermo_parameters[4],
             thermo_parameters[5], thermo_parameters[6], thermo_parameters[7], thermo_parameters[8],
             thermo_parameters[9])
-
+    if not latent_heating:
+        Lvap = Lvap * 0.
     Tsat_p = Tsat_P(play, thermo_parameters[5], thermo_parameters[8], thermo_parameters[9])
 
-    if verbose: print('in rainout, RH, T:', qarray[idx_vap]/qsat, tlay)
+    if verbose: print('in rainout, RH, T, qice:', qarray[idx_vap]/qsat,  tlay, qarray[idx_cond])
     mass_cond = 0.
     for i_lay in range(Nlay):
         #  if evap_coeff =1, rain vaporisation in an undersaturated layer can fill the layer up to the (estimated) saturation
         #  if 0 < evap_coeff < 1, rain vaporisation in one layer is limited to a fraction of the amount that would saturate the layer
         #  This allows not to exceed saturation, to spread rain vaporization in more and denser layers
         qvap = qarray[idx_vap,i_lay]
         if (tlay[i_lay] >= Tsat_p[i_lay]): # above boiling temperature, try to evaporate everything
             dqvap = (qsat[i_lay] - qvap) / (1. + Lvap[i_lay]*dqsat_dt[i_lay]/cp)
         else:
             dqvap = evap_coeff * (qsat[i_lay] - qvap) / (1. + Lvap[i_lay]*dqsat_dt[i_lay]/cp)
         dqvap = np.core.umath.minimum(dqvap, 1.- qvap)
-        mass_cond += qarray[idx_cond,i_lay]*dmass[i_lay]
-        qarray[idx_cond,i_lay] = 0.
+        if qarray[idx_cond,i_lay]>=q_cloud:
+            mass_cond += (qarray[idx_cond,i_lay] - q_cloud) * dmass[i_lay]
+            qarray[idx_cond,i_lay] = q_cloud
         # dqvap is the change in vapor content to reach saturation and accounting for the temperature change.
         # dqvap < 0 implies condensation, meaning that there is a remaining excess of vapor after the previous 
         # condensation step. In such case we apply this new change in vapor content and temperature and
         # increase the amount of falling condensed species (mass_cond).
         # dqvap > 0 implies evaporation. Here there are two possibilities:
         #   - the amount of condensates is lower than dqvap. All condensates are vaporised in the layer
         #    and the tempertaure change is -Ldqv/cp where dqv is the actual change in vapor.
@@ -547,14 +551,15 @@
                 mass_cond = 0.
             else:
                 if verbose: print('mass_dvap < mass_cond:', i_lay, dqvap, qvap, mass_cond, mass_cond/dmass[i_lay])
                 qarray[idx_vap,i_lay] += dqvap
                 H_rain[i_lay] = -Lvap[i_lay]*dqvap/(cp*timestep)
                 mass_cond -= dqvap*dmass[i_lay]
     if mass_cond != 0.:
+        if verbose: print('mass_cond=',mass_cond)
         qarray[idx_cond,-1]+= mass_cond/dmass[-1]
         # Issue : qarray[idx_cond,-1] sometimes can become large (when starting with a hot atmosphere dominated with H2O that cools to saturation)
     if qvap_deep>=0.:
         qarray[idx_vap,-1] = qvap_deep
     return H_rain
 
 
@@ -578,30 +583,30 @@
 
     Parameters
     ----------
         timestep: float
             Time step in seconds.
         Nlay: int
             Number of atmospheric layers
-        t_lay_ov_mu: array
+        t_lay_ov_mu: array, np.ndarray
             Temperatures of the atmospheric layers divided by the molar_mass in kg/mol
-        p_lay: array
+        p_lay: array, np.ndarray
             Pressure at the layer centers (Pa)
-        p_lev: array
+        p_lev: array, np.ndarray
             Presure at the Nlay+1 level boundaries (Pa)
-        dmass: array
+        dmass: array, np.ndarray
             Mass of gas in each layer (kg/m^2)
         g: float
             Gravity (m/s^2)
         Dmol: float
             molecular diffusion coefficient (m^2/s)
 
     Returns
     -------
-        new_tlay: array (Nlay)
+        new_tlay: array, np.ndarray (Nlay)
             Array containing the temperature at each layer
             after the mixing
     """
     mid_density = p_lev[1:-1]*2.*(mu[1:]+mu[:-1])/(cst.RGP*(tlay[1:]+tlay[:-1]))
     mid_factor = - g * g * timestep * mid_density**2 / np.diff(p_lay) * Dmol
     if verbose:
         print(mid_factor)
```

### Comparing `Exo_k-1.2.0/exo_k/atm_evolution/settings.py` & `exo_k-1.2.1/exo_k/atm_evolution/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,33 +26,32 @@
                         'latent_heating': True,
                         'moist_convection': False,
                         'moist_inhibition': False,
                         'surface_reservoir': False,
                         'mass_redistribution': False,
                         'compute_mass_fluxes': True,
                         'dTmax_use_kernel': 10.,
-                        'qvap_deep': -1.,
                         'evap_coeff': 1.,
                         'acceleration_mode': 0,
                         'radiative_acceleration_reducer': 1.,
                         'condensation_timestep_reducer': .8,
                         'convective_acceleration_mode': 0,
                         'qcond_surf_layer': 0.1,
+                        'q_cloud': 0.,
                         }
             
         self._forbidden_changes = ['logplay', 'play']
 
         self._non_radiative_parameters = set(self.parameters.keys())
 
     def set_parameters(self, **kwargs):
         """Sets various global options
         """
         for key, val in kwargs.items():
-            if val is not None:
-                self.parameters[key]=val
+            self.parameters[key]=val
         if 'logplay' in self.keys():
             self['Nlay']=self['logplay'].size
 
     def use_or_set(self, key, value):
         """Returns the value stored in the parameters if available.
         Stores the given value if not. 
         """
```

### Comparing `Exo_k-1.2.0/exo_k/atm_profile.py` & `exo_k-1.2.1/exo_k/atm_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 
     The derived class :class:`~exo_k.atm.Atm` handles
     radiative transfer calculations.
 
     """
     
     def __init__(self, composition=None, psurf=None, ptop=None, logplay=None, tlay=None,
-            Tsurf=None, Tstrat=None, grav=None, Rp=None, Mgas=None, rcp=None, Nlay=20,
-            logplev=None, aerosols=None,
+            Tsurf=None, Tstrat=None, grav=None, Rp=None, Mgas=None, Rstar=None,
+            rcp=None, Nlay=20, logplev=None, aerosols=None,
             ## old parameters that should be None. THey are left here to catch
             ## exceptions and warn the user that their use is obsolete
             Nlev=None, tlev=None,
             **kwargs):
         """Initializes atmospheric profiles
 
         Parameters
@@ -61,16 +61,16 @@
         * Tstrat: float
           Stratospheric temperature        
 
         This way you will have an adiabatic atmosphere with Tsurf at the ground that
         becomes isothermal wherever T=<Tstrat.
         You can also specify:
 
-        * logplay or play: array
-        * tlay: array (same size)
+        * logplay or play: array, np.ndarray
+        * tlay: array, np.ndarray (same size)
           These will become the pressures (Pa; the log10 if you give
           logplay) and temperatures of the layers.
           This will be used to define the surface and top pressures.
           Nlay becomes the size of the arrays. 
 
         .. warning::
             Layers are counted from the top down (increasing pressure order).
@@ -99,28 +99,29 @@
             self.compute_pressure_levels()
             self.set_adiab_profile(Tsurf=Tsurf, Tstrat=Tstrat)
         else:
             self.set_logPT_profile(logplay, tlay, logplev=logplev)
         self.set_Rp(Rp)        
         self.set_grav(grav)
         self.set_Mgas(Mgas=Mgas)
+        self.set_Rstar(Rstar=Rstar)
 
     def set_logPT_profile(self, logplay, tlay, logplev=None):
         """Set the logP-T profile of the atmosphere with a new one
 
         Parameters
         ----------
-            logplay: array
+            logplay: array, np.ndarray
                 Log pressure (in Pa) of the layer
-            tlay: array (same size)
+            tlay: array, np.ndarray (same size)
                 temperature of the layers.
         
         Other Parameters
         ----------------
-            logplev: array (size Nlay+1)
+            logplev: array, np.ndarray (size Nlay+1)
                 If provided, allows the user to choose the location
                 of the level surfaces separating the layers.
         """
         self.logplay=np.array(logplay, dtype=float)
         self.Nlay=self.logplay.size
         self.Nlev=self.Nlay+1
         if logplev is not None:
@@ -175,15 +176,15 @@
 
         self.logp_opac=self.logplev[1:-1]
         self.psurf=self.plev[-1]
         self.dp_lay=np.diff(self.plev) ### probably redundant with dmass
         self.exner=(self.play/self.psurf)**self.rcp
         self.compute_layer_masses()
 
-    def update_pressure_profile(self, play = None, plev = None):
+    def update_pressure_profile(self, play=None, plev=None):
         """Updates pressure levels without changing temperatures.
         
         To be used Atm_evolution class.
         """
         play = np.array(play, dtype=float)
         if play.size != self.Nlay:
             raise RuntimeError("You cannot change the number of layers in update_pressure_profile")
@@ -262,14 +263,15 @@
                 tmp_vmr=np.array(vmr)
                 # geometrical average:
                 with np.errstate(invalid='raise'):
                     try:
                         vmr_midlevel_dict[mol] = np.sqrt(tmp_vmr[1:]*tmp_vmr[:-1])
                     except FloatingPointError:
                         print('inset_gas, mol, tmp_vmr=',mol,tmp_vmr)
+                        print(composition_dict)
                         vmr_midlevel_dict[mol] = tmp_vmr[1:]
             else:
                 vmr_midlevel_dict[mol] = vmr
         if self.gas_mix is None:
             self.gas_mix = Gas_mix(vmr_midlevel_dict)
         else:
             self.gas_mix.set_composition(vmr_midlevel_dict)
@@ -286,14 +288,17 @@
         """
         if Mgas is not None:
             self.Mgas_rad=Mgas
         else:
             self.Mgas_rad=self.gas_mix.molar_mass()
         if not isinstance(self.Mgas_rad, np.ndarray):
             self.Mgas_rad=self.Mgas_rad*np.ones(self.Nlay-1, dtype=float)
+        else:
+            if (self.Mgas_rad.size != self.Nlay-1) :
+                self.Mgas_rad = 0.5 * (self.Mgas_rad[1:] + self.Mgas_rad[:-1])
 
     def set_rcp(self, rcp = None):
         """Sets the adiabatic index of the atmosphere
 
         Parameters
         ----------
             rcp: float
@@ -356,25 +361,31 @@
             self.Rstar = None
             return
         if isinstance(Rstar,u.quantity.Quantity):
             self.Rstar=Rstar.to(u.m).value
         else:
             self.Rstar=Rstar
 
-    def compute_density(self):
+    def compute_number_density(self):
         """Computes the number density (m^-3) profile of the atmosphere
         in the radiative layers
         """
-        self.density=np.power(10., self.logp_opac)/(KBOLTZ*self.t_opac)
+        self.n_density = np.power(10., self.logp_opac)/(KBOLTZ*self.t_opac)
+
+    def compute_mass_density(self):
+        """Computes the mass density (kg/m^-3) profile of the atmosphere
+        in the radiative layers
+        """
+        self.mass_density = np.power(10., self.logp_opac)*self.Mgas_rad/(RGP*self.t_opac)
 
     def compute_layer_col_density(self):
         """Computes the column number density (molecules/m^2) per
         radiative layer of the atmosphere.
 
-        There are Nlay-1 radiative layers as they go from the midle of a layer to the next.
+        There are Nlay-1 radiative layers as they go from the middle of a layer to the next.
         """
         factor=N_A/(self.grav * self.Mgas_rad)
         self.dcol_density_rad = np.diff(self.play)*factor[:]
 
         if self.Rp is not None: #includes the altitude effect if radius is known
             self.compute_altitudes()
             self.dcol_density_rad*=(1.+self.zlev[1:-1]/self.Rp)**2
@@ -466,29 +477,32 @@
             if invert_p: ax.invert_yaxis()
             ax.set_ylabel('Pressure (Pa)')
         ax.set_xlabel('Temperature (K)')
         if xscale is not None: ax.set_xscale(xscale)
         if yscale is not None: ax.set_yscale(yscale)
 
 
-    def write_soundings(self, dirname='.', fmt='%.10e', cp=None, qvap=None, p_dry=None):
+    def write_soundings(self, dirname='.', fmt='%.10e', cp=None, qvap=None, p0=None, p_dry=None):
         """Writes sounding files that can be used to initiate the mesoscale model
         """
         self.compute_altitudes()
         mgas = np.zeros(self.Nlay)
         mgas[:-1] = self.Mgas_rad
         mgas[-1] = self.Mgas_rad[-1]
         r = RGP/mgas
         rho_lay = self.play/(r*self.tlay)
         if cp is not None:
             cp_array = cp * np.ones(self.Nlay)
         else:
             cp_array =  r / self.rcp
         zeros=np.zeros(self.Nlay)
-        teta = self.tlay / self.exner
+        if p0 is None:
+            teta = self.tlay / self.exner
+        else:
+            teta = self.tlay * (p0 / self.play)**(self.rcp)
         if qvap is not None:
             q=qvap
         else:
             q=zeros
         filename=dirname+'/input_sounding'
         np.savetxt(filename, np.transpose([self.zlay[::-1], teta[::-1], q[::-1], zeros ,zeros]),
             fmt=fmt, header=str(self.psurf/100.)+'  '+str(self.tlay[-1])+'    0.0', comments=' ')
```

### Comparing `Exo_k-1.2.0/exo_k/chemistry.py` & `exo_k-1.2.1/exo_k/chemistry.py`

 * *Files identical despite different names*

```diff
@@ -181,17 +181,17 @@
     def compute_vmr(self, molecule = None, logp_array = None, t_array = None):
         """
 
         Parameters
         ----------
             molecule: str
                 Name of molecule to deal with
-            logp_array: array
+            logp_array: array, np.ndarray
                 Array of log10 pressures (Pa)
-            t_array: array
+            t_array: array, np.ndarray
                 Array of temperatures (K)
 
         """
         if (molecule is None) or (logp_array is None) or (t_array is None):
             raise RuntimeError('Missing keyword argument.')
         logp_array=np.array(logp_array, dtype=float)
         t_array=np.array(t_array, dtype=float)
```

### Comparing `Exo_k-1.2.0/exo_k/cia_table.py` & `exo_k-1.2.1/exo_k/cia_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,23 +84,20 @@
         if self.abs_coeff is not None:
             if self._settings._convert_to_mks or mks: self.convert_to_mks()
             if remove_zeros : self.remove_zeros(deltalog_min_value = deltalog_min_value)
 
     def _init_empty(self):
         """Initializes attributes to none.
         """
+        super().__init__()
         self.mol1=None
         self.mol2=None
-        self.wns=None
-        self.wnedges=None
         self.tgrid=None
         self.abs_coeff=None
         self.abs_coeff_unit='unspecified'
-        self.wn_unit='cm^-1'
-        self.Nt=None
         self.Nw=None
         self.filename=None
 
 
     def read_hitran_cia(self, filename, old_cia_unit='cm^5'):
         """Reads hitran cia files and load temperature, wavenumber, and absorption coefficient grid.
 
@@ -249,15 +246,15 @@
 
 
     def sample(self, wngrid, remove_zeros=False, use_grid_filter=False, **kwargs):
         """Method to re sample a cia table to a new grid of wavenumbers (inplace).
 
         Parameters
         ----------
-            wngrid : array
+            wngrid : array, np.ndarray
                 new wavenumber grid (cm-1)
             use_grid_filter: boolean, optional
                 If true, the table is sampled only within the boundaries
                 of its current wavenumber grid. The coefficients are set to zero elswere
                 (except if remove_zeros is set to True).
                 If false, the values at the boundaries are used when sampling outside the grid.
         """
@@ -299,15 +296,15 @@
         """interpolate_cia interpolates the kdata at on a given temperature profile.
 
         Parameters
         ----------
             t_array: float or array
                 Temperature array to interpolate to.
                 If a float is given, it is interpreted as an array of size 1.
-            wngrid_limit: array, optional
+            wngrid_limit: array, np.ndarray, optional
                 If an array is given, interpolates only within this array.
             log_interp: bool, optional
                 Whether the interpolation is linear in kdata or in log(kdata).
 
         Returns
         -------
             array of shape (logp_array.size, self.Nw)
@@ -356,15 +353,15 @@
         ----------
             logP: float or array
                 Log10 of the pressure (Pa).
             T: float or array
                 Temperature (K).
             x_mol1/2: float or array
                 Volume mixing ratio of the 1st and 2nd molecule of the pair.
-            wngrid_limit: array, optional
+            wngrid_limit: array, np.ndarray, optional
                 If an array is given, interpolates only within this array.
 
         Returns
         -------
             float or array
                 total cross section for the molecule pair in m^2 per total number of molecules.
         """
```

### Comparing `Exo_k-1.2.0/exo_k/ciadatabase.py` & `exo_k-1.2.1/exo_k/ciadatabase.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,17 +39,16 @@
 
         The default path searched is set with :func:`exo_k.settings.Settings.set_cia_search_path`
         or :func:`~exo_k.settings.Settings.add_cia_search_path`.
         A local search path can be specified with the `search_path` keyword.
 
         See the options of :class:`~exo_k.cia_table.Cia_table` __init__ method.
         """
+        super().__init__()
         self.cia_tables={}
-        self.wns=None
-        self.Nw=None
         self.abs_coeff_unit=None
         if filenames is not None:
             for filename in filenames:
                 tmp_cia_table=Cia_table(*([filename]+list(str_filters)),
                     remove_zeros=remove_zeros, **kwargs)
                 self.add_cia_tables(tmp_cia_table)
         elif molecule_pairs is not None:
@@ -127,15 +126,15 @@
 
     def sample(self, wngrid, remove_zeros=False, use_grid_filter=False):
         """Samples all the cia_table in the database on the same wavenumber grid
         to be able to use them in radiative transfer modules (inplace).
 
         Parameters
         ----------
-            wngrid : array
+            wngrid : array, np.ndarray
                 new wavenumber grid (cm-1)
 
         .. seealso::
             See :func:`exo_k.cia_table.Cia_table.sample for further details on options.
 
         """
         for mol1 in self.cia_tables.values():
@@ -159,23 +158,23 @@
     def cia_cross_section(self, logP_array, T_array, gas_comp,
         wngrid_limit=None, Nw=None):
         """Computes the absorption coefficient in m^-1 for the whole mix specified 
         (assumes data in MKS).
 
         Parameters
         ----------
-            logP_array: array
+            logP_array: array, np.ndarray
 
-            T_array: array
+            T_array: array, np.ndarray
                 log10 Pressure (Pa) and temperature profiles
 
             gas_comp: :class:`~exo_k.gas_mix.Gas_mix` object
                 behaves like a dict with mol names as keys and vmr as values.
 
-            wngrid_limit: array, optional
+            wngrid_limit: array, np.ndarray, optional
                 Smaller and bigger wavenumbers inside which to perform the calculation.
 
         Returns
         -------
             array:
                 The cia effective cross section coefficient profile for the whole gas (in m^2).
 
@@ -222,15 +221,15 @@
 
             T_array: 1d array
                 log10 Pressure (Pa) and temperature grids
 
             gas_comp: :class:`~exo_k.gas_mix.Gas_mix` object
                 behaves like a dict with mol names as keys and vmr as values.
 
-            wngrid_limit: array, optional
+            wngrid_limit: array, np.ndarray, optional
                 Smaller and bigger wavenumbers inside which to perform the calculation.
 
         Returns
         -------
             array:
                 The cia effective cross section coefficient profile for the whole gas (in m^2).
```

### Comparing `Exo_k-1.2.0/exo_k/data_table.py` & `exo_k-1.2.1/exo_k/data_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,41 +23,38 @@
     __array_priority__=1000
     # this allows __rmul__ to take precedence over numpy array broadcasting in multiplications
     # See https://stackoverflow.com/questions/40694380/
     # forcing-multiplication-to-use-rmul-instead-of-numpy-array-mul-or-byp/44634634#44634634
 
     def __init__(self):
         """Initializes all attributes to `None`"""
+        super().__init__()
         self.filename=None
         self.mol=None
         self.isotopolog_id=0
         self.pgrid=None
         self.logpgrid=None
         self.tgrid=None
-        self.wns=None
-        self.wnedges=None
         self.kdata=None
         self.logk=None
         self.Np=None
         self.Nt=None
-        self.Nw=None
         self.Ng=None   # If the table is for xsec, Ng will stay at None.
                        # This will allow us to differentiate xsec from corrk
                        # when needed in the interpolation routines.
                        # Especially to reshape the output.
         self.DOI='unknown'
         self.sampling_method='unknown'
         version = pkg_resources.require("exo_k")[0].version
         self.Date_ID='exo_k-v'+version+'-'+date.today().strftime("%d/%m/%Y")
         self.Nx=None   # If we are dealing with a Qtable with a variable gas, Nx is the size of the
                        # grid along the dimension of the Volume mixing ratio of the variable gas.
                        # A None value means that we have either a regular Ktable or a Xtable.
         self.p_unit='unspecified'
         self.kdata_unit='unspecified'
-        self.wn_unit='cm^-1'
         self._settings=Settings()
 
     def finalize_init(self, p_unit='unspecified', file_p_unit='unspecified',
         kdata_unit='unspecified', file_kdata_unit='unspecified',
         remove_zeros=False):
         """Common code at the end of the initialization of
         inheriting classes put here to avoid duplicates
@@ -176,17 +173,17 @@
         """interpolate_kdata interpolates the kdata at on a given temperature and
         log pressure profile. If a volume mixing ratio profile (`x_array`) is given,
         the cross section computed for the species is multiplied by `x_array` to account for the
         'dilution' of the opacity.
 
         Parameters
         ----------
-            logp_array: array
+            logp_array: array, np.ndarray
                 log 10 pressure array to interpolate to
-            t_array: array, same size as logp_array
+            t_array: array, np.ndarray, same size as logp_array
                 Temperature array to interpolate to
             x_array: None
                 Volume mixing ratio array used to renormalize the cross section.
 
         If floats are given, they are interpreted as arrays of size 1.
 
         Other Parameters
@@ -479,15 +476,15 @@
 
     def set_kdata(self, new_kdata):
         """Changes kdata (inplace). this is preferred to directly accessing kdata because this
         method checks that the array has the right dimensions
 
         Parameters
         ----------
-            new_kdata: array
+            new_kdata: array, np.ndarray
                 New array of kdata.
         """
         if not isinstance(new_kdata,np.ndarray):
             new_kdata=np.array(new_kdata)
         sh=np.array(new_kdata.shape)
         if sh.size != self.shape.size:
             raise RuntimeError('new_kdata does not have the right number of dimensions')
@@ -514,17 +511,17 @@
             wnedges_left=None, wnedges_right=None,
             remove_zeros=False):
         """Extends the spectral range of an existing table (inplace).
         The new bins are filled with zeros (except if remove_zeros=True)
 
         Parameters
         ----------
-            wngrid_left: array
+            wngrid_left: array, np.ndarray
                 Array of wavenumbers to add to the small wn end of the table.
-            wngrid_right: array
+            wngrid_right: array, np.ndarray
                 Array of wavenumbers to add to the high wn end of the table.
 
         .. warning::
             There should not be any overlap between wngrid_left, wngrid_right,
             and the current wavenumber grid of the table.
 
         Other Parameters
@@ -631,36 +628,18 @@
 
     @property
     def molar_mass(self):
         """Computes molar mass from molecule name
         """
         return Molar_mass().fetch(self.mol)
 
-    def blackbody(self, Temperature, integral=True):
-        """Computes the surface black body flux (in W/m^2/cm^-1) at Temperature.
-
-        Parameters
-        ----------
-            Temperature; float
-                Blackbody temperature
-            integral: boolean, optional
-                * If true, the black body is integrated within each wavenumber bin.
-                * If not, only the central value is used.
-                  False is faster and should be ok for small bins,
-                  but True is the correct version.
-        Returns
-        -------
-            Spectrum object
-                Spectral flux in W/m^2/cm^-1
+    def blackbody(self, Temperature, **kwargs):
+        """See Spectral_object.blackbody
         """
-        if integral:
-            piB=PI*Bnu_integral_num(self.wnedges, Temperature)/np.diff(self.wnedges)
-        else:
-            piB=PI*Bnu(self.wns[:], Temperature)
-        return Spectrum(piB,self.wns,self.wnedges)
+        return Spectrum(super().blackbody(Temperature, **kwargs), self.wns, self.wnedges)
 
     def write_hdf5_common(self, f, compression="gzip", compression_level=9,
         p_unit=None):
         """Method that writes datasets and attributes that are common to
         X and Ktables.
 
         Parameters
```

### Comparing `Exo_k-1.2.0/exo_k/gas_mix.py` & `exo_k-1.2.1/exo_k/gas_mix.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,21 +21,19 @@
 
     def __init__(self, composition=None, logp_array=None, t_array=None,
         k_database=None, cia_database=None):
         """__init_ Instantiates
         a Gas_mix object and computes the vmr of the 'background' gas.
         """
         if composition is None: composition=dict()
+        super().__init__()
         self.Narray=None
         self._wn_range=None
         self.iw_min=None
         self.iw_max=None
-        self.wns=None
-        self.wnedges=None
-        self.Nw=None
         self.need_to_recompute_vmr_array = True
 
         self.set_composition(composition)
         self.set_logPT(logp_array=logp_array, t_array=t_array)
         self.set_k_database(k_database)
         self.set_cia_database(cia_database)
 
@@ -135,15 +133,16 @@
         vmr_active_gases=0.
 
         for mol,vmr in self.composition.items():
             if mol!='inactive_gas':
                 Mmol=Molar_mass().fetch(mol)
                 mol_mass_active_gases+=vmr*Mmol
                 vmr_active_gases+=vmr
-        mol_mass=mol_mass_active_gases/vmr_active_gases     
+
+        mol_mass=mol_mass_active_gases/vmr_active_gases
         return mol_mass
 
     def cp(self):
         """Computes and returns the specific heat capacity (cp)
         of a mix of gases
 
         Returns
@@ -315,38 +314,14 @@
                 but beware that this global setting is overridden by local options
                 specified during the loading.
                 You will have to reload all your data though.
                 (A good thing it does not take so long). """)
 
                 raise RuntimeError("Bad units in the CIAdatabase used with Gas_mix.")
 
-    def _compute_spectral_range(self, wn_range=None, wl_range=None):
-        """Converts an unordered spectral range in either wavenumber or wavelength
-        in an ordered wavenumber range.
-
-        Parameters
-        ----------
-            wn_range: list or array of size 2
-                Minimum and maximum wavenumber (in cm^-1).
-            wl_range: list or array of size 2
-                Minimum and maximum wavelength (in micron)
-        """
-        if wl_range is not None:
-            if wn_range is not None:
-                print('Cannot specify both wl and wn range!')
-                raise RuntimeError()
-            else:
-                _wn_range=np.sort(10000./np.array(wl_range))
-        else:
-            if wn_range is not None:
-                _wn_range=np.sort(np.array(wn_range))
-            else:
-                _wn_range=self._wn_range
-        return _wn_range
-
     def set_spectral_range(self, wn_range=None, wl_range=None):
         """Sets the default spectral range in which computations will be done by specifying
         either the wavenumber or the wavelength range.
 
         Parameters
         ----------
             wn_range: list or array of size 2
@@ -369,33 +344,34 @@
         else:
             self.iw_min, self.iw_max = np.where((self.k_database.wnedges > local_wn_range[0]) \
                 & (self.k_database.wnedges <= local_wn_range[1]))[0][[0,-1]]
             # to be consistent with interpolate_kdata
 
     def cross_section(self, composition=None, logp_array=None, t_array=None,
             wl_range=None, wn_range=None, rayleigh=True,
-            write=0, random_overlap=False, logp_interp=True, use_basic_molecules=False, **kwargs):
+            write=0, random_overlap=False, logp_interp=True, use_basic_molecules=False,
+            inactive_molecules=None, **kwargs):
         """Computes the cross section (m^2/total number of molecule) for the mix
         at each of the logPT points as a function of wavenumber (and possibly g point).
 
         Parameters
         ----------
-            wl_range: array or list of two values, optional
+            wl_range: array, np.ndarray or list of two values, optional
                 Wavelength range to cover.
-            wn_range: array or list of two values, optional
+            wn_range: array, np.ndarray or list of two values, optional
                 Wavenumber range to cover.
             rayleigh: boolean, optional
                 Whether to compute rayleigh scattering.
             random_overlap: boolean, optional
                 Whether Ktable opacities are added linearly (False),
                 or using random overlap method (True).
 
         Returns
         -------
-            kdata_array: array
+            kdata_array: array, np.ndarray
                 Cross section array of shape (layer number, Nw (, Ng if corrk)).
 
         After every computation, the following variables are updated to account for any possible
         change in spectral range:
 
           * self.Nw, Number of wavenumber bins
           * self.wns, Wavenumber array
@@ -423,14 +399,18 @@
             self.need_to_recompute_vmr_array = False
             if write>6 :
                 print('recomputed vmr array:', self.vmr_arr_base_mol, self.vmr_arr) 
         if use_basic_molecules:
             molecs=self.vmr_arr_base_mol.keys()
         else:
             molecs=self.vmr_arr.keys()
+        if inactive_molecules is not None:
+            molecs = list(molecs)
+            for inac_mol in inactive_molecules:
+                molecs.remove(inac_mol)
         if write>6 :
             print('molecs:', molecs) 
         mol_to_be_done=list(set(molecs).intersection(self.k_database.molecules))
         if not mol_to_be_done:
             if 'total' in self.k_database.molecules:
                 #special case where you have one ktable that describes the whole gas.
                 mol_to_be_done=['total']
```

### Comparing `Exo_k-1.2.0/exo_k/hires_spectrum.py` & `exo_k-1.2.1/exo_k/hires_spectrum.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 @author: jeremy leconte
 """
 import os.path
 import numpy as np
+import pandas as pd
 import h5py
 from exo_k.util.interp import rm_molec,unit_convert
 from exo_k.settings import Settings
 from exo_k.util.filenames import select_kwargs
 from .util.spectral_object import Spectral_object
 from .util.cst import KBOLTZ, N_A
 
@@ -33,23 +34,25 @@
             mult_factor: float
                 A multiplicative factor that can be applied to kdata (for example to correct for
                 any dilution effect, or specific conversion).
         
         see :func:`read_ascii` for additional arguments to use with ascii files
         """
         
+        super().__init__()
         self.filename=None
         self.kdata=None
         self.kdata_unit='unspecified'
-        self.wns=None
-        self.wn_unit='cm^-1'
         self.data_type=None # 'xsec' or 'abs_coeff'
 
         if filename.lower().endswith(('.hdf5', '.h5')):
             self.read_hdf5(filename)
+        elif filename.lower().endswith(('.out','.bin')):
+            if filename.lower().endswith(('.bin')): binary = True
+            self.read_turbet(filename,  file_kdata_unit=file_kdata_unit, binary=binary, **kwargs)
         elif binary:
             self.read_binary(filename,  **select_kwargs(kwargs,['mass_amu']))
         else:
             self.read_ascii(filename, **select_kwargs(kwargs,['skiprows','wn_column',
                 'kdata_column','data_type']))
 
         if mult_factor is not None: self.kdata=self.kdata*mult_factor
@@ -62,15 +65,50 @@
                 kdata_unit='m^-1'
         else:
             raise RuntimeError("""Data type (xsec or abs_coeff) not recognized.
                 You should specify it with the data_type keyword
                 (and probably the file_kdata_unit as well).""")
 
         self.convert_kdata_unit(kdata_unit=kdata_unit,file_kdata_unit=file_kdata_unit)
-       
+
+    def read_turbet(self, filename, data_type='abs_coeff', file_kdata_unit='cm^-1',
+            wns=None, binary=False, wns_filename='sigma_grid.bin', **kwargs):
+        """Read native format from HR code by M. Turbet anf G. Chaverot
+    
+        Parameters
+        ----------
+            filename: str
+                Initial hires-spectrum filename.
+        """
+        import os
+        if data_type is None:
+            raise RuntimeError("You did not provide a data_type ('xsec' or 'abs_coeff')")
+        self.data_type = data_type
+        self.filename = filename
+        directory = os.path.dirname(filename) 
+        if binary:
+            with open(filename, 'rb') as f:
+                self.kdata = np.fromfile(f, dtype=np.float64)
+        else:
+            raw = pd.read_csv(filename) 
+            self.kdata = raw.values.flatten()
+        self.kdata_unit = file_kdata_unit
+        if wns is None:
+            if binary:
+                wns_filename = directory + '/' + wns_filename
+                with open(wns_filename, 'rb') as f:
+                    self.wns = np.fromfile(f, dtype=np.float64)
+            else:
+                wns_filename = directory + '/wavelength_grid.out'
+                raw = pd.read_csv(wns_filename) 
+                self.wns = raw.values.flatten()
+        else:
+            self.wns = wns
+        self.wn_unit = 'cm^-1'
+
     def read_ascii(self, filename, data_type=None, skiprows=0, wn_column=None,
         kdata_column=None):
         """Read native kspectrum format
 
         Parameters
         ----------
             filename: str
@@ -145,15 +183,14 @@
         dirname=os.path.dirname(self.filename)
         self.data_type='xsec'
         wls_cm=np.fromfile(os.path.join(dirname,'wlen.dat'))
         self.wns=1./wls_cm[::-1]
         self.kdata=np.fromfile(self.filename)[::-1]*mass_amu/N_A
         self.kdata_unit='cm^2/molecule'
 
-
     def convert_kdata_unit(self, kdata_unit='unspecified', file_kdata_unit='unspecified'):
         """Converts kdata to a new unit (inplace)
 
         Parameters
         ----------
             kdata_unit: str
                 String to identify the units to convert to. Accepts 'cm^2', 'm^2'
```

### Comparing `Exo_k-1.2.0/exo_k/kdatabase.py` & `exo_k-1.2.1/exo_k/kdatabase.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,14 +44,15 @@
         Loads an empty database to be filled later with
         :func:`~exo_k.kdatabase.Kdatabase.add_ktables`.
 
         .. important::
             By default, Ktables have zeros removed when loaded to avoid log interpolation
             issues. You can avoid that with the `remove_zeros=False` keyword.
         """
+        super().__init__()
         self.ktables={}
         self._settings=Settings()
         self.consolidated_wn_grid=True
         self.consolidated_PT_grid=True
         self.consolidated_p_unit=True
         self.consolidated_kdata_unit=True
         self.N_ktable5d=0
```

### Comparing `Exo_k-1.2.0/exo_k/ktable.py` & `exo_k-1.2.1/exo_k/ktable.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,15 @@
             xtable: :class:`~exo_k.xtable.Xtable`
                 input Xtable object instance
             wnedges: Array
                 edges of the wavenumber bins to be used to compute the corrk
 
         Other Parameters
         ----------------
-            weights: array, optional
+            weights: array, np.ndarray, optional
                 If weights are provided, they are used instead of the legendre quadrature.
             quad: string, optional
                 Type of quadrature used. Default is 'legendre'.
                 Also available: 'split-legendre' which uses half quadrature
                 points between 0. and `g_split` and half between `g_split` and 1.
             order: Integer, optional
                 Order of the Gauss legendre quadrature used. Default is 20.
@@ -227,31 +227,31 @@
             By default, log pressures are specified in Pa in logpgrid!!! If you want
             to use another unit, do not forget to specify it with the grid_p_unit keyword.
 
         Parameters
         ----------
             path : String
                 directory with the input files
-            filename_grid : array of str with shape (logpgrid.size,tgrid.size)
+            filename_grid : array, np.ndarray of str with shape (logpgrid.size,tgrid.size)
                 Names of the input high-res spectra. If None, the files are assumed to
                 follow Kspectrum/LMDZ convention, i.e.
                 be of the type 'k001', 'k002', etc.
                 See :func:`~exo_k.util.filenames.create_fname_grid_Kspectrum_LMDZ`
                 for possible additional keyword arguments.
-            logpgrid: array
+            logpgrid: array, np.ndarray
                 Grid in log(pressure) of the input. Default unit is Pa, but can be changed
                 with the `grid_p_unit` keyword.
-            tgrid: array
+            tgrid: array, np.ndarray
                 Grid in temperature of the input.
-            wnedges : array
+            wnedges : array, np.ndarray
                 Edges of the wavenumber bins to be used to compute the corr-k
 
         Other Parameters
         ----------------
-            weights: array, optional
+            weights: array, np.ndarray, optional
                 If weights are provided, they are used instead of the legendre quadrature.
             quad: string, optional
                 Type of quadrature used. Default is 'legendre'.
                 Also available: 'split-legendre' which uses half quadrature
                 points between 0. and `g_split` and half between `g_split` and 1.
             order: Integer, optional
                 Order of the Gauss legendre quadrature used. Default is 20.
@@ -528,23 +528,23 @@
 
     def bin_down(self, wnedges=None, weights=None, ggrid=None,
         remove_zeros=False, num=300, use_rebin=False, write=0):
         """Method to bin down a kcoeff table to a new grid of wavenumbers (inplace).
 
         Parameters
         ----------
-            wnedges: array
+            wnedges: array, np.ndarray
                 Edges of the new bins of wavenumbers (cm-1)
                 onto which the kcoeff should be binned down.
                 if you want Nwnew bin in the end, wnedges.size must be Nwnew+1
                 wnedges[0] should be greater than self.wnedges[0] (JL20 not sure anymore)
                 wnedges[-1] should be lower than self.wnedges[-1]
-            weights: array, optional
+            weights: array, np.ndarray, optional
                 Desired weights for the resulting Ktable.
-            ggrid: array, optional
+            ggrid: array, np.ndarray, optional
                 Desired g-points for the resulting Ktable.
                 Must be consistent with provided weights.
                 If not given, they are taken at the midpoints of the array
                 given by the cumulative sum of the weights
         """
         old_ggrid=self.ggrid
         if weights is not None:
@@ -573,17 +573,17 @@
         if remove_zeros : self.remove_zeros(deltalog_min_value=10.)
 
     def remap_g(self, ggrid=None, weights=None):
         """Method to resample a kcoeff table to a new g grid (inplace).
 
         Parameters
         ----------
-            ggrid: array
+            ggrid: array, np.ndarray
                 New grid of abcissas for quadrature
-            weights: array
+            weights: array, np.ndarray
                 New grid of weights
         """
         weights=np.array(weights)
         ggrid=np.array(ggrid)
         self.Ng=weights.size
         newkdata=np.zeros((self.Np, self.Nt, self.Nw, self.Ng))
         g_sample_4d(ggrid, newkdata, self.ggrid, self.kdata)
```

### Comparing `Exo_k-1.2.0/exo_k/ktable5d.py` & `exo_k-1.2.1/exo_k/ktable5d.py`

 * *Files 0% similar despite different names*

```diff
@@ -308,15 +308,15 @@
         objects.
 
         see :func:`exo_k.ktable.Ktable.hires_to_ktable` method for details
         on the arguments and options.
 
         Other Parameters
         ----------------
-            xgrid: array
+            xgrid: array, np.ndarray
                 Input grid in vmr of the variable gas. Needed for a Ktable5d.
 
         .. warning::
             By default, log pressures are specified in Pa in logpgrid!!! If you want
             to use another unit, do not forget to specify it with the grid_p_unit keyword.
 
         """
@@ -434,15 +434,15 @@
 
     def set_kdata(self, new_kdata):
         """Changes kdata (inplace). this is preferred to directly accessing kdata because one
         could forget to run setup_interpolation().
 
         Parameters
         ----------
-            new_kdata: array
+            new_kdata: array, np.ndarray
                 New array of kdata.
         """
         super().set_kdata(new_kdata)
         self.setup_interpolation()
 
     def interpolate_kdata(self, logp_array=None, t_array=None, x_array= None,
             log_interp=None, logp_interp=True, wngrid_limit=None, **kwargs):
@@ -693,23 +693,23 @@
 
     def bin_down(self, wnedges=None, weights=None, ggrid=None,
         remove_zeros=False, num=300, use_rebin=False, write=0):
         """Method to bin down a kcoeff table to a new grid of wavenumbers (inplace).
 
         Parameters
         ----------
-            wnedges: array
+            wnedges: array, np.ndarray
                 Edges of the new bins of wavenumbers (cm-1)
                 onto which the kcoeff should be binned down.
                 if you want Nwnew bin in the end, wnedges.size must be Nwnew+1
                 wnedges[0] should be greater than self.wnedges[0] (JL20 not sure anymore)
                 wnedges[-1] should be lower than self.wnedges[-1]
-            weights: array, optional
+            weights: array, np.ndarray, optional
                 Desired weights for the resulting Ktable.
-            ggrid: array, optional
+            ggrid: array, np.ndarray, optional
                 Desired g-points for the resulting Ktable.
                 Must be consistent with provided weights.
                 If not given, they are taken at the midpoints of the array
                 given by the cumulative sum of the weights
         """
         old_ggrid=self.ggrid
         if weights is not None:
@@ -761,17 +761,17 @@
         self.setup_interpolation()
 
     def remap_g(self, ggrid=None, weights=None):
         """Method to resample a kcoeff table to a new g grid (inplace).
 
         Parameters
         ----------
-            ggrid: array
+            ggrid: array, np.ndarray
                 New grid of abcissas for quadrature
-            weights: array
+            weights: array, np.ndarray
                 New grid of weights
         """
         weights=np.array(weights)
         ggrid=np.array(ggrid)
         self.Ng=weights.size
         newkdata=np.zeros((self.Np, self.Nt, self.Nx, self.Nw, self.Ng))
         g_sample_5d(ggrid, newkdata, self.ggrid, self.kdata)
@@ -793,15 +793,15 @@
     -------
         background_mol_names: list
             list of names of molecules in background gas
         var_mol: str
             Name of variable molecule
         Nx: int
             Size of xgrid
-        xgrid: array
+        xgrid: array, np.ndarray
             grid of vmr for variable gas
     """
     with open(filename, "r") as file:
         Nmol=int(file.readline())
         background_mol_names=[]
         for ii in range(Nmol-1):
             #print(file.readline().split()[0])
```

### Comparing `Exo_k-1.2.0/exo_k/ktable_io.py` & `exo_k-1.2.1/exo_k/ktable_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,15 +173,15 @@
         self.Nw=self.wns.size
 
         self.kdata_unit='cm^2/molecule'
         if band is None:
             file_to_load=os.path.join(path,res,'corrk_gcm.dat')
         else:
             file_to_load=os.path.join(path,res,'corrk_gcm_'+band+'.dat')
-        tmp=np.loadtxt(file_to_load).reshape((self.Nt,self.Np,self.Nw,self.Ng+1),order='F')
+        tmp=np.loadtxt(file_to_load).flatten().reshape((self.Nt,self.Np,self.Nw,self.Ng+1),order='F')
         self.kdata=tmp[:,:,:,:-1].transpose((1,0,2,3))
         # also removing the last g point which is equal to 0.
         self.logk=False
         return None
 
     def write_LMDZ(self, path, band='IR', fmt='%22.15e', write_only_metadata=False):
         """Saves data in a LMDZ friendly format.
```

### Comparing `Exo_k-1.2.0/exo_k/rayleigh.py` & `exo_k-1.2.1/exo_k/rayleigh.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     def sigma(self, wns, vmr):
         """Computes the Rayleigh cross section for the gas.
         This one is faster than sigma_array, but can be used only
         when vmr values are constants.
 
         Parameters
         ----------
-            wns: array
+            wns: array, np.ndarray
                 array of wavenumbers
 
             vmr: dict of arrays
                 Keys are molecule names. Values are the volume mixing ratios.
                 For speedup, only the first value will be used because we assume
                 that the vmr arrays are constant
 
@@ -51,15 +51,15 @@
         return res
 
     def sigma_array(self, wns, vmr):
         """Computes the Rayleigh cross section for the gas.
 
         Parameters
         ----------
-            wns: array
+            wns: array, np.ndarray
                 array of wavenumbers
 
             vmr: dict of arrays
                 Keys are molecule names. Values are arrays the volume mixing ratios
 
         Returns
         -------
@@ -82,24 +82,24 @@
     def sigma_mol(self, mol, wn2, wn4):
         """Intermediary function to compute rayleigh for each molecule.
 
         Parameters
         ----------
             mol: str
                 Molecule name.
-            wn2, wn4: arrays
+            wn2, wn4: array, np.ndarrays
                 Array of the wavenumber (in cm^-1) to the 2nd and 4th power.
                 (To avoid recomputing it each time).
         
         Returns
         -------
             to_add: bool
                 Says whether the molecule has been found
                 and the contribution needs to be added.
-            tmp: array of size self.wns or None
+            tmp: array, np.ndarray of size self.wns or None
                 The cross section for the molecule as a function of wns.
                 None if the molecule has not
                 been found.
 
         """
         to_add=True
         tmp=None
```

### Comparing `Exo_k-1.2.0/exo_k/settings.py` & `exo_k-1.2.1/exo_k/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 @author: jeremy leconte
 
-A class based on a singleton to store global options only once for every instance. 
+A class based on a singleton to store global options only once for every instance.
 """
 import os.path
 import re
 from glob import glob
 from string import Template
 from .util.singleton import Singleton
 
@@ -14,20 +14,21 @@
     """A class based on a singleton to store global options only once for every instance.
 
     So all the following methods can be called using the following syntax:
 
     >>> exo_k.Settings().method_name(agrs)
 
     In gerneal, they will change internal global attributes
-    that change the global behavior of some routines in the library. 
+    that change the global behavior of some routines in the library.
     """
 
     def init(self, *args, **kwds):
         self.reset_search_path()
         self._log_interp = True
+        self._log_interp_aerosol = False
         self._convert_to_mks = False
         self._delimiter = '_'
         self.set_delimiters(r"_.\-")
 
         self._case_sensitive = False
 
     def reset_search_path(self, path_type = 'all', no_path = False):
@@ -91,16 +92,16 @@
             if path_type in ('kdata', 'xtable'):
                 path_to_change.append(self._xtable_search_path)
 
         if path_to_change == []:
             raise RuntimeError('I did not understand the path type provided.')
         for path in search_paths:
             if not os.path.isdir(path):
-                raise NotADirectoryError("""The search_path you provided
-                    does not exist or is not a directory""")
+                raise NotADirectoryError("The search_path you provided "\
+                    f"does not exist or is not a directory ({path})")
             else:
                 for to_change in path_to_change:
                     if os.path.abspath(path) not in to_change:
                         to_change.append(os.path.abspath(path))
 
     def add_cia_search_path(self, *search_paths):
         """Add path(s) to the list of paths that will be searched for
@@ -172,17 +173,17 @@
         Example
         -------
             If I have a file named 'H2O.R10000_xsec.hdf5'
             that I want to load in a `Kdatabase`, the default
             settings will result in an error:
 
             >>> database=xk.Kdatabase(['H2O'],'R10000')
-             No file was found with these filters: 
+             No file was found with these filters:
              ('H2O_', 'R1000') in the following directories:
-             ['/home/falco/xsec/xsec_sampled_R10000_0.3-15'] 
+             ['/home/falco/xsec/xsec_sampled_R10000_0.3-15']
 
             Using
 
             >>> xk.Settings().set_delimiter('.')
             >>> database=xk.Kdatabase(['H2O'],'R10000')
 
             finds the file.
@@ -203,50 +204,60 @@
         self._search_mol_template = Template('(?=^$mol['+self._delimiters+  \
                 ']|['+self._delimiters+']$mol['+self._delimiters+'])')
         self._search_cia_template = Template('(?=^$mol1\\-$mol2['+self._delimiters+  \
                 ']|^$mol2\\-$mol1['+self._delimiters+'])')
 
 
     def set_log_interp(self, log_interp):
-        """Sets the default interpolation mode for kdata. Default is Log. 
+        """Sets the default interpolation mode for kdata. Default is Log.
 
         Parameters
         ----------
             log_interp: boolean
                 If True, log interpolation. Linear if False.
         """
         self._log_interp = log_interp
 
+    def set_log_interp_aerosol(self, log_interp):
+        """Sets the default interpolation mode for aerosols. Default is Linear. 
+
+        Parameters
+        ----------
+            log_interp: boolean
+                If True, log interpolation. Linear if False.
+        """
+        self._log_interp_aerosol = log_interp
+
     def set_case_sensitive(self, case_sensitive):
         """Set whether name matching is case sensitive. Default is False.
 
         Parameters
         ----------
             case_sensitive: boolean
                 If True, name matching is case sensitive.
         """
         self._case_sensitive = case_sensitive
 
     def set_mks(self, set_mks):
         """Forces conversion to mks system.
-        
+
         Parameters
         ----------
             set_mks: boolean
                 If True, all datasets are converted to mks upon loading.
         """
         self._convert_to_mks = set_mks
 
-    def list_files(self, *str_filters, molecule = None, 
+    def list_files(self, *str_filters, molecule = None,
             only_one = False, search_path = None, path_type = 'kdata'):
         """A routine that provides a list of all filenames containing
         a set of string filters in one of the global _search_path or a local one.
 
         Whether the search is case sensitive is specified through the
-        Settings.set_case_sensitive() method. 
+        Settings.set_case_sensitive() method.
 
         .. warning::
             The pattern matching with the `str_filters` is done using regular expressions.
             If you want to match special characters (like a dot in a filename), do not
             forget to put a backslash in front of it.
 
         Parameters
@@ -302,40 +313,40 @@
             if self._case_sensitive:
                 basename=os.path.basename(filename)
             else:
                 basename=os.path.basename(filename).lower()
             if re.search(template, basename) is None:
                 finalnames.remove(filename)
                 continue
-        if len(finalnames)>1 and only_one: 
+        if len(finalnames)>1 and only_one:
             print("""be careful: {filt}
             String filters not specific enough, several corresponding files have been found.
             We will use the first one:
             {file}
             Other files are:
             {other_files}""".format(filt=str_filters,file=finalnames[0], \
                 other_files=finalnames[1:]))
             finalnames=[finalnames[0]]
         if not finalnames:
             raise NoFileFoundError("""No file found to match this regular expression
-            (based on your filters): 
+            (based on your filters):
             {filt}
             in the following directories:
             {path}
             """.format(filt=template,path=local_search_path))
-        # an empty sequence yields False in a conditional statement ! 
+        # an empty sequence yields False in a conditional statement !
         return finalnames
 
-    def list_cia_files(self, *str_filters, molecule_pair = None, 
+    def list_cia_files(self, *str_filters, molecule_pair = None,
             only_one = False, search_path = None):
         """A routine that provides a list of all filenames containing
         a set of string filters in the global _search_path or a local one.
 
         Whether the search is case sensitive is specified through the
-        Settings.set_case_sensitive() method. 
+        Settings.set_case_sensitive() method.
 
         .. warning::
             The pattern matching with the `str_filters` is done using regular expressions.
             If you want to match special characters (like a dot in a filename), do not
             forget to put a backslash in front of it.
 
         Parameters
@@ -386,29 +397,29 @@
             if self._case_sensitive:
                 basename=os.path.basename(filename)
             else:
                 basename=os.path.basename(filename).lower()
             if re.search(template, basename) is None:
                 finalnames.remove(filename)
                 continue
-        if len(finalnames)>1 and only_one: 
+        if len(finalnames)>1 and only_one:
             print("""be careful: {filt}
             String filters not specific enough, several corresponding files have been found.
             We will use the first one:
             {file}
             Other files are:
             {other_files}""".format(filt=str_filters,file=finalnames[0], \
                 other_files=finalnames[1:]))
             finalnames=[finalnames[0]]
         if not finalnames:
             raise NoFileFoundError("""No file found to match this regular expression
-            (based on your filters): 
+            (based on your filters):
             {filt}
             in the following directories:
             {path}
             """.format(filt=template,path=local_search_path))
-        # an empty sequence yields False in a conditional statement ! 
+        # an empty sequence yields False in a conditional statement !
         return finalnames
 
 class NoFileFoundError(Exception):
     """Error when no file is found
     """
```

### Comparing `Exo_k-1.2.0/exo_k/two_stream/two_stream_crisp.py` & `exo_k-1.2.1/exo_k/two_stream/two_stream_crisp.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,41 +73,41 @@
           FOR NO DOWNWARD DIFFUSE FLUX AT THE TOP OF THE ATMOSPHERE,
           THE USER MUST INITIALIZE flux_dw(1) TO ZERO IN THE CALLING   
           PROGRAM.                                                  
 
 
     Parameters
     ----------
-        source: array
+        source: array, np.ndarray
             PLANCK function AT EACH LEVEL FROM TOP OF THE          
             ATMOSPHERE (L=0) TO THE SURFACE (L=NLAY) (NLAY+1 VALUES)  
             JL: actually seems to be pi times the planck function
             as defined in the rest of the code. 
-        dtau: array
+        dtau: array, np.ndarray
             ARRAY OF NORMAL INCIDENCE OPTICAL DEPTHS IN EACH       
             HOMOGENEOUS MODEL LAYER. (NLAY VALUES)                 
-        omega0: array
+        omega0: array, np.ndarray
             ARRAY OF SINGLE SCATTERING ALBEDOS FOR EACH HOMO-      
             GENEOUS MODEL LAYER. (NLAY VALUES)                     
-        g_asym: array
+        g_asym: array, np.ndarray
             ARRAY OF ASSYMETRY parameterS FOR EACH HOMOGENEOUS     
             MODEL LAYER. (NLAY VALUES)                             
     
     Returns
     -------                                                        
 
-        flux_up: array
+        flux_up: array, np.ndarray
             UPWARD FLUX AT NLAY+1 LAYER BOUNDARIES.                 
             (flux_up(L) REFERS TO THE UPWARD FLUX AT THE TOP          
             OF LAYER L)                                           
-        flux_dw: array
+        flux_dw: array, np.ndarray
             DOWNWARD FLUX AT NLAY+1 LAYER BOUNDARIES.               
             (flux_dw(L) REFERS TO THE DOWNWARD FLUX AT THE BOTTOM     
             OF LAYER L-1) 
-        flux_up-flux_dw: array
+        flux_up-flux_dw: array, np.ndarray
             Net flux at the same levels
 
     Other Parameters
     ----------------
         mu0: float
             Cos of quadrature angle (Original mu0 was 2/3.)
         flux_top_dw: float
```

### Comparing `Exo_k-1.2.0/exo_k/two_stream/two_stream_lmdz.py` & `exo_k-1.2.1/exo_k/two_stream/two_stream_lmdz.py`

 * *Files identical despite different names*

### Comparing `Exo_k-1.2.0/exo_k/two_stream/two_stream_toon.py` & `exo_k-1.2.1/exo_k/two_stream/two_stream_toon.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,29 +51,29 @@
     
     emis_surf=1.-alb_surf
     
     As we only consider hemispheric mean or quadrature, mu1==mu0
 
     Parameters
     ----------
-        source: array
+        source: array, np.ndarray
             pi*B (Planck function) at each of the Nlay+1 level interfaces of the model
             (top to bottom). Thanks to the pi factor it can be compared to the incoming
             flux.
-        dtau: array
+        dtau: array, np.ndarray
             optical depth of each of the Nlay model layers.
         omega0: float or array
             single scattering albedo of each layer
         g_asym: float or array
             asymmetry factor (g in Toon et al.)
         mu0: float
-            1./2. yields hemisperic mean approx
+            1./2. yields hemispheric mean approx
             1./sqrt(3) yields quadrature
         flux_top_dw: float
-            Incoming difuse flux at the upper boundary
+            Incoming diffuse flux at the upper boundary
         alb_surf: float
             Surface albedo. Emissivity is assumed to be 1.-alb_surf
         flux_at_level: bool, optional
             if flux_at_level is True, fluxes are calculated at the level surfaces.
             If False, fluxes are computed at the middle of the layers.
             The top of atmosphere flux is always computed at the top of the uppermost layer
             (1st level).
@@ -110,15 +110,15 @@
 
 @numba.jit(nopython=True, fastmath=True, cache=True)
 def matrix_toon_tridiag(Nlay, source, dtau, gam_1, gam_2, mu1,
         flux_top_dw, alb_surf, flux_at_level):
     """
     Returns
     -------
-        flux_net: array
+        flux_net: array, np.ndarray
             Net flux at the bottom of the Nlay layers.
     """
     e_1, e_2, e_3, e_4 = e_i_toon(dtau, gam_1, gam_2)
     c_up_top, c_dw_top, c_up_bot, c_dw_bot = c_planck(source, dtau, gam_1, gam_2, mu1)
     A=np.empty((2*Nlay))
     B=np.empty((2*Nlay))
     D=np.empty((2*Nlay))
@@ -266,15 +266,15 @@
     return XK
     
 #@numba.jit(nopython=True,fastmath=True, cache=True)
 def matrix_toon(Nlay, source, dtau, gam_1, gam_2, mu1, flux_top_dw, alb_surf):
     """
     Returns
     -------
-        flux_net: array
+        flux_net: array, np.ndarray
             Net flux at the bottom of the Nlay layers.
     """
     e_1, e_2, e_3, e_4 = e_i_toon(dtau, gam_1, gam_2)
     c_up_top, c_dw_top, c_up_bot, c_dw_bot = c_planck(source, dtau, gam_1, gam_2, mu1)
     A=np.empty((2*Nlay))
     B=np.empty((2*Nlay))
     D=np.empty((2*Nlay))
```

### Comparing `Exo_k-1.2.0/exo_k/util/cst.py` & `exo_k-1.2.1/exo_k/util/cst.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 """Defines constants in SI units"""
 
 G = 6.67384e-11
 RSOL = 6.955e8
 RJUP = 7.1492e7
 RJUP_POL = 6.9911e7 # Polar Radius
+REARTH = 6.371e6
 PI = 3.14159265359
 MSOL = 1.98847542e+30
 MJUP = 1.898e27
+MEARTH = 5.97e24
+LSOL = 3.839e26
 AU = 1.49597871e+11
 KBOLTZ = 1.380648813e-23
 RGP = 8.31446
 PLANCK = 6.62606957e-34
 C_LUM = 299792458
 SIG_SB = 5.670367e-08
 N_A = 6.022140857e+23
+PARSEC = 3.08568e16
 DAY = 86400. #s
+YEAR = 31557600.
 tiny=1.e-13
 OneMintiny=1.-tiny
 
 ktable_long_name_attributes={
     'p': 'Pressure grid',
     't': 'Temperature grid',
     'x': 'Volume mixing ratio grid',
```

### Comparing `Exo_k-1.2.0/exo_k/util/filenames.py` & `exo_k-1.2.1/exo_k/util/filenames.py`

 * *Files identical despite different names*

### Comparing `Exo_k-1.2.0/exo_k/util/interp.py` & `exo_k-1.2.1/exo_k/util/interp.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 def bilinear_interpolation(z00, z10, z01, z11, x, y):
     """
     2D interpolation
     Applies linear interpolation across x and y between xmin,xmax and ymin,ymax
 
     Parameters
     ----------
-        z00: array
+        z00: array, np.ndarray
             Array corresponding to xmin,ymin
-        z10: array
+        z10: array, np.ndarray
             Array corresponding to xmax,ymin
-        z01: array
+        z01: array, np.ndarray
             Array corresponding to xmin,ymax
-        z11: array
+        z11: array, np.ndarray
             Array corresponding to xmax,ymax
         x: float
             weight on x coord
         y: float
             weight on y coord
     """
     xy = x*y
@@ -42,25 +42,25 @@
     2D interpolation
     Applies linear interpolation across x and y between xmin,xmax and ymin,ymax.
     For this variant of bilinear_interpolation (mainly for chemistry),
     x, y and z must be 1D-arrays of the same length.
 
     Parameters
     ----------
-        z00: array
+        z00: array, np.ndarray
             Array corresponding to xmin,ymin
-        z10: array
+        z10: array, np.ndarray
             Array corresponding to xmax,ymin
-        z01: array
+        z01: array, np.ndarray
             Array corresponding to xmin,ymax
-        z11: array
+        z11: array, np.ndarray
             Array corresponding to xmax,ymax
-        x: array
+        x: array, np.ndarray
             weights on x coord
-        y: array
+        y: array, np.ndarray
             weights on y coord
     """
     xy = x*y
     res = np.zeros_like(z00)
     for i in range(z00.shape[0]):
         res[i] = (z11[i]-z01[i]+z00[i]-z10[i])*xy[i] +(z01[i]-z00[i])*y[i] +(z10[i]-z00[i])*x[i] +z00[i]
     return res
@@ -70,17 +70,17 @@
 def linear_interpolation(z00, z10, x):
     """1D interpolation.
 
     Applies linear interpolation in x between xmin, xmax.
 
     Parameters
     ----------
-        z00: array
+        z00: array, np.ndarray
             Array corresponding to xmin
-        z10: array
+        z10: array, np.ndarray
             Array corresponding to xmax
         x: float
             weight on x coord
     """
     res = np.zeros_like(z00)
     for i in range(z00.shape[0]):
 #        res[i] = z10[i]*x+z00[i]*x2
@@ -130,19 +130,19 @@
 
 @numba.njit(cache=True)
 def kdata_conv_loop(kdata1,kdata2,kdataconv,shape):
     """Computes the convolution of two kdata tables.
 
     Parameters
     ----------
-        kdata1,kdata2 : arrays
+        kdata1,kdata2 : array, np.ndarrays
             The two ktable.kdata tables to convolve.
-        shape : array
+        shape : array, np.ndarray
             shape of the ktabke.kdata tables to convolve (last size is Ng).
-        kdataconv : array
+        kdataconv : array, np.ndarray
             Result table where the last dimension as a length equal to Ng^2.
     """
     Ng=shape[-1]
     for i in range(shape[0]):
      for j in range(shape[1]):
       for k in range(shape[2]):
        for l in range(Ng):
@@ -153,17 +153,17 @@
 def kdata_conv_loop_profile(kdata1,kdata2,kdataconv,Nlay,Nw,Ng):
     """Computes the convolution of two atmospheric kdata profiles.
 
     Nothing is returned. kdataconv is changed in place. 
 
     Parameters
     ----------
-        kdata1,kdata2 : arrays
+        kdata1,kdata2 : array, np.ndarrays
             The two ktable.kdata tables to convolve.
-        kdataconv : array
+        kdataconv : array, np.ndarray
             Result table where the last dimension as a length equal to Ng^2.
         Nlay : int
             Number of atmospheric layers
         Nw : int
             Number of wavenumber points
         Ng : int
             Number of g-points
@@ -177,19 +177,19 @@
 @numba.njit(fastmath=True)
 def rebin(f_fine,fine_grid,coarse_grid):
     """Computes the binned version of a function on a coarser grid.
     The two grids do not need to have the same boundaries.
 
     Parameters
     ----------
-        f_fine: array
+        f_fine: array, np.ndarray
             Function to be rebinned, given on the fine_grid.
-        fine_grid: array
+        fine_grid: array, np.ndarray
             The high resolution grid edges we start with.
-        coarse_grid: array
+        coarse_grid: array, np.ndarray
             The coarser resolution grid edges inside which we want to bin the function f.
        """
     indicestosum=np.searchsorted(fine_grid,coarse_grid,side='right')
     Nfine=fine_grid.size
     if indicestosum[-1]==Nfine : 
         indicestosum=np.where(indicestosum<Nfine,indicestosum,Nfine-1)
     dgrid=np.diff(fine_grid)
@@ -240,19 +240,19 @@
 def RandOverlap_2_kdata_prof(Nlay, Nw, Ng, kdata1, kdata2, weights, ggrid):
     """Function to randomely mix the opacities of 2 species in an atmospheric profile.
 
     Parameters
     ----------
         Nlay, Nw, Ng: int
             Number of layers, spectral bins, and gauss points. 
-        kdata1, kdata2: arrays of size (Nlay, Nw, Ng)
+        kdata1, kdata2: array, np.ndarrays of size (Nlay, Nw, Ng)
             vmr weighted cross-sections for the two species.
-        weights: array
+        weights: array, np.ndarray
             gauss weights.
-        ggrid: array
+        ggrid: array, np.ndarray
             g-points.
     
     Returns
     -------
         array
             k-coefficient array of the mix over the atmospheric column.
     """
@@ -357,19 +357,19 @@
     Parameters
     ----------
         order: int
             Order of the quadrature wanted.
 
     Returns
     -------
-        weights: array(order)
+        weights: array, np.ndarray(order)
             Weights to be used in the quadrature.
-        ggrid: array(order)
+        ggrid: array, np.ndarray(order)
             Abscissa to be used for the quadrature.
-        gedges: array(order+1)
+        gedges: array, np.ndarray(order+1)
             Cumulative sum of the weights. Goes from 0 to 1.
        """ 
     ggrid,weights=leggauss(order)
     weights=weights/2.
     ggrid=(ggrid+1.)/2.
     gedges=np.insert(np.cumsum(weights),0,0.)
     return weights,ggrid,gedges
@@ -385,19 +385,19 @@
         order: int
             Order of the quadrature wanted. Needs to be even.
         g_split: float between 0 and 1
             Splitting point.
 
     Returns
     -------
-        weights: array(order)
+        weights: array, np.ndarray(order)
             Weights to be used in the quadrature.
-        ggrid: array(order)
+        ggrid: array, np.ndarray(order)
             Abscissa to be used for the quadrature.
-        gedges: array(order+1)
+        gedges: array, np.ndarray(order+1)
             Cumulative sum of the weights. Goes from 0 to 1.
        """ 
     if order%2==1:
         print('order should be an even number')
         raise RuntimeError()
     ggrid,weights=leggauss(order//2)
     weights1=weights*g_split/2.
@@ -411,28 +411,28 @@
 
 @numba.njit
 def spectrum_to_kdist(k_hr,wn_hr,dwn_hr,wnedges,ggrid):
     """Creates the k-distribution from a single high resolution spectrum
     
     Parameters
     ----------
-        k_hr : array
+        k_hr : array, np.ndarray
             Spectrum
-        wn_hr : array
+        wn_hr : array, np.ndarray
             Wavenumber grid
-        dwn_hr : array
+        dwn_hr : array, np.ndarray
             Width of the high resolution wavenumber bins.
-        wnedges : array
+        wnedges : array, np.ndarray
             Lower resolution wavenumber bin edges inside which the k-dist will be computed.
-        ggrid : array
+        ggrid : array, np.ndarray
             Grid of g-point abscissas
 
     Returns
     -------
-        kdata : array
+        kdata : array, np.ndarray
             k coefficients for each (Wn, g) bin.
     """
     pos=np.searchsorted(wn_hr,wnedges)
     #print(pos)
     kdata=np.zeros((wnedges.size-1,ggrid.size))
     for ib in range(wnedges.size-1):
         if pos[ib+1]==pos[ib]:
@@ -457,28 +457,28 @@
 @numba.njit(cache=True)
 def bin_down_corrk_numba(newshape, kdata, old_ggrid, new_ggrid, gedges, indicestosum, \
         wngrid_filter, wn_weigths, num, use_rebin):
     """bins down a kcoefficient table (see :func:`~exo_k.ktable.Ktable.bin_down` for details)
     
     Parameters
     ----------
-        newshape : array
+        newshape : array, np.ndarray
             Shape of kdata.
-        kdata : array
+        kdata : array, np.ndarray
             table to bin down.
-        old_ggrid : array
+        old_ggrid : array, np.ndarray
             Grid of old g-point abscissas for kdata.
-        new_ggrid : array
+        new_ggrid : array, np.ndarray
             New g-points for the binned-down k-coefficients.
-        gedges : array
+        gedges : array, np.ndarray
             Cumulative sum of the weights. Goes from 0 to 1.
             Used only if use_rebin=True
         indicestosum: list of lists
             Indices of wavenumber bins to be used for the averaging
-        wngrid_filter: array
+        wngrid_filter: array, np.ndarray
             Indices of the new table where there will actually be data (zero elsewhere)
         wn_weigths: list of lists
             Weights to be used for the averaging (same size as indicestosum)
         num: int
             Number of points to fine sample the g function in log-k space
         use_rebin: boolean
             Whether to use rebin or interp method.
```

### Comparing `Exo_k-1.2.0/exo_k/util/molar_heat_capacity.py` & `exo_k-1.2.1/exo_k/util/molar_heat_capacity.py`

 * *Files identical despite different names*

### Comparing `Exo_k-1.2.0/exo_k/util/molar_mass.py` & `exo_k-1.2.1/exo_k/util/molar_mass.py`

 * *Files identical despite different names*

### Comparing `Exo_k-1.2.0/exo_k/util/radiation.py` & `exo_k-1.2.1/exo_k/util/radiation.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 def Bnu_integral(nu_edges, T):
     """Computes the integral of the Planck function in wavenumber bins.
     
     Uses scipy.integrate.quad. Quite slow.
 
     Parameters
     ----------
-        nu_edges: array
+        nu_edges: array, np.ndarray
             Edges of the wavenumber bins in cm^-1.
         T: float
             Temperature (K).
 
     Returns
     -------
         array
@@ -76,15 +76,15 @@
     "PLANCK FUNCTIONS AND INTEGRALS; METHODS OF COMPUTATION
     by Thomas E. Michels
     Goddard Space Flight Center Greenbelt, Md.
     MARCH 1968"
     
     Parameters
     ----------
-        nu_edges: array
+        nu_edges: array, np.ndarray
             Edges of the wavenumber bins in cm^-1.
         T: float
             Temperature (K).
         n: int
             number of terms to take into account in the black body calculation.
     
     Returns
@@ -117,17 +117,17 @@
     "PLANCK FUNCTIONS AND INTEGRALS; METHODS OF COMPUTATION
     by Thomas E. Michels
     Goddard Space Flight Center Greenbelt, Md.
     MARCH 1968"
 
     Parameters
     ----------
-        nu_edges: array
+        nu_edges: array, np.ndarray
             Edges of the wavenumber bins in cm^-1.
-        T: array
+        T: array, np.ndarray
             Array of temperature (K).
         Nw: int
             Number of spectral bins.
         Nt: int
             Number of temperatures.
         n: int, optional
             number of terms to take into account in the black body calculation.
@@ -163,17 +163,17 @@
 
 @numba.jit(nopython=True, fastmath=True)
 def dBnudT_array(nu, T_array, Nw, Nt):
     """Computes the derivative of the Planck function with respect to temperature.
 
     Parameters
     ----------
-        nu: array
+        nu: array, np.ndarray
             Wavenumbers in cm^-1.
-        T: array
+        T: array, np.ndarray
             Array of temperature (K).
         Nw: int
             Number of spectral bins.
         Nt: int
             Number of temperatures.
     
     Returns
@@ -181,16 +181,16 @@
         Array of shape (T_array.size,nu.size)
             dBnudT: derivative of the Planck function at
             temperatures T_array.
     """
     res=np.empty((Nt,Nw))
     sigma=nu*1.e2
     for iT, T in enumerate(T_array):
-        exp=np.exp(PLANCK_CST2*sigma/T)
-        tmp=((exp-1.)*T)**2
+        exp=np.exp(-PLANCK_CST2*sigma/T)
+        tmp=((1. - exp) * T)**2
         res[iT]=exp * PLANCK_CST3 * sigma**4 / tmp
     return res
 
 @numba.jit(nopython=True, cache=True)
 def Bmicron(lamb, T):
     """Computes the Planck law in wavelength domain.
 
@@ -300,17 +300,17 @@
 @numba.njit
 def rad_prop_corrk(dcol_density, opacity_prof, mu0):
     """Computes the optical depth of each of the radiative layers
     for the opacity given for every wavelength and g point.
 
     Parameters
     ----------
-        dcol_density: array
+        dcol_density: array, np.ndarray
             Column density per radiative layer (molecules/m^2/layer).
-        opacity_prof: array
+        opacity_prof: array, np.ndarray
             effective cross section per molecule (m^2/molecule).
         mu0: cosine of the equivalent zenith angle for the rays.
             e.g. Cos(60deg)=0.5 is chosen (See, for example, chap 4 of Pierrehumbert 2010)
 
     Returns
     -------
         tau: Array
@@ -334,17 +334,17 @@
 @numba.njit
 def rad_prop_xsec(dcol_density, opacity_prof, mu0):
     """Computes the optical depth of each of the radiative layers
     for the opacity given for every wavelength.
 
     Parameters
     ----------
-        dcol_density: array
+        dcol_density: array, np.ndarray
             Column density per radiative layer (molecules/m^2/layer).
-        opacity_prof: array
+        opacity_prof: array, np.ndarray
             effective cross section per molecule (m^2/molecule).
         mu0: cosine of the equivalent zenith angle for the rays.
             e.g. Cos(60deg)=0.5 is chosen (See, for example, chap 4 of Pierrehumbert 2010)
 
     Returns
     -------
         tau: Array
@@ -375,24 +375,24 @@
             Number of layers.
         Nw: int
             Number of wavenumber bins.
         Ng: int
             Number of gauss points.
         tangent_path: List of arrays
             Triangular array of tangent path for each layer.
-        density_prof: array
+        density_prof: array, np.ndarray
             Array with the number density of molecules in the atmosphere.
-        opacity_prof: array
+        opacity_prof: array, np.ndarray
             Effective cross section of the atmsophere for each (layer,wavenumber,g-point).
-        weights: array
+        weights: array, np.ndarray
             Weights for the quadrature in g-space.
 
     Returns
     -------
-        transmittance: array
+        transmittance: array, np.ndarray
             Transmittance for each layer and wavenumber bin (Exp(-tau_sigma)).
     """
     exp_min_tau=np.zeros((Nlay,Nw,Ng))
     transmittance=np.zeros((Nlay,Nw))
     for ilay in range(Nlay):
         for jlay in range(ilay+1):
             dm=tangent_path[ilay][jlay]*density_prof[jlay]
@@ -417,22 +417,22 @@
     ----------
         Nlay: int
             Number of layers.
         Nw: int
             Number of wavenumber bins.
         tangent_path: List of arrays
             Triangular array of tangent path for each layer.
-        density_prof: array
+        density_prof: array, np.ndarray
             Array with the number density of molecules in the atmosphere.
-        opacity_prof: array
+        opacity_prof: array, np.ndarray
             Effective cross section of the atmsophere for each (layer,wavenumber).
 
     Returns
     -------
-        transmittance: array
+        transmittance: array, np.ndarray
             Transmittance for each layer and wavenumber bin (Exp(-tau_sigma)).
     """
     transmittance=np.zeros((Nlay,Nw))
     for ilay in range(Nlay):
         for jlay in range(ilay+1):
             dm=tangent_path[ilay][jlay]*density_prof[jlay]
             for iW in range(Nw):
```

### Comparing `Exo_k-1.2.0/exo_k/util/singleton.py` & `exo_k-1.2.1/exo_k/util/singleton.py`

 * *Files identical despite different names*

### Comparing `Exo_k-1.2.0/exo_k/util/spectrum.py` & `exo_k-1.2.1/exo_k/util/spectrum.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,59 @@
 # -*- coding: utf-8 -*-
 """
 @author: jeremy leconte
 
 A module to handle ouputs rebinning and plotting
 """
-import numpy as np
-import h5py
+from __future__ import annotations
+
+from typing import Optional
+
 import astropy.units as u
+import h5py
+import numpy as np
+
 from exo_k.util.interp import rebin
 from exo_k.util.spectral_object import Spectral_object
+from exo_k.util.cst import PLANCK, C_LUM
+
+planckovclum = PLANCK * 100. * C_LUM  #100 is a conversion factor from cm^-1 to m^-1
 
 class Spectrum(Spectral_object):
     """A class defining a Spectrum object to plot and manipulate.
     """
 
     def __init__(self, value = None, wns = None, wnedges = None, input_spectral_unit='cm^-1', spectral_unit='cm^-1',
             filename = None, spectral_radiance = False, 
             from_taurex = False, dataset = 'native_spectrum', **kwargs):
         """Instanciate with a value, bin centers, and bin edges.
         Can also load a Taurex spectrum if filename is provided.
 
         Parameters
         ----------
-            value : Array
+            value: Array
                 spectrum values
-            wns : Array
+            wns: Array
                 Spectral grid (can be wavenumbers or wavelengths)
-            wnedges : Array
+            wnedges: Array
                 Bin edges grid (can be wavenumbers or wavelengths)
-            input_spectral_unit : str
+            input_spectral_unit: str
                 Unit of the input spectral grid
-            spectral_unit : str
+            spectral_unit: str
                 desired output unit for the spectral grid
-            filename : str
+            filename: str
                 Name of a file where the spectrum is stored. 
                 If a filename is given, there is no need to provide
                 values, wns, ...
-            spectral_radiance : bool
+            spectral_radiance: bool
                 If True, the spectrum is assumed to be a flux in units of
                 inverse spectral units (for example W/micron if the spectral unit is microns)
-                If False, the spectrum is considered as monochormatic values (like Rp/Rs**2)
+                If False, the spectrum is considered as monochromatic values (like Rp/Rs**2)
         """
+        super().__init__()
         self.value = value
         self.wns = wns
         self.wnedges = wnedges
         self.spec_unit = input_spectral_unit
         self.spectral_radiance = spectral_radiance
 
         if filename is not None:
@@ -56,42 +65,76 @@
                 self.read_ascii(filename, **kwargs)
 
         if (self.wnedges is None) and (self.wns is not None):
             self.wnedges = np.concatenate(([self.wns[0]],
                 (self.wns[:-1]+self.wns[1:])*0.5,[self.wns[-1]]))
 
         self.convert_spectral_units(input_spectral_unit=input_spectral_unit,
-            spectral_unit=spectral_unit, spectral_radiance = spectral_radiance)
+                                    spectral_unit=spectral_unit, spectral_radiance=spectral_radiance)
+
+        if self.wnedges is not None:
+            self.dwnedges = np.diff(self.wnedges)
+        else:
+            self.dwnedges = None
 
-    def convert_spectral_units(self, input_spectral_unit='cm^-1', spectral_unit='cm^-1', spectral_radiance = None):
-        if (spectral_unit != input_spectral_unit):
+    def convert_spectral_units(self, input_spectral_unit='cm^-1', spectral_unit='cm^-1',
+                               spectral_radiance: Optional[bool] = None):
+        if spectral_unit != input_spectral_unit:
             wns_tmp = (self.wns*u.Unit(input_spectral_unit)).to(u.Unit(spectral_unit), equivalencies=u.spectral()).value
             wnedges_tmp = (self.wnedges*u.Unit(input_spectral_unit)).to(u.Unit(spectral_unit), equivalencies=u.spectral()).value
+
             if spectral_radiance is not None:
                 self.spectral_radiance = spectral_radiance
+
             if self.spectral_radiance:
                 dwnedges = np.diff(self.wnedges)
                 dwnedges_tmp = np.diff(wnedges_tmp)
                 self.value = self.value * np.abs(dwnedges / dwnedges_tmp)
                 # assumes that the wavelength unit
                 # is the same as the spectral unit (for example F in W/nm if wl in nm).
+
             if wnedges_tmp[-1] > wnedges_tmp[0]:
                 self.wns = wns_tmp
                 self.wnedges = wnedges_tmp
             else:
                 self.wns = np.copy(wns_tmp[::-1])
                 self.wnedges = np.copy(wnedges_tmp[::-1])
                 self.value = np.copy(self.value[::-1])
 
-    
+    def normalize(self, bolometric_flux: float):
+        """Normalize the spectrum to a specified bolometric flux
+
+        Parameters
+        ----------
+            bolometric_flux: float
+                Integral of the flux over the total bandpass after normalization. 
+        """
+        factor = bolometric_flux / self.total
+        self.value *= factor
+
+    def photonize(self):
+        """Translate to photon count in each bin
+        """
+        self.value /= self.wns * planckovclum
+
+    def dephotonize(self):
+        """Translate back to energy
+        """
+        self.value *= self.wns * planckovclum
+
+    def integrate_per_bin(self):
+        """integrate energy in each bin
+        """
+        self.value *= self.dwnedges
+
     def copy(self):
         """Deep copy of the spectrum.
         """
-        return Spectrum(self.value.copy(),self.wns.copy(),self.wnedges.copy(),
-            input_spectral_unit = self.spec_unit, spectral_unit = self.spec_unit)
+        return Spectrum(self.value.copy(), self.wns.copy(), self.wnedges.copy(),
+                        input_spectral_unit=self.spec_unit, spectral_unit=self.spec_unit)
 
     def plot_spectrum(self, ax, per_wavenumber = True, x_axis = 'wls',
             xscale=None, yscale=None, **kwarg):
         """Plot the spectrum
         
         Parameters
         ----------
@@ -120,86 +163,122 @@
         if yscale is not None: ax.set_yscale(yscale)
 
     def bin_down(self, wnedges):
         """Bins down the spectrum to a new grid of wnedges by conserving area.
         
         Parameters
         ----------
-            wnedges: array
+            wnedges: array, np.ndarray
                 Wavenumbers of the bin edges to be used
         """
         wnedges=np.array(wnedges)
         self.value=rebin(self.value,self.wnedges,wnedges)
         self.wnedges=wnedges
+        self.dwnedges = np.diff(self.wnedges)
         self.wns=0.5*(self.wnedges[:-1]+self.wnedges[1:])
 
     def bin_down_cp(self, wnedges):
         """Returns a new binned down spectrum to a grid of wnedges by conserving area.
         
         Parameters
         ----------
-            wnedges: array
+            wnedges: array, np.ndarray
                 Wavenumbers of the bin edges to be used
 
         Returns
         -------
             :class:`Spectrum`
                 Binned down spectrum
         """
         res=self.copy()
         res.bin_down(wnedges)
         return res
 
+    def clip_spectral_range(self, wn_range=None, wl_range=None):
+        """Limits the data to the provided spectral range (inplace):
+
+           * Wavenumber in cm^-1 if using wn_range argument
+           * Wavelength in micron if using wl_range
+        """
+        iw_min, iw_max = self.select_spectral_range(wn_range, wl_range)
+        self.value = self.value[iw_min:iw_max]
+
     def randomize(self, uncertainty = 0.):
         """Adds random noise with a given uncertainty.
         """
         self.noise = uncertainty * np.random.randn((self.value.size))
         self.value += self.noise
 
-    def __add__(self,other):
+    def __add__(self, other):
         """Defines addition
         """
-        if (isinstance(other,float) or isinstance(other,int)):
-            return Spectrum(self.value+other,self.wns,self.wnedges)
-        elif (self.wns.size==other.wns.size) and np.array_equal(self.wns,other.wns):
-            val=self.value+other.value
-            return Spectrum(val,self.wns,self.wnedges)
+        if isinstance(other, (float, int, np.ndarray)):
+            return Spectrum(self.value + other, self.wns, self.wnedges)
+
+        if (self.wns.size == other.wns.size) and np.array_equal(self.wns, other.wns):
+            val = self.value + other.value
+            return Spectrum(val, self.wns, self.wnedges)
         else:
             raise RuntimeError('The two spectra do not have the same spectral sampling.')
 
-    def __sub__(self,other):
-        """Defines substraction
+    def __radd__(self, other):
+        """Use commutativity v + S == S + v"""
+
+        return self.__add__(other)
+
+    def __sub__(self, other):
+        """Defines subtraction
         """
-        if (isinstance(other,float) or isinstance(other,int)):
-            return Spectrum(self.value-other,self.wns,self.wnedges)
-        elif (self.wns.size==other.wns.size) and np.array_equal(self.wns,other.wns):
-            val=self.value-other.value
-            return Spectrum(val,self.wns,self.wnedges)
+        if isinstance(other, (float, int, np.ndarray)):
+            return Spectrum(self.value - other, self.wns, self.wnedges)
+
+        if (self.wns.size == other.wns.size) and np.array_equal(self.wns, other.wns):
+            val = self.value - other.value
+            return Spectrum(val, self.wns, self.wnedges)
         else:
             raise RuntimeError('The two spectra do not have the same spectral sampling.')
 
-    def __mul__(self,other):
+    def __mul__(self, other):
         """Defines multiplication
         """
-        if (isinstance(other,float) or isinstance(other,int)):
-            return Spectrum(self.value*other,self.wns,self.wnedges)
-        elif (self.wns.size==other.wns.size) and np.array_equal(self.wns,other.wns):
-            val=self.value*other.value
-            return Spectrum(val,self.wns,self.wnedges)
+        if isinstance(other, (float, int, np.ndarray)):
+            return Spectrum(self.value * other, self.wns, self.wnedges)
+
+        if (self.wns.size == other.wns.size) and np.array_equal(self.wns, other.wns):
+            val = self.value * other.value
+            return Spectrum(val, self.wns, self.wnedges)
         else:
             raise RuntimeError('The two spectra do not have the same spectral sampling.')
 
-    def __truediv__(self,other):
+    def __rmul__(self, other):
+        """Use commutativity v * S == S * v"""
+
+        return self.__mul__(other)
+
+    def __truediv__(self, other):
+        """Defines division
+        """
+        if isinstance(other, (float, int, np.ndarray)):
+            return Spectrum(self.value / other, self.wns, self.wnedges)
+
+        if (self.wns.size == other.wns.size) and np.array_equal(self.wns, other.wns):
+            val = self.value / other.value
+            return Spectrum(val, self.wns, self.wnedges)
+        else:
+            raise RuntimeError('The two spectra do not have the same spectral sampling.')
+
+    def __rtruediv__(self, other):
         """Defines division
         """
-        if (isinstance(other,float) or isinstance(other,int)):
-            return Spectrum(self.value/other,self.wns,self.wnedges)
-        elif (self.wns.size==other.wns.size) and np.array_equal(self.wns,other.wns):
-            val=self.value/other.value
-            return Spectrum(val,self.wns,self.wnedges)
+        if isinstance(other, (float, int, np.ndarray)):
+            return Spectrum(other / self.value, self.wns, self.wnedges)
+
+        if (self.wns.size == other.wns.size) and np.array_equal(self.wns, other.wns):
+            val = other.value / self.value
+            return Spectrum(val, self.wns, self.wnedges)
         else:
             raise RuntimeError('The two spectra do not have the same spectral sampling.')
 
     def std(self):
         """Defines standard deviation
         """
         return self.value.std()
@@ -214,16 +293,15 @@
         """
         return Spectrum(np.log10(self.value),self.wns,self.wnedges)
 
     @property
     def total(self):
         """Defines the weighted sum over the spectrum
         """
-        dw=np.diff(self.wnedges)
-        return np.dot(self.value,dw)
+        return np.dot(self.value,self.dwnedges)
 
     def read_hdf5(self, filename=None):
         """Reads data in a hdf5 file
 
         Parameters
         ----------
             filename: str
@@ -311,15 +389,14 @@
         """
         with h5py.File(filename, 'r') as f:
             self.wns = f['Output/Spectra/native_wngrid'][...]
             self.value = f['Output/Spectra/'+dataset][...]
 
         self.wnedges=np.concatenate(([self.wns[0]],(self.wns[:-1]+self.wns[1:])*0.5,[self.wns[-1]]))
 
-
     def __repr__(self):
         """Method to output header
         """
         output="""
         value        : {val}
         wl (microns) : {wl}
         """.format(val=self.value,wl=self.wls)
```

### Comparing `Exo_k-1.2.0/exo_k/util/user_func.py` & `exo_k-1.2.1/exo_k/util/user_func.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,35 +12,36 @@
 import numpy as np
 from exo_k.ktable import Ktable
 from exo_k.ktable5d import Ktable5d
 from exo_k.xtable import Xtable
 from exo_k.hires_spectrum import Hires_spectrum
 from exo_k.util.cst import PI
 from exo_k.atm_evolution.atm_evol import Atm_evolution
+from exo_k.aerosol import mmr_to_number_density # noqa
 
 def create_table(logpgrid=None, tgrid=None, xgrid=None, wngrid=None, wnedges=None,
         ggrid=None, weights=None, p_unit='Pa', kdata_unit='m^2/molecule',
         value=None, mol=None):
     """Create a new table with the required dimensions padded with zeros.
 
     The class of the object created will depend on the dimensions required. 
 
     Parameters
     ----------
-        logpgrid: array
+        logpgrid: array, np.ndarray
             Grid in log p
-        tgrid: array
+        tgrid: array, np.ndarray
             Grid in T
-        xgrid: array
+        xgrid: array, np.ndarray
             Grid in volume mixing ratio
-        wngrid: array
+        wngrid: array, np.ndarray
             Grid wavenumber
-        ggrid: array
+        ggrid: array, np.ndarray
             Grid g-space
-        weights: array
+        weights: array, np.ndarray
             Grid of quadrature weights
         p_unit: str (optional)
             Unit of pressure (default Pa)
         kdata_unit: str (optional)
             Unit of cross section (default is m^2/molecule)
 
     Returns
@@ -239,32 +240,14 @@
     os.symlink('../IR'+str(IRsize)+'/corrk_gcm_IR.dat',os.path.join(newdir,'corrk_gcm_IR.dat'))
     os.symlink('../IR'+str(IRsize)+'/narrowbands_IR.in',os.path.join(newdir,'narrowbands_IR.in'))
     os.symlink('../VI'+str(VIsize)+'/corrk_gcm_VI.dat',os.path.join(newdir,'corrk_gcm_VI.dat'))
     os.symlink('../VI'+str(VIsize)+'/narrowbands_VI.in',os.path.join(newdir,'narrowbands_VI.in'))
     print('Everything went ok. Your ktable is in:',newdir)
     print("You'll probably need to add Q.dat before using it though!")
 
-def mmr_to_number_density(mmr, gas_density, r_eff, condensate_density):
-    """Converts a mass mixing ratio (mmr or q) in a number density of particles
-    (in number per unit volume)
-
-    Parameters
-    ----------
-        mmr: float or array
-            Mass mixing ratio (in kg per kg of air)
-        gas_density: float or array
-            Density of the gas (in kg/m^3)
-        r_eff: float or array
-            Effective radius of the particles
-        condensate_density: float or array
-            Density of the constituent of the condensed particles (in kg/m^3)
-    """
-    particle_mass=4.*PI*r_eff**3*condensate_density/3.
-    return mmr*gas_density/particle_mass
-
 def load_atm_evolution(pickle_filename):
     """Load an Atm_evolution instance from a pickle file
 
     Parameters
     ----------
         pickle_filename: str
             name of pickle file
```

### Comparing `Exo_k-1.2.0/exo_k/xtable.py` & `exo_k-1.2.1/exo_k/xtable.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,15 +281,15 @@
         self.convert_p_unit(p_unit=p_unit)
 
     def bin_down(self, wnedges=None, remove_zeros=False, write=0):
         """Method to bin down a xsec table to a new grid of wavenumbers (inplace).
 
         Parameters
         ----------
-            wnedges : array
+            wnedges : array, np.ndarray
                 Edges of the new bins of wavenumbers (cm-1) onto which the xsec
                 should be binned down.
                 if you want Nwnew bin in the end, wngrid.size must be Nwnew+1
                 wnedges[0] should be greater than self.wnedges[0]
                 wnedges[-1] should be lower than self.wnedges[-1]
             remove_zeros: bool, optional
                 If True, remove zeros in kdata.
@@ -318,15 +318,15 @@
         if remove_zeros : self.remove_zeros(deltalog_min_value=10.)
 
     def sample(self, wngrid, remove_zeros=False, log_interp=None):
         """Method to re sample a xsec table to a new grid of wavenumbers (inplace).
 
         Parameters
         ----------
-            wngrid : array
+            wngrid : array, np.ndarray
                 Location of the new wavenumbers points (cm-1)
         """
         wngrid=np.array(wngrid)
         wngrid_filter = np.where((wngrid <= self.wnedges[-1]) & (wngrid >= self.wnedges[0]))[0]
         Nnew=wngrid.size
         newxsec=np.zeros((self.Np,self.Nt,Nnew))
         if log_interp is None: log_interp=self._settings._log_interp
```

### Comparing `Exo_k-1.2.0/pyproject.toml` & `exo_k-1.2.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Exo_k"
-version = "1.2.0"
+version = "1.2.1"
 description = "Library to handle radiative opacities from various sources for atmospheric applications"
 authors = ["Jeremy Leconte <jeremy.leconte@u-bordeaux.fr>"]
 
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://forge.oasu.u-bordeaux.fr/jleconte/exo_k-public"
 repository = "https://forge.oasu.u-bordeaux.fr/jleconte/exo_k-public"
@@ -30,71 +30,85 @@
     "Topic :: Scientific/Engineering :: Astronomy",
     "Topic :: Scientific/Engineering :: Atmospheric Science",
     "Topic :: Scientific/Engineering :: Physics",
     "Topic :: Software Development :: Libraries",
 ]
 
 [tool.poetry-dynamic-versioning]
-enable = true
+enable = false
 vcs = "git"
 style = "pep440"
 bump = true
 pattern = "default-unprefixed"
 
 [tool.poetry.dependencies]
-python = ">=3.7.1, <3.10"
+python = ">=3.8, <3.12"
 
 numpy = ">=1.21.6"
-scipy = ">=1.7.3"
-numba = ">=0.55.2"
-llvmlite = ">=0.38.1"
-
-astropy = ">=4.3.1"
-h5py = ">=3.7.0"
-matplotlib = ">=3.5.2"
-pandas = ">=1.3.5"
+scipy = ">=1.10.1"
+numba = ">=0.57.0"
+llvmlite = ">=0.40.0"
+
+astropy = ">=5.0, <5.3"
+h5py = ">=3.8.0"
+matplotlib = ">=3.7.1"
+pandas = ">=2.0.2"
+
 
 [tool.poetry.group.doc.dependencies]
-nbclient= "^0.6.6"
-papermill = "^2.3.4"
+nbclient = "^0.6.8"
+papermill = "^2.4.0"
 
-Sphinx = "^5.0.2"
-nbsphinx = "^0.8.9"
-sphinx-autoapi = "^1.8.4"
-sphinx-rtd-theme = "^1.0.0"
+Sphinx = "^5.3.0"
+nbsphinx = "^0.8.12"
+nbsphinx-link = "^1.3.0"
+sphinx-autoapi = "^1.9.0"
+sphinx-rtd-theme = "^1.2.1"
 sphinx-autobuild = "^2021.3.14"
+sphinx-math-dollar = "^1.2.1"
+sphinx-paramlinks = "^0.5.4"
+sphinx-autodoc-typehints = "^1.23.0"
 
 [tool.poetry.group.dev.dependencies]
-poetryup = "^0.9.0"
+setuptools = "^67.8.0"
+
+types-decorator = "^5.1.8.3"
+netCDF4 = "^1.6.4"
 
 jupyter = "^1.0.0"
 
-nb-clean = "^2.1.0"
-pydocstyle = "^6.1.1"
 
-coverage = "^6.4.2"
+[tool.poetry.group.tools.dependencies]
+deptry = "^0.6.6"
+nb-clean = "^2.4.0"
+pydocstyle = { extras = ["toml"], version = "^6.3.0" }
+
+
+[tool.poetry.group.testing.dependencies]
+coverage = "^6.5.0"
 
-pytest = "^7.1.2"
+pytest = "^7.3.1"
 pytest-cov = "^3.0.0"
 pytest-clarity = "^1.0.1"
-pytest-colordots = "^1.1"
+pytest-mypy = "^0.9.1"
+pytest-sugar = "^0.9.7"
+pytest-xdist = { extras = ["psutil"], version = "^2.5.0" }
+
 pytest-parallel = "^0.1.1"
 pytest-regtest = "^1.5.0"
-pytest-regressions = "^2.3.1"
-pytest-xdist = { extras = ["psutil"], version = "^2.5.0" }
+pytest-regressions = "^2.4.2"
 
-GitPython = "^3.1.27"
 
-types-decorator = "^5.1.8"
-netCDF4 = "^1.6.0"
 
+[tool.poetry.group.test.dependencies]
+tox = "^4.6.0"
 
 [tool.pytest.ini_options]
 minversion = '7.0'
-addopts = '--quiet --capture=no -p no:warnings'
+addopts = '-p no:warnings --cov' # --capture=no
 testpaths = ['tests']
 
 
 [tool.coverage.report]
 show_missing = true
 exclude_lines = [
     'if TYPE_CHECKING:',
@@ -103,11 +117,17 @@
 ]
 
 [tool.coverage.run]
 omit = [
     "tests/*",
 ]
 
+[tool.deptry]
+ignore_notebooks = true
+
+[tool.pydocstyle]
+convention = 'numpy'
+#ignore = 'D105, D200, D205, D212, D213, D400, D413, D415, D417'
 
 [build-system]
-requires = ["poetry-core>=1.1.0b2", "poetry-dynamic-versioning"]
-build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core>=1.1.0", "poetry-dynamic-versioning"]
+build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `Exo_k-1.2.0/PKG-INFO` & `exo_k-1.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: exo-k
-Version: 1.2.0
+Version: 1.2.1
 Summary: Library to handle radiative opacities from various sources for atmospheric applications
 Home-page: https://forge.oasu.u-bordeaux.fr/jleconte/exo_k-public
 License: GPLv3
 Keywords: opacities,cross sections,correlated-k,spectra,atmosphere,atmospheric,exoplanet,radiative transfer
 Author: Jeremy Leconte
 Author-email: jeremy.leconte@u-bordeaux.fr
-Requires-Python: >=3.7.1,<3.10
+Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Jupyter
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -20,54 +20,59 @@
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries
-Requires-Dist: astropy (>=4.3.1)
-Requires-Dist: h5py (>=3.7.0)
-Requires-Dist: llvmlite (>=0.38.1)
-Requires-Dist: matplotlib (>=3.5.2)
-Requires-Dist: numba (>=0.55.2)
+Requires-Dist: astropy (>=5.0,<5.3)
+Requires-Dist: h5py (>=3.8.0)
+Requires-Dist: llvmlite (>=0.40.0)
+Requires-Dist: matplotlib (>=3.7.1)
+Requires-Dist: numba (>=0.57.0)
 Requires-Dist: numpy (>=1.21.6)
-Requires-Dist: pandas (>=1.3.5)
-Requires-Dist: scipy (>=1.7.3)
+Requires-Dist: pandas (>=2.0.2)
+Requires-Dist: scipy (>=1.10.1)
 Project-URL: Documentation, http://perso.astrophy.u-bordeaux.fr/~jleconte/exo_k-doc/index.html
 Project-URL: Repository, https://forge.oasu.u-bordeaux.fr/jleconte/exo_k-public
 Description-Content-Type: text/markdown
 
 # Exo_k
 
 Author: Jeremy Leconte (CNRS/LAB/Univ. Bordeaux)
 
 `Exo_k` is a Python 3 based library to handle radiative opacities from various sources for atmospheric applications.
+It now comes with a full-fledged 1D atmospheric evolution model.
+
 It enables you to:
 
 * Interpolate efficiently and easily in correlated-k and cross section tables.
 * Convert easily correlated-k and cross section tables from one format to another
   (hdf5, LMDZ GCM, Exomol, Nemesis, PetitCode, TauREx, ExoREM, ARCIS, etc.).
 * Adapt precomputed correlated-k tables to your needs by changing:
 
-  * the resolution and quadrature (g) grid,
+  * the spectral and quadrature (g) grids,
   * the pressure/temperature grid.
 * Create tables for a mix of gases using tables for individual gases.
 * Create your own tables from high-resolution spectra (for example from K-spectrum, Helios-K, etc.).
 * Use your data in an integrated radiative transfer framework to simulate planetary atmospheres.
+* Compute the physical state of planetary atmospheres in radiative-convective equilibrium.
   
 For a complete online documentation, checkout:
 http://perso.astrophy.u-bordeaux.fr/~jleconte/exo_k-doc/index.html
 
-In this repository, you'll find a [tutorial jupyter notebook](https://forge.oasu.u-bordeaux.fr/jleconte/exo_k-public/-/blob/public/tutorial-exo_k.ipynb) that will show you how to do all that
+In this repository, you'll find a [tutorial jupyter notebook](https://forge.oasu.u-bordeaux.fr/jleconte/exo_k-public/-/blob/public/tutorials/tutorial-exo_k.ipynb) that will show you how to do all that
 with concrete examples that you can run on your own machine. Many important concepts and options are
 presented along the way.
 
 Enjoy!
 
 J. Leconte
 
@@ -83,30 +88,24 @@
 (grant agreement n° 679030/WHIPLASH).
 
 The framework for this documentation has been developped by Aurelien Falco using Sphinx.
 The Framework for automatic testing has been developped by Alexandre Mechineau. 
 
 # last release (see past releases below)
 
-v1.2.0 (July 2022): The model for atmospheric evolution is finally stable and documented.
-The atm module has also seen several note worthy additions: surface albedo, oceans. 
-We also added a framework for an automatic test suite. In particular, we can test several python versions. Additional tests should rapidly come along.
-Rosseland and Planck mean opacities can now be computed from radiative tables. 
+v1.2.1 (June 2023): Fixes some minor bugs in the atmospheric evolution module.
+Addition of a contribution function in the atmospheric radiative transfer module. See the atmosphere tutorial for an example.
 
 # Installation
 
 Exo_k can be installed using pip (without cloning the repository;
 dependencies should be downloaded automatically):
 ```
 pip install exo_k
 ```
-Or by running the [setup.py](https://forge.oasu.u-bordeaux.fr/jleconte/exo_k-public/-/blob/public/setup.py) script in the cloned repository:
-```
-python setup.py install
-```
 
 # Usage
 
 To learn how to use `exo_k`, you can follow the [tutorial jupyter notebook](https://forge.oasu.u-bordeaux.fr/jleconte/exo_k-public/-/blob/public/tutorial-exo_k.ipynb).
 
 Have fun!
 
@@ -116,14 +115,19 @@
 * Code repository: https://forge.oasu.u-bordeaux.fr/jleconte/exo_k-public
 * Documentation: http://perso.astrophy.u-bordeaux.fr/~jleconte/exo_k-doc/index.html
 * Contact: jeremy.leconte at u-bordeaux.fr
 
 
 # past releases
 
+v1.2.0 (July 2022): The model for atmospheric evolution is finally stable and documented.
+The atm module has also seen several note worthy additions: surface albedo, oceans. 
+We also added a framework for an automatic test suite. In particular, we can test several python versions. Additional tests should rapidly come along.
+Rosseland and Planck mean opacities can now be computed from radiative tables. 
+
 v1.1.0 (August 2021): New scheme for the computation of atmospheric emission/transmission
 to ensure an improved numerical accuracy. The variable names to instantiate atm objects have
 changed accordingly (see tutorial). 
 
 v1.0.2 (June 2021): Adds a few missing dependencies. Enables computation of thermal
 emission spectra with scattering through the two-stream method (full documentation pending). 
 Enables creating Xtables for a mix of gases (CIA can be added as well). Solves some issues
```

