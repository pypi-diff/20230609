# Comparing `tmp/tagreader-4.0.1.tar.gz` & `tmp/tagreader-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tagreader-4.0.1.tar", max compression
+gzip compressed data, was "tagreader-4.0.3.tar", max compression
```

## Comparing `tagreader-4.0.1.tar` & `tagreader-4.0.3.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0     1064 2023-05-10 10:09:58.051900 tagreader-4.0.1/LICENSE
--rw-r--r--   0        0        0     2767 2023-06-04 08:39:01.932022 tagreader-4.0.1/README.md
--rw-r--r--   0        0        0     1408 2023-06-05 11:45:51.193262 tagreader-4.0.1/pyproject.toml
--rw-r--r--   0        0        0      587 2023-06-04 08:39:01.936509 tagreader-4.0.1/tagreader/__init__.py
--rw-r--r--   0        0        0    16016 2023-06-04 08:39:01.937333 tagreader-4.0.1/tagreader/cache.py
--rw-r--r--   0        0        0    18678 2023-06-04 08:39:01.937705 tagreader-4.0.1/tagreader/clients.py
--rw-r--r--   0        0        0    23714 2023-06-04 08:39:01.938228 tagreader-4.0.1/tagreader/odbc_handlers.py
--rw-r--r--   0        0        0     7574 2023-06-04 08:39:01.938561 tagreader-4.0.1/tagreader/utils.py
--rw-r--r--   0        0        0    31605 2023-06-04 08:39:01.938889 tagreader-4.0.1/tagreader/web_handlers.py
--rw-r--r--   0        0        0     4391 1970-01-01 00:00:00.000000 tagreader-4.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-06 13:10:02.326221 tagreader-4.0.3/LICENSE
+-rw-r--r--   0        0        0     2982 2023-06-09 06:31:44.774759 tagreader-4.0.3/README.md
+-rw-r--r--   0        0        0     1565 2023-06-09 06:49:48.996497 tagreader-4.0.3/pyproject.toml
+-rw-r--r--   0        0        0      329 2023-06-09 06:24:33.101565 tagreader-4.0.3/tagreader/__init__.py
+-rw-r--r--   0        0        0      282 2023-06-09 06:24:33.101915 tagreader-4.0.3/tagreader/__version__.py
+-rw-r--r--   0        0        0    17751 2023-06-09 06:24:33.103078 tagreader-4.0.3/tagreader/cache.py
+-rw-r--r--   0        0        0    21162 2023-06-09 06:24:33.103962 tagreader-4.0.3/tagreader/clients.py
+-rw-r--r--   0        0        0      198 2023-06-09 06:24:33.104271 tagreader-4.0.3/tagreader/logger.py
+-rw-r--r--   0        0        0    25064 2023-06-09 06:24:33.105099 tagreader-4.0.3/tagreader/odbc_handlers.py
+-rw-r--r--   0        0        0     7755 2023-06-09 06:24:33.105868 tagreader-4.0.3/tagreader/utils.py
+-rw-r--r--   0        0        0    33019 2023-06-09 06:24:33.106754 tagreader-4.0.3/tagreader/web_handlers.py
+-rw-r--r--   0        0        0     4720 1970-01-01 00:00:00.000000 tagreader-4.0.3/PKG-INFO
```

### Comparing `tagreader-4.0.1/LICENSE` & `tagreader-4.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tagreader-4.0.1/README.md` & `tagreader-4.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -58,17 +58,26 @@
 ```
 import tagreader
 c = tagreader.IMSClient("mysource", "aspenone")
 print(c.search("tag*"))
 df = c.read_tags(["tag1", "tag2"], "18.06.2020 08:00:00", "18.06.2020 09:00:00", 60)
 ```
 
+## Jupyter Notebook Quickstart
+Jupyter Notebook examples can be found in /examples. In order to run these examples, you need to install the optional
+dependencies.
+
+```bash
+pip install tagreader[notebooks]
+```
+
+
 ## Documentation
 
-There is a [quickstart](docs/quickstart.ipynb) example file that should get
+There is a [quickstart](examples/quickstart.ipynb) example file that should get
 you going. Also check out the [manual](docs/manual.md) for more information.
 
 ## Contributing
 
 All contributions are welcome, including code, bug reports, issues, feature
 requests, and documentation. The preferred way of submitting a contribution
 is to either create an issue on GitHub or to fork the project and make a pull
