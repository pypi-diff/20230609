# Comparing `tmp/pascal_voc-0.0.3.tar.gz` & `tmp/pascal_voc-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pascal_voc-0.0.3.tar", last modified: Wed Nov 24 13:47:56 2021, max compression
+gzip compressed data, was "pascal_voc-0.0.4.tar", last modified: Thu Jun  8 20:53:57 2023, max compression
```

## Comparing `pascal_voc-0.0.3.tar` & `pascal_voc-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0 alexander  (1000) alexander  (1000)        0 2021-11-24 13:47:56.258308 pascal_voc-0.0.3/
--rwxrwxrwx   0 alexander  (1000) alexander  (1000)     3006 2021-11-24 13:47:56.257984 pascal_voc-0.0.3/PKG-INFO
--rwxrwxrwx   0 alexander  (1000) alexander  (1000)     2642 2021-10-25 08:09:26.000000 pascal_voc-0.0.3/README.md
-drwxrwxrwx   0 alexander  (1000) alexander  (1000)        0 2021-11-24 13:47:56.255420 pascal_voc-0.0.3/pascal/
--rwxrwxrwx   0 alexander  (1000) alexander  (1000)       84 2021-10-25 07:47:22.000000 pascal_voc-0.0.3/pascal/__init__.py
--rwxrwxrwx   0 alexander  (1000) alexander  (1000)    14741 2021-10-27 13:19:31.000000 pascal_voc-0.0.3/pascal/main.py
-drwxrwxrwx   0 alexander  (1000) alexander  (1000)        0 2021-11-24 13:47:56.257528 pascal_voc-0.0.3/pascal_voc.egg-info/
--rwxrwxrwx   0 alexander  (1000) alexander  (1000)     3006 2021-11-24 13:47:56.000000 pascal_voc-0.0.3/pascal_voc.egg-info/PKG-INFO
--rwxrwxrwx   0 alexander  (1000) alexander  (1000)      221 2021-11-24 13:47:56.000000 pascal_voc-0.0.3/pascal_voc.egg-info/SOURCES.txt
--rwxrwxrwx   0 alexander  (1000) alexander  (1000)        1 2021-11-24 13:47:56.000000 pascal_voc-0.0.3/pascal_voc.egg-info/dependency_links.txt
--rwxrwxrwx   0 alexander  (1000) alexander  (1000)       26 2021-11-24 13:47:56.000000 pascal_voc-0.0.3/pascal_voc.egg-info/requires.txt
--rwxrwxrwx   0 alexander  (1000) alexander  (1000)        7 2021-11-24 13:47:56.000000 pascal_voc-0.0.3/pascal_voc.egg-info/top_level.txt
--rwxrwxrwx   0 alexander  (1000) alexander  (1000)       38 2021-11-24 13:47:56.258386 pascal_voc-0.0.3/setup.cfg
--rwxrwxrwx   0 alexander  (1000) alexander  (1000)      645 2021-11-24 13:47:28.000000 pascal_voc-0.0.3/setup.py
+drwxrwxrwx   0 alexander  (1000) alexander  (1000)        0 2023-06-08 20:53:57.665713 pascal_voc-0.0.4/
+-rwxrwxrwx   0 alexander  (1000) alexander  (1000)     3099 2023-06-08 20:53:57.665488 pascal_voc-0.0.4/PKG-INFO
+-rwxrwxrwx   0 alexander  (1000) alexander  (1000)     2642 2023-02-28 17:56:32.000000 pascal_voc-0.0.4/README.md
+drwxrwxrwx   0 alexander  (1000) alexander  (1000)        0 2023-06-08 20:53:57.662505 pascal_voc-0.0.4/pascal/
+-rwxrwxrwx   0 alexander  (1000) alexander  (1000)      111 2023-06-08 20:39:24.000000 pascal_voc-0.0.4/pascal/__init__.py
+-rwxrwxrwx   0 alexander  (1000) alexander  (1000)    16327 2023-06-08 20:39:24.000000 pascal_voc-0.0.4/pascal/main.py
+drwxrwxrwx   0 alexander  (1000) alexander  (1000)        0 2023-06-08 20:53:57.664961 pascal_voc-0.0.4/pascal_voc.egg-info/
+-rwxrwxrwx   0 alexander  (1000) alexander  (1000)     3099 2023-06-08 20:53:57.000000 pascal_voc-0.0.4/pascal_voc.egg-info/PKG-INFO
+-rwxrwxrwx   0 alexander  (1000) alexander  (1000)      236 2023-06-08 20:53:57.000000 pascal_voc-0.0.4/pascal_voc.egg-info/SOURCES.txt
+-rwxrwxrwx   0 alexander  (1000) alexander  (1000)        1 2023-06-08 20:53:57.000000 pascal_voc-0.0.4/pascal_voc.egg-info/dependency_links.txt
+-rwxrwxrwx   0 alexander  (1000) alexander  (1000)       26 2023-06-08 20:53:57.000000 pascal_voc-0.0.4/pascal_voc.egg-info/requires.txt
+-rwxrwxrwx   0 alexander  (1000) alexander  (1000)        7 2023-06-08 20:53:57.000000 pascal_voc-0.0.4/pascal_voc.egg-info/top_level.txt
+-rwxrwxrwx   0 alexander  (1000) alexander  (1000)      434 2023-06-08 20:52:50.000000 pascal_voc-0.0.4/pyproject.toml
+-rwxrwxrwx   0 alexander  (1000) alexander  (1000)       38 2023-06-08 20:53:57.665793 pascal_voc-0.0.4/setup.cfg
+-rwxrwxrwx   0 alexander  (1000) alexander  (1000)      625 2023-06-08 20:51:39.000000 pascal_voc-0.0.4/setup.py
```

### Comparing `pascal_voc-0.0.3/PKG-INFO` & `pascal_voc-0.0.4/pascal_voc.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
-Name: pascal_voc
-Version: 0.0.3
-Summary: Working with PascalVOC annotations
-Home-page: UNKNOWN
+Name: pascal-voc
+Version: 0.0.4
+Summary: Tool to work with annotation formats
 Author: Alexander Barmin
