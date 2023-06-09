# Comparing `tmp/hypothesis-rdkit-0.4.tar.gz` & `tmp/hypothesis-rdkit-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypothesis-rdkit-0.4.tar", last modified: Tue May 23 15:33:44 2023, max compression
+gzip compressed data, was "hypothesis-rdkit-0.5.tar", last modified: Fri Jun  9 08:53:58 2023, max compression
```

## Comparing `hypothesis-rdkit-0.4.tar` & `hypothesis-rdkit-0.5.tar`

### file list

```diff
@@ -1,23 +1,28 @@
-drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2023-05-23 15:33:44.769496 hypothesis-rdkit-0.4/
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1081 2023-03-06 20:54:00.000000 hypothesis-rdkit-0.4/LICENSE
--rw-rw-r--   0 hirte     (1000) hirte     (1000)       38 2023-02-19 23:12:21.000000 hypothesis-rdkit-0.4/MANIFEST.in
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1475 2023-05-23 15:33:44.769496 hypothesis-rdkit-0.4/PKG-INFO
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      829 2023-02-19 23:12:21.000000 hypothesis-rdkit-0.4/README.md
-drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2023-05-23 15:33:44.769496 hypothesis-rdkit-0.4/hypothesis_rdkit/
--rw-rw-r--   0 hirte     (1000) hirte     (1000)       24 2023-02-19 23:11:07.000000 hypothesis-rdkit-0.4/hypothesis_rdkit/__init__.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)   441809 2023-05-23 15:28:37.000000 hypothesis-rdkit-0.4/hypothesis_rdkit/fragments.smi
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      199 2023-02-19 23:12:21.000000 hypothesis-rdkit-0.4/hypothesis_rdkit/hook.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     6131 2023-05-23 15:28:37.000000 hypothesis-rdkit-0.4/hypothesis_rdkit/strategy.py
-drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2023-05-23 15:33:44.769496 hypothesis-rdkit-0.4/hypothesis_rdkit.egg-info/
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1475 2023-05-23 15:33:44.000000 hypothesis-rdkit-0.4/hypothesis_rdkit.egg-info/PKG-INFO
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      459 2023-05-23 15:33:44.000000 hypothesis-rdkit-0.4/hypothesis_rdkit.egg-info/SOURCES.txt
--rw-rw-r--   0 hirte     (1000) hirte     (1000)        1 2023-05-23 15:33:44.000000 hypothesis-rdkit-0.4/hypothesis_rdkit.egg-info/dependency_links.txt
--rw-rw-r--   0 hirte     (1000) hirte     (1000)       62 2023-05-23 15:33:44.000000 hypothesis-rdkit-0.4/hypothesis_rdkit.egg-info/entry_points.txt
--rw-rw-r--   0 hirte     (1000) hirte     (1000)       30 2023-05-23 15:33:44.000000 hypothesis-rdkit-0.4/hypothesis_rdkit.egg-info/requires.txt
--rw-rw-r--   0 hirte     (1000) hirte     (1000)       17 2023-05-23 15:33:44.000000 hypothesis-rdkit-0.4/hypothesis_rdkit.egg-info/top_level.txt
--rw-rw-r--   0 hirte     (1000) hirte     (1000)       38 2023-05-23 15:33:44.769496 hypothesis-rdkit-0.4/setup.cfg
--rw-rw-r--   0 hirte     (1000) hirte     (1000)     1006 2023-05-23 15:33:30.000000 hypothesis-rdkit-0.4/setup.py
-drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2023-05-23 15:33:44.769496 hypothesis-rdkit-0.4/tests/
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      648 2023-02-19 23:12:21.000000 hypothesis-rdkit-0.4/tests/test_mol_blocks.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      665 2023-05-23 15:28:37.000000 hypothesis-rdkit-0.4/tests/test_mols.py
--rw-rw-r--   0 hirte     (1000) hirte     (1000)      607 2023-02-19 23:12:21.000000 hypothesis-rdkit-0.4/tests/test_smiles.py
+drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2023-06-09 08:53:58.112559 hypothesis-rdkit-0.5/
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1081 2023-03-06 20:54:00.000000 hypothesis-rdkit-0.5/LICENSE
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)       81 2023-06-09 08:49:07.000000 hypothesis-rdkit-0.5/MANIFEST.in
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1785 2023-06-09 08:53:58.112559 hypothesis-rdkit-0.5/PKG-INFO
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1118 2023-06-09 08:49:07.000000 hypothesis-rdkit-0.5/README.md
+drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2023-06-09 08:53:58.112559 hypothesis-rdkit-0.5/hypothesis_rdkit/
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)       24 2023-02-19 23:11:07.000000 hypothesis-rdkit-0.5/hypothesis_rdkit/__init__.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     9399 2023-06-09 08:49:07.000000 hypothesis-rdkit-0.5/hypothesis_rdkit/fragment.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000) 22377762 2023-06-09 08:49:07.000000 hypothesis-rdkit-0.5/hypothesis_rdkit/fragments_100000.pkl
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)  2730143 2023-06-09 08:49:07.000000 hypothesis-rdkit-0.5/hypothesis_rdkit/fragments_100000.smi
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)  5932863 2023-06-09 08:49:07.000000 hypothesis-rdkit-0.5/hypothesis_rdkit/fragments_30000.pkl
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)   725332 2023-06-09 08:49:07.000000 hypothesis-rdkit-0.5/hypothesis_rdkit/fragments_30000.smi
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      199 2023-02-19 23:12:21.000000 hypothesis-rdkit-0.5/hypothesis_rdkit/hook.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     8201 2023-06-09 08:49:07.000000 hypothesis-rdkit-0.5/hypothesis_rdkit/strategy.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     3685 2023-06-09 08:49:07.000000 hypothesis-rdkit-0.5/hypothesis_rdkit/util.py
+drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2023-06-09 08:53:58.112559 hypothesis-rdkit-0.5/hypothesis_rdkit.egg-info/
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1785 2023-06-09 08:53:58.000000 hypothesis-rdkit-0.5/hypothesis_rdkit.egg-info/PKG-INFO
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      632 2023-06-09 08:53:58.000000 hypothesis-rdkit-0.5/hypothesis_rdkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)        1 2023-06-09 08:53:58.000000 hypothesis-rdkit-0.5/hypothesis_rdkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)       62 2023-06-09 08:53:58.000000 hypothesis-rdkit-0.5/hypothesis_rdkit.egg-info/entry_points.txt
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)       45 2023-06-09 08:53:58.000000 hypothesis-rdkit-0.5/hypothesis_rdkit.egg-info/requires.txt
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)       17 2023-06-09 08:53:58.000000 hypothesis-rdkit-0.5/hypothesis_rdkit.egg-info/top_level.txt
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)       38 2023-06-09 08:53:58.112559 hypothesis-rdkit-0.5/setup.cfg
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)     1025 2023-06-09 08:49:07.000000 hypothesis-rdkit-0.5/setup.py
+drwxrwxr-x   0 hirte     (1000) hirte     (1000)        0 2023-06-09 08:53:58.112559 hypothesis-rdkit-0.5/tests/
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      648 2023-02-19 23:12:21.000000 hypothesis-rdkit-0.5/tests/test_mol_blocks.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      916 2023-06-09 08:49:07.000000 hypothesis-rdkit-0.5/tests/test_mols.py
+-rw-rw-r--   0 hirte     (1000) hirte     (1000)      607 2023-02-19 23:12:21.000000 hypothesis-rdkit-0.5/tests/test_smiles.py
```

### Comparing `hypothesis-rdkit-0.4/LICENSE` & `hypothesis-rdkit-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hypothesis-rdkit-0.4/PKG-INFO` & `hypothesis-rdkit-0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,55 +1,65 @@
 Metadata-Version: 2.1
 Name: hypothesis-rdkit
