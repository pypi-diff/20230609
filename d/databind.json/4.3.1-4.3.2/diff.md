# Comparing `tmp/databind.json-4.3.1.tar.gz` & `tmp/databind.json-4.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databind.json-4.3.1.tar", max compression
+gzip compressed data, was "databind.json-4.3.2.tar", max compression
```

## Comparing `databind.json-4.3.1.tar` & `databind.json-4.3.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     3339 2023-06-07 22:10:11.709365 databind.json-4.3.1/README.md
--rw-r--r--   0        0        0     1563 2023-06-09 13:14:16.060716 databind.json-4.3.1/pyproject.toml
--rw-r--r--   0        0        0     2411 2023-06-09 13:14:16.060716 databind.json-4.3.1/src/databind/json/__init__.py
--rw-r--r--   0        0        0    34633 2023-06-09 13:14:11.728672 databind.json-4.3.1/src/databind/json/converters.py
--rw-r--r--   0        0        0     2706 2023-06-07 22:10:11.709365 databind.json-4.3.1/src/databind/json/module.py
--rw-r--r--   0        0        0        0 2023-06-07 22:10:11.709365 databind.json-4.3.1/src/databind/json/py.typed
--rw-r--r--   0        0        0     1773 2023-06-07 22:10:11.709365 databind.json-4.3.1/src/databind/json/settings.py
--rw-r--r--   0        0        0    20840 2023-06-09 13:14:11.728672 databind.json-4.3.1/src/databind/json/tests/converters_test.py
--rw-r--r--   0        0        0     4246 2023-06-09 13:14:30.710408 databind.json-4.3.1/setup.py
--rw-r--r--   0        0        0     4368 2023-06-09 13:14:30.710867 databind.json-4.3.1/PKG-INFO
+-rw-r--r--   0        0        0     3339 2023-06-07 22:10:11.709365 databind.json-4.3.2/README.md
+-rw-r--r--   0        0        0     1563 2023-06-09 13:43:37.674709 databind.json-4.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2411 2023-06-09 13:43:37.674709 databind.json-4.3.2/src/databind/json/__init__.py
+-rw-r--r--   0        0        0    34876 2023-06-09 13:40:15.388664 databind.json-4.3.2/src/databind/json/converters.py
+-rw-r--r--   0        0        0     2706 2023-06-07 22:10:11.709365 databind.json-4.3.2/src/databind/json/module.py
+-rw-r--r--   0        0        0        0 2023-06-07 22:10:11.709365 databind.json-4.3.2/src/databind/json/py.typed
+-rw-r--r--   0        0        0     1773 2023-06-07 22:10:11.709365 databind.json-4.3.2/src/databind/json/settings.py
+-rw-r--r--   0        0        0    20842 2023-06-09 13:40:08.508594 databind.json-4.3.2/src/databind/json/tests/converters_test.py
+-rw-r--r--   0        0        0     4246 2023-06-09 13:43:50.705751 databind.json-4.3.2/setup.py
+-rw-r--r--   0        0        0     4368 2023-06-09 13:43:50.706195 databind.json-4.3.2/PKG-INFO
```

### Comparing `databind.json-4.3.1/README.md` & `databind.json-4.3.2/README.md`

 * *Files identical despite different names*

### Comparing `databind.json-4.3.1/pyproject.toml` & `databind.json-4.3.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "databind.json"
-version = "4.3.1"
+version = "4.3.2"
 description = "De-/serialize Python dataclasses to or from JSON payloads. Compatible with Python 3.7 and newer."
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "databind/json", from = "src"}]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/NiklasRosenstein/python-databind/issues"
 Documentation = "https://niklasrosenstein.github.io/python-databind/"
 # Homepage = ""
 Repository = "https://github.com/NiklasRosenstein/python-databind"
 
 [tool.poetry.dependencies]
 python = "^3.6.3"
-"databind.core" = "^4.3.1"
+"databind.core" = "^4.3.2"
 nr-date = "^2.0.0"
 typeapi = "^1.4.2"
 typing-extensions = ">=3.10.0"
 
 [tool.poetry.dev-dependencies]
 black = "*"
 flake8 = "*"
```

### Comparing `databind.json-4.3.1/src/databind/json/__init__.py` & `databind.json-4.3.2/src/databind/json/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing as t
 
 from databind.core import ObjectMapper, Setting, Settings
 
 from databind.json.module import JsonModule
 from databind.json.settings import JsonConverter
 
-__version__ = "4.3.1"
+__version__ = "4.3.2"
 __all__ = [
     "dump",
     "dumps",
     "get_object_mapper",
     "JsonConverter",
     "JsonModule",
     "JsonType",
```

### Comparing `databind.json-4.3.1/src/databind/json/converters.py` & `databind.json-4.3.2/src/databind/json/converters.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,17 @@
             isinstance(datatype, ClassTypeHint)
             and issubclass(datatype.type, tuple)
             and getattr(datatype.type, "__annotations__", None)
         ):
             schema = Schema(
                 fields={
                     name: Field(
-                        datatype=TypeHint(type_),
+                        # We need to evaluate the type hint to remove forward references. The source is needed to
+                        # understand the context in which forward references must be evaluated.
+                        datatype=TypeHint(type_, source=datatype.type).evaluate(),
                     )
                     for name, type_ in getattr(datatype.type, "__annotations__").items()
                 },
                 constructor=datatype.type,
                 type=datatype.type,
             )
             if ctx.direction.is_serialize():
