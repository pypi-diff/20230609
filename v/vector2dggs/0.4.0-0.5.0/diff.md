# Comparing `tmp/vector2dggs-0.4.0.tar.gz` & `tmp/vector2dggs-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector2dggs-0.4.0.tar", max compression
+gzip compressed data, was "vector2dggs-0.5.0.tar", max compression
```

## Comparing `vector2dggs-0.4.0.tar` & `vector2dggs-0.5.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     8208 2023-06-04 03:24:25.334318 vector2dggs-0.4.0/README.md
--rw-r--r--   0        0        0     1092 2023-06-04 03:24:09.972154 vector2dggs-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       27 2023-06-04 03:24:32.375320 vector2dggs-0.4.0/vector2dggs/__init__.py
--rw-r--r--   0        0        0      599 2023-05-29 05:44:55.043652 vector2dggs-0.4.0/vector2dggs/cli.py
--rw-r--r--   0        0        0    12344 2023-06-04 03:20:22.172432 vector2dggs-0.4.0/vector2dggs/h3.py
--rw-r--r--   0        0        0     3173 2023-05-29 05:44:55.043652 vector2dggs-0.4.0/vector2dggs/katana.py
--rw-r--r--   0        0        0     9642 1970-01-01 00:00:00.000000 vector2dggs-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     8360 2023-06-09 00:47:52.784100 vector2dggs-0.5.0/README.md
+-rw-r--r--   0        0        0     1092 2023-06-09 00:47:52.792101 vector2dggs-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-06-09 00:47:52.792101 vector2dggs-0.5.0/vector2dggs/__init__.py
+-rw-r--r--   0        0        0      599 2023-05-29 05:44:55.043652 vector2dggs-0.5.0/vector2dggs/cli.py
+-rw-r--r--   0        0        0    12629 2023-06-09 00:47:52.792101 vector2dggs-0.5.0/vector2dggs/h3.py
+-rw-r--r--   0        0        0     3173 2023-05-29 05:44:55.043652 vector2dggs-0.5.0/vector2dggs/katana.py
+-rw-r--r--   0        0        0     9794 1970-01-01 00:00:00.000000 vector2dggs-0.5.0/PKG-INFO
```

### Comparing `vector2dggs-0.4.0/README.md` & `vector2dggs-0.5.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -41,20 +41,18 @@
   -id, --id_field TEXT            Field to use as an ID; defaults to a
                                   constructed single 0...n index on the
                                   original feature order.
   -k, --keep_attributes           Retain attributes in output. The default is
                                   to create an output that only includes H3
                                   cell ID and the ID given by the -id field
                                   (or the default index ID).
-  -p, --partitions INTEGER        The number of partitions to create.
-                                  Recommendation: at least as many partitions
-                                  as there are available `--threads`.
-                                  Partitions are processed in parallel once
-                                  they have been formed.  [default: 50;
-                                  required]
+  -ch, --chunksize INTEGER        The number of rows per index partition to
+                                  use when spatially partioning. Adjusting
+                                  this number will trade off memory use and
+                                  time.  [default: 50; required]
   -s, --spatial_sorting [hilbert|morton|geohash]
                                   Spatial sorting method when perfoming
                                   spatial partitioning.  [default: hilbert]
   -crs, --cut_crs INTEGER         Set the coordinate reference system (CRS)
                                   used for cutting large polygons (see `--cur-
                                   threshold`). Defaults to the same CRS as the
                                   input. Should be a valid EPSG code.
@@ -67,14 +65,18 @@
   -t, --threads INTEGER           Amount of threads used for operation
                                   [default: 7]
   -tbl, --table TEXT              Name of the table to read when using a
                                   spatial database connection as input
   -g, --geom_col TEXT             Column name to use when using a spatial
                                   database connection as input  [default:
                                   geom]