-Version: 0.4
+Version: 0.5
 Home-page: https://github.com/shirte/hypothesis-rdkit
 Maintainer: Steffen Hirte
 Maintainer-email: shirte@users.noreply.github.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Framework :: Hypothesis
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: test
 License-File: LICENSE
 
 # hypothesis-rdkit
 
+A strategy to generate random molecules for the hypothesis testing framework.
+
+![demo](demo.png)
+
+
 ## Installation
 
 ```sh
 pip install -U hypothesis-rdkit
 ```
 
 ## Usage
 
-The module ```hypothesis-rdkit``` provides a strategy for the generating RDKit 
+The module ```hypothesis-rdkit``` provides a strategy for generating RDKit 
 molecules. During the installation of the package, this strategy is linked to the 
 ```rdkit.Chem.Mol``` type:
 
 
 ```python
 from hypothesis import given
 from rdkit.Chem import Mol
 
 @given(...)
 def test_molecule_method(mol : Mol):
+    # mol is a randomly generated molecule
     assert mol.GetNumAtoms() > 0
-    # ...
 ```
 
 You can use the ```mols``` strategy directly for further customization:
 
 ```python
 from hypothesis import given  # import hypothesis before hypothesis_rdkit!
 from hypothesis_rdkit import mols
 from rdkit.Chem import GetMolFrags, Mol
+from rdkit.Chem.rdMolDescriptors import CalcNumRotatableBonds
 
-@given(mols(n_connected_components=2))
+@given(mols(n_connected_components=2, max_num_rotatable_bonds=5))
 def test_molecule_mixtures(mol : Mol):
     frags = GetMolFrags(mol, asMols=True)
     assert len(frags) == 2
+
+    for frag in frags:
+        assert CalcNumRotatableBonds(frag) <= 5
 ```