-Author-email: barmin1@mail.ru
+Author-email: Alexander Barmin <barmin1@mail.ru>
 License: MIT
-Platform: UNKNOWN
+Project-URL: Homepage, https://github.com/Alek-dr/PascalVOC
 Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 ### pascal
 
 Python utility to work with PascalVoc annotation format
@@ -109,9 +109,7 @@
 ```
 
 #### Installation
 
 ```
 python setup.py install
 ```
-
-
```

### Comparing `pascal_voc-0.0.3/README.md` & `pascal_voc-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pascal_voc-0.0.3/pascal/main.py` & `pascal_voc-0.0.4/pascal/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import base64
+import xml.etree.ElementTree as xml
 from collections import namedtuple
 from io import BytesIO
+from pathlib import Path
+from typing import List, Union
 
-import xml.etree.ElementTree as xml
 from lxml import etree
-from pathlib import Path
 from PIL import Image
-from typing import List, Union
 
 size_block = namedtuple("size", "width,height,depth")
 
 
 def _add_tab(str):
     """Add tab to each line"""
     lines = str.split("\n")
@@ -22,17 +22,19 @@
     pass
 
 
 class BndBox(namedtuple("BndBox", ["xmin", "ymin", "xmax", "ymax"])):
     __slots__ = ()
 
     def __str__(self):
-        return f"<bndbox>\n\t<xmin>{self.xmin}</xmin>\n" \
-               f"\t<ymin>{self.ymin}</ymin>\n\t<xmax>{self.xmax}" \
-               f"</xmax>\n\t<ymax>{self.ymax}</ymax>\n</bndbox>"
+        return (
+            f"<bndbox>\n\t<xmin>{self.xmin}</xmin>\n"
+            f"\t<ymin>{self.ymin}</ymin>\n\t<xmax>{self.xmax}"
+            f"</xmax>\n\t<ymax>{self.ymax}</ymax>\n</bndbox>"
+        )
 
     def to_xml(self):
         bndbox = xml.Element("bndbox")
         xmin = xml.Element("xmin")
         xmin.text = str(self.xmin)
         ymin = xml.Element("ymin")
         ymin.text = str(self.ymin)
@@ -44,20 +46,23 @@
         bndbox.append(ymin)
         bndbox.append(xmax)
         bndbox.append(ymax)
         return bndbox
 
 
 class PascalObject:
-
-    def __init__(self, name: str = str(),
-                 pose: str = "Unspecified",
-                 truncated: bool = False,
-                 difficult: bool = False,
-                 bndbox: BndBox = None, **kwargs):
+    def __init__(
+        self,
+        name: str = str(),
+        pose: str = "Unspecified",
+        truncated: bool = False,
+        difficult: bool = False,
+        bndbox: BndBox = None,
+        **kwargs,
+    ):
         self._name = name
         self._pose = pose
         self._truncated = truncated
         self._difficult = difficult
         self._bndbox = bndbox
         self.other_fields = kwargs
 
