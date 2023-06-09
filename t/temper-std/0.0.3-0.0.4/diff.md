# Comparing `tmp/temper_std-0.0.3.tar.gz` & `tmp/temper_std-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "temper_std-0.0.3.tar", max compression
+gzip compressed data, was "temper_std-0.0.4.tar", max compression
```

## Comparing `temper_std-0.0.3.tar` & `temper_std-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rwxr-xr-x   0        0        0      828 2022-12-19 20:41:55.897569 temper_std-0.0.3/pyproject.toml
--rwxr-xr-x   0        0        0        0 2022-12-19 18:05:07.811130 temper_std-0.0.3/temper_std/__init__.py
--rwxr-xr-x   0        0        0      120 2022-12-19 18:05:07.814032 temper_std-0.0.3/temper_std/__init__.py.map
--rwxr-xr-x   0        0        0      124 2022-12-19 18:05:07.814922 temper_std-0.0.3/temper_std/config.py
--rwxr-xr-x   0        0        0      656 2022-12-19 18:05:07.816937 temper_std-0.0.3/temper_std/config.py.map
--rwxr-xr-x   0        0        0    29421 2022-12-19 18:05:07.895455 temper_std-0.0.3/temper_std/regex.py
--rwxr-xr-x   0        0        0    54172 2022-12-19 18:05:07.913439 temper_std-0.0.3/temper_std/regex.py.map
--rwxr-xr-x   0        0        0       36 2022-12-19 18:05:07.817950 temper_std-0.0.3/temper_std/regex__preface.py
--rwxr-xr-x   0        0        0    20183 2022-12-19 18:05:07.823333 temper_std-0.0.3/temper_std/regex__preface.py.map
--rwxr-xr-x   0        0        0     1175 2022-12-19 18:05:07.828905 temper_std-0.0.3/temper_std/testing.py
--rwxr-xr-x   0        0        0     2590 2022-12-19 18:05:07.831402 temper_std-0.0.3/temper_std/testing.py.map
--rwxr-xr-x   0        0        0       36 2022-12-19 18:05:07.824341 temper_std-0.0.3/temper_std/testing__preface.py
--rwxr-xr-x   0        0        0      912 2022-12-19 18:05:07.825636 temper_std-0.0.3/temper_std/testing__preface.py.map
--rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 temper_std-0.0.3/setup.py
--rw-r--r--   0        0        0      562 1970-01-01 00:00:00.000000 temper_std-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1115 2023-06-09 17:13:19.968197 temper_std-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-09 17:13:19.953308 temper_std-0.0.4/temper_std/__init__.py
+-rw-r--r--   0        0        0      120 2023-06-09 17:13:19.975192 temper_std-0.0.4/temper_std/__init__.py.map
+-rw-r--r--   0        0        0      445 2023-06-09 17:13:19.961195 temper_std-0.0.4/temper_std/config.py
+-rw-r--r--   0        0        0     1824 2023-06-09 17:13:19.962197 temper_std-0.0.4/temper_std/config.py.map
+-rw-r--r--   0        0        0    33661 2023-06-09 17:13:20.066194 temper_std-0.0.4/temper_std/regex.py
+-rw-r--r--   0        0        0    57772 2023-06-09 17:13:20.074195 temper_std-0.0.4/temper_std/regex.py.map
+-rw-r--r--   0        0        0       44 2023-06-09 17:13:19.960196 temper_std-0.0.4/temper_std/regex__preface.py
+-rw-r--r--   0        0        0    20439 2023-06-09 17:13:19.983680 temper_std-0.0.4/temper_std/regex__preface.py.map
+-rw-r--r--   0        0        0     1608 2023-06-09 17:13:19.996672 temper_std-0.0.4/temper_std/testing.py
+-rw-r--r--   0        0        0     3412 2023-06-09 17:13:20.002682 temper_std-0.0.4/temper_std/testing.py.map
+-rw-r--r--   0        0        0       44 2023-06-09 17:13:19.960196 temper_std-0.0.4/temper_std/testing__preface.py
+-rw-r--r--   0        0        0     1432 2023-06-09 17:13:19.961195 temper_std-0.0.4/temper_std/testing__preface.py.map
+-rw-r--r--   0        0        0      633 1970-01-01 00:00:00.000000 temper_std-0.0.4/PKG-INFO
```

### Comparing `temper_std-0.0.3/temper_std/regex.py` & `temper_std-0.0.4/temper_std/regex.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,859 +1,973 @@
-from builtins import isinstance as isinstance0, Exception as Exception5, len as len_1273, list as list_1285
-from abc import ABC as ABC3
-from temper_core import TemperObject as TemperObject1, cast_by_type as cast_by_type4, Label as Label6, NoResultException as NoResultException7, isinstance_int as isinstance_int8, cast_by_test as cast_by_test9, list_join as list_join_1264, generic_eq as generic_eq_1266, list_builder_add as list_builder_add_1267, string_code_points as string_code_points_1239, bool_not as bool_not_1270, generic_lt as generic_lt_1274, list_get as list_get_1275, int_to_string as int_to_string_1240, str_cat as str_cat_1241, generic_not_eq as generic_not_eq_1281, generic_gt_eq as generic_gt_eq_1284
-from temper_core.regex import compiled_regex_compile_formatted as compiled_regex_compile_formatted_1260, compiled_regex_compiled_found_in as compiled_regex_compiled_found_in_1261, compiled_regex_compiled_find as compiled_regex_compiled_find_1262, regex_formatter_push_capture_name as regex_formatter_push_capture_name_1268, regex_formatter_push_code_to as regex_formatter_push_code_to_1269
-def Regex(x_1245):
-  return isinstance0(x_1245, Regex__8)
-def CodePart(x_1247):
-  return isinstance0(x_1247, CodePart__13)
-def Special(x_1249):
-  return isinstance0(x_1249, Special__15)
-def SpecialSet(x_1250):
-  return isinstance0(x_1250, SpecialSet__20)
-class Regex__8(ABC3):
-  def compiled(this__9):
-    t_1230 = CompiledRegex(this__9)
-    return__57 = t_1230
-    return return__57
-  def foundIn(this__10, text__133):
-    t_1227 = this__10.compiled()
-    t_1228 = t_1227.foundIn(text__133)
-    return__58 = t_1228
-    return return__58
-  def find(this__11, text__136):
-    t_1225 = this__11.compiled()
-    t_865 = t_1225.find(text__136)
-    return__59 = t_865
-    return return__59
-def Capture(*args_1246):
-  return Capture__12(*args_1246)
-class Capture__12(Regex__8, TemperObject1):
-  def constructor__140(this__60, name__141, item__142):
-    return__61 = None
-    this__60.name__138 = name__141
-    this__60.item__139 = item__142
-    return return__61
-  def __init__(this__60, name__141, item__142):
-    this__60.constructor__140(name__141, item__142)
-  def getname__306(this__307):
-    return__308 = this__307.name__138
-    return return__308
-  def getitem__310(this__311):
-    return__312 = this__311.item__139
-    return return__312
-  name = property(getname__306, None)
-  item = property(getitem__310, None)
-class CodePart__13(Regex__8, ABC3):
-  pass
-def CodePoints(*args_1248):
-  return CodePoints__14(*args_1248)
-class CodePoints__14(CodePart__13, TemperObject1):
-  def constructor__144(this__62, value__145):
-    return__63 = None
-    this__62.value__143 = value__145
-    return return__63
-  def __init__(this__62, value__145):
-    this__62.constructor__144(value__145)
-  def getvalue__314(this__315):
-    return__316 = this__315.value__143
-    return return__316
-  value = property(getvalue__314, None)
-class Special__15(Regex__8, ABC3):
-  pass
-class SpecialSet__20(CodePart__13, Special__15, ABC3):
-  pass
-def CodeRange(*args_1251):
-  return CodeRange__24(*args_1251)
-class CodeRange__24(CodePart__13, TemperObject1):
-  def constructor__162(this__78, min__163, max__164):
-    return__79 = None
-    this__78.min__160 = min__163
-    this__78.max__161 = max__164
-    return return__79
-  def __init__(this__78, min__163, max__164):
-    this__78.constructor__162(min__163, max__164)
-  def getmin__318(this__319):
-    return__320 = this__319.min__160
-    return return__320
-  def getmax__322(this__323):
-    return__324 = this__323.max__161
-    return return__324
-  min = property(getmin__318, None)
-  max = property(getmax__322, None)
-def CodeSet(*args_1252):
-  return CodeSet__25(*args_1252)
-class CodeSet__25(Regex__8, TemperObject1):
-  def constructor__167(this__80, items__168, negated = ...):
-    negated__169 = negated
-    return__82 = None
-    if negated__169 is ...:
-      negated__169 = False
-    this__80.items__165 = items__168
-    this__80.negated__166 = negated__169
-    return return__82
-  def __init__(this__80, items__168, negated = ...):
-    negated__169 = negated
-    this__80.constructor__167(items__168, negated__169)
-  def getitems__326(this__327):
-    return__328 = this__327.items__165
-    return return__328
-  def getnegated__330(this__331):
-    return__332 = this__331.negated__166
-    return return__332
-  items = property(getitems__326, None)
-  negated = property(getnegated__330, None)
-def Or(*args_1253):
-  return Or__26(*args_1253)
-class Or__26(Regex__8, TemperObject1):
-  def constructor__171(this__83, items__172):
-    return__85 = None
-    this__83.items__170 = items__172
-    return return__85
-  def __init__(this__83, items__172):
-    this__83.constructor__171(items__172)
-  def getitems__334(this__335):
-    return__336 = this__335.items__170
-    return return__336
-  items = property(getitems__334, None)
-def Repeat(*args_1254):
-  return Repeat__27(*args_1254)
-class Repeat__27(Regex__8, TemperObject1):
-  def constructor__177(this__86, item__178, min__179, max__180, reluctant = ...):
-    reluctant__181 = reluctant
+from temper_core import TemperObject as TemperObject0, cast_by_type as cast_by_type8, Label as Label10, NoResultException as NoResultException11, isinstance_int as isinstance_int12, cast_by_test as cast_by_test13, list_join as list_join_1213, generic_eq as generic_eq_1222, list_builder_add as list_builder_add_1215, string_code_points as string_code_points_1225, bool_not as bool_not_1214, list_get as list_get_1231, int_to_string as int_to_string_1241, str_cat as str_cat_1212
+from typing import Union as Union4, NoReturn as NoReturn5, Callable as Callable2, Any as Any6, Tuple as Tuple7, List as List1
+from builtins import Exception as Exception9, len as len_1230, list as list_1210
+from temper_core.regex import compiled_regex_compile_formatted as compiled_regex_compile_formatted_1216, compiled_regex_compiled_found as compiled_regex_compiled_found_1217, compiled_regex_compiled_find as compiled_regex_compiled_find_1218, compiled_regex_compiled_replace as compiled_regex_compiled_replace_1219, regex_formatter_push_capture_name as regex_formatter_push_capture_name_1223, regex_formatter_push_code_to as regex_formatter_push_code_to_1224
+class Regex(TemperObject0):
+  __slots__ = ()
+  def compiled(this__8) -> 'CompiledRegex':
+    return__46: 'CompiledRegex'
+    t_1201: 'CompiledRegex' = CompiledRegex(this__8)
+    return__46 = t_1201
+    return return__46
+  def found(this__9, text__120: 'str') -> 'bool':
+    return__47: 'bool'
+    t_1198: 'CompiledRegex' = this__9.compiled()
+    t_1199: 'bool' = t_1198.found(text__120)
+    return__47 = t_1199
+    return return__47
+  def find(this__10, text__123: 'str') -> 'Union4[(Map__16[str, Group]), NoReturn5]':
+    return__48: 'Map__16[str, Group]'
+    t_836: 'Map__16[str, Group]'
+    t_1196: 'CompiledRegex' = this__10.compiled()
+    t_836 = t_1196.find(text__123)
+    return__48 = t_836
+    return return__48
+  def replace(this__11, text__126: 'str', format__127: 'Callable2[[Map__16[str, Group]], str]') -> 'str':
+    return__49: 'str'
+    t_1193: 'CompiledRegex' = this__11.compiled()
+    t_1194: 'str' = t_1193.replace(text__126, format__127)
+    return__49 = t_1194
+    return return__49
+class Capture(Regex):
+  name__129: 'str'
+  item__130: 'Regex'
+  __slots__ = ('name__129', 'item__130')
+  def constructor__131(this__50, name__132: 'str', item__133: 'Regex') -> Any6:
+    return__51: 'None'
+    return__51 = None
+    this__50.name__129 = name__132
+    this__50.item__130 = item__133
+    return return__51
+  def __init__(this__50, name__132: 'str', item__133: 'Regex') -> None:
+    this__50.constructor__131(name__132, item__133)
+  @property
+  def name(this__298) -> 'str':
+    return__299: 'str'
+    return__299 = this__298.name__129
+    return return__299
+  @property
+  def item(this__302) -> 'Regex':
+    return__303: 'Regex'
+    return__303 = this__302.item__130
+    return return__303
+class CodePart(Regex):
+  __slots__ = ()
+class CodePoints(CodePart):
+  value__134: 'str'
+  __slots__ = ('value__134',)
+  def constructor__135(this__52, value__136: 'str') -> Any6:
+    return__53: 'None'
+    return__53 = None
+    this__52.value__134 = value__136
+    return return__53
+  def __init__(this__52, value__136: 'str') -> None:
+    this__52.constructor__135(value__136)
+  @property
+  def value(this__306) -> 'str':
+    return__307: 'str'
+    return__307 = this__306.value__134
+    return return__307
+class Special(Regex):
+  __slots__ = ()
+class SpecialSet(CodePart, Special):
+  __slots__ = ()
+class CodeRange(CodePart):
+  min__144: 'int'
+  max__145: 'int'
+  __slots__ = ('min__144', 'max__145')
+  def constructor__146(this__68, min__147: 'int', max__148: 'int') -> Any6:
+    return__69: 'None'
+    return__69 = None
+    this__68.min__144 = min__147
+    this__68.max__145 = max__148
+    return return__69
+  def __init__(this__68, min__147: 'int', max__148: 'int') -> None:
+    this__68.constructor__146(min__147, max__148)
+  @property
+  def min(this__310) -> 'int':
+    return__311: 'int'
+    return__311 = this__310.min__144
+    return return__311
+  @property
+  def max(this__314) -> 'int':
+    return__315: 'int'
+    return__315 = this__314.max__145
+    return return__315
+class CodeSet(Regex):
+  items__149: 'Tuple7[CodePart, ...]'
+  negated__150: 'bool'
+  __slots__ = ('items__149', 'negated__150')
+  def constructor__151(this__70, items__152: 'Tuple7[CodePart, ...]', negated: 'bool' = ...) -> Any6:
+    negated__153: 'bool' = negated
+    return__72: 'None'
+    return__72 = None
+    if negated__153 is ...:
+      negated__153 = False
+    this__70.items__149 = items__152
+    this__70.negated__150 = negated__153
+    return return__72
+  def __init__(this__70, items__152: 'Tuple7[CodePart, ...]', negated: 'bool' = ...) -> None:
+    negated__153: 'bool' = negated
+    this__70.constructor__151(items__152, negated__153)
+  @property
+  def items(this__318) -> 'Tuple7[CodePart, ...]':
+    return__319: 'Tuple7[CodePart, ...]'
+    return__319 = this__318.items__149
+    return return__319
+  @property
+  def negated(this__322) -> 'bool':
+    return__323: 'bool'
+    return__323 = this__322.negated__150
+    return return__323
+class Or(Regex):
+  items__154: 'Tuple7[Regex, ...]'
+  __slots__ = ('items__154',)
+  def constructor__155(this__73, items__156: 'Tuple7[Regex, ...]') -> Any6:
+    return__75: 'None'
+    return__75 = None
+    this__73.items__154 = items__156
+    return return__75
+  def __init__(this__73, items__156: 'Tuple7[Regex, ...]') -> None:
+    this__73.constructor__155(items__156)
+  @property
+  def items(this__326) -> 'Tuple7[Regex, ...]':
+    return__327: 'Tuple7[Regex, ...]'
+    return__327 = this__326.items__154
+    return return__327
+class Repeat(Regex):
+  item__157: 'Regex'
+  min__158: 'int'
+  max__159: 'Union4[int, None]'
+  reluctant__160: 'bool'
+  __slots__ = ('item__157', 'min__158', 'max__159', 'reluctant__160')
+  def constructor__161(this__76, item__162: 'Regex', min__163: 'int', max__164: 'Union4[int, None]', reluctant: 'bool' = ...) -> Any6:
+    reluctant__165: 'bool' = reluctant
+    return__78: 'None'
+    return__78 = None
+    if reluctant__165 is ...:
+      reluctant__165 = False
+    this__76.item__157 = item__162
+    this__76.min__158 = min__163
+    this__76.max__159 = max__164
+    this__76.reluctant__160 = reluctant__165
+    return return__78
+  def __init__(this__76, item__162: 'Regex', min__163: 'int', max__164: 'Union4[int, None]', reluctant: 'bool' = ...) -> None:
+    reluctant__165: 'bool' = reluctant
+    this__76.constructor__161(item__162, min__163, max__164, reluctant__165)
+  @property
+  def item(this__330) -> 'Regex':
+    return__331: 'Regex'
+    return__331 = this__330.item__157
+    return return__331
+  @property
+  def min(this__334) -> 'int':
+    return__335: 'int'
+    return__335 = this__334.min__158
+    return return__335
+  @property
+  def max(this__338) -> 'Union4[int, None]':
+    return__339: 'Union4[int, None]'
+    return__339 = this__338.max__159
+    return return__339
+  @property
+  def reluctant(this__342) -> 'bool':
+    return__343: 'bool'
+    return__343 = this__342.reluctant__160
+    return return__343
+class Sequence(Regex):
+  items__174: 'Tuple7[Regex, ...]'
+  __slots__ = ('items__174',)
+  def constructor__175(this__82, items__176: 'Tuple7[Regex, ...]') -> Any6:
+    return__84: 'None'
+    return__84 = None
+    this__82.items__174 = items__176
+    return return__84
+  def __init__(this__82, items__176: 'Tuple7[Regex, ...]') -> None:
+    this__82.constructor__175(items__176)
+  @property
+  def items(this__346) -> 'Tuple7[Regex, ...]':
+    return__347: 'Tuple7[Regex, ...]'
+    return__347 = this__346.items__174
+    return return__347
+class Group(TemperObject0):
+  name__177: 'str'
+  value__178: 'str'
+  codePointsBegin__179: 'int'
+  __slots__ = ('name__177', 'value__178', 'codePointsBegin__179')
+  def constructor__180(this__85, name__181: 'str', value__182: 'str', codePointsBegin__183: 'int') -> Any6:
+    return__86: 'None'
+    return__86 = None
+    this__85.name__177 = name__181
+    this__85.value__178 = value__182
+    this__85.codePointsBegin__179 = codePointsBegin__183
+    return return__86
+  def __init__(this__85, name__181: 'str', value__182: 'str', codePointsBegin__183: 'int') -> None:
+    this__85.constructor__180(name__181, value__182, codePointsBegin__183)
+  @property
+  def name(this__350) -> 'str':
+    return__351: 'str'
+    return__351 = this__350.name__177
+    return return__351
+  @property
+  def value(this__354) -> 'str':
+    return__355: 'str'
+    return__355 = this__354.value__178
+    return return__355
+  @property
+  def code_points_begin(this__358) -> 'int':
+    return__359: 'int'
+    return__359 = this__358.codePointsBegin__179
+    return return__359
+class RegexRefs__19(TemperObject0):
+  codePoints__184: 'CodePoints'
+  group__185: 'Group'
+  orObject__186: 'Or'
+  __slots__ = ('codePoints__184', 'group__185', 'orObject__186')
+  def constructor__187(this__87, code_points: 'CodePoints' = ..., group: 'Group' = ..., or_object: 'Or' = ...) -> Any6:
+    codePoints__188: 'CodePoints' = code_points
+    group__189: 'Group' = group
+    orObject__190: 'Or' = or_object
+    return__88: 'None'
+    t_1145: 'CodePoints'
+    t_1147: 'Group'
+    t_1149: 'Or'
     return__88 = None
-    if reluctant__181 is ...:
-      reluctant__181 = False
-    this__86.item__173 = item__178
-    this__86.min__174 = min__179
-    this__86.max__175 = max__180
-    this__86.reluctant__176 = reluctant__181
+    if codePoints__188 is ...:
+      t_1145 = CodePoints('')
+      codePoints__188 = t_1145
+    if group__189 is ...:
+      t_1147 = Group('', '', 0)
+      group__189 = t_1147
+    if orObject__190 is ...:
+      t_1149 = Or(())
+      orObject__190 = t_1149
+    this__87.codePoints__184 = codePoints__188
+    this__87.group__185 = group__189
+    this__87.orObject__186 = orObject__190
     return return__88
-  def __init__(this__86, item__178, min__179, max__180, reluctant = ...):
-    reluctant__181 = reluctant
-    this__86.constructor__177(item__178, min__179, max__180, reluctant__181)
-  def getitem__338(this__339):
-    return__340 = this__339.item__173
-    return return__340
-  def getmin__342(this__343):
-    return__344 = this__343.min__174
-    return return__344
-  def getmax__346(this__347):
-    return__348 = this__347.max__175
-    return return__348
-  def getreluctant__350(this__351):
-    return__352 = this__351.reluctant__176
-    return return__352
-  item = property(getitem__338, None)
-  min = property(getmin__342, None)
-  max = property(getmax__346, None)
-  reluctant = property(getreluctant__350, None)
-def Sequence(*args_1255):
-  return Sequence__28(*args_1255)
-class Sequence__28(Regex__8, TemperObject1):
-  def constructor__191(this__92, items__192):
-    return__94 = None
-    this__92.items__190 = items__192
-    return return__94
-  def __init__(this__92, items__192):
-    this__92.constructor__191(items__192)
-  def getitems__354(this__355):
-    return__356 = this__355.items__190
-    return return__356
-  items = property(getitems__354, None)
-def Match(*args_1256):
-  return Match__29(*args_1256)
-class Match__29(TemperObject1):
-  def constructor__194(this__95, groups__195):
-    return__97 = None
-    this__95.groups__193 = groups__195
+  def __init__(this__87, code_points: 'CodePoints' = ..., group: 'Group' = ..., or_object: 'Or' = ...) -> None:
+    codePoints__188: 'CodePoints' = code_points
+    group__189: 'Group' = group
+    orObject__190: 'Or' = or_object
+    this__87.constructor__187(codePoints__188, group__189, orObject__190)
+  @property
+  def code_points(this__362) -> 'CodePoints':
+    return__363: 'CodePoints'
+    return__363 = this__362.codePoints__184
+    return return__363
+  @property
+  def group(this__366) -> 'Group':
+    return__367: 'Group'
+    return__367 = this__366.group__185
+    return return__367
+  @property
+  def or_object(this__370) -> 'Or':
+    return__371: 'Or'
+    return__371 = this__370.orObject__186
+    return return__371
+class CompiledRegex(TemperObject0):
+  data__192: 'Regex'
+  compiled__206: 'Any6'
+  __slots__ = ('data__192', 'compiled__206')
+  def constructor__193(this__20, data__194: 'Regex') -> Any6:
+    return__89: 'None'
+    return__89 = None
+    this__20.data__192 = data__194
+    t_1139: 'str' = this__20.format__225()
+    t_1140: 'Any6' = compiled_regex_compile_formatted_1216(this__20, t_1139)
+    this__20.compiled__206 = t_1140
+    return return__89
+  def __init__(this__20, data__194: 'Regex') -> None:
+    this__20.constructor__193(data__194)
+  def found(this__21, text__197: 'str') -> 'bool':
+    return__90: 'bool'
+    t_1138: 'bool' = compiled_regex_compiled_found_1217(this__21, this__21.compiled__206, text__197)
+    return__90 = t_1138
+    return return__90
+  def find(this__22, text__200: 'str') -> 'Union4[(Map__16[str, Group]), NoReturn5]':
+    return__91: 'Map__16[str, Group]'
+    t_795: 'Map__16[str, Group]'
+    t_795 = compiled_regex_compiled_find_1218(this__22, this__22.compiled__206, text__200, regexRefs__191)
+    return__91 = t_795
+    return return__91
+  def replace(this__23, text__203: 'str', format__204: 'Callable2[[Map__16[str, Group]], str]') -> 'str':
+    return__92: 'str'
+    t_1135: 'str' = compiled_regex_compiled_replace_1219(this__23, this__23.compiled__206, text__203, format__204, regexRefs__191)
+    return__92 = t_1135
+    return return__92
+  def format__225(this__28) -> 'str':
+    return__97: 'str'
+    t_1128: 'RegexFormatter__29' = RegexFormatter__29()
+    t_1129: 'str' = t_1128.format(this__28.data__192)
+    return__97 = t_1129
     return return__97
-  def __init__(this__95, groups__195):
-    this__95.constructor__194(groups__195)
-  def getgroups__358(this__359):
-    return__360 = this__359.groups__193
-    return return__360
-  groups = property(getgroups__358, None)
-def Group(*args_1257):
-  return Group__30(*args_1257)
-class Group__30(TemperObject1):
-  def constructor__199(this__98, name__200, value__201, codePointsBegin__202):
-    return__99 = None
-    this__98.name__196 = name__200
-    this__98.value__197 = value__201
-    this__98.codePointsBegin__198 = codePointsBegin__202
-    return return__99
-  def __init__(this__98, name__200, value__201, codePointsBegin__202):
-    this__98.constructor__199(name__200, value__201, codePointsBegin__202)
-  def getname__362(this__363):
-    return__364 = this__363.name__196
-    return return__364
-  def getvalue__366(this__367):
-    return__368 = this__367.value__197
-    return return__368
-  def getcodePointsBegin__370(this__371):
-    return__372 = this__371.codePointsBegin__198
-    return return__372
-  name = property(getname__362, None)
-  value = property(getvalue__366, None)
-  code_points_begin = property(getcodePointsBegin__370, None)
-def RegexRefs__128(*args_1258):
-  return RegexRefs__31(*args_1258)
-class RegexRefs__31(TemperObject1):
-  def constructor__206(this__100, code_points = ..., match__208 = ..., or_object = ...):
-    codePoints__207 = code_points
-    match__208 = match__208
-    orObject__209 = or_object
-    return__101 = None
-    if codePoints__207 is ...:
-      t_1174 = CodePoints('')
-      codePoints__207 = t_1174
-    if match__208 is ...:
-      t_1176 = Group('', '', 0)
-      t_1178 = Match((t_1176,))
-      match__208 = t_1178
-    if orObject__209 is ...:
-      t_1179 = Or(())
-      orObject__209 = t_1179
-    this__100.codePoints__203 = codePoints__207
-    this__100.match__204 = match__208
-    this__100.orObject__205 = orObject__209
+  @property
+  def data(this__374) -> 'Regex':
+    return__375: 'Regex'
+    return__375 = this__374.data__192
+    return return__375
+class RegexFormatter__29(TemperObject0):
+  out__227: 'List1[str]'
+  __slots__ = ('out__227',)
+  def format(this__30, regex__229: 'Regex') -> 'str':
+    return__101: 'str'
+    this__30.pushRegex__232(regex__229)
+    t_1124: 'List1[str]' = this__30.out__227
+    def fn__1120(x__231: 'str') -> 'str':
+      return__866: 'str'
+      return__866 = x__231
+      return return__866
+    t_1123: 'Callable2[[str], str]' = fn__1120
+    t_1125: 'str' = list_join_1213(t_1124, '', t_1123)
+    return__101 = t_1125
     return return__101
-  def __init__(this__100, code_points = ..., match__208 = ..., or_object = ...):
-    codePoints__207 = code_points
-    match__208 = match__208
-    orObject__209 = or_object
-    this__100.constructor__206(codePoints__207, match__208, orObject__209)
-  def getcodePoints__374(this__375):
-    return__376 = this__375.codePoints__203
-    return return__376
-  def getmatch__378(this__379):
-    return__380 = this__379.match__204
-    return return__380
-  def getorObject__382(this__383):
-    return__384 = this__383.orObject__205
-    return return__384
-  code_points = property(getcodePoints__374, None)
-  match = property(getmatch__378, None)
-  or_object = property(getorObject__382, None)
-def CompiledRegex(*args_1259):
-  return CompiledRegex__32(*args_1259)
-class CompiledRegex__32(TemperObject1):
-  def constructor__212(this__33, data__213):
+  def pushRegex__232(this__31, regex__233: 'Regex') -> 'None':
+    return__102: 'None'
     return__102 = None
-    this__33.data__211 = data__213
-    t_1168 = this__33.format()
-    t_1169 = compiled_regex_compile_formatted_1260(this__33, t_1168)
-    this__33.compiled__221 = t_1169
-    return return__102
-  def __init__(this__33, data__213):
-    this__33.constructor__212(data__213)
-  def foundIn(this__34, text__216):
-    t_1167 = compiled_regex_compiled_found_in_1261(this__34, this__34.compiled__221, text__216)
-    return__103 = t_1167
-    return return__103
-  def find(this__35, text__219):
-    t_824 = compiled_regex_compiled_find_1262(this__35, this__35.compiled__221, text__219, regexRefs__210)
-    return__104 = t_824
-    return return__104
-  def format(this__39):
-    t_1160 = RegexFormatter__129()
-    t_1161 = t_1160.format(this__39.data__211)
-    return__108 = t_1161
-    return return__108
-  def getdata__386(this__387):
-    return__388 = this__387.data__211
-    return return__388
-  data = property(getdata__386, None)
-  compiled = property(None, None)
-def RegexFormatter__129(*args_1263):
-  return RegexFormatter__40(*args_1263)
-class RegexFormatter__40(TemperObject1):
-  def format(this__41, regex__238):
-    this__41.pushRegex(regex__238)
-    t_1156 = this__41.out__236
-    def fn__1152(x__240):
-      return__895 = x__240
-      return return__895
-    t_1155 = fn__1152
-    t_1157 = list_join_1264(t_1156, '', t_1155)
-    return__112 = t_1157
-    return return__112
-  def pushRegex(this__42, regex__242):
-    return__113 = None
+    t_755: 'bool'
+    t_756: 'Capture'
+    t_759: 'bool'
+    t_760: 'CodePoints'
+    t_763: 'bool'
+    t_764: 'CodeRange'
+    t_767: 'bool'
+    t_768: 'CodeSet'
+    t_771: 'bool'
+    t_772: 'Or'
+    t_775: 'bool'
+    t_776: 'Repeat'
+    t_779: 'bool'
+    t_780: 'Sequence'
     try:
-      cast_by_type4(regex__242, Capture__12)
-      t_785 = True
-    except Exception5:
-      t_785 = False
-    with Label6() as s_1265:
-      if t_785:
+      cast_by_type8(regex__233, Capture)
+      t_755 = True
+    except Exception9:
+      t_755 = False
+    with Label10() as s__1220_1221:
+      if t_755:
         try:
-          t_786 = cast_by_type4(regex__242, Capture__12)
-        except Exception5:
-          s_1265.break_()
-        this__42.pushCapture(t_786)
+          t_756 = cast_by_type8(regex__233, Capture)
+        except Exception9:
+          s__1220_1221.break_()
+        this__31.pushCapture__235(t_756)
       else:
         try:
-          cast_by_type4(regex__242, CodePoints__14)
-          t_789 = True
-        except Exception5:
-          t_789 = False
-        if t_789:
+          cast_by_type8(regex__233, CodePoints)
+          t_759 = True
+        except Exception9:
+          t_759 = False
+        if t_759:
           try:
-            t_790 = cast_by_type4(regex__242, CodePoints__14)
-          except Exception5:
-            s_1265.break_()
-          this__42.pushCodePoints(t_790, False)
+            t_760 = cast_by_type8(regex__233, CodePoints)
+          except Exception9:
+            s__1220_1221.break_()
+          this__31.pushCodePoints__251(t_760, False)
         else:
           try:
-            cast_by_type4(regex__242, CodeRange__24)
-            t_793 = True
-          except Exception5:
-            t_793 = False
-          if t_793:
+            cast_by_type8(regex__233, CodeRange)
+            t_763 = True
+          except Exception9:
+            t_763 = False
+          if t_763:
             try:
-              t_794 = cast_by_type4(regex__242, CodeRange__24)
-            except Exception5:
-              s_1265.break_()
-            this__42.pushCodeRange(t_794)
+              t_764 = cast_by_type8(regex__233, CodeRange)
+            except Exception9:
+              s__1220_1221.break_()
+            this__31.pushCodeRange__256(t_764)
           else:
             try:
-              cast_by_type4(regex__242, CodeSet__25)
-              t_797 = True
-            except Exception5:
-              t_797 = False
-            if t_797:
+              cast_by_type8(regex__233, CodeSet)
+              t_767 = True
+            except Exception9:
+              t_767 = False
+            if t_767:
               try:
