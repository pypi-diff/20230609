# Comparing `tmp/nomic-1.1.6.tar.gz` & `tmp/nomic-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomic-1.1.6.tar", last modified: Thu Apr  6 22:31:32 2023, max compression
+gzip compressed data, was "nomic-1.1.9.tar", last modified: Thu Jun  8 20:02:34 2023, max compression
```

## Comparing `nomic-1.1.6.tar` & `nomic-1.1.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 andriy    (1000) andriy    (1000)        0 2023-04-06 22:31:32.312450 nomic-1.1.6/
--rw-rw-r--   0 andriy    (1000) andriy    (1000)      420 2023-04-06 22:31:32.312450 nomic-1.1.6/PKG-INFO
--rw-rw-r--   0 andriy    (1000) andriy    (1000)     1419 2023-02-24 20:22:52.000000 nomic-1.1.6/README.md
-drwxrwxr-x   0 andriy    (1000) andriy    (1000)        0 2023-04-06 22:31:32.308450 nomic-1.1.6/nomic/
--rw-rw-r--   0 andriy    (1000) andriy    (1000)      105 2023-03-16 13:10:11.000000 nomic-1.1.6/nomic/__init__.py
--rw-rw-r--   0 andriy    (1000) andriy    (1000)    10110 2023-03-23 17:25:32.000000 nomic-1.1.6/nomic/atlas.py
--rw-rw-r--   0 andriy    (1000) andriy    (1000)     4542 2023-03-23 17:25:32.000000 nomic-1.1.6/nomic/cli.py
--rw-rw-r--   0 andriy    (1000) andriy    (1000)     1982 2023-03-23 17:25:32.000000 nomic-1.1.6/nomic/data_inference.py
--rw-rw-r--   0 andriy    (1000) andriy    (1000)     2028 2022-08-15 15:51:51.000000 nomic-1.1.6/nomic/embedders.py
-drwxrwxr-x   0 andriy    (1000) andriy    (1000)        0 2023-04-06 22:31:32.312450 nomic-1.1.6/nomic/gpt4all/
--rw-rw-r--   0 andriy    (1000) andriy    (1000)       49 2023-04-06 18:14:35.000000 nomic-1.1.6/nomic/gpt4all/__init__.py
--rw-rw-r--   0 andriy    (1000) andriy    (1000)     8102 2023-04-05 15:49:22.000000 nomic-1.1.6/nomic/gpt4all/gpt4all.py
-drwxrwxr-x   0 andriy    (1000) andriy    (1000)        0 2023-04-06 22:31:32.312450 nomic-1.1.6/nomic/pl_callbacks/
--rw-rw-r--   0 andriy    (1000) andriy    (1000)       47 2023-03-16 13:10:11.000000 nomic-1.1.6/nomic/pl_callbacks/__init__.py
--rw-rw-r--   0 andriy    (1000) andriy    (1000)     6875 2023-03-16 20:32:14.000000 nomic-1.1.6/nomic/pl_callbacks/pl_callback.py
--rw-rw-r--   0 andriy    (1000) andriy    (1000)    65960 2023-04-06 18:14:30.000000 nomic-1.1.6/nomic/project.py
--rw-rw-r--   0 andriy    (1000) andriy    (1000)      487 2023-02-08 22:19:27.000000 nomic-1.1.6/nomic/settings.py
-drwxrwxr-x   0 andriy    (1000) andriy    (1000)        0 2023-04-06 22:31:32.312450 nomic-1.1.6/nomic/tests/
--rw-rw-r--   0 andriy    (1000) andriy    (1000)        0 2022-08-31 16:46:06.000000 nomic-1.1.6/nomic/tests/__init__.py
--rw-rw-r--   0 andriy    (1000) andriy    (1000)     9409 2023-03-23 18:12:51.000000 nomic-1.1.6/nomic/tests/test_atlas_client.py
--rw-rw-r--   0 andriy    (1000) andriy    (1000)     1284 2023-02-08 22:19:27.000000 nomic-1.1.6/nomic/utils.py
-drwxrwxr-x   0 andriy    (1000) andriy    (1000)        0 2023-04-06 22:31:32.308450 nomic-1.1.6/nomic.egg-info/
--rw-rw-r--   0 andriy    (1000) andriy    (1000)      420 2023-04-06 22:31:32.000000 nomic-1.1.6/nomic.egg-info/PKG-INFO
--rw-rw-r--   0 andriy    (1000) andriy    (1000)      506 2023-04-06 22:31:32.000000 nomic-1.1.6/nomic.egg-info/SOURCES.txt
--rw-rw-r--   0 andriy    (1000) andriy    (1000)        1 2023-04-06 22:31:32.000000 nomic-1.1.6/nomic.egg-info/dependency_links.txt
--rw-rw-r--   0 andriy    (1000) andriy    (1000)       41 2023-04-06 22:31:32.000000 nomic-1.1.6/nomic.egg-info/entry_points.txt
--rw-rw-r--   0 andriy    (1000) andriy    (1000)      466 2023-04-06 22:31:32.000000 nomic-1.1.6/nomic.egg-info/requires.txt
--rw-rw-r--   0 andriy    (1000) andriy    (1000)        6 2023-04-06 22:31:32.000000 nomic-1.1.6/nomic.egg-info/top_level.txt
--rw-rw-r--   0 andriy    (1000) andriy    (1000)       38 2023-04-06 22:31:32.312450 nomic-1.1.6/setup.cfg
--rw-rw-r--   0 andriy    (1000) andriy    (1000)     1722 2023-04-06 22:31:30.000000 nomic-1.1.6/setup.py
+drwxr-xr-x   0 andriy     (501) staff       (20)        0 2023-06-08 20:02:34.593768 nomic-1.1.9/
+-rw-r--r--   0 andriy     (501) staff       (20)      409 2023-06-08 20:02:34.593371 nomic-1.1.9/PKG-INFO
+-rw-r--r--   0 andriy     (501) staff       (20)     1419 2023-05-18 03:34:02.000000 nomic-1.1.9/README.md
+drwxr-xr-x   0 andriy     (501) staff       (20)        0 2023-06-08 20:02:34.588679 nomic-1.1.9/nomic/
+-rw-r--r--   0 andriy     (501) staff       (20)      105 2023-05-18 03:34:02.000000 nomic-1.1.9/nomic/__init__.py
+-rw-r--r--   0 andriy     (501) staff       (20)    10318 2023-05-18 03:34:02.000000 nomic-1.1.9/nomic/atlas.py
+-rw-r--r--   0 andriy     (501) staff       (20)     4542 2023-05-18 03:34:02.000000 nomic-1.1.9/nomic/cli.py
+-rw-r--r--   0 andriy     (501) staff       (20)     1982 2023-05-18 03:34:02.000000 nomic-1.1.9/nomic/data_inference.py
+-rw-r--r--   0 andriy     (501) staff       (20)     2028 2023-05-18 03:34:02.000000 nomic-1.1.9/nomic/embedders.py
+drwxr-xr-x   0 andriy     (501) staff       (20)        0 2023-06-08 20:02:34.591003 nomic-1.1.9/nomic/gpt4all/
+-rw-r--r--   0 andriy     (501) staff       (20)       49 2023-05-18 03:34:02.000000 nomic-1.1.9/nomic/gpt4all/__init__.py
+-rw-r--r--   0 andriy     (501) staff       (20)     8102 2023-05-18 03:34:02.000000 nomic-1.1.9/nomic/gpt4all/gpt4all.py
+drwxr-xr-x   0 andriy     (501) staff       (20)        0 2023-06-08 20:02:34.592814 nomic-1.1.9/nomic/pl_callbacks/
+-rw-r--r--   0 andriy     (501) staff       (20)       47 2023-05-18 03:34:02.000000 nomic-1.1.9/nomic/pl_callbacks/__init__.py
+-rw-r--r--   0 andriy     (501) staff       (20)     6875 2023-05-18 03:34:02.000000 nomic-1.1.9/nomic/pl_callbacks/pl_callback.py
+-rw-r--r--   0 andriy     (501) staff       (20)    72218 2023-06-08 19:59:08.000000 nomic-1.1.9/nomic/project.py
+-rw-r--r--   0 andriy     (501) staff       (20)      521 2023-06-08 19:56:46.000000 nomic-1.1.9/nomic/settings.py
+drwxr-xr-x   0 andriy     (501) staff       (20)        0 2023-06-08 20:02:34.593126 nomic-1.1.9/nomic/tests/
+-rw-r--r--   0 andriy     (501) staff       (20)        0 2023-05-18 03:34:02.000000 nomic-1.1.9/nomic/tests/__init__.py
+-rw-r--r--   0 andriy     (501) staff       (20)    10418 2023-05-18 03:34:02.000000 nomic-1.1.9/nomic/tests/test_atlas_client.py
+-rw-r--r--   0 andriy     (501) staff       (20)     1284 2023-05-18 03:34:02.000000 nomic-1.1.9/nomic/utils.py
+drwxr-xr-x   0 andriy     (501) staff       (20)        0 2023-06-08 20:02:34.590590 nomic-1.1.9/nomic.egg-info/
+-rw-r--r--   0 andriy     (501) staff       (20)      409 2023-06-08 20:02:34.000000 nomic-1.1.9/nomic.egg-info/PKG-INFO
+-rw-r--r--   0 andriy     (501) staff       (20)      506 2023-06-08 20:02:34.000000 nomic-1.1.9/nomic.egg-info/SOURCES.txt
+-rw-r--r--   0 andriy     (501) staff       (20)        1 2023-06-08 20:02:34.000000 nomic-1.1.9/nomic.egg-info/dependency_links.txt
+-rw-r--r--   0 andriy     (501) staff       (20)       41 2023-06-08 20:02:34.000000 nomic-1.1.9/nomic.egg-info/entry_points.txt
+-rw-r--r--   0 andriy     (501) staff       (20)      468 2023-06-08 20:02:34.000000 nomic-1.1.9/nomic.egg-info/requires.txt
+-rw-r--r--   0 andriy     (501) staff       (20)        6 2023-06-08 20:02:34.000000 nomic-1.1.9/nomic.egg-info/top_level.txt
+-rw-r--r--   0 andriy     (501) staff       (20)       38 2023-06-08 20:02:34.593823 nomic-1.1.9/setup.cfg
+-rw-r--r--   0 andriy     (501) staff       (20)     1722 2023-06-08 19:56:46.000000 nomic-1.1.9/setup.py
```

### Comparing `nomic-1.1.6/README.md` & `nomic-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `nomic-1.1.6/nomic/atlas.py` & `nomic-1.1.9/nomic/atlas.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,14 +152,16 @@
     organization_name: str = None,
     reset_project_if_exists: bool = False,
     add_datums_if_exists: bool = False,
     shard_size: None = None,
     projection_n_neighbors: int = DEFAULT_PROJECTION_N_NEIGHBORS,
     projection_epochs: int = DEFAULT_PROJECTION_EPOCHS,
     projection_spread: float = DEFAULT_PROJECTION_SPREAD,
+    duplicate_detection: bool = False,
+    duplicate_threshold: float = DEFAULT_DUPLICATE_THRESHOLD, 
 ) -> AtlasProject:
     '''
     Generates or updates a map of the given text.
 
     Args:
         data: An [N,] element list of dictionaries containing metadata for each embedding.
         indexed_field: The name the data field containing the text your want to map.
@@ -234,14 +236,16 @@
             indexed_field=indexed_field,
             colorable_fields=colorable_fields,
             build_topic_model=build_topic_model,
             projection_n_neighbors=projection_n_neighbors,
             projection_epochs=projection_epochs,
             projection_spread=projection_spread,
             multilingual=multilingual,
+            duplicate_detection=duplicate_detection,
+            duplicate_threshold=duplicate_threshold,
         )
         logger.info(str(projection))
     else:
         # otherwise refresh the maps
         project.rebuild_maps()
 
     project = project._latest_project_state()
```

