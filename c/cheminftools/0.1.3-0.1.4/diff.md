# Comparing `tmp/cheminftools-0.1.3.tar.gz` & `tmp/cheminftools-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cheminftools-0.1.3.tar", last modified: Thu Jun  1 07:47:17 2023, max compression
+gzip compressed data, was "cheminftools-0.1.4.tar", last modified: Thu Jun  8 22:06:21 2023, max compression
```

## Comparing `cheminftools-0.1.3.tar` & `cheminftools-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:47:17.407322 cheminftools-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-06-01 07:47:17.407322 cheminftools-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-06-01 07:47:01.000000 cheminftools-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:47:17.403322 cheminftools-0.1.3/cheminftools/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-01 07:47:01.000000 cheminftools-0.1.3/cheminftools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:47:17.403322 cheminftools-0.1.3/cheminftools/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 07:47:01.000000 cheminftools-0.1.3/cheminftools/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-06-01 07:47:01.000000 cheminftools-0.1.3/cheminftools/tools/featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7655 2023-06-01 07:47:01.000000 cheminftools-0.1.3/cheminftools/tools/filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)    17757 2023-06-01 07:47:01.000000 cheminftools-0.1.3/cheminftools/tools/sanitizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-06-01 07:47:01.000000 cheminftools-0.1.3/cheminftools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:47:17.403322 cheminftools-0.1.3/cheminftools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-06-01 07:47:17.000000 cheminftools-0.1.3/cheminftools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-01 07:47:17.000000 cheminftools-0.1.3/cheminftools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 07:47:17.000000 cheminftools-0.1.3/cheminftools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 07:47:17.000000 cheminftools-0.1.3/cheminftools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-01 07:47:17.000000 cheminftools-0.1.3/cheminftools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-01 07:47:17.000000 cheminftools-0.1.3/cheminftools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 07:47:17.407322 cheminftools-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-01 07:47:01.000000 cheminftools-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:06:21.676814 cheminftools-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    10918 2023-06-08 22:06:21.676814 cheminftools-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-06-08 22:05:49.000000 cheminftools-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:06:21.672814 cheminftools-0.1.4/cheminftools/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-08 22:05:49.000000 cheminftools-0.1.4/cheminftools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:06:21.672814 cheminftools-0.1.4/cheminftools/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:05:49.000000 cheminftools-0.1.4/cheminftools/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-08 22:05:49.000000 cheminftools-0.1.4/cheminftools/data/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-06-08 22:05:49.000000 cheminftools-0.1.4/cheminftools/data/data_gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-08 22:05:49.000000 cheminftools-0.1.4/cheminftools/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:06:21.672814 cheminftools-0.1.4/cheminftools/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:05:49.000000 cheminftools-0.1.4/cheminftools/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-06-08 22:05:49.000000 cheminftools-0.1.4/cheminftools/tools/featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-06-08 22:05:49.000000 cheminftools-0.1.4/cheminftools/tools/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17773 2023-06-08 22:05:49.000000 cheminftools-0.1.4/cheminftools/tools/sanitizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-06-08 22:05:49.000000 cheminftools-0.1.4/cheminftools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:06:21.672814 cheminftools-0.1.4/cheminftools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10918 2023-06-08 22:06:21.000000 cheminftools-0.1.4/cheminftools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-08 22:06:21.000000 cheminftools-0.1.4/cheminftools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 22:06:21.000000 cheminftools-0.1.4/cheminftools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 22:06:21.000000 cheminftools-0.1.4/cheminftools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-08 22:06:21.000000 cheminftools-0.1.4/cheminftools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-08 22:06:21.000000 cheminftools-0.1.4/cheminftools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 22:06:21.676814 cheminftools-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-08 22:05:49.000000 cheminftools-0.1.4/setup.py
```

### Comparing `cheminftools-0.1.3/PKG-INFO` & `cheminftools-0.1.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: cheminftools
-Version: 0.1.3
-Summary: A collection of tools for daily cheminformatics tasks.
-Home-page: https://github.com/marcossantanaioc/cheminftools
-Author: marcossantanaioc
-Author-email: marcosvssantana@gmail.com
-License: Apache Software License 2.0
-Keywords: cheminformatics computational chemistry rdkit
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-
 cheminftools
 ================
 
 ## Installation
 
 > From GitHub repo:
     ```pip install git+https://github.com/marcossantanaioc/cheminftools.git```
