# Comparing `tmp/pascal_voc-0.0.5.tar.gz` & `tmp/pascal_voc-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pascal_voc-0.0.5.tar", last modified: Thu Jun  8 22:24:56 2023, max compression
+gzip compressed data, was "pascal_voc-0.0.6.tar", last modified: Thu Jun  8 22:50:00 2023, max compression
```

## Comparing `pascal_voc-0.0.5.tar` & `pascal_voc-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 alexander  (1000) alexander  (1000)        0 2023-06-08 22:24:56.862708 pascal_voc-0.0.5/
--rwxrwxrwx   0 alexander  (1000) alexander  (1000)     3152 2023-06-08 22:24:56.862476 pascal_voc-0.0.5/PKG-INFO
--rwxrwxrwx   0 alexander  (1000) alexander  (1000)     2694 2023-06-08 22:04:18.000000 pascal_voc-0.0.5/README.md
-drwxrwxrwx   0 alexander  (1000) alexander  (1000)        0 2023-06-08 22:24:56.859458 pascal_voc-0.0.5/pascal/
--rwxrwxrwx   0 alexander  (1000) alexander  (1000)      111 2023-06-08 20:39:24.000000 pascal_voc-0.0.5/pascal/__init__.py
--rwxrwxrwx   0 alexander  (1000) alexander  (1000)    16384 2023-06-08 22:22:44.000000 pascal_voc-0.0.5/pascal/main.py
-drwxrwxrwx   0 alexander  (1000) alexander  (1000)        0 2023-06-08 22:24:56.861941 pascal_voc-0.0.5/pascal_voc.egg-info/
--rwxrwxrwx   0 alexander  (1000) alexander  (1000)     3152 2023-06-08 22:24:56.000000 pascal_voc-0.0.5/pascal_voc.egg-info/PKG-INFO
--rwxrwxrwx   0 alexander  (1000) alexander  (1000)      236 2023-06-08 22:24:56.000000 pascal_voc-0.0.5/pascal_voc.egg-info/SOURCES.txt
--rwxrwxrwx   0 alexander  (1000) alexander  (1000)        1 2023-06-08 22:24:56.000000 pascal_voc-0.0.5/pascal_voc.egg-info/dependency_links.txt
--rwxrwxrwx   0 alexander  (1000) alexander  (1000)       26 2023-06-08 22:24:56.000000 pascal_voc-0.0.5/pascal_voc.egg-info/requires.txt
--rwxrwxrwx   0 alexander  (1000) alexander  (1000)        7 2023-06-08 22:24:56.000000 pascal_voc-0.0.5/pascal_voc.egg-info/top_level.txt
--rwxrwxrwx   0 alexander  (1000) alexander  (1000)      434 2023-06-08 22:24:39.000000 pascal_voc-0.0.5/pyproject.toml
--rwxrwxrwx   0 alexander  (1000) alexander  (1000)       38 2023-06-08 22:24:56.862794 pascal_voc-0.0.5/setup.cfg
--rwxrwxrwx   0 alexander  (1000) alexander  (1000)      625 2023-06-08 22:24:39.000000 pascal_voc-0.0.5/setup.py
+drwxrwxrwx   0 alexander  (1000) alexander  (1000)        0 2023-06-08 22:50:00.166118 pascal_voc-0.0.6/
+-rwxrwxrwx   0 alexander  (1000) alexander  (1000)     3152 2023-06-08 22:50:00.165875 pascal_voc-0.0.6/PKG-INFO
+-rwxrwxrwx   0 alexander  (1000) alexander  (1000)     2694 2023-06-08 22:04:18.000000 pascal_voc-0.0.6/README.md
+drwxrwxrwx   0 alexander  (1000) alexander  (1000)        0 2023-06-08 22:50:00.162810 pascal_voc-0.0.6/pascal/
+-rwxrwxrwx   0 alexander  (1000) alexander  (1000)      111 2023-06-08 20:39:24.000000 pascal_voc-0.0.6/pascal/__init__.py
+-rwxrwxrwx   0 alexander  (1000) alexander  (1000)    16736 2023-06-08 22:48:06.000000 pascal_voc-0.0.6/pascal/main.py
+drwxrwxrwx   0 alexander  (1000) alexander  (1000)        0 2023-06-08 22:50:00.165349 pascal_voc-0.0.6/pascal_voc.egg-info/
+-rwxrwxrwx   0 alexander  (1000) alexander  (1000)     3152 2023-06-08 22:50:00.000000 pascal_voc-0.0.6/pascal_voc.egg-info/PKG-INFO
+-rwxrwxrwx   0 alexander  (1000) alexander  (1000)      236 2023-06-08 22:50:00.000000 pascal_voc-0.0.6/pascal_voc.egg-info/SOURCES.txt
+-rwxrwxrwx   0 alexander  (1000) alexander  (1000)        1 2023-06-08 22:50:00.000000 pascal_voc-0.0.6/pascal_voc.egg-info/dependency_links.txt
+-rwxrwxrwx   0 alexander  (1000) alexander  (1000)       26 2023-06-08 22:50:00.000000 pascal_voc-0.0.6/pascal_voc.egg-info/requires.txt
+-rwxrwxrwx   0 alexander  (1000) alexander  (1000)        7 2023-06-08 22:50:00.000000 pascal_voc-0.0.6/pascal_voc.egg-info/top_level.txt
+-rwxrwxrwx   0 alexander  (1000) alexander  (1000)      434 2023-06-08 22:49:47.000000 pascal_voc-0.0.6/pyproject.toml
+-rwxrwxrwx   0 alexander  (1000) alexander  (1000)       38 2023-06-08 22:50:00.166193 pascal_voc-0.0.6/setup.cfg
+-rwxrwxrwx   0 alexander  (1000) alexander  (1000)      625 2023-06-08 22:49:42.000000 pascal_voc-0.0.6/setup.py
```

### Comparing `pascal_voc-0.0.5/PKG-INFO` & `pascal_voc-0.0.6/pascal_voc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pascal_voc
-Version: 0.0.5
+Name: pascal-voc
+Version: 0.0.6
 Summary: Tool to work with annotation formats
 Author: Alexander Barmin
 Author-email: Alexander Barmin <barmin1@mail.ru>
 License: MIT
 Project-URL: Homepage, https://github.com/Alek-dr/PascalVOC
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pascal_voc-0.0.5/README.md` & `pascal_voc-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pascal_voc-0.0.5/pascal/main.py` & `pascal_voc-0.0.6/pascal/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,21 +47,21 @@
         bndbox.append(xmax)
         bndbox.append(ymax)
         return bndbox
 
 
 class PascalObject:
     def __init__(
-        self,
-        name: str = str(),
-        pose: str = "Unspecified",
-        truncated: bool = False,
-        difficult: bool = False,
-        bndbox: BndBox = None,
-        **kwargs,
+            self,
+            name: str = str(),
+            pose: str = "Unspecified",
+            truncated: bool = False,
+            difficult: bool = False,
+            bndbox: BndBox = None,
+            **kwargs,
     ):
         self._name = name
         self._pose = pose
         self._truncated = truncated
         self._difficult = difficult
         self._bndbox = bndbox
         self.other_fields = kwargs