### Comparing `nomic-1.1.6/nomic/cli.py` & `nomic-1.1.9/nomic/cli.py`

 * *Files identical despite different names*

### Comparing `nomic-1.1.6/nomic/data_inference.py` & `nomic-1.1.9/nomic/data_inference.py`

 * *Files identical despite different names*

### Comparing `nomic-1.1.6/nomic/embedders.py` & `nomic-1.1.9/nomic/embedders.py`

 * *Files identical despite different names*

### Comparing `nomic-1.1.6/nomic/gpt4all/gpt4all.py` & `nomic-1.1.9/nomic/gpt4all/gpt4all.py`

 * *Files identical despite different names*

### Comparing `nomic-1.1.6/nomic/pl_callbacks/pl_callback.py` & `nomic-1.1.9/nomic/pl_callbacks/pl_callback.py`

 * *Files identical despite different names*

### Comparing `nomic-1.1.6/nomic/project.py` & `nomic-1.1.9/nomic/project.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import concurrent.futures
 import io
 import json
 import os
 import pickle
 import time
 import uuid
+from collections import defaultdict
 from datetime import date, datetime
 from pathlib import Path
 from typing import Dict, List, Optional, Tuple, Iterable, Union
 from typing import TYPE_CHECKING
 
 from contextlib import contextmanager
 