@@ -87,15 +92,16 @@
             self._truncated = truncated
         elif isinstance(truncated, str):
             self._truncated = False if truncated == "0" else True
         elif isinstance(truncated, int):
             self._truncated = False if truncated == 0 else True
         else:
             raise ParseException(
-                f"Cannot understand truncated field of type: {type(truncated)}. truncated one of type: bool. str, int")
+                f"Cannot understand truncated field of type: {type(truncated)}. truncated one of type: bool. str, int"
+            )
 
     @property
     def difficult(self):
         return self._difficult
 
     @difficult.setter
     def difficult(self, difficult: Union[bool, str, int]):
@@ -103,15 +109,16 @@
             self._truncated = difficult
         elif isinstance(difficult, str):
             self._truncated = False if difficult == "0" else True
         elif isinstance(difficult, int):
             self._truncated = False if difficult == 0 else True
         else:
             raise ParseException(
-                f"Cannot understand difficult field of type: {type(difficult)}. truncated one of type: bool. str, int")
+                f"Cannot understand difficult field of type: {type(difficult)}. truncated one of type: bool. str, int"
+            )
 
     @property
     def bndbox(self):
         return self._bndbox
 
     @bndbox.setter
     def bndbox(self, bnd_block: BndBox):
@@ -124,15 +131,22 @@
         truncated = f"<truncated>{truncated_value}</truncated>"
         difficult_value = "1" if self._difficult else "0"
         difficult = f"<difficult>{difficult_value}</difficult>"
         other_attributes = []
         for k, v in self.other_fields.items():
             line = f"<{k}>{v}</{k}>"
             other_attributes.append(line)
-        attributes = [name, pose, truncated, difficult, *other_attributes, str(self.bndbox)]
+        attributes = [
+            name,
+            pose,
+            truncated,
+            difficult,
+            *other_attributes,
+            str(self.bndbox),
+        ]
         s_attributes = list(map(_add_tab, attributes))
         s = "\n".join(s_attributes)
         h = f"<object>\n{s}\n</object>"
         return h
 
     def to_xml(self):
         obj = xml.Element("object")
@@ -164,22 +178,24 @@
 
     def remove_feature(self, fname: str):
         if self.other_fields.get(fname):
             del self.other_fields[fname]
 
 
 class PascalVOC:
-
-    def __init__(self, filename: Union[Path, str],
-                 size: size_block,
-                 objects: List[PascalObject] = None,
-                 path: Path = None,
-                 folder: str = None,
-                 segmented: int = 0,
-                 database: str = "Unknown"):
+    def __init__(
+        self,
+        filename: Union[Path, str],
+        size: size_block,
+        objects: List[PascalObject] = None,
+        path: Path = None,
+        folder: str = None,
+        segmented: int = 0,
+        database: str = "Unknown",
+    ):
         if isinstance(filename, Path):
             self.filename = filename.name
         else:
             self.filename = filename
         self.folder = folder
         self.path = path
         self.database = database
@@ -211,15 +227,15 @@
             else:
                 segmented = 0
             objects = doc.findall("object")
             objects_ = []
             for obj in objects:
                 obj_ = PascalObject()
                 for field in obj:
-                    if field.tag != 'bndbox':
+                    if field.tag != "bndbox":
                         if hasattr(obj_, field.tag):
                             setattr(obj_, field.tag, field.text)
                         else:
                             obj_.add_feature(field.tag, field.text)
                 box_tag = obj.find("bndbox")
                 xmin = int(box_tag.find("xmin").text)
                 ymin = int(box_tag.find("ymin").text)
@@ -228,40 +244,81 @@
                 obj_.bndbox = BndBox(xmin, ymin, xmax, ymax)
                 objects_.append(obj_)
         except IndexError as ex:
             raise ParseException(ex)
         return PascalVOC(filename, size, objects_, path, folder, segmented, database)
 
     @classmethod
+    def _parse_yolo(
+        cls, path: Union[Path, str], data: List[str], size: size_block, labels_map: dict
+    ):
+        if isinstance(path, str):
+            path = Path(path)
+        try:
+            filename = path.name
+            folder = None
+            database = str()
+            segmented = 0
+            objects_ = []
+            for line in data:
+                obj_ = PascalObject()
+                try:
+                    class_id, xc, yc, dx, dy = line.split()
+                except ValueError:
+                    continue
+                obj_.name = labels_map.get(int(class_id))
+                xc = float(xc) * size.width
+                yc = float(yc) * size.height
+                dx = (0.5 * float(dx)) * size.width
+                dy = (0.5 * float(dy)) * size.height
+                xmin = int(xc - dx)
+                xmax = int(xc + dx)
+                ymin = int(yc - dy)
+                ymax = int(yc + dy)
+                obj_.bndbox = BndBox(xmin, ymin, xmax, ymax)
+                objects_.append(obj_)
+        except IndexError as ex:
+            raise ParseException(ex)
+        return PascalVOC(filename, size, objects_, path, folder, segmented, database)
+
+    @classmethod
     def from_xml(cls, path: Union[Path, str]):
         """
         Read xml annotation file by path
         """
         doc = xml.parse(str(path))
         return PascalVOC._parse(doc)
 
     @classmethod