@@ -179,52 +179,61 @@
     def remove_feature(self, fname: str):
         if self.other_fields.get(fname):
             del self.other_fields[fname]
 
 
 class PascalVOC:
     def __init__(
-        self,
-        filename: Union[Path, str],
-        size: size_block,
-        objects: List[PascalObject] = None,
-        path: Path = None,
-        folder: str = None,
-        segmented: int = 0,
-        database: str = "Unknown",
+            self,
+            filename: Union[Path, str],
+            size: size_block,
+            objects: List[PascalObject] = None,
+            path: Path = None,
+            folder: str = None,
+            segmented: int = 0,
+            database: str = "Unknown",
     ):
         if isinstance(filename, Path):
             self.filename = filename.name
         else:
             self.filename = filename
         self.folder = folder
         self.path = path
         self.database = database
         self.size = size
         self.segmented = segmented
         self.objects = objects if objects is not None else []
 
+    @staticmethod
+    def _get_attribute(doc, attr_name, attr_type, default=None):
+        attr_ = doc.find(attr_name)
+        if attr_ is not None:
+            try:
+                val = attr_type(attr_.text)
+            except TypeError:
+                return default
+            else:
+                return val
+        return None
+
     @classmethod
     def _parse(cls, doc):
         try:
             filename = doc.find("filename").text