@@ -181,7 +162,37 @@
 array([[0, 0, 0, 0, 0],
        [0, 0, 0, 0, 0],
        [0, 0, 0, 0, 0],
        [0, 0, 0, 0, 0],
        [0, 0, 0, 0, 0]], dtype=uint8)
 
 ```
+# Collecting data from ChEMBL
+The current version of cheminftools support queries to ChEMBL based on UNIPROT accession codes.
+It should be straightforward to get activity data for multiple targets using the `ChemblFetcher` class.
+Users can find the latest version (and also older ones) of ChEMBL on the official [page](https://ftp.ebi.ac.uk/pub/databases/chembl/ChEMBLdb/latest/).
+Installation instructions come together with each ChEMBL release.
+
+`ChbemlFetcher` expects a configuration file for the database. This file includes information such as
+the host, user, password and port to connect to the database. 
+An example is shown below:
+
+```markdown
+[postgresql]
+host = localhost
+database = customer
+user = postgres
+password = admindb
+port = 5432
+```
+
+```python
+from cheminftools.data.data_gather import ChemblFetcher
+
+target_uniprot = ['P00742', 'P50613']
+chembl = ChemblFetcher(database_config_filename='database.ini',  # Path to configuration file. You can find \an example in the cheminftools.examples folder
+                       database_name='chembl',  # Name of database
+                       version='32')  # ChEMBL version to use
+df = chembl.query_target_uniprot(target_uniprot=target_uniprot)
+```
+The output is a pandas DataFrame with the desired activity types (e.g. IC50, Kd, Ki)
+for each target in `target_uniprot`.
```

### Comparing `cheminftools-0.1.3/cheminftools/tools/filtering.py` & `cheminftools-0.1.4/cheminftools/tools/filtering.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-from typing import Dict, Any, List
 import logging
-import pandas as pd
-from rdkit import Chem
 import sys
+from typing import Dict, Any, List
+
+import pandas as pd
 from joblib import cpu_count
+from rdkit import Chem
 from rdkit.Chem import FilterCatalog
+
 from cheminftools.utils import MolBatcher
 
 logging.basicConfig(level=logging.INFO, stream=sys.stdout, datefmt='%Y/%m/%d')
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
 
 
@@ -90,15 +92,29 @@
             catalog.AddEntry(FilterCatalog.FilterCatalogEntry(pname_final, fil))
             catalog.GetEntry(i).SetProp('Scope', smarts)
 
         self.catalog = catalog
         return catalog
 
 
-def get_alerts(smi: str, catalog: FilterCatalog.FilterCatalog) -> pd.DataFrame:
+def get_one_alert(smi: str, catalog: FilterCatalog.FilterCatalog) -> pd.DataFrame:
+    """
+    Finds alerts for one SMILES.
+
+    Parameters
+    ----------
+    smi
+        input SMILES.
+    catalog
+        a FilterCatalog object.
+    Returns
+    -------
+        Output DataFrame with alerts for `smi`.
+    """
+
     results = []
     info_names = [x.split('key=')[1] for x in catalog.GetEntryWithIdx(0).GetDescription().split('__') if 'key=' in x]
     mol = Chem.MolFromSmiles(smi)
 
     entries = catalog.GetMatches(mol)
 
     if len(entries) == 0:
@@ -112,14 +128,21 @@
 
     results = pd.concat(results).drop_duplicates()
     results['SMILES'] = smi
     results.reset_index(drop=True, inplace=True)
     return results
 
 
+def get_alerts_from_smiles_list(idxs, smiles_list: List[str], catalog: FilterCatalog.FilterCatalog) -> pd.DataFrame:
+    res = [get_one_alert(smi=smiles_list[i], catalog=catalog) for i in idxs]
+    if len(res) == 1:
+        return res[0]
+    return pd.concat(res)
+
+
 class MolFilter:
     @classmethod
     def filter(cls, df: pd.DataFrame, conditions: Dict[str, Dict[str, Any]]) -> pd.DataFrame:
         conditions = parse_conditions(conditions)
         logger.info(f'Filter conditions: {conditions}')
         return df.query(conditions)
 
@@ -128,22 +151,22 @@
                    n_workers: int = None, pause: int = 1):
 
         if n_workers is None:
             n_workers = cpu_count()
 
         logger.info('Processing SMILES.')
 
-        batcher = MolBatcher(get_alerts,
+        batcher = MolBatcher(get_alerts_from_smiles_list,
                              smiles_list=smiles_list,
                              catalog=catalog,
                              chunk_size=chunk_size,
                              n_workers=n_workers,
                              pause=pause)
 
-        all_alerts = pd.concat(batcher)
+        all_alerts = next(iter(batcher))
 
         if all_alerts.empty:
             pass
 
         n_flagged = len(all_alerts['SMILES'].unique())
         most_common_alert = all_alerts['SMARTS'].mode().tolist()
         most_common_desc = all_alerts[all_alerts.columns[0]].mode().tolist()
@@ -199,21 +222,20 @@
                            n_workers=n_workers,
                            pause=pause,
                            filters=filters)
 
     @classmethod
     def from_list(cls, smiles_list: List[str],
                   catalog: FilterCatalog.FilterCatalog,
-                  smiles_column: str,
                   chunk_size: int = 64,
                   n_workers: int = 1,
                   pause: int = 0,
                   filters: Dict[str, Dict[str, Any]] = {}):
 
         df = pd.DataFrame({'SMILES': smiles_list, 'ID': list(range(len(smiles_list)))})
         return cls.from_df(df,
                            catalog=catalog,
-                           smiles_column=smiles_column,
+                           smiles_column='SMILES',
                            chunk_size=chunk_size,
                            n_workers=n_workers,
                            pause=pause,
                            filters=filters)
