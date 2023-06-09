# Comparing `tmp/spin_phonon_suite-1.1.0.tar.gz` & `tmp/spin_phonon_suite-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spin_phonon_suite-1.1.0.tar", last modified: Mon Jun  5 14:15:09 2023, max compression
+gzip compressed data, was "spin_phonon_suite-1.2.0.tar", last modified: Fri Jun  9 11:27:02 2023, max compression
```

## Comparing `spin_phonon_suite-1.1.0.tar` & `spin_phonon_suite-1.2.0.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 14:15:09.481142 spin_phonon_suite-1.1.0/
--rw-rw-rw-   0 root         (0) root         (0)    35085 2023-06-05 14:14:39.000000 spin_phonon_suite-1.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3750 2023-06-05 14:15:09.480225 spin_phonon_suite-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3031 2023-06-05 14:14:39.000000 spin_phonon_suite-1.1.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      215 2023-06-05 14:14:39.000000 spin_phonon_suite-1.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 14:15:09.481142 spin_phonon_suite-1.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1680 2023-06-05 14:15:06.000000 spin_phonon_suite-1.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 14:15:09.479309 spin_phonon_suite-1.1.0/spin_phonon_suite/
--rw-rw-rw-   0 root         (0) root         (0)      152 2023-06-05 14:14:39.000000 spin_phonon_suite-1.1.0/spin_phonon_suite/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      105 2023-06-05 14:15:06.000000 spin_phonon_suite-1.1.0/spin_phonon_suite/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)    10740 2023-06-05 14:14:39.000000 spin_phonon_suite-1.1.0/spin_phonon_suite/cells.py
--rw-rw-rw-   0 root         (0) root         (0)    36219 2023-06-05 14:14:39.000000 spin_phonon_suite-1.1.0/spin_phonon_suite/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     3904 2023-06-05 14:14:39.000000 spin_phonon_suite-1.1.0/spin_phonon_suite/coordinates.py
--rw-rw-rw-   0 root         (0) root         (0)     1309 2023-06-05 14:14:39.000000 spin_phonon_suite-1.1.0/spin_phonon_suite/derivative.py
--rw-rw-rw-   0 root         (0) root         (0)    22303 2023-06-05 14:14:39.000000 spin_phonon_suite-1.1.0/spin_phonon_suite/lvc.py
--rw-rw-rw-   0 root         (0) root         (0)    18786 2023-06-05 14:14:39.000000 spin_phonon_suite-1.1.0/spin_phonon_suite/vibrations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 14:15:09.480225 spin_phonon_suite-1.1.0/spin_phonon_suite.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3750 2023-06-05 14:15:09.000000 spin_phonon_suite-1.1.0/spin_phonon_suite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      526 2023-06-05 14:15:09.000000 spin_phonon_suite-1.1.0/spin_phonon_suite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 14:15:09.000000 spin_phonon_suite-1.1.0/spin_phonon_suite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-05 14:15:09.000000 spin_phonon_suite-1.1.0/spin_phonon_suite.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-05 14:15:09.000000 spin_phonon_suite-1.1.0/spin_phonon_suite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-05 14:15:09.000000 spin_phonon_suite-1.1.0/spin_phonon_suite.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 11:27:02.067175 spin_phonon_suite-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35085 2023-06-09 11:26:26.000000 spin_phonon_suite-1.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3750 2023-06-09 11:27:02.066186 spin_phonon_suite-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3031 2023-06-09 11:26:26.000000 spin_phonon_suite-1.2.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      215 2023-06-09 11:26:26.000000 spin_phonon_suite-1.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 11:27:02.067175 spin_phonon_suite-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1680 2023-06-09 11:26:59.000000 spin_phonon_suite-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 11:27:02.065197 spin_phonon_suite-1.2.0/spin_phonon_suite/
+-rw-rw-rw-   0 root         (0) root         (0)      152 2023-06-09 11:26:26.000000 spin_phonon_suite-1.2.0/spin_phonon_suite/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      105 2023-06-09 11:26:59.000000 spin_phonon_suite-1.2.0/spin_phonon_suite/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10850 2023-06-09 11:26:26.000000 spin_phonon_suite-1.2.0/spin_phonon_suite/cells.py
+-rw-rw-rw-   0 root         (0) root         (0)    34732 2023-06-09 11:26:26.000000 spin_phonon_suite-1.2.0/spin_phonon_suite/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1309 2023-06-09 11:26:26.000000 spin_phonon_suite-1.2.0/spin_phonon_suite/derivative.py
+-rw-rw-rw-   0 root         (0) root         (0)    22303 2023-06-09 11:26:26.000000 spin_phonon_suite-1.2.0/spin_phonon_suite/lvc.py
+-rw-rw-rw-   0 root         (0) root         (0)    18786 2023-06-09 11:26:26.000000 spin_phonon_suite-1.2.0/spin_phonon_suite/vibrations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 11:27:02.066186 spin_phonon_suite-1.2.0/spin_phonon_suite.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3750 2023-06-09 11:27:02.000000 spin_phonon_suite-1.2.0/spin_phonon_suite.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      493 2023-06-09 11:27:02.000000 spin_phonon_suite-1.2.0/spin_phonon_suite.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 11:27:02.000000 spin_phonon_suite-1.2.0/spin_phonon_suite.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-09 11:27:02.000000 spin_phonon_suite-1.2.0/spin_phonon_suite.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-09 11:27:02.000000 spin_phonon_suite-1.2.0/spin_phonon_suite.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-09 11:27:02.000000 spin_phonon_suite-1.2.0/spin_phonon_suite.egg-info/top_level.txt
```

### Comparing `spin_phonon_suite-1.1.0/LICENSE` & `spin_phonon_suite-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spin_phonon_suite-1.1.0/PKG-INFO` & `spin_phonon_suite-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spin_phonon_suite
-Version: 1.1.0
+Version: 1.2.0
 Summary: A package for performing spin-phonon coupling calculations with openMOLCAS, VASP, and Gaussian
 Home-page: https://gitlab.com/chilton-group/spin_phonon_suite
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Project-URL: Bug Tracker, https://gitlab.com/chilton-group/spin_phonon_suite/-/issues
 Project-URL: Documentation, https://chilton-group.gitlab.io/spin_phonon_suite
 Classifier: Programming Language :: Python :: 3