@@ -57,14 +58,17 @@
             api_hostname = 'api-atlas.nomic.ai'
             web_hostname = 'atlas.nomic.ai'
         else:
             raise ValueError("Invalid tenant.")
 
         self.atlas_api_path = f"https://{api_hostname}"
         self.web_path = f"https://{web_hostname}"
+        override_api_path = os.environ['ATLAS_API_PATH']
+        if override_api_path:
+            self.atlas_api_path = override_api_path
 
         token = self.credentials['token']
         self.token = token
 
         self.header = {"Authorization": f"Bearer {token}"}
 
         if self.token:
@@ -199,22 +203,28 @@
                 raise ValueError(msg)
         if project.meta['modality'] == 'embedding':
             if "_embeddings" not in data.column_names:
                 msg = "Must include embeddings in embedding project upload."
                 raise ValueError(msg)
 
         if project.id_field == ATLAS_DEFAULT_ID_FIELD and not ATLAS_DEFAULT_ID_FIELD in data.column_names:
-            data = data.append_column(ATLAS_DEFAULT_ID_FIELD, pa.array([str(uuid.uuid4()) for _ in range(len(data))]))
+            # Generate random ids.
+            data = data.append_column(ATLAS_DEFAULT_ID_FIELD, pa.array([base64.b64encode(uuid.uuid4().bytes[:8]).decode('utf-8').rstrip('=') for _ in range(len(data))]))
 
         if project.schema is None:
             project._schema = convert_pyarrow_schema_for_atlas(data.schema)
         # Reformat to match the schema of the project.
         # This includes shuffling the order around if necessary,
         # filling in nulls, etc.
         reformatted = {}
