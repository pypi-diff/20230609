# Comparing `tmp/morecantile-4.1.1.tar.gz` & `tmp/morecantile-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morecantile-4.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "morecantile-4.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `morecantile-4.1.1.tar` & `morecantile-4.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      215 2023-06-07 13:57:21.361458 morecantile-4.1.1/.bumpversion.cfg
--rw-r--r--   0        0        0     1817 2023-06-07 13:57:21.361458 morecantile-4.1.1/.gitignore
--rw-r--r--   0        0        0      822 2023-06-07 13:57:21.361458 morecantile-4.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1073 2023-06-07 13:57:21.361458 morecantile-4.1.1/LICENSE
--rw-r--r--   0        0        0     5305 2023-06-07 13:57:21.361458 morecantile-4.1.1/README.md
--rw-r--r--   0        0        0      436 2023-06-07 13:57:21.361458 morecantile-4.1.1/morecantile/__init__.py
--rw-r--r--   0        0        0     1015 2023-06-07 13:57:21.361458 morecantile-4.1.1/morecantile/commons.py
--rw-r--r--   0        0        0     7267 2023-06-07 13:57:21.361458 morecantile-4.1.1/morecantile/data/CanadianNAD83_LCC.json
--rw-r--r--   0        0        0     4679 2023-06-07 13:57:21.361458 morecantile-4.1.1/morecantile/data/EuropeanETRS89_LAEAQuad.json
--rw-r--r--   0        0        0     5176 2023-06-07 13:57:21.361458 morecantile-4.1.1/morecantile/data/LINZAntarticaMapTilegrid.json
--rw-r--r--   0        0        0     8457 2023-06-07 13:57:21.361458 morecantile-4.1.1/morecantile/data/NZTM2000Quad.json
--rw-r--r--   0        0        0      242 2023-06-07 13:57:21.361458 morecantile-4.1.1/morecantile/data/README.md
--rw-r--r--   0        0        0     7374 2023-06-07 13:57:21.361458 morecantile-4.1.1/morecantile/data/UPSAntarcticWGS84Quad.json
--rw-r--r--   0        0        0     7365 2023-06-07 13:57:21.361458 morecantile-4.1.1/morecantile/data/UPSArcticWGS84Quad.json
--rw-r--r--   0        0        0     7367 2023-06-07 13:57:21.361458 morecantile-4.1.1/morecantile/data/UTM31WGS84Quad.json
--rw-r--r--   0        0        0     6932 2023-06-07 13:57:21.361458 morecantile-4.1.1/morecantile/data/WGS1984Quad.json
--rw-r--r--   0        0        0     7843 2023-06-07 13:57:21.361458 morecantile-4.1.1/morecantile/data/WebMercatorQuad.json
--rw-r--r--   0        0        0     7072 2023-06-07 13:57:21.361458 morecantile-4.1.1/morecantile/data/WorldCRS84Quad.json
--rw-r--r--   0        0        0     7001 2023-06-07 13:57:21.361458 morecantile-4.1.1/morecantile/data/WorldMercatorWGS84Quad.json
--rw-r--r--   0        0        0     1748 2023-06-07 13:57:21.361458 morecantile-4.1.1/morecantile/defaults.py
--rw-r--r--   0        0        0      907 2023-06-07 13:57:21.365458 morecantile-4.1.1/morecantile/errors.py
--rw-r--r--   0        0        0    41387 2023-06-07 13:57:21.365458 morecantile-4.1.1/morecantile/models.py
--rw-r--r--   0        0        0        0 2023-06-07 13:57:21.365458 morecantile-4.1.1/morecantile/py.typed
--rw-r--r--   0        0        0       23 2023-06-07 13:57:21.365458 morecantile-4.1.1/morecantile/scripts/__init__.py
--rw-r--r--   0        0        0    16657 2023-06-07 13:57:21.365458 morecantile-4.1.1/morecantile/scripts/cli.py
--rw-r--r--   0        0        0     3364 2023-06-07 13:57:21.365458 morecantile-4.1.1/morecantile/utils.py
--rw-r--r--   0        0        0     2295 2023-06-07 13:57:21.365458 morecantile-4.1.1/pyproject.toml
--rw-r--r--   0        0        0     6732 1970-01-01 00:00:00.000000 morecantile-4.1.1/PKG-INFO
+-rw-r--r--   0        0        0      215 2023-06-09 09:16:46.762144 morecantile-4.2.0/.bumpversion.cfg
+-rw-r--r--   0        0        0     1817 2023-06-09 09:16:46.762144 morecantile-4.2.0/.gitignore
+-rw-r--r--   0        0        0      822 2023-06-09 09:16:46.762144 morecantile-4.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1073 2023-06-09 09:16:46.762144 morecantile-4.2.0/LICENSE
+-rw-r--r--   0        0        0     5305 2023-06-09 09:16:46.762144 morecantile-4.2.0/README.md
+-rw-r--r--   0        0        0      436 2023-06-09 09:16:46.766144 morecantile-4.2.0/morecantile/__init__.py
+-rw-r--r--   0        0        0     1015 2023-06-09 09:16:46.766144 morecantile-4.2.0/morecantile/commons.py
+-rw-r--r--   0        0        0     7267 2023-06-09 09:16:46.766144 morecantile-4.2.0/morecantile/data/CanadianNAD83_LCC.json
+-rw-r--r--   0        0        0     4679 2023-06-09 09:16:46.766144 morecantile-4.2.0/morecantile/data/EuropeanETRS89_LAEAQuad.json
+-rw-r--r--   0        0        0     5176 2023-06-09 09:16:46.766144 morecantile-4.2.0/morecantile/data/LINZAntarticaMapTilegrid.json
+-rw-r--r--   0        0        0     8457 2023-06-09 09:16:46.766144 morecantile-4.2.0/morecantile/data/NZTM2000Quad.json
+-rw-r--r--   0        0        0      242 2023-06-09 09:16:46.766144 morecantile-4.2.0/morecantile/data/README.md
+-rw-r--r--   0        0        0     7374 2023-06-09 09:16:46.766144 morecantile-4.2.0/morecantile/data/UPSAntarcticWGS84Quad.json
+-rw-r--r--   0        0        0     7365 2023-06-09 09:16:46.766144 morecantile-4.2.0/morecantile/data/UPSArcticWGS84Quad.json
+-rw-r--r--   0        0        0     7367 2023-06-09 09:16:46.766144 morecantile-4.2.0/morecantile/data/UTM31WGS84Quad.json
+-rw-r--r--   0        0        0     6932 2023-06-09 09:16:46.766144 morecantile-4.2.0/morecantile/data/WGS1984Quad.json
+-rw-r--r--   0        0        0     7843 2023-06-09 09:16:46.766144 morecantile-4.2.0/morecantile/data/WebMercatorQuad.json
+-rw-r--r--   0        0        0     7072 2023-06-09 09:16:46.766144 morecantile-4.2.0/morecantile/data/WorldCRS84Quad.json
+-rw-r--r--   0        0        0     7001 2023-06-09 09:16:46.766144 morecantile-4.2.0/morecantile/data/WorldMercatorWGS84Quad.json
+-rw-r--r--   0        0        0     1748 2023-06-09 09:16:46.766144 morecantile-4.2.0/morecantile/defaults.py
+-rw-r--r--   0        0        0      907 2023-06-09 09:16:46.766144 morecantile-4.2.0/morecantile/errors.py
+-rw-r--r--   0        0        0    41795 2023-06-09 09:16:46.766144 morecantile-4.2.0/morecantile/models.py
+-rw-r--r--   0        0        0        0 2023-06-09 09:16:46.766144 morecantile-4.2.0/morecantile/py.typed
+-rw-r--r--   0        0        0       23 2023-06-09 09:16:46.766144 morecantile-4.2.0/morecantile/scripts/__init__.py
+-rw-r--r--   0        0        0    16657 2023-06-09 09:16:46.766144 morecantile-4.2.0/morecantile/scripts/cli.py
+-rw-r--r--   0        0        0     3364 2023-06-09 09:16:46.766144 morecantile-4.2.0/morecantile/utils.py
+-rw-r--r--   0        0        0     2295 2023-06-09 09:16:46.766144 morecantile-4.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6732 1970-01-01 00:00:00.000000 morecantile-4.2.0/PKG-INFO
```

### Comparing `morecantile-4.1.1/.gitignore` & `morecantile-4.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `morecantile-4.1.1/.pre-commit-config.yaml` & `morecantile-4.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `morecantile-4.1.1/LICENSE` & `morecantile-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `morecantile-4.1.1/README.md` & `morecantile-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `morecantile-4.1.1/morecantile/commons.py` & `morecantile-4.2.0/morecantile/commons.py`

 * *Files identical despite different names*

### Comparing `morecantile-4.1.1/morecantile/data/CanadianNAD83_LCC.json` & `morecantile-4.2.0/morecantile/data/CanadianNAD83_LCC.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.1.1/morecantile/data/EuropeanETRS89_LAEAQuad.json` & `morecantile-4.2.0/morecantile/data/EuropeanETRS89_LAEAQuad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.1.1/morecantile/data/LINZAntarticaMapTilegrid.json` & `morecantile-4.2.0/morecantile/data/LINZAntarticaMapTilegrid.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.1.1/morecantile/data/NZTM2000Quad.json` & `morecantile-4.2.0/morecantile/data/NZTM2000Quad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.1.1/morecantile/data/UPSAntarcticWGS84Quad.json` & `morecantile-4.2.0/morecantile/data/UPSAntarcticWGS84Quad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.1.1/morecantile/data/UPSArcticWGS84Quad.json` & `morecantile-4.2.0/morecantile/data/UPSArcticWGS84Quad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.1.1/morecantile/data/UTM31WGS84Quad.json` & `morecantile-4.2.0/morecantile/data/UTM31WGS84Quad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.1.1/morecantile/data/WGS1984Quad.json` & `morecantile-4.2.0/morecantile/data/WGS1984Quad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.1.1/morecantile/data/WebMercatorQuad.json` & `morecantile-4.2.0/morecantile/data/WebMercatorQuad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.1.1/morecantile/data/WorldCRS84Quad.json` & `morecantile-4.2.0/morecantile/data/WorldCRS84Quad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.1.1/morecantile/data/WorldMercatorWGS84Quad.json` & `morecantile-4.2.0/morecantile/data/WorldMercatorWGS84Quad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.1.1/morecantile/defaults.py` & `morecantile-4.2.0/morecantile/defaults.py`

 * *Files identical despite different names*

### Comparing `morecantile-4.1.1/morecantile/errors.py` & `morecantile-4.2.0/morecantile/errors.py`

 * *Files identical despite different names*

### Comparing `morecantile-4.1.1/morecantile/models.py` & `morecantile-4.2.0/morecantile/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,26 +104,36 @@
     __root__: Union[str, Union[CRSUri, CRSWKT]] = Field(..., title="CRS")
     _pyproj_crs: CRS = PrivateAttr()
 
     def __init__(self, **data):
         """Custom Init to validate CRS string and create Pyproj CRS object."""
         super().__init__(**data)
 