-                t_798 = cast_by_type4(regex__242, CodeSet__25)
-              except Exception5:
-                s_1265.break_()
-              this__42.pushCodeSet(t_798)
+                t_768 = cast_by_type8(regex__233, CodeSet)
+              except Exception9:
+                s__1220_1221.break_()
+              this__31.pushCodeSet__262(t_768)
             else:
               try:
-                cast_by_type4(regex__242, Or__26)
-                t_801 = True
-              except Exception5:
-                t_801 = False
-              if t_801:
+                cast_by_type8(regex__233, Or)
+                t_771 = True
+              except Exception9:
+                t_771 = False
+              if t_771:
                 try:
-                  t_802 = cast_by_type4(regex__242, Or__26)
-                except Exception5:
-                  s_1265.break_()
-                this__42.pushOr(t_802)
+                  t_772 = cast_by_type8(regex__233, Or)
+                except Exception9:
+                  s__1220_1221.break_()
+                this__31.pushOr__274(t_772)
               else:
                 try:
-                  cast_by_type4(regex__242, Repeat__27)
-                  t_805 = True
-                except Exception5:
-                  t_805 = False
-                if t_805:
+                  cast_by_type8(regex__233, Repeat)
+                  t_775 = True
+                except Exception9:
+                  t_775 = False
+                if t_775:
                   try:
-                    t_806 = cast_by_type4(regex__242, Repeat__27)
-                  except Exception5:
-                    s_1265.break_()
-                  this__42.pushRepeat(t_806)
+                    t_776 = cast_by_type8(regex__233, Repeat)
+                  except Exception9:
+                    s__1220_1221.break_()
+                  this__31.pushRepeat__278(t_776)
                 else:
                   try:
-                    cast_by_type4(regex__242, Sequence__28)
-                    t_809 = True
-                  except Exception5:
-                    t_809 = False
-                  if t_809:
+                    cast_by_type8(regex__233, Sequence)
+                    t_779 = True
+                  except Exception9:
+                    t_779 = False
+                  if t_779:
                     try:
-                      t_810 = cast_by_type4(regex__242, Sequence__28)
-                    except Exception5:
-                      s_1265.break_()
-                    this__42.pushSequence(t_810)
-                  elif generic_eq_1266(regex__242, Begin):
+                      t_780 = cast_by_type8(regex__233, Sequence)
+                    except Exception9:
+                      s__1220_1221.break_()
+                    this__31.pushSequence__283(t_780)
+                  elif generic_eq_1222(regex__233, begin):
                     try:
-                      list_builder_add_1267(this__42.out__236, '^')
-                    except Exception5:
-                      s_1265.break_()
-                  elif generic_eq_1266(regex__242, Dot):
+                      list_builder_add_1215(this__31.out__227, '^')
+                    except Exception9:
+                      s__1220_1221.break_()
+                  elif generic_eq_1222(regex__233, dot):
                     try:
-                      list_builder_add_1267(this__42.out__236, '.')
-                    except Exception5:
-                      s_1265.break_()
-                  elif generic_eq_1266(regex__242, End):
+                      list_builder_add_1215(this__31.out__227, '.')
+                    except Exception9:
+                      s__1220_1221.break_()
+                  elif generic_eq_1222(regex__233, end):
                     try:
-                      list_builder_add_1267(this__42.out__236, '$')
-                    except Exception5:
-                      s_1265.break_()
-                  elif generic_eq_1266(regex__242, WordBoundary):
+                      list_builder_add_1215(this__31.out__227, '$')
+                    except Exception9:
+                      s__1220_1221.break_()
+                  elif generic_eq_1222(regex__233, word_boundary):
                     try:
-                      list_builder_add_1267(this__42.out__236, '\\b')
-                    except Exception5:
-                      s_1265.break_()
-                  elif generic_eq_1266(regex__242, Digit):
+                      list_builder_add_1215(this__31.out__227, '\\b')
+                    except Exception9:
+                      s__1220_1221.break_()
+                  elif generic_eq_1222(regex__233, digit):
                     try:
-                      list_builder_add_1267(this__42.out__236, '\\d')
-                    except Exception5:
-                      s_1265.break_()
-                  elif generic_eq_1266(regex__242, Space):
+                      list_builder_add_1215(this__31.out__227, '\\d')
+                    except Exception9:
+                      s__1220_1221.break_()
+                  elif generic_eq_1222(regex__233, space):
                     try:
-                      list_builder_add_1267(this__42.out__236, '\\s')
-                    except Exception5:
-                      s_1265.break_()
-                  elif generic_eq_1266(regex__242, Word):
+                      list_builder_add_1215(this__31.out__227, '\\s')
+                    except Exception9:
+                      s__1220_1221.break_()
+                  elif generic_eq_1222(regex__233, word):
                     try:
-                      list_builder_add_1267(this__42.out__236, '\\w')
-                    except Exception5:
-                      s_1265.break_()
-      return return__113
-    raise NoResultException7()
-  def pushCapture(this__43, capture__245):
-    return__114 = None
-    list_builder_add_1267(this__43.out__236, '(')
-    t_780 = this__43.out__236
-    t_1138 = capture__245.name
-    regex_formatter_push_capture_name_1268(this__43, t_780, t_1138)
-    t_1140 = capture__245.item
-    this__43.pushRegex(t_1140)
-    list_builder_add_1267(this__43.out__236, ')')
-    return return__114
-  def pushCode(this__45, code__252, insideCodeSet__253):
-    return__116 = None
-    regex_formatter_push_code_to_1269(this__45, this__45.out__236, code__252, insideCodeSet__253)
-    return return__116
-  def pushCodePoints(this__47, codePoints__261, insideCodeSet__262):
-    return__118 = None
-    t_1126 = codePoints__261.value
-    t_1132 = string_code_points_1239(t_1126)
-    slice__264 = t_1132
+                      list_builder_add_1215(this__31.out__227, '\\w')
+                    except Exception9:
+                      s__1220_1221.break_()
+      return return__102
+    raise NoResultException11()
+  def pushCapture__235(this__32, capture__236: 'Capture') -> 'None':
+    return__103: 'None'
+    t_1106: 'str'
+    t_1108: 'Regex'
+    return__103 = None
+    t_750: 'List1[str]'
+    list_builder_add_1215(this__32.out__227, '(')
+    t_750 = this__32.out__227
+    t_1106 = capture__236.name
+    regex_formatter_push_capture_name_1223(this__32, t_750, t_1106)
+    t_1108 = capture__236.item
+    this__32.pushRegex__232(t_1108)
+    list_builder_add_1215(this__32.out__227, ')')
+    return return__103
+  def pushCode__242(this__34, code__243: 'int', insideCodeSet__244: 'bool') -> 'None':
+    return__105: 'None'
+    return__105 = None
+    regex_formatter_push_code_to_1224(this__34, this__34.out__227, code__243, insideCodeSet__244)
+    return return__105
+  def pushCodePoints__251(this__36, codePoints__252: 'CodePoints', insideCodeSet__253: 'bool') -> 'None':
+    return__107: 'None'
+    t_1096: 'bool'
+    t_1097: 'int'
+    t_1098: 'Any6'
+    return__107 = None
+    t_1095: 'str' = codePoints__252.value
+    t_1100: 'Any6' = string_code_points_1225(t_1095)
+    slice__255: 'Any6' = t_1100
     while True:
-      t_1127 = slice__264.is_empty
-      t_1131 = bool_not_1270(t_1127)
-      if t_1131:
-        t_1128 = slice__264.read()
-        this__47.pushCode(t_1128, insideCodeSet__262)
-        t_1129 = slice__264.advance(1)
-        slice__264 = t_1129
+      t_1096 = slice__255.is_empty
+      if bool_not_1214(t_1096):
+        t_1097 = slice__255.read()
+        this__36.pushCode__242(t_1097, insideCodeSet__253)
+        t_1098 = slice__255.advance(1)
+        slice__255 = t_1098
       else:
         break
-    return return__118
-  def pushCodeRange(this__48, codeRange__266):
-    return__119 = None
-    list_builder_add_1267(this__48.out__236, '[')
-    this__48.pushCodeRangeUnwrapped(codeRange__266)
-    list_builder_add_1267(this__48.out__236, ']')
-    return return__119
-  def pushCodeRangeUnwrapped(this__49, codeRange__269):
-    return__120 = None
-    t_1119 = codeRange__269.min
-    this__49.pushCode(t_1119, True)
-    list_builder_add_1267(this__49.out__236, '-')
-    t_1121 = codeRange__269.max
-    this__49.pushCode(t_1121, True)
-    return return__120
-  def pushCodeSet(this__50, codeSet__272):
-    return__121 = None
-    t_1111 = this__50.adjustCodeSet(codeSet__272, regexRefs__210)
-    adjusted__274 = t_1111
+    return return__107
+  def pushCodeRange__256(this__37, codeRange__257: 'CodeRange') -> 'None':
+    return__108: 'None'
+    return__108 = None
+    list_builder_add_1215(this__37.out__227, '[')
+    this__37.pushCodeRangeUnwrapped__259(codeRange__257)
+    list_builder_add_1215(this__37.out__227, ']')
+    return return__108
+  def pushCodeRangeUnwrapped__259(this__38, codeRange__260: 'CodeRange') -> 'None':
+    return__109: 'None'
+    t_1090: 'int'
+    return__109 = None
+    t_1088: 'int' = codeRange__260.min
+    this__38.pushCode__242(t_1088, True)
+    list_builder_add_1215(this__38.out__227, '-')
+    t_1090 = codeRange__260.max
+    this__38.pushCode__242(t_1090, True)
+    return return__109
+  def pushCodeSet__262(this__39, codeSet__263: 'CodeSet') -> 'None':
+    return__110: 'None'
+    t_1082: 'Tuple7[CodePart, ...]'
+    t_1083: 'Tuple7[CodePart, ...]'
+    t_1085: 'int'
+    t_1086: 'bool'
+    return__110 = None
+    t_720: 'bool'
+    t_721: 'CodeSet'
+    t_727: 'CodePart'
+    t_1080: 'Regex' = this__39.adjustCodeSet__267(codeSet__263, regexRefs__191)
+    adjusted__265: 'Regex' = t_1080
     try:
-      cast_by_type4(adjusted__274, CodeSet__25)
-      t_747 = True
-    except Exception5:
-      t_747 = False
-    with Label6() as s_1271:
-      if t_747:
-        with Label6() as s_1272:
+      cast_by_type8(adjusted__265, CodeSet)
+      t_720 = True
+    except Exception9:
+      t_720 = False
+    with Label10() as s__1226_1228:
+      if t_720:
+        with Label10() as s__1227_1229:
           try:
-            t_748 = cast_by_type4(adjusted__274, CodeSet__25)
-            list_builder_add_1267(this__50.out__236, '[')
-          except Exception5:
-            s_1272.break_()
-          t_1117 = t_748.negated
-          if t_1117:
+            t_721 = cast_by_type8(adjusted__265, CodeSet)
+            list_builder_add_1215(this__39.out__227, '[')
+          except Exception9:
+            s__1227_1229.break_()
+          t_1086 = t_721.negated
+          if t_1086:
             try:
-              list_builder_add_1267(this__50.out__236, '^')
-            except Exception5:
-              s_1272.break_()
-          i__275 = 0
+              list_builder_add_1215(this__39.out__227, '^')
+            except Exception9:
+              s__1227_1229.break_()
+          i__266: 'int' = 0
           while True:
-            t_1113 = t_748.items
-            t_1116 = len_1273(t_1113)
-            try:
-              t_753 = generic_lt_1274(i__275, t_1116)
-            except Exception5:
-              break
-            if t_753:
-              t_1114 = t_748.items
+            t_1082 = t_721.items
+            t_1085 = len_1230(t_1082)
+            if i__266 < t_1085:
+              t_1083 = t_721.items
               try:
-                t_756 = list_get_1275(t_1114, i__275)
-              except Exception5:
-                break
-              this__50.pushCodeSetItem(t_756)
-              t_754 = i__275 + 1
-              i__275 = t_754
+                t_727 = list_get_1231(t_1083, i__266)
+              except Exception9:
+                s__1227_1229.break_()
+              this__39.pushCodeSetItem__271(t_727)
+              i__266 = i__266 + 1
             else:
-              try:
-                list_builder_add_1267(this__50.out__236, ']')
-              except Exception5:
-                s_1272.break_()
-              s_1271.break_()
-        raise NoResultException7()
-      this__50.pushRegex(adjusted__274)
-    return return__121
-  def adjustCodeSet(this__51, codeSet__277, regexRefs__278):
-    return__122 = codeSet__277
-    return return__122
-  def pushCodeSetItem(this__52, codePart__281):
-    return__123 = None
+              break
+          try:
+            list_builder_add_1215(this__39.out__227, ']')
+            s__1226_1228.break_()
+          except Exception9:
+            pass
+        raise NoResultException11()
+      this__39.pushRegex__232(adjusted__265)
+    return return__110
+  def adjustCodeSet__267(this__40, codeSet__268: 'CodeSet', regexRefs__269: 'RegexRefs__19') -> 'Regex':
+    return__111: 'Regex'
+    return__111 = codeSet__268
+    return return__111
+  def pushCodeSetItem__271(this__41, codePart__272: 'CodePart') -> 'None':
+    return__112: 'None'
+    return__112 = None
+    t_707: 'bool'
+    t_708: 'CodePoints'
+    t_711: 'bool'
+    t_712: 'CodeRange'
+    t_715: 'bool'
+    t_716: 'SpecialSet'
     try:
-      cast_by_type4(codePart__281, CodePoints__14)
-      t_734 = True
-    except Exception5:
-      t_734 = False
-    with Label6() as s_1276:
-      if t_734:
+      cast_by_type8(codePart__272, CodePoints)
+      t_707 = True
+    except Exception9:
+      t_707 = False
+    with Label10() as s__1232_1233:
+      if t_707:
         try:
-          t_735 = cast_by_type4(codePart__281, CodePoints__14)
-        except Exception5:
-          s_1276.break_()
-        this__52.pushCodePoints(t_735, True)
+          t_708 = cast_by_type8(codePart__272, CodePoints)
+        except Exception9:
+          s__1232_1233.break_()
+        this__41.pushCodePoints__251(t_708, True)
       else:
         try:
-          cast_by_type4(codePart__281, CodeRange__24)
-          t_738 = True
-        except Exception5:
-          t_738 = False
-        if t_738:
+          cast_by_type8(codePart__272, CodeRange)
+          t_711 = True
+        except Exception9:
+          t_711 = False
+        if t_711:
           try:
-            t_739 = cast_by_type4(codePart__281, CodeRange__24)
-          except Exception5:
-            s_1276.break_()
-          this__52.pushCodeRangeUnwrapped(t_739)
+            t_712 = cast_by_type8(codePart__272, CodeRange)
+          except Exception9:
+            s__1232_1233.break_()
+          this__41.pushCodeRangeUnwrapped__259(t_712)
         else:
           try:
-            cast_by_type4(codePart__281, SpecialSet__20)
-            t_742 = True
-          except Exception5:
-            t_742 = False
-          if t_742:
+            cast_by_type8(codePart__272, SpecialSet)
+            t_715 = True
+          except Exception9:
+            t_715 = False
+          if t_715:
             try:
-              t_743 = cast_by_type4(codePart__281, SpecialSet__20)
-            except Exception5:
-              s_1276.break_()
-            this__52.pushRegex(t_743)
-      return return__123
-    raise NoResultException7()
-  def pushOr(this__53, or__284):
-    return__124 = None
-    t_1096 = or__284.items
-    t_1104 = not t_1096
-    t_1103 = bool_not_1270(t_1104)
-    with Label6() as s_1278:
-      if t_1103:
-        with Label6() as s_1279:
+              t_716 = cast_by_type8(codePart__272, SpecialSet)
+            except Exception9:
+              s__1232_1233.break_()
+            this__41.pushRegex__232(t_716)
+      return return__112
+    raise NoResultException11()
+  def pushOr__274(this__42, or__275: 'Or') -> 'None':
+    return__113: 'None'
+    t_1067: 'Tuple7[Regex, ...]'
+    t_1068: 'Tuple7[Regex, ...]'
+    t_1070: 'int'
+    t_1071: 'Tuple7[Regex, ...]'
+    return__113 = None
+    t_697: 'Regex'
+    t_702: 'Regex'
+    t_1066: 'Tuple7[Regex, ...]' = or__275.items
+    t_1073: 'bool' = not t_1066
+    with Label10() as s__1234_1237:
+      if bool_not_1214(t_1073):
+        with Label10() as s__1235_1238:
           try:
-            list_builder_add_1267(this__53.out__236, '(?:')
-            t_1101 = or__284.items
-            t_722 = list_get_1275(t_1101, 0)
-          except Exception5:
-            s_1279.break_()
-          this__53.pushRegex(t_722)
-          i__286 = 1
+            list_builder_add_1215(this__42.out__227, '(?:')
+            t_1071 = or__275.items
+            t_697 = list_get_1231(t_1071, 0)
+          except Exception9:
+            s__1235_1238.break_()
+          this__42.pushRegex__232(t_697)
+          i__277: 'int' = 1
           while True:
-            t_1097 = or__284.items
-            t_1100 = len_1273(t_1097)
-            try:
-              t_726 = generic_lt_1274(i__286, t_1100)
-            except Exception5:
-              break
-            if t_726:
+            t_1067 = or__275.items
+            t_1070 = len_1230(t_1067)
+            if i__277 < t_1070:
               try:
-                list_builder_add_1267(this__53.out__236, '|')
-                t_1098 = or__284.items
-                t_729 = list_get_1275(t_1098, i__286)
-              except Exception5:
+                list_builder_add_1215(this__42.out__227, '|')
+                t_1068 = or__275.items
+                t_702 = list_get_1231(t_1068, i__277)
+              except Exception9:
                 break
-              this__53.pushRegex(t_729)
-              t_727 = i__286 + 1
-              i__286 = t_727
+              this__42.pushRegex__232(t_702)
+              i__277 = i__277 + 1
             else:
               try:
-                list_builder_add_1267(this__53.out__236, ')')
-              except Exception5:
-                s_1279.break_()
-              s_1278.break_()
-        raise NoResultException7()
-    return return__124
-  def pushRepeat(this__54, repeat__288):
-    return__125 = None
-    with Label6() as s_1280:
+                list_builder_add_1215(this__42.out__227, ')')
+              except Exception9:
+                s__1235_1238.break_()
+              s__1234_1237.break_()
+        raise NoResultException11()
+    return return__113
+  def pushRepeat__278(this__43, repeat__279: 'Repeat') -> 'None':
+    return__114: 'None'
+    t_1059: 'Regex'
+    t_1061: 'int'
+    t_1062: 'str'
+    t_1063: 'str'
+    t_1064: 'bool'
+    return__114 = None
+    t_676: 'Union4[int, None]'
+    t_677: 'bool'
+    t_679: 'bool'
+    t_681: 'bool'
+    t_684: 'List1[str]'
+    t_685: 'int'
+    t_687: 'List1[str]'
+    with Label10() as s__1239_1240:
+      min__281: 'int'
       try:
-        list_builder_add_1267(this__54.out__236, '(?:')
-        t_1089 = repeat__288.item
-        this__54.pushRegex(t_1089)
-        list_builder_add_1267(this__54.out__236, ')')
-        t_1091 = repeat__288.min
-        min__290 = t_1091
-        t_700 = repeat__288.max
-      except Exception5:
-        s_1280.break_()
-      max__291 = t_700
-      if generic_eq_1266(min__290, 0):
-        t_701 = generic_eq_1266(max__291, 1)
+        list_builder_add_1215(this__43.out__227, '(?:')
+        t_1059 = repeat__279.item
+        this__43.pushRegex__232(t_1059)
+        list_builder_add_1215(this__43.out__227, ')')
+        t_1061 = repeat__279.min
+        min__281 = t_1061
+        t_676 = repeat__279.max
+      except Exception9:
+        s__1239_1240.break_()
+      max__282: 'Union4[int, None]' = t_676
+      if min__281 == 0:
+        t_677 = max__282 == 1
       else:
-        t_701 = False
-      if t_701:
+        t_677 = False
+      if t_677:
         try:
-          list_builder_add_1267(this__54.out__236, '?')
-        except Exception5:
-          s_1280.break_()
+          list_builder_add_1215(this__43.out__227, '?')
+        except Exception9:
+          s__1239_1240.break_()
       else:
-        if generic_eq_1266(min__290, 0):
-          t_703 = generic_eq_1266(max__291, None)
+        if min__281 == 0:
+          t_679 = max__282 == None
         else:
-          t_703 = False
-        if t_703:
+          t_679 = False
+        if t_679:
           try:
-            list_builder_add_1267(this__54.out__236, '*')
-          except Exception5:
-            s_1280.break_()
+            list_builder_add_1215(this__43.out__227, '*')
+          except Exception9:
+            s__1239_1240.break_()
         else:
-          if generic_eq_1266(min__290, 1):
-            t_705 = generic_eq_1266(max__291, None)
+          if min__281 == 1:
+            t_681 = max__282 == None
           else:
-            t_705 = False
-          if t_705:
+            t_681 = False
+          if t_681:
             try:
-              list_builder_add_1267(this__54.out__236, '+')
-            except Exception5:
-              s_1280.break_()
+              list_builder_add_1215(this__43.out__227, '+')
+            except Exception9:
+              s__1239_1240.break_()
           else:
-            t_708 = this__54.out__236
-            t_1092 = int_to_string_1240(min__290)
+            t_684 = this__43.out__227
+            t_1062 = int_to_string_1241(min__281)
             try:
-              list_builder_add_1267(t_708, str_cat_1241('{', t_1092))
-            except Exception5:
-              s_1280.break_()
-            if generic_not_eq_1281(min__290, max__291):
+              list_builder_add_1215(t_684, str_cat_1212('{', t_1062))
+            except Exception9:
+              s__1239_1240.break_()
+            if min__281 != max__282:
               try:
-                list_builder_add_1267(this__54.out__236, ',')
-              except Exception5:
-                s_1280.break_()
-              if generic_not_eq_1281(max__291, None):
-                t_711 = this__54.out__236
+                list_builder_add_1215(this__43.out__227, ',')
+              except Exception9:
+                s__1239_1240.break_()
+              if max__282 != None:
+                t_687 = this__43.out__227
                 try:
-                  t_709 = cast_by_test9(max__291, isinstance_int8)
-                  t_1093 = int_to_string_1240(t_709)
-                  list_builder_add_1267(t_711, t_1093)
-                except Exception5:
-                  s_1280.break_()
+                  t_685 = cast_by_test13(max__282, isinstance_int12)
+                  t_1063 = int_to_string_1241(t_685)
+                  list_builder_add_1215(t_687, t_1063)
+                except Exception9:
+                  s__1239_1240.break_()
             try:
-              list_builder_add_1267(this__54.out__236, '}')
-            except Exception5:
-              s_1280.break_()
-      t_1094 = repeat__288.reluctant
-      if t_1094:
+              list_builder_add_1215(this__43.out__227, '}')
+            except Exception9:
+              s__1239_1240.break_()
+      t_1064 = repeat__279.reluctant
+      if t_1064:
         try:
-          list_builder_add_1267(this__54.out__236, '?')
-        except Exception5:
-          s_1280.break_()
-      return return__125
-    raise NoResultException7()
-  def pushSequence(this__55, sequence__293):
-    return__126 = None
-    i__295 = 0
-    with Label6() as s_1282:
+          list_builder_add_1215(this__43.out__227, '?')
+        except Exception9:
+          s__1239_1240.break_()
+      return return__114
+    raise NoResultException11()
+  def pushSequence__283(this__44, sequence__284: 'Sequence') -> 'None':
+    return__115: 'None'
+    t_1054: 'Tuple7[Regex, ...]'
+    t_1055: 'Tuple7[Regex, ...]'
+    t_1057: 'int'
+    return__115 = None
+    t_670: 'Regex'
+    i__286: 'int' = 0
+    with Label10() as s__1242_1243:
       while True:
-        t_1084 = sequence__293.items
-        t_1087 = len_1273(t_1084)
-        try:
-          t_691 = generic_lt_1274(i__295, t_1087)
-        except Exception5:
-          break
-        if t_691:
-          t_1085 = sequence__293.items
+        t_1054 = sequence__284.items
+        t_1057 = len_1230(t_1054)
+        if i__286 < t_1057:
+          t_1055 = sequence__284.items
           try:
-            t_694 = list_get_1275(t_1085, i__295)
-          except Exception5:
+            t_670 = list_get_1231(t_1055, i__286)
+          except Exception9:
             break
-          this__55.pushRegex(t_694)
-          t_692 = i__295 + 1
-          i__295 = t_692
+          this__44.pushRegex__232(t_670)
+          i__286 = i__286 + 1
         else:
-          s_1282.break_()
-      raise NoResultException7()
-    return return__126
-  def maxCode(this__56, codePart__297):
+          s__1242_1243.break_()
+      raise NoResultException11()
+    return return__115
+  def max_code(this__45, codePart__288: 'CodePart') -> 'Union4[int, None]':
+    return__116: 'Union4[int, None]'
+    t_1041: 'Any6'
+    t_1042: 'Any6'
+    t_1043: 'Any6'
+    t_1044: 'str'
+    t_1045: 'bool'
+    t_1046: 'Any6'
+    t_1047: 'bool'
+    t_1048: 'int'
+    t_1049: 'Any6'
+    t_1050: 'Union4[int, None]'
+    t_1051: 'Union4[int, None]'
+    t_1052: 'Union4[int, None]'
+    t_1053: 'Union4[int, None]'
+    t_643: 'bool'
+    t_644: 'CodePoints'
+    t_651: 'Union4[int, None]'
+    t_652: 'Union4[int, None]'
+    t_656: 'bool'
+    t_657: 'CodeRange'
+    t_666: 'Union4[int, None]'
     try:
-      cast_by_type4(codePart__297, CodePoints__14)
-      t_663 = True
-    except Exception5:
-      t_663 = False
-    with Label6() as s_1283:
-      if t_663:
+      cast_by_type8(codePart__288, CodePoints)
+      t_643 = True
+    except Exception9:
+      t_643 = False
+    with Label10() as s__1244_1245:
+      if t_643:
         try:
-          t_664 = cast_by_type4(codePart__297, CodePoints__14)
-        except Exception5:
-          s_1283.break_()
-        t_1073 = t_664.value
-        value__299 = t_1073
-        t_1074 = not value__299
-        if t_1074:
-          t_674 = None
+          t_644 = cast_by_type8(codePart__288, CodePoints)
+        except Exception9:
+          s__1244_1245.break_()
+        t_1044 = t_644.value
+        value__290: 'str' = t_1044
+        t_1045 = not value__290
+        if t_1045:
+          t_652 = None
         else:
-          max__300 = 0
-          t_1075 = string_code_points_1239(value__299)
-          slice__301 = t_1075
+          max__291: 'int' = 0
+          t_1046 = string_code_points_1225(value__290)
+          slice__292: 'Any6' = t_1046
           while True:
-            t_1076 = slice__301.is_empty
-            t_1079 = bool_not_1270(t_1076)
-            if t_1079:
-              t_1077 = slice__301.read()
-              next__302 = t_1077
-              try:
-                t_672 = generic_gt_eq_1284(next__302, max__300)
-              except Exception5:
-                s_1283.break_()
-              if t_672:
-                max__300 = next__302
-              t_1078 = slice__301.advance(1)
-              slice__301 = t_1078
+            t_1047 = slice__292.is_empty
+            if bool_not_1214(t_1047):
+              t_1048 = slice__292.read()
+              next__293: 'int' = t_1048
+              if next__293 > max__291:
+                max__291 = next__293
+              t_1049 = slice__292.advance(1)
+              slice__292 = t_1049
             else:
               break
-          t_673 = max__300
-          t_674 = t_673
-        t_688 = t_674
+          t_651 = max__291
+          t_652 = t_651
+        t_666 = t_652
       else:
         try:
-          cast_by_type4(codePart__297, CodeRange__24)
-          t_678 = True
-        except Exception5:
-          t_678 = False
-        if t_678:
+          cast_by_type8(codePart__288, CodeRange)
+          t_656 = True
+        except Exception9:
+          t_656 = False
+        if t_656:
           try:
-            t_679 = cast_by_type4(codePart__297, CodeRange__24)
-          except Exception5:
-            s_1283.break_()
-          t_1080 = t_679.max
-          t_688 = t_1080
-        elif generic_eq_1266(codePart__297, Digit):
-          t_1070 = string_code_points_1239('9')
-          t_1081 = t_1070.read()
-          t_688 = t_1081
-        elif generic_eq_1266(codePart__297, Space):
-          t_1071 = string_code_points_1239(' ')
-          t_1082 = t_1071.read()
-          t_688 = t_1082
-        elif generic_eq_1266(codePart__297, Word):
-          t_1072 = string_code_points_1239('z')
-          t_1083 = t_1072.read()
-          t_688 = t_1083
+            t_657 = cast_by_type8(codePart__288, CodeRange)
+          except Exception9:
+            s__1244_1245.break_()
+          t_1050 = t_657.max
+          t_666 = t_1050
+        elif generic_eq_1222(codePart__288, digit):
+          t_1041 = string_code_points_1225('9')
+          t_1051 = t_1041.read()
+          t_666 = t_1051
+        elif generic_eq_1222(codePart__288, space):
+          t_1042 = string_code_points_1225(' ')
+          t_1052 = t_1042.read()
+          t_666 = t_1052
+        elif generic_eq_1222(codePart__288, word):
+          t_1043 = string_code_points_1225('z')
+          t_1053 = t_1043.read()
+          t_666 = t_1053
         else:
-          t_688 = None
+          t_666 = None
       try:
-        return__127 = t_688
-        return return__127
-      except Exception5:
+        return__116 = t_666
+        return return__116
+      except Exception9:
         pass
-    raise NoResultException7()
-  def constructor__303(this__109, out = ...):
-    out__304 = out
-    return__111 = None
-    if out__304 is ...:
-      t_1066 = list_1285()
-      out__304 = t_1066
-    this__109.out__236 = out__304
-    return return__111
-  def __init__(this__109, out = ...):
-    out__304 = out
-    this__109.constructor__303(out__304)
-  out = property(None, None)
-def Begin__146(*args_1286):
-  return Begin__16(*args_1286)
-class Begin__16(Special__15, TemperObject1):
-  def constructor__147(this__64):
+    raise NoResultException11()
+  def constructor__294(this__98, out: 'List1[str]' = ...) -> Any6:
+    out__295: 'List1[str]' = out
+    return__100: 'None'
+    t_1037: 'List1[str]'
+    return__100 = None
+    if out__295 is ...:
+      t_1037 = list_1210()
+      out__295 = t_1037
+    this__98.out__227 = out__295
+    return return__100
+  def __init__(this__98, out: 'List1[str]' = ...) -> None:
+    out__295: 'List1[str]' = out
+    this__98.constructor__294(out__295)
+class Begin__12(Special):
+  __slots__ = ()
+  def constructor__137(this__54) -> Any6:
+    return__55: 'None'
+    return__55 = None
+    return return__55
+  def __init__(this__54) -> None:
+    this__54.constructor__137()
+t_1202: 'Begin__12' = Begin__12()
+begin: 'Begin__12' = t_1202
+class Dot__13(Special):
+  __slots__ = ()
+  def constructor__138(this__56) -> Any6:
+    return__57: 'None'
+    return__57 = None
+    return return__57
+  def __init__(this__56) -> None:
+    this__56.constructor__138()
+t_1203: 'Dot__13' = Dot__13()
+dot: 'Dot__13' = t_1203
+class End__14(Special):
+  __slots__ = ()
+  def constructor__139(this__58) -> Any6:
+    return__59: 'None'
+    return__59 = None
+    return return__59
+  def __init__(this__58) -> None:
+    this__58.constructor__139()
+t_1204: 'End__14' = End__14()
+end: 'End__14' = t_1204
+class WordBoundary__15(Special):
+  __slots__ = ()
+  def constructor__140(this__60) -> Any6:
+    return__61: 'None'
+    return__61 = None
+    return return__61
+  def __init__(this__60) -> None:
+    this__60.constructor__140()
+t_1205: 'WordBoundary__15' = WordBoundary__15()
+word_boundary: 'WordBoundary__15' = t_1205
+class Digit__16(SpecialSet):
+  __slots__ = ()
+  def constructor__141(this__62) -> Any6:
+    return__63: 'None'
+    return__63 = None
+    return return__63
+  def __init__(this__62) -> None:
+    this__62.constructor__141()
+t_1206: 'Digit__16' = Digit__16()
+digit: 'Digit__16' = t_1206
+class Space__17(SpecialSet):
+  __slots__ = ()
+  def constructor__142(this__64) -> Any6:
+    return__65: 'None'
     return__65 = None
     return return__65
