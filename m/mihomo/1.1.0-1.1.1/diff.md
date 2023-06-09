# Comparing `tmp/mihomo-1.1.0.tar.gz` & `tmp/mihomo-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mihomo-1.1.0.tar", max compression
+gzip compressed data, was "mihomo-1.1.1.tar", max compression
```

## Comparing `mihomo-1.1.0.tar` & `mihomo-1.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1090 2023-06-01 05:14:24.496130 mihomo-1.1.0/LICENSE
--rw-r--r--   0        0        0       90 2023-06-07 08:41:32.652372 mihomo-1.1.0/mihomo/__init__.py
--rw-r--r--   0        0        0     9743 2023-06-07 08:48:35.687054 mihomo-1.1.0/mihomo/api.py
--rw-r--r--   0        0        0     3075 2023-06-07 08:17:47.615390 mihomo-1.1.0/mihomo/model.py
--rw-r--r--   0        0        0      479 2023-06-07 08:49:53.637921 mihomo-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1434 2023-06-01 05:26:11.111124 mihomo-1.1.0/README.md
--rw-r--r--   0        0        0     2141 1970-01-01 00:00:00.000000 mihomo-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-06-01 05:14:24.496130 mihomo-1.1.1/LICENSE
+-rw-r--r--   0        0        0       90 2023-06-07 08:41:32.652372 mihomo-1.1.1/mihomo/__init__.py
+-rw-r--r--   0        0        0     9766 2023-06-09 07:38:11.404566 mihomo-1.1.1/mihomo/api.py
+-rw-r--r--   0        0        0     2580 2023-06-09 09:39:14.940762 mihomo-1.1.1/mihomo/model.py
+-rw-r--r--   0        0        0      479 2023-06-09 09:41:32.149006 mihomo-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1434 2023-06-01 05:26:11.111124 mihomo-1.1.1/README.md
+-rw-r--r--   0        0        0     2141 1970-01-01 00:00:00.000000 mihomo-1.1.1/PKG-INFO
```

### Comparing `mihomo-1.1.0/LICENSE` & `mihomo-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mihomo-1.1.0/mihomo/api.py` & `mihomo-1.1.1/mihomo/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
             if response.status_code != 200:
                 return None
             return response
 
     def character_parse(
         self, data: CharacterData, language: Optional[Language] = None
     ) -> Optional[CharacterInfo]:
-        if data.equipment:
+        if data.equipment and data.equipment.tid:
             light_cone = LightConeBasicInfo(
                 id=str(data.equipment.tid),
                 rank=data.equipment.rank,
                 level=data.equipment.level,
                 promotion=data.equipment.promotion,
             )
         else:
```

### Comparing `mihomo-1.1.0/mihomo/model.py` & `mihomo-1.1.1/mihomo/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,119 +17,105 @@
     KR = "kr"
     PT = "pt"
     RU = "ru"
     TH = "th"
     VI = "vi"
 
 
-class BaseData(Struct):
-    def to_dict(self):
-        result = {}
-        for field in self.__struct_fields__:
-            value = getattr(self, field)
-            if hasattr(value, "to_dict"):
-                result[field] = value.to_dict()
-            elif isinstance(value, list) and all(hasattr(i, "to_dict") for i in value):
-                result[field] = [i.to_dict() for i in value]
-            else:
-                result[field] = value
-        return result
-
-
-class SpaceChallengeData(BaseData):
+class SpaceChallengeData(Struct):
     scheduleMaxLevel: int = 0
     scheduleGroupId: int = 0
     noneScheduleMaxLevel: int = 0
 
 
-class SpaceData(BaseData):
+class SpaceData(Struct):
     challengeInfo: Optional[SpaceChallengeData] = None
     maxRogueChallengeScore: int = 0
     equipmentCount: int = 0
     avatarCount: int = 0
     achievementCount: int = 0
 
 
-class EquipmentData(BaseData):
-    tid: int
+class EquipmentData(Struct):
+    tid: Optional[int] = None
     rank: int = 1
     level: int = 1
     promotion: int = 0
 
 
-class SkillTreeData(BaseData):
+class SkillTreeData(Struct):
     pointId: int
     level: int = 0
 
 
-class SubAffixData(BaseData):
+class SubAffixData(Struct):
     affixId: int
     cnt: int = 0
     step: int = 0
 
 
-class RelicData(BaseData):
+class RelicData(Struct):
     tid: int
     mainAffixId: int
     type: int
     level: int = 0
     exp: int = 0
     subAffixList: List[SubAffixData] = []
 
 
-class CharacterData(BaseData):
+class CharacterData(Struct):
     avatarId: int
     rank: int = 0
     level: int = 1
     promotion: int = 0
     equipment: Optional[EquipmentData] = None
     skillTreeList: List[SkillTreeData] = []
     relicList: List[RelicData] = []
 
 
-class PlayerData(BaseData):
+class PlayerData(Struct):
     uid: int
     nickname: str
     level: int = 0
     worldLevel: int = 0
     friendCount: int = 0
     headIcon: int = 200001
     signature: str = ""
     isDisplayAvatar: bool = False
     recordInfo: Optional[SpaceData] = None
     assistAvatarDetail: Optional[CharacterData] = None
     avatarDetailList: List[CharacterData] = []
 
 
-class MihomoApiData(BaseData):
+class MihomoApiData(Struct):
     detailInfo: Optional[PlayerData] = None
 
 
-class SpaceChallengeInfo(BaseData):
+class SpaceChallengeInfo(Struct):
     maze_group_id: int = 0
     maze_group_index: int = 0
     pre_maze_group_index: int = 0
 
 
-class SpaceInfo(BaseData):
+class SpaceInfo(Struct):
     challenge_data: Optional[SpaceChallengeInfo] = None
     pass_area_progress: int = 0
     light_cone_count: int = 0
     avatar_count: int = 0
     achievement_count: int = 0
 
 
-class PlayerInfo(BaseData):
+class PlayerInfo(Struct):
     uid: str
     nickname: str
     level: int = 0
     world_level: int = 0
     friend_count: int = 0
     avatar: Optional[AvatarInfo] = None
     signature: str = ""
     is_display: bool = False
     space_info: Optional[SpaceInfo] = None
 
 
-class FormattedApiInfo(BaseData):
+class FormattedApiInfo(Struct):
     player: PlayerInfo
     characters: List[CharacterInfo] = []
```

### Comparing `mihomo-1.1.0/README.md` & `mihomo-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mihomo-1.1.0/PKG-INFO` & `mihomo-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: mihomo
-Version: 1.1.0
+Version: 1.1.1
 Summary: Library for API wrapper data from mihomo
 Home-page: https://github.com/Mar-7th/mihomo.py
 License: MIT
 Author: mobyw
 Author-email: mobyw66@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: msgspec (>=0.15.1,<0.16.0)
-Requires-Dist: starrailres (>=1.0.1,<2.0.0)
+Requires-Dist: starrailres (>=1.1.0,<2.0.0)
 Project-URL: Repository, https://github.com/Mar-7th/mihomo.py
 Description-Content-Type: text/markdown
 
 # mihomo.py
 
 ## Introduction
```