-        _pyproj_crs = CRS.from_user_input(data.get("__root__"))
-
-        self._pyproj_crs = _pyproj_crs
+        self._pyproj_crs = CRS.from_user_input(data.get("__root__"))
 
     def to_epsg(self) -> Optional[int]:
         """return EPSG number of the CRS."""
         return self._pyproj_crs.to_epsg()
 
     def to_wkt(self) -> str:
         """return WKT version of the CRS."""
         return self._pyproj_crs.to_wkt()
 
+    def to_proj4(self) -> str:
+        """return PROJ4 version of the CRS."""
+        return self._pyproj_crs.to_proj4()
+
+    def to_dict(self) -> Dict:
+        """return DICT version of the CRS."""
+        return self._pyproj_crs.to_dict()
+
+    def to_json(self) -> str:
+        """return JSON version of the CRS."""
+        return self._pyproj_crs.to_json()
+
 
 def CRS_to_uri(crs: CRS) -> str:
     """Convert CRS to URI."""
     authority = "EPSG"
     code = None
     version = "0"
     # attempt to grab the authority, version, and code from the CRS
@@ -282,15 +292,14 @@
     )
     tileMatrices: List[TileMatrix] = Field(
         ..., description="Describes scale levels and its tile matrices"
     )
 
     # Private attributes
     _is_quadtree: bool = PrivateAttr()