-            path_ = doc.find("path")
-            path = Path(path_.text) if path_ is not None else None
-            folder_ = doc.find("folder")
-            folder = folder_.text if folder_ is not None else None
+            path = PascalVOC._get_attribute(doc, "path", Path)
+            folder = PascalVOC._get_attribute(doc, "folder", str)
             source = doc.find("source")
             if source:
                 database = source.find("database").text
             else:
                 database = str()
             size_tag = doc.find("size")
             width = int(size_tag.find("width").text)
             height = int(size_tag.find("height").text)
-            depth_ = size_tag.find("depth")
-            depth = int(depth_.text) if depth_ is not None else 3
+            depth = PascalVOC._get_attribute(size_tag, "depth", int, default=3)
             size = size_block(width, height, depth)
             segmented_ = doc.find("segmented")
             if segmented_:
                 segmented = segmented_.text
             else:
                 segmented = 0
             objects = doc.findall("object")
@@ -246,15 +255,15 @@
                 objects_.append(obj_)
         except IndexError as ex:
             raise ParseException(ex)
         return PascalVOC(filename, size, objects_, path, folder, segmented, database)
 
     @classmethod
     def _parse_yolo(
-        cls, path: Union[Path, str], data: List[str], size: size_block, labels_map: dict
+            cls, path: Union[Path, str], data: List[str], size: size_block, labels_map: dict
     ):
         if isinstance(path, str):
             path = Path(path)
         try:
             filename = path.name
             folder = None
             database = str()
@@ -333,21 +342,21 @@
             obj = self.objects[self.n]
             self.n += 1
             return obj
         else:
             raise StopIteration
 
     def to_xml(
-        self,
-        drop_path: bool = False,
-        drop_folder: bool = False,
-        drop_source: bool = False,
-        drop_pose: bool = False,
-        drop_segmented: bool = False,
-        drop_truncated: bool = False,
+            self,
+            drop_path: bool = False,
+            drop_folder: bool = False,
+            drop_source: bool = False,
+            drop_pose: bool = False,
+            drop_segmented: bool = False,
+            drop_truncated: bool = False,
     ) -> xml.Element:
         root = xml.Element("annotation")
         if not drop_folder:
             folder = xml.Element("folder")
             folder.text = str(self.folder)
             root.append(folder)
         filename = xml.Element("filename")
@@ -461,23 +470,23 @@
             x /= self.size.width
             y /= self.size.height
             s = f"{label} {x:.3f} {y:.3f} {dx:.3f} {dy:.3f}"
             objects.append(s)
         return "\n".join(objects)
 
     def save(
-        self,
-        output: Union[Path, str],
-        drop_all=False,
-        drop_path: bool = False,
-        drop_folder: bool = False,
-        drop_source: bool = False,
-        drop_pose: bool = False,
-        drop_segmented: bool = False,
-        drop_truncated: bool = False,
+            self,
+            output: Union[Path, str],
+            drop_all=False,
+            drop_path: bool = False,
+            drop_folder: bool = False,
+            drop_source: bool = False,
+            drop_pose: bool = False,
+            drop_segmented: bool = False,
+            drop_truncated: bool = False,
     ) -> None:
         """Save pascal annotation to xml file"""
         if drop_all:
             drop_path = (True,)
             drop_folder = (True,)
             drop_source = (True,)
             drop_pose = (True,)
```

### Comparing `pascal_voc-0.0.5/pascal_voc.egg-info/PKG-INFO` & `pascal_voc-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pascal-voc
-Version: 0.0.5
+Name: pascal_voc
+Version: 0.0.6
 Summary: Tool to work with annotation formats
 Author: Alexander Barmin
 Author-email: Alexander Barmin <barmin1@mail.ru>
 License: MIT
 Project-URL: Homepage, https://github.com/Alek-dr/PascalVOC
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pascal_voc-0.0.5/setup.py` & `pascal_voc-0.0.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="pascal_voc",
-    version="0.0.5",
+    version="0.0.6",
     author="Alexander Barmin",
     author_email="barmin1@mail.ru",
     description="Tool to work with annotation formats",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     install_requires=["lxml>=4.6.2", "Pillow>=8.1.0"],
```