```

### Comparing `hypothesis-rdkit-0.4/hypothesis_rdkit.egg-info/PKG-INFO` & `hypothesis-rdkit-0.5/hypothesis_rdkit.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,55 +1,65 @@
 Metadata-Version: 2.1
 Name: hypothesis-rdkit
-Version: 0.4
+Version: 0.5
 Home-page: https://github.com/shirte/hypothesis-rdkit
 Maintainer: Steffen Hirte
 Maintainer-email: shirte@users.noreply.github.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Framework :: Hypothesis
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: test
 License-File: LICENSE
 
 # hypothesis-rdkit
 
+A strategy to generate random molecules for the hypothesis testing framework.
+
+![demo](demo.png)
+
+
 ## Installation
 
 ```sh
 pip install -U hypothesis-rdkit
 ```
 
 ## Usage
 
-The module ```hypothesis-rdkit``` provides a strategy for the generating RDKit 
+The module ```hypothesis-rdkit``` provides a strategy for generating RDKit 
 molecules. During the installation of the package, this strategy is linked to the 
 ```rdkit.Chem.Mol``` type:
 
 
 ```python
 from hypothesis import given
 from rdkit.Chem import Mol
 
 @given(...)
 def test_molecule_method(mol : Mol):
+    # mol is a randomly generated molecule
     assert mol.GetNumAtoms() > 0
-    # ...
 ```
 
 You can use the ```mols``` strategy directly for further customization:
 
 ```python
 from hypothesis import given  # import hypothesis before hypothesis_rdkit!
 from hypothesis_rdkit import mols
 from rdkit.Chem import GetMolFrags, Mol
+from rdkit.Chem.rdMolDescriptors import CalcNumRotatableBonds
 
-@given(mols(n_connected_components=2))
+@given(mols(n_connected_components=2, max_num_rotatable_bonds=5))
 def test_molecule_mixtures(mol : Mol):
     frags = GetMolFrags(mol, asMols=True)
     assert len(frags) == 2
+
+    for frag in frags:
+        assert CalcNumRotatableBonds(frag) <= 5
 ```
```

### Comparing `hypothesis-rdkit-0.4/setup.py` & `hypothesis-rdkit-0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-from setuptools import setup, find_packages
-
+from setuptools import find_packages, setup
 
 setup(
     name="hypothesis-rdkit",
-    version="0.4",
+    version="0.5",
     maintainer="Steffen Hirte",
     maintainer_email="shirte@users.noreply.github.com",
     packages=find_packages(),
     url="https://github.com/shirte/hypothesis-rdkit",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     license="MIT",
     license_files=("LICENSE",),
     install_requires=["hypothesis"],
-    extras_require={"dev": ["black", "isort"]},
+    extras_require={"dev": ["black", "isort"], "test": ["pytest"]},
     entry_points={"hypothesis": {"_ = hypothesis_rdkit.hook:_hypothesis_setup_hook"}},
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Software Development :: Testing",
```

### Comparing `hypothesis-rdkit-0.4/tests/test_mol_blocks.py` & `hypothesis-rdkit-0.5/tests/test_mol_blocks.py`

 * *Files identical despite different names*

### Comparing `hypothesis-rdkit-0.4/tests/test_mols.py` & `hypothesis-rdkit-0.5/tests/test_smiles.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from hypothesis import given
-from hypothesis_rdkit import mols
-from rdkit.Chem import Mol, MolFromSmiles, GetMolFrags
+from hypothesis_rdkit import smiles
+from rdkit.Chem import MolFromSmiles, GetMolFrags
 
 
 dummy_pattern = MolFromSmiles("[*]")
 
 
-@given(...)
-def test_mols(mol: Mol):
-    # mols have atoms
+@given(smiles())
+def test_smiles(smiles: str):
+    # smiles are valid
+    mol = MolFromSmiles(smiles)
+    assert mol is not None
+
+    # mols from smiles have atoms
     assert len(mol.GetAtoms()) > 0
 
-    # mols have no dummy atoms
+    # mols from smiles have no dummy atoms
     assert not mol.HasSubstructMatch(dummy_pattern)
 
     # by default, mols consist of one single connected component
     frags = GetMolFrags(mol, asMols=True, sanitizeFrags=False)
     assert len(frags) == 1
-
-
-@given(mols(n_connected_components=3))
-def test_connected_components(mol: Mol):
-    frags = GetMolFrags(mol, asMols=True, sanitizeFrags=False)
-    assert len(frags) == 3
```

