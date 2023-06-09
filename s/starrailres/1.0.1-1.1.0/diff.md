# Comparing `tmp/starrailres-1.0.1.tar.gz` & `tmp/starrailres-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starrailres-1.0.1.tar", max compression
+gzip compressed data, was "starrailres-1.1.0.tar", max compression
```

## Comparing `starrailres-1.0.1.tar` & `starrailres-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0     1083 2023-05-23 12:01:47.249793 starrailres-1.0.1/LICENSE
--rw-r--r--   0        0        0      499 2023-05-31 13:17:20.467326 starrailres-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      924 2023-05-31 11:58:49.998393 starrailres-1.0.1/README.md
--rw-r--r--   0        0        0       22 2023-05-29 15:05:23.416606 starrailres-1.0.1/starrailres/__init__.py
--rw-r--r--   0        0        0    28999 2023-05-31 13:16:18.774488 starrailres-1.0.1/starrailres/index.py
--rw-r--r--   0        0        0      216 2023-05-31 13:14:58.577684 starrailres-1.0.1/starrailres/models/avatars.py
--rw-r--r--   0        0        0     1723 2023-05-29 05:55:48.065843 starrailres-1.0.1/starrailres/models/characters.py
--rw-r--r--   0        0        0      210 2023-05-26 14:44:56.999166 starrailres-1.0.1/starrailres/models/common.py
--rw-r--r--   0        0        0      245 2023-05-25 07:04:39.480460 starrailres-1.0.1/starrailres/models/descriptions.py
--rw-r--r--   0        0        0      295 2023-05-23 14:27:36.388191 starrailres-1.0.1/starrailres/models/elements.py
--rw-r--r--   0        0        0     3265 2023-05-31 13:16:18.582411 starrailres-1.0.1/starrailres/models/info.py
--rw-r--r--   0        0        0      352 2023-05-25 07:16:41.407713 starrailres-1.0.1/starrailres/models/items.py
--rw-r--r--   0        0        0      734 2023-05-29 13:34:04.145217 starrailres-1.0.1/starrailres/models/light_cones.py
--rw-r--r--   0        0        0      269 2023-05-23 14:27:09.523569 starrailres-1.0.1/starrailres/models/paths.py
--rw-r--r--   0        0        0      429 2023-05-29 14:28:24.391190 starrailres-1.0.1/starrailres/models/properties.py
--rw-r--r--   0        0        0      993 2023-05-30 04:32:44.019242 starrailres-1.0.1/starrailres/models/relics.py
--rw-r--r--   0        0        0        0 2023-05-25 07:11:50.015616 starrailres-1.0.1/starrailres/starrailres.py
--rw-r--r--   0        0        0      323 2023-05-25 07:32:33.386416 starrailres-1.0.1/starrailres/utils.py
--rw-r--r--   0        0        0     1573 1970-01-01 00:00:00.000000 starrailres-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-05-23 12:01:47.249793 starrailres-1.1.0/LICENSE
+-rw-r--r--   0        0        0      499 2023-06-09 09:36:07.597528 starrailres-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      924 2023-05-31 11:58:49.998393 starrailres-1.1.0/README.md
+-rw-r--r--   0        0        0       22 2023-05-29 15:05:23.416606 starrailres-1.1.0/starrailres/__init__.py
+-rw-r--r--   0        0        0    29302 2023-06-09 09:19:54.028504 starrailres-1.1.0/starrailres/index.py
+-rw-r--r--   0        0        0      216 2023-05-31 13:14:58.577684 starrailres-1.1.0/starrailres/models/avatars.py
+-rw-r--r--   0        0        0     1723 2023-05-29 05:55:48.065843 starrailres-1.1.0/starrailres/models/characters.py
+-rw-r--r--   0        0        0      210 2023-05-26 14:44:56.999166 starrailres-1.1.0/starrailres/models/common.py
+-rw-r--r--   0        0        0      245 2023-05-25 07:04:39.480460 starrailres-1.1.0/starrailres/models/descriptions.py
+-rw-r--r--   0        0        0      295 2023-05-23 14:27:36.388191 starrailres-1.1.0/starrailres/models/elements.py
+-rw-r--r--   0        0        0     2774 2023-06-09 09:28:24.494447 starrailres-1.1.0/starrailres/models/info.py
+-rw-r--r--   0        0        0      352 2023-05-25 07:16:41.407713 starrailres-1.1.0/starrailres/models/items.py
+-rw-r--r--   0        0        0      734 2023-05-29 13:34:04.145217 starrailres-1.1.0/starrailres/models/light_cones.py
+-rw-r--r--   0        0        0      269 2023-05-23 14:27:09.523569 starrailres-1.1.0/starrailres/models/paths.py
+-rw-r--r--   0        0        0      429 2023-05-29 14:28:24.391190 starrailres-1.1.0/starrailres/models/properties.py
+-rw-r--r--   0        0        0      993 2023-05-30 04:32:44.019242 starrailres-1.1.0/starrailres/models/relics.py
+-rw-r--r--   0        0        0      323 2023-05-25 07:32:33.386416 starrailres-1.1.0/starrailres/utils.py
+-rw-r--r--   0        0        0     1573 1970-01-01 00:00:00.000000 starrailres-1.1.0/PKG-INFO
```

### Comparing `starrailres-1.0.1/LICENSE` & `starrailres-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `starrailres-1.0.1/README.md` & `starrailres-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `starrailres-1.0.1/starrailres/index.py` & `starrailres-1.1.0/starrailres/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,14 +141,17 @@
             level=basic.level,
             promotion=basic.promotion,
             name=self.characters[basic.id].name,
             rarity=self.characters[basic.id].rarity,
             icon=self.characters[basic.id].icon,
             preview=self.characters[basic.id].preview,
             portrait=self.characters[basic.id].portrait,