```

### Comparing `tagreader-4.0.1/pyproject.toml` & `tagreader-4.0.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tagreader"
-version = "4.0.1"
+version = "4.0.3"
 description = "Tagreader is a Python package for reading trend data from the OSIsoft PI and Aspen Infoplus.21 IMS systems."
 authors = ["Einar S. Idsø <eiids@equinor.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "tagreader"}]
 keywords=["Aspen InfoPlus.21", "OSIsoft PI"]
 classifiers=[
@@ -23,23 +23,27 @@
     "Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Utilities",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pandas = "^2.0.1"
-pyodbc = "^4.0.39"
-certifi = "^2023.5.7"
-requests = "^2.31.0"
-requests-kerberos = "^0.14.0"
-tables = "^3.8.0"
+pandas = ">=1"
+pyodbc = "^4"
+certifi = "^2023"
+requests = "^2"
+requests-kerberos = "^0"
+tables = { version = "^3", markers = "platform_machine != 'arm64'" }
+jupyter = { version = "^1", optional = true }
+matplotlib = { version = "^3", optional = true }
 
 
 [tool.poetry.group.dev.dependencies]
-pre-commit = "^3.3.2"
-jupyter = "^1.0.0"
-pytest = "^7.3.1"
+pre-commit = "^3"
+pytest = "^7"
+
+[tool.poetry.extras]
+notebooks = ["jupyter", "matplotlib"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `tagreader-4.0.1/tagreader/cache.py` & `tagreader-4.0.3/tagreader/cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import os
 import warnings
 from importlib.util import find_spec
-from typing import Dict, List, Tuple, Union
+from typing import Dict, List, Literal, Optional, Tuple, Union, cast
 
 import pandas as pd
 
-from .utils import ReaderType
+from tagreader.utils import ReaderType
 
 
 def safe_tagname(tagname: str) -> str:
     tagname = tagname.replace(".", "_")
     tagname = "".join(c for c in tagname if c.isalnum() or c == "_").strip()
     if tagname[0].isnumeric():
         tagname = "_" + tagname  # Conform to NaturalName
     return tagname
 
 
 def timestamp_to_epoch(timestamp: pd.Timestamp) -> int:
     origin = pd.Timestamp("1970-01-01")
     if timestamp.tzinfo is not None:
         timestamp = timestamp.tz_convert("UTC").tz_localize(None)
-    return (timestamp - origin) // pd.Timedelta("1s")  # type: ignore
+    return (timestamp - origin) // pd.Timedelta("1s")
 
 
 class BucketCache:
     def __init__(self, filename: str, path: str = ".") -> None:
         if not find_spec("tables"):
             warnings.warn("Package 'tables' not installed. Disabling cache.")
             return None
@@ -34,16 +34,16 @@
     def _key_path(
         self,
         tagname: str,
         readtype: ReaderType,
         ts: Union[int, pd.Timedelta],
         stepped: bool,
         status: bool,
-        starttime: pd.Timestamp = None,
-        endtime: pd.Timestamp = None,
+        starttime: Optional[pd.Timestamp] = None,
+        endtime: Optional[pd.Timestamp] = None,
     ) -> str:
         """Return a string on the form
         /tagname/readtype[/sample_time][/stepped][/status]/_starttime_endtime
         tagname: safe tagname
         sample_time: integer value. Empty for RAW.
         stepped: "stepped" if value was read as stepped. Empty if not.
         status: "status" if value contains status. Empty if not.
@@ -56,15 +56,15 @@
             int(ts.total_seconds())
             if readtype != ReaderType.RAW and isinstance(ts, pd.Timedelta)
             else ts
         )
         timespan = ""
         if starttime is not None:
             starttime_epoch = timestamp_to_epoch(starttime)
-            endtime_epoch = timestamp_to_epoch(endtime)
+            endtime_epoch = timestamp_to_epoch(endtime)  # type: ignore[arg-type]
             timespan = f"/_{starttime_epoch}_{endtime_epoch}"
 
         keyval = (
             f"/{tagname}"
             f"/{readtype.name}"
             f"{(ts is not None and readtype != ReaderType.RAW) * f'/s{ts}'}"
             f"{stepped * '/stepped'}"
@@ -78,82 +78,96 @@
     ) -> None:
         tagname = safe_tagname(tagname)
         key = f"/{tagname}"
         with pd.HDFStore(self.filename, mode="a") as f:
             if key not in f:
                 f.put(key, pd.DataFrame())
             origmetadata = {}
-            if "metadata" in f.get_storer(key).attrs:
-                origmetadata = f.get_storer(key).attrs.metadata
-            f.get_storer(key).attrs.metadata = {**origmetadata, **metadata}
+            if "metadata" in f.get_storer(key).attrs:  # type: ignore[operator]
+                origmetadata = f.get_storer(key).attrs.metadata  # type: ignore[operator]
+            f.get_storer(key).attrs.metadata = {**origmetadata, **metadata}  # type: ignore[operator]
 
     def fetch_tag_metadata(
         self, tagname: str, properties: Union[str, List[str]]
     ) -> Dict[str, Union[str, int]]:
-        res = {}  # type: Dict[str, Union[str, int]]
+        res: Dict[str, Union[str, int]] = {}
         if not os.path.isfile(self.filename):
             return res
         tagname = safe_tagname(tagname)
         key = f"/{tagname}"
         if isinstance(properties, str):
             properties = [properties]
         with pd.HDFStore(self.filename, mode="r") as f:
-            if key not in f or "metadata" not in f.get_storer(key).attrs:
+            if key not in f or "metadata" not in f.get_storer(key).attrs:  # type: ignore[operator]
                 return {}
-            metadata = f.get_storer(key).attrs.metadata
+            metadata = f.get_storer(key).attrs.metadata  # type: ignore[operator]
         for p in properties:
             if p in metadata.keys():
                 res[p] = metadata.get(p)
         return res
 
-    def remove(self, filename: str = None) -> None:  # type: ignore[assignment]
+    def remove(self, filename: Optional[str] = None) -> None:
         if not filename:
             filename = self.filename
         if os.path.isfile(filename):
             os.unlink(filename)
 
     def store(
         self,
         df: pd.DataFrame,
         tagname: str,
         readtype: ReaderType,
-        ts: pd.Timestamp,
+        ts: pd.Timedelta,
         stepped: bool,
         status: bool,
         starttime: pd.Timestamp,
         endtime: pd.Timestamp,
     ) -> None:
         if df.empty:
             return
 
         intersecting = self.get_intersecting_datasets(
-            tagname, readtype, ts, stepped, status, starttime, endtime
+            tagname=tagname,
+            readtype=readtype,
+            ts=ts,
+            stepped=stepped,
+            status=status,
+            starttime=starttime,
+            endtime=endtime,
         )
         if len(intersecting) > 0:
             with pd.HDFStore(self.filename, mode="a") as f:
                 for dataset in intersecting:
                     this_start, this_end = self._get_intervals_from_dataset_name(
                         dataset
                     )
                     starttime = min(starttime, this_start)
                     endtime = max(endtime, this_end)
-                    df = pd.concat([df, f.get(dataset)])
+                    df = pd.concat([df, f.get(dataset)])  # type: ignore[list-item]
                     del f[dataset]
             df = df[~df.index.duplicated(keep="first")].sort_index()
-        key = self._key_path(tagname, readtype, ts, stepped, status, starttime, endtime)
+        key = self._key_path(
+            tagname=tagname,
+            readtype=readtype,
+            ts=ts,
+            stepped=stepped,
+            status=status,
+            starttime=starttime,
+            endtime=endtime,
+        )
         with pd.HDFStore(self.filename, mode="a") as f:
             f.put(key, df, format="table")
 
     @staticmethod
     def _get_intervals_from_dataset_name(
         name: str,
     ) -> Tuple[pd.Timestamp, pd.Timestamp]:
         name_with_times = name.split("/")[-1]
         if not name_with_times.count("_") == 2:
-            return (None, None)
+            return (None, None)  # type: ignore[return-value]
         _, starttime_epoch, endtime_epoch = name_with_times.split("_")
         starttime = pd.to_datetime(int(starttime_epoch), unit="s").tz_localize("UTC")
         endtime = pd.to_datetime(int(endtime_epoch), unit="s").tz_localize("UTC")
         return starttime, endtime
 
     def get_intersecting_datasets(
         self,
@@ -166,15 +180,23 @@
         endtime: pd.Timestamp,
     ) -> List[str]:
         if not os.path.isfile(self.filename):
             return []
         intersecting_datasets = []
         with pd.HDFStore(self.filename, mode="r") as f:
             for bucket in f.walk(
-                where=self._key_path(tagname, readtype, ts, stepped, status)
+                where=self._key_path(
+                    tagname=tagname,
+                    readtype=readtype,
+                    starttime=None,
+                    endtime=None,
+                    ts=ts,
+                    stepped=stepped,
+                    status=status,
+                )
             ):
                 for leaf in bucket[2]:
                     dataset = bucket[0] + "/" + leaf
                     starttime_ds, endtime_ds = self._get_intervals_from_dataset_name(
                         dataset
                     )
                     if endtime_ds >= starttime and endtime >= starttime_ds:
@@ -188,15 +210,21 @@
         ts: Union[int, pd.Timedelta],
         stepped: bool,
         status: bool,
         starttime: pd.Timestamp,
         endtime: pd.Timestamp,
     ) -> List[Tuple[pd.Timestamp, pd.Timestamp]]:
         datasets = self.get_intersecting_datasets(
-            tagname, readtype, ts, stepped, status, starttime, endtime
+            tagname=tagname,
+            readtype=readtype,
+            ts=ts,
+            stepped=stepped,
+            status=status,
+            starttime=starttime,
+            endtime=endtime,
         )
         missing_intervals = [(starttime, endtime)]
         for dataset in datasets:
             b = self._get_intervals_from_dataset_name(dataset)
             for _ in range(0, len(missing_intervals)):
                 r = missing_intervals.pop(0)
                 if b[1] < r[0] or b[0] > r[1]:
@@ -228,26 +256,32 @@
         endtime: pd.Timestamp,
     ) -> pd.DataFrame:
         df = pd.DataFrame()
         if not os.path.isfile(self.filename):
             return df
 
         datasets = self.get_intersecting_datasets(
-            tagname, readtype, ts, stepped, status, starttime, endtime
+            tagname=tagname,
+            readtype=readtype,
+            ts=ts,
+            stepped=stepped,
+            status=status,
+            starttime=starttime,
+            endtime=endtime,
         )
 
         with pd.HDFStore(self.filename, mode="r") as f:
             for dataset in datasets:
                 # df = df.append(
                 #     f.select(dataset, where="index >= starttime and index <= endtime")
                 # )
                 df = pd.concat(
                     [
                         df,
-                        f.select(
+                        f.select(  # type: ignore[list-item]
                             dataset, where="index >= starttime and index <= endtime"
                         ),
                     ]
                 )
 
         return df.sort_index()
 
@@ -269,44 +303,44 @@
     # def close(self):
     #     self.hdfstore.close()
 
     @staticmethod
     def key_path(
         df: Union[str, pd.DataFrame],
         readtype: ReaderType,
-        ts: Union[int, pd.Timedelta] = None,
+        ts: Optional[Union[int, pd.Timedelta]] = None,
     ) -> str:
         """Return a string on the form
         XXX/sYY/ZZZ where XXX is the ReadType, YY is the interval between samples
         (in seconds) and ZZZ is a safe tagname.
         """
         name = list(df)[0] if isinstance(df, pd.DataFrame) else df
-        name = safe_tagname(name)
+        name = safe_tagname(name)  # type: ignore[arg-type]
         ts = int(ts.total_seconds()) if isinstance(ts, pd.Timedelta) else ts
         if readtype != ReaderType.RAW:
             if ts is None:
                 # Determine sample time by reading interval between first two
                 # samples of dataframe.
                 if isinstance(df, pd.DataFrame):
-                    interval = int(df[0:2].index.to_series().diff().mean().value / 1e9)
+                    interval = int(df[0:2].index.to_series().diff().mean().value / 1e9)  # type: ignore[attr-defined]
                 else:
                     raise TypeError
             else:
                 interval = int(ts)
             return f"{readtype.name}/s{interval}/{name}"
         else:
             return f"{readtype.name}/{name}"
 
     def store(
         self,
         df: pd.DataFrame,
         readtype: ReaderType,
-        ts: Union[int, pd.Timedelta] = None,
+        ts: Optional[Union[int, pd.Timedelta]] = None,
     ) -> None:
-        key = self.key_path(df, readtype, ts)
+        key = self.key_path(df=df, readtype=readtype, ts=ts)
         if df.empty:
             return  # Weirdness ensues when using empty df in select statement below
         with pd.HDFStore(self.filename, mode="a") as f:
             if key in f:
                 idx = f.select(  # noqa: F841
                     key, where="index in df.index", columns=["index"]
                 ).index
@@ -314,118 +348,126 @@
             else:
                 f.append(key, df)
 
     def fetch(
         self,
         tagname: str,
         readtype: ReaderType,
-        ts: Union[int, pd.Timestamp] = None,
-        start_time: pd.Timestamp = None,
-        stop_time: pd.Timestamp = None,
+        ts: Optional[Union[int, pd.Timestamp]] = None,
+        start_time: Optional[pd.Timestamp] = None,
+        stop_time: Optional[pd.Timestamp] = None,
     ) -> pd.DataFrame:
         df = pd.DataFrame()
         if not os.path.isfile(self.filename):
             return df
-        key = self.key_path(tagname, readtype, ts)
+        key = self.key_path(df=tagname, readtype=readtype, ts=ts)  # type: ignore[arg-type]
         where = []
         if start_time is not None:
             where.append("index >= start_time")
         if stop_time is not None:
             where.append("index <= stop_time")
         wheretxt = " and ".join(where)
         with pd.HDFStore(self.filename, mode="r") as f:
             if key in f:
                 if wheretxt:
-                    df = f.select(key, where=wheretxt)
+                    df = f.select(key, where=wheretxt)  # type: ignore[assignment]
                 else:
-                    df = f.select(key)
+                    df = f.select(key)  # type: ignore[assignment]
         return df.sort_index()
 
     def store_tag_metadata(
         self, tagname: str, metadata: Dict[str, Union[str, int]]
     ) -> None:
         tagname = safe_tagname(tagname)
         key = f"/metadata/{tagname}"
         with pd.HDFStore(self.filename, mode="a") as f:
             if key not in f:
                 f.put(key, pd.DataFrame())
             origmetadata = {}
-            if "metadata" in f.get_storer(key).attrs:
-                origmetadata = f.get_storer(key).attrs.metadata
-            f.get_storer(key).attrs.metadata = {**origmetadata, **metadata}
+            if "metadata" in f.get_storer(key).attrs:  # type: ignore[operator]
+                origmetadata = f.get_storer(key).attrs.metadata  # type: ignore[operator]
+            f.get_storer(key).attrs.metadata = {**origmetadata, **metadata}  # type: ignore[operator]
 
     def fetch_tag_metadata(
         self, tagname: str, properties: Union[str, List[str]]
     ) -> Dict[str, Union[str, int]]:
-        res = {}  # type: Dict[str, Union[str, int]]
+        res: Dict[str, Union[str, int]] = {}
         if not os.path.isfile(self.filename):
             return res
         tagname = safe_tagname(tagname)
         key = f"/metadata/{tagname}"
         if isinstance(properties, str):
             properties = [properties]
         with pd.HDFStore(self.filename, mode="r") as f:
-            if key not in f or "metadata" not in f.get_storer(key).attrs:
+            if key not in f or "metadata" not in f.get_storer(key).attrs:  # type: ignore[operator]
                 return {}
-            metadata = f.get_storer(key).attrs.metadata
+            metadata = f.get_storer(key).attrs.metadata  # type: ignore[operator]
         for p in properties:
             if p in metadata.keys():
                 res[p] = metadata.get(p)
         return res
 
-    def remove(self, filename: str = None) -> None:  # type: ignore[assignment]
+    def remove(self, filename: Optional[str] = None) -> None:
         if not filename:
             filename = self.filename
             # self.close()
         if os.path.isfile(filename):
             os.unlink(filename)
 
-    def _match_tag(self, key, readtype=None, ts=None, tagname=None):  # type: ignore
+    def _match_tag(
+        self,
+        key: str,
+        readtype: Optional[Union[List[ReaderType], ReaderType]] = None,
+        ts: Optional[List[Optional[Union[int, pd.Timestamp]]]] = None,
+        tagname: Optional[Union[List[str], str]] = None,
+    ) -> bool:
         def readtype_to_str(rt):  # type: ignore
             return getattr(
                 rt, "name", rt
             )  # if isinstance(rt, ReaderType) always returns False...?
 
-        def timedelta_to_str(t):  # type: ignore
+        def timedelta_to_str(t):  # type: ignore[no-untyped-def]
             if isinstance(t, pd.Timedelta):
                 return str(int(t.total_seconds()))
             return t
 
-        key = "/" + key.lstrip("/")  # Ensure absolute path
-        readtype = readtype if isinstance(readtype, list) else [readtype]
+        key = "/" + key.lstrip("/")  # Ensure absolute path:
+        readtype = readtype if isinstance(readtype, list) else [readtype]  # type: ignore[list-item]
         ts = ts if isinstance(ts, list) else [ts]
-        tagname = tagname if isinstance(tagname, list) else [tagname]
+        tagname = tagname if isinstance(tagname, list) else [tagname]  # type: ignore[list-item]
         readtype = list(map(readtype_to_str, readtype))
         ts = list(map(timedelta_to_str, ts))
         if tagname[0] is not None:
             tagname = list(map(safe_tagname, tagname))
         # print(f"Readtype: {readtype}, ts: {ts}, tagname: {tagname}")
         elements = key.split("/")[1:]
         if len(elements) == 2:
-            elements.insert(1, None)
+            elements.insert(1, None)  # type: ignore[arg-type]
         else:
-            elements[1] = int(elements[1][1:])  # Discard the initial s
-        if elements[0] not in readtype and readtype[0] is not None:
+            elements[1] = int(  # type: ignore[call-overload]
+                elements[1][1:]
+            )  # Discard the initial s
+        if elements[0] not in readtype and readtype[0] is not None:  # type: ignore[comparison-overlap]
             # print(f"{elements[0]} not in {readtype}")
             return False
         if elements[1] not in ts and ts[0] is not None:
             # print(f"{elements[1]} not in {ts}")
             return False
         if elements[2] not in tagname and tagname[0] is not None:
             # print(f"{elements[2]} not in {tagname}")
             return False
         return True
 
     def delete_key(
         self,
-        tagname: str = None,  # type: ignore[assignment]
-        readtype: ReaderType = None,  # type: ignore[assignment]
-        ts: Union[int, List[int]] = None,  # type: ignore[assignment]
+        tagname: Optional[str] = None,
+        readtype: Optional[ReaderType] = None,
+        ts: Optional[Union[int, pd.Timestamp]] = None,
     ) -> None:
         with pd.HDFStore(self.filename) as f:
             for key in f:
-                if self._match_tag(key, tagname=tagname, readtype=readtype, ts=ts):
-                    f.remove(key)
+                if self._match_tag(key=key, tagname=tagname, readtype=readtype, ts=ts):  # type: ignore[arg-type]
+                    f.remove(key)  # type: ignore[operator]
 
-    def _get_hdfstore(self, mode: str = "r") -> pd.HDFStore:
-        f = pd.HDFStore(self.filename, mode)
+    def _get_hdfstore(self, mode: Literal["a", "w", "r", "r+"] = "r") -> pd.HDFStore:
+        f = pd.HDFStore(self.filename, mode=mode)
         return f
```

### Comparing `tagreader-4.0.1/tagreader/clients.py` & `tagreader-4.0.3/tagreader/clients.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,59 @@
 import os
 import warnings
+from datetime import datetime, timedelta
 from itertools import groupby
 from operator import itemgetter
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 import pandas as pd
 
-from .cache import BucketCache, SmartCache
-from .utils import (
+from tagreader.cache import BucketCache, SmartCache
+from tagreader.logger import logger
+from tagreader.utils import (
     ReaderType,
     ensure_datetime_with_tz,
     find_registry_key,
     find_registry_key_from_name,
     is_windows,
-    logging,
 )
-from .web_handlers import (
+from tagreader.web_handlers import (
     AspenHandlerWeb,
     PIHandlerWeb,
     get_auth_aspen,
     get_auth_pi,
-    get_url_aspen,
-    get_url_pi,
     list_aspenone_sources,
     list_piwebapi_sources,
 )
 
 if is_windows():
     import pyodbc
 
-    from .odbc_handlers import (
+    from tagreader.odbc_handlers import (
         AspenHandlerODBC,
         PIHandlerODBC,
         list_aspen_sources,
         list_pi_sources,
     )
-    from .utils import winreg
-
-logging.basicConfig(
-    format=" %(asctime)s %(levelname)s: %(message)s", level=logging.INFO
-)
+    from tagreader.utils import winreg
 
 
 class DuplicateTagsWarning(UserWarning):
     pass
 
 
 warnings.simplefilter("always", DuplicateTagsWarning)
 
 
-def list_sources(imstype, url=None, auth=None, verifySSL=None):
+def list_sources(
+    imstype: str,
+    url: Optional[str] = None,
+    auth: Optional[Any] = None,
+    verifySSL: bool = True,
+) -> List[str]:
     accepted_values = ["piwebapi", "aspenone"]
     win_accepted_values = ["pi", "aspen", "ip21"]
     if is_windows():
         accepted_values.extend(win_accepted_values)
 
     if imstype is None or imstype.lower() not in accepted_values:
         import platform
@@ -75,15 +76,21 @@
         if auth is None:
             auth = get_auth_aspen()
         if verifySSL is None:
             verifySSL = True
         return list_aspenone_sources(url=url, auth=auth, verifySSL=verifySSL)
 
 
-def get_missing_intervals(df, start_time, stop_time, ts, read_type):
+def get_missing_intervals(
+    df: pd.DataFrame,
+    start_time: pd.Timestamp,
+    stop_time: pd.Timestamp,
+    ts: Optional[Union[int, pd.Timestamp]],
+    read_type: ReaderType,
+):
     if (
         read_type == ReaderType.RAW
     ):  # Fixme: How to check for completeness for RAW data?
         return [[start_time, stop_time]]
     seconds = int(ts.total_seconds())
     tvec = pd.date_range(start=start_time, end=stop_time, freq=f"{seconds}s")
     if len(df) == len(tvec):  # Short-circuit if dataset is complete
@@ -99,29 +106,34 @@
             # Should be unnecessary to fetch overlapping points since get_next_timeslice
             # ensures start <= t <= stop
             # missingintervals.append((pd.Timestamp(tvec[seq[0]]),
             #                          pd.Timestamp(tvec[min(seq[-1]+1, len(tvec)-1)])))
     return missing_intervals
 
 
-def get_next_timeslice(start_time, stop_time, ts, max_steps=None):
+def get_next_timeslice(
+    start_time: pd.Timestamp,
+    stop_time: pd.Timestamp,
+    ts: Optional[Union[int, pd.Timestamp]],
+    max_steps: Optional[int] = None,
+) -> Tuple[datetime, datetime]:
     if max_steps is None:
         calc_stop_time = stop_time
     else:
         calc_stop_time = start_time + ts * max_steps
     calc_stop_time = min(stop_time, calc_stop_time)
     # Ensure we include the last data point.
     # Discrepancies between Aspen and Pi for +ts
     # Discrepancies between IMS and cache for e.g. ts.
     # if calc_stop_time == stop_time:
     #     calc_stop_time += ts / 2
     return start_time, calc_stop_time
 
 
-def get_server_address_aspen(datasource):
+def get_server_address_aspen(datasource: str) -> Optional[Tuple[str, int]]:
     """Data sources are listed under
     HKEY_CURRENT_USER\\Software\\AspenTech\\ADSA\\Caches\\AspenADSA\\username.
     For each data source there are multiple keys with Host entries. We start by
     identifying the correct key to use by locating the UUID for Aspen SQLplus
     services located under Aspen SQLplus service component. Then we find the
     host and port based on the path above and the UUID.
     """
@@ -151,15 +163,15 @@
         host = winreg.QueryValueEx(reg_site_key, "Host")[0]
         port = int(winreg.QueryValueEx(reg_site_key, "Port")[0])
         return host, port
     except FileNotFoundError:
         return None
 
 
-def get_server_address_pi(datasource):
+def get_server_address_pi(datasource: str) -> Optional[Tuple[str, int]]:
     """
     PI data sources are listed under
     HKEY_LOCAL_MACHINE\\Software\\Wow6432Node\\PISystem\\PI-SDK\\x.x\\ServerHandles or
     \\Software\\PISystem\\PI-SDK\\x.x\\ServerHandles.
 
     :param datasource: Name of data source
     :return: host, port
@@ -186,22 +198,22 @@
             port = int(winreg.QueryValueEx(reg_site_key, "port")[0])
             return host, port
     except FileNotFoundError:
         return None
 
 
 def get_handler(
-    imstype,
-    datasource,
-    url=None,
-    host=None,
-    port=None,
-    options={},
-    verifySSL=None,
-    auth=None,
+    imstype: str,
+    datasource: str,
+    url: Optional[str] = None,
+    host: Optional[str] = None,
+    port: Optional[int] = None,
+    options: Dict[str, Union[int, float, str]] = {},
+    verifySSL: Optional[bool] = None,
+    auth: Optional[Any] = None,
 ):
     if imstype is None:
         if datasource in list_aspenone_sources():
             imstype = "aspenone"
         elif datasource in list_piwebapi_sources():
             imstype = "piwebapi"
 
@@ -274,95 +286,120 @@
             auth=auth,
         )
 
 
 class IMSClient:
     def __init__(
         self,
-        datasource,
-        imstype=None,
-        tz="Europe/Oslo",
-        url=None,
-        host=None,
-        port=None,
-        handler_options={},
-        verifySSL=None,
-        auth=None,
+        datasource: str,
+        imstype: Optional[str] = None,
+        tz: str = "Europe/Oslo",
+        url: Optional[str] = None,
+        host: Optional[str] = None,
+        port: Optional[int] = None,
+        handler_options: Dict[str, Union[int, float, str]] = {},  # noqa:
+        verifySSL: bool = True,
+        auth: Optional[Any] = None,
     ):
         self.handler = None
         self.datasource = datasource.lower()  # FIXME
         self.tz = tz
         self.handler = get_handler(
-            imstype,
-            datasource,
+            imstype=imstype,
+            datasource=datasource,
             url=url,
             host=host,
             port=port,
             options=handler_options,
             verifySSL=verifySSL,
             auth=auth,
         )
-        self.cache = SmartCache(datasource)
+        self.cache = SmartCache(filename=datasource)
 
     def connect(self):
         self.handler.connect()
 
-    def search_tag(self, tag=None, desc=None):
+    def search_tag(
+        self, tag: Optional[str] = None, desc: Optional[str] = None
+    ) -> List[Tuple[str, str]]:
         warnings.warn("This function is deprecated. Please call 'search()' instead")
         return self.search(tag=tag, desc=desc)
 
-    def search(self, tag=None, desc=None):
-        return self.handler.search(tag, desc)
-
-    def _get_metadata(self, tag):
-        return self.handler._get_tag_metadata(tag)
+    def search(
+        self, tag: Optional[str] = None, desc: Optional[str] = None
+    ) -> List[Tuple[str, str]]:
+        return self.handler.search(tag=tag, desc=desc)
+
+    def _get_metadata(self, tag: str):
+        return self.handler._get_tag_metadata(
+            tag
+        )  # noqa: Should probably expose this as a public method if needed.
 
     def _read_single_tag(
-        self, tag, start_time, stop_time, ts, read_type, get_status, cache=None
+        self,
+        tag: str,
+        start_time: Optional[pd.Timestamp],
+        stop_time: Optional[pd.Timestamp],
+        ts: Optional[Union[int, pd.Timestamp]],
+        read_type: ReaderType,
+        get_status: bool,
+        cache: Optional[Union[BucketCache, SmartCache]],
     ):
         if read_type == ReaderType.SNAPSHOT:
             metadata = self._get_metadata(tag)
             df = self.handler.read_tag(
-                tag, start_time, stop_time, ts, read_type, metadata, get_status
+                tag=tag,
+                start_time=start_time,
+                stop_time=stop_time,
+                sample_time=ts,
+                read_type=read_type,
+                metadata=metadata,
+                get_status=get_status,
             )
         else:
             stepped = False
             missing_intervals = [(start_time, stop_time)]
             df = pd.DataFrame()
 
             if (
                 isinstance(cache, SmartCache)
                 and read_type != ReaderType.RAW
                 and not get_status
             ):
-                time_slice = get_next_timeslice(start_time, stop_time, ts)
+                time_slice = get_next_timeslice(
+                    start_time=start_time, stop_time=stop_time, ts=ts, max_steps=None
+                )
                 df = cache.fetch(
-                    tag,
+                    tagname=tag,
                     readtype=read_type,
                     ts=ts,
                     start_time=time_slice[0],
                     stop_time=time_slice[1],
                 )
                 missing_intervals = get_missing_intervals(
-                    df, start_time, stop_time, ts, read_type
+                    df=df,
+                    start_time=start_time,
+                    stop_time=stop_time,
+                    ts=ts,
+                    read_type=read_type,
                 )
                 if not missing_intervals:
                     return df.tz_convert(self.tz).sort_index()
             elif isinstance(cache, BucketCache):
                 df = cache.fetch(
-                    tag,
+                    tagname=tag,
                     readtype=read_type,
                     ts=ts,
                     stepped=stepped,
                     status=get_status,
                     starttime=start_time,
                     endtime=stop_time,
                 )
                 missing_intervals = cache.get_missing_intervals(
-                    tag,
+                    tagname=tag,
                     readtype=read_type,
                     ts=ts,
                     stepped=stepped,
                     status=get_status,
                     starttime=start_time,
                     endtime=stop_time,
                 )
@@ -370,27 +407,33 @@
                     return df.tz_convert(self.tz).sort_index()
 
             metadata = self._get_metadata(tag)
             frames = [df]
             for start, stop in missing_intervals:
                 while True:
                     df = self.handler.read_tag(
-                        tag, start, stop, ts, read_type, metadata, get_status
+                        tag=tag,
+                        start_time=start,
+                        stop_time=stop,
+                        sample_time=ts,
+                        read_type=read_type,
+                        metadata=metadata,
+                        get_status=get_status,
                     )
                     if len(df.index) > 0:
                         if (
                             cache is not None
                             and read_type
                             not in [
                                 ReaderType.SNAPSHOT,
                                 ReaderType.RAW,
                             ]
                             and not get_status
                         ):
-                            cache.store(df, read_type, ts)
+                            cache.store(df=df, readtype=read_type, ts=ts)
                     frames.append(df)
                     if len(df) < self.handler._max_rows:
                         break
                     start = df.index[-1]
                 # if read_type != ReaderType.RAW:
                 #     time_slice = [start, start]
                 #     while time_slice[1] < stop:
@@ -412,71 +455,81 @@
             # Aggregate read_types (should) align perfectly and don't
             # (shouldn't) need deduplication.
             df = df[~df.index.duplicated(keep="first")]  # Deduplicate on index
         df = df.tz_convert(self.tz).sort_index()
         df = df.rename(columns={"value": tag})
         return df
 
-    def get_units(self, tags):
+    def get_units(self, tags: Union[str, List[str]]):
         if isinstance(tags, str):
             tags = [tags]
         units = {}
         for tag in tags:
             if self.cache is not None:
-                r = self.cache.fetch_tag_metadata(tag, "unit")
+                r = self.cache.fetch_tag_metadata(tagname=tag, properties="unit")
                 if "unit" in r:
                     units[tag] = r["unit"]
             if tag not in units:
                 unit = self.handler._get_tag_unit(tag)
                 if self.cache is not None and unit is not None:
-                    self.cache.store_tag_metadata(tag, {"unit": unit})
+                    self.cache.store_tag_metadata(tagname=tag, metadata={"unit": unit})
                 units[tag] = unit
         return units
 
-    def get_descriptions(self, tags):
+    def get_descriptions(self, tags: Union[str, List[str]]) -> Dict[str, str]:
         if isinstance(tags, str):
             tags = [tags]
         descriptions = {}
         for tag in tags:
             if self.cache is not None:
-                r = self.cache.fetch_tag_metadata(tag, "description")
+                r = self.cache.fetch_tag_metadata(tagname=tag, properties="description")
                 if "description" in r:
                     descriptions[tag] = r["description"]
             if tag not in descriptions:
                 desc = self.handler._get_tag_description(tag)
                 if self.cache is not None and desc is not None:
-                    self.cache.store_tag_metadata(tag, {"description": desc})
+                    self.cache.store_tag_metadata(
+                        tagname=tag, metadata={"description": desc}
+                    )
                 descriptions[tag] = desc
         return descriptions
 
-    def read_tags(self, tags, start_time, stop_time, ts, read_type=ReaderType.INT):
-        warnings.warn(
+    def read_tags(
+        self,
+        tags: Union[str, List[str]],
+        start_time: Optional[Union[datetime, pd.Timestamp, str]],
+        stop_time: Optional[Union[datetime, pd.Timestamp, str]],
+        ts: Optional[Union[timedelta, pd.Timedelta]] = timedelta(seconds=60),
+        read_type: ReaderType = ReaderType.INT,
+        get_status: bool = False,
+    ):
+        logger.warn(
             (
                 "This function has been renamed to read() and is deprecated. "
                 "Please call 'read()' instead"
             )
         )
         return self.read(
             tags=tags,
             start_time=start_time,
             end_time=stop_time,
             ts=ts,
             read_type=read_type,
-            get_status=False,
+            get_status=get_status,
         )
 
     def read(
         self,
-        tags,
-        start_time=None,
-        end_time=None,
-        ts=60,
-        read_type=ReaderType.INT,
-        get_status=False,
-    ):
+        tags: Union[str, List[str]],
+        start_time: Optional[Union[datetime, pd.Timestamp, str]] = None,
+        end_time: Optional[Union[datetime, pd.Timestamp, str]] = None,
+        ts: Optional[Union[timedelta, pd.Timedelta, int]] = 60,
+        read_type: ReaderType = ReaderType.INT,
+        get_status: bool = False,
+    ) -> pd.DataFrame:
         """Reads values for the specified [tags] from the IMS server for the
         time interval from [start_time] to [stop_time] in intervals [ts].
 
         The interval [ts] can be specified as pd.Timedelta or as an integer,
         in which case it will be interpreted as seconds.
 
         Default value for [read_type] is ReaderType.INT, which interpolates
@@ -503,28 +556,27 @@
         if not isinstance(ts, pd.Timedelta):
             ts = pd.Timedelta(ts, unit="s")
 
         oldtags = tags
         tags = list(dict.fromkeys(tags))
         if len(oldtags) > len(tags):
             duplicates = set([x for n, x in enumerate(oldtags) if x in oldtags[:n]])
-            warnings.warn(
-                f"Duplicate tags found, removed duplicates: {', '.join(duplicates)}",
-                DuplicateTagsWarning,
+            logger.warning(
+                f"Duplicate tags found, removed duplicates: {', '.join(duplicates)}"
             )
         cols = []
         for tag in tags:
             cols.append(
                 self._read_single_tag(
-                    tag,
-                    start_time,
-                    end_time,
-                    ts,
-                    read_type,
-                    get_status,
+                    tag=tag,
+                    start_time=start_time,
+                    stop_time=end_time,
+                    ts=ts,
+                    read_type=read_type,
+                    get_status=get_status,
                     cache=self.cache,
                 )
             )
         return pd.concat(cols, axis=1)
 
     def query_sql(self, query: str, parse: bool = True):
         """[summary]
```

### Comparing `tagreader-4.0.1/tagreader/odbc_handlers.py` & `tagreader-4.0.3/tagreader/odbc_handlers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import warnings
-from typing import Union
+from typing import Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 import pyodbc
 
-from .utils import ReaderType, find_registry_key, logging, winreg
+from tagreader.utils import ReaderType, find_registry_key, logging, winreg
 
 logging.basicConfig(
     format=" %(asctime)s %(levelname)s: %(message)s", level=logging.INFO
 )
 
 
 def list_aspen_servers():
@@ -29,15 +29,15 @@
             "This function is deprecated and will be removed."
             "Please call 'list_sources(\"pi\")' instead"
         )
     )
     return list_pi_sources()
 
 
-def list_aspen_sources():
+def list_aspen_sources() -> List[str]:
     source_list = []
     reg_adsa = winreg.OpenKey(
         winreg.HKEY_CURRENT_USER,
         r"Software\AspenTech\ADSA\Caches\AspenADSA\\" + os.getlogin(),
     )
     num_sources, _, _ = winreg.QueryInfoKey(reg_adsa)
     for i in range(0, num_sources):
@@ -58,31 +58,42 @@
         num_sources, _, _ = winreg.QueryInfoKey(reg_key)
         for i in range(0, num_sources):
             source_list.append(winreg.EnumKey(reg_key, i))
     return source_list
 
 
 class AspenHandlerODBC:
-    def __init__(self, host=None, port=None, options={}):
+    def __init__(
+        self,
+        host: Optional[str] = None,
+        port: Optional[int] = None,
+        options: Dict[str, Union[int, float, str]] = {},
+    ):
         self.host = host
         self.port = port
         self.conn = None
         self.cursor = None
         self._max_rows = options.get("max_rows", 100000)
         self._connection_string = options.get("connection_string", None)
 
     def generate_connection_string(self):
         if self._connection_string is None:
-            return f"DRIVER={{AspenTech SQLPlus}};HOST={self.host};PORT={self.port};READONLY=Y;MAXROWS={self._max_rows}"  # noqa E501
+            return f"DRIVER={{AspenTech SQLPlus}};HOST={self.host};PORT={self.port};READONLY=Y;MAXROWS={self._max_rows}"
         else:
             return self._connection_string
 
     @staticmethod
     def generate_read_query(
-        tag, mapdef, start_time, stop_time, sample_time, read_type, get_status=False
+        tag: str,
+        mapdef: Optional[Dict[str, str]],
+        start_time: pd.Timestamp,
+        stop_time: pd.Timestamp,
+        sample_time: Optional[Union[int, pd.Timestamp]],
+        read_type: ReaderType,
+        get_status: bool = False,
     ):
         if mapdef is None:
             mapdef = {}
         if read_type in [
             ReaderType.COUNT,
             ReaderType.GOOD,
             ReaderType.BAD,
@@ -115,15 +126,15 @@
                 if seconds <= 0:
                     raise NotImplementedError
                     # sample_time = (stop_time-start_time).totalseconds
 
         timecast_format_query = "%Y-%m-%dT%H:%M:%SZ"  # 05-jan-18 14:00:00
 
         request_num = {
-            ReaderType.SAMPLED: 4,  # VALUES request (actual recorded data), history  # noqa: E501
+            ReaderType.SAMPLED: 4,  # VALUES request (actual recorded data), history
             ReaderType.SHAPEPRESERVING: 3,  # FITS request, history
             ReaderType.INT: 7,  # TIMES2_EXTENDED request, history
             ReaderType.COUNT: 0,  # Actual data points are used, aggregates
             ReaderType.GOOD: 0,  # Actual data points are used, aggregates
             ReaderType.TOTAL: 0,  # Actual data points are used, aggregates
             ReaderType.NOTGOOD: 0,  # Actual data points are used, aggregates
             ReaderType.SNAPSHOT: None,
@@ -134,15 +145,15 @@
         from_column = {
             ReaderType.SAMPLED: "history",
             ReaderType.SHAPEPRESERVING: "history",
             ReaderType.INT: "history",
             ReaderType.SNAPSHOT: '"' + str(tag) + '"',
         }.get(read_type, "aggregates")
         # For RAW: historyevent?
-        # Ref https://help.sap.com/saphelp_pco151/helpdata/en/4c/72e34ee631469ee10000000a15822d/content.htm?no_cache=true  # noqa: E501
+        # Ref https://help.sap.com/saphelp_pco151/helpdata/en/4c/72e34ee631469ee10000000a15822d/content.htm?no_cache=true
 
         ts = "ts"
         if from_column == "aggregates":
             ts = "ts_start"
         elif read_type == ReaderType.SNAPSHOT:
             ts = mapdef.get("MAP_CurrentTimeStamp", "IP_INPUT_TIME")
 
@@ -209,78 +220,81 @@
         if "%" in tag:
             query.append(f"LIKE '{tag}'")
         else:
             query.append(f"='{tag}'")
         query.append("AND m.MAP_IsDefault = 'TRUE'")
         return " ".join(query)
 
-    def _get_mapdef_for_search(self, tag):
+    def _get_mapdef_for_search(self, tag: str):
         query = self._generate_query_get_mapdef_for_search(tag)
         self.cursor.execute(query)
         colnames = [col[0] for col in self.cursor.description]
         rows = self.cursor.fetchall()
         temp = [dict(zip(colnames, row)) for row in rows]
         mapdef = {}
         for t in temp:
             if t["tagname"] not in mapdef:
                 mapdef[t["tagname"]] = [t]
             else:
                 mapdef[t["tagname"]].append(t)
         return mapdef
 
     @staticmethod
-    def _generate_query_search_tag(mapdef, desc=None):
+    def _generate_query_search_tag(
+        mapdef: Optional[Dict[str, str]], desc: Optional[str] = None
+    ):
         if mapdef["MAP_DefinitionRecord"] is None:
             return None
         query = [
             f"SELECT \"{mapdef['MAP_Description']}\"",
             f"FROM {mapdef['MAP_DefinitionRecord']}",
             f"WHERE name = '{mapdef['tagname']}'",
         ]
         if desc is not None:
             query.append(f"AND {mapdef['MAP_Description']} like '{desc}'")
         return " ".join(query)
 
     @staticmethod
-    def _generate_query_get_mapdefs(tag):
+    def _generate_query_get_mapdefs(tag: str) -> str:
         query = [
             "SELECT m.NAME, m.MAP_DefinitionRecord, m.MAP_IsDefault,",
             "m.MAP_Description, m.MAP_Units, m.MAP_Base, m.MAP_Range,",
             "m.MAP_CurrentValue, m.MAP_CurrentTimeStamp, m.MAP_CurrentQuality,",
             f'm.MAP_HistoryValue FROM "{tag}" t',
             "LEFT JOIN atmapdef m ON t.definition = m.MAP_DefinitionRecord",
         ]
         return " ".join(query)
 
-    def _get_mapdefs(self, tag):
+    def _get_mapdefs(self, tag: str) -> List[Dict[str, str]]:
         query = self._generate_query_get_mapdefs(tag)
         self.cursor.execute(query)
         colnames = [col[0] for col in self.cursor.description]
         rows = self.cursor.fetchall()
         mapdefs = [dict(zip(colnames, row)) for row in rows]
         return mapdefs
 
-    def _get_specific_mapdef(self, tagname, mapping):
+    def _get_specific_mapdef(
+        self, tagname: str, mapping: str
+    ) -> Optional[Dict[str, str]]:
         mapdefs = self._get_mapdefs(tagname)
         for mapdef in mapdefs:
             if mapdef["NAME"].lower() == mapping.lower():
                 return mapdef
         return None
 
-    def _get_default_mapdef(self, tagname):
+    def _get_default_mapdef(self, tagname: str) -> Optional[Dict[str, str]]:
         mapdefs = self._get_mapdefs(tagname)
         for mapdef in mapdefs:
             if mapdef["MAP_IsDefault"] == "TRUE":
                 return mapdef
         return None
 
-    def search(self, tag=None, desc=None):
-        if tag is None:
-            raise ValueError("Tag is a required argument")
-
+    def search(
+        self, tag: Optional[str] = None, desc: Optional[str] = None
+    ) -> List[Tuple[str, str]]:
         tag = tag.replace("*", "%") if isinstance(tag, str) else None
         desc = desc.replace("*", "%") if isinstance(desc, str) else None
 
         mapdef = self._get_mapdef_for_search(tag)
 
         res = []
         for tagname in mapdef:  # TODO: Refactor
@@ -297,64 +311,70 @@
             # Match, but no value for description
             if r[0] is not None:
                 description = r[0]
             res.append((tagname, description))
         res = list(set(res))
         return res
 
-    def _get_tag_metadata(self, tag):
+    def _get_tag_metadata(self, tag: str):
         return None
 
-    def _get_tag_unit(self, tag):
+    def _get_tag_unit(self, tag: str):
         (tagname, mapping) = tag.split(";") if ";" in tag else (tag, None)
         if mapping is None:
             mapdef = self._get_default_mapdef(tagname)
         else:
-            mapdef = self._get_specific_mapdef(tagname, mapping)
+            mapdef = self._get_specific_mapdef(tagname=tagname, mapping=mapping)
         query = f"SELECT name, \"{mapdef['MAP_Units']}\" as engunit FROM \"{tagname}\""
         self.cursor.execute(query)
         res = self.cursor.fetchone()
         if not res.engunit:
             res.engunit = ""
         return res.engunit
 
-    def _get_tag_description(self, tag):
+    def _get_tag_description(self, tag: str):
         (tagname, mapping) = tag.split(";") if ";" in tag else (tag, None)
         if mapping is None:
             mapping = self._get_default_mapdef(tagname)
         else:
-            mapping = self._get_specific_mapdef(tagname, mapping)
+            mapping = self._get_specific_mapdef(tagname=tagname, mapping=mapping)
         query = [
             f"SELECT name, \"{mapping['MAP_Description']}\" as description",
             f' FROM "{tagname}"',
         ]
         query = " ".join(query)
         self.cursor.execute(query)
         res = self.cursor.fetchone()
         if not res.description:
             res.description = ""
         return res.description
 
     def read_tag(
         self,
-        tag,
-        start_time,
-        stop_time,
-        sample_time,
-        read_type,
-        metadata=None,
-        get_status=False,
+        tag: str,
+        start_time: pd.Timestamp,
+        stop_time: pd.Timestamp,
+        sample_time: Optional[Union[int, pd.Timestamp]],
+        read_type: ReaderType,
+        metadata: Optional[Dict[str, str]] = None,
+        get_status: bool = False,
     ):
         (cleantag, mapping) = tag.split(";") if ";" in tag else (tag, None)
         mapdef = dict()
 
         if mapping is not None:
-            mapdef = self._get_specific_mapdef(cleantag, mapping)
+            mapdef = self._get_specific_mapdef(tagname=cleantag, mapping=mapping)
         query = self.generate_read_query(
-            cleantag, mapdef, start_time, stop_time, sample_time, read_type, get_status
+            tag=cleantag,
+            mapdef=mapdef,
+            start_time=start_time,
+            stop_time=stop_time,
+            sample_time=sample_time,
+            read_type=read_type,
+            get_status=get_status,
         )
 
         with warnings.catch_warnings():
             warnings.filterwarnings(
                 "ignore", message="^pandas.*SQLAlchemy.*", category=UserWarning
             )
             df = pd.read_sql(
@@ -367,30 +387,35 @@
         if get_status:
             df["status"] = df["status"].astype(int)
         df = df.tz_localize("UTC")
         return df.rename(columns={"value": tag, "status": tag + "::status"})
 
     def query_sql(
         self, query: str, parse: bool = True
-    ) -> Union[pd.DataFrame, pyodbc.Cursor]:  # noqa:E501
+    ) -> Union[pd.DataFrame, pyodbc.Cursor]:
         if not parse:
             cursor = self.conn.cursor()
             cursor.execute(query)
             return cursor
         else:
             with warnings.catch_warnings():
                 warnings.filterwarnings(
                     "ignore", message="^pandas.*SQLAlchemy.*", category=UserWarning
                 )
                 res = pd.read_sql(query, self.conn)
             return res
 
 
 class PIHandlerODBC:
-    def __init__(self, host=None, port=None, options={}):
+    def __init__(
+        self,
+        host: Optional[str] = None,
+        port: Optional[int] = None,
+        options: Dict[str, Union[int, float, str]] = {},
+    ):
         self.host = host
         self.port = port
         self.conn = None
         self.cursor = None
         self._max_rows = options.get("max_rows", 100000)
         # TODO: Find default das_server under
         # HKLM\SOFTWARE\Wow6432Node\PISystem\Analytics\InstallData/AFServer
@@ -402,42 +427,42 @@
         # print(self._das_server)
 
     def generate_connection_string(self):
         if self._connection_string is None:
             return (
                 f"DRIVER={{PI ODBC Driver}};Server={self._das_server};"
                 "Trusted_Connection=Yes;Command Timeout=1800;Provider Type=PIOLEDB;"
-                f'Provider String={{Data source={self.host.replace(".statoil.net", "")};'  # noqa: E501
+                f'Provider String={{Data source={self.host.replace(".statoil.net", "")};'
                 "Integrated_Security=SSPI;Time Zone=UTC};"
             )
         else:
             return self._connection_string
 
     @staticmethod
-    def generate_search_query(tag=None, desc=None):
+    def generate_search_query(tag: Optional[str] = None, desc: Optional[str] = None):
         query = ["SELECT tag, descriptor as description FROM pipoint.pipoint2 WHERE"]
         if tag is not None:
             query.extend(["tag LIKE '{tag}'".format(tag=tag.replace("*", "%"))])
         if tag is not None and desc is not None:
             query.extend(["AND"])
         if desc is not None:
             query.extend(
                 ["descriptor LIKE '{desc}'".format(desc=desc.replace("*", "%"))]
             )
         return " ".join(query)
 
     def generate_read_query(
         self,
-        tag,
-        start_time,
-        stop_time,
-        sample_time,
-        read_type,
-        metadata=None,
-        get_status=False,
+        tag: str,
+        start_time: pd.Timestamp,
+        stop_time: pd.Timestamp,
+        sample_time: Optional[Union[int, pd.Timestamp]],
+        read_type: ReaderType,
+        metadata: Optional[Dict[str, str]] = None,
+        get_status: bool = False,
     ):
         if read_type in [
             ReaderType.COUNT,
             ReaderType.GOOD,
             ReaderType.BAD,
             ReaderType.TOTAL,
             ReaderType.SUM,
@@ -490,15 +515,15 @@
         elif ReaderType.BAD == read_type:
             query = ["SELECT 100-CAST(pctgood as FLOAT32)"]
         elif ReaderType.RAW == read_type:
             query = [f"SELECT TOP {self._max_rows} CAST(value as FLOAT32)"]
         else:
             query = ["SELECT CAST(value as FLOAT32)"]
 
-        # query.extend([f"AS value, FORMAT(time, '{timecast_format_output}') AS timestamp FROM {source} WHERE tag='{tag}'"])  # noqa E501
+        # query.extend([f"AS value, FORMAT(time, '{timecast_format_output}') AS timestamp FROM {source} WHERE tag='{tag}'"])
         query.extend(["AS value,"])
 
         if get_status:
             query.extend(["status, questionable, substituted,"])
 
         query.extend([f"time FROM {source} WHERE tag='{tag}'"])  # __utctime also works
 
@@ -510,96 +535,104 @@
         if ReaderType.GOOD == read_type:
             query.extend(["AND questionable = FALSE"])
         elif ReaderType.NOTGOOD == read_type:
             query.extend(["AND questionable = TRUE"])
         elif ReaderType.SHAPEPRESERVING == read_type:
             query.extend(
                 [
-                    f"AND (intervalcount = {int((stop_time-start_time).total_seconds()/seconds)})"  # noqa E501
+                    f"AND (intervalcount = {int((stop_time - start_time).total_seconds() / seconds)})"
                 ]
             )
         elif ReaderType.RAW == read_type:
             pass
         elif read_type not in [ReaderType.SNAPSHOT, ReaderType.RAW]:
             query.extend([f"AND (timestep = '{seconds}s')"])
 
         if ReaderType.SNAPSHOT != read_type:
             query.extend(["ORDER BY time"])
 
         return " ".join(query)
 
-    def set_options(self, options):
+    def set_options(self, options: Dict[str, str]):
         pass
 
     def connect(self):
         connection_string = self.generate_connection_string()
         # The default autocommit=False is not supported by PI odbc driver.
         self.conn = pyodbc.connect(connection_string, autocommit=True)
         self.cursor = self.conn.cursor()
 
-    def search(self, tag=None, desc=None):
-        query = self.generate_search_query(tag, desc)
+    def search(
+        self, tag: Optional[str] = None, desc: Optional[str] = None
+    ) -> List[Tuple[str, str]]:
+        query = self.generate_search_query(tag=tag, desc=desc)
         self.cursor.execute(query)
         return self.cursor.fetchall()
 
-    def _get_tag_metadata(self, tag):
+    def _get_tag_metadata(self, tag: str) -> Optional[Dict[str, str]]:
         # Returns None if tag not found.
-        query = f"SELECT digitalset, engunits, descriptor FROM pipoint.pipoint2 WHERE tag='{tag}'"  # noqa E501
+        query = f"SELECT digitalset, engunits, descriptor FROM pipoint.pipoint2 WHERE tag='{tag}'"
         self.cursor.execute(query)
         desc = self.cursor.description
         col_names = [col[0] for col in desc]
         res = self.cursor.fetchone()
         if res is None:
             warnings.warn(f"Tag {tag} not found")
             return None
         metadata = dict(zip(col_names, res))
         return metadata
 
-    def _get_tag_description(self, tag):
+    def _get_tag_description(self, tag: str):
         query = f"SELECT descriptor FROM pipoint.pipoint2 WHERE tag='{tag}'"
         self.cursor.execute(query)
         desc = self.cursor.fetchone()
         return desc[0]
 
     def _get_tag_unit(self, tag):
         query = f"SELECT engunits FROM pipoint.pipoint2 WHERE tag='{tag}'"
         self.cursor.execute(query)
         unit = self.cursor.fetchone()
         return unit[0]
 
     @staticmethod
-    def _is_summary(read_type):
+    def _is_summary(read_type: ReaderType):
         if read_type in [
             ReaderType.AVG,
             ReaderType.MIN,
             ReaderType.MAX,
             ReaderType.RNG,
             ReaderType.STD,
             ReaderType.VAR,
         ]:
             return True
         return False
 
     def read_tag(
         self,
-        tag,
-        start_time,
-        stop_time,
-        sample_time,
-        read_type,
-        metadata=None,
-        get_status=False,
+        tag: str,
+        start_time: pd.Timestamp,
+        stop_time: pd.Timestamp,
+        sample_time: Optional[Union[int, pd.Timestamp]],
+        read_type: ReaderType,
+        metadata: Optional[Dict[str, str]] = None,
+        get_status: bool = False,
     ):
         if metadata is None:
             # Tag not found
             # TODO: Handle better and similarly across all handlers.
             return pd.DataFrame()
 
         query = self.generate_read_query(
-            tag, start_time, stop_time, sample_time, read_type, get_status=get_status
+            tag=tag,
+            start_time=start_time,
+            stop_time=stop_time,
+            sample_time=sample_time,
+            read_type=read_type,
+            get_status=get_status,
+            metadata=None,
         )
 
         with warnings.catch_warnings():
             warnings.filterwarnings(
                 "ignore", message="^pandas.*SQLAlchemy.*", category=UserWarning
             )
             df = pd.read_sql(
@@ -616,15 +649,15 @@
             df.index = df.index - sample_time
             df = df.drop(df.index[0])
 
         df = df.tz_localize("UTC")
 
         if len(metadata["digitalset"]) > 0:
             self.cursor.execute(
-                f"SELECT code, offset FROM pids WHERE digitalset='{metadata['digitalset']}'"  # noqa: E501
+                f"SELECT code, offset FROM pids WHERE digitalset='{metadata['digitalset']}'"
             )
             digitalset = self.cursor.fetchall()
             code = [x[0] for x in digitalset]
             offset = [x[1] for x in digitalset]
             df = df.replace(code, offset)
 
         if get_status:
@@ -637,15 +670,15 @@
             )
             df = df.drop(columns=["questionable", "substituted"])
 
         return df.rename(columns={"value": tag, "status": tag + "::status"})
 
     def query_sql(
         self, query: str, parse: bool = True
-    ) -> Union[pd.DataFrame, pyodbc.Cursor]:  # noqa: E501
+    ) -> Union[pd.DataFrame, pyodbc.Cursor]:
         if not parse:
             cursor = self.conn.cursor()
             cursor.execute(query)
             return cursor
         else:
             with warnings.catch_warnings():
                 warnings.filterwarnings(
```

### Comparing `tagreader-4.0.1/tagreader/utils.py` & `tagreader-4.0.3/tagreader/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import enum
 import logging
 import platform
 import warnings
+from datetime import datetime
+from typing import Union
 
 import pandas as pd
 import pytz
 
 
 def is_windows() -> bool:
     return platform.system() == "Windows"
@@ -24,15 +26,15 @@
 
 
 if is_mac():
     import socket
     import subprocess
 
 
-def find_registry_key(base_key, search_key_name):
+def find_registry_key(base_key, search_key_name: str):
     search_key_name = search_key_name.lower()
     if base_key is not None:
         num_keys, _, _ = winreg.QueryInfoKey(base_key)
         for i in range(0, num_keys):
             key_name = winreg.EnumKey(base_key, i)
             if key_name.lower() == search_key_name:
                 return winreg.OpenKey(base_key, key_name)
@@ -41,15 +43,15 @@
                     winreg.OpenKey(base_key, key_name), search_key_name
                 )
             if key is not None:
                 return key
     return None
 
 
-def find_registry_key_from_name(base_key, search_key_name):
+def find_registry_key_from_name(base_key, search_key_name: str):
     search_key_name = search_key_name.lower()
     num_keys, _, _ = winreg.QueryInfoKey(base_key)
     key = key_string = None
     for i in range(0, num_keys):
         try:
             key_string = winreg.EnumKey(base_key, i)
             key = winreg.OpenKey(base_key, key_string)
@@ -59,28 +61,31 @@
                 if str(key_name).lower() == search_key_name:
                     break
         except Exception as err:
             logging.error("{}: {}".format(i, err))
     return key, key_string
 
 
-def ensure_datetime_with_tz(date_stamp, tz="Europe/Oslo"):
+def ensure_datetime_with_tz(
+    date_stamp: Union[datetime, str, pd.Timestamp],
+    tz: str = "Europe/Oslo",
+) -> pd.Timestamp:
     if isinstance(date_stamp, str):
         try:
             date_stamp = pd.to_datetime(date_stamp, format="ISO8601")
         except ValueError:
             date_stamp = pd.to_datetime(date_stamp, dayfirst=True)
 
     if not date_stamp.tzinfo:
         date_stamp = pytz.timezone(tz).localize(date_stamp)
 
     return date_stamp
 
 
-def urljoin(*args):
+def urljoin(*args) -> str:
     """Joins components of URL. Ensures slashes are inserted or removed where
     needed, and does not strip trailing slash of last element.
 
     Arguments:
         str
     Returns:
         str -- Generated URL
@@ -110,15 +115,15 @@
     GOOD = enum.auto()  # Number of good data points
     BAD = NOTGOOD = enum.auto()  # Number of not good data points
     TOTAL = enum.auto()  # Number of total data
     SUM = enum.auto()  # Sum of data
     SNAPSHOT = FINAL = LAST = enum.auto()  # Last sampled value
 
 
-def add_statoil_root_certificate(noisy=True):
+def add_statoil_root_certificate(noisy: bool = True) -> bool:
     """This is a utility function for Equinor employees on Equinor managed machines.
 
     The function searches for the Statoil Root certificate in the
     cert store and imports it to the cacert bundle. Does nothing if not
     running on Equinor host.
 
     This needs to be repeated after updating the cacert module.
@@ -130,14 +135,15 @@
     import ssl
 
     import certifi
 
     STATOIL_ROOT_PEM_HASH = "ce7bb185ab908d2fea28c7d097841d9d5bbf2c76"
 
     found = False
+    der = None
 
     if is_linux():
         return True
     elif is_windows():
         if noisy:
             print("Scanning CA certs in Windows cert store", end="")
         for cert in ssl.enum_certificates("CA"):
@@ -161,15 +167,15 @@
             c = get_macos_statoil_certificates()
             for cert in c:
                 if hashlib.sha1(cert).hexdigest() == STATOIL_ROOT_PEM_HASH:
                     der = cert
                     found = True
                     break
 
-    if found:
+    if found and der:
         pem = ssl.DER_cert_to_PEM_cert(der)
         if pem in certifi.contents():
             if noisy:
                 print("Certificate already exists in certifi store. Nothing to do.")
         else:
             if noisy:
                 print("Writing certificate to certifi store.")
```

### Comparing `tagreader-4.0.1/tagreader/web_handlers.py` & `tagreader-4.0.3/tagreader/web_handlers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,66 +1,67 @@
 import datetime
 import re
-import urllib
+import urllib.parse
 import warnings
-from typing import Union
+from abc import ABC, abstractmethod
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 import pytz
 import requests
+import urllib3
+from requests import Response
 from requests_kerberos import OPTIONAL, HTTPKerberosAuth
 
-from .utils import ReaderType, is_mac, is_windows, logging, urljoin
+from tagreader.utils import ReaderType, is_mac, is_windows, urljoin
 
 # Requests will use simplejson if it has been installed, so handle both errors here
 try:
     from simplejson.errors import JSONDecodeError
 except ImportError:
     from json.decoder import JSONDecodeError
 
-logging.basicConfig(
-    format=" %(asctime)s %(levelname)s: %(message)s", level=logging.INFO
-)
 
-
-def get_verifySSL():
+def get_verifySSL() -> Union[bool, str]:
     if is_windows() or is_mac():
         return True
     return "/etc/ssl/certs/ca-bundle.trust.crt"
 
 
-def get_auth_pi():
+def get_auth_pi() -> HTTPKerberosAuth:
     return HTTPKerberosAuth(mutual_authentication=OPTIONAL)
 
 
-def get_url_pi():
+def get_url_pi() -> str:
     return r"https://piwebapi.equinor.com/piwebapi"
 
 
-def get_auth_aspen():
+def get_auth_aspen() -> HTTPKerberosAuth:
     return HTTPKerberosAuth(mutual_authentication=OPTIONAL)
 
 
-def get_url_aspen():
+def get_url_aspen() -> str:
     # internal url (redirects to dll)
     return r"https://aspenone.api.equinor.com"
 
 
-def list_aspenone_sources(url=None, auth=None, verifySSL=None):
+def list_aspenone_sources(
+    url: Optional[str] = None,
+    auth: Optional[Any] = None,
+    verifySSL: Optional[bool] = None,
+) -> List[str]:
     if url is None:
         url = get_url_aspen()
 
     if auth is None:
         auth = get_auth_aspen()
 
     if verifySSL is False:
-        requests.packages.urllib3.disable_warnings(
-            requests.packages.urllib3.exceptions.InsecureRequestWarning
-        )
+        urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
     elif verifySSL is None:
         verifySSL = get_verifySSL()
 
     url_ = urljoin(url, "DataSources")
     params = {"service": "ProcessData", "allQuotes": 1}
 
     res = requests.get(url_, params=params, auth=auth, verify=verifySSL)
@@ -73,25 +74,27 @@
     elif res.status_code == 404:
         print("Not found")
     elif res.status_code == 401:
         print("Not authorized")
     res.raise_for_status()
 
 
-def list_piwebapi_sources(url=None, auth=None, verifySSL=None):
+def list_piwebapi_sources(
+    url: Optional[str] = None,
+    auth: Optional[Any] = None,
+    verifySSL: Optional[bool] = None,
+) -> List[str]:
     if url is None:
         url = get_url_pi()
 
     if auth is None:
         auth = get_auth_pi()
 
     if verifySSL is False:
-        requests.packages.urllib3.disable_warnings(
-            requests.packages.urllib3.exceptions.InsecureRequestWarning
-        )
+        urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
     elif verifySSL is None:
         verifySSL = get_verifySSL()
 
     url_ = urljoin(url, "dataservers")
     res = requests.get(url_, auth=auth, verify=verifySSL)
 
     if res.status_code == 200:
@@ -103,59 +106,99 @@
     elif res.status_code == 404:
         print("Not found")
     elif res.status_code == 401:
         print("Not authorized")
     res.raise_for_status()
 
 
-class AspenHandlerWeb:
+class BaseHandlerWeb(ABC):
     def __init__(
         self,
-        datasource=None,
-        url=None,
-        auth=None,
-        verifySSL=None,
-        options={},
+        datasource: Optional[str] = None,
+        url: Optional[str] = None,
+        auth: Optional[Any] = None,
+        verifySSL: Optional[bool] = None,
     ):
-        self._max_rows = options.get("max_rows", 100000)
-        if url is None:
-            url = get_url_aspen()
         self.datasource = datasource
         self.base_url = url
         self.session = requests.Session()
         self.session.auth = auth if auth is not None else get_auth_aspen()
         if verifySSL is False:
-            requests.packages.urllib3.disable_warnings(
-                requests.packages.urllib3.exceptions.InsecureRequestWarning
-            )
+            urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
         self.session.verify = verifySSL if verifySSL is not None else get_verifySSL()
+
+    def fetch(self, url, params=None) -> Response:
+        if not self.session.verify:
+            urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
+
+        res = self.session.get(url, params=params)
+        res.raise_for_status()
+        return res
+
+    def connect(self):
+        try:
+            self.verify_connection(self.datasource)
+        except requests.ConnectionError:
+            raise ConnectionError(
+                f"Not able to connect to {self.base_url}. Check network connection."
+            ) from None
+
+    @abstractmethod
+    def verify_connection(self, datasource: str):
+        ...
+
+
+class AspenHandlerWeb(BaseHandlerWeb):
+    def __init__(
+        self,
+        datasource: Optional[str] = None,
+        url: Optional[str] = None,
+        auth: Optional[Any] = None,
+        verifySSL: Optional[bool] = None,
+        options: Dict[str, Any] = {},
+    ):
+        if url is None:
+            url = get_url_aspen()
+        if auth is None:
+            auth = get_auth_aspen()
+        super().__init__(
+            datasource=datasource,
+            url=url,
+            auth=auth,
+            verifySSL=verifySSL,
+        )
+        self._max_rows = options.get("max_rows", 100000)
         self._connection_string = ""  # Used for raw SQL queries
 
     @staticmethod
     def generate_connection_string(host, *_, **__):
         raise NotImplementedError
 
     @staticmethod
-    def generate_search_query(tag=None, desc=None, datasource=None):
+    def generate_search_query(
+        tag: Optional[str] = None,
+        desc: Optional[str] = None,
+        datasource: Optional[str] = None,
+    ) -> Dict[str, Any]:
         if not datasource:
             raise ValueError("Data source is required argument")
         # Aspen Web API expects single space instead of consecutive spaces.
         tag = " ".join(tag.split())
         params = {"datasource": datasource, "tag": tag, "max": 100, "getTrendable": 0}
         return params
 
     def generate_read_query(
         self,
-        tagname,
-        mapname,
-        start_time,
-        stop_time,
-        sample_time,
-        read_type,
-        metadata=None,
+        tagname: str,
+        mapname: Optional[str],
+        start_time: pd.Timestamp,
+        stop_time: pd.Timestamp,
+        sample_time: Optional[Union[int, pd.Timestamp]],
+        read_type: ReaderType,
+        metadata: Optional[Any] = None,
     ):
         # Maxpoints is used for Actual (raw) and Bestfit (shapepreserving).
         # Probably need to handle this in another way at some point
         maxpoints = self._max_rows
         stepped = 0
         outsiders = 0
 
@@ -197,16 +240,16 @@
         query += f"<D><![CDATA[{self.datasource}]]></D>" "<F><![CDATA[VAL]]></F>"
 
         if read_type == ReaderType.SNAPSHOT:
             query += "<VS>1</VS>"
         else:
             query += (
                 "<HF>0</HF>"  # History format: 0=Raw, 1=RecordAsString
-                f"<St>{int(start_time.timestamp())*1000}</St>"
-                f"<Et>{int(stop_time.timestamp())*1000}</Et>"
+                f"<St>{int(start_time.timestamp()) * 1000}</St>"
+                f"<Et>{int(stop_time.timestamp()) * 1000}</Et>"
                 f"<RT>{rt}</RT>"
             )
         if read_type in [ReaderType.RAW, ReaderType.SHAPEPRESERVING]:
             query += f"<X>{maxpoints}</X>"
         if read_type not in [ReaderType.INT, ReaderType.SNAPSHOT]:
             query += f"<O>{outsiders}</O>"
         if read_type not in [ReaderType.RAW]:
@@ -236,51 +279,37 @@
                 # TODO: Unify anchor selection among all handlers
                 "<DSA>0</DSA>"  # DS Adjust: 0=False, 1=True
             )
         query += "</Tag></Q>"
 
         return query
 
-    def verify_connection(self, datasource):
+    def verify_connection(self, datasource: str):
         """Connects to the URL and verifies that the provided data source exists.
 
         :param datasource: Data source to look for
         :type datasource: String
         :raises ConnectionError: If connection fails
         :return: True if datasource exists, False if not.
         :rtype: Bool
         """
         url = urljoin(self.base_url, "Datasources")
         params = {"service": "ProcessData", "allQuotes": 1}
-        if not self.session.verify:
-            requests.packages.urllib3.disable_warnings(
-                requests.packages.urllib3.exceptions.InsecureRequestWarning
-            )
-
-        res = self.session.get(url, params=params)
-        res.raise_for_status()
-        j = res.json()
+        r = self.fetch(url=url, params=params)
+        j = r.json()
         for item in j["data"]:
             if item["n"] == datasource:
                 return True
         return False
 
-    def connect(self):
-        try:
-            self.verify_connection(self.datasource)
-        except requests.ConnectionError:
-            raise ConnectionError(
-                f"Not able to connect to {self.base_url}. Check network connection."
-            ) from None
-
     @staticmethod
     def split_tagmap(tagmap):
         return tuple(tagmap.split(";") if ";" in tagmap else (tagmap, None))
 
-    def generate_get_unit_query(self, tag):
+    def generate_get_unit_query(self, tag: str):
         tagname, _ = self.split_tagmap(tag)
         parts = [
             '<Q allQuotes="1" attributeData="1">',
             "<Tag>",
             f"<N><![CDATA[{tagname}]]></N>",
             "<T>0</T>",  # What is this?
             f"<G><![CDATA[{tagname}]]></G>",
@@ -292,70 +321,72 @@
             "<VS>0</VS>",  # What is this?
             "</AL>",
             "</Tag>",
             "</Q>",
         ]
         return "".join(parts)
 
-    def generate_get_map_query(self, tagname):
+    def generate_get_map_query(self, tagname: str):
         parts = [
             '<Q allQuotes="1" categoryInfo="1">',
             "<Tag>",
             f"<N><![CDATA[{tagname}]]></N>",
             "<T>0</T>",  # What is this?
             f"<G><![CDATA[{tagname}]]></G>",
             f"<D><![CDATA[{self.datasource}]]></D>",
             "</Tag>",
             "</Q>",
         ]
         return "".join(parts)
 
-    def _get_maps(self, tagname):
+    def _get_maps(self, tagname: str):
         params = self.generate_get_map_query(tagname)
         url = urljoin(self.base_url, "TagInfo")
-        res = self.session.get(url, params=params)
-        res.raise_for_status()
+        res = self.fetch(url, params=params)
         j = res.json()
 
         if "tags" not in j["data"]:
             return {}
 
         ret = {}
         for item in j["data"]["tags"][0]["categories"][0]["ta"]:
             ret[item["m"]] = True if item["d"] == "True" else False
         return ret
 
-    def _get_default_mapname(self, tagname):
+    def _get_default_mapname(self, tagname: str):
         (tagname, _) = self.split_tagmap(tagname)
         allmaps = self._get_maps(tagname)
         for k, v in allmaps.items():
             if v:
                 return k
 
-    def search(self, tag=None, desc=None):
+    def search(
+        self, tag: Optional[str] = None, desc: Optional[str] = None
+    ) -> List[Tuple[str, str]]:
         if tag is None:
             raise ValueError("Tag is a required argument")
 
         tag = tag.replace("%", "*") if isinstance(tag, str) else None
         # Prepare for regex
         desc = desc.replace("%", "*") if isinstance(desc, str) else None
         desc = desc.replace("*", ".*") if isinstance(desc, str) else None
 
-        params = self.generate_search_query(tag, desc, self.datasource)
+        params = self.generate_search_query(
+            tag=tag, desc=desc, datasource=self.datasource
+        )
         # Ensure space is encoded as "%20" instead of default "+" and leave asterisks
         # unencoded. Otherwise searches for tags containing spaces break, as do wildcard
         # searches.
         encoded_params = urllib.parse.urlencode(
             params, safe="*", quote_via=urllib.parse.quote
         )
         url = urljoin(self.base_url, "Browse?")
         url += encoded_params
-        res = self.session.get(url)
+        res = self.fetch(url)
 
-        res.raise_for_status()
         j = res.json()
 
         if "tags" not in j["data"]:
             return []
 
         ret = []
         for item in j["data"]["tags"]:
@@ -366,36 +397,35 @@
         if not desc:
             return ret
 
         r = re.compile(desc)
         ret = [x for x in ret if r.search(x[1])]
         return ret
 
-    def _get_tag_metadata(self, tag):
+    def _get_tag_metadata(self, tag: str):
         return {}  # FIXME
 
-    def _get_tag_unit(self, tag):
+    def _get_tag_unit(self, tag: str):
         query = self.generate_get_unit_query(tag)
         url = urljoin(self.base_url, "TagInfo")
-        res = self.session.get(url, params=query)
-        res.raise_for_status()
+        res = self.fetch(url, params=query)
         j = res.json()
         try:
             attrdata = j["data"]["tags"][0]["attrData"]
         except Exception:
             print(f"Error. I got this: {j}")
             raise KeyError
         unit = ""
         for a in attrdata:
             if a["g"] == "Units":
                 unit = a["samples"][0]["v"]
                 break
         return unit
 
-    def generate_get_description_query(self, tag):
+    def generate_get_description_query(self, tag: str):
         tagname, _ = self.split_tagmap(tag)
         parts = [
             '<Q allQuotes="1" attributeData="1">',
             "<Tag>",
             f"<N><![CDATA[{tagname}]]></N>",
             "<T>0</T>",  # What is this?
             f"<G><![CDATA[{tagname}]]></G>",
@@ -405,35 +435,34 @@
             "<VS>0</VS>",  # What is this?
             "</AL>",
             "</Tag>",
             "</Q>",
         ]
         return "".join(parts)
 
-    def _get_tag_description(self, tag):
+    def _get_tag_description(self, tag: str):
         query = self.generate_get_description_query(tag)
         url = urljoin(self.base_url, "TagInfo")
-        res = self.session.get(url, params=query)
-        res.raise_for_status()
+        res = self.fetch(url, params=query)
         j = res.json()
         try:
             desc = j["data"]["tags"][0]["attrData"][0]["samples"][0]["v"]
         except Exception:
             desc = ""
         return desc
 
     def read_tag(
         self,
-        tag,
-        start_time,
-        stop_time,
-        sample_time,
-        read_type,
-        metadata=None,
-        get_status=False,
+        tag: str,
+        start_time: Optional[pd.Timestamp],
+        stop_time: Optional[pd.Timestamp],
+        sample_time: Optional[Union[int, pd.Timestamp]],
+        read_type: ReaderType,
+        metadata: Optional[Dict[str, str]] = None,
+        get_status: bool = False,
     ):
         if read_type not in [
             ReaderType.INT,
             ReaderType.MIN,
             ReaderType.MAX,
             ReaderType.RNG,
             ReaderType.AVG,
@@ -458,19 +487,24 @@
         # both start and end time.
         if read_type == ReaderType.INT:
             stop_time = min(stop_time, start_time + sample_time * (self._max_rows - 1))
 
         tagname, mapname = self.split_tagmap(tag)
 
         params = self.generate_read_query(
-            tagname, mapname, start_time, stop_time, sample_time, read_type
+            tagname=tagname,
+            mapname=mapname,
+            start_time=start_time,
+            stop_time=stop_time,
+            sample_time=sample_time,
+            read_type=read_type,
+            metadata={},
         )
 
-        res = self.session.get(url, params=params)
-        res.raise_for_status()
+        res = self.fetch(url, params=params)
 
         if len(res.text) == 0:  # res.text='' for timestamps in future
             return pd.DataFrame(columns=[tag])
 
         try:
             j = res.json()
         except JSONDecodeError:
@@ -520,15 +554,18 @@
                 f'm="{max_rows}" to="30" s="1">'
             )
 
         connstr += f"<![CDATA[{query}]]></SQL>"
         return connstr
 
     def initialize_connectionstring(
-        self, host=None, port=10014, connection_string=None
+        self,
+        host: Optional[str] = None,
+        port: int = 10014,
+        connection_string: Optional[str] = None,
     ):
         if connection_string:
             self._connection_string = connection_string
         else:
             self._connection_string = (
                 f"DRIVER=AspenTech SQLPlus;HOST={host};"
                 f"PORT={port};CHARINT=N;CHARFLOAT=N;"
@@ -543,62 +580,60 @@
             )
         else:
             params = self.generate_sql_query(
                 connection_string=self._connection_string,
                 query=query,
                 max_rows=self._max_rows,
             )
-        res = self.session.get(url, params=params)
-        res.raise_for_status()
+        res = self.fetch(url, params=params)
         # For now just return result as text regardless of value of parse
         if parse:
             raise NotImplementedError(
                 "Use parse=False to receive and handle text result instead"
             )
         return res.text
 
 
-class PIHandlerWeb:
+class PIHandlerWeb(BaseHandlerWeb):
     def __init__(
         self,
-        url=None,
-        datasource=None,
-        auth=None,
-        verifySSL=None,
-        options={},
+        url: Optional[str] = None,
+        datasource: Optional[str] = None,
+        auth: Optional[Any] = None,
+        verifySSL: Optional[bool] = None,
+        options: Dict[str, Union[int, float, str]] = {},
     ):
-        self._max_rows = options.get("max_rows", 10000)
         if url is None:
             url = get_url_pi()
-        self.base_url = url
-        self.datasource = datasource
-        self.session = requests.Session()
-        self.session.auth = auth if auth is not None else get_auth_pi()
-        if verifySSL is False:
-            requests.packages.urllib3.disable_warnings(
-                requests.packages.urllib3.exceptions.InsecureRequestWarning
-            )
-        self.session.verify = verifySSL if verifySSL is not None else get_verifySSL()
+        if auth is None:
+            auth = get_auth_pi()
+        super().__init__(
+            url=url,
+            datasource=datasource,
+            auth=auth,
+            verifySSL=verifySSL,
+        )
+        self._max_rows = options.get("max_rows", 10000)
         self.webidcache = {}
 
     @staticmethod
-    def _time_to_UTC_string(time):
+    def _time_to_UTC_string(time: pd.Timestamp) -> str:
         timecast_format_query = "%d-%b-%y %H:%M:%S"
         if isinstance(time, datetime.datetime):
             return time.astimezone(pytz.UTC).strftime(timecast_format_query)
         else:
             return time.tz_convert("UTC").strftime(timecast_format_query)
 
     @staticmethod
     def generate_connection_string(host, *_, **__):
         raise NotImplementedError
 
     @staticmethod
-    def escape(s):
-        # https://techsupport.osisoft.com/Documentation/PI-Web-API/help/topics/search-queries.html  # noqa: E501
+    def escape(s: str) -> str:
+        # https://techsupport.osisoft.com/Documentation/PI-Web-API/help/topics/search-queries.html
         return s.translate(
             str.maketrans(
                 {
                     "+": r"\+",
                     "-": r"\-",
                     "&": r"\&",
                     "|": r"\|",
@@ -617,15 +652,19 @@
                     "\\": r"\\",
                     " ": r"\ ",
                 }
             )
         )
 
     @staticmethod
-    def generate_search_query(tag=None, desc=None, datasource=None):
+    def generate_search_query(
+        tag: Optional[str] = None,
+        desc: Optional[str] = None,
+        datasource: Optional[str] = None,
+    ) -> Dict[str, str]:
         q = []
         if tag is not None:
             q.extend([f"name:{PIHandlerWeb.escape(tag)}"])
         if desc is not None:
             q.extend([f"description:{PIHandlerWeb.escape(desc)}"])
         query = " AND ".join(q)
         params = {"q": f"{query}"}
@@ -633,22 +672,22 @@
         if datasource is not None:
             params["scope"] = f"pi:{datasource}"
 
         return params
 
     def generate_read_query(
         self,
-        tag,
-        start_time,
-        stop_time,
-        sample_time,
-        read_type,
-        metadata=None,
-        get_status=False,
-    ):
+        tag: str,
+        start_time: pd.Timestamp,
+        stop_time: pd.Timestamp,
+        sample_time: Optional[Union[int, pd.Timestamp]],
+        read_type: ReaderType,
+        metadata: Optional[Dict[str, str]] = None,
+        get_status: bool = False,
+    ) -> Tuple[str, Dict[str, str]]:
         if read_type in [
             ReaderType.COUNT,
             ReaderType.GOOD,
             ReaderType.BAD,
             ReaderType.TOTAL,
             ReaderType.SUM,
             ReaderType.SHAPEPRESERVING,
@@ -712,161 +751,159 @@
             params["selectedFields"] = "Timestamp;Value"
             if get_status:
                 params["selectedFields"] += ";Good;Questionable;Substituted"
 
         if read_type == ReaderType.RAW:
             params["maxCount"] = self._max_rows
 
-        return (url, params)
+        return url, params
 
-    def verify_connection(self, datasource):
+    def verify_connection(self, datasource: str) -> bool:
         """Connects to the URL and verifies that the provided data source exists.
 
-        :param source: Data source to look for
-        :type source: String
+        :param datasource: Data source to look for
+        :type datasource: String
         :raises ConnectionError: If connection fails
         :return: True if data source exists, False if not.
         :rtype: Bool
         """
         url = urljoin(self.base_url, "dataservers")
-        res = self.session.get(url)
-        res.raise_for_status()
+        res = self.fetch(url)
         j = res.json()
         for item in j["Items"]:
             if item["Name"] == datasource:
                 return True
         return False
 
-    def connect(self):
-        try:
-            self.verify_connection(self.datasource)
-        except requests.ConnectionError:
-            raise ConnectionError(
-                f"Not able to connect to {self.base_url}. Check network connection."
-            ) from None
-
-    def search(self, tag=None, desc=None):
-        params = self.generate_search_query(tag, desc, self.datasource)
+    def search(
+        self, tag: Optional[str] = None, desc: Optional[str] = None
+    ) -> List[Tuple]:
+        params = self.generate_search_query(
+            tag=tag, desc=desc, datasource=self.datasource
+        )
         url = urljoin(self.base_url, "search", "query")
         done = False
         ret = []
         while not done:
-            res = self.session.get(url, params=params)
+            res = self.fetch(url, params=params)
 
-            res.raise_for_status()
             j = res.json()
             for item in j["Items"]:
                 description = item["Description"] if "Description" in item else ""
                 ret.append((item["Name"], description))
             next_start = int(j["Links"]["Next"].split("=")[-1])
             if int(j["Links"]["Last"].split("=")[-1]) >= next_start:
                 params["start"] = next_start
             else:
                 done = True
         return ret
 
-    def _get_tag_metadata(self, tag):
+    def _get_tag_metadata(self, tag: str) -> Dict[str, str]:
         return {}  # FIXME
 
-    def _get_tag_unit(self, tag):
+    def _get_tag_unit(self, tag: str) -> Optional[str]:
         webid = self.tag_to_webid(tag)
         if webid is None:
             return None
         url = urljoin(self.base_url, "points", webid)
-        res = self.session.get(url)
-        res.raise_for_status()
+        res = self.fetch(url)
         j = res.json()
         unit = j["EngineeringUnits"]
         return unit
 
-    def _get_tag_description(self, tag):
+    def _get_tag_description(self, tag: str) -> Optional[str]:
         webid = self.tag_to_webid(tag)
         if webid is None:
             return None
         url = urljoin(self.base_url, "points", webid)
-        res = self.session.get(url)
-        res.raise_for_status()
+        res = self.fetch(url)
         j = res.json()
         description = j["Descriptor"]
         return description
 
-    def tag_to_webid(self, tag):
+    def tag_to_webid(self, tag: str) -> Optional[str]:
         """Given a tag, returns the WebId.
 
         :param tag: The tag
         :type tag: str
         :raises ConnectionError: If connection or query fails
         :return: WebId
         :rtype: str
         """
         if tag not in self.webidcache:
-            params = self.generate_search_query(tag=tag, datasource=self.datasource)
+            params = self.generate_search_query(
+                tag=tag, datasource=self.datasource, desc=None
+            )
             params["fields"] = "name;webid"
             url = urljoin(self.base_url, "search", "query")
-            res = self.session.get(url, params=params)
-            res.raise_for_status()
+            res = self.fetch(url, params=params)
             j = res.json()
 
             if len(j["Errors"]) > 0:
-                msg = f"Received error from server when searching for WebId for {tag}: {j['Errors']}"  # noqa: E501
+                msg = f"Received error from server when searching for WebId for {tag}: {j['Errors']}"
                 raise ValueError(msg)
 
             if len(j["Items"]) > 1:
                 # Compare elements and if same, return the first
                 first = j["Items"][0]
                 for item in j["Items"][1:]:
                     if item != first:
                         raise AssertionError(
-                            f"Received {len(j['Items'])} results when trying to find unique WebId for {tag}."  # noqa: E501
+                            f"Received {len(j['Items'])} results when trying to find unique WebId for {tag}."
                         )
             elif len(j["Items"]) == 0:
                 warnings.warn(f"Tag {tag} not found")
                 return None
 
             webid = j["Items"][0]["WebId"]
             self.webidcache[tag] = webid
         return self.webidcache[tag]
 
     @staticmethod
-    def _is_summary(read_type):
+    def _is_summary(read_type: ReaderType) -> bool:
         if read_type in [
             ReaderType.AVG,
             ReaderType.MIN,
             ReaderType.MAX,
             ReaderType.RNG,
             ReaderType.STD,
             ReaderType.VAR,
         ]:
             return True
         return False
 
     def read_tag(
         self,
-        tag,
-        start_time=None,
-        stop_time=None,
-        sample_time=None,
-        read_type=ReaderType.INTERPOLATED,
-        metadata=None,
-        get_status=False,
+        tag: str,
+        start_time: Optional[pd.Timestamp] = None,
+        stop_time: Optional[pd.Timestamp] = None,
+        sample_time: Optional[Union[int, pd.Timestamp]] = None,
+        read_type: ReaderType = ReaderType.INTERPOLATED,
+        metadata: Optional[Dict[str, str]] = None,
+        get_status: bool = False,
     ):
         webid = self.tag_to_webid(tag)
         if not webid:
             return pd.DataFrame()
 
         (url, params) = self.generate_read_query(
-            webid, start_time, stop_time, sample_time, read_type, get_status=get_status
+            tag=webid,
+            start_time=start_time,
+            stop_time=stop_time,
+            sample_time=sample_time,
+            read_type=read_type,
+            metadata={},
+            get_status=get_status,
         )
         url = urljoin(self.base_url, url)
-        res = self.session.get(url, params=params)
-        res.raise_for_status()
+        res = self.fetch(url, params=params)
 
         j = res.json()
         if read_type == ReaderType.SNAPSHOT:
-            df = pd.DataFrame.from_dict([j])
+            df = pd.DataFrame.from_dict([j])  # noqa
         else:
             # Summary (aggregated) data and DigitalSets return Value as dict
             df = pd.json_normalize(data=j, record_path="Items")
 
         # Can happen for RAW reads w/o data in interval
         if df.empty:
             return df
@@ -877,15 +914,15 @@
             if "Value.Name" in df.columns:
                 df.loc[df["Value.Name"] == "No Data", "Value.Value"] = np.nan
             # Replaced below replacement test with above when adding get_status
             # since we should avoid getting Good when get_status == False
             # Value.Name can also be the name of the digitalset, e.g. "Active"
             # Alternative: df["Value.IsSystem"] == True since it seems to be False
             # for digitalsets?
-            #    df.loc[df.Good == False, "Value.Value"] = np.nan  # noqa E712
+            #    df.loc[df.Good == False, "Value.Value"] = np.nan
             df = df.rename(
                 columns={
                     "Value.Value": "Value",
                     "Value.Timestamp": "Timestamp",
                     "Value.Good": "Good",
                     "Value.Questionable": "Questionable",
                     "Value.Substituted": "Substituted",
```

### Comparing `tagreader-4.0.1/PKG-INFO` & `tagreader-4.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tagreader
-Version: 4.0.1
+Version: 4.0.3
 Summary: Tagreader is a Python package for reading trend data from the OSIsoft PI and Aspen Infoplus.21 IMS systems.
 License: MIT
 Keywords: Aspen InfoPlus.21,OSIsoft PI
 Author: Einar S. Idsø
 Author-email: eiids@equinor.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,20 +23,23 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
-Requires-Dist: certifi (>=2023.5.7,<2024.0.0)
-Requires-Dist: pandas (>=2.0.1,<3.0.0)
-Requires-Dist: pyodbc (>=4.0.39,<5.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: requests-kerberos (>=0.14.0,<0.15.0)
-Requires-Dist: tables (>=3.8.0,<4.0.0)
+Provides-Extra: notebooks
+Requires-Dist: certifi (>=2023,<2024)
+Requires-Dist: jupyter (>=1,<2) ; extra == "notebooks"
+Requires-Dist: matplotlib (>=3,<4) ; extra == "notebooks"
+Requires-Dist: pandas (>=1)
+Requires-Dist: pyodbc (>=4,<5)
+Requires-Dist: requests (>=2,<3)
+Requires-Dist: requests-kerberos (>=0,<1)
+Requires-Dist: tables (>=3,<4) ; platform_machine != "arm64"
 Description-Content-Type: text/markdown
 
 # tagreader-python <!-- omit in toc -->
 
 ![GitHub Build Status](https://github.com/equinor/tagreader-python/workflows/Test/badge.svg)
 [![Devops Build Status](https://dev.azure.com/EIIDS/tagreader/_apis/build/status/equinor.tagreader-python?branchName=master)](https://dev.azure.com/EIIDS/tagreader/_build/latest?definitionId=5&branchName=master)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tagreader) 
@@ -95,17 +98,26 @@
 ```
 import tagreader
 c = tagreader.IMSClient("mysource", "aspenone")
 print(c.search("tag*"))
 df = c.read_tags(["tag1", "tag2"], "18.06.2020 08:00:00", "18.06.2020 09:00:00", 60)
 ```
 
+## Jupyter Notebook Quickstart
+Jupyter Notebook examples can be found in /examples. In order to run these examples, you need to install the optional
+dependencies.
+
+```bash
+pip install tagreader[notebooks]
+```
+
+
 ## Documentation
 
-There is a [quickstart](docs/quickstart.ipynb) example file that should get
+There is a [quickstart](examples/quickstart.ipynb) example file that should get
 you going. Also check out the [manual](docs/manual.md) for more information.
 
 ## Contributing
 
 All contributions are welcome, including code, bug reports, issues, feature
 requests, and documentation. The preferred way of submitting a contribution
 is to either create an issue on GitHub or to fork the project and make a pull
```