```

### Comparing `spin_phonon_suite-1.1.0/README.md` & `spin_phonon_suite-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `spin_phonon_suite-1.1.0/setup.py` & `spin_phonon_suite-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import setuptools
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 # DO NOT EDIT THIS NUMBER!
 # IT IS AUTOMATICALLY CHANGED BY python-semantic-release
-__version__ = "1.1.0"
+__version__ = "1.2.0"
 
 setuptools.setup(
     name='spin_phonon_suite',
     version=__version__,
     author='Chilton Group',
     author_email='nicholas.chilton@manchester.ac.uk',
     description='A package for performing spin-phonon coupling calculations with openMOLCAS, VASP, and Gaussian', # noqa
```

### Comparing `spin_phonon_suite-1.1.0/spin_phonon_suite/cells.py` & `spin_phonon_suite-1.2.0/spin_phonon_suite/cells.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,21 @@
 from phonopy.interface.vasp import read_vasp
 import numpy as np
 import numpy.linalg as la
 import molvis.core as mvis
 import matplotlib.cm as cm
 
 
-def generate_molecular_graph(structure, equivalent_positions):
+def generate_molecular_graph(structure):
     strategy = IsayevNN(cutoff=3.0, allow_pathological=True)
     graph = StructureGraph.with_local_env_strategy(structure, strategy, weights=True)
 
+    sym_structure = SpacegroupAnalyzer(structure).get_symmetrized_structure()
+    equivalent_positions = sym_structure.as_dict()['equivalent_positions']
+
     # build directed multi-graph
     twoway = nx.MultiDiGraph(graph.graph)
     # nodes are labelled by species
     nx.set_node_attributes(twoway,
         {node: {'symm_equiv': (structure[node].specie, equivalent_positions[node])} for node in twoway})
 
     def flip_edge(u, v, data):
@@ -95,15 +98,15 @@
 
 def get_unique_entities(structure):
 
     sym_structure = SpacegroupAnalyzer(structure).get_symmetrized_structure()
     structure_dict = sym_structure.as_dict()
     equivalent_positions = structure_dict['equivalent_positions']
 
-    molecular_graph = generate_molecular_graph(structure, equivalent_positions)
+    molecular_graph = generate_molecular_graph(structure)
     connected_graphs = split_molecular_graph(molecular_graph, filter_unique=True)
     indices, molecules = zip(*map(lambda x: extract_molecule(structure, x), connected_graphs))
 
     elements = [site.specie.symbol for site in structure]
 
     mappings = [[equivalent_positions[idx] for idx in shift_dict]
                 for shift_dict in indices]
```

### Comparing `spin_phonon_suite-1.1.0/spin_phonon_suite/cli.py` & `spin_phonon_suite-1.2.0/spin_phonon_suite/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 from angmom_suite import crystal
 from angmom_suite.basis import Level
 from angmom_suite.multi_electron import Ion
 import molvis.core as mvis
 from pymatgen.core.structure import Molecule, Structure
 from pymatgen.transformations.site_transformations import TranslateSitesTransformation
 