-    _crs: CRS = PrivateAttr()
     _geographic_crs: CRS = PrivateAttr(default=WGS84_CRS)
     _to_geographic: Transformer = PrivateAttr()
     _from_geographic: Transformer = PrivateAttr()
 
     class Config:
         """Configure TileMatrixSet."""
 
@@ -302,23 +311,22 @@
             raise DeprecationError(
                 "Tile Matrix Set must be version 2.0. Use morecantile <4.0 for TMS 1.0 support"
             )
 
         super().__init__(**data)
 
         self._is_quadtree = check_quadkey_support(self.tileMatrices)
-        self._crs = CRS.from_user_input(self.crs.__root__)
         self._geographic_crs = data.get("_geographic_crs", WGS84_CRS)
 
         try:
             self._to_geographic = Transformer.from_crs(
-                self._crs, self._geographic_crs, always_xy=True
+                self.crs._pyproj_crs, self._geographic_crs, always_xy=True
             )
             self._from_geographic = Transformer.from_crs(
-                self._geographic_crs, self._crs, always_xy=True
+                self._geographic_crs, self.crs._pyproj_crs, always_xy=True
             )
         except ProjError:
             warnings.warn(
                 "Could not create coordinate Transformer from input CRS to the given geographic CRS"
                 "some methods might not be available.",
                 UserWarning,
             )