+  --tempdir PATH                  Temporary data is created during the
+                                  execution of this program. This parameter
+                                  allows you to control where this data will
+                                  be written.
   -o, --overwrite
   --version                       Show the version and exit.
   --help                          Show this message and exit.
 ```
 
 ### Example 
 
@@ -151,17 +153,17 @@
 ## Citation
 
 ```bibtex
 @software{vector2dggs,
   title={{vector2dggs}},
   author={Ardo, James and Law, Richard},
   url={https://github.com/manaakiwhenua/vector2dggs},
-  version={0.4.0},
+  version={0.5.0},
   date={2023-04-20}
 }
 ```
 
 APA/Harvard
 
-> Ardo, J., & Law, R. (2023). vector2dggs (0.4.0) [Computer software]. https://github.com/manaakiwhenua/vector2dggs
+> Ardo, J., & Law, R. (2023). vector2dggs (0.5.0) [Computer software]. https://github.com/manaakiwhenua/vector2dggs
 
 [![manaakiwhenua-standards](https://github.com/manaakiwhenua/vector2dggs/workflows/manaakiwhenua-standards/badge.svg)](https://github.com/manaakiwhenua/manaakiwhenua-standards)
```

### Comparing `vector2dggs-0.4.0/pyproject.toml` & `vector2dggs-0.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vector2dggs"
-version = "0.4.0"
+version = "0.5.0"
 description = "CLI DGGS indexer for vector geospatial data"
 authors = ["James Ardo <ardoj@landcareresearch.co.nz>"]
 maintainers = ["Richard Law <lawr@landcareresearch.co.nz>"]
 readme = "README.md"
 license = "LGPL-3.0-or-later"
 repository = "https://github.com/manaakiwhenua/vector2dggs"
 keywords = ["dggs", "vector", "h3", "cli"]
```

### Comparing `vector2dggs-0.4.0/vector2dggs/cli.py` & `vector2dggs-0.5.0/vector2dggs/cli.py`

 * *Files identical despite different names*

### Comparing `vector2dggs-0.4.0/vector2dggs/h3.py` & `vector2dggs-0.5.0/vector2dggs/h3.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 warnings.filterwarnings(
     "ignore"
 )  # This is to filter out the polyfill warnings when rows failed to get indexed at a resolution, can be commented out to find missing rows
 
 
 DEFAULT_PARENT_OFFSET = 6
-
+DEFAULT_CHUNK_SIZE = 50
 
 class ParentResolutionException(Exception):
     pass
 
 
 def _get_parent_res(parent_res: Union[None, int], resolution: int):
     """
@@ -71,24 +71,30 @@
     Reads a geoparquet, performs H3 polyfilling,
     and writes out to parquet.
     """
     df = (
         gpd.read_parquet(pq_in)
         .reset_index()
         .drop(columns=[spatial_sort_col])
-        .h3.polyfill_resample(resolution, return_geometry=False)
     )
+    if len(df.index) == 0:
+        # Input is empty, nothing to polyfill
+        return None
+    df = df.h3.polyfill_resample(resolution, return_geometry=False)
+    if len(df.index) == 0:
+        # Polyfill resulted in empty output (e.g. large cell, small feature)
+        return None
     df = pd.DataFrame(df).drop(columns=["index", "geometry"])
     df.index.rename(f"h3_{resolution:02}", inplace=True)
     parent_res: int = _get_parent_res(parent_res, resolution)
     # Secondary (parent) H3 index, used later for partitioning
     df.h3.h3_to_parent(parent_res).to_parquet(
         PurePath(output_directory, pq_in.name),
         engine="auto",
-        compression="ZSTD",
+        compression="ZSTD"
     )
     return None
 
 
 def polyfill_star(args) -> None:
     return polyfill(*args)
 
@@ -125,15 +131,15 @@
 
 def _index(
     input_file: Union[Path, str],
     output_directory: Union[Path, str],
     resolution: int,
     parent_res: Union[None, int],
     keep_attributes: bool,
-    npartitions: int,
+    chunksize: int,
     spatial_sorting: str,
     cut_threshold: int,
     processes: int,
     id_field: str = None,
     cut_crs: pyproj.CRS = None,
     con: Union[sqlalchemy.engine.Connection, sqlalchemy.engine.Engine] = None,
     table: str = None,
@@ -177,23 +183,24 @@
     with tqdm(total=df.shape[0]) as pbar:
         for index, row in df.iterrows():
             df.loc[index, "geometry"] = GeometryCollection(
                 katana.katana(row.geometry, cut_threshold)
             )
             pbar.update(1)
 
-    LOGGER.info("Preparing for spatial partitioning....")
+    LOGGER.info("Preparing for spatial partitioning...")
     df = (
         df.to_crs(4326)
         .explode(index_parts=False)  # Explode from GeometryCollection
         .explode(index_parts=False)  # Explode multipolygons to polygons
+        .drop(df[(df.geometry.is_empty|df.geometry.isna())].index)
         .reset_index()
     )
 
-    ddf = dgpd.from_geopandas(df, npartitions=npartitions)
+    ddf = dgpd.from_geopandas(df, chunksize=max(1, chunksize), sort=True)
 
     LOGGER.info("Spatially sorting and partitioning (%s)", spatial_sorting)
     ddf = ddf.spatial_shuffle(by=spatial_sorting)
     spatial_sort_col = (
         spatial_sorting
         if spatial_sorting == "geohash"
         else f"{spatial_sorting}_distance"
@@ -258,20 +265,20 @@
     "--keep_attributes",
     is_flag=True,
     show_default=True,
     default=False,
     help="Retain attributes in output. The default is to create an output that only includes H3 cell ID and the ID given by the -id field (or the default index ID).",
 )
 @click.option(
-    "-p",
-    "--partitions",
+    "-ch",
+    "--chunksize",
     required=True,
     type=int,
-    default=50,
-    help="The number of partitions to create. Recommendation: at least as many partitions as there are available `--threads`. Partitions are processed in parallel once they have been formed.",
+    default=DEFAULT_CHUNK_SIZE,
+    help="The number of rows per index partition to use when spatially partioning. Adjusting this number will trade off memory use and time.",
     nargs=1,
 )
 @click.option(
     "-s",
     "--spatial_sorting",
     type=click.Choice(["hilbert", "morton", "geohash"]),
     default="hilbert",
@@ -333,15 +340,15 @@
 def h3(
     vector_input: Union[str, Path],
     output_directory: Union[str, Path],
     resolution: str,
     parent_res: str,
     id_field: str,
     keep_attributes: bool,
-    partitions: int,
+    chunksize: int,
     spatial_sorting: str,
     cut_crs: int,
     cut_threshold: int,
     threads: int,
     table: str,
     geom_col: str,
     tempdir: Union[str, Path],
@@ -394,15 +401,15 @@
     try:
         _index(
             vector_input,
             output_directory,
             int(resolution),
             parent_res,
             keep_attributes,
-            partitions,
+            chunksize,
             spatial_sorting,
             cut_threshold,
             threads,
             cut_crs=cut_crs,
             id_field=id_field,
             con=con,
             table=table,
```

### Comparing `vector2dggs-0.4.0/vector2dggs/katana.py` & `vector2dggs-0.5.0/vector2dggs/katana.py`

 * *Files identical despite different names*

### Comparing `vector2dggs-0.4.0/PKG-INFO` & `vector2dggs-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector2dggs
-Version: 0.4.0
+Version: 0.5.0
 Summary: CLI DGGS indexer for vector geospatial data
 Home-page: https://github.com/manaakiwhenua/vector2dggs
 License: LGPL-3.0-or-later
 Keywords: dggs,vector,h3,cli
 Author: James Ardo
 Author-email: ardoj@landcareresearch.co.nz
 Maintainer: Richard Law
@@ -76,20 +76,18 @@
   -id, --id_field TEXT            Field to use as an ID; defaults to a
                                   constructed single 0...n index on the
                                   original feature order.
   -k, --keep_attributes           Retain attributes in output. The default is
                                   to create an output that only includes H3
                                   cell ID and the ID given by the -id field
                                   (or the default index ID).
-  -p, --partitions INTEGER        The number of partitions to create.
-                                  Recommendation: at least as many partitions
-                                  as there are available `--threads`.
-                                  Partitions are processed in parallel once
-                                  they have been formed.  [default: 50;
-                                  required]
+  -ch, --chunksize INTEGER        The number of rows per index partition to
+                                  use when spatially partioning. Adjusting
+                                  this number will trade off memory use and
+                                  time.  [default: 50; required]
   -s, --spatial_sorting [hilbert|morton|geohash]
                                   Spatial sorting method when perfoming
                                   spatial partitioning.  [default: hilbert]
   -crs, --cut_crs INTEGER         Set the coordinate reference system (CRS)
                                   used for cutting large polygons (see `--cur-
                                   threshold`). Defaults to the same CRS as the
                                   input. Should be a valid EPSG code.
@@ -102,14 +100,18 @@
   -t, --threads INTEGER           Amount of threads used for operation
                                   [default: 7]
   -tbl, --table TEXT              Name of the table to read when using a
                                   spatial database connection as input
   -g, --geom_col TEXT             Column name to use when using a spatial
                                   database connection as input  [default:
                                   geom]
+  --tempdir PATH                  Temporary data is created during the
+                                  execution of this program. This parameter
+                                  allows you to control where this data will
+                                  be written.
   -o, --overwrite
   --version                       Show the version and exit.
   --help                          Show this message and exit.
 ```
 
 ### Example 
 
@@ -186,18 +188,18 @@
 ## Citation
 
 ```bibtex
 @software{vector2dggs,
   title={{vector2dggs}},
   author={Ardo, James and Law, Richard},
   url={https://github.com/manaakiwhenua/vector2dggs},
-  version={0.4.0},
+  version={0.5.0},
   date={2023-04-20}
 }
 ```
 
 APA/Harvard
 
-> Ardo, J., & Law, R. (2023). vector2dggs (0.4.0) [Computer software]. https://github.com/manaakiwhenua/vector2dggs
+> Ardo, J., & Law, R. (2023). vector2dggs (0.5.0) [Computer software]. https://github.com/manaakiwhenua/vector2dggs
 
 [![manaakiwhenua-standards](https://github.com/manaakiwhenua/vector2dggs/workflows/manaakiwhenua-standards/badge.svg)](https://github.com/manaakiwhenua/manaakiwhenua-standards)
```