-  def __init__(this__64):
-    this__64.constructor__147()
-t_1231 = Begin__146()
-Begin = t_1231
-def Dot__148(*args_1287):
-  return Dot__17(*args_1287)
-class Dot__17(Special__15, TemperObject1):
-  def constructor__149(this__66):
+  def __init__(this__64) -> None:
+    this__64.constructor__142()
+t_1207: 'Space__17' = Space__17()
+space: 'Space__17' = t_1207
+class Word__18(SpecialSet):
+  __slots__ = ()
+  def constructor__143(this__66) -> Any6:
+    return__67: 'None'
     return__67 = None
     return return__67
-  def __init__(this__66):
-    this__66.constructor__149()
-t_1232 = Dot__148()
-Dot = t_1232
-def End__150(*args_1288):
-  return End__18(*args_1288)
-class End__18(Special__15, TemperObject1):
-  def constructor__151(this__68):
-    return__69 = None
-    return return__69
-  def __init__(this__68):
-    this__68.constructor__151()
-t_1233 = End__150()
-End = t_1233
-def WordBoundary__152(*args_1289):
-  return WordBoundary__19(*args_1289)
-class WordBoundary__19(Special__15, TemperObject1):
-  def constructor__153(this__70):
-    return__71 = None
-    return return__71
-  def __init__(this__70):
-    this__70.constructor__153()
-t_1234 = WordBoundary__152()
-WordBoundary = t_1234
-def Digit__154(*args_1290):
-  return Digit__21(*args_1290)
-class Digit__21(SpecialSet__20, TemperObject1):
-  def constructor__155(this__72):
-    return__73 = None
-    return return__73
-  def __init__(this__72):
-    this__72.constructor__155()
-t_1235 = Digit__154()
-Digit = t_1235
-def Space__156(*args_1291):
-  return Space__22(*args_1291)
-class Space__22(SpecialSet__20, TemperObject1):
-  def constructor__157(this__74):
-    return__75 = None
-    return return__75
-  def __init__(this__74):
-    this__74.constructor__157()
-t_1236 = Space__156()
-Space = t_1236
-def Word__158(*args_1292):
-  return Word__23(*args_1292)
-class Word__23(SpecialSet__20, TemperObject1):
-  def constructor__159(this__76):
-    return__77 = None
-    return return__77
-  def __init__(this__76):
-    this__76.constructor__159()
-t_1237 = Word__158()
-Word = t_1237
-def entire(item__182):
-  global Begin, End, Sequence
-  t_1197 = Sequence((Begin, item__182, End))
-  return__89 = t_1197
-  return return__89
-def one_or_more(item__184, reluctant = ...):
-  reluctant__185 = reluctant
-  global Repeat
-  if reluctant__185 is ...:
-    reluctant__185 = False
-  t_1195 = Repeat(item__184, 1, None, reluctant__185)
-  return__90 = t_1195
-  return return__90
-def optional(item__187, reluctant = ...):
-  reluctant__188 = reluctant
-  global Repeat
-  if reluctant__188 is ...:
-    reluctant__188 = False
-  t_1192 = Repeat(item__187, 0, 1, reluctant__188)
-  return__91 = t_1192
-  return return__91
-t_1238 = RegexRefs__128()
-regexRefs__210 = t_1238
-return__894 = RegexFormatter__129
-export = return__894
+  def __init__(this__66) -> None:
+    this__66.constructor__143()
+t_1208: 'Word__18' = Word__18()
+word: 'Word__18' = t_1208
+def entire(item__166: 'Regex') -> 'Regex':
+  global begin, end
+  return__79: 'Regex'
+  t_1165: 'Regex' = Sequence((begin, item__166, end))
+  return__79 = t_1165
+  return return__79
+def one_or_more(item__168: 'Regex', reluctant: 'bool' = ...) -> 'Repeat':
+  reluctant__169: 'bool' = reluctant
+  return__80: 'Repeat'
+  if reluctant__169 is ...:
+    reluctant__169 = False
+  t_1163: 'Repeat' = Repeat(item__168, 1, None, reluctant__169)
+  return__80 = t_1163
+  return return__80
+def optional(item__171: 'Regex', reluctant: 'bool' = ...) -> 'Repeat':
+  reluctant__172: 'bool' = reluctant
+  return__81: 'Repeat'
+  if reluctant__172 is ...:
+    reluctant__172 = False
+  t_1160: 'Repeat' = Repeat(item__171, 0, 1, reluctant__172)
+  return__81 = t_1160
+  return return__81
+t_1209: 'RegexRefs__19' = RegexRefs__19()
+regexRefs__191: 'RegexRefs__19' = t_1209
+return__865: 'Any6' = ('<<lang.temper.value.TypeTag<out kotlin.Any>: Type, lang.temper.value.Value<*>: RegexFormatter__29: Type>>', NotImplemented)[1]
+export = return__865
```

### Comparing `temper_std-0.0.3/temper_std/regex.py.map` & `temper_std-0.0.4/temper_std/regex.py.map`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7636704119850187%*

 * *Differences: {"'mappings'": "'A,wB,Y,I,a,E,Y,I,a,E,K,I,O,E,iB,I,mB,E,c,I,gB,E,Y,I,c,E,S,I,c,E,U,I,e,E,gB,I,qB,E,kB,I,uB,E,Q,I,a,E,Q,I,a,E,a,I,kB,E,O,I;A,mB,K,I,M,E,Q,I,S,E,Q,I,S,E,G,I,I,E,K,I,M,E,I,I;A,qB,S,I,U,E,G,I,Q,E,I,I;A,8B,gC,I,qC,E,6B,I,kC,E,4B,I,iC,E,+B,I,oC,E,iC,I,sC,E,4B,I;AA4B4B,MAAA6C,KAAA,CAAA7C,aAuCzB,EAAA;AAvCyB,WAuCzB,EAAA,AAvCyB,GAuCzB;AA9BM,cAAqD,CAAA,AAA3C8C,OAA2C,IAAA,AAAzC,gBAAa,CAAA;AAAb,IAAAC,UAAA;AAAgB,IAAAC,MAAuB,CAAA,AAAvB,gBAAuB,EAAA,AAAnB,CAAAC,aAAa,CAACH,OAAI,CAAC;AAAvC,IAAAC,UAAA,EAAgB,CAA […]*

```diff
@@ -1,289 +1,255 @@
 {
     "file": "OUTPUT_ROOT/temper-std/py/temper_std/regex.py",
-    "mappings": "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",
+    "mappings": "A,wB,Y,I,a,E,Y,I,a,E,K,I,O,E,iB,I,mB,E,c,I,gB,E,Y,I,c,E,S,I,c,E,U,I,e,E,gB,I,qB,E,kB,I,uB,E,Q,I,a,E,Q,I,a,E,a,I,kB,E,O,I;A,mB,K,I,M,E,Q,I,S,E,Q,I,S,E,G,I,I,E,K,I,M,E,I,I;A,qB,S,I,U,E,G,I,Q,E,I,I;A,8B,gC,I,qC,E,6B,I,kC,E,4B,I,iC,E,+B,I,oC,E,iC,I,sC,E,4B,I;AA4B4B,MAAA6C,KAAA,CAAA7C,aAuCzB,EAAA;AAvCyB,WAuCzB,EAAA,AAvCyB,GAuCzB;AA9BM,cAAqD,CAAA,AAA3C8C,OAA2C,IAAA,AAAzC,gBAAa,CAAA;AAAb,IAAAC,UAAA;AAAgB,IAAAC,MAAuB,CAAA,AAAvB,gBAAuB,EAAA,AAAnB,CAAAC,aAAa,CAACH,OAAI,CAAC;AAAvC,IAAAC,UAAA,EAAgB,CAAAC,MAAuB;AAAE,UAAA,AAAzC,CAAAD;AAQZ,WAAuD,CAAA,AAAjDD,OAAA,EAAAI,SAAI,CAAE,MAA2C,IAAA,AAAlC,OAAO,CAAA;AAAP,IAAAH,UAAA;AAAU,IAAAI,MAAU,CAAA,AAAV,gBAAU,EAAA,AAAV,CAAAL,OAAQ,CAAA,AAAR,QAAQ,EAAE;AAAV,IAAAM,MAAsB,CAAA,AAAtB,OAAsB,EAAA,AAAtB,CAAAD,MAAU,CAAA,AAAV,KAAgB,CAACD,SAAI,CAAC;AAAhC,IAAAH,UAAA,EAAU,CAAAK,MAAsB;AAAE,UAAA,AAAlC,CAAAL;AAcrB,UAEN,CAAA,AAFWD,QAAA,EAAAI,SAAI,CAAE,MAEjB,IAAA,AAF0B,2CAA6B,CAAA;AAA7B,IAAAH,UAAA;AACzB,IAAAM,KAAqB,CAAA,AAArB,sBAAqB;AAArB,IAAAC,MAAU,CAAA,AAAV,gBAAU,EAAA,AAAV,CAAAR,QAAQ,CAAA,AAAR,QAAQ,EAAE;AAAV,IAAAO,KAAA,EAAW,AAAX,CAAAC,MAAU,CAAA,AAAV,IAAe,CAACJ,SAAI,CAAC;AADI,IAAAH,UAAA,EACzB,CAAAM,KAAqB;AACtB,UAAA,AAF0B,CAAAN;AAIpB,aAIN,CAAA,AAHCD,QAAA,EAAAI,SAAI,CAAE,MAAM,CAAE,CAAAK,WAAM,CAAE,wCAGvB,IAAA,AAFE,MAAM,CAAA;AAAN,IAAAR,UAAA;AACD,IAAAS,MAAU,CAAA,AAAV,gBAAU,EAAA,AAAV,CAAAV,QAAQ,CAAA,AAAR,QAAQ,EAAE;AAAV,IAAAW,MAAgC,CAAA,AAAhC,MAAgC,EAAA,AAAhC,CAAAD,MAAU,CAAA,AAAV,OAAkB,CAACN,SAAI,CAAE,CAAAK,WAAM,CAAC;AAD/B,IAAAR,UAAA,EACD,CAAAU,MAAgC;AACjC,UAAA,AAFE,CAAAV;AAiCQ,MAAAW,OAAA,CAAAb,KAEiB,EAAA;AADrB,EAAAc,SAAI,CAAE;AACI,EAAAC,SAAI,CAAE,QAAK;AAFjB,WAEiB,EAAA,AAFjB,EACJ,WAAY,CACF,YAAW,CAAA;AAFK,MAAAC,gBAAA,CAAAf,QAAA,CAC1B,CAAAa,SAAI,CAAE,MAAM,CACF,CAAAC,SAAI,CAAE,QAAK,AAFK,IAAA,A,C,I;AAAA,IAAAb,UAEL,CAAA,AAFK;AAEL,IAAAA,UAAA,OAAA;AADrB,IAAAD,QAAA,CAAAa,SAAI,EAAA,AAAJ,CAAAA;AACU,IAAAb,QAAA,CAAAc,SAAI,EAAA,AAAJ,CAAAA;AAAW,UAAA,AAFK,CAAAb,UAEL;AAFjB,KAAsB,UAAAD,QAAA,CAC1B,CAAAa,SAAI,CAAE,MAAM,CACF,CAAAC,SAAI,CAAE,QAAK,AAFK;AAAA,IAAAd,QAAA,CAAAe,gBAAA,CAC1BF,SAAY,CACF,CAAAC,SAAW,CAAA;AADrB;AAAA,WAAAd,SAAA;AAAA,IAAAC,WAAM,OAAM;AAAZ,IAAAA,WAAA,GAAAD,SAAA,CAAAa;AAAA,WAAAZ,WAAM;AACI;AAAA,WAAAD,SAAA;AAAA,IAAAC,WAAM,SAAK;AAAX,IAAAA,WAAA,GAAAD,SAAA,CAAAc;AAAA,WAAAb,WAAM;AAaG,MAAAe,QAAA,CAAAjB,KAAuB,EAAA;AAAvB,WAAuB,EAAA,AAAvB;AAef,MAAAkB,UAAA,CAAAD,QACS,EAAA;AAAb,EAAAE,UAAK,CAAE,MAAM;AADT,WACS,EAAA,AADT,EACJ,YAAa,EAAA;AADmB,MAAAH,gBAAA,CAAAf,QAAA,CAChC,CAAAkB,UAAK,CAAE,MAAM,AADmB,IAAA,A,C,I;AAAA,IAAAjB,UACnB,CAAA,AADmB;AACnB,IAAAA,UAAA,OAAA;AAAb,IAAAD,QAAA,CAAAkB,UAAK,EAAA,AAAL,CAAAA;AAAa,UAAA,AADmB,CAAAjB,UACnB;AADT,KAA4B,UAAAD,QAAA,CAChC,CAAAkB,UAAK,CAAE,MAAM,AADmB;AAAA,IAAAlB,QAAA,CAAAe,gBAAA,CAChCG,UAAa,CAAA;AAAb;AAAA,YAAAlB,SAAA;AAAA,IAAAC,WAAO,OAAM;AAAb,IAAAA,WAAA,GAAAD,SAAA,CAAAkB;AAAA,WAAAjB,WAAO;AA4BY,MAAAkB,OAAA,CAAApB,KAAsB,EAAA;AAAtB,WAAsB,EAAA,AAAtB;AAYA,MAAAqB,UAAA,CAAAJ,QAAsC,CAAA,AAAtC,CAAAG,OAAsC,EAAA;AAAtC,WAAsC,EAAA,AAAtC;AAgBf,MAAAE,SAAA,CAAAL,QAEI,EAAA;AADR,EAAAM,QAAG,CAAE;AACL,EAAAC,QAAG,CAAE,MAAG;AAFJ,WAEI,EAAA,AAFJ,EACJ,UAAQ,CACR,WAAQ,CAAA;AAFuB,MAAAR,gBAAA,CAAAf,QAAA,CAC/B,CAAAsB,QAAG,CAAE,MAAG,CACR,CAAAC,QAAG,CAAE,MAAG,AAFuB,IAAA,A,C,I;AAAA,IAAAtB,UAEvB,CAAA,AAFuB;AAEvB,IAAAA,UAAA,OAAA;AADR,IAAAD,QAAA,CAAAsB,QAAG,EAAA,AAAH,CAAAA;AACA,IAAAtB,QAAA,CAAAuB,QAAG,EAAA,AAAH,CAAAA;AAAQ,UAAA,AAFuB,CAAAtB,UAEvB;AAFJ,KAA2B,UAAAD,QAAA,CAC/B,CAAAsB,QAAG,CAAE,MAAG,CACR,CAAAC,QAAG,CAAE,MAAG,AAFuB;AAAA,IAAAvB,QAAA,CAAAe,gBAAA,CAC/BO,QAAQ,CACR,CAAAC,QAAQ,CAAA;AADR;AAAA,UAAAvB,SAAA;AAAA,IAAAC,WAAK,OAAG;AAAR,IAAAA,WAAA,GAAAD,SAAA,CAAAsB;AAAA,WAAArB,WAAK;AACL;AAAA,UAAAD,SAAA;AAAA,IAAAC,WAAK,OAAG;AAAR,IAAAA,WAAA,GAAAD,SAAA,CAAAuB;AAAA,WAAAtB,WAAK;AAgBD,MAAAuB,OAAA,CAAAzB,KAEoB,EAAA;AADxB,EAAA0B,UAAK,CAAE;AACP,EAAAC,YAAO,CAAE,OAAe;AAFpB,WAEoB,EAAA,AAFpB,EACJ,YAAqB,CACrB,eAAwB,CAAA;AAFE,MAAAX,gBAAA,CAAAf,QAAA,CAC1B,CAAAyB,UAAK,CAAE,wBAAc,CACrB,CAAAC,OAAO,CAAE,OAAO,EAAA,AAAhB,IAAwB,AAFE,IAAA,A,C,I;AAE1B,IAAAA,YAAO,CAAE,OAAO,EAAA,AAAhB,CAAAA,OAAO;AAFmB,IAAAzB,UAEF,CAAA,AAFE;AAEF,IAAAA,UAAA,OAAA;AADxB,MACmB,AAAnB,CAAAyB,YAAO,AAAP,GAAmB,IAAK,CAAA;AAAxB,MAAAA,YAAO,EAAY,MAAK;AADxB,IAAA1B,QAAA,CAAAyB,UAAK,EAAA,AAAL,CAAAA;AACA,IAAAzB,QAAA,CAAA0B,YAAO,EAAA,AAAP,CAAAA;AAAwB,UAAA,AAFE,CAAAzB,UAEF;AAFpB,KAAsB,UAAAD,QAAA,CAC1B,CAAAyB,UAAK,CAAE,wBAAc,CACrB,CAAAC,OAAO,CAAE,OAAO,EAAA,AAAhB,IAAwB,AAFE;AAE1B,IAAAA,YAAO,CAAE,OAAO,EAAA,AAAhB,CAAAA,OAAO;AAFmB,IAAA1B,QAAA,CAAAe,gBAAA,CAC1BU,UAAqB,CACrB,CAAAC,YAAwB,CAAA;AADxB;AAAA,YAAA1B,SAAA;AAAA,IAAAC,WAAO,yBAAc;AAArB,IAAAA,WAAA,GAAAD,SAAA,CAAAyB;AAAA,WAAAxB,WAAO;AACP;AAAA,cAAAD,SAAA;AAAA,IAAAC,WAAS,QAAO;AAAhB,IAAAA,WAAA,GAAAD,SAAA,CAAA0B;AAAA,WAAAzB,WAAS;AASL,MAAA0B,EAAA,CAAA5B,KACwB,EAAA;AAAlB,EAAA0B,UAAK,CAAE,qBAAW;AADxB,WACwB,EAAA,AADxB,EACM,YAAkB,EAAA;AADP,MAAAV,gBAAA,CAAAf,QAAA,CACX,CAAAyB,UAAK,CAAE,qBAAW,AADP,IAAA,A,C,I;AAAA,IAAAxB,UACO,CAAA,AADP;AACO,IAAAA,UAAA,OAAA;AAAlB,IAAAD,QAAA,CAAAyB,UAAK,EAAA,AAAL,CAAAA;AAAkB,UAAA,AADP,CAAAxB,UACO;AADxB,KAAiB,UAAAD,QAAA,CACX,CAAAyB,UAAK,CAAE,qBAAW,AADP;AAAA,IAAAzB,QAAA,CAAAe,gBAAA,CACXU,UAAkB,CAAA;AAAlB;AAAA,YAAAzB,SAAA;AAAA,IAAAC,WAAO,sBAAW;AAAlB,IAAAA,WAAA,GAAAD,SAAA,CAAAyB;AAAA,WAAAxB,WAAO;AAqBb,MAAA2B,MAAA,CAAA7B,KAIsB,EAAA;AAHhB,EAAAe,SAAI,CAAE;AAChB,EAAAQ,QAAG,CAAE;AACL,EAAAC,QAAG,CAAE;AACL,EAAAM,cAAS,CAAE,OAAe;AAJtB,WAIsB,EAAA,AAJtB,EACM,WAAW,CACrB,WAAQ,CACR,WAAe,CACf,iBAA0B,CAAA;AAJD,MAAAd,gBAAA,CAAAf,QAAA,CACf,CAAAc,SAAI,CAAE,QAAK,CACrB,CAAAQ,QAAG,CAAE,MAAG,CACR,CAAAC,QAAG,CAAE,oBAAU,CACf,CAAAM,SAAS,CAAE,OAAO,EAAA,AAAlB,IAA0B,AAJD,IAAA,A,C,I;AAIzB,IAAAA,cAAS,CAAE,OAAO,EAAA,AAAlB,CAAAA,SAAS;AAJgB,IAAA5B,UAIC,CAAA,AAJD;AAIC,IAAAA,UAAA,OAAA;AAHhB,MAGW,AAArB,CAAA4B,cAAS,AAAT,GAAqB,IAAK,CAAA;AAA1B,MAAAA,cAAS,EAAY,MAAK;AAHhB,IAAA7B,QAAA,CAAAc,SAAI,EAAA,AAAJ,CAAAA;AACV,IAAAd,QAAA,CAAAsB,QAAG,EAAA,AAAH,CAAAA;AACA,IAAAtB,QAAA,CAAAuB,QAAG,EAAA,AAAH,CAAAA;AACA,IAAAvB,QAAA,CAAA6B,cAAS,EAAA,AAAT,CAAAA;AAA0B,UAAA,AAJD,CAAA5B,UAIC;AAJtB,KAAqB,UAAAD,QAAA,CACf,CAAAc,SAAI,CAAE,QAAK,CACrB,CAAAQ,QAAG,CAAE,MAAG,CACR,CAAAC,QAAG,CAAE,oBAAU,CACf,CAAAM,SAAS,CAAE,OAAO,EAAA,AAAlB,IAA0B,AAJD;AAIzB,IAAAA,cAAS,CAAE,OAAO,EAAA,AAAlB,CAAAA,SAAS;AAJgB,IAAA7B,QAAA,CAAAe,gBAAA,CACfD,SAAW,CACrB,CAAAQ,QAAQ,CACR,CAAAC,QAAe,CACf,CAAAM,cAA0B,CAAA;AAHhB;AAAA,WAAA7B,SAAA;AAAA,IAAAC,WAAM,SAAK;AAAX,IAAAA,WAAA,GAAAD,SAAA,CAAAc;AAAA,WAAAb,WAAM;AAChB;AAAA,UAAAD,SAAA;AAAA,IAAAC,WAAK,OAAG;AAAR,IAAAA,WAAA,GAAAD,SAAA,CAAAsB;AAAA,WAAArB,WAAK;AACL;AAAA,UAAAD,SAAA;AAAA,IAAAC,WAAK,qBAAU;AAAf,IAAAA,WAAA,GAAAD,SAAA,CAAAuB;AAAA,WAAAtB,WAAK;AACL;AAAA,gBAAAD,SAAA;AAAA,IAAAC,WAAW,QAAO;AAAlB,IAAAA,WAAA,GAAAD,SAAA,CAAA6B;AAAA,WAAA5B,WAAW;AAyBP,MAAA6B,QAAA,CAAA/B,KACwB,EAAA;AAAlB,EAAA0B,UAAK,CAAE,qBAAW;AADxB,WACwB,EAAA,AADxB,EACM,YAAkB,EAAA;AADD,MAAAV,gBAAA,CAAAf,QAAA,CACjB,CAAAyB,UAAK,CAAE,qBAAW,AADD,IAAA,A,C,I;AAAA,IAAAxB,UACC,CAAA,AADD;AACC,IAAAA,UAAA,OAAA;AAAlB,IAAAD,QAAA,CAAAyB,UAAK,EAAA,AAAL,CAAAA;AAAkB,UAAA,AADD,CAAAxB,UACC;AADxB,KAAuB,UAAAD,QAAA,CACjB,CAAAyB,UAAK,CAAE,qBAAW,AADD;AAAA,IAAAzB,QAAA,CAAAe,gBAAA,CACjBU,UAAkB,CAAA;AAAlB;AAAA,YAAAzB,SAAA;AAAA,IAAAC,WAAO,sBAAW;AAAlB,IAAAA,WAAA,GAAAD,SAAA,CAAAyB;AAAA,WAAAxB,WAAO;AAgBb,MAAA8B,KAAA,CAAA7E,aAGoB,EAAA;AAFpB,EAAA2D,SAAI,CAAE;AACN,EAAAK,UAAK,CAAE;AACP,EAAAc,oBAAe,CAAE,MAAG;AAHpB,WAGoB,EAAA,AAHpB,EACJ,WAAgB,CAChB,aAAiB,CACjB,uBAAwB,CAAA;AAHd,MAAAjB,gBAAA,CAAAf,QAAA,CACN,CAAAa,SAAI,CAAE,MAAM,CACZ,CAAAK,UAAK,CAAE,MAAM,CACb,CAAAc,oBAAe,CAAE,MAAG,AAHd,IAAA,A,C,I;AAAA,IAAA/B,UAGc,CAAA,AAHd;AAGc,IAAAA,UAAA,OAAA;AAFpB,IAAAD,QAAA,CAAAa,SAAI,EAAA,AAAJ,CAAAA;AACA,IAAAb,QAAA,CAAAkB,UAAK,EAAA,AAAL,CAAAA;AACA,IAAAlB,QAAA,CAAAgC,oBAAe,EAAA,AAAf,CAAAA;AAAoB,UAAA,AAHd,CAAA/B,UAGc;AAHpB,KAAM,UAAAD,QAAA,CACN,CAAAa,SAAI,CAAE,MAAM,CACZ,CAAAK,UAAK,CAAE,MAAM,CACb,CAAAc,oBAAe,CAAE,MAAG,AAHd;AAAA,IAAAhC,QAAA,CAAAe,gBAAA,CACNF,SAAY,CACZ,CAAAK,UAAa,CACb,CAAAc,oBAAoB,CAAA;AAFxB;AAAA,WAAAhC,SAAA;AAAA,IAAAC,WAAU,OAAM;AAAhB,IAAAA,WAAA,GAAAD,SAAA,CAAAa;AAAA,WAAAZ,WAAU;AACV;AAAA,YAAAD,SAAA;AAAA,IAAAC,WAAW,OAAM;AAAjB,IAAAA,WAAA,GAAAD,SAAA,CAAAkB;AAAA,WAAAjB,WAAW;AACX;AAAA,wBAAAD,SAAA;AAAA,IAAAC,WAAqB,OAAG;AAAxB,IAAAA,WAAA,GAAAD,SAAA,CAAAgC;AAAA,WAAA/B,WAAqB;AAaxB,MAAAgC,aAAA,CAAA/E,aAGgC,EAAA;AAFzB,EAAAgF,eAAU,CAAE;AACZ,EAAAC,UAAK,CAAE;AACP,EAAAC,aAAQ,CAAE,KAAe;AAHhC,WAGgC,EAAA,AAHhC,EACG,iBAA+C,CAC/C,aAA8D,CAC9D,gBAA6B,CAAA;AAHtB,MAAArB,gBAAA,CAAAf,QAAA,CACH,CAAAkC,WAAU,CAAE,aAAU,EAAA,AAA1B,IAA+C,CAC3C,CAAAC,KAAK,CAAE,QAAK,EAAA,AAAhB,IAA8D,CAC1D,CAAAC,SAAQ,CAAE,KAAE,EAAA,AAAhB,IAA6B,AAHtB,IAAA,A,C,I;AACH,IAAAF,eAAU,CAAE,aAAU,EAAA,AAAtB,CAAAA;AACA,IAAAC,UAAK,CAAE,QAAK,EAAA,AAAZ,CAAAA;AACA,IAAAC,aAAQ,CAAE,KAAE,EAAA,AAAZ,CAAAA,SAAQ;AAHL,IAAAnC,UAGsB,CAAA,AAHtB,OAGsB;AAFA,IAAAoC,MAAkB,CAAA,AAAlB;AACV,IAAAC,MAA2C,CAAA,AAA3C;AACA,IAAAC,MAAU,CAAA,AAAV;AAAU,IAAAtC,UAAA,OAAA;AAFA,MAAA,AAAzB,CAAAiC,eAAU,AAAV,GAAyB,IAAkB,CAAA;AAAlB,MAAAG,MAAA,EAAI,CAAApB,UAAU,CAAC,EAAE,CAAC;AAA3C,MAAAiB,eAAU,EAAe,CAAAG,MAAkB;AAAA,MAC5B,AAAf,CAAAF,UAAK,AAAL,GAAe,IAA2C,CAAA;AAA3C,MAAAG,MAAA,EAAE,CAAAP,KAAA,CAAM,EAAE,CAAS,GAAE,CAAmB,EAAC,CAAE;AAA1D,MAAAI,UAAK,EAAU,CAAAG,MAA2C;AAD1D,MAEe,AAAf,CAAAF,aAAQ,AAAR,GAAe,IAAU,CAAA;AAAV,MAAAG,MAAA,EAAI,CAAAZ,EAAE,CAAC,EAAE,CAAC;AAAzB,MAAAS,aAAQ,EAAO,CAAAG,MAAU;AAFzB,IAAAvC,QAAA,CAAAkC,eAAU,EAAA,AAAV,CAAAA;AACA,IAAAlC,QAAA,CAAAmC,UAAK,EAAA,AAAL,CAAAA;AACA,IAAAnC,QAAA,CAAAoC,aAAQ,EAAA,AAAR,CAAAA;AAAyB,UAAA,AAHtB,CAAAnC,UAGsB;AAHhC,KAAU,UAAAD,QAAA,CACH,CAAAkC,WAAU,CAAE,aAAU,EAAA,AAA1B,IAA+C,CAC3C,CAAAC,KAAK,CAAE,QAAK,EAAA,AAAhB,IAA8D,CAC1D,CAAAC,SAAQ,CAAE,KAAE,EAAA,AAAhB,IAA6B,AAHtB;AACH,IAAAF,eAAU,CAAE,aAAU,EAAA,AAAtB,CAAAA;AACA,IAAAC,UAAK,CAAE,QAAK,EAAA,AAAZ,CAAAA;AACA,IAAAC,aAAQ,CAAE,KAAE,EAAA,AAAZ,CAAAA,SAAQ;AAHL,IAAApC,QAAA,CAAAe,gBAAA,CACHmB,eAA2C,CAC3C,CAAAC,UAA0D,CAC1D,CAAAC,aAAyB,CAAA;AAF7B;AAAA,kBAAApC,SAAA;AAAA,IAAAC,WAAgB,cAAU;AAA1B,IAAAA,WAAA,GAAAD,SAAA,CAAAkC;AAAA,WAAAjC,WAAgB;AAChB;AAAA,YAAAD,SAAA;AAAA,IAAAC,WAAW,SAAK;AAAhB,IAAAA,WAAA,GAAAD,SAAA,CAAAmC;AAAA,WAAAlC,WAAW;AACX;AAAA,gBAAAD,SAAA;AAAA,IAAAC,WAAc,MAAE;AAAhB,IAAAA,WAAA,GAAAD,SAAA,CAAAoC;AAAA,WAAAnC,WAAc;AAUV,MAAAE,aAAA,CAAAjD,aA8D2C,EAAA;AAvD3C,EAAAsF,SAAI,CAAE;AA+Bb,EAAAC,aAAQ,CAAE,OAAQ;AAtCX,WA8D2C,EAAA,AA9D3C,EAOJ,WAAe,CA+BtB,gBAAsB,CAwBgC;AArD/C,MAAA1B,gBAAW,CAAA,AAACf,QAAA,EAAAwC,SAAI,CAAE,QAGxB,IAAA,A,C,I;AAH+B,IAAAvC,UAAA;AAG/B,IAAAA,UAAA,OAAA;AAFC,IAAAD,QAAI,CAACwC,SAAI,EAAG,CAAAA,SAAI;AACY,IAAAE,MAAQ,CAAA,AAAR,MAAQ,EAAA,AAAR,CAAA1C,QAAM,CAAA,AAAN,WAAM,EAAE;AAAzB,IAAA2C,MAA0B,CAAA,AAA1B,OAA0B,EAAA,AAA1B,CAAAvD,qCAAgB,CAAA,AAAhBY,QAAgB,CAAC,CAAA0C,MAAQ,CAAC;AAArC,IAAA1C,QAAQ,CAAA,AAARyC,aAAQ,EAAG,CAAAE,MAA0B;AACtC,UAAA,AAH+B,CAAA1C,UAG/B;AAZU,KASJ,SAGN,CAAA,AAHkBD,QAAA,EAAAwC,SAAI,CAAE,QAGxB,IAAA,AAHM,KAGN,CAAA;AAHkB,IAAAxC,QAAA,CAAAe,gBAGlB,CAAA,AAHkByB,SAAW,CAqDwB;AA3C/C,WAA8D,CAAA,AAAxDxC,QAAA,EAAAI,SAAI,CAAE,MAAkD,IAAA,AAAzC,OAAO,CAAA;AAAP,IAAAH,UAAA;AAAU,IAAA2C,MAA6B,CAAA,AAA7B,OAA6B,EAAA,AAA7B,CAAAtD,kCAAa,CAAA,AAAbU,QAAa,CAAC,CAAAA,QAAQ,CAAA,AAARyC,aAAQ,CAAE,CAAArC,SAAI,CAAC;AAAvC,IAAAH,UAAA,EAAU,CAAA2C,MAA6B;AAAE,UAAA,AAAzC,CAAA3C;AAErB,UAEN,CAAA,AAFWD,QAAA,EAAAI,SAAI,CAAE,MAEjB,IAAA,AAF0B,2CAA6B,CAAA;AAA7B,IAAAH,UAAA;AACzB,IAAA4C,KAAuC,CAAA,AAAvC,sBAAuC;AAAvC,IAAAA,KAAA,GAAArD,iCAAY,CAAA,AAAZQ,QAAY,CAAC,CAAAA,QAAQ,CAAA,AAARyC,aAAQ,CAAE,CAAArC,SAAI,CAAE,CAAA0C,cAAS,CAAC;AADd,IAAA7C,UAAA,EACzB,CAAA4C,KAAuC;AACxC,UAAA,AAF0B,CAAA5C;AAIpB,aAIN,CAAA,AAHCD,QAAA,EAAAI,SAAI,CAAE,MAAM,CAAE,CAAAK,WAAM,CAAE,wCAGvB,IAAA,AAFE,MAAM,CAAA;AAAN,IAAAR,UAAA;AACD,IAAA8C,MAAkD,CAAA,AAAlD,MAAkD,EAAA,AAAlD,CAAArD,oCAAe,CAAA,AAAfM,QAAe,CAAC,CAAAA,QAAQ,CAAA,AAARyC,aAAQ,CAAE,CAAArC,SAAI,CAAE,CAAAK,WAAM,CAAE,CAAAqC,cAAS,CAAC;AADjD,IAAA7C,UAAA,EACD,CAAA8C,MAAkD;AACnD,UAAA,AAFE,CAAA9C;AAmCH,MAAAQ,WAAsD,CAAA,AAA9CT,QAA8C,IAAA,AAA5C,MAAM,CAAA;AAAN,IAAAC,UAAA;AAAS,IAAA+C,MAAoB,CAAA,AAApB,qBAAoB,EAAA,AAAhB,CAAAC,kBAAc,EAAE;AAApB,IAAAC,MAAiC,CAAA,AAAjC,MAAiC,EAAA,AAAjC,CAAAF,MAAoB,CAAA,AAApB,MAA2B,CAAChD,QAAI,CAAA,AAAJwC,SAAI,CAAC;AAA1C,IAAAvC,UAAA,EAAS,CAAAiD,MAAiC;AAAE,UAAA,AAA5C,CAAAjD,UAA4C;AAvD/C;AAAA,WAAAD,SAAA;AAAA,IAAAC,WAAU,SAAK;AAAf,IAAAA,WAAA,GAAAD,SAAA,CAAAwC;AAAA,WAAAvC,WAAU;AA+Eb,MAAAgD,kBAAA,CAAA/F,aAmMH,EAAA;AAlMG,EAAAiG,QAAG,CAAE,aAA+C;AADpD,WAmMH,EAAA,AAnMG,EACJ,UAAwD,EAkMvD;AAhMM,YAGN,CAAA,AAHanD,QAAA,EAAAoD,UAAK,CAAE,QAGpB,IAAA,AAH4B,MAAM,CAAA;AAAN,IAAAnD,WAAA;AAC3B,IAAAD,QAAS,CAAA,AAAT,cAAS,CAACoD,UAAK;AACf,IAAAC,MAAG,CAAA,AAAH,aAAG,EAAA,AAAH,CAAArD,QAAG,CAAA,AAAHmD;AAAa,QAAAG,QAAA,CAAGC,MAAC,CAAA,AAAD,MAAQ,IAAA,AAAH;AAAA,MAAAtD,WAAA;AAAA,MAAAA,WAAA,GAAAsD,MAAC;AAAA,YAAA,AAAD,CAAAtD,WAAC;AAAE,IAAAuD,MAAA,4BAAAF,QAAA;AAAxB,IAAAG,MAAwB,CAAA,AAAxB,MAAwB,EAAA,AAApB,CAAAhG,cAAI,CAAA,AAAR4F,MAAG,CAAM,GAAE,CAAE,CAAAG,MAAW,CAAA;AAFG,IAAAvD,WAAA,EAE3B,CAAAwD,MAAwB;AACzB,UAAA,AAH4B,CAAAxD;AAK7B,MAAAyD,cAsBC,CAAA,AAtBS1D,QAAA,EAAAoD,UAAK,CAAE,QAsBhB,IAAA,AAtBwB,OAAI,CAAA;AAAJ,IAAAnD,WAAA;AAsBxB,IAAAA,WAAA,OAAA;AAnBM,IAAA0D,KAAO,CAAA,AAAP,OAAO;AAAP,IAAAC,KAAO,CAAA,AAAP;AACA,IAAAC,KAAU,CAAA,AAAV,OAAU;AAAV,IAAAC,KAAU,CAAA,AAAV;AACA,IAAAC,KAAS,CAAA,AAAT,OAAS;AAAT,IAAAC,KAAS,CAAA,AAAT;AACA,IAAAC,KAAO,CAAA,AAAP,OAAO;AAAP,IAAAC,KAAO,CAAA,AAAP;AACA,IAAAC,KAAE,CAAA,AAAF,OAAE;AAAF,IAAAC,KAAE,CAAA,AAAF;AACA,IAAAC,KAAM,CAAA,AAAN,OAAM;AAAN,IAAAC,KAAM,CAAA,AAAN;AACA,IAAAC,KAAQ,CAAA,AAAR,OAAQ;AAAR,IAAAC,KAAQ,CAAA,AAAR,WAAQ;AANR;AAAA,MAAArH,aAAO,CAAA,AAFLiG,UAAK,CAEP,CAAAxC,OAAO,CAAA;AAAP,MAAA+C,KAAA,OAAO;AAAP,UAAO,CAAA7E,UAAA,CAAA;AAAP,MAAA6E,KAAA,QAAO;AAAP,SAAAvG,OAmBN,KAAA,AAnBM,CAAAqH,YAmBN,CAAA;AAnBM,SAAAd,KAAO,CAAA;AAAP;AAAA,UAAAC,KAAA,GAAAzG,aAAO,CAAA,AAFLiG,UAAK,CAEP,CAAAxC,OAAO,CAAA;AAmBb,cAAA,AAnBa,CAAA9B,UAAA;AAmBb,UAAA2F,YAAA,SAAA;AAnBiB,QAAAzE,QAAW,CAAA,AAAX,gBAAW,CAAC4D,KAAK;AAAC;AAC7B;AAAA,UAAAzG,aAAU,CAAA,AAHRiG,UAAK,CAGP,CAAAnC,UAAU,CAAA;AAAV,UAAA4C,KAAA,OAAU;AAAV,cAAU,CAAA/E,UAAA,CAAA;AAAV,UAAA+E,KAAA,QAAU;AAAV,WAAAA,KAAU,CAAA;AAAV;AAAA,YAAAC,KAAA,GAAA3G,aAAU,CAAA,AAHRiG,UAAK,CAGP,CAAAnC,UAAU,CAAA;AAkBhB,gBAAA,AAlBgB,CAAAnC,UAAA;AAkBhB,YAAA2F,YAAA,SAAA;AAlBoB,UAAAzE,QAAc,CAAA,AAAd,mBAAc,CAAC8D,KAAK,CAAE,MAAK;AAAC;AAC1C;AAAA,YAAA3G,aAAS,CAAA,AAJPiG,UAAK,CAIP,CAAA/B,SAAS,CAAA;AAAT,YAAA0C,KAAA,OAAS;AAAT,gBAAS,CAAAjF,UAAA,CAAA;AAAT,YAAAiF,KAAA,QAAS;AAAT,aAAAA,KAAS,CAAA;AAAT;AAAA,cAAAC,KAAA,GAAA7G,aAAS,CAAA,AAJPiG,UAAK,CAIP,CAAA/B,SAAS,CAAA;AAiBf,kBAAA,AAjBe,CAAAvC,UAAA;AAiBf,cAAA2F,YAAA,SAAA;AAjBmB,YAAAzE,QAAa,CAAA,AAAb,kBAAa,CAACgE,KAAK;AAAC;AACjC;AAAA,cAAA7G,aAAO,CAAA,AALLiG,UAAK,CAKP,CAAA5B,OAAO,CAAA;AAAP,cAAAyC,KAAA,OAAO;AAAP,kBAAO,CAAAnF,UAAA,CAAA;AAAP,cAAAmF,KAAA,QAAO;AAAP,eAAAA,KAAO,CAAA;AAAP;AAAA,gBAAAC,KAAA,GAAA/G,aAAO,CAAA,AALLiG,UAAK,CAKP,CAAA5B,OAAO,CAAA;AAgBb,oBAAA,AAhBa,CAAA1C,UAAA;AAgBb,gBAAA2F,YAAA,SAAA;AAhBiB,cAAAzE,QAAW,CAAA,AAAX,gBAAW,CAACkE,KAAK;AAAC;AAC7B;AAAA,gBAAA/G,aAAE,CAAA,AANAiG,UAAK,CAMP,CAAAzB,EAAE,CAAA;AAAF,gBAAAwC,KAAA,OAAE;AAAF,oBAAE,CAAArF,UAAA,CAAA;AAAF,gBAAAqF,KAAA,QAAE;AAAF,iBAAAA,KAAE,CAAA;AAAF;AAAA,kBAAAC,KAAA,GAAAjH,aAAE,CAAA,AANAiG,UAAK,CAMP,CAAAzB,EAAE,CAAA;AAeR,sBAAA,AAfQ,CAAA7C,UAAA;AAeR,kBAAA2F,YAAA,SAAA;AAfY,gBAAAzE,QAAM,CAAA,AAAN,WAAM,CAACoE,KAAK;AAAC;AACnB;AAAA,kBAAAjH,aAAM,CAAA,AAPJiG,UAAK,CAOP,CAAAxB,MAAM,CAAA;AAAN,kBAAAyC,KAAA,OAAM;AAAN,sBAAM,CAAAvF,UAAA,CAAA;AAAN,kBAAAuF,KAAA,QAAM;AAAN,mBAAAA,KAAM,CAAA;AAAN;AAAA,oBAAAC,KAAA,GAAAnH,aAAM,CAAA,AAPJiG,UAAK,CAOP,CAAAxB,MAAM,CAAA;AAcZ,wBAAA,AAdY,CAAA9C,UAAA;AAcZ,oBAAA2F,YAAA,SAAA;AAdgB,kBAAAzE,QAAU,CAAA,AAAV,eAAU,CAACsE,KAAK;AAAC;AAC3B;AAAA,oBAAAnH,aAAQ,CAAA,AARNiG,UAAK,CAQP,CAAAtB,QAAQ,CAAA;AAAR,oBAAAyC,KAAA,OAAQ;AAAR,wBAAQ,CAAAzF,UAAA,CAAA;AAAR,oBAAAyF,KAAA,QAAQ;AAAR,qBAAAA,KAAQ,CAAA;AAAR;AAAA,sBAAAC,KAAA,GAAArH,aAAQ,CAAA,AARNiG,UAAK,CAQP,CAAAtB,QAAQ,CAAA;AAad,0BAAA,AAbc,CAAAhD,UAAA;AAad,sBAAA2F,YAAA,SAAA;AAbkB,oBAAAzE,QAAY,CAAA,AAAZ,iBAAY,CAACwE,KAAK,CAAC;AAAvB,sBAGX,CAAA7G,eAAK,CAAA,AAXAyF,UAAK,CAWV,CAAAsB,KAAK;AAAI;AAAI,sBAAA7G,qBAAG,CAAA,AAAPmC,QAAG,CAAA,AAAHmD,QAAG,CAAK,IAAG;AAUvB,0BAAA,AAVwB,CAAArE,UAAA;AAUxB,sBAAA2F,YAAA,SAAA;AAbc,sBAIX,CAAA9G,eAAG,CAAA,AAZEyF,UAAK,CAYV,CAAAuB,GAAG;AAAI;AAAI,sBAAA9G,qBAAG,CAAA,AAAPmC,QAAG,CAAA,AAAHmD,QAAG,CAAK,IAAG;AASrB,0BAAA,AATsB,CAAArE,UAAA;AAStB,sBAAA2F,YAAA,SAAA;AAbc,sBAKX,CAAA9G,eAAG,CAAA,AAbEyF,UAAK,CAaV,CAAAwB,GAAG;AAAI;AAAI,sBAAA/G,qBAAG,CAAA,AAAPmC,QAAG,CAAA,AAAHmD,QAAG,CAAK,IAAG;AAQrB,0BAAA,AARsB,CAAArE,UAAA;AAQtB,sBAAA2F,YAAA,SAAA;AAbc,sBAMX,CAAA9G,eAAY,CAAA,AAdPyF,UAAK,CAcV,CAAAyB,aAAY;AAAI;AAAI,sBAAAhH,qBAAG,CAAA,AAAPmC,QAAG,CAAA,AAAHmD,QAAG,CAAK,MAAK;AAOhC,0BAAA,AAPiC,CAAArE,UAAA;AAOjC,sBAAA2F,YAAA,SAAA;AAbc,sBAQX,CAAA9G,eAAK,CAAA,AAhBAyF,UAAK,CAgBV,CAAA0B,KAAK;AAAI;AAAI,sBAAAjH,qBAAG,CAAA,AAAPmC,QAAG,CAAA,AAAHmD,QAAG,CAAK,MAAK;AAKzB,0BAAA,AAL0B,CAAArE,UAAA;AAK1B,sBAAA2F,YAAA,SAAA;AAbc,sBASX,CAAA9G,eAAK,CAAA,AAjBAyF,UAAK,CAiBV,CAAA2B,KAAK;AAAI;AAAI,sBAAAlH,qBAAG,CAAA,AAAPmC,QAAG,CAAA,AAAHmD,QAAG,CAAK,MAAK;AAIzB,0BAAA,AAJ0B,CAAArE,UAAA;AAI1B,sBAAA2F,YAAA,SAAA;AAbc,sBAUX,CAAA9G,eAAI,CAAA,AAlBCyF,UAAK,CAkBV,CAAA4B,IAAI;AAAI;AAAI,sBAAAnH,qBAAG,CAAA,AAAPmC,QAAG,CAAA,AAAHmD,QAAG,CAAK,MAAK;AAGxB,0BAAA,AAHyB,CAAArE,UAAA;AAGzB,sBAAA2F,YAAA,SAAA;AAAA,YAAA,AAtBwB,CAAAxE;AAsBxB,UAAA5C,mBAAA;AAED,MAAA4H,gBAQC,CAAA,AARWjF,QAAA,EAAAkF,YAAO,CAAE,UAQpB,IAAA,AAR8B,OAAI,CAAA;AAAJ,IAAAjF,WAAA;AAKR,IAAAkF,MAAY,CAAA,AAAZ;AACX,IAAAC,MAAY,CAAA,AAAZ;AAEX,IAAAnF,WAAA,OAAA;AAHiB,IAAAoF,KAAG,CAAA,AAAH,aAAG;AAJf,IAAAxH,qBAAG,CAAA,AAAPmC,QAAG,CAAA,AAAHmD,QAAG,CAAK,IAAG;AAIK,IAAAkC,KAAA,GAAArF,QAAG,CAAA,AAAHmD,QAAG;AAAE,IAAAgC,MAAA,GAAAD,YAAO,CAAK,IAAA;AAAjC,IAAAtF,sCAAe,CAAA,AAAfI,QAAe,CAAC,CAAAqF,KAAG,CAAE,CAAAF,MAAY;AACvB,IAAAC,MAAA,GAAAF,YAAO,CAAK,IAAA;AAAtB,IAAAlF,QAAS,CAAA,AAAT,cAAS,CAACoF,MAAY;AAClB,IAAAvH,qBAAG,CAAA,AAAPmC,QAAG,CAAA,AAAHmD,QAAG,CAAK,IAAG;AACZ,UAAA,AAR8B,CAAAlD;AAgB/B,MAAAqF,aAQC,CAAA,AARQtF,QAAA,EAAAuF,SAAI,CAAE,MAAG,CAAE,CAAAC,kBAAa,CAAE,OAQlC,IAAA,AAR4C,OAAI,CAAA;AAAJ,IAAAvF,WAAA;AAQ5C,IAAAA,WAAA,OAAA;AANC,IAAAH,iCAAU,CAAA,AAAVE,QAAU,CAAC,CAAAA,QAAG,CAAA,AAAHmD,QAAG,CAAE,CAAAoC,SAAI,CAAE,CAAAC,kBAAa;AAMpC,UAAA,AAR4C,CAAAvF;AAa7C,MAAAwF,mBAQC,CAAA,AARczF,QAAA,EAAAkC,eAAU,CAAE,aAAU,CAAE,CAAAsD,kBAAa,CAAE,OAQrD,IAAA,AAR+D,OAAI,CAAA;AAAJ,IAAAvF,WAAA;AAG3D,IAAAyF,MAAa,CAAA,AAAb;AAGQ,IAAAC,MAAY,CAAA,AAAZ,MAAY;AAFb,IAAAC,MAAgB,CAAA,AAAhB;AAIX,IAAA3F,WAAA,OAAA;AANe,IAAA4F,MAAgB,CAAA,AAAhB,MAAgB,EAAA,AAAhB,CAAA3D,eAAU,CAAM,KAAA;AAAhB,IAAA4D,MAA2B,CAAA,AAA3B,OAA2B,EAAA,AAAV,CAAA/H,uBAAU,CAAA,AAA3B8H,MAAgB,CAAW;AAAnC,IAAAE,UAAK,CAAA,AAAL,OAAK,EAAG,CAAAD;AAMf,eAAA;AALI,MAAAJ,MAAA,GAAAK,UAAK,CAAQ,QAAA;AAFhB,QAEE,CAAA9H,aAAC,CAAAyH,MAAa;AAGL,QAAAC,MAAA,EAAM,AAAN,CAAAI,UAAK,CAAA,AAAL,IAAU,EAAE;AAArB,QAAA/F,QAAQ,CAAA,AAAR,aAAQ,CAAC2F,MAAY,CAAE,CAAAH,kBAAa,CAAC;AAF7B,QAAAI,MAAA,EAAM,AAAN,CAAAG,UAAK,CAAA,AAAL,OAAa,CAAC,CAAC,CAAC;AAAxB,QAAAA,UAAK,EAAG,CAAAH,MAAgB;AAAnB;AAIR;AAAA,UAAA,AAR+D,CAAA3F;AAUhE,MAAA+F,kBAIC,CAAA,AAJahG,QAAA,EAAAiG,cAAS,CAAE,YAIxB,IAAA,AAJoC,OAAI,CAAA;AAAJ,IAAAhG,WAAA;AAIpC,IAAAA,WAAA,OAAA;AAHK,IAAApC,qBAAG,CAAA,AAAPmC,QAAG,CAAA,AAAHmD,QAAG,CAAK,IAAG;AACX,IAAAnD,QAAsB,CAAA,AAAtB,2BAAsB,CAACiG,cAAS;AAC5B,IAAApI,qBAAG,CAAA,AAAPmC,QAAG,CAAA,AAAHmD,QAAG,CAAK,IAAG;AACZ,UAAA,AAJoC,CAAAlD;AAMrC,MAAAiG,2BAIC,CAAA,AAJsBlG,QAAA,EAAAiG,cAAS,CAAE,YAIjC,IAAA,AAJ6C,OAAI,CAAA;AAAJ,IAAAhG,WAAA;AAGnC,IAAAkG,MAAa,CAAA,AAAb;AACV,IAAAlG,WAAA,OAAA;AAHU,IAAAmG,MAAa,CAAA,AAAb,MAAa,EAAA,AAAb,CAAAH,cAAS,CAAI,GAAA;AAAtB,IAAAjG,QAAQ,CAAA,AAAR,aAAQ,CAACoG,MAAa,CAAE,KAAI;AACxB,IAAAvI,qBAAG,CAAA,AAAPmC,QAAG,CAAA,AAAHmD,QAAG,CAAK,IAAG;AACF,IAAAgD,MAAA,GAAAF,cAAS,CAAI,GAAA;AAAtB,IAAAjG,QAAQ,CAAA,AAAR,aAAQ,CAACmG,MAAa,CAAE,KAAI;AAC7B,UAAA,AAJ6C,CAAAlG;AAM9C,MAAAoG,gBAeC,CAAA,AAfWrG,QAAA,EAAAsG,YAAO,CAAE,UAepB,IAAA,AAf8B,OAAI,CAAA;AAAJ,IAAArG,WAAA;AAQL,IAAAsG,MAAc,CAAA,AAAd;AACF,IAAAC,MAAc,CAAA,AAAd,wBAAc;AADZ,IAAAC,MAAqB,CAAA,AAArB,MAAqB;AAHrC,IAAAC,MAAgB,CAAA,AAAhB;AAUT,IAAAzG,WAAA,OAAA;AAZM,IAAA0G,KAAO,CAAA,AAAP,OAAO;AAAP,IAAAC,KAAO,CAAA,AAAP;AAMiB,IAAAC,KAAiB,CAAA,AAAjB,WAAiB;AARxB,IAAAC,MAAiC,CAAA,AAAjC,QAAiC,EAAA,AAAjC,CAAA9G,QAAa,CAAA,AAAb,kBAAa,CAACsG,YAAO,CAAE,CAAAxD,cAAS,CAAC;AAA5C,IAAAiE,aAAQ,CAAA,AAAR,QAAQ,EAAG,CAAAD;AAEV;AAAA,MAAA3J,aAAO,CAAA,AADL4J,aAAQ,CACV,CAAAvF,OAAO,CAAA;AAAP,MAAAmF,KAAA,OAAO;AAAP,UAAO,CAAA7H,UAAA,CAAA;AAAP,MAAA6H,KAAA,QAAO;AAAA,SAAAvJ,OAAA,MAAA4J,YAAA,CAAA;AAAP,SAAAL,KAAO,CAAA;AAAP,aAAAvJ,OAYN,KAAA,AAZM,CAAA6J,YAYN,CAAA;AAZM;AAAA,YAAAL,KAAA,GAAAzJ,aAAO,CAAA,AADL4J,aAAQ,CACV,CAAAvF,OAAO,CAAA;AACJ,YAAA3D,qBAAG,CAAA,AAAPmC,QAAG,CAAA,AAAHmD,QAAG,CAAK,IAAG;AAWhB,gBAAA,AAXiB,CAAArE,UAAA;AAWjB,YAAAmI,YAAA,SAAA;AAVS,UAAAP,MAAA,GAAAE,KAAQ,CAAQ,OAAA;AAAhB,aAAAF,MAAgB;AAClB;AAAI,cAAA7I,qBAAG,CAAA,AAAPmC,QAAG,CAAA,AAAHmD,QAAG,CAAK,IAAG;AASlB,kBAAA,AATmB,CAAArE,UAAA;AASnB,cAAAmI,YAAA,SAAA;AAPc,UAAAC,MAAC,CAAA,AAAD,MAAC,EAAG;AAGb,qBAAA;AAHoB,YAAAX,MAAA,GAAAK,KAAQ,CAAM,KAAA;AAAd,YAAAH,MAAA,EAAe,CAAAzH,QAAM,CAAA,AAArBuH,MAAc,CAAO;AAAzC,cAAgB,CAAAW,MAAC,AAAD,EAAI,CAAAT,MAAqB;AACvB,cAAAD,MAAA,GAAAI,KAAQ,CAAM,KAAA;AAAd;AAAA,gBAAAC,KAAA,EAAc,CAAA1I,aAAA,CAAA,AAAdqI,MAAc,CAAC,CAAAU,MAAC,CAAC;AAMxC,oBAAA,AANwC,CAAApI,UAAA;AAMxC,gBAAAmI,YAAA,SAAA;AANO,cAAAjH,QAAe,CAAA,AAAf,oBAAe,CAAC6G,KAAiB,CAAC;AADO,cAAAK,MAAC,EAAA,AAAD,CAAAA,MAAC,AAAD,EAAK,EAAC;AAAL;AAG5C,mBAAY;AAAZ;AAAI,YAAArJ,qBAAG,CAAA,AAAPmC,QAAG,CAAA,AAAHmD,QAAG,CAAK,IAAG;AAIhB,YAAA6D,YAAA;AAAA,iBAAAlI,UAAA;AAAA,gBAAA;AAAA,cAAAzB,mBAAA,EAAA;AAFW,MAAA2C,QAAS,CAAA,AAAT,cAAS,CAAC+G,aAAQ,CAAC;AAE9B,UAAA,AAf8B,CAAA9G;AAkB/B,MAAAkH,kBAAwE,CAAA,AAA1DnH,QAAA,EAAAsG,YAAO,CAAE,UAAO,CAAE,CAAAxD,cAAS,CAAE,gBAA6B,IAAA,AAAjB,QAAK,CAAA;AAAL,IAAA7C,WAAA,SAAK;AAAL,IAAAA,WAAA,EAAQ,CAAAqG,YAAO;AAAE,UAAA,AAAjB,CAAArG;AAEvD,MAAAmH,oBAMC,CAAA,AANepH,QAAA,EAAAqH,aAAQ,CAAE,WAMzB,IAAA,AANoC,OAAI,CAAA;AAAJ,IAAApH,WAAA;AAMpC,IAAAA,WAAA,OAAA;AAJM,IAAAqH,KAAU,CAAA,AAAV,OAAU;AAAV,IAAAC,KAAU,CAAA,AAAV;AACA,IAAAC,KAAS,CAAA,AAAT,OAAS;AAAT,IAAAC,KAAS,CAAA,AAAT;AACA,IAAAC,KAAU,CAAA,AAAV,OAAU;AAAV,IAAAC,KAAU,CAAA,AAAV,aAAU;AAFV;AAAA,MAAAxK,aAAU,CAAA,AADRkK,aAAQ,CACV,CAAApG,UAAU,CAAA;AAAV,MAAAqG,KAAA,OAAU;AAAV,UAAU,CAAAxI,UAAA,CAAA;AAAV,MAAAwI,KAAA,QAAU;AAAV,SAAAlK,OAIN,KAAA,AAJM,CAAAwK,YAIN,CAAA;AAJM,SAAAN,KAAU,CAAA;AAAV;AAAA,UAAAC,KAAA,GAAApK,aAAU,CAAA,AADRkK,aAAQ,CACV,CAAApG,UAAU,CAAA;AAIhB,cAAA,AAJgB,CAAAnC,UAAA;AAIhB,UAAA8I,YAAA,SAAA;AAJoB,QAAA5H,QAAc,CAAA,AAAd,mBAAc,CAACuH,KAAQ,CAAE,KAAI;AAAC;AAC5C;AAAA,UAAApK,aAAS,CAAA,AAFPkK,aAAQ,CAEV,CAAAhG,SAAS,CAAA;AAAT,UAAAmG,KAAA,OAAS;AAAT,cAAS,CAAA1I,UAAA,CAAA;AAAT,UAAA0I,KAAA,QAAS;AAAT,WAAAA,KAAS,CAAA;AAAT;AAAA,YAAAC,KAAA,GAAAtK,aAAS,CAAA,AAFPkK,aAAQ,CAEV,CAAAhG,SAAS,CAAA;AAGf,gBAAA,AAHe,CAAAvC,UAAA;AAGf,YAAA8I,YAAA,SAAA;AAHmB,UAAA5H,QAAsB,CAAA,AAAtB,2BAAsB,CAACyH,KAAQ;AAAC;AAC7C;AAAA,YAAAtK,aAAU,CAAA,AAHRkK,aAAQ,CAGV,CAAAjG,UAAU,CAAA;AAAV,YAAAsG,KAAA,OAAU;AAAV,gBAAU,CAAA5I,UAAA,CAAA;AAAV,YAAA4I,KAAA,QAAU;AAAV,aAAAA,KAAU,CAAA;AAAV;AAAA,cAAAC,KAAA,GAAAxK,aAAU,CAAA,AAHRkK,aAAQ,CAGV,CAAAjG,UAAU,CAAA;AAEhB,kBAAA,AAFgB,CAAAtC,UAAA;AAEhB,cAAA8I,YAAA,SAAA;AAFoB,YAAA5H,QAAS,CAAA,AAAT,cAAS,CAAC2H,KAAQ;AAEtC,YAAA,AANoC,CAAA1H;AAMpC,UAAA5C,mBAAA;AAED,MAAAwK,WAYC,CAAA,AAZM7H,QAAA,EAAA8H,OAAE,CAAE,KAYV,IAAA,AAZe,OAAI,CAAA;AAAJ,IAAA7H,WAAA;AAMQ,IAAA8H,MAAQ,CAAA,AAAR;AAER,IAAAC,MAAQ,CAAA,AAAR,qBAAQ;AAFA,IAAAC,MAAe,CAAA,AAAf,MAAe;AADzB,IAAAC,MAAQ,CAAA,AAAR;AAOb,IAAAjI,WAAA,OAAA;AAPa,IAAAkI,KAAW,CAAA,AAAX;AAGE,IAAAC,KAAW,CAAA,AAAX,QAAW;AAPpB,IAAAC,MAAQ,CAAA,AAAR,qBAAQ,EAAA,AAAR,CAAAP,OAAE,CAAM,KAAA;AAAR,IAAAQ,MAAgB,CAAA,AAAhB,OAAgB,EAAA,AAAhB,IAAgB,AAAhB,CAAAD;AAAgB,SAAAjL,OAAA,MAAAmL,YAAA,CAAA;AAAjB,SAAAtK,aAAC,CAAAqK,MAAgB;AACnB,aAAAlL,OAUH,KAAA,AAVG,CAAAoL,YAUH,CAAA;AAVG;AAAI,YAAA3K,qBAAG,CAAA,AAAPmC,QAAG,CAAA,AAAHmD,QAAG,CAAK,MAAK;AAGH,YAAA+E,MAAA,GAAAJ,OAAE,CAAM,KAAA;AAAR,YAAAK,KAAA,EAAQ,CAAAhK,aAAA,CAAA,AAAR+J,MAAQ,CAAC,EAAC,CAAC;AAOxB,gBAAA,AAPwB,CAAApJ,UAAA;AAOxB,YAAA0J,YAAA,SAAA;AAPG,UAAAxI,QAAS,CAAA,AAAT,cAAS,CAACmI,KAAW;AACZ,UAAAjB,MAAC,CAAA,AAAD,MAAC,EAAG;AAIb,qBAAA;AAJoB,YAAAa,MAAA,GAAAD,OAAE,CAAM,KAAA;AAAR,YAAAG,MAAA,EAAS,CAAAjJ,QAAM,CAAA,AAAf+I,MAAQ,CAAO;AAAnC,cAAgB,CAAAb,MAAC,AAAD,EAAI,CAAAe,MAAe;AACjC;AAAI,gBAAApK,qBAAG,CAAA,AAAPmC,QAAG,CAAA,AAAHmD,QAAG,CAAK,IAAG;AACD,gBAAA6E,MAAA,GAAAF,OAAE,CAAM,KAAA;AAAR,gBAAAM,KAAA,EAAQ,CAAAjK,aAAA,CAAA,AAAR6J,MAAQ,CAAC,CAAAd,MAAC,CAAC;AACtB,oBAAA,AADsB,CAAApI,UAAA;AACtB,qBAAA;AADC,cAAAkB,QAAS,CAAA,AAAT,cAAS,CAACoI,KAAW,CAAC;AAFa,cAAAlB,MAAC,EAAA,AAAD,CAAAA,MAAC,AAAD,EAAK,EAAC;AAAL;AAItC;AAAI,gBAAArJ,qBAAG,CAAA,AAAPmC,QAAG,CAAA,AAAHmD,QAAG,CAAK,IAAG;AAEd,oBAAA,AAFe,CAAArE,UAAA;AAEf,gBAAA0J,YAAA,SAAA;AAAA,cAAAD,YAAA,SAAA;AAAA,cAAAlL,mBAAA,EAAA;AAAA,UAAA,AAZe,CAAA4C;AAchB,MAAAwI,eA4BC,CAAA,AA5BUzI,QAAA,EAAA0I,WAAM,CAAE,SA4BlB,IAAA,AA5B2B,OAAI,CAAA;AAAJ,IAAAzI,WAAA;AAGhB,IAAA0I,MAAW,CAAA,AAAX;AAGA,IAAAC,MAAU,CAAA,AAAV;AAUI,IAAAC,MAAc,CAAA,AAAd;AAIA,IAAAC,MAAwB,CAAA,AAAxB;AAKV,IAAAC,MAAgB,CAAA,AAAhB;AAGL,IAAA9I,WAAA,OAAA;AArBW,IAAA+I,KAAU,CAAA,AAAV;AAEa,IAAAC,KAAQ,CAAA,AAAR;AAEA,IAAAC,KAAW,CAAA,AAAX;AAEA,IAAAC,KAAW,CAAA,AAAX;AAGrB,IAAAC,KAAG,CAAA,AAAH;AAIY,IAAAC,KAAsB,CAAA,AAAtB,MAAsB;AAA9B,IAAAC,KAAG,CAAA,AAAH,aAAG;AAlBT,SAAAlM,OA0BD,KAAA,AA1BC,CAAAmM,YA0BD,CAAA;AAtBK,MAAAjI,QAAG,CAAA,AAAH,MAAgB;AAJpB;AAAI,QAAAzD,qBAAG,CAAA,AAAPmC,QAAG,CAAA,AAAHmD,QAAG,CAAK,MAAK;AACH,QAAAwF,MAAA,GAAAD,WAAM,CAAK,IAAA;AAArB,QAAA1I,QAAS,CAAA,AAAT,cAAS,CAAC2I,MAAW;AACjB,QAAA9K,qBAAG,CAAA,AAAPmC,QAAG,CAAA,AAAHmD,QAAG,CAAK,IAAG;AAED,QAAAyF,MAAA,GAAAF,WAAM,CAAI,GAAA;AAAhB,QAAApH,QAAG,EAAG,CAAAsH,MAAU;AACV,QAAAI,KAAA,GAAAN,WAAM,CAAI,GAAA;AAqBrB,YAAA,AArBqB,CAAA5J,UAAA;AAqBrB,QAAAyK,YAAA,SAAA;AArBK,MAAAhI,QAAG,CAAA,AAAH,oBAAG,EAAG,CAAAyH;AACD,QACE,CAAA1H,QAAG,AAAH,GAAO,EAAC;AAAI,QAAA2H,KAAA,GAAA1H,QAAG,AAAH,GAAO,EAAC;AAAR;AAAQ,QAAA0H,KAAA,QAAA;AAApB,SAAAA,KAAA;AACT;AAAI,UAAApL,qBAAG,CAAA,AAAPmC,QAAG,CAAA,AAAHmD,QAAG,CAAK,IAAG;AAkBd,cAAA,AAlBe,CAAArE,UAAA;AAkBf,UAAAyK,YAAA,SAAA;AAlBe,WAAA;AADH,UAEA,CAAAjI,QAAG,AAAH,GAAO,EAAC;AAAI,UAAA4H,KAAA,GAAA3H,QAAG,AAAH,GAAO,KAAI;AAAX;AAAW,UAAA2H,KAAA,QAAA;AAAvB,WAAAA,KAAA;AACT;AAAI,YAAArL,qBAAG,CAAA,AAAPmC,QAAG,CAAA,AAAHmD,QAAG,CAAK,IAAG;AAgBd,gBAAA,AAhBe,CAAArE,UAAA;AAgBf,YAAAyK,YAAA,SAAA;AAhBe,aAAA;AADH,YAEA,CAAAjI,QAAG,AAAH,GAAO,EAAC;AAAI,YAAA6H,KAAA,GAAA5H,QAAG,AAAH,GAAO,KAAI;AAAX;AAAW,YAAA4H,KAAA,QAAA;AAAvB,aAAAA,KAAA;AACT;AAAI,cAAAtL,qBAAG,CAAA,AAAPmC,QAAG,CAAA,AAAHmD,QAAG,CAAK,IAAG;AAcd,kBAAA,AAde,CAAArE,UAAA;AAcf,cAAAyK,YAAA,SAAA;AAde;AAEZ,YAAAH,KAAA,GAAApJ,QAAG,CAAA,AAAHmD,QAAG;AAAS,YAAA0F,MAAA,EAAI,CAAAxK,kBAAQ,CAAA,AAAZiD,QAAG,CAAW;AAA1B;AAAI,cAAAzD,qBAAG,CAAA,AAAPuL,KAAG,CAAK,CAAA7K,YAAA,CAAC,GAAC,CAAE,CAAAsK,MAAc,CAAE;AAY/B,kBAAA,AAZgC,CAAA/J,UAAA;AAYhC,cAAAyK,YAAA,SAAA;AAZgC,cACzB,CAAAjI,QAAG,AAAH,GAAO,CAAAC,QAAG;AACZ;AAAI,gBAAA1D,qBAAG,CAAA,AAAPmC,QAAG,CAAA,AAAHmD,QAAG,CAAK,IAAG;AAUhB,oBAAA,AAViB,CAAArE,UAAA;AAUjB,gBAAAyK,YAAA,SAAA;AAViB,gBACR,CAAAhI,QAAG,AAAH,GAAO,KAAI;AACb,gBAAA+H,KAAA,GAAAtJ,QAAG,CAAA,AAAHmD,QAAG;AAAK;AAAA,kBAAAkG,KAAA,GAAA9L,cAAsB,CAAA,AAAtBgE,QAAG,CAAI,CAAAjE,gBAAG,CAAY;AAAtB,kBAAAwL,MAAA,EAAc,CAAAzK,kBAAQ,CAAA,AAAtBgL,KAAsB,CAAE;AAA5B,kBAAAxL,qBAAG,CAAA,AAAPyL,KAAG,CAAK,CAAAR,MAAwB;AAQvC,sBAAA,AARwC,CAAAhK,UAAA;AAQxC,kBAAAyK,YAAA,SAAA;AALG;AAAI,cAAA1L,qBAAG,CAAA,AAAPmC,QAAG,CAAA,AAAHmD,QAAG,CAAK,IAAG;AAKd,kBAAA,AALe,CAAArE,UAAA;AAKf,cAAAyK,YAAA,SAAA;AAHK,MAAAR,MAAA,GAAAL,WAAM,CAAU,SAAA;AAAhB,SAAAK,MAAgB;AAClB;AAAI,UAAAlL,qBAAG,CAAA,AAAPmC,QAAG,CAAA,AAAHmD,QAAG,CAAK,IAAG;AAEd,cAAA,AAFe,CAAArE,UAAA;AAEf,UAAAyK,YAAA,SAAA;AAAA,YAAA,AA5B2B,CAAAtJ;AA4B3B,UAAA5C,mBAAA;AAED,MAAAmM,iBAKC,CAAA,AALYxJ,QAAA,EAAAyJ,aAAQ,CAAE,WAKtB,IAAA,AALiC,OAAI,CAAA;AAAJ,IAAAxJ,WAAA;AAEZ,IAAAyJ,MAAc,CAAA,AAAd;AACR,IAAAC,MAAc,CAAA,AAAd,qBAAc;AADN,IAAAC,MAAqB,CAAA,AAArB;AAGrB,IAAA3J,WAAA,OAAA;AAFa,IAAA4J,KAAiB,CAAA,AAAjB,QAAiB;AADpB,IAAA3C,MAAC,CAAA,AAAD,MAAC,EAAG;AAGd,SAAA9J,OAAA,MAAA0M,YAAA;AAAA,iBAAA;AAHqB,QAAAJ,MAAA,GAAAD,aAAQ,CAAM,KAAA;AAAd,QAAAG,MAAA,EAAe,CAAA5K,QAAM,CAAA,AAArB0K,MAAc,CAAO;AAAzC,UAAgB,CAAAxC,MAAC,AAAD,EAAI,CAAA0C,MAAqB;AAC7B,UAAAD,MAAA,GAAAF,aAAQ,CAAM,KAAA;AAAd;AAAA,YAAAI,KAAA,EAAc,CAAA1L,aAAA,CAAA,AAAdwL,MAAc,CAAC,CAAAzC,MAAC,CAAC;AAE9B,gBAAA,AAF8B,CAAApI,UAAA;AAE9B,iBAAA;AAFG,UAAAkB,QAAS,CAAA,AAAT,cAAS,CAAC6J,KAAiB,CAAC;AADa,UAAA3C,MAAC,EAAA,AAAD,CAAAA,MAAC,AAAD,EAAK,EAAC;AAAL;AAG7C,UAAA4C,YAAA;AAAA,YAAAzM,mBAAA;AAAA,UAAA,AALiC,CAAA4C;AAS3B,cA+BN,CAAA,AA/BcD,QAAA,EAAAqH,aAAQ,CAAE,WA+BxB,IAAA,AA/BmC,oBAAU,CAAA;AAAV,IAAApH,WAAA;AAyBvB,IAAA8J,MAAc,CAAA,AAAd;AACA,IAAAC,MAAc,CAAA,AAAd;AACD,IAAAC,MAAc,CAAA,AAAd,OAAc;AAvBR,IAAAC,MAAc,CAAA,AAAd;AACR,IAAAC,MAAa,CAAA,AAAb;AAMY,IAAAC,MAAgB,CAAA,AAAhB;AACX,IAAAC,MAAa,CAAA,AAAb;AAGU,IAAAC,MAAY,CAAA,AAAZ,MAAY;AAFf,IAAAC,MAAgB,CAAA,AAAhB;AAWE,IAAAC,MAAY,CAAA,AAAZ;AACP,IAAAC,MAAqB,CAAA,AAArB;AACA,IAAAC,MAAqB,CAAA,AAArB;AACD,IAAAC,MAAqB,CAAA,AAArB,oBAAqB;AAzB1B,IAAAC,KAAU,CAAA,AAAV,OAAU;AAAV,IAAAC,KAAU,CAAA,AAAV;AAkBC,IAAAC,KAAG,CAAA,AAAH,oBAAG;AAfc,IAAAC,KAElB,CAAA,AAFkB;AAmBlB,IAAAC,KAAS,CAAA,AAAT,OAAS;AAAT,IAAAC,KAAS,CAAA,AAAT,YAAS;AAtBK,IAAAC,KAoBhB,CAAA,AApBgB,oBAoBhB;AApBE;AAAA,MAAA/N,aAAU,CAAA,AADRkK,aAAQ,CACV,CAAApG,UAAU,CAAA;AAAV,MAAA2J,KAAA,OAAU;AAAV,UAAU,CAAA9L,UAAA,CAAA;AAAV,MAAA8L,KAAA,QAAU;AADf,SAAAxN,OA8BD,KAAA,AA9BC,CAAA+N,YA8BD,CAAA;AA7BM,SAAAP,KAAU,CAAA;AAAV;AAAA,UAAAC,KAAA,GAAA1N,aAAU,CAAA,AADRkK,aAAQ,CACV,CAAApG,UAAU,CAAA;AA6BhB,cAAA,AA7BgB,CAAAnC,UAAA;AA6BhB,UAAAqM,YAAA,SAAA;AA3BiB,QAAAjB,MAAA,GAAAW,KAAQ,CAAM,KAAA;AAAtB,QAAA3J,UAAK,CAAA,AAAL,MAAK,EAAG,CAAAgJ;AACR,QAAAC,MAAA,MAAa,AAAb,CAAAjJ,UAAa;AAHF,UAGX,CAAAiJ,MAAa;AACf,UAAAY,KAAA,OAAI;AAAJ;AAGI,UAAAxJ,QAAG,CAAA,AAAH,MAAG,EAAG;AAEI,UAAA6I,MAAA,EAAM,CAAArM,uBAAU,CAAA,AAAhBmD,UAAK,CAAW;AAAxB,UAAA6E,UAAK,CAAA,AAAL,OAAK,EAAG,CAAAqE;AASd,qBAAA;AARG,YAAAC,MAAA,GAAAtE,UAAK,CAAQ,QAAA;AAFhB,cAEE,CAAA9H,aAAC,CAAAoM,MAAa;AAGH,cAAAC,MAAA,EAAM,AAAN,CAAAvE,UAAK,CAAA,AAAL,IAAU,EAAE;AAAnB,cAAAqF,SAAI,CAAA,AAAJ,MAAI,EAAG,CAAAd;AAAY,gBACnB,CAAAc,SAAI,AAAJ,EAAO,CAAA7J,QAAG;AACZ,gBAAAA,QAAG,EAAG,CAAA6J,SAAI;AAJJ,cAAAb,MAAA,EAAM,AAAN,CAAAxE,UAAK,CAAA,AAAL,OAAa,CAAC,CAAC,CAAC;AAAxB,cAAAA,UAAK,EAAG,CAAAwE,MAAgB;AAAnB;AAOP,mBAAG;AAAH,UAAAO,KAAA,GAAAvJ,QAAG;AAbE,UAAAwJ,KAAA,GAAAD,KAcN;AAnBc,QAAAI,KAAA,GAAAH,KAoBhB;AApBgB;AAsBd;AAAA,UAAA5N,aAAS,CAAA,AAvBPkK,aAAQ,CAuBV,CAAAhG,SAAS,CAAA;AAAT,UAAA2J,KAAA,OAAS;AAAT,cAAS,CAAAlM,UAAA,CAAA;AAAT,UAAAkM,KAAA,QAAS;AAAT,WAAAA,KAAS,CAAA;AAAT;AAAA,YAAAC,KAAA,GAAA9N,aAAS,CAAA,AAvBPkK,aAAQ,CAuBV,CAAAhG,SAAS,CAAA;AAOf,gBAAA,AAPe,CAAAvC,UAAA;AAOf,YAAAqM,YAAA,SAAA;AAPmB,UAAAX,MAAA,GAAAS,KAAQ,CAAI,GAAA;AAAZ,UAAAC,KAAA,GAAAV,MAAY;AAAhB,YACZ,CAAA7M,eAAK,CAAA,AAxBA0J,aAAQ,CAwBb,CAAAvC,KAAK;AAAI,UAAAiF,MAAA,EAAI,CAAAhM,uBAAU,CAAA,AAAd,GAAG,CAAW;AAAd,UAAA0M,MAAA,EAAe,AAAf,CAAAV,MAAc,CAAA,AAAd,IAAmB,EAAE;AAArB,UAAAmB,KAAA,GAAAT,MAAqB;AADlB,YAEZ,CAAA9M,eAAK,CAAA,AAzBA0J,aAAQ,CAyBb,CAAAtC,KAAK;AAAI,UAAAiF,MAAA,EAAI,CAAAjM,uBAAU,CAAA,AAAd,GAAG,CAAW;AAAd,UAAA2M,MAAA,EAAe,AAAf,CAAAV,MAAc,CAAA,AAAd,IAAmB,EAAE;AAArB,UAAAkB,KAAA,GAAAR,MAAqB;AAFlB,YAGZ,CAAA/M,eAAI,CAAA,AA1BC0J,aAAQ,CA0Bb,CAAArC,IAAI;AAAI,UAAAiF,MAAA,EAAI,CAAAlM,uBAAU,CAAA,AAAd,GAAG,CAAW;AAAd,UAAA4M,MAAA,EAAe,AAAf,CAAAV,MAAc,CAAA,AAAd,IAAmB,EAAE;AAArB,UAAAiB,KAAA,GAAAP,MAAqB;AAEjB,aAAA;AAAJ,UAAAO,KAAA,OAAI;AA5Bd,UAAA;AADkC,QAAAjL,WAAA,EAClC,CAAAiL,KA6BC;AACF,cAAA,AA/BmC,CAAAjL;AA+BnC,aAAAnB,UAAA;AAAA,YAAA;AAAA,UAAAzB,mBAAA,EAAA;AAnMkB,MAAA0D,gBAAA,CAAAf,QAAA,CACf,CAAAmD,GAAG,CAAE,aAAmB,EAAA,AAA5B,IAAwD,AADrC,IAAA,A,C,I;AACf,IAAAA,QAAG,CAAE,aAAmB,EAAA,AAAxB,CAAAA,GAAG;AADY,IAAAlD,WACqC,CAAA,AADrC,OACqC;AAAzB,IAAAoL,MAAyB,CAAA,AAAzB;AAAyB,IAAApL,WAAA,OAAA;AAApD,MAA2B,AAA3B,CAAAkD,QAAG,AAAH,GAA2B,IAAyB,CAAA;AAAzB,MAAAkI,MAAA,EAAI,CAAAnM,SAAmB,EAAE;AAApD,MAAAiE,QAAG,EAAwB,CAAAkI,MAAyB;AAApD,IAAArL,QAAA,CAAAmD,QAAG,EAAA,AAAH,CAAAA;AAAoD,UAAA,AADrC,CAAAlD,WACqC;AADpD,KAAe,UAAAD,QAAA,CACf,CAAAmD,GAAG,CAAE,aAAmB,EAAA,AAA5B,IAAwD,AADrC;AACf,IAAAA,QAAG,CAAE,aAAmB,EAAA,AAAxB,CAAAA,GAAG;AADY,IAAAnD,QAAA,CAAAe,gBAAA,CACfoC,QAAoD,CAAA;AAhP5B,MAAAuB,SAAA,CAAAvD,OAAsB,EAAA;AAAtB,WAAsB,EAAA,AAAtB;AAAsB,MAAAJ,gBAAA,CAAAf,QAAA,IAAA,A,C,I;AAAA,IAAAC,UAAA;AAAA,IAAAA,UAAA;AAAA,WAAAA,UAAA;AAAtB,KAAsB,UAAAD,QAAA;AAAA,IAAAA,QAAA,CAAAe,gBAAA;AAAIuK,MAAW,CAAA,AAAX,YAAW,EAAA,AAAP,CAAA5G,SAAK,EAAE;AAAxDA,KAAK,CAAA,AAAL,YAAK,EAAG,CAAA4G;AACS,MAAA3G,OAAA,CAAAxD,OAAoB,EAAA;AAApB,WAAoB,EAAA,AAApB;AAAoB,MAAAJ,gBAAA,CAAAf,QAAA,IAAA,A,C,I;AAAA,IAAAC,UAAA;AAAA,IAAAA,UAAA;AAAA,WAAAA,UAAA;AAApB,KAAoB,UAAAD,QAAA;AAAA,IAAAA,QAAA,CAAAe,gBAAA;AAAIwK,MAAS,CAAA,AAAT,UAAS,EAAA,AAAL,CAAA5G,OAAG,EAAE;AAAlDA,GAAG,CAAA,AAAH,UAAG,EAAG,CAAA4G;AACW,MAAA3G,OAAA,CAAAzD,OAAoB,EAAA;AAApB,WAAoB,EAAA,AAApB;AAAoB,MAAAJ,gBAAA,CAAAf,QAAA,IAAA,A,C,I;AAAA,IAAAC,UAAA;AAAA,IAAAA,UAAA;AAAA,WAAAA,UAAA;AAApB,KAAoB,UAAAD,QAAA;AAAA,IAAAA,QAAA,CAAAe,gBAAA;AAAIyK,MAAS,CAAA,AAAT,UAAS,EAAA,AAAL,CAAA5G,OAAG,EAAE;AAAlDA,GAAG,CAAA,AAAH,UAAG,EAAG,CAAA4G;AAMT,MAAA3G,gBAAA,CAAA1D,OAA6B,EAAA;AAA7B,WAA6B,EAAA,AAA7B;AAA6B,MAAAJ,gBAAA,CAAAf,QAAA,IAAA,A,C,I;AAAA,IAAAC,UAAA;AAAA,IAAAA,UAAA;AAAA,WAAAA,UAAA;AAA7B,KAA6B,UAAAD,QAAA;AAAA,IAAAA,QAAA,CAAAe,gBAAA;AAAI0K,MAAkB,CAAA,AAAlB,mBAAkB,EAAA,AAAd,CAAA5G,gBAAY,EAAE;AADhDA,aAAY,CAAA,AAAZ,mBAAY,EAAG,CAAA4G;AAKI,MAAA3G,SAAA,CAAA1D,UAAyB,EAAA;AAAzB,WAAyB,EAAA,AAAzB;AAAyB,MAAAL,gBAAA,CAAAf,QAAA,IAAA,A,C,I;AAAA,IAAAC,UAAA;AAAA,IAAAA,UAAA;AAAA,WAAAA,UAAA;AAAzB,KAAyB,UAAAD,QAAA;AAAA,IAAAA,QAAA,CAAAe,gBAAA;AAAI2K,MAAW,CAAA,AAAX,YAAW,EAAA,AAAP,CAAA5G,SAAK,EAAE;AAA3DA,KAAK,CAAA,AAAL,YAAK,EAAG,CAAA4G;AACW,MAAA3G,SAAA,CAAA3D,UAAyB,EAAA;AAAzB,WAAyB,EAAA,AAAzB;AAAyB,MAAAL,gBAAA,CAAAf,QAAA,IAAA,A,C,I;AAAA,IAAAC,UAAA;AAAA,IAAAA,UAAA;AAAA,WAAAA,UAAA;AAAzB,KAAyB,UAAAD,QAAA;AAAA,IAAAA,QAAA,CAAAe,gBAAA;AAAI4K,MAAW,CAAA,AAAX,YAAW,EAAA,AAAP,CAAA5G,SAAK,EAAE;AAA3DA,KAAK,CAAA,AAAL,YAAK,EAAG,CAAA4G;AACU,MAAA3G,QAAA,CAAA5D,UAAwB,EAAA;AAAxB,WAAwB,EAAA,AAAxB;AAAwB,MAAAL,gBAAA,CAAAf,QAAA,IAAA,A,C,I;AAAA,IAAAC,UAAA;AAAA,IAAAA,UAAA;AAAA,WAAAA,UAAA;AAAxB,KAAwB,UAAAD,QAAA;AAAA,IAAAA,QAAA,CAAAe,gBAAA;AAAI6K,MAAU,CAAA,AAAV,WAAU,EAAA,AAAN,CAAA5G,QAAI,EAAE;AAAxDA,IAAI,CAAA,AAAJ,WAAI,EAAG,CAAA4G;AA2EX,GAAI,CAAAC,MAAM,CAAA,AAAC/K,SAAI,CAAE,QAEvB,IAAA,AAF+B,QAAK;AACrB,SAAA4D,KAAK,CAAQ,CAAAE,GAAG;AADA,EAAA3E,UAAA;AAC9B,EAAA6L,MAAgC,CAAA,AAAhC,QAAgC,EAAA,AAA5B,CAAAhK,QAAQ,CAAC,CAAC4C,KAAK,CAAE,CAAA5D,SAAI,CAAE,CAAA8D,GAAG,CAAC,CAAC;AADF,EAAA3E,UAAA,EAC9B,CAAA6L,MAAgC;AACjC,QAAA,AAF+B,CAAA7L;AAIzB,GAAI,CAAA8L,WAAS,CAAA,AAACjL,SAAI,CAAE,QAAK,CAAE,CAAAe,SAAS,CAAE,OAAO,EAAA,AAAlB,IAEjC,IAAA,AAF8D,SAAM,CAAA;AAAnC,EAAAA,cAAS,CAAE,OAAO,EAAA,AAAlB,CAAAA;AAA6B,EAAA5B,UAAA,UAAM;AAAd,IAAA,AAArB,CAAA4B,cAAS,AAAT,GAAqB,IAAK,CAAA;AAA1B,IAAAA,cAAS,EAAY,MAAK;AAC1D,EAAAmK,MAAsC,CAAA,AAAtC,SAAsC,EAAA,AAApC,CAAApK,MAAA,CAAAd,SAAI,CAAO,EAAC,CAAO,KAAI,CAAE,CAAAe,cAAS,CAAE;AADuB,EAAA5B,UAAA,EAC7D,CAAA+L,MAAsC;AACvC,QAAA,AAF8D,CAAA/L;AAIxD,GAAI,CAAAgM,QAAQ,CAAA,AAACnL,SAAI,CAAE,QAAK,CAAE,CAAAe,SAAS,CAAE,OAAO,EAAA,AAAlB,IAEhC,IAAA,AAF6D,SAAM,CAAA;AAAnC,EAAAA,cAAS,CAAE,OAAO,EAAA,AAAlB,CAAAA;AAA6B,EAAA5B,UAAA,UAAM;AAAd,IAAA,AAArB,CAAA4B,cAAS,AAAT,GAAqB,IAAK,CAAA;AAA1B,IAAAA,cAAS,EAAY,MAAK;AACzD,EAAAqK,MAAmC,CAAA,AAAnC,SAAmC,EAAA,AAAjC,CAAAtK,MAAA,CAAAd,SAAI,CAAO,EAAC,CAAO,EAAC,CAAE,CAAAe,cAAS,CAAE;AADyB,EAAA5B,UAAA,EAC5D,CAAAiM,MAAmC;AACpC,QAAA,AAF6D,CAAAjM;AAiD9CkM,MAAe,CAAA,AAAf,gBAAe,EAAA,AAAX,CAAAlK,aAAS,EAAE;AAA3Ba,cAAS,CAAA,AAAT,gBAAS,EAAG,CAAAqJ,MAAe;AApR/BlM,WAAA,UAiXM,6GAAc,CAAA,AAAd,eAAc,EAAA,AAAd,CAAc,CAAA;AAoMnB,SAAAA",
     "names": [
-        "isinstance",
-        "Exception",
-        "len",
-        "len#1273",
-        "list",
-        "list#1285",
-        "ABC",
         "TemperObject",
         "cast_by_type",
         "Label",
         "NoResultException",
         "isinstance_int",
         "cast_by_test",
         "list_join",
-        "list_join#1264",
+        "list_join#1213",
         "generic_eq",
-        "generic_eq#1266",
+        "generic_eq#1222",
         "list_builder_add",
-        "list_builder_add#1267",
+        "list_builder_add#1215",
         "string_code_points",
-        "string_code_points#1239",
+        "string_code_points#1225",
         "bool_not",
-        "bool_not#1270",
-        "generic_lt",
-        "generic_lt#1274",
+        "bool_not#1214",
         "list_get",
-        "list_get#1275",
+        "list_get#1231",
         "int_to_string",
-        "int_to_string#1240",
+        "int_to_string#1241",
         "str_cat",
-        "str_cat#1241",
-        "generic_not_eq",
-        "generic_not_eq#1281",
-        "generic_gt_eq",
-        "generic_gt_eq#1284",
+        "str_cat#1212",
+        "Union",
+        "NoReturn",
+        "Callable",
+        "Any",
+        "Tuple",
+        "List",
+        "Exception",
+        "len",
+        "len#1230",
+        "list",
+        "list#1210",
         "compiled_regex_compile_formatted",
-        "compiled_regex_compile_formatted#1260",
-        "compiled_regex_compiled_found_in",
-        "compiled_regex_compiled_found_in#1261",
+        "compiled_regex_compile_formatted#1216",
+        "compiled_regex_compiled_found",
+        "compiled_regex_compiled_found#1217",
         "compiled_regex_compiled_find",
-        "compiled_regex_compiled_find#1262",
+        "compiled_regex_compiled_find#1218",
+        "compiled_regex_compiled_replace",
+        "compiled_regex_compiled_replace#1219",
         "regex_formatter_push_capture_name",
-        "regex_formatter_push_capture_name#1268",
+        "regex_formatter_push_capture_name#1223",
         "regex_formatter_push_code_to",
-        "regex_formatter_push_code_to#1269",
+        "regex_formatter_push_code_to#1224",
         "Regex",
-        "x#1245",
-        "CodePart",
-        "x#1247",
-        "Special",
-        "x#1249",
-        "SpecialSet",
-        "x#1250",
         "this",
-        "t#1230",
-        "CompiledRegex",
         "return",
+        "t#1201",
+        "CompiledRegex",
         "text",
-        "t#1227",
-        "t#1228",
-        "t#1225",
-        "t#865",
+        "t#1198",
+        "t#1199",
+        "t#836",
+        "t#1196",
+        "format",
+        "t#1193",
+        "t#1194",
         "Capture",
-        "args#1246",
-        "constructor",
         "name",
         "item",
-        "getname",
-        "getitem",
+        "constructor",
+        "CodePart",
         "CodePoints",
-        "args#1248",
         "value",
-        "getvalue",
+        "Special",
+        "SpecialSet",
         "CodeRange",
-        "args#1251",
         "min",
         "max",
-        "getmin",
-        "getmax",
         "CodeSet",
-        "args#1252",
         "items",
         "negated",
-        "getitems",
-        "getnegated",
         "Or",
-        "args#1253",
         "Repeat",
-        "args#1254",
         "reluctant",
-        "getreluctant",
         "Sequence",
-        "args#1255",
-        "Match",
-        "args#1256",
-        "groups",
-        "getgroups",
         "Group",
-        "args#1257",
         "codePointsBegin",
-        "getcodePointsBegin",
         "RegexRefs",
-        "args#1258",
         "codePoints",
-        "match",
+        "group",
         "orObject",
-        "t#1174",
-        "t#1176",
-        "t#1178",
-        "t#1179",
-        "getcodePoints",
-        "getmatch",
-        "getorObject",
-        "args#1259",
+        "t#1145",
+        "t#1147",
+        "t#1149",
         "data",
-        "t#1168",
-        "t#1169",
         "compiled",
-        "t#1167",
-        "t#824",
+        "t#1139",
+        "t#1140",
+        "t#1138",
+        "t#795",
         "regexRefs",
-        "t#1160",
+        "t#1135",
+        "t#1128",
         "RegexFormatter",
-        "t#1161",
-        "getdata",
-        "args#1263",
-        "regex",
-        "t#1156",
+        "t#1129",
         "out",
+        "regex",
+        "t#1124",
         "fn",
         "x",
-        "t#1155",
-        "t#1157",
-        "t#785",
-        "s#1265",
-        "t#786",
-        "t#789",
-        "t#790",
-        "t#793",
-        "t#794",
-        "t#797",
-        "t#798",
-        "t#801",
-        "t#802",
-        "t#805",
-        "t#806",
-        "t#809",
-        "t#810",
+        "t#1123",
+        "t#1125",
+        "pushRegex",
+        "t#755",
+        "t#756",
+        "t#759",
+        "t#760",
+        "t#763",
+        "t#764",
+        "t#767",
+        "t#768",
+        "t#771",
+        "t#772",
+        "t#775",
+        "t#776",
+        "t#779",
+        "t#780",
+        "s__1220#1221",
         "Begin",
         "Dot",
         "End",
         "WordBoundary",
         "Digit",
         "Space",
         "Word",
+        "pushCapture",
         "capture",
-        "t#780",
-        "t#1138",
-        "t#1140",
+        "t#1106",
+        "t#1108",
+        "t#750",
+        "pushCode",
         "code",
         "insideCodeSet",
-        "t#1126",
-        "t#1132",
+        "pushCodePoints",
+        "t#1096",
+        "t#1097",
+        "t#1098",
+        "t#1095",
+        "t#1100",
         "slice",
-        "t#1127",
-        "t#1131",
-        "t#1128",
-        "t#1129",
+        "pushCodeRange",
         "codeRange",
-        "t#1119",
-        "t#1121",
+        "pushCodeRangeUnwrapped",
+        "t#1090",
+        "t#1088",
+        "pushCodeSet",
         "codeSet",
-        "t#1111",
+        "t#1082",
+        "t#1083",
+        "t#1085",
+        "t#1086",
+        "t#720",
+        "t#721",
+        "t#727",
+        "t#1080",
         "adjusted",
-        "t#747",
-        "s#1271",
-        "s#1272",
-        "t#748",
-        "t#1117",
+        "s__1226#1228",
+        "s__1227#1229",
         "i",
-        "t#1113",
-        "t#1116",
-        "t#753",
-        "t#1114",
-        "t#756",
-        "t#754",
+        "adjustCodeSet",
+        "pushCodeSetItem",
         "codePart",
-        "t#734",
-        "s#1276",
-        "t#735",
-        "t#738",
-        "t#739",
-        "t#742",
-        "t#743",
-        "or",
-        "t#1096",
-        "t#1104",
-        "t#1103",
-        "s#1278",
-        "s#1279",
-        "t#1101",
-        "t#722",
-        "t#1097",
-        "t#1100",
-        "t#726",
-        "t#1098",
-        "t#729",
-        "t#727",
-        "repeat",
-        "s#1280",
-        "t#1089",
-        "t#1091",
-        "t#700",
-        "t#701",
-        "t#703",
-        "t#705",
+        "t#707",
         "t#708",
-        "t#1092",
         "t#711",
-        "t#709",
-        "t#1093",
-        "t#1094",
-        "sequence",
-        "s#1282",
-        "t#1084",
-        "t#1087",
-        "t#691",
-        "t#1085",
-        "t#694",
-        "t#692",
-        "t#663",
-        "s#1283",
-        "t#664",
-        "t#1073",
-        "t#1074",
-        "t#674",
-        "t#1075",
-        "t#1076",
-        "t#1079",
-        "t#1077",
-        "next",
-        "t#672",
-        "t#1078",
-        "t#673",
-        "t#688",
-        "t#678",
-        "t#679",
-        "t#1080",
+        "t#712",
+        "t#715",
+        "t#716",
+        "s__1232#1233",
+        "pushOr",
+        "or",
+        "t#1067",
+        "t#1068",
         "t#1070",
-        "t#1081",
         "t#1071",
-        "t#1082",
-        "t#1072",
-        "t#1083",
+        "t#697",
+        "t#702",
         "t#1066",
-        "args#1286",
-        "t#1231",
-        "args#1287",
-        "t#1232",
-        "args#1288",
-        "t#1233",
-        "args#1289",
-        "t#1234",
-        "args#1290",
-        "t#1235",
-        "args#1291",
-        "t#1236",
-        "args#1292",
-        "t#1237",
+        "t#1073",
+        "s__1234#1237",
+        "s__1235#1238",
+        "pushRepeat",
+        "repeat",
+        "t#1059",
+        "t#1061",
+        "t#1062",
+        "t#1063",
+        "t#1064",
+        "t#676",
+        "t#677",
+        "t#679",
+        "t#681",
+        "t#684",
+        "t#685",
+        "t#687",
+        "s__1239#1240",
+        "pushSequence",
+        "sequence",
+        "t#1054",
+        "t#1055",
+        "t#1057",
+        "t#670",
+        "s__1242#1243",
+        "t#1041",
+        "t#1042",
+        "t#1043",
+        "t#1044",
+        "t#1045",
+        "t#1046",
+        "t#1047",
+        "t#1048",
+        "t#1049",
+        "t#1050",
+        "t#1051",
+        "t#1052",
+        "t#1053",
+        "t#643",
+        "t#644",
+        "t#651",
+        "t#652",
+        "t#656",
+        "t#657",
+        "t#666",
+        "s__1244#1245",
+        "next",
+        "t#1037",
+        "t#1202",
+        "t#1203",
+        "t#1204",
+        "t#1205",
+        "t#1206",
+        "t#1207",
+        "t#1208",
         "entire",
-        "t#1197",
+        "t#1165",
         "oneOrMore",
-        "t#1195",
+        "t#1163",
         "optional",
-        "t#1192",
-        "t#1238"
+        "t#1160",
+        "t#1209"
     ],
     "sources": [
         "std/regex.temper.md"
     ],
     "sourcesContent": [
-        "# Regex Data Model and Functionality\n\nThe structural data model for regex patterns enables direct construction, and\nthe Temper regex dialect compiles static regex text patterns to these objects.\n\nA focus here is on providing tools people can actually reach for when they need\nto do text processing. The execution should be faster on backends like Python\nthan writing raw code, and the implementation in backends like C should\napproximate what you'd like to have written manually.\n\nDue to inadequate and distinct Unicode handling in backend regex engines, the\ninitial feature set avoids character classes and properties but is still aware\nof code points. Parsing focused on limited sets of delimiters works best for\nnow.\n\nThe core feature set here focuses on both the data model and utility functions,\nsuch as matching regexes against strings.\n\n## Regex Data Model\n\nAll regexes are composed hierarchically of `Regex` nodes. Regexes are a\nsequence of component parts. For example, `/hi./` is a sequence of\n[CodePoint](#codepoint) `/h/` and `/i/` and dot `/./`.\n\nAnd perhaps the most fundamental `Regex` is the [Sequence](#sequence),\nbecause it enables multiple regex components to be strung together.\n\n```temper ;lit\nexport /*sealed*/ interface Regex {\n```\n\nBefore a regex is used, it must be compiled. Some helper functions compile on\nthe fly, although it is faster to reuse a pre-compiled regex.\n\n```temper ;lit\n  // TODO(tjp, regex): Make this into a macro behind the scenes.\n  // TODO(tjp, regex): `compiled<T>(): CompiledRegex<T>`\n  public compiled(): CompiledRegex { new CompiledRegex(this) }\n```\n\nThe simplest use of a regular expression is if it is found in a string.\nRepeatedly calling these methods on a single `Regex` instance is inefficient.\nBetter for reuse is to compile in advance.\n\n```temper ;lit\n  public foundIn(text: String): Boolean { compiled().foundIn(text) }\n```\n\n```temper ;lit\n  // TODO(tjp, regex): Also macro because reification.\n  // TODO(tjp, regex): `find<T>(): Match<T> | NoResult`\n  public find(text: String): Match | NoResult { compiled().find(text) }\n```\n\nThat's it for what you can do with regex patterns in Temper today, but there's\nmuch more to say on what kinds of regexes can be built.\n\n```temper ;lit\n}\n```\n\n## Regex Item Types\n\nA `Regex` is composed of a potential variety of subtypes.\n\n### Groups\n\nMultiple types of groups exist:\n\n- [Capture](#capture) `/(?<name>...)/` to remember match groups for later use.\n- Non-capturing group syntax `/(?:...)/`, which is simply a [Regex](#regex)\n  instance in the data model.\n\n### Capture\n\nTODO(tjp, regex): Change to named captures only!\n\n`Capture` is a [group](#groups) that remembers the matched text for later\naccess. Temper supports only named matches, with current intended syntax\n`/(?name = ...)/`.\n\n```temper ;lit\nexport class Capture extends Regex {\n  public name: String;\n  public /*early*/ item: Regex;\n}\n```\n\n### CodePart\n\nA component of a [CodeSet][#codeset], aka character class, which applies to a\nsubset of regex data types.\n\nHere, \"code\" is short for \"code point\" although \"char\" might work better,\ndepending on expectations.\n\n```temper ;lit\nexport /*sealed*/ interface CodePart extends Regex {}\n```\n\n### CodePoints\n\nOne or more verbatim code points, where the sequence matters if within a\n[Regex](#regex) or not if within a [CodeSet](#codeset). Some escapes in\ntextual regex source, such as `/\\t/`, can be stored as raw code points.\n\nThe `String` here can enable more efficient storage than individual code\npoints, although the source text may require non-capture grouping. For example,\n`/(?:abc)?/` optionally matches the string `\"abc\"`, whereas `/abc?/` matches\n`\"ab\"` with an optional `\"c\"`.\n\n```temper ;lit\nexport class CodePoints extends CodePart {\n  public value: String;\n}\n```\n\n### Specials\n\nA number of special match forms exist. In the data model, these are empty\nclasses.\n\n- `.` - `Dot` In default mode, matches any Unicode code point except newline.\n- `^` - `Begin` in default mode matches zero-length at the beginning of a\n  string.\n- `$` - `End` in default mode matches zero-length at the end of a string.\n- `\\b` - `WordBoundary` matches zero-length at the boundary between word and\n  non-word code points. More sophisticated Unicode compliance is TBD.\n- `\\s` (negated as `\\S`) - `Space` matches any horizontal space code point.\n  Details are TBD.\n- `\\w` (negated as `\\W`) - `Word` matches any word code point. Details are TBD.\n  This is currently defined in terms of old ASCII definitions because those are\n  clear. Perhaps this will stay that way, and Unicode properties like `\\p{L}`\n  will be used for human language needs.\n- `\\X` - `GraphemeCluster` might not be supported, but [here is some discussion\n  of how to implement it](\n  https://github.com/rust-lang/regex/issues/54#issuecomment-661905060).\n\n<details>\n\n```temper ;lit\nexport /*sealed*/ interface Special extends Regex {}\nexport let Begin = do { class Begin extends Special {}; new Begin() };\nexport let Dot = do { class Dot extends Special {}; new Dot() };\nexport let End = do { class End extends Special {}; new End() };\n// TODO(tjp, regex): We can't easily support this at present across backends.\n// export let GraphemeCluster = do {\n//   class GraphemeCluster extends Special {}; new GraphemeCluster()\n// };\nexport let WordBoundary = do {\n  class WordBoundary extends Special {}; new WordBoundary()\n};\n\nexport /*sealed*/ interface SpecialSet extends CodePart & Special {}\nexport let Digit = do { class Digit extends SpecialSet {}; new Digit() };\nexport let Space = do { class Space extends SpecialSet {}; new Space() };\nexport let Word = do { class Word extends SpecialSet {}; new Word() };\n```\n\n</details>\n\n### CodeRange\n\nA code point range matches any code point in its inclusive bounds, such as\n`/[a-c]/`. In source, `-` is included in a code set either by escaping or by\nincluding it as the first or last character. A `CodeRange` is usually contained\ninside a [CodeSet](#codeset), and syntactically always is.\n\n```temper ;lit\nexport class CodeRange extends CodePart {\n  public min: Int;\n  public max: Int;\n}\n```\n\n### CodeSet\n\nA set of code points, any of which can match, such as `/[abc]/` matching any of\n`\"a\"`, `\"b\"`, or `\"c\"`. Alternatively, a negated set is the inverse of the code\npoints given, such as `/[^abc]/`, matching any code point that's not any of\nthese. This is also often called a character class.\n\nFurther, a subset of [specials](#specials) can also be used in code sets. A\nnegated code set of just a special set often has custom syntax. For example,\nnon-space can be said as either `/[^\\s]/` or `/\\S/`.\n\n```temper ;lit\nexport class CodeSet extends Regex {\n  public items: List<CodePart>;\n  public negated: Boolean = false;\n}\n```\n\n### Or\n\n`Or` matches any one of multiple options, such as `/ab|cd|e*/`.\n\n```temper ;lit\nexport class Or extends Regex {\n  public /*early*/ items: List<Regex>;\n}\n```\n\n### Repeat\n\n`Repeat` matches from an minimum to a maximum number of repeats of a\nsubregex. This can be represented in regex source in a number of ways:\n\n- `?` matches 0 or 1.\n- `*` matches 0 or more.\n- `+` matches 1 or more.\n- `{m}` matches exactly `m` repetitions.\n- `{m,n}` matches between `m` and `n`. Missing `n` is a max of infinity. For\n  example, `{0,1}` is equivalent to `?`, and `{1,}` is equivalent to `+`.\n\nBy default, repetitions are greedy, matching as many repetitions as possible.\nIn regex source, any of the above can have `?` appended to indicated reluctant\n(aka non-greedy), matching as few repetitions as possible.\n\n```temper ;lit\nexport class Repeat extends Regex {\n  public /*early*/ item: Regex;\n  public min: Int;\n  public max: Int | Null; // where null means infinite\n  public reluctant: Boolean = false;\n}\n```\n\nWe also have convenience builders.\n\n```temper ;lit\nexport let entire(item: Regex): Regex {\n  new Sequence([Begin, item, End])\n}\n\nexport let oneOrMore(item: Regex, reluctant: Boolean = false): Repeat {\n  { item, min: 1, max: null, reluctant }\n}\n\nexport let optional(item: Regex, reluctant: Boolean = false): Repeat {\n  { item, min: 0, max: 1, reluctant }\n}\n```\n\n### Sequence\n\n`Sequence` strings along multiple other regexes in order.\n\n```temper ;lit\nexport class Sequence extends Regex {\n  public /*early*/ items: List<Regex>;\n}\n```\n\n## Match Objects\n\nFor detailed match results, call `find` on a regex to get a `Match` object.\n\n```temper ;lit\n// TODO(tjp, regex): Generate subtypes of this interface later.\n// TODO(tjp, regex): If we can keep this to `groups` only, can we make the\n// TODO(tjp, regex): groups list or object the whole match value?\nexport class Match { // interface ... <T> {\n  // TODO(tjp, regex): After custom, do we still also want a generic group list?\n  /**\n   * By default, includes a \"full\" group at index 0 for the full match. If\n   * another \"full\" capture is defined, the default is excluded. Keeping the\n   * full match uniform with other named groups enables unification, including\n   * with custom match types.\n   */\n  public let groups: List<Group>;\n  // TODO(tjp, regex): Custom capture storage goes here once we're ready.\n  // public let storage: T;\n}\n\nexport class Group {\n  public let name: String;\n  public let value: String;\n  public let codePointsBegin: Int;\n}\n```\n\n## Compiled Regex Objects\n\nThe compiled form of a regex is mostly opaque, but it can be cached for more\nefficient reuse than working from a source [Regex](#regex-data-model).\n\n<details>\n\n```temper ;lit\n// Provides a workaround for access to std/regex from extension methods.\nclass RegexRefs {\n  public let codePoints: CodePoints = new CodePoints(\"\");\n  public let match: Match = {\n    groups: [{ name: \"\", value: \"\", codePointsBegin: 0 }],\n  };\n  public let orObject: Or = new Or([]);\n}\n\nlet regexRefs = new RegexRefs();\n```\n\n</details>\n\n```temper ;lit\n// TODO(tjp, regex): Generate subtypes of this interface later.\nexport class CompiledRegex { // interface ... <T> {\n```\n\nThe source `Regex` data is still available on compiled objects in case it's\nneeded for composition or other purposes.\n\n```temper ;lit\n  public let data: Regex;\n\n  public constructor(data: Regex): Void {\n    this.data = data;\n    compiled = compileFormatted(format());\n  }\n```\n\nA compiled regex exposes many of the same capabilities as `Regex`, but they are\nmore efficient to use repeatedly.\n\n```temper ;lit\n  public foundIn(text: String): Boolean { compiledFoundIn(compiled, text) }\n```\n\n```temper ;lit\n  public let find(text: String): Match | NoResult {\n    compiledFind(compiled, text, regexRefs)\n  }\n```\n\nTODO(tjp, regex): Public method for replace with named references.\nTODO(tjp, regex): Any static checking?\n\n<details>\n\n```temper ;lit\n  let compiled: AnyValue;\n\n  // Extension functions on some backends need the private `compiled` value\n  // passed in directly.\n  @extension(\"CompiledRegex::compiledFoundIn\")\n  compiledFoundIn(compiled: AnyValue, text: String): Boolean;\n\n  @extension(\"CompiledRegex::compiledFind\")\n  compiledFind(\n    compiled: AnyValue, text: String, regexRefs: RegexRefs\n  ): Match | NoResult;\n\n  @extension(\"CompiledRegex::compileFormatted\")\n  compileFormatted(formatted: String): AnyValue;\n\n  @extension(\"CompiledRegex::format\")\n  format(): String { new RegexFormatter().format(data) }\n```\n\n</details>\n\n```temper ;lit\n}\n```\n\n## Private implementation matters\n\nSome regex logic can be shared across backends. These features aren't directly\nexported to the user, however.\n\nThe intent is that these support features only get included in compiled Temper\ncode if usage depends on dynamically constructed regexes. If all regex building\nis done as stable values, we hope to generated backend compiled regexes purely\nat Temper compile time.\n\n### RegexFormatter\n\n<details>\n\n```temper ;lit\nclass RegexFormatter {\n  let out: ListBuilder<String> = new ListBuilder<String>();\n\n  public format(regex: Regex): String {\n    pushRegex(regex)\n    out.join(\"\") { (x);; x }\n  }\n\n  pushRegex(regex: Regex): Void {\n    match (regex) {\n      // Aggregate types.\n      is Capture -> pushCapture(regex);\n      is CodePoints -> pushCodePoints(regex, false);\n      is CodeRange -> pushCodeRange(regex);\n      is CodeSet -> pushCodeSet(regex);\n      is Or -> pushOr(regex);\n      is Repeat -> pushRepeat(regex);\n      is Sequence -> pushSequence(regex);\n      // Specials.\n      // Some of these will need customized on future backends.\n      Begin -> out.add(\"^\");\n      Dot -> out.add(\".\");\n      End -> out.add(\"$\");\n      WordBoundary -> out.add(\"\\\\b\");\n      // Special sets.\n      Digit -> out.add(\"\\\\d\");\n      Space -> out.add(\"\\\\s\");\n      Word -> out.add(\"\\\\w\");\n      // ...\n    }\n  }\n\n  pushCapture(capture: Capture): Void {\n    out.add(\"(\");\n    // TODO(tjp, regex): Consistent name validation rules for all backends???\n    // TODO(tjp, regex): Validate here or in `Capture` constructor???\n    // TODO(tjp, regex): Validate here or where against reused names???\n    pushCaptureName(out, capture.name);\n    pushRegex(capture.item);\n    out.add(\")\");\n  }\n\n  @extension(\"RegexFormatter::pushCaptureName\")\n  pushCaptureName(out: ListBuilder<String>, name: String): Void {\n    // All so far except Python use this form.\n    out.add(\"?<${name}>\");\n  }\n\n  pushCode(code: Int, insideCodeSet: Boolean): Void {\n    // Expose private property to extension.\n    pushCodeTo(out, code, insideCodeSet);\n    // TODO(tjp, regex): Implement more in Temper once we can.\n    // if (escapeCodes[code] && false) {\n    //   out.add(\"\\\\\");\n    //   // TODO(tjp, regex): How to convert back to strings?\n    // }\n  }\n\n  @extension(\"RegexFormatter::pushCodeTo\")\n  pushCodeTo(out: ListBuilder<String>, code: Int, insideCodeSet: Boolean): Void;\n\n  pushCodePoints(codePoints: CodePoints, insideCodeSet: Boolean): Void {\n    for (\n      var slice = codePoints.value.codePoints;\n      !slice.isEmpty;\n      slice = slice.advance(1)\n    ) {\n      pushCode(slice.read(), insideCodeSet);\n    }\n  }\n\n  pushCodeRange(codeRange: CodeRange): Void {\n    out.add(\"[\");\n    pushCodeRangeUnwrapped(codeRange);\n    out.add(\"]\");\n  }\n\n  pushCodeRangeUnwrapped(codeRange: CodeRange): Void {\n    pushCode(codeRange.min, true);\n    out.add(\"-\");\n    pushCode(codeRange.max, true);\n  }\n\n  pushCodeSet(codeSet: CodeSet): Void {\n    let adjusted = adjustCodeSet(codeSet, regexRefs);\n    match (adjusted) {\n      is CodeSet -> do {\n        out.add(\"[\");\n        if (adjusted.negated) {\n          out.add(\"^\");\n        }\n        for (var i = 0; i < adjusted.items.length; i += 1) {\n          pushCodeSetItem(adjusted.items[i]);\n        }\n        out.add(\"]\");\n      }\n      else -> pushRegex(adjusted);\n    }\n  }\n\n  @extension(\"RegexFormatter::adjustCodeSet\")\n  adjustCodeSet(codeSet: CodeSet, regexRefs: RegexRefs): Regex { codeSet }\n\n  pushCodeSetItem(codePart: CodePart): Void {\n    match (codePart) {\n      is CodePoints -> pushCodePoints(codePart, true);\n      is CodeRange -> pushCodeRangeUnwrapped(codePart);\n      is SpecialSet -> pushRegex(codePart);\n    }\n  }\n\n  pushOr(or: Or): Void {\n    if (!or.items.isEmpty) {\n      out.add(\"(?:\");\n      // TODO(tjp, regex): See #822. Until `this` works better, no this in funs.\n      // TODO(tjp, regex): So just manually loop here. Sometimes faster, anyway?\n      pushRegex(or.items[0]);\n      for (var i = 1; i < or.items.length; i += 1) {\n        out.add(\"|\");\n        pushRegex(or.items[i]);\n      }\n      out.add(\")\");\n    }\n  }\n\n  pushRepeat(repeat: Repeat): Void {\n    // Always wrap the main sub-pattern here to make life easy\n    out.add(\"(?:\");\n    pushRegex(repeat.item);\n    out.add(\")\");\n    // Then add the repetition part.\n    let min = repeat.min;\n    let max = repeat.max;\n    if (false) {\n    } else if (min == 0 && max == 1) {\n      out.add(\"?\");\n    } else if (min == 0 && max == null) {\n      out.add(\"*\");\n    } else if (min == 1 && max == null) {\n      out.add(\"+\");\n    } else {\n      out.add(\"{${min.toString()}\");\n      if (min != max) {\n        out.add(\",\");\n        if (max != null) {\n          out.add(max.as<Int>().toString());\n        }\n      }\n      out.add(\"}\");\n    }\n    if (repeat.reluctant) {\n      out.add(\"?\");\n    }\n  }\n\n  pushSequence(sequence: Sequence): Void {\n    // TODO(tjp, regex): Foreach loop/function would be nice.\n    for (var i = 0; i < sequence.items.length; i += 1) {\n      pushRegex(sequence.items[i]);\n    }\n  }\n\n  // Put this here instead of the data model for now because I'm not sure this\n  // makes sense to be part of the public api right now.\n  public maxCode(codePart: CodePart): Int | Null {\n    match (codePart) {\n      is CodePoints -> do {\n        // Iterating code points is the hardest of the current cases.\n        let value = codePart.value;\n        if (value.isEmpty) {\n          null\n        } else {\n          // My kingdom for a fold, or even just a max, in builtins.\n          var max = 0;\n          for (\n            var slice = value.codePoints;\n            !slice.isEmpty;\n            slice = slice.advance(1)\n          ) {\n            let next = slice.read();\n            if (next > max) {\n              max = next;\n            }\n          }\n          max\n        }\n      }\n      // Others below are easy for now.\n      is CodeRange -> codePart.max;\n      Digit -> \"9\".codePoints.read();\n      Space -> \" \".codePoints.read();\n      Word -> \"z\".codePoints.read();\n      // Actually unexpected, ever, but eh.\n      else -> null;\n    }\n  }\n}\n\n// // TODO(tjp, regex): Delete all the below (comment included) if unused.\n// // TODO(tjp, regex): Replace all this with a compile-time regex once we can.\n// let escapeCodeList = [\n//   \"\\\\\".codePoints.read(),\n//   \"^\".codePoints.read(),\n//   \"$\".codePoints.read(),\n//   \"{\".codePoints.read(),\n//   \"[\".codePoints.read(),\n//   \"(\".codePoints.read(),\n//   \"}\".codePoints.read(),\n//   \"]\".codePoints.read(),\n//   \")\".codePoints.read(),\n//   \"|\".codePoints.read(),\n//   \"+\".codePoints.read(),\n//   \"?\".codePoints.read(),\n//   \"/\".codePoints.read(),\n//   \"*\".codePoints.read(),\n// ];\n// let escapeCodes = new DenseBitVector(128);\n// // This `for` loop has to be after type definitions for now because\n// // https://github.com/temper-lang/temper/issues/817\n// for (var i = 0; i < escapeCodeList.length; i += 1) {\n//   escapeCodes[i] = true;\n// }\n```\n\n</details>\n"
+        "# Regex Data Model and Functionality\n\nThe structural data model for regex patterns enables direct construction, and\nthe Temper regex dialect compiles static regex text patterns to these objects.\n\nA focus here is on providing tools people can actually reach for when they need\nto do text processing. The execution should be faster on backends like Python\nthan writing raw code, and the implementation in backends like C should\napproximate what you'd like to have written manually.\n\nDue to inadequate and distinct Unicode handling in backend regex engines, the\ninitial feature set avoids character classes and properties but is still aware\nof code points. Parsing focused on limited sets of delimiters works best for\nnow.\n\nThe core feature set here focuses on both the data model and utility functions,\nsuch as matching regexes against strings.\n\n## Regex Data Model\n\nAll regexes are composed hierarchically of `Regex` nodes. Regexes are a\nsequence of component parts. For example, `/hi./` is a sequence of\n[CodePoint](#codepoint) `/h/` and `/i/` and dot `/./`.\n\nAnd perhaps the most fundamental `Regex` is the [Sequence](#sequence),\nbecause it enables multiple regex components to be strung together.\n\n```\nexport /*sealed*/ interface Regex {\n```\n\nBefore a regex is used, it must be compiled. Some helper functions compile on\nthe fly, although it is faster to reuse a pre-compiled regex.\n\n```\n  // TODO(tjp, regex): Make this into a macro behind the scenes.\n  // TODO(tjp, regex): `compiled<T>(): CompiledRegex<T>`\n  public compiled(): CompiledRegex { new CompiledRegex(this) }\n```\n\nThe simplest use of a regular expression is if it is found in a string.\nRepeatedly calling these methods on a single `Regex` instance is inefficient.\nBetter for reuse is to compile in advance.\n\n```\n  public found(text: String): Boolean { compiled().found(text) }\n```\n\nYou can also return match details or perform text replacement. The returned\ngroups map contains an entry for each key in the order defined in the regex\npattern. If no \"full\" group is defined, one is added automatically to capture\nthe full matched text.\n\nIn the future, we intend to support customized match types with fields to match\ncapture groups, statically checked where possible.\n\n```\n  // TODO(tjp, regex): Also macro because reification.\n  // TODO(tjp, regex): `find<T = Map<String, Group>>(): T | NoResult`\n  public find(text: String): Map<String, Group> | NoResult {\n    compiled().find(text)\n  }\n\n  public replace(\n    text: String, format: fn (Map<String, Group>): String\n  ): String {\n    compiled().replace(text, format)\n  }\n```\n\nThat's it for what you can do with regex patterns in Temper today, but there's\nmuch more to say on what kinds of regexes can be built.\n\n```\n}\n```\n\n## Regex Item Types\n\nA `Regex` is composed of a potential variety of subtypes.\n\n### Groups\n\nMultiple types of groups exist:\n\n- [Capture](#capture) `/(?<name>...)/` to remember match groups for later use.\n- Non-capturing group syntax `/(?:...)/`, which is simply a [Regex](#regex)\n  instance in the data model.\n\n### Capture\n\nTODO(tjp, regex): Change to named captures only!\n\n`Capture` is a [group](#groups) that remembers the matched text for later\naccess. Temper supports only named matches, with current intended syntax\n`/(?name = ...)/`.\n\n```\nexport class Capture extends Regex {\n  public name: String;\n  public /*early*/ item: Regex;\n}\n```\n\n### CodePart\n\nA component of a [CodeSet][#codeset], aka character class, which applies to a\nsubset of regex data types.\n\nHere, \"code\" is short for \"code point\" although \"char\" might work better,\ndepending on expectations.\n\n```\nexport /*sealed*/ interface CodePart extends Regex {}\n```\n\n### CodePoints\n\nOne or more verbatim code points, where the sequence matters if within a\n[Regex](#regex) or not if within a [CodeSet](#codeset). Some escapes in\ntextual regex source, such as `/\\t/`, can be stored as raw code points.\n\nThe `String` here can enable more efficient storage than individual code\npoints, although the source text may require non-capture grouping. For example,\n`/(?:abc)?/` optionally matches the string `\"abc\"`, whereas `/abc?/` matches\n`\"ab\"` with an optional `\"c\"`.\n\n```\nexport class CodePoints extends CodePart {\n  public value: String;\n}\n```\n\n### Specials\n\nA number of special match forms exist. In the data model, these are empty\nclasses.\n\n- `.` - `Dot` In default mode, matches any Unicode code point except newline.\n- `^` - `Begin` in default mode matches zero-length at the beginning of a\n  string.\n- `$` - `End` in default mode matches zero-length at the end of a string.\n- `\\b` - `WordBoundary` matches zero-length at the boundary between word and\n  non-word code points. More sophisticated Unicode compliance is TBD.\n- `\\s` (negated as `\\S`) - `Space` matches any horizontal space code point.\n  Details are TBD.\n- `\\w` (negated as `\\W`) - `Word` matches any word code point. Details are TBD.\n  This is currently defined in terms of old ASCII definitions because those are\n  clear. Perhaps this will stay that way, and Unicode properties like `\\p{L}`\n  will be used for human language needs.\n- `\\X` - `GraphemeCluster` might not be supported, but [here is some discussion\n  of how to implement it](\n  https://github.com/rust-lang/regex/issues/54#issuecomment-661905060).\n\n<details>\n\n```\nexport /*sealed*/ interface Special extends Regex {}\nexport let Begin = do { class Begin extends Special {}; new Begin() };\nexport let Dot = do { class Dot extends Special {}; new Dot() };\nexport let End = do { class End extends Special {}; new End() };\n// TODO(tjp, regex): We can't easily support this at present across backends.\n// export let GraphemeCluster = do {\n//   class GraphemeCluster extends Special {}; new GraphemeCluster()\n// };\nexport let WordBoundary = do {\n  class WordBoundary extends Special {}; new WordBoundary()\n};\n\nexport /*sealed*/ interface SpecialSet extends CodePart & Special {}\nexport let Digit = do { class Digit extends SpecialSet {}; new Digit() };\nexport let Space = do { class Space extends SpecialSet {}; new Space() };\nexport let Word = do { class Word extends SpecialSet {}; new Word() };\n```\n\n</details>\n\n### CodeRange\n\nA code point range matches any code point in its inclusive bounds, such as\n`/[a-c]/`. In source, `-` is included in a code set either by escaping or by\nincluding it as the first or last character. A `CodeRange` is usually contained\ninside a [CodeSet](#codeset), and syntactically always is.\n\n```\nexport class CodeRange extends CodePart {\n  public min: Int;\n  public max: Int;\n}\n```\n\n### CodeSet\n\nA set of code points, any of which can match, such as `/[abc]/` matching any of\n`\"a\"`, `\"b\"`, or `\"c\"`. Alternatively, a negated set is the inverse of the code\npoints given, such as `/[^abc]/`, matching any code point that's not any of\nthese. This is also often called a character class.\n\nFurther, a subset of [specials](#specials) can also be used in code sets. A\nnegated code set of just a special set often has custom syntax. For example,\nnon-space can be said as either `/[^\\s]/` or `/\\S/`.\n\n```\nexport class CodeSet extends Regex {\n  public items: List<CodePart>;\n  public negated: Boolean = false;\n}\n```\n\n### Or\n\n`Or` matches any one of multiple options, such as `/ab|cd|e*/`.\n\n```\nexport class Or extends Regex {\n  public /*early*/ items: List<Regex>;\n}\n```\n\n### Repeat\n\n`Repeat` matches from an minimum to a maximum number of repeats of a\nsubregex. This can be represented in regex source in a number of ways:\n\n- `?` matches 0 or 1.\n- `*` matches 0 or more.\n- `+` matches 1 or more.\n- `{m}` matches exactly `m` repetitions.\n- `{m,n}` matches between `m` and `n`. Missing `n` is a max of infinity. For\n  example, `{0,1}` is equivalent to `?`, and `{1,}` is equivalent to `+`.\n\nBy default, repetitions are greedy, matching as many repetitions as possible.\nIn regex source, any of the above can have `?` appended to indicated reluctant\n(aka non-greedy), matching as few repetitions as possible.\n\n```\nexport class Repeat extends Regex {\n  public /*early*/ item: Regex;\n  public min: Int;\n  public max: Int | Null; // where null means infinite\n  public reluctant: Boolean = false;\n}\n```\n\nWe also have convenience builders.\n\n```\nexport let entire(item: Regex): Regex {\n  new Sequence([Begin, item, End])\n}\n\nexport let oneOrMore(item: Regex, reluctant: Boolean = false): Repeat {\n  { item, min: 1, max: null, reluctant }\n}\n\nexport let optional(item: Regex, reluctant: Boolean = false): Repeat {\n  { item, min: 0, max: 1, reluctant }\n}\n```\n\n### Sequence\n\n`Sequence` strings along multiple other regexes in order.\n\n```\nexport class Sequence extends Regex {\n  public /*early*/ items: List<Regex>;\n}\n```\n\n## Match Objects\n\nFor detailed match results, call `find` on a regex to get a `Map` object from\n`String` keys to `Group` values.\n\n```\n// TODO Go back to a `Match` object with `groups` as a member so we can also\n// TODO easily return metadata alongside groups? Or is simpler better?\n// export class Match { // interface ... <T = Map<String, Group>> {\n//   public let groups: Map<String, Group>;\n// }\n\nexport class Group {\n  public let name: String;\n  public let value: String;\n  public let codePointsBegin: Int;\n}\n```\n\n## Compiled Regex Objects\n\nThe compiled form of a regex is mostly opaque, but it can be cached for more\nefficient reuse than working from a source [Regex](#regex-data-model).\n\n<details>\n\n```\n// Provides a workaround for access to std/regex from extension methods.\nclass RegexRefs {\n  public let codePoints: CodePoints = new CodePoints(\"\");\n  public let group: Group = { name: \"\", value: \"\", codePointsBegin: 0 }\n  public let orObject: Or = new Or([]);\n}\n\nlet regexRefs = new RegexRefs();\n```\n\n</details>\n\n```\n// TODO(tjp, regex): Generate subtypes of this interface later.\nexport class CompiledRegex { // interface ... <T> {\n```\n\nThe source `Regex` data is still available on compiled objects in case it's\nneeded for composition or other purposes.\n\n```\n  public let data: Regex;\n\n  public constructor(data: Regex) {\n    this.data = data;\n    compiled = compileFormatted(format());\n  }\n```\n\nA compiled regex exposes many of the same capabilities as `Regex`, but they are\nmore efficient to use repeatedly.\n\n```\n  public found(text: String): Boolean { compiledFound(compiled, text) }\n\n  public find(text: String): Map<String, Group> | NoResult {\n    compiledFind(compiled, text, regexRefs)\n  }\n\n  public replace(\n    text: String, format: fn (Map<String, Group>): String\n  ): String {\n    compiledReplace(compiled, text, format, regexRefs)\n  }\n```\n\nTODO(tjp, regex): Public method for replace with named references.\nTODO(tjp, regex): Any static checking?\n\n<details>\n\n```\n  let compiled: AnyValue;\n\n  // Extension functions on some backends need the private `compiled` value\n  // passed in directly.\n  @connected(\"CompiledRegex::compiledFound\")\n  compiledFound(compiled: AnyValue, text: String): Boolean;\n\n  @connected(\"CompiledRegex::compiledFind\")\n  compiledFind(\n    compiled: AnyValue, text: String, regexRefs: RegexRefs\n  ): Map<String, Group> | NoResult;\n\n  @connected(\"CompiledRegex::compileFormatted\")\n  compileFormatted(formatted: String): AnyValue;\n\n  @connected(\"CompiledRegex::compiledReplace\")\n  compiledReplace(\n    compiled: AnyValue,\n    text: String,\n    format: fn (Map<String, Group>): String,\n    regexRefs: RegexRefs,\n  ): String;\n\n  @connected(\"CompiledRegex::format\")\n  format(): String { new RegexFormatter().format(data) }\n```\n\n</details>\n\n```\n}\n```\n\n## Private implementation matters\n\nSome regex logic can be shared across backends. These features aren't directly\nexported to the user, however.\n\nThe intent is that these support features only get included in compiled Temper\ncode if usage depends on dynamically constructed regexes. If all regex building\nis done as stable values, we hope to generated backend compiled regexes purely\nat Temper compile time.\n\n### RegexFormatter\n\n<details>\n\n```\nclass RegexFormatter {\n  let out: ListBuilder<String> = new ListBuilder<String>();\n\n  public format(regex: Regex): String {\n    pushRegex(regex)\n    out.join(\"\") { (x);; x }\n  }\n\n  pushRegex(regex: Regex): Void {\n    match (regex) {\n      // Aggregate types.\n      is Capture -> pushCapture(regex);\n      is CodePoints -> pushCodePoints(regex, false);\n      is CodeRange -> pushCodeRange(regex);\n      is CodeSet -> pushCodeSet(regex);\n      is Or -> pushOr(regex);\n      is Repeat -> pushRepeat(regex);\n      is Sequence -> pushSequence(regex);\n      // Specials.\n      // Some of these will need to be customized on future backends.\n      Begin -> out.add(\"^\");\n      Dot -> out.add(\".\");\n      End -> out.add(\"$\");\n      WordBoundary -> out.add(\"\\\\b\");\n      // Special sets.\n      Digit -> out.add(\"\\\\d\");\n      Space -> out.add(\"\\\\s\");\n      Word -> out.add(\"\\\\w\");\n      // ...\n    }\n  }\n\n  pushCapture(capture: Capture): Void {\n    out.add(\"(\");\n    // TODO(tjp, regex): Consistent name validation rules for all backends???\n    // TODO(tjp, regex): Validate here or in `Capture` constructor???\n    // TODO(tjp, regex): Validate here or where against reused names???\n    pushCaptureName(out, capture.name);\n    pushRegex(capture.item);\n    out.add(\")\");\n  }\n\n  @connected(\"RegexFormatter::pushCaptureName\")\n  pushCaptureName(out: ListBuilder<String>, name: String): Void {\n    // All so far except Python use this form.\n    out.add(\"?<${name}>\");\n  }\n\n  pushCode(code: Int, insideCodeSet: Boolean): Void {\n    // Expose private property to extension.\n    pushCodeTo(out, code, insideCodeSet);\n    // TODO(tjp, regex): Implement more in Temper once we can.\n    // if (escapeCodes[code] && false) {\n    //   out.add(\"\\\\\");\n    //   // TODO(tjp, regex): How to convert back to strings?\n    // }\n  }\n\n  @connected(\"RegexFormatter::pushCodeTo\")\n  pushCodeTo(out: ListBuilder<String>, code: Int, insideCodeSet: Boolean): Void;\n\n  pushCodePoints(codePoints: CodePoints, insideCodeSet: Boolean): Void {\n    for (\n      var slice = codePoints.value.codePoints;\n      !slice.isEmpty;\n      slice = slice.advance(1)\n    ) {\n      pushCode(slice.read(), insideCodeSet);\n    }\n  }\n\n  pushCodeRange(codeRange: CodeRange): Void {\n    out.add(\"[\");\n    pushCodeRangeUnwrapped(codeRange);\n    out.add(\"]\");\n  }\n\n  pushCodeRangeUnwrapped(codeRange: CodeRange): Void {\n    pushCode(codeRange.min, true);\n    out.add(\"-\");\n    pushCode(codeRange.max, true);\n  }\n\n  pushCodeSet(codeSet: CodeSet): Void {\n    let adjusted = adjustCodeSet(codeSet, regexRefs);\n    match (adjusted) {\n      is CodeSet -> do {\n        out.add(\"[\");\n        if (adjusted.negated) {\n          out.add(\"^\");\n        }\n        for (var i = 0; i < adjusted.items.length; i += 1) {\n          pushCodeSetItem(adjusted.items[i]);\n        }\n        out.add(\"]\");\n      }\n      else -> pushRegex(adjusted);\n    }\n  }\n\n  @connected(\"RegexFormatter::adjustCodeSet\")\n  adjustCodeSet(codeSet: CodeSet, regexRefs: RegexRefs): Regex { codeSet }\n\n  pushCodeSetItem(codePart: CodePart): Void {\n    match (codePart) {\n      is CodePoints -> pushCodePoints(codePart, true);\n      is CodeRange -> pushCodeRangeUnwrapped(codePart);\n      is SpecialSet -> pushRegex(codePart);\n    }\n  }\n\n  pushOr(or: Or): Void {\n    if (!or.items.isEmpty) {\n      out.add(\"(?:\");\n      // TODO(tjp, regex): See #822. Until `this` works better, no this in funs.\n      // TODO(tjp, regex): So just manually loop here. Sometimes faster, anyway?\n      pushRegex(or.items[0]);\n      for (var i = 1; i < or.items.length; i += 1) {\n        out.add(\"|\");\n        pushRegex(or.items[i]);\n      }\n      out.add(\")\");\n    }\n  }\n\n  pushRepeat(repeat: Repeat): Void {\n    // Always wrap the main sub-pattern here to make life easy\n    out.add(\"(?:\");\n    pushRegex(repeat.item);\n    out.add(\")\");\n    // Then add the repetition part.\n    let min = repeat.min;\n    let max = repeat.max;\n    if (false) {\n    } else if (min == 0 && max == 1) {\n      out.add(\"?\");\n    } else if (min == 0 && max == null) {\n      out.add(\"*\");\n    } else if (min == 1 && max == null) {\n      out.add(\"+\");\n    } else {\n      out.add(\"{${min.toString()}\");\n      if (min != max) {\n        out.add(\",\");\n        if (max != null) {\n          out.add(max.as<Int>().toString());\n        }\n      }\n      out.add(\"}\");\n    }\n    if (repeat.reluctant) {\n      out.add(\"?\");\n    }\n  }\n\n  pushSequence(sequence: Sequence): Void {\n    // TODO(tjp, regex): Foreach loop/function would be nice.\n    for (var i = 0; i < sequence.items.length; i += 1) {\n      pushRegex(sequence.items[i]);\n    }\n  }\n\n  // Put this here instead of the data model for now because I'm not sure this\n  // makes sense to be part of the public api right now.\n  public maxCode(codePart: CodePart): Int | Null {\n    match (codePart) {\n      is CodePoints -> do {\n        // Iterating code points is the hardest of the current cases.\n        let value = codePart.value;\n        if (value.isEmpty) {\n          null\n        } else {\n          // My kingdom for a fold, or even just a max, in builtins.\n          var max = 0;\n          for (\n            var slice = value.codePoints;\n            !slice.isEmpty;\n            slice = slice.advance(1)\n          ) {\n            let next = slice.read();\n            if (next > max) {\n              max = next;\n            }\n          }\n          max\n        }\n      }\n      // Others below are easy for now.\n      is CodeRange -> codePart.max;\n      Digit -> \"9\".codePoints.read();\n      Space -> \" \".codePoints.read();\n      Word -> \"z\".codePoints.read();\n      // Actually unexpected, ever, but eh.\n      else -> null;\n    }\n  }\n}\n\n// // TODO(tjp, regex): Delete all the below (comment included) if unused.\n// // TODO(tjp, regex): Replace all this with a compile-time regex once we can.\n// let escapeCodeList = [\n//   \"\\\\\".codePoints.read(),\n//   \"^\".codePoints.read(),\n//   \"$\".codePoints.read(),\n//   \"{\".codePoints.read(),\n//   \"[\".codePoints.read(),\n//   \"(\".codePoints.read(),\n//   \"}\".codePoints.read(),\n//   \"]\".codePoints.read(),\n//   \")\".codePoints.read(),\n//   \"|\".codePoints.read(),\n//   \"+\".codePoints.read(),\n//   \"?\".codePoints.read(),\n//   \"/\".codePoints.read(),\n//   \"*\".codePoints.read(),\n// ];\n// let escapeCodes = new DenseBitVector(128);\n// // This `for` loop has to be after type definitions for now because\n// // https://github.com/temper-lang/temper/issues/817\n// for (var i = 0; i < escapeCodeList.length; i += 1) {\n//   escapeCodes[i] = true;\n// }\n```\n\n</details>\n"
     ],
     "version": 3
 }