@@ -333,25 +341,25 @@
     def __iter__(self):
         """Iterate over matrices"""
         for matrix in self.tileMatrices:
             yield matrix
 
     def __repr__(self):
         """Simplify default pydantic model repr."""
-        return f"<TileMatrixSet title='{self.title}' id='{self.id}' crs='{self._crs}>"
+        return f"<TileMatrixSet title='{self.title}' id='{self.id}' crs='{self.crs.__root__}>"
 
     @property
     def geographic_crs(self) -> CRSType:
         """Return the TMS's geographic CRS."""
         return self._geographic_crs
 
     @property
     def rasterio_crs(self):
         """Return rasterio CRS."""
-        return to_rasterio_crs(self._crs)
+        return to_rasterio_crs(self.crs._pyproj_crs)
 
     @property
     def rasterio_geographic_crs(self):
         """Return the geographic CRS as a rasterio CRS."""
         return to_rasterio_crs(self._geographic_crs)
 
     @property
@@ -366,15 +374,15 @@
 
     @property
     def _invert_axis(self) -> bool:
         """Check if CRS has inverted AXIS (lat,lon) instead of (lon,lat)."""
         return (
             ordered_axis_inverted(self.orderedAxes)
             if self.orderedAxes
-            else crs_axis_inverted(self._crs)
+            else crs_axis_inverted(self.crs._pyproj_crs)
         )
 
     @classmethod
     def from_v1(cls, tms: Dict) -> "TileMatrixSet":
         """
         Makes a TMS from a v1 TMS definition
 
@@ -594,15 +602,15 @@
         Tile resolution for a TileMatrix.
 
         From note g in http://docs.opengeospatial.org/is/17-083r2/17-083r2.html#table_2:
           The pixel size of the tile can be obtained from the scaleDenominator
           by multiplying the later by 0.28 10-3 / metersPerUnit.
 
         """
-        return matrix.scaleDenominator * 0.28e-3 / meters_per_unit(self._crs)
+        return matrix.scaleDenominator * 0.28e-3 / meters_per_unit(self.crs._pyproj_crs)
 
     def zoom_for_res(
         self,
         res: float,
         max_z: Optional[int] = None,
         zoom_level_strategy: str = "auto",
         min_z: Optional[int] = None,
@@ -1052,15 +1060,20 @@
         if projected:
             warnings.warn(
                 "CRS is no longer part of the GeoJSON specification."
                 "Other projection than EPSG:4326 might not be supported.",
                 UserWarning,
             )
             feat.update(
-                {"crs": {"type": "EPSG", "properties": {"code": self._crs.to_epsg()}}}
+                {
+                    "crs": {
+                        "type": "EPSG",
+                        "properties": {"code": self.crs.to_epsg()},
+                    }
+                }
             )
 
         if props:
             feat["properties"].update(props)
 
         if fid is not None:
             feat["id"] = fid
```

### Comparing `morecantile-4.1.1/morecantile/scripts/cli.py` & `morecantile-4.2.0/morecantile/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `morecantile-4.1.1/morecantile/utils.py` & `morecantile-4.2.0/morecantile/utils.py`

 * *Files identical despite different names*

### Comparing `morecantile-4.1.1/pyproject.toml` & `morecantile-4.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `morecantile-4.1.1/PKG-INFO` & `morecantile-4.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morecantile
-Version: 4.1.1
+Version: 4.2.0
 Summary: Construct and use map tile grids (a.k.a TileMatrixSet / TMS).
 Keywords: GIS,TMS,TileMatrixSet,Map Tile
 Author-email: Vincent Sarago <vincent@developmentseed.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: morecantile Version: 4.1.1 Summary: Construct and
+Metadata-Version: 2.1 Name: morecantile Version: 4.2.0 Summary: Construct and
 use map tile grids (a.k.a TileMatrixSet / TMS). Keywords:
 GIS,TMS,TileMatrixSet,Map Tile Author-email: Vincent Sarago
 developmentseed.com> Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 BSD License Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