+    
+        if data[project.id_field].null_count > 0:            
+            raise ValueError(f"{project.id_field} must not contain null values, but {data[project.id_field].null_count} found.")
+
+
         for field in project.schema:
             if field.name in data.column_names:                
                 # Allow loss of precision in dates and ints, etc.
                 reformatted[field.name] = data[field.name].cast(field.type, safe=False)
             else:                
                 raise KeyError(f"Field {field.name} present in table schema not found in data. Present fields: {data.column_names}")
             if pa.types.is_string(field.type):
@@ -240,25 +250,22 @@
         # The following two conditions should never occur given the above, but just in case...
         assert project.id_field in data.column_names, f"Upload does not contain your specified id_field"
 
         if not pa.types.is_string(data[project.id_field].type):
             logger.warning(f"id_field is not a string. Converting to string from {data[project.id_field].type}")
             data = data.drop([project.id_field]).append_column(project.id_field, data[project.id_field].cast(pa.string()))
 
-        if data[project.id_field].null_count > 0:            
-            raise ValueError(f"{project.id_field} must not contain null values, but {data[project.id_field].null_count} found.")
         
         for key in data.column_names:
             if key.startswith('_'):
                 if key == '_embeddings':
                     continue
                 raise ValueError('Metadata fields cannot start with _')
-
         if pc.max(pc.utf8_length(data[project.id_field])).as_py() > 36:
-            first_match = data.filter(data[project.id_field].utf8_length() > 36).to_pylist()[0]
+            first_match = data.filter(pc.greater(pc.utf8_length(data[project.id_field]), 36)).to_pylist()[0][project.id_field]
             raise ValueError(
                 f"The id_field {first_match} is greater than 36 characters. Atlas does not support id_fields longer than 36 characters."
             )
         return data
     
     def _get_organization(self, organization_name=None, organization_id=None) -> Tuple[str, str]:
         '''
@@ -364,14 +371,15 @@
         Creates an AtlasProjection.
         """
         self.project = project
         self.id = projection_id
         self.atlas_index_id = atlas_index_id
         self.projection_id = projection_id
         self.name = name
+        self.tile_data = None
 
     @property
     def map_link(self):
         '''
         Retrieves a map link.
         '''
         return f"{self.project.web_path}/map/{self.project.id}/{self.id}"
@@ -448,39 +456,93 @@
         if state != 'Completed':
             return f"""Atlas Projection {self.name}. Status {state}. <a target="_blank" href="{self.map_link}">view online</a>"""
         return f"""
             <h3>Project: {self.name}</h3>
             {self._embed_html()}
             """
     
-    def _download_feather(self, dest: str = "tiles"):
+    def web_tile_data(self, tile_destination=None):
+        """
+        Downloads all web data for the projection to the specified directory and returns it as a memmapped arrow table.
+
+        Args:
+            tile_destination: The directory to download the tiles to. Defaults to "web_tiles".
+        """
+        if tile_destination is None:
+            # Default download directory is ~/.nomic/cache/
+            home_dir = os.path.expanduser("~")
+            tile_destination = os.path.join(home_dir, ".nomic", "cache")
+        self._download_feather(tile_destination, overwrite=True)
+        tbs = []
+        root = feather.read_table(f"{tile_destination}/0/0/0.feather")
+        try:
+            sidecars = set([v for k, v in json.loads(root.schema.metadata[b'sidecars']).items()])
+        except KeyError:
+            sidecars = []
+        for path in Path(tile_destination).glob('**/*.feather'):
+            if len(path.stem.split(".")) > 1:
+                # Sidecars are loaded alonside
+                continue
+            tb = pa.feather.read_table(path)
+            for sidecar_file in sidecars:
+                carfile = pa.feather.read_table(path.parent / f"{path.stem}.{sidecar_file}.feather")
+                for col in carfile.column_names:
+                    tb = tb.append_column(col, carfile[col])
+            tbs.append(tb)
+        self.tile_data = pa.concat_tables(tbs)
+
+        return self.tile_data
+                
+
+    def _download_feather(self, dest: str = None, overwrite: bool = True):
         '''
         Downloads the feather tree.
         Args:
             dest: the destination to download the quadtree.
+            overwrite: if True then overwrite existing feather files.
 
         Returns:
             A list containing all quadtiles downloads
         '''
+        if dest is None:
+            # Default download directory is ~/.nomic/cache/
+            home_dir = os.path.expanduser("~")
+            dest = os.path.join(home_dir, ".nomic", "cache")
+            if not os.path.exists(dest):
+                os.mkdir(dest)
         dest = Path(dest)
         root = f'{self.project.atlas_api_path}/v1/project/public/{self.project.id}/index/projection/{self.id}/quadtree/'
         quads = [f'0/0/0']
         all_quads = []
+        sidecars = None
         while len(quads) > 0:
-            quad = quads.pop(0) + ".feather"
-            all_quads.append(quad)
+            rawquad = quads.pop(0)
+            quad = rawquad + ".feather"
+            all_quads.append(quad)            
             path = dest / quad
-            if not path.exists():
+            if not path.exists() or overwrite:
                 data = requests.get(root + quad)
                 readable = io.BytesIO(data.content)
                 readable.seek(0)
                 tb = feather.read_table(readable)
                 path.parent.mkdir(parents=True, exist_ok=True)
                 feather.write_feather(tb, path)
             schema = ipc.open_file(path).schema
+            if sidecars is None and b'sidecars' in schema.metadata:
+                # Grab just the filenames
+                sidecars = set([v for k, v in json.loads(schema.metadata.get(b'sidecars')).items()])
+            elif sidecars is None:
+                sidecars = set()
+            if not "." in rawquad:
+                for sidecar in sidecars:
+                    # The sidecar loses the feather suffix because it's supposed to be raw.
+                    quads.append(quad.replace(".feather", f'.{sidecar}'))
+            if not schema.metadata or b'children' not in schema.metadata:
+                # Sidecars don't have children.
+                continue
             kids = schema.metadata.get(b'children')
             children = json.loads(kids)
             quads.extend(children)
         return all_quads
 
     def download_embeddings(self, save_directory: str, num_workers: int = 10) -> bool:
         '''