```

### Comparing `temper_std-0.0.3/temper_std/regex__preface.py.map` & `temper_std-0.0.4/temper_std/regex__preface.py.map`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'sourcesContent'": "['# Regex Data Model and Functionality\\n\\nThe structural data model for "*

 * *                     'regex patterns enables direct construction, and\\nthe Temper regex dialect '*

 * *                     'compiles static regex text patterns to these objects.\\n\\nA focus here is '*

 * *                     'on providing tools people can actually reach for when they need\\nto do text '*

 * *                     'processing. The execution should be faster on backends like Python\\nthan '*

 * *                  […]*

```diff
@@ -4,11 +4,11 @@
     "names": [
         "return"
     ],
     "sources": [
         "std/regex.temper.md"
     ],
     "sourcesContent": [
-        "# Regex Data Model and Functionality\n\nThe structural data model for regex patterns enables direct construction, and\nthe Temper regex dialect compiles static regex text patterns to these objects.\n\nA focus here is on providing tools people can actually reach for when they need\nto do text processing. The execution should be faster on backends like Python\nthan writing raw code, and the implementation in backends like C should\napproximate what you'd like to have written manually.\n\nDue to inadequate and distinct Unicode handling in backend regex engines, the\ninitial feature set avoids character classes and properties but is still aware\nof code points. Parsing focused on limited sets of delimiters works best for\nnow.\n\nThe core feature set here focuses on both the data model and utility functions,\nsuch as matching regexes against strings.\n\n## Regex Data Model\n\nAll regexes are composed hierarchically of `Regex` nodes. Regexes are a\nsequence of component parts. For example, `/hi./` is a sequence of\n[CodePoint](#codepoint) `/h/` and `/i/` and dot `/./`.\n\nAnd perhaps the most fundamental `Regex` is the [Sequence](#sequence),\nbecause it enables multiple regex components to be strung together.\n\n```temper ;lit\nexport /*sealed*/ interface Regex {\n```\n\nBefore a regex is used, it must be compiled. Some helper functions compile on\nthe fly, although it is faster to reuse a pre-compiled regex.\n\n```temper ;lit\n  // TODO(tjp, regex): Make this into a macro behind the scenes.\n  // TODO(tjp, regex): `compiled<T>(): CompiledRegex<T>`\n  public compiled(): CompiledRegex { new CompiledRegex(this) }\n```\n\nThe simplest use of a regular expression is if it is found in a string.\nRepeatedly calling these methods on a single `Regex` instance is inefficient.\nBetter for reuse is to compile in advance.\n\n```temper ;lit\n  public foundIn(text: String): Boolean { compiled().foundIn(text) }\n```\n\n```temper ;lit\n  // TODO(tjp, regex): Also macro because reification.\n  // TODO(tjp, regex): `find<T>(): Match<T> | NoResult`\n  public find(text: String): Match | NoResult { compiled().find(text) }\n```\n\nThat's it for what you can do with regex patterns in Temper today, but there's\nmuch more to say on what kinds of regexes can be built.\n\n```temper ;lit\n}\n```\n\n## Regex Item Types\n\nA `Regex` is composed of a potential variety of subtypes.\n\n### Groups\n\nMultiple types of groups exist:\n\n- [Capture](#capture) `/(?<name>...)/` to remember match groups for later use.\n- Non-capturing group syntax `/(?:...)/`, which is simply a [Regex](#regex)\n  instance in the data model.\n\n### Capture\n\nTODO(tjp, regex): Change to named captures only!\n\n`Capture` is a [group](#groups) that remembers the matched text for later\naccess. Temper supports only named matches, with current intended syntax\n`/(?name = ...)/`.\n\n```temper ;lit\nexport class Capture extends Regex {\n  public name: String;\n  public /*early*/ item: Regex;\n}\n```\n\n### CodePart\n\nA component of a [CodeSet][#codeset], aka character class, which applies to a\nsubset of regex data types.\n\nHere, \"code\" is short for \"code point\" although \"char\" might work better,\ndepending on expectations.\n\n```temper ;lit\nexport /*sealed*/ interface CodePart extends Regex {}\n```\n\n### CodePoints\n\nOne or more verbatim code points, where the sequence matters if within a\n[Regex](#regex) or not if within a [CodeSet](#codeset). Some escapes in\ntextual regex source, such as `/\\t/`, can be stored as raw code points.\n\nThe `String` here can enable more efficient storage than individual code\npoints, although the source text may require non-capture grouping. For example,\n`/(?:abc)?/` optionally matches the string `\"abc\"`, whereas `/abc?/` matches\n`\"ab\"` with an optional `\"c\"`.\n\n```temper ;lit\nexport class CodePoints extends CodePart {\n  public value: String;\n}\n```\n\n### Specials\n\nA number of special match forms exist. In the data model, these are empty\nclasses.\n\n- `.` - `Dot` In default mode, matches any Unicode code point except newline.\n- `^` - `Begin` in default mode matches zero-length at the beginning of a\n  string.\n- `$` - `End` in default mode matches zero-length at the end of a string.\n- `\\b` - `WordBoundary` matches zero-length at the boundary between word and\n  non-word code points. More sophisticated Unicode compliance is TBD.\n- `\\s` (negated as `\\S`) - `Space` matches any horizontal space code point.\n  Details are TBD.\n- `\\w` (negated as `\\W`) - `Word` matches any word code point. Details are TBD.\n  This is currently defined in terms of old ASCII definitions because those are\n  clear. Perhaps this will stay that way, and Unicode properties like `\\p{L}`\n  will be used for human language needs.\n- `\\X` - `GraphemeCluster` might not be supported, but [here is some discussion\n  of how to implement it](\n  https://github.com/rust-lang/regex/issues/54#issuecomment-661905060).\n\n<details>\n\n```temper ;lit\nexport /*sealed*/ interface Special extends Regex {}\nexport let Begin = do { class Begin extends Special {}; new Begin() };\nexport let Dot = do { class Dot extends Special {}; new Dot() };\nexport let End = do { class End extends Special {}; new End() };\n// TODO(tjp, regex): We can't easily support this at present across backends.\n// export let GraphemeCluster = do {\n//   class GraphemeCluster extends Special {}; new GraphemeCluster()\n// };\nexport let WordBoundary = do {\n  class WordBoundary extends Special {}; new WordBoundary()\n};\n\nexport /*sealed*/ interface SpecialSet extends CodePart & Special {}\nexport let Digit = do { class Digit extends SpecialSet {}; new Digit() };\nexport let Space = do { class Space extends SpecialSet {}; new Space() };\nexport let Word = do { class Word extends SpecialSet {}; new Word() };\n```\n\n</details>\n\n### CodeRange\n\nA code point range matches any code point in its inclusive bounds, such as\n`/[a-c]/`. In source, `-` is included in a code set either by escaping or by\nincluding it as the first or last character. A `CodeRange` is usually contained\ninside a [CodeSet](#codeset), and syntactically always is.\n\n```temper ;lit\nexport class CodeRange extends CodePart {\n  public min: Int;\n  public max: Int;\n}\n```\n\n### CodeSet\n\nA set of code points, any of which can match, such as `/[abc]/` matching any of\n`\"a\"`, `\"b\"`, or `\"c\"`. Alternatively, a negated set is the inverse of the code\npoints given, such as `/[^abc]/`, matching any code point that's not any of\nthese. This is also often called a character class.\n\nFurther, a subset of [specials](#specials) can also be used in code sets. A\nnegated code set of just a special set often has custom syntax. For example,\nnon-space can be said as either `/[^\\s]/` or `/\\S/`.\n\n```temper ;lit\nexport class CodeSet extends Regex {\n  public items: List<CodePart>;\n  public negated: Boolean = false;\n}\n```\n\n### Or\n\n`Or` matches any one of multiple options, such as `/ab|cd|e*/`.\n\n```temper ;lit\nexport class Or extends Regex {\n  public /*early*/ items: List<Regex>;\n}\n```\n\n### Repeat\n\n`Repeat` matches from an minimum to a maximum number of repeats of a\nsubregex. This can be represented in regex source in a number of ways:\n\n- `?` matches 0 or 1.\n- `*` matches 0 or more.\n- `+` matches 1 or more.\n- `{m}` matches exactly `m` repetitions.\n- `{m,n}` matches between `m` and `n`. Missing `n` is a max of infinity. For\n  example, `{0,1}` is equivalent to `?`, and `{1,}` is equivalent to `+`.\n\nBy default, repetitions are greedy, matching as many repetitions as possible.\nIn regex source, any of the above can have `?` appended to indicated reluctant\n(aka non-greedy), matching as few repetitions as possible.\n\n```temper ;lit\nexport class Repeat extends Regex {\n  public /*early*/ item: Regex;\n  public min: Int;\n  public max: Int | Null; // where null means infinite\n  public reluctant: Boolean = false;\n}\n```\n\nWe also have convenience builders.\n\n```temper ;lit\nexport let entire(item: Regex): Regex {\n  new Sequence([Begin, item, End])\n}\n\nexport let oneOrMore(item: Regex, reluctant: Boolean = false): Repeat {\n  { item, min: 1, max: null, reluctant }\n}\n\nexport let optional(item: Regex, reluctant: Boolean = false): Repeat {\n  { item, min: 0, max: 1, reluctant }\n}\n```\n\n### Sequence\n\n`Sequence` strings along multiple other regexes in order.\n\n```temper ;lit\nexport class Sequence extends Regex {\n  public /*early*/ items: List<Regex>;\n}\n```\n\n## Match Objects\n\nFor detailed match results, call `find` on a regex to get a `Match` object.\n\n```temper ;lit\n// TODO(tjp, regex): Generate subtypes of this interface later.\n// TODO(tjp, regex): If we can keep this to `groups` only, can we make the\n// TODO(tjp, regex): groups list or object the whole match value?\nexport class Match { // interface ... <T> {\n  // TODO(tjp, regex): After custom, do we still also want a generic group list?\n  /**\n   * By default, includes a \"full\" group at index 0 for the full match. If\n   * another \"full\" capture is defined, the default is excluded. Keeping the\n   * full match uniform with other named groups enables unification, including\n   * with custom match types.\n   */\n  public let groups: List<Group>;\n  // TODO(tjp, regex): Custom capture storage goes here once we're ready.\n  // public let storage: T;\n}\n\nexport class Group {\n  public let name: String;\n  public let value: String;\n  public let codePointsBegin: Int;\n}\n```\n\n## Compiled Regex Objects\n\nThe compiled form of a regex is mostly opaque, but it can be cached for more\nefficient reuse than working from a source [Regex](#regex-data-model).\n\n<details>\n\n```temper ;lit\n// Provides a workaround for access to std/regex from extension methods.\nclass RegexRefs {\n  public let codePoints: CodePoints = new CodePoints(\"\");\n  public let match: Match = {\n    groups: [{ name: \"\", value: \"\", codePointsBegin: 0 }],\n  };\n  public let orObject: Or = new Or([]);\n}\n\nlet regexRefs = new RegexRefs();\n```\n\n</details>\n\n```temper ;lit\n// TODO(tjp, regex): Generate subtypes of this interface later.\nexport class CompiledRegex { // interface ... <T> {\n```\n\nThe source `Regex` data is still available on compiled objects in case it's\nneeded for composition or other purposes.\n\n```temper ;lit\n  public let data: Regex;\n\n  public constructor(data: Regex): Void {\n    this.data = data;\n    compiled = compileFormatted(format());\n  }\n```\n\nA compiled regex exposes many of the same capabilities as `Regex`, but they are\nmore efficient to use repeatedly.\n\n```temper ;lit\n  public foundIn(text: String): Boolean { compiledFoundIn(compiled, text) }\n```\n\n```temper ;lit\n  public let find(text: String): Match | NoResult {\n    compiledFind(compiled, text, regexRefs)\n  }\n```\n\nTODO(tjp, regex): Public method for replace with named references.\nTODO(tjp, regex): Any static checking?\n\n<details>\n\n```temper ;lit\n  let compiled: AnyValue;\n\n  // Extension functions on some backends need the private `compiled` value\n  // passed in directly.\n  @extension(\"CompiledRegex::compiledFoundIn\")\n  compiledFoundIn(compiled: AnyValue, text: String): Boolean;\n\n  @extension(\"CompiledRegex::compiledFind\")\n  compiledFind(\n    compiled: AnyValue, text: String, regexRefs: RegexRefs\n  ): Match | NoResult;\n\n  @extension(\"CompiledRegex::compileFormatted\")\n  compileFormatted(formatted: String): AnyValue;\n\n  @extension(\"CompiledRegex::format\")\n  format(): String { new RegexFormatter().format(data) }\n```\n\n</details>\n\n```temper ;lit\n}\n```\n\n## Private implementation matters\n\nSome regex logic can be shared across backends. These features aren't directly\nexported to the user, however.\n\nThe intent is that these support features only get included in compiled Temper\ncode if usage depends on dynamically constructed regexes. If all regex building\nis done as stable values, we hope to generated backend compiled regexes purely\nat Temper compile time.\n\n### RegexFormatter\n\n<details>\n\n```temper ;lit\nclass RegexFormatter {\n  let out: ListBuilder<String> = new ListBuilder<String>();\n\n  public format(regex: Regex): String {\n    pushRegex(regex)\n    out.join(\"\") { (x);; x }\n  }\n\n  pushRegex(regex: Regex): Void {\n    match (regex) {\n      // Aggregate types.\n      is Capture -> pushCapture(regex);\n      is CodePoints -> pushCodePoints(regex, false);\n      is CodeRange -> pushCodeRange(regex);\n      is CodeSet -> pushCodeSet(regex);\n      is Or -> pushOr(regex);\n      is Repeat -> pushRepeat(regex);\n      is Sequence -> pushSequence(regex);\n      // Specials.\n      // Some of these will need customized on future backends.\n      Begin -> out.add(\"^\");\n      Dot -> out.add(\".\");\n      End -> out.add(\"$\");\n      WordBoundary -> out.add(\"\\\\b\");\n      // Special sets.\n      Digit -> out.add(\"\\\\d\");\n      Space -> out.add(\"\\\\s\");\n      Word -> out.add(\"\\\\w\");\n      // ...\n    }\n  }\n\n  pushCapture(capture: Capture): Void {\n    out.add(\"(\");\n    // TODO(tjp, regex): Consistent name validation rules for all backends???\n    // TODO(tjp, regex): Validate here or in `Capture` constructor???\n    // TODO(tjp, regex): Validate here or where against reused names???\n    pushCaptureName(out, capture.name);\n    pushRegex(capture.item);\n    out.add(\")\");\n  }\n\n  @extension(\"RegexFormatter::pushCaptureName\")\n  pushCaptureName(out: ListBuilder<String>, name: String): Void {\n    // All so far except Python use this form.\n    out.add(\"?<${name}>\");\n  }\n\n  pushCode(code: Int, insideCodeSet: Boolean): Void {\n    // Expose private property to extension.\n    pushCodeTo(out, code, insideCodeSet);\n    // TODO(tjp, regex): Implement more in Temper once we can.\n    // if (escapeCodes[code] && false) {\n    //   out.add(\"\\\\\");\n    //   // TODO(tjp, regex): How to convert back to strings?\n    // }\n  }\n\n  @extension(\"RegexFormatter::pushCodeTo\")\n  pushCodeTo(out: ListBuilder<String>, code: Int, insideCodeSet: Boolean): Void;\n\n  pushCodePoints(codePoints: CodePoints, insideCodeSet: Boolean): Void {\n    for (\n      var slice = codePoints.value.codePoints;\n      !slice.isEmpty;\n      slice = slice.advance(1)\n    ) {\n      pushCode(slice.read(), insideCodeSet);\n    }\n  }\n\n  pushCodeRange(codeRange: CodeRange): Void {\n    out.add(\"[\");\n    pushCodeRangeUnwrapped(codeRange);\n    out.add(\"]\");\n  }\n\n  pushCodeRangeUnwrapped(codeRange: CodeRange): Void {\n    pushCode(codeRange.min, true);\n    out.add(\"-\");\n    pushCode(codeRange.max, true);\n  }\n\n  pushCodeSet(codeSet: CodeSet): Void {\n    let adjusted = adjustCodeSet(codeSet, regexRefs);\n    match (adjusted) {\n      is CodeSet -> do {\n        out.add(\"[\");\n        if (adjusted.negated) {\n          out.add(\"^\");\n        }\n        for (var i = 0; i < adjusted.items.length; i += 1) {\n          pushCodeSetItem(adjusted.items[i]);\n        }\n        out.add(\"]\");\n      }\n      else -> pushRegex(adjusted);\n    }\n  }\n\n  @extension(\"RegexFormatter::adjustCodeSet\")\n  adjustCodeSet(codeSet: CodeSet, regexRefs: RegexRefs): Regex { codeSet }\n\n  pushCodeSetItem(codePart: CodePart): Void {\n    match (codePart) {\n      is CodePoints -> pushCodePoints(codePart, true);\n      is CodeRange -> pushCodeRangeUnwrapped(codePart);\n      is SpecialSet -> pushRegex(codePart);\n    }\n  }\n\n  pushOr(or: Or): Void {\n    if (!or.items.isEmpty) {\n      out.add(\"(?:\");\n      // TODO(tjp, regex): See #822. Until `this` works better, no this in funs.\n      // TODO(tjp, regex): So just manually loop here. Sometimes faster, anyway?\n      pushRegex(or.items[0]);\n      for (var i = 1; i < or.items.length; i += 1) {\n        out.add(\"|\");\n        pushRegex(or.items[i]);\n      }\n      out.add(\")\");\n    }\n  }\n\n  pushRepeat(repeat: Repeat): Void {\n    // Always wrap the main sub-pattern here to make life easy\n    out.add(\"(?:\");\n    pushRegex(repeat.item);\n    out.add(\")\");\n    // Then add the repetition part.\n    let min = repeat.min;\n    let max = repeat.max;\n    if (false) {\n    } else if (min == 0 && max == 1) {\n      out.add(\"?\");\n    } else if (min == 0 && max == null) {\n      out.add(\"*\");\n    } else if (min == 1 && max == null) {\n      out.add(\"+\");\n    } else {\n      out.add(\"{${min.toString()}\");\n      if (min != max) {\n        out.add(\",\");\n        if (max != null) {\n          out.add(max.as<Int>().toString());\n        }\n      }\n      out.add(\"}\");\n    }\n    if (repeat.reluctant) {\n      out.add(\"?\");\n    }\n  }\n\n  pushSequence(sequence: Sequence): Void {\n    // TODO(tjp, regex): Foreach loop/function would be nice.\n    for (var i = 0; i < sequence.items.length; i += 1) {\n      pushRegex(sequence.items[i]);\n    }\n  }\n\n  // Put this here instead of the data model for now because I'm not sure this\n  // makes sense to be part of the public api right now.\n  public maxCode(codePart: CodePart): Int | Null {\n    match (codePart) {\n      is CodePoints -> do {\n        // Iterating code points is the hardest of the current cases.\n        let value = codePart.value;\n        if (value.isEmpty) {\n          null\n        } else {\n          // My kingdom for a fold, or even just a max, in builtins.\n          var max = 0;\n          for (\n            var slice = value.codePoints;\n            !slice.isEmpty;\n            slice = slice.advance(1)\n          ) {\n            let next = slice.read();\n            if (next > max) {\n              max = next;\n            }\n          }\n          max\n        }\n      }\n      // Others below are easy for now.\n      is CodeRange -> codePart.max;\n      Digit -> \"9\".codePoints.read();\n      Space -> \" \".codePoints.read();\n      Word -> \"z\".codePoints.read();\n      // Actually unexpected, ever, but eh.\n      else -> null;\n    }\n  }\n}\n\n// // TODO(tjp, regex): Delete all the below (comment included) if unused.\n// // TODO(tjp, regex): Replace all this with a compile-time regex once we can.\n// let escapeCodeList = [\n//   \"\\\\\".codePoints.read(),\n//   \"^\".codePoints.read(),\n//   \"$\".codePoints.read(),\n//   \"{\".codePoints.read(),\n//   \"[\".codePoints.read(),\n//   \"(\".codePoints.read(),\n//   \"}\".codePoints.read(),\n//   \"]\".codePoints.read(),\n//   \")\".codePoints.read(),\n//   \"|\".codePoints.read(),\n//   \"+\".codePoints.read(),\n//   \"?\".codePoints.read(),\n//   \"/\".codePoints.read(),\n//   \"*\".codePoints.read(),\n// ];\n// let escapeCodes = new DenseBitVector(128);\n// // This `for` loop has to be after type definitions for now because\n// // https://github.com/temper-lang/temper/issues/817\n// for (var i = 0; i < escapeCodeList.length; i += 1) {\n//   escapeCodes[i] = true;\n// }\n```\n\n</details>\n"
+        "# Regex Data Model and Functionality\n\nThe structural data model for regex patterns enables direct construction, and\nthe Temper regex dialect compiles static regex text patterns to these objects.\n\nA focus here is on providing tools people can actually reach for when they need\nto do text processing. The execution should be faster on backends like Python\nthan writing raw code, and the implementation in backends like C should\napproximate what you'd like to have written manually.\n\nDue to inadequate and distinct Unicode handling in backend regex engines, the\ninitial feature set avoids character classes and properties but is still aware\nof code points. Parsing focused on limited sets of delimiters works best for\nnow.\n\nThe core feature set here focuses on both the data model and utility functions,\nsuch as matching regexes against strings.\n\n## Regex Data Model\n\nAll regexes are composed hierarchically of `Regex` nodes. Regexes are a\nsequence of component parts. For example, `/hi./` is a sequence of\n[CodePoint](#codepoint) `/h/` and `/i/` and dot `/./`.\n\nAnd perhaps the most fundamental `Regex` is the [Sequence](#sequence),\nbecause it enables multiple regex components to be strung together.\n\n```\nexport /*sealed*/ interface Regex {\n```\n\nBefore a regex is used, it must be compiled. Some helper functions compile on\nthe fly, although it is faster to reuse a pre-compiled regex.\n\n```\n  // TODO(tjp, regex): Make this into a macro behind the scenes.\n  // TODO(tjp, regex): `compiled<T>(): CompiledRegex<T>`\n  public compiled(): CompiledRegex { new CompiledRegex(this) }\n```\n\nThe simplest use of a regular expression is if it is found in a string.\nRepeatedly calling these methods on a single `Regex` instance is inefficient.\nBetter for reuse is to compile in advance.\n\n```\n  public found(text: String): Boolean { compiled().found(text) }\n```\n\nYou can also return match details or perform text replacement. The returned\ngroups map contains an entry for each key in the order defined in the regex\npattern. If no \"full\" group is defined, one is added automatically to capture\nthe full matched text.\n\nIn the future, we intend to support customized match types with fields to match\ncapture groups, statically checked where possible.\n\n```\n  // TODO(tjp, regex): Also macro because reification.\n  // TODO(tjp, regex): `find<T = Map<String, Group>>(): T | NoResult`\n  public find(text: String): Map<String, Group> | NoResult {\n    compiled().find(text)\n  }\n\n  public replace(\n    text: String, format: fn (Map<String, Group>): String\n  ): String {\n    compiled().replace(text, format)\n  }\n```\n\nThat's it for what you can do with regex patterns in Temper today, but there's\nmuch more to say on what kinds of regexes can be built.\n\n```\n}\n```\n\n## Regex Item Types\n\nA `Regex` is composed of a potential variety of subtypes.\n\n### Groups\n\nMultiple types of groups exist:\n\n- [Capture](#capture) `/(?<name>...)/` to remember match groups for later use.\n- Non-capturing group syntax `/(?:...)/`, which is simply a [Regex](#regex)\n  instance in the data model.\n\n### Capture\n\nTODO(tjp, regex): Change to named captures only!\n\n`Capture` is a [group](#groups) that remembers the matched text for later\naccess. Temper supports only named matches, with current intended syntax\n`/(?name = ...)/`.\n\n```\nexport class Capture extends Regex {\n  public name: String;\n  public /*early*/ item: Regex;\n}\n```\n\n### CodePart\n\nA component of a [CodeSet][#codeset], aka character class, which applies to a\nsubset of regex data types.\n\nHere, \"code\" is short for \"code point\" although \"char\" might work better,\ndepending on expectations.\n\n```\nexport /*sealed*/ interface CodePart extends Regex {}\n```\n\n### CodePoints\n\nOne or more verbatim code points, where the sequence matters if within a\n[Regex](#regex) or not if within a [CodeSet](#codeset). Some escapes in\ntextual regex source, such as `/\\t/`, can be stored as raw code points.\n\nThe `String` here can enable more efficient storage than individual code\npoints, although the source text may require non-capture grouping. For example,\n`/(?:abc)?/` optionally matches the string `\"abc\"`, whereas `/abc?/` matches\n`\"ab\"` with an optional `\"c\"`.\n\n```\nexport class CodePoints extends CodePart {\n  public value: String;\n}\n```\n\n### Specials\n\nA number of special match forms exist. In the data model, these are empty\nclasses.\n\n- `.` - `Dot` In default mode, matches any Unicode code point except newline.\n- `^` - `Begin` in default mode matches zero-length at the beginning of a\n  string.\n- `$` - `End` in default mode matches zero-length at the end of a string.\n- `\\b` - `WordBoundary` matches zero-length at the boundary between word and\n  non-word code points. More sophisticated Unicode compliance is TBD.\n- `\\s` (negated as `\\S`) - `Space` matches any horizontal space code point.\n  Details are TBD.\n- `\\w` (negated as `\\W`) - `Word` matches any word code point. Details are TBD.\n  This is currently defined in terms of old ASCII definitions because those are\n  clear. Perhaps this will stay that way, and Unicode properties like `\\p{L}`\n  will be used for human language needs.\n- `\\X` - `GraphemeCluster` might not be supported, but [here is some discussion\n  of how to implement it](\n  https://github.com/rust-lang/regex/issues/54#issuecomment-661905060).\n\n<details>\n\n```\nexport /*sealed*/ interface Special extends Regex {}\nexport let Begin = do { class Begin extends Special {}; new Begin() };\nexport let Dot = do { class Dot extends Special {}; new Dot() };\nexport let End = do { class End extends Special {}; new End() };\n// TODO(tjp, regex): We can't easily support this at present across backends.\n// export let GraphemeCluster = do {\n//   class GraphemeCluster extends Special {}; new GraphemeCluster()\n// };\nexport let WordBoundary = do {\n  class WordBoundary extends Special {}; new WordBoundary()\n};\n\nexport /*sealed*/ interface SpecialSet extends CodePart & Special {}\nexport let Digit = do { class Digit extends SpecialSet {}; new Digit() };\nexport let Space = do { class Space extends SpecialSet {}; new Space() };\nexport let Word = do { class Word extends SpecialSet {}; new Word() };\n```\n\n</details>\n\n### CodeRange\n\nA code point range matches any code point in its inclusive bounds, such as\n`/[a-c]/`. In source, `-` is included in a code set either by escaping or by\nincluding it as the first or last character. A `CodeRange` is usually contained\ninside a [CodeSet](#codeset), and syntactically always is.\n\n```\nexport class CodeRange extends CodePart {\n  public min: Int;\n  public max: Int;\n}\n```\n\n### CodeSet\n\nA set of code points, any of which can match, such as `/[abc]/` matching any of\n`\"a\"`, `\"b\"`, or `\"c\"`. Alternatively, a negated set is the inverse of the code\npoints given, such as `/[^abc]/`, matching any code point that's not any of\nthese. This is also often called a character class.\n\nFurther, a subset of [specials](#specials) can also be used in code sets. A\nnegated code set of just a special set often has custom syntax. For example,\nnon-space can be said as either `/[^\\s]/` or `/\\S/`.\n\n```\nexport class CodeSet extends Regex {\n  public items: List<CodePart>;\n  public negated: Boolean = false;\n}\n```\n\n### Or\n\n`Or` matches any one of multiple options, such as `/ab|cd|e*/`.\n\n```\nexport class Or extends Regex {\n  public /*early*/ items: List<Regex>;\n}\n```\n\n### Repeat\n\n`Repeat` matches from an minimum to a maximum number of repeats of a\nsubregex. This can be represented in regex source in a number of ways:\n\n- `?` matches 0 or 1.\n- `*` matches 0 or more.\n- `+` matches 1 or more.\n- `{m}` matches exactly `m` repetitions.\n- `{m,n}` matches between `m` and `n`. Missing `n` is a max of infinity. For\n  example, `{0,1}` is equivalent to `?`, and `{1,}` is equivalent to `+`.\n\nBy default, repetitions are greedy, matching as many repetitions as possible.\nIn regex source, any of the above can have `?` appended to indicated reluctant\n(aka non-greedy), matching as few repetitions as possible.\n\n```\nexport class Repeat extends Regex {\n  public /*early*/ item: Regex;\n  public min: Int;\n  public max: Int | Null; // where null means infinite\n  public reluctant: Boolean = false;\n}\n```\n\nWe also have convenience builders.\n\n```\nexport let entire(item: Regex): Regex {\n  new Sequence([Begin, item, End])\n}\n\nexport let oneOrMore(item: Regex, reluctant: Boolean = false): Repeat {\n  { item, min: 1, max: null, reluctant }\n}\n\nexport let optional(item: Regex, reluctant: Boolean = false): Repeat {\n  { item, min: 0, max: 1, reluctant }\n}\n```\n\n### Sequence\n\n`Sequence` strings along multiple other regexes in order.\n\n```\nexport class Sequence extends Regex {\n  public /*early*/ items: List<Regex>;\n}\n```\n\n## Match Objects\n\nFor detailed match results, call `find` on a regex to get a `Map` object from\n`String` keys to `Group` values.\n\n```\n// TODO Go back to a `Match` object with `groups` as a member so we can also\n// TODO easily return metadata alongside groups? Or is simpler better?\n// export class Match { // interface ... <T = Map<String, Group>> {\n//   public let groups: Map<String, Group>;\n// }\n\nexport class Group {\n  public let name: String;\n  public let value: String;\n  public let codePointsBegin: Int;\n}\n```\n\n## Compiled Regex Objects\n\nThe compiled form of a regex is mostly opaque, but it can be cached for more\nefficient reuse than working from a source [Regex](#regex-data-model).\n\n<details>\n\n```\n// Provides a workaround for access to std/regex from extension methods.\nclass RegexRefs {\n  public let codePoints: CodePoints = new CodePoints(\"\");\n  public let group: Group = { name: \"\", value: \"\", codePointsBegin: 0 }\n  public let orObject: Or = new Or([]);\n}\n\nlet regexRefs = new RegexRefs();\n```\n\n</details>\n\n```\n// TODO(tjp, regex): Generate subtypes of this interface later.\nexport class CompiledRegex { // interface ... <T> {\n```\n\nThe source `Regex` data is still available on compiled objects in case it's\nneeded for composition or other purposes.\n\n```\n  public let data: Regex;\n\n  public constructor(data: Regex) {\n    this.data = data;\n    compiled = compileFormatted(format());\n  }\n```\n\nA compiled regex exposes many of the same capabilities as `Regex`, but they are\nmore efficient to use repeatedly.\n\n```\n  public found(text: String): Boolean { compiledFound(compiled, text) }\n\n  public find(text: String): Map<String, Group> | NoResult {\n    compiledFind(compiled, text, regexRefs)\n  }\n\n  public replace(\n    text: String, format: fn (Map<String, Group>): String\n  ): String {\n    compiledReplace(compiled, text, format, regexRefs)\n  }\n```\n\nTODO(tjp, regex): Public method for replace with named references.\nTODO(tjp, regex): Any static checking?\n\n<details>\n\n```\n  let compiled: AnyValue;\n\n  // Extension functions on some backends need the private `compiled` value\n  // passed in directly.\n  @connected(\"CompiledRegex::compiledFound\")\n  compiledFound(compiled: AnyValue, text: String): Boolean;\n\n  @connected(\"CompiledRegex::compiledFind\")\n  compiledFind(\n    compiled: AnyValue, text: String, regexRefs: RegexRefs\n  ): Map<String, Group> | NoResult;\n\n  @connected(\"CompiledRegex::compileFormatted\")\n  compileFormatted(formatted: String): AnyValue;\n\n  @connected(\"CompiledRegex::compiledReplace\")\n  compiledReplace(\n    compiled: AnyValue,\n    text: String,\n    format: fn (Map<String, Group>): String,\n    regexRefs: RegexRefs,\n  ): String;\n\n  @connected(\"CompiledRegex::format\")\n  format(): String { new RegexFormatter().format(data) }\n```\n\n</details>\n\n```\n}\n```\n\n## Private implementation matters\n\nSome regex logic can be shared across backends. These features aren't directly\nexported to the user, however.\n\nThe intent is that these support features only get included in compiled Temper\ncode if usage depends on dynamically constructed regexes. If all regex building\nis done as stable values, we hope to generated backend compiled regexes purely\nat Temper compile time.\n\n### RegexFormatter\n\n<details>\n\n```\nclass RegexFormatter {\n  let out: ListBuilder<String> = new ListBuilder<String>();\n\n  public format(regex: Regex): String {\n    pushRegex(regex)\n    out.join(\"\") { (x);; x }\n  }\n\n  pushRegex(regex: Regex): Void {\n    match (regex) {\n      // Aggregate types.\n      is Capture -> pushCapture(regex);\n      is CodePoints -> pushCodePoints(regex, false);\n      is CodeRange -> pushCodeRange(regex);\n      is CodeSet -> pushCodeSet(regex);\n      is Or -> pushOr(regex);\n      is Repeat -> pushRepeat(regex);\n      is Sequence -> pushSequence(regex);\n      // Specials.\n      // Some of these will need to be customized on future backends.\n      Begin -> out.add(\"^\");\n      Dot -> out.add(\".\");\n      End -> out.add(\"$\");\n      WordBoundary -> out.add(\"\\\\b\");\n      // Special sets.\n      Digit -> out.add(\"\\\\d\");\n      Space -> out.add(\"\\\\s\");\n      Word -> out.add(\"\\\\w\");\n      // ...\n    }\n  }\n\n  pushCapture(capture: Capture): Void {\n    out.add(\"(\");\n    // TODO(tjp, regex): Consistent name validation rules for all backends???\n    // TODO(tjp, regex): Validate here or in `Capture` constructor???\n    // TODO(tjp, regex): Validate here or where against reused names???\n    pushCaptureName(out, capture.name);\n    pushRegex(capture.item);\n    out.add(\")\");\n  }\n\n  @connected(\"RegexFormatter::pushCaptureName\")\n  pushCaptureName(out: ListBuilder<String>, name: String): Void {\n    // All so far except Python use this form.\n    out.add(\"?<${name}>\");\n  }\n\n  pushCode(code: Int, insideCodeSet: Boolean): Void {\n    // Expose private property to extension.\n    pushCodeTo(out, code, insideCodeSet);\n    // TODO(tjp, regex): Implement more in Temper once we can.\n    // if (escapeCodes[code] && false) {\n    //   out.add(\"\\\\\");\n    //   // TODO(tjp, regex): How to convert back to strings?\n    // }\n  }\n\n  @connected(\"RegexFormatter::pushCodeTo\")\n  pushCodeTo(out: ListBuilder<String>, code: Int, insideCodeSet: Boolean): Void;\n\n  pushCodePoints(codePoints: CodePoints, insideCodeSet: Boolean): Void {\n    for (\n      var slice = codePoints.value.codePoints;\n      !slice.isEmpty;\n      slice = slice.advance(1)\n    ) {\n      pushCode(slice.read(), insideCodeSet);\n    }\n  }\n\n  pushCodeRange(codeRange: CodeRange): Void {\n    out.add(\"[\");\n    pushCodeRangeUnwrapped(codeRange);\n    out.add(\"]\");\n  }\n\n  pushCodeRangeUnwrapped(codeRange: CodeRange): Void {\n    pushCode(codeRange.min, true);\n    out.add(\"-\");\n    pushCode(codeRange.max, true);\n  }\n\n  pushCodeSet(codeSet: CodeSet): Void {\n    let adjusted = adjustCodeSet(codeSet, regexRefs);\n    match (adjusted) {\n      is CodeSet -> do {\n        out.add(\"[\");\n        if (adjusted.negated) {\n          out.add(\"^\");\n        }\n        for (var i = 0; i < adjusted.items.length; i += 1) {\n          pushCodeSetItem(adjusted.items[i]);\n        }\n        out.add(\"]\");\n      }\n      else -> pushRegex(adjusted);\n    }\n  }\n\n  @connected(\"RegexFormatter::adjustCodeSet\")\n  adjustCodeSet(codeSet: CodeSet, regexRefs: RegexRefs): Regex { codeSet }\n\n  pushCodeSetItem(codePart: CodePart): Void {\n    match (codePart) {\n      is CodePoints -> pushCodePoints(codePart, true);\n      is CodeRange -> pushCodeRangeUnwrapped(codePart);\n      is SpecialSet -> pushRegex(codePart);\n    }\n  }\n\n  pushOr(or: Or): Void {\n    if (!or.items.isEmpty) {\n      out.add(\"(?:\");\n      // TODO(tjp, regex): See #822. Until `this` works better, no this in funs.\n      // TODO(tjp, regex): So just manually loop here. Sometimes faster, anyway?\n      pushRegex(or.items[0]);\n      for (var i = 1; i < or.items.length; i += 1) {\n        out.add(\"|\");\n        pushRegex(or.items[i]);\n      }\n      out.add(\")\");\n    }\n  }\n\n  pushRepeat(repeat: Repeat): Void {\n    // Always wrap the main sub-pattern here to make life easy\n    out.add(\"(?:\");\n    pushRegex(repeat.item);\n    out.add(\")\");\n    // Then add the repetition part.\n    let min = repeat.min;\n    let max = repeat.max;\n    if (false) {\n    } else if (min == 0 && max == 1) {\n      out.add(\"?\");\n    } else if (min == 0 && max == null) {\n      out.add(\"*\");\n    } else if (min == 1 && max == null) {\n      out.add(\"+\");\n    } else {\n      out.add(\"{${min.toString()}\");\n      if (min != max) {\n        out.add(\",\");\n        if (max != null) {\n          out.add(max.as<Int>().toString());\n        }\n      }\n      out.add(\"}\");\n    }\n    if (repeat.reluctant) {\n      out.add(\"?\");\n    }\n  }\n\n  pushSequence(sequence: Sequence): Void {\n    // TODO(tjp, regex): Foreach loop/function would be nice.\n    for (var i = 0; i < sequence.items.length; i += 1) {\n      pushRegex(sequence.items[i]);\n    }\n  }\n\n  // Put this here instead of the data model for now because I'm not sure this\n  // makes sense to be part of the public api right now.\n  public maxCode(codePart: CodePart): Int | Null {\n    match (codePart) {\n      is CodePoints -> do {\n        // Iterating code points is the hardest of the current cases.\n        let value = codePart.value;\n        if (value.isEmpty) {\n          null\n        } else {\n          // My kingdom for a fold, or even just a max, in builtins.\n          var max = 0;\n          for (\n            var slice = value.codePoints;\n            !slice.isEmpty;\n            slice = slice.advance(1)\n          ) {\n            let next = slice.read();\n            if (next > max) {\n              max = next;\n            }\n          }\n          max\n        }\n      }\n      // Others below are easy for now.\n      is CodeRange -> codePart.max;\n      Digit -> \"9\".codePoints.read();\n      Space -> \" \".codePoints.read();\n      Word -> \"z\".codePoints.read();\n      // Actually unexpected, ever, but eh.\n      else -> null;\n    }\n  }\n}\n\n// // TODO(tjp, regex): Delete all the below (comment included) if unused.\n// // TODO(tjp, regex): Replace all this with a compile-time regex once we can.\n// let escapeCodeList = [\n//   \"\\\\\".codePoints.read(),\n//   \"^\".codePoints.read(),\n//   \"$\".codePoints.read(),\n//   \"{\".codePoints.read(),\n//   \"[\".codePoints.read(),\n//   \"(\".codePoints.read(),\n//   \"}\".codePoints.read(),\n//   \"]\".codePoints.read(),\n//   \")\".codePoints.read(),\n//   \"|\".codePoints.read(),\n//   \"+\".codePoints.read(),\n//   \"?\".codePoints.read(),\n//   \"/\".codePoints.read(),\n//   \"*\".codePoints.read(),\n// ];\n// let escapeCodes = new DenseBitVector(128);\n// // This `for` loop has to be after type definitions for now because\n// // https://github.com/temper-lang/temper/issues/817\n// for (var i = 0; i < escapeCodeList.length; i += 1) {\n//   escapeCodes[i] = true;\n// }\n```\n\n</details>\n"
     ],
     "version": 3
 }