-from .coordinates import CoordinateInfo
 from .derivative import print_tau_style, read_tau_style
 from .lvc import LVC, generate_lvc_input, make_lvc_evaluator, ANG2BOHR, \
     LVCModelHamiltonian, LVCAdiabaticEnergies, LVCDiabaticHamiltonian
 from .vibrations import Harmonic
 from . import cells
 
 plt.rcParams['font.family'] = "Arial"
@@ -54,21 +53,14 @@
 def str_int(x):
     try:
         return int(x)
     except ValueError:
         return str(x)
 
 
-def coords_func(args):
-    sp_data = CoordinateInfo.from_args(args)
-    sp_data.to_file(args.distortion_info)
-
-    return
-
-
 def lvc_func(args):
 
     if args.add is not None:
         def join(a, b):
             return a.join(b, xyzp.load_xyz(args.reference_xyz)[1] * ANG2BOHR)
         lvc = reduce(join, (LVC.from_file(f_lvc) for f_lvc in args.add))
 
@@ -680,69 +672,14 @@
     parser = ArgumentParser(
             description=description,
             formatter_class=RawDescriptionHelpFormatter
             )
 
     subparsers = parser.add_subparsers(dest='prog')
 
-    coords = subparsers.add_parser('coords')
-    coords.set_defaults(func=coords_func)
-
-    coords.add_argument(
-        '-D',
-        '--distortion_info',
-        type=str,
-        help='HDF5 database containing information about the distortion.'
-    )
-
-    coords.add_argument(
-        '--num_atoms',
-        type=int,
-        default=1,
-        help='Number of atoms.'
-    )
-
-    coords.add_argument(
-        '--mode_wise',
-        nargs='*',
-        default=None,
-        type=parse_range,
-        help='Mode indices to be included in distortions calculations ' +
-             '- activates mode-wise distortions.'
-        )
-
-    coords.add_argument(
-        '--atomic',
-        nargs='*',
-        default=None,
-        type=parse_range,
-        help='Atomic indices to be included in distortion calculations ' +
-             '- activates atomic distortions.'
-        )
-
-    coords.add_argument(
-        '--num_steps',
-        type=int,
-        default=0,
-        help='Number of distortion steps.'
-    )
-
-    coords.add_argument(
-        '--order',
-        type=int,
-        default=1,
-        help='Order of distortion.'
-    )
-
-    coords.add_argument(
-        '--constant_step',
-        type=float,
-        help='Step size factor for constant displacement.'
-    )
-
     evaluate = subparsers.add_parser('eval')
     evaluate.set_defaults(func=eval_func)
 
     evaluate.add_argument(
         '-H',
         '--Help',
         action=FunctionHelp,
@@ -752,17 +689,15 @@
     evaluate.add_argument(
         '-L',
         '--lvc_data',
         type=str,
         help='HDF5 database containing the LVC parameters.'
     )
 
-    coords = evaluate.add_mutually_exclusive_group()
-
-    coords.add_argument(
+    evaluate.add_argument(
         '-V',
         '--vibration_info',
         type=str,
         help=('HDF5 database containing information about the vibrations.'
               'Derivatives are evaluated in the basis of dimension-less'
               'mass-frequency weighted normal mode coordinates.')
     )
```

### Comparing `spin_phonon_suite-1.1.0/spin_phonon_suite/derivative.py` & `spin_phonon_suite-1.2.0/spin_phonon_suite/derivative.py`

 * *Files identical despite different names*

### Comparing `spin_phonon_suite-1.1.0/spin_phonon_suite/lvc.py` & `spin_phonon_suite-1.2.0/spin_phonon_suite/lvc.py`

 * *Files identical despite different names*

### Comparing `spin_phonon_suite-1.1.0/spin_phonon_suite/vibrations.py` & `spin_phonon_suite-1.2.0/spin_phonon_suite/vibrations.py`

 * *Files identical despite different names*

### Comparing `spin_phonon_suite-1.1.0/spin_phonon_suite.egg-info/PKG-INFO` & `spin_phonon_suite-1.2.0/spin_phonon_suite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spin-phonon-suite
-Version: 1.1.0
+Version: 1.2.0
 Summary: A package for performing spin-phonon coupling calculations with openMOLCAS, VASP, and Gaussian
 Home-page: https://gitlab.com/chilton-group/spin_phonon_suite
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Project-URL: Bug Tracker, https://gitlab.com/chilton-group/spin_phonon_suite/-/issues
 Project-URL: Documentation, https://chilton-group.gitlab.io/spin_phonon_suite
 Classifier: Programming Language :: Python :: 3
```