@@ -634,14 +696,82 @@
         if response.status_code != 200:
             raise Exception(response.text)
 
         response = response.json()
 
         return response['neighbors'], response['distances']
 
+    def group_by_topic(self, topic_depth = 1):
+        """
+        Group datums by topic at a set topic depth.
+
+        Args:
+            topic_depth: Topic depth to group datums by. Acceptable values
+            currently are (1, 2, 3). Default is 1.
+        Returns:
+            List of dictionaries where each dictionary contains
+                next depth subtopics, topic_id, topic_short_description, topic_long_description,
+                and list of datum_ids.
+        """
+        if not self.tile_data:
+            self.web_tile_data()
+
+        topic_cols = []
+        # TODO: This will need to be changed once topic depths becomes dynamic and not hard-coded
+        if topic_depth not in (1, 2, 3):
+            raise ValueError("Topic depth out of range.")
+
+        # Unique datum id column to aggregate
+        datum_id_col = self.project.meta["unique_id_field"]
+
+        cols = [datum_id_col, f"_topic_depth_{topic_depth}"]
+
+        df = self.tile_data.select(cols).to_pandas()
+        topic_datum_dict = df.groupby(f"_topic_depth_{topic_depth}")[datum_id_col].apply(set).to_dict()
+
+        topic_data = self.get_topic_data()
+        topic_df, hierarchy = self._get_topic_artifacts(topic_data)
+
+        result = []
+
+        for topic, datum_ids in topic_datum_dict.items():
+            # Encountered topic with zero datums
+            if len(datum_ids) == 0:
+                continue
+            
+            result_dict = {}
+            topic_metadata = topic_df[topic_df["topic_short_description"] == topic]
+
+            result_dict["subtopics"] = hierarchy[topic]
+            result_dict["topic_id"] = topic_metadata["topic_id"]
+            result_dict["topic_short_description"] = topic_metadata["topic_short_description"]
+            result_dict["topic_long_description"] = topic_metadata["topic_description"]
+            result_dict["datum_ids"] = datum_ids
+            result.append(result_dict)
+        return result
+
+    @staticmethod
+    def _get_topic_artifacts(topic_data):
+        topic_df = pd.DataFrame(topic_data)
+        topic_df = topic_df.rename(columns={"topic": "topic_id"})
+
+        topic_hierarchy = defaultdict(list)
+        cols = ["topic_id", "_topic_depth_1", "_topic_depth_2", "_topic_depth_3"]
+
+        for i, row in topic_df[cols].iterrows():
+            # Only consider the non-null values for each row
+            topics = [topic for topic in row if pd.notna(topic)]
+            
+            # Iterate over the topics in each row, adding each topic to the
+            # list of subtopics for the topic at the previous depth
+            for i in range(1, len(topics) - 1):
+                if topics[i + 1] not in topic_hierarchy[topics[i]]:
+                    topic_hierarchy[topics[i]].append(topics[i + 1]) 
+        return topic_df, dict(topic_hierarchy)
+
     def get_topic_data(self) -> List:
         '''
         Retrieves metadata about a maps pre-computed topics
 
         Returns:
             A dictionary of metadata for each topic in the model
 
@@ -872,15 +1002,15 @@
                     f"Found existing project `{name}` in organization `{organization_name}`. Clearing it of data by request."
                 )
                 self._delete_project_by_id(project_id=project_id)
                 project_id = None
             elif not add_datums_if_exists: #prevent adding datums to existing project explicitly
                 raise ValueError(
                     f"Project already exists with the name `{name}` in organization `{organization_name}`. "
-                    f"You can add datums to it by settings `add_datums_if_exists = True` or reset it by specifying `reset_project_if_exist=True` on a new upload."
+                    f"You can add datums to it by settings `add_datums_if_exists = True` or reset it by specifying `reset_project_if_exists=True` on a new upload."
                 )
             else:
                 logger.info(
                     f"Loading existing project `{name}` from organization `{organization_name}`."
                 )
 
         if project_id is None: #if there is no existing project, make a new one.
@@ -1140,14 +1270,16 @@
         multilingual: bool = False,
         build_topic_model: bool = False,
         projection_n_neighbors: int = DEFAULT_PROJECTION_N_NEIGHBORS,
         projection_epochs: int = DEFAULT_PROJECTION_EPOCHS,
         projection_spread: float = DEFAULT_PROJECTION_SPREAD,
         topic_label_field: str = None,
         reuse_embeddings_from_index: str = None,
+        duplicate_detection: bool = False,
+        duplicate_threshold: float = DEFAULT_DUPLICATE_THRESHOLD,
     ) -> AtlasProjection:
         '''
         Creates an index in the specified project.
 
         Args:
             name: The name of the index and the map.
             indexed_field: For text projects, name the data field corresponding to the text to be mapped.