```

### Comparing `cheminftools-0.1.3/cheminftools/tools/sanitizer.py` & `cheminftools-0.1.4/cheminftools/tools/sanitizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,29 +264,29 @@
     Parameters
     ----------
     data
         Input DataFrame.
     smiles_column
         Name of column with SMILES.
     act_column
-        Name of column with activity data.
+        Name of column with activity examples.
         It doesn't need to be activity - any
         numberical value is ok.
     cols_to_check
         Relevant columns to use for aggregation.
         See pandas groupby operation for detailed
         explanation.
     keep
         Which compound to keep
         first means the one with highest ´act_column´ value.
         last will keep the one with lowest ´act_column´ value.
 
     Returns
     -------
-        Aggregated version of data.
+        Aggregated version of examples.
 
     """
     assert keep in ['first', 'last']
     data = data.copy()
 
     # Generate inchikeys and stereo info
     logger.info(f'Converting {smiles_column} into inchikeys.')
@@ -351,30 +351,30 @@
     elif not to_keep.empty and keep == 'last':
         duplis_kept = to_keep.groupby('inchikey', group_keys=False).apply(
             lambda x: x.loc[x[act_column].idxmin()]).copy().reset_index(drop=True)
 
         duplis_kept.reset_index(drop=True, inplace=True)
         results.append(duplis_kept)
 
-    # Recombine data
+    # Recombine examples
     recombined_data = pd.concat([no_duplicates, *results], axis=0, ignore_index=True)
     logger.info(f'Duplicates removal reduced the number of rows from {len(data)} to {len(recombined_data)}')
     recombined_data.reset_index(drop=True, inplace=True)
 
     return recombined_data
 
 
 class MolCleaner:
     """
     Use one of the factory methods (´from_df´, ´from_csv´ or ´from_list´) instead of using directly.
 
     1. Standardize unknown stereochemistry (Handled by the RDKit Mol file parser)
         i) Fix wiggly bonds on sp3 carbons - sets atoms and bonds marked as unknown stereo to no stereo
         ii) Fix wiggly bonds on double bonds – set double bond to crossed bond
-    2. Clears S Group data from the mol file
+    2. Clears S Group examples from the mol file
     3. Kekulize the structure
     4. Remove H atoms (See the page on explicit Hs for more details)
     5. Normalization:
         Fix hypervalent nitro groups
         Fix KO to K+ O- and NaO to Na+ O- (Also add Li+ to this)
         Correct amides with N=COH
         Standardise sulphoxides to charge separated form
```

### Comparing `cheminftools-0.1.3/cheminftools/utils.py` & `cheminftools-0.1.4/cheminftools/utils.py`

 * *Files identical despite different names*

### Comparing `cheminftools-0.1.3/cheminftools.egg-info/PKG-INFO` & `cheminftools-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cheminftools
-Version: 0.1.3
+Version: 0.1.4
 Summary: A collection of tools for daily cheminformatics tasks.
 Home-page: https://github.com/marcossantanaioc/cheminftools
 Author: marcossantanaioc
 Author-email: marcosvssantana@gmail.com
 License: Apache Software License 2.0
 Keywords: cheminformatics computational chemistry rdkit
 Classifier: Development Status :: 4 - Beta
@@ -181,7 +181,37 @@
 array([[0, 0, 0, 0, 0],
        [0, 0, 0, 0, 0],
        [0, 0, 0, 0, 0],
        [0, 0, 0, 0, 0],
        [0, 0, 0, 0, 0]], dtype=uint8)
 
 ```
+# Collecting data from ChEMBL
+The current version of cheminftools support queries to ChEMBL based on UNIPROT accession codes.
+It should be straightforward to get activity data for multiple targets using the `ChemblFetcher` class.
+Users can find the latest version (and also older ones) of ChEMBL on the official [page](https://ftp.ebi.ac.uk/pub/databases/chembl/ChEMBLdb/latest/).
+Installation instructions come together with each ChEMBL release.
+
+`ChbemlFetcher` expects a configuration file for the database. This file includes information such as
+the host, user, password and port to connect to the database. 
+An example is shown below:
+
+```markdown
+[postgresql]
+host = localhost
+database = customer
+user = postgres
+password = admindb
+port = 5432
+```
+
+```python
+from cheminftools.data.data_gather import ChemblFetcher
+
+target_uniprot = ['P00742', 'P50613']
+chembl = ChemblFetcher(database_config_filename='database.ini',  # Path to configuration file. You can find \an example in the cheminftools.examples folder
+                       database_name='chembl',  # Name of database
+                       version='32')  # ChEMBL version to use
+df = chembl.query_target_uniprot(target_uniprot=target_uniprot)
+```
+The output is a pandas DataFrame with the desired activity types (e.g. IC50, Kd, Ki)
+for each target in `target_uniprot`.
```

### Comparing `cheminftools-0.1.3/setup.py` & `cheminftools-0.1.4/setup.py`

 * *Files identical despite different names*