```

### Comparing `temper_std-0.0.3/temper_std/testing.py` & `temper_std-0.0.4/temper_std/testing.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,43 @@
-from abc import ABC as ABC3
-from builtins import list as list_1285
-from temper_core import temper_print as temper_print_1243, str_cat as str_cat_1241, list_join as list_join_1264, bool_not as bool_not_1270, list_builder_add as list_builder_add_1267
-TestFixtureBase = TestFixtureBase__6
-class TestFixtureBase__1(ABC3):
-  pass
-passing__2 = True
-t_76 = list_1285()
-messages__3 = t_76
-def test(name__4, body__5):
-  global messages__3, passing__2
-  passing__2 = True
-  t_68 = list_1285()
-  messages__3 = t_68
-  body__5()
-  if passing__2:
-    t_71 = temper_print_1243(str_cat_1241(name__4, ': Passed'))
-    t_39 = t_71
+from temper_core import TemperObject as TemperObject0, str_cat as str_cat_1212, list_join as list_join_1213, bool_not as bool_not_1214, list_builder_add as list_builder_add_1215
+from typing import List as List1, Callable as Callable2
+from builtins import list as list_1210
+from temper_core import LoggingConsole
+vGlobalConsole__36_1211 = LoggingConsole(__name__)
+class TestFixtureBase(TemperObject0):
+  __slots__ = ()
+passing__3: 'bool' = True
+t_72: 'List1[str]' = list_1210()
+messages__4: 'List1[str]' = t_72
+def test(name__5: 'str', body__6: 'Callable2[[], None]') -> 'None':
+  global list_1210, list_join_1213, messages__4, passing__3, str_cat_1212, vGlobalConsole__36_1211
+  return__1: 'None'
+  t_67: 'Callable2[[str], str]'
+  t_68: 'str'
+  return__1 = None
+  passing__3 = True
+  t_63: 'List1[str]' = list_1210()
+  messages__4 = t_63
+  body__6()
+  if passing__3:
+    vGlobalConsole__36_1211.log(str_cat_1212(name__5, ': Passed'))
   else:
-    def fn__65(it__7):
-      return__8 = it__7
-      return return__8
-    t_72 = fn__65
-    t_73 = list_join_1264(messages__3, '\n', t_72)
-    t_74 = temper_print_1243(str_cat_1241(name__4, ': Failed ', t_73))
-    t_39 = t_74
-  return__43 = t_39
-  return return__43
-def assert2(success__9, message__10):
-  global messages__3, passing__2
-  t_61 = bool_not_1270(success__9)
-  if t_61:
-    passing__2 = False
-    t_63 = message__10()
-    list_builder_add_1267(messages__3, t_63)
-  return__44 = None
-  return return__44
-return__42 = None
-export = return__42
+    def fn__61(it__8: 'str') -> 'str':
+      return__42: 'str'
+      return__42 = it__8
+      return return__42
+    t_67 = fn__61
+    t_68 = list_join_1213(messages__4, '\n', t_67)
+    vGlobalConsole__36_1211.log(str_cat_1212(name__5, ': Failed ', t_68))
+  return return__1
+def assert3(success__9: 'bool', message__10: 'Callable2[[], str]') -> 'None':
+  global bool_not_1214, list_builder_add_1215, messages__4, passing__3
+  return__2: 'None'
+  t_58: 'str'
+  return__2 = None
+  if bool_not_1214(success__9):
+    passing__3 = False
+    t_58 = message__10()
+    list_builder_add_1215(messages__4, t_58)
+  return return__2
+return__41: 'None' = None
+export = return__41
```

### Comparing `temper_std-0.0.3/temper_std/testing.py.map` & `temper_std-0.0.4/temper_std/testing.py.map`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7772108843537415%*

 * *Differences: {"'mappings'": "'A,wB,Y,I,a,E,O,I,Y,E,S,I,c,E,Q,I,a,E,gB,I;A,mB,I,I,K,E,Q,I;A,qB,I,I;AAcQ,gBAAO,OAAA,AAAP,eAAO;AAAP,uBAAO,EAAA,AAAP,eAAO,CAAA,AAAP,QAAO;AASM,MAAAa,eAAA,CAAAb,aAAgB,EAAA;AAAhB,WAAgB,EAAA,AAAhB,GAAgB;AArBrBc,UAAO,CAAE,OAAO,EAAG;AACRC,IAAyB,CAAA,AAAzB,aAAyB,EAAA,AAArB,CAAAH,SAAmB,EAAE;AAApCI,WAAQ,CAAA,AAAR,aAAQ,EAAG,CAAAD;AAKhB,GAAI,CAAAE,IAAI,CAAA,AAACC,OAAI,CAAE,MAAM,CAAE,CAAAC,OAAI,CAAE,sBAUnC,IAAA,AAViD,OAAI;AAErC,SAAAP,SAAmB,CAMQ,CAAAR,cAAI,CAAA,AAAb,CAAAY,WAAQ,CAAA,AAHrC,CAAAF,UAAO,CAGG,C […]*

```diff
@@ -1,47 +1,44 @@
 {
     "file": "OUTPUT_ROOT/temper-std/py/temper_std/testing.py",
-    "mappings": "A,gB,G,I;A,qB,I,I;A,wB,Y,I,iB,E,O,I,Y,E,S,I,c,E,Q,I,a,E,gB,I;AAiBiBa,eAAe,EAAC,CAAAA,kBAAA;AAAhB,MAAAA,kBAAA,CAAAb,IAAgB;AAAA,MAAA;AAhBrBc,UAAO,EAAY,KAAI;AACZC,IAAyB,EAAA,AAArB,CAAAb,SAAW,EAAU;AAApCc,WAAQ,EAAG,CAAAD,IAAyB;AAGzC,GAAI,CAAAE,IAAI,CAAA,AAACC,OAAY,CAAE,CAAAC,OAU7B,EAAA;AAF4B,SAAAH,WAAQ,CAAA,AAHhC,CAAAF,UAGgC;AAPnC,EAAAA,UAAO,EAAG,KAAI;AACH,EAAAM,IAAyB,EAAA,AAArB,CAAAlB,SAAW,EAAU;AAApC,EAAAc,WAAQ,EAAG,CAAAI,IAAyB;AAEpC,EAAAD,OAAI;AAAE,IACH,CAAAL,UAAO;AACR,IAAAO,IAAA,GAAAjB,iBAAK,CAACE,YAAA,CAAGY,OAAI,CAAC,WAAQ,CAAC,CAAC;AAAxB,IAAAI,IAAA,GAAAD,IAAwB;AAAxB;AAE6C,QAAAE,MAAA,CAAGC,KAA0B,EAAA;AAAb,MAAAC,SAAA,EAAS,CAAAD,KAAE;AAAA,YAAA,AAAX,CAAAC,SAAW;AAAE,IAAAC,IAAA,GAAAH,MAAA;AAAjD,IAAAI,IAAA,EAAS,CAAAnB,cAAI,CAAA,AAAbQ,WAAQ,CAAM,KAAI,CAAE,CAAAU,IAA6B,CAAA;AAA1E,IAAAE,IAAA,GAAAxB,iBAAK,CAACE,YAAA,CAAGY,OAAI,CAAC,YAAS,CAAE,CAAAS,IAAiD,CAAE,CAAC;AAA7E,IAAAL,IAAA,GAAAM,IAA6E;AARhC,EAAAH,UAAA,EAK/C,CAAAH,IAIC;AACF,QAAA,AAVgD,CAAAG;AAgB1C,GAAI,CAAAI,OAAM,CAAA,AAACC,UAAgB,CAAE,CAAAC,WAKnC,EAAA;AAFG,SAAAf,WAAQ,CAAA,AADR,CAAAF,UACQ;AAFP,EAAAkB,IAAQ,EAAA,AAAR,CAAAtB,aAAC,CAAAoB,UAAO,CAAA;AAAX,IAAG,CAAAE,IAAQ;AACT,IAAAlB,UAAO,EAAG,MAAK;AACF,IAAAmB,IAAA,GAAAF,WAAO,EAAE;AAAb,IAAAnB,qBAAG,CAAA,AAAZI,WAAQ,CAAK,CAAAiB,IAAS,CAEzB;AAL2D,EAAAR,UAAA,EAC1D,KAGC;AACF,QAAA,AAL2D,CAAAA,UAK3D;AAzBDA,UAAA,EAyBC,KAAA;AAAA,SAAAA",
+    "mappings": "A,wB,Y,I,a,E,O,I,Y,E,S,I,c,E,Q,I,a,E,gB,I;A,mB,I,I,K,E,Q,I;A,qB,I,I;AAcQ,gBAAO,OAAA,AAAP,eAAO;AAAP,uBAAO,EAAA,AAAP,eAAO,CAAA,AAAP,QAAO;AASM,MAAAa,eAAA,CAAAb,aAAgB,EAAA;AAAhB,WAAgB,EAAA,AAAhB,GAAgB;AArBrBc,UAAO,CAAE,OAAO,EAAG;AACRC,IAAyB,CAAA,AAAzB,aAAyB,EAAA,AAArB,CAAAH,SAAmB,EAAE;AAApCI,WAAQ,CAAA,AAAR,aAAQ,EAAG,CAAAD;AAKhB,GAAI,CAAAE,IAAI,CAAA,AAACC,OAAI,CAAE,MAAM,CAAE,CAAAC,OAAI,CAAE,sBAUnC,IAAA,AAViD,OAAI;AAErC,SAAAP,SAAmB,CAMQ,CAAAR,cAAI,CAAA,AAAb,CAAAY,WAAQ,CAAA,AAHrC,CAAAF,UAAO,CAGG,CAAAZ,YAAA,CAAA,AAAZ,CAAAkB,uBAAO;AARuC,EAAAC,SAAA;AAQkB,EAAAC,IAAA,yBAAA;AAAjC,EAAAC,IAAiC,CAAA,AAAjC;AAElC,EAAAF,SAAA,OAAA;AATC,EAAAP,UAAO,EAAG,KAAI;AACH,EAAAU,IAAyB,CAAA,AAAzB,aAAyB,EAAA,AAArB,CAAAZ,SAAmB,EAAE;AAApC,EAAAI,WAAQ,EAAG,CAAAQ,IAAyB;AAEpC,EAAAL,OAAI;AAAE,IACF,CAAAL,UAAO,CACD;AAAR,IAAAM,uBAAO,CAAA,AAAP,GAAW,CAAClB,YAAA,CAAGgB,OAAI,CAAC,WAAQ,CAAC;AAAC;AAEqB,QAAAO,MAAA,CAAGC,KAAE,CAAA,AAAF,MAAU,IAAA,AAAJ;AAAA,MAAAL,UAAA;AAAA,MAAAA,UAAA,GAAAK,KAAE;AAAA,YAAA,AAAF,CAAAL,UAAE;AAAE,IAAAC,IAAA,GAAAG,MAAA;AAAjC,IAAAF,IAAA,EAAS,CAAAnB,cAAI,CAAA,AAAbY,WAAQ,CAAM,KAAI,CAAE,CAAAM,IAAa,CAAA;AAAhE,IAAAF,uBAAO,CAAA,AAAP,GAAW,CAAClB,YAAA,CAAGgB,OAAI,CAAC,YAAS,CAAE,CAAAK,IAAiC,CAAE;AAErE,QAAA,AAViD,CAAAF;AAuB3C,GAAI,CAAAM,OAAM,CAAA,AAACC,UAAO,CAAE,OAAO,CAAE,CAAAC,WAAO,CAAE,qBAK5C,IAAA,AAL4D,OAAI;AAC3D,SAAAvB,aAAC,CAEM,CAAAE,qBAAG,CAAA,AAAZ,CAAAQ,WAAQ,CAAA,AADR,CAAAF,UAAO;AAFkD,EAAAO,SAAA;AAG5C,EAAAS,IAAS,CAAA,AAAT;AAEhB,EAAAT,SAAA,OAAA;AALiE,IAC5D,CAAAf,aAAC,CAAAsB,UAAO;AACV,IAAAd,UAAO,EAAG,MAAK;AACF,IAAAgB,IAAA,GAAAD,WAAO,EAAE;AAAb,IAAArB,qBAAG,CAAA,AAAZQ,WAAQ,CAAK,CAAAc,IAAS;AAEzB,QAAA,AAL4D,CAAAT,SAK5D;AAlCDA,UAAA,UAkCC,KAAA;AAAA,SAAAA",
     "names": [
-        "ABC",
-        "list",
-        "list#1285",
-        "temper_print",
-        "temper_print#1243",
+        "TemperObject",
         "str_cat",
-        "str_cat#1241",
+        "str_cat#1212",
         "list_join",
-        "list_join#1264",
+        "list_join#1213",
         "bool_not",
-        "bool_not#1270",
+        "bool_not#1214",
         "list_builder_add",
-        "list_builder_add#1267",
+        "list_builder_add#1215",
+        "List",
+        "Callable",
+        "list",
+        "list#1210",
         "TestFixtureBase",
         "passing",
-        "t#76",
+        "t#72",
         "messages",
         "test",
         "name",
         "body",
+        "vGlobalConsole__36#1211",
+        "return",
+        "t#67",
         "t#68",
-        "t#71",
-        "t#39",
+        "t#63",
         "fn",
         "it",
-        "return",
-        "t#72",
-        "t#73",
-        "t#74",
         "assert",
         "success",
         "message",
-        "t#61",
-        "t#63"
+        "t#58"
     ],
     "sources": [
         "std/testing.temper.md"
     ],
     "sourcesContent": [
-        "```temper ;lit\nprivate var passing: Boolean = true;\nprivate var messages = new ListBuilder<String>();\n\n@extension(\"::test\")\nexport let test(name: String, body: fn (): Void) {\n  passing = true;\n  messages = new ListBuilder<String>();\n  // TODO exception handling?\n  body();\n  if(passing) {\n    print(\"${name}: Passed\");\n  } else {\n    print(\"${name}: Failed ${messages.join(\"\\n\") { (it: String): String;; it }}\");\n  }\n}\n\nexport interface TestFixtureBase {\n\n}\n\nexport let assert(success: Boolean, message: fn (): String) {\n  if(!success) {\n    passing = false;\n    messages.add(message());\n  }\n}\n```\n"
+        "For now, we use mutable global state to track test results in the interpreter.\n\n    private var passing: Boolean = true;\n    private var messages = new ListBuilder<String>();\n\nTODO We looked at the idea of test blocks, but do we still support this?\n\n    @connected(\"::test\")\n    export let test(name: String, body: fn (): Void): Void {\n      passing = true;\n      messages = new ListBuilder<String>();\n      // TODO exception handling?\n      body();\n      if (passing) {\n        console.log(\"${name}: Passed\");\n      } else {\n        console.log(\"${name}: Failed ${messages.join(\"\\n\") { (it);; it }}\");\n      }\n    }\n\nCurrently for tests, you should extend `TestFixtureBase` and then decorate test\nmethods inside your test class with `@test`.\n\n    export interface TestFixtureBase {\n\n    }\n\nWe currently support a single `assert` method, for which we still need to refine\nhow we provide failure messages.\n\n    @connected(\"::assert\")\n    export let assert(success: Boolean, message: fn (): String): Void {\n      if (!success) {\n        passing = false;\n        messages.add(message());\n      }\n    }\n"
     ],
     "version": 3
 }