@@ -1155,14 +1287,16 @@
             multilingual: Should the map take language into account? If true, points from different languages but semantically similar text are close together.
             build_topic_model: Should a topic model be built?
             projection_n_neighbors: A projection hyperparameter
             projection_epochs: A projection hyperparameter
             projection_spread: A projection hyperparameter
             topic_label_field: A text field in your metadata to estimate topic labels from. Defaults to the indexed_field for text projects if not specified.
             reuse_embeddings_from_index: the name of the index to reuse embeddings from.
+            duplicate_detection: A boolean whether to run duplicate detection 
+            duplicate_threshold: At which threshold to consider points to be duplicates
 
         Returns:
             The projection this index has built.
 
         '''
 
         self._latest_project_state()
@@ -1173,14 +1307,17 @@
                 projection_epochs == DEFAULT_PROJECTION_EPOCHS
                 and projection_n_neighbors == DEFAULT_PROJECTION_N_NEIGHBORS
             ):
                 projection_n_neighbors = DEFAULT_LARGE_PROJECTION_N_NEIGHBORS
                 projection_epochs = DEFAULT_LARGE_PROJECTION_EPOCHS
 
         if self.modality == 'embedding':
+            if duplicate_detection:
+                raise ValueError("Cannot tag duplicates in an embedding project.")
+
             build_template = {
                 'project_id': self.id,
                 'index_name': name,
                 'indexed_field': None,
                 'atomizer_strategies': None,
                 'model': None,
                 'colorable_fields': colorable_fields,
@@ -1240,14 +1377,17 @@
                 'projection': 'NomicProject',
                 'projection_hyperparameters': json.dumps(
                     {'n_neighbors': projection_n_neighbors, 'n_epochs': projection_epochs, 'spread': projection_spread}
                 ),
                 'topic_model_hyperparameters': json.dumps(
                     {'build_topic_model': build_topic_model, 'community_description_target_field': indexed_field}
                 ),
+                'duplicate_detection_hyperparameters': json.dumps(
+                    {'tag_duplicates': duplicate_detection, 'duplicate_cutoff': duplicate_threshold}
+                )
             }
 
         response = requests.post(
             self.atlas_api_path + "/v1/project/index/create",
             headers=self.header,
             json=build_template,
         )
```

### Comparing `nomic-1.1.6/nomic/tests/test_atlas_client.py` & `nomic-1.1.9/nomic/tests/test_atlas_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 def gen_random_datetime(min_year=1900, max_year=datetime.now().year):
     # generate a datetime in format yyyy-mm-dd hh:mm:ss.000000
     start = datetime(min_year, 1, 1, 00, 00, 00)
     years = max_year - min_year + 1
     end = start + timedelta(days=365 * years)
     return start + (end - start) * random.random()
 
-
 def test_map_idless_embeddings():
     num_embeddings = 50
     embeddings = np.random.rand(num_embeddings, 512)
 
-    response = atlas.map_embeddings(embeddings=embeddings)
-    print(response)
+    response = atlas.map_embeddings(name="test1", embeddings=embeddings, reset_project_if_exists = True)
+
+    AtlasProject(name="test1").delete()
 
 
 def test_map_embeddings_with_errors():
     num_embeddings = 20
     embeddings = np.random.rand(num_embeddings, 10)
 
     # test nested dictionaries
@@ -100,15 +100,15 @@
 
     project.delete()
 
 
 def test_date_metadata():
     num_embeddings = 20
     embeddings = np.random.rand(num_embeddings, 10)
-    data = [{'my_date': datetime.datetime(2022, 1, i),
+    data = [{'my_date': datetime(2022, 1, i),
              'my_random_date': gen_random_datetime()} for i in range(1, len(embeddings) + 1)]
 
     project = atlas.map_embeddings(
         embeddings=embeddings, name='test_date_metadata', data=data, is_public=True, reset_project_if_exists=True
     )
 
     assert project.id
@@ -135,15 +135,15 @@
             data=[{'key': 'a'}],
             indexed_field='text',
             is_public=True,
             name='test_map_text_errors',
             description='test map description',
             reset_project_if_exists=True,
         )
-
+    AtlasProject(name='test_map_text_errors').delete()
 
 def test_map_embedding_progressive():
     num_embeddings = 100
     embeddings = np.random.rand(num_embeddings, 10)
     data = [{'field': str(uuid.uuid4()), 'id': str(uuid.uuid4()), 'upload': 0.0} for i in range(len(embeddings))]
 
     project = atlas.map_embeddings(
@@ -261,14 +261,45 @@
                        build_topic_model=True
                        )
         assert p.total_datums == 200
 
     with p.wait_for_project_lock():
         p.delete()
 
+def test_flawed_ids():
+    """
+    Check that null and empty strings do not block an index build.
+    """
+    p = AtlasProject(
+        name='test_flawed_ids',
+        modality='text',
+        unique_id_field='id',
+        reset_project_if_exists=True
+    )
+
+    elements = []
+    for i in range(10):
+        if i % 3 == 0 and i % 5 == 0:
+            elements.append({'text': 'fizzbuzz', 'id': str(i)})
+        elif i % 3 == 0:
+            elements.append({'text': 'fizz', 'id': str(i)})
+        elif i % 5 == 0:
+            elements.append({'text': 'buzz', 'id': str(i)})
+    p.add_text(data=elements)
+    with pytest.raises(ValueError):
+        p.add_text(data=[{
+            'text': 'fizzbuzz',
+            'id': None
+        }])
+    with pytest.raises(ValueError):
+        p.add_text(data=[{
+            'text': 'fizzbuzz',
+            'id': 'A' * 100
+        }])
+    p.delete()
 
 def test_weird_inputs():
     """
     Check that null and empty strings do not block an index build.
     """
     p = AtlasProject(
         name='test_weird_inputs',
@@ -294,8 +325,9 @@
     p.add_text(data=elements)
     p.create_index(
         name='test_weird_inputs',
         indexed_field='text',
         build_topic_model=True
     )
     with p.wait_for_project_lock():
-        assert True
+        assert True
+    p.delete()
```

### Comparing `nomic-1.1.6/nomic/utils.py` & `nomic-1.1.9/nomic/utils.py`

 * *Files identical despite different names*

### Comparing `nomic-1.1.6/setup.py` & `nomic-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
             'sentencepiece',
             f"transformers @ file://localhost/{os.getcwd()}/bin/transformers-4.28.0.dev0-py3-none-any.whl",
             f"peft @ file://localhost/{os.getcwd()}/bin/peft-0.3.0.dev0-py3-none-any.whl"
         ]
     
 setup(
     name='nomic',
-    version='1.1.6',
+    version='1.1.9',
     url='https://github.com/nomic-ai/nomic',
     description=description,
     long_description=description,
     packages=find_packages(),
     author_email="support@nomic.ai",
     author="nomic.ai",
     classifiers=[
```