```

### Comparing `databind.json-4.3.1/src/databind/json/module.py` & `databind.json-4.3.2/src/databind/json/module.py`

 * *Files identical despite different names*

### Comparing `databind.json-4.3.1/src/databind/json/settings.py` & `databind.json-4.3.2/src/databind/json/settings.py`

 * *Files identical despite different names*

### Comparing `databind.json-4.3.1/src/databind/json/tests/converters_test.py` & `databind.json-4.3.2/src/databind/json/tests/converters_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -535,11 +535,11 @@
 
 
 def test__typing_NamedTuple() -> None:
     mapper = make_mapper([CollectionConverter(), PlainDatatypeConverter()])
 
     class Nt(t.NamedTuple):
         a: int
-        b: str
+        b: "str"
 
     assert mapper.serialize(Nt(1, "2"), Nt) == {"a": 1, "b": "2"}
     assert mapper.deserialize({"a": 1, "b": "2"}, Nt) == Nt(1, "2")
```

### Comparing `databind.json-4.3.1/setup.py` & `databind.json-4.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 packages = \
 ['json', 'json.tests']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['databind.core>=4.3.1,<5.0.0',
+['databind.core>=4.3.2,<5.0.0',
  'nr-date>=2.0.0,<3.0.0',
  'typeapi>=1.4.2,<2.0.0',
  'typing-extensions>=3.10.0']
 
 setup_kwargs = {
     'name': 'databind.json',
-    'version': '4.3.1',
+    'version': '4.3.2',
     'description': 'De-/serialize Python dataclasses to or from JSON payloads. Compatible with Python 3.7 and newer.',
     'long_description': '# databind.json\n\nThe `databind.json` package implements the de-/serialization to or from JSON payloads using\nthe `databind.core` framework.\n\nCheck out the [Documentation][0] for examples.\n\n[0]: https://niklasrosenstein.github.io/python-databind/\n\n## Built-in converters\n\nThe following tables shows which types can be deserialized from / serialize to Python types with the native\nconverters provided by the `databind.json` module:\n\n| Converter name | Types | Description |\n| -------------- | ----- | ----------- |\n| `AnyConverter` | `typing.Any` | Accept any value (useful for arbitrary JSON). |\n| `CollectionConverter` | `typing.Collection[T]`, excl. `str`, `bytes`, `bytearray`, `memoryview` and `typing.Mapping[K, V]` | Converts between native Python collections and JSON arrays. |\n| `DatetimeConverter` | `datetime.date`, `datetime.datetime`, `datetime.time` | Converts between strings and date/time formats, using ISO 8601 time format by default (can be changed with the `databind.core.settings.DateFormat` setting). |\n| `DecimalConverter` | `decimal.Decimal` | Converts between strings (and ints/floats if strict mode is off, strict mode is on by default) and decimals. The precision can be controlled with the `databind.core.settings.Precision` setting. |\n| `EnumConverter` | `enum.Enum`, `enum.IntEnum` | Convert between strings and Python enumerations. The serialized form of `IntEnum` is the integer value, whereas the serialized form of `Enum` is a string (name of the enumeration value). |\n| `MappingConverter` | `typing.Mapping[K, V]` | Converts between Python dicts and JSON objects. (While in theory `K` can be any type, for JSON `K` always needs to be `str`). |\n| `OptionalConverter` | `typing.Optional[T]` | Handles optional fields in a schema. |\n| `PlainDatatypeConverter` | `bytes`, `str`, `int`, `float`, `bool` | Converts between plain datatypes. In non-strict mode (off by default), numeric types will also accept strings as input for the deserialization. |\n| `SchemaConverter` | `dataclasses.dataclass`, `typing.TypedDict` | Converts between Python dataclasses or typed dictionary and JSON objects. |\n| `UnionConverter` | `typing.Union[...]` | Handles union types. Unions in JSON can be expressed in a multitide of ways, e.g. using a discriminator key and flat, keyed or nested structure or "best match". Check out the examples section of the documentation for more information. |\n| `LiteralConverter` | `typing.Literal[...]` | Accepts or rejects a value based on whether it matches one of the values in the literal type hint. |\n\n\nThe following converters are provided for convenience:\n\n| Converter name | Types | Description |\n| -------------- | ----- | ----------- |\n| `StringifyConverter` | n/a | A helper that allows to easily create de/serializers from a "to string" and "from string" function. |\n\nThe following additional types are natively supported by `databind.json` using `StringifyConverter`:\n\n| Types | Description |\n| ----- | ----------- |\n| `uuid.UUID` | Convert between strings and UUIDs. |\n| `pathlib.Path` | Convert between strings and paths. |\n| `pathlib.PurePath` | Convert between strings and paths. |\n| `nr.date.duration` | Deserialize from ISO 8601 duration strings or the object form, serialize to ISO 8601 strings. |\n\n---\n\n<p align="center">Copyright &copy; 2020 &ndash; Niklas Rosenstein</p>\n',
     'author': 'Niklas Rosenstein',
     'author_email': 'rosensteinniklas@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `databind.json-4.3.1/PKG-INFO` & `databind.json-4.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: databind.json
-Version: 4.3.1
+Version: 4.3.2
 Summary: De-/serialize Python dataclasses to or from JSON payloads. Compatible with Python 3.7 and newer.
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.6.3,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: databind.core (>=4.3.1,<5.0.0)
+Requires-Dist: databind.core (>=4.3.2,<5.0.0)
 Requires-Dist: nr-date (>=2.0.0,<3.0.0)
 Requires-Dist: typeapi (>=1.4.2,<2.0.0)
 Requires-Dist: typing-extensions (>=3.10.0)
 Project-URL: Bug Tracker, https://github.com/NiklasRosenstein/python-databind/issues
 Project-URL: Documentation, https://niklasrosenstein.github.io/python-databind/
 Project-URL: Repository, https://github.com/NiklasRosenstein/python-databind
 Description-Content-Type: text/markdown
```