+    def from_yolo(cls, path: Union[Path, str], size: size_block, labels_map: dict):
+        with open(path, "r") as f:
+            data = f.readlines()
+        return PascalVOC._parse_yolo(path, data, size, labels_map)
+
+    @classmethod
     def from_bytes(cls, bdata):
         doc = etree.XML(bdata)
         return PascalVOC._parse(doc)
 
     def __str__(self):
-        head = f"\n\t<folder>{self.folder}</folder>" \
-               f"\n\t<filename>{self.filename}</filename>" \
-               f"\n\t<path>{str(self.path)}</path>" \
-               f"\n\t<source>" \
-               f"\n\t\t<database>{self.database}</database>" \
-               f"\n\t</source>\n" \
-               f"\t<size>" \
-               f"\n\t\t<width>{self.size.width}</width>" \
-               f"\n\t\t<height>{self.size.height}</height>" \
-               f"\n\t\t<depth>{self.size.depth}" \
-               f"</depth>" \
-               f"\n\t</size>" \
-               f"\n\t<segmented>{self.segmented}</segmented>\n"
+        head = (
+            f"\n\t<folder>{self.folder}</folder>"
+            f"\n\t<filename>{self.filename}</filename>"
+            f"\n\t<path>{str(self.path)}</path>"
+            f"\n\t<source>"
+            f"\n\t\t<database>{self.database}</database>"
+            f"\n\t</source>\n"
+            f"\t<size>"
+            f"\n\t\t<width>{self.size.width}</width>"
+            f"\n\t\t<height>{self.size.height}</height>"
+            f"\n\t\t<depth>{self.size.depth}"
+            f"</depth>"
+            f"\n\t</size>"
+            f"\n\t<segmented>{self.segmented}</segmented>\n"
+        )
         objects = "\n".join([str(obj) for obj in self.objects])
         objects = _add_tab(objects)
         s = f"<annotation>{head}{objects}\n</annotation>"
         return s
 
     def __iter__(self):
         self.n = 0
@@ -274,20 +331,23 @@
         if self.n < len(self):
             obj = self.objects[self.n]
             self.n += 1
             return obj
         else:
             raise StopIteration
 
-    def to_xml(self, drop_path: bool = False,
-               drop_folder: bool = False,
-               drop_source: bool = False,
-               drop_pose: bool = False,
-               drop_segmented: bool = False,
-               drop_truncated: bool = False) -> xml.Element:
+    def to_xml(
+        self,
+        drop_path: bool = False,
+        drop_folder: bool = False,
+        drop_source: bool = False,
+        drop_pose: bool = False,
+        drop_segmented: bool = False,
+        drop_truncated: bool = False,
+    ) -> xml.Element:
         root = xml.Element("annotation")
         if not drop_folder:
             folder = xml.Element("folder")
             folder.text = str(self.folder)
             root.append(folder)
         filename = xml.Element("filename")
         filename.text = self.filename
@@ -328,17 +388,17 @@
             root.append(obj_xml)
         return root
 
     @staticmethod
     def base64img(img, img_path) -> str:
         buffered = BytesIO()
         suffix = img_path.suffix
-        if suffix in ['.JPG', ".jpg", '.JPEG', '.jpeg']:
+        if suffix in [".JPG", ".jpg", ".JPEG", ".jpeg"]:
             format = "JPEG"
-        elif suffix in ['.PNG', ".png"]:
+        elif suffix in [".PNG", ".png"]:
             format = "PNG"
         else:
             format = "PNG"
         img.save(buffered, format=format)
         buffered.seek(0)
         img_byte = buffered.getvalue()
         encoded_string = base64.b64encode(img_byte).decode("utf-8")
@@ -357,35 +417,37 @@
         if save_img_data:
             img = Image.open(img_path)
             encoded_string = PascalVOC.base64img(img, img_path)
 
         shapes = []
         for obj in self.objects:
             label = obj.name