+            rank_icons=[
+                self.character_ranks[i].icon for i in self.characters[basic.id].ranks
+            ],
             path=self.get_path_info(self.characters[basic.id].path),
             element=self.get_element_info(self.characters[basic.id].element),
             skills=self.get_character_skill_info(
                 basic.id,
                 self.merge_character_skill_upgrade(
                     [
                         self.get_character_skill_upgrade_from_rank(
@@ -270,14 +273,16 @@
         relic_sets = []
         for k, v in set_num.items():
             if v >= 2:
                 relic_sets.append(
                     RelicSetInfo(
                         id=k,
                         name=self.relic_sets[k].name,
+                        icon=self.relic_sets[k].icon,
+                        num=2,
                         desc=self.relic_sets[k].desc[0],
                         properties=[
                             PropertyInfo(
                                 type=i.type,
                                 field=self.properties[i.type].field,
                                 name=self.properties[i.type].name,
                                 icon=self.properties[i.type].icon,
@@ -293,14 +298,16 @@
                     )
                 )
             if v >= 4:
                 relic_sets.append(
                     RelicSetInfo(
                         id=k,
                         name=self.relic_sets[k].name,
+                        icon=self.relic_sets[k].icon,
+                        num=4,
                         desc=self.relic_sets[k].desc[0],
                         properties=[
                             PropertyInfo(
                                 type=i.type,
                                 field=self.properties[i.type].field,
                                 name=self.properties[i.type].name,
                                 icon=self.properties[i.type].icon,
```

### Comparing `starrailres-1.0.1/starrailres/models/characters.py` & `starrailres-1.1.0/starrailres/models/characters.py`

 * *Files identical despite different names*

### Comparing `starrailres-1.0.1/starrailres/models/info.py` & `starrailres-1.1.0/starrailres/models/info.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,160 +1,147 @@
 from typing import List, Optional
 
 from msgspec import Struct
 
 
-class BaseInfo(Struct):
-    def to_dict(self):
-        result = {}
-        for field in self.__struct_fields__:
-            value = getattr(self, field)
-            if isinstance(value, BaseInfo):
-                result[field] = value.to_dict()
-            elif isinstance(value, list) and all(
-                isinstance(i, BaseInfo) for i in value
-            ):
-                result[field] = [i.to_dict() for i in value]
-            else:
-                result[field] = value
-        return result
-
-
-class LevelInfo(BaseInfo):
+class LevelInfo(Struct):
     id: str
     level: int = 0
 
 
-class AvatarInfo(BaseInfo):
+class AvatarInfo(Struct):
     id: str
     name: str
     icon: str
 
 
-class PathInfo(BaseInfo):
+class PathInfo(Struct):
     id: str
     name: str
     icon: str
 
 
-class ElementInfo(BaseInfo):
+class ElementInfo(Struct):
     id: str
     name: str
     color: str
     icon: str
 
 
-class SkillInfo(BaseInfo):
+class SkillInfo(Struct):
     id: str
     name: str
     level: int
     max_level: int
     element: Optional[ElementInfo]
     type: str
     type_text: str
     effect: str
     effect_text: str
     simple_desc: str
     desc: str
     icon: str
 
 
-class PropertyInfo(BaseInfo):
+class PropertyInfo(Struct):
     type: str
     field: str
     name: str
     icon: str
     value: float
     display: str
     percent: bool
 
 
-class AttributeInfo(BaseInfo):
+class AttributeInfo(Struct):
     field: str
     name: str
     icon: str
     value: float
     display: str
     percent: bool
 
 
-class SubAffixInfo(BaseInfo):
+class SubAffixInfo(Struct):
     id: str
     cnt: int
     step: int = 0
 
 
-class RelicBasicInfo(BaseInfo):
+class RelicBasicInfo(Struct):
     id: str
     level: int = 1
     main_affix_id: Optional[str] = None
     sub_affix_info: List[SubAffixInfo] = []
 
 
-class LightConeBasicInfo(BaseInfo):
+class LightConeBasicInfo(Struct):
     id: str
     rank: int = 1
     level: int = 1
     promotion: int = 0
 
 
-class CharacterBasicInfo(BaseInfo):
+class CharacterBasicInfo(Struct):
     id: str
     rank: int = 0
     level: int = 1
     promotion: int = 0
     skill_tree_levels: List[LevelInfo] = []
     light_cone: Optional[LightConeBasicInfo] = None
     relics: Optional[List[RelicBasicInfo]] = None
 
 
-class RelicInfo(BaseInfo):
+class RelicInfo(Struct):
     id: str
     name: str
     set_id: str
     set_name: str
     rarity: int
     level: int
     icon: str
     main_affix: Optional[PropertyInfo] = None
     sub_affix: List[PropertyInfo] = []
 
 
-class RelicSetInfo(BaseInfo):
+class RelicSetInfo(Struct):
     id: str
     name: str
+    icon: str
+    num: int
     desc: str = ""
     properties: List[PropertyInfo] = []
 
 
-class LightConeInfo(BaseInfo):
+class LightConeInfo(Struct):
     id: str
     name: str
     rarity: int
     rank: int
     level: int
     promotion: int
     icon: str
     preview: str
     portrait: str
     path: Optional[PathInfo] = None
     attributes: List[AttributeInfo] = []
     properties: List[PropertyInfo] = []
 
 
-class CharacterInfo(BaseInfo):
+class CharacterInfo(Struct):
     id: str
     name: str
     rarity: int
     rank: int
     level: int
     promotion: int
     icon: str
     preview: str
     portrait: str
+    rank_icons: List[str] = []
     path: Optional[PathInfo] = None
     element: Optional[ElementInfo] = None
     skills: List[SkillInfo] = []
     light_cone: Optional[LightConeInfo] = None
     relics: List[RelicInfo] = []
     relic_sets: List[RelicSetInfo] = []
     attributes: List[AttributeInfo] = []
```

### Comparing `starrailres-1.0.1/starrailres/models/light_cones.py` & `starrailres-1.1.0/starrailres/models/light_cones.py`

 * *Files identical despite different names*

### Comparing `starrailres-1.0.1/starrailres/models/relics.py` & `starrailres-1.1.0/starrailres/models/relics.py`

 * *Files identical despite different names*

### Comparing `starrailres-1.0.1/PKG-INFO` & `starrailres-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrailres
-Version: 1.0.1
+Version: 1.1.0
 Summary: StarRailRes index package.
 Home-page: https://github.com/Mar-7th/StarRailRes-Python
 License: MIT
 Author: mobyw
 Author-email: mobyw66@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