```

### Comparing `temper_std-0.0.3/temper_std/testing__preface.py.map` & `temper_std-0.0.4/temper_std/testing__preface.py.map`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'sourcesContent'": "['For now, we use mutable global state to track test results in the "*

 * *                     'interpreter.\\n\\n    private var passing: Boolean = true;\\n    private var '*

 * *                     'messages = new ListBuilder<String>();\\n\\nTODO We looked at the idea of '*

 * *                     'test blocks, but do we still support this?\\n\\n    '*

 * *                     '@connected("::test")\\n    export let test(name: String, body: fn (): Void): '*

 * *                     'Void {\\n      passing  […]*

```diff
@@ -4,11 +4,11 @@
     "names": [
         "return"
     ],
     "sources": [
         "std/testing.temper.md"
     ],
     "sourcesContent": [
-        "```temper ;lit\nprivate var passing: Boolean = true;\nprivate var messages = new ListBuilder<String>();\n\n@extension(\"::test\")\nexport let test(name: String, body: fn (): Void) {\n  passing = true;\n  messages = new ListBuilder<String>();\n  // TODO exception handling?\n  body();\n  if(passing) {\n    print(\"${name}: Passed\");\n  } else {\n    print(\"${name}: Failed ${messages.join(\"\\n\") { (it: String): String;; it }}\");\n  }\n}\n\nexport interface TestFixtureBase {\n\n}\n\nexport let assert(success: Boolean, message: fn (): String) {\n  if(!success) {\n    passing = false;\n    messages.add(message());\n  }\n}\n```\n"
+        "For now, we use mutable global state to track test results in the interpreter.\n\n    private var passing: Boolean = true;\n    private var messages = new ListBuilder<String>();\n\nTODO We looked at the idea of test blocks, but do we still support this?\n\n    @connected(\"::test\")\n    export let test(name: String, body: fn (): Void): Void {\n      passing = true;\n      messages = new ListBuilder<String>();\n      // TODO exception handling?\n      body();\n      if (passing) {\n        console.log(\"${name}: Passed\");\n      } else {\n        console.log(\"${name}: Failed ${messages.join(\"\\n\") { (it);; it }}\");\n      }\n    }\n\nCurrently for tests, you should extend `TestFixtureBase` and then decorate test\nmethods inside your test class with `@test`.\n\n    export interface TestFixtureBase {\n\n    }\n\nWe currently support a single `assert` method, for which we still need to refine\nhow we provide failure messages.\n\n    @connected(\"::assert\")\n    export let assert(success: Boolean, message: fn (): String): Void {\n      if (!success) {\n        passing = false;\n        messages.add(message());\n      }\n    }\n"
     ],
     "version": 3
 }
```

### Comparing `temper_std-0.0.3/PKG-INFO` & `temper_std-0.0.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: temper-std
-Version: 0.0.3
-Summary: 
+Version: 0.0.4
+Summary: Optional support library provided with Temper
+Home-page: https://temperlang.dev/
 License: Apache-2.0
-Requires-Python: >=3.6,<4.0
+Author: Temper Contributors
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: temper-core (==0.0.3)
+Requires-Dist: temper-core (==0.0.4)
+Project-URL: Repository, https://github.com/temper-lang/temper
```