-            points = [[obj.bndbox.xmin, obj.bndbox.ymin],
-                      [obj.bndbox.xmax, obj.bndbox.ymin],
-                      [obj.bndbox.xmax, obj.bndbox.ymax],
-                      [obj.bndbox.xmin, obj.bndbox.ymax]]
+            points = [
+                [obj.bndbox.xmin, obj.bndbox.ymin],
+                [obj.bndbox.xmax, obj.bndbox.ymin],
+                [obj.bndbox.xmax, obj.bndbox.ymax],
+                [obj.bndbox.xmin, obj.bndbox.ymax],
+            ]
             shape = dict(
                 label=label,
                 points=points,
                 group_id=None,
                 shape_type="polygon",
-                flags={}
+                flags={},
             )
             shapes.append(shape)
 
         res = dict(
             version="4.5.6",
             flags={},
             shapes=shapes,
             imagePath=str(img_path),
             imageData=encoded_string,
             imageHeight=self.size.height,
-            imageWidth=self.size.width
+            imageWidth=self.size.width,
         )
         return res
 
     def to_yolo(self, labels_map: dict) -> str:
         objects = []
         for obj in self.objects:
             label = labels_map[obj.name]
@@ -397,34 +459,44 @@
             dy /= self.size.height
             x /= self.size.width
             y /= self.size.height
             s = f"{label} {x:.3f} {y:.3f} {dx:.3f} {dy:.3f}"
             objects.append(s)
         return "\n".join(objects)
 
-    def save(self, output: Union[Path, str],
-             drop_all=False,
-             drop_path: bool = False,
-             drop_folder: bool = False,
-             drop_source: bool = False,
-             drop_pose: bool = False,
-             drop_segmented: bool = False,
-             drop_truncated: bool = False) -> None:
+    def save(
+        self,
+        output: Union[Path, str],
+        drop_all=False,
+        drop_path: bool = False,
+        drop_folder: bool = False,
+        drop_source: bool = False,
+        drop_pose: bool = False,
+        drop_segmented: bool = False,
+        drop_truncated: bool = False,
+    ) -> None:
         """Save pascal annotation to xml file"""
         if drop_all:
-            drop_path = True,
-            drop_folder = True,
-            drop_source = True,
-            drop_pose = True,
-            drop_segmented = True,
+            drop_path = (True,)
+            drop_folder = (True,)
+            drop_source = (True,)
+            drop_pose = (True,)
+            drop_segmented = (True,)
             drop_truncated = True
-        doc = self.to_xml(drop_path, drop_folder, drop_source, drop_pose, drop_segmented, drop_truncated)
+        doc = self.to_xml(
+            drop_path,
+            drop_folder,
+            drop_source,
+            drop_pose,
+            drop_segmented,
+            drop_truncated,
+        )
         tree = xml.ElementTree(doc)
         with open(output, "w") as out:
-            tree.write(out, encoding='unicode', method='xml')
+            tree.write(out, encoding="unicode", method="xml")
 
     def add_object(self, obj: PascalObject) -> None:
         self.objects.append(obj)
 
     def add_feature(self, fname: str, fvalue):
         """Add feature <fname> with <fvalue> to each object"""
         for obj in self.objects:
```

### Comparing `pascal_voc-0.0.3/pascal_voc.egg-info/PKG-INFO` & `pascal_voc-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
-Name: pascal-voc
-Version: 0.0.3
-Summary: Working with PascalVOC annotations
-Home-page: UNKNOWN
+Name: pascal_voc
+Version: 0.0.4
+Summary: Tool to work with annotation formats
 Author: Alexander Barmin
-Author-email: barmin1@mail.ru
+Author-email: Alexander Barmin <barmin1@mail.ru>
 License: MIT
-Platform: UNKNOWN
+Project-URL: Homepage, https://github.com/Alek-dr/PascalVOC
 Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 ### pascal
 
 Python utility to work with PascalVoc annotation format
@@ -109,9 +109,7 @@
 ```
 
 #### Installation
 
 ```
 python setup.py install
 ```
-
-
```

### Comparing `pascal_voc-0.0.3/setup.py` & `pascal_voc-0.0.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="pascal_voc",
-    version="0.0.3",
+    version="0.0.4",
     author="Alexander Barmin",
     author_email="barmin1@mail.ru",
-    description="Working with PascalVOC annotations",
+    description="Tool to work with annotation formats",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
-    install_requires=["lxml>=4.6.2",
-                      "Pillow>=8.1.0"],
+    install_requires=["lxml>=4.6.2", "Pillow>=8.1.0"],
     license="MIT",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.6',
+    python_requires=">=3.6",
 )
```

