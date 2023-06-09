# Comparing `tmp/TheengsDecoder-1.4.2.tar.gz` & `tmp/TheengsDecoder-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TheengsDecoder-1.4.2.tar", last modified: Thu May 11 12:14:59 2023, max compression
+gzip compressed data, was "TheengsDecoder-1.5.0.tar", last modified: Fri Jun  9 00:04:46 2023, max compression
```

## Comparing `TheengsDecoder-1.4.2.tar` & `TheengsDecoder-1.5.0.tar`

### file list

```diff
@@ -1,272 +1,276 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 12:14:59.581378 TheengsDecoder-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1266 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)    35147 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2443 2023-05-11 12:14:59.581378 TheengsDecoder-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2222 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 12:14:59.529377 TheengsDecoder-1.4.2/TheengsDecoder/
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/TheengsDecoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2521 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/TheengsDecoder/_decoder.cpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 12:14:59.529377 TheengsDecoder-1.4.2/TheengsDecoder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2443 2023-05-11 12:14:59.000000 TheengsDecoder-1.4.2/TheengsDecoder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    11421 2023-05-11 12:14:59.000000 TheengsDecoder-1.4.2/TheengsDecoder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 12:14:59.000000 TheengsDecoder-1.4.2/TheengsDecoder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-11 12:14:59.000000 TheengsDecoder-1.4.2/TheengsDecoder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      123 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-11 12:14:59.581378 TheengsDecoder-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1395 2023-05-11 12:14:56.000000 TheengsDecoder-1.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 12:14:59.533377 TheengsDecoder-1.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 12:14:59.533377 TheengsDecoder-1.4.2/src/arduino_json/
--rw-r--r--   0 runner    (1001) docker     (122)      283 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/.clang-format
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-05-11 12:14:45.000000 TheengsDecoder-1.4.2/src/arduino_json/.git
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (122)      241 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/.mbedignore
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/ArduinoJson.h
--rw-r--r--   0 runner    (1001) docker     (122)    40084 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)      265 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (122)    10845 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      871 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/SUPPORT.md
--rw-r--r--   0 runner    (1001) docker     (122)      894 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/appveyor.yml
--rw-r--r--   0 runner    (1001) docker     (122)    32515 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/banner.svg
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/component.mk
--rw-r--r--   0 runner    (1001) docker     (122)      932 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/keywords.txt
--rw-r--r--   0 runner    (1001) docker     (122)      852 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/library.json
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/library.properties
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 12:14:59.537377 TheengsDecoder-1.4.2/src/arduino_json/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 12:14:59.537377 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 12:14:59.537377 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Array/
--rw-r--r--   0 runner    (1001) docker     (122)      807 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Array/ArrayFunctions.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      746 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Array/ArrayImpl.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2413 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Array/ArrayIterator.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     5393 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Array/ArrayRef.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1308 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Array/ArrayShortcuts.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     5295 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Array/ElementProxy.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3810 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Array/Utilities.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 12:14:59.537377 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Collection/
--rw-r--r--   0 runner    (1001) docker     (122)     1960 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Collection/CollectionData.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     5837 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Collection/CollectionImpl.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     7657 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Configuration.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 12:14:59.541377 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Deserialization/
--rw-r--r--   0 runner    (1001) docker     (122)     3587 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Deserialization/DeserializationError.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1197 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Deserialization/Filter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      630 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Deserialization/NestingLimit.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Deserialization/Reader.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 12:14:59.541377 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Deserialization/Readers/
--rw-r--r--   0 runner    (1001) docker     (122)      700 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Deserialization/Readers/ArduinoStreamReader.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      450 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Deserialization/Readers/ArduinoStringReader.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1172 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Deserialization/Readers/FlashReader.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Deserialization/Readers/IteratorReader.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Deserialization/Readers/RamReader.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      680 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Deserialization/Readers/StdStreamReader.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Deserialization/Readers/VariantReader.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3108 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Deserialization/deserialize.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 12:14:59.541377 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Document/
--rw-r--r--   0 runner    (1001) docker     (122)     4061 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Document/BasicJsonDocument.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      573 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Document/DynamicJsonDocument.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     9071 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Document/JsonDocument.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1230 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Document/StaticJsonDocument.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 12:14:59.545377 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Json/
--rw-r--r--   0 runner    (1001) docker     (122)      828 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Json/EscapeSequence.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    18680 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Json/JsonDeserializer.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2946 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Json/JsonSerializer.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Json/Latch.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2233 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Json/PrettyJsonSerializer.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3937 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Json/TextFormatter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Json/Utf16.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1192 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Json/Utf8.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 12:14:59.545377 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Memory/
--rw-r--r--   0 runner    (1001) docker     (122)     1165 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Memory/Alignment.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     4855 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Memory/MemoryPool.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 12:14:59.545377 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Misc/
--rw-r--r--   0 runner    (1001) docker     (122)     1370 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Misc/SerializedValue.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      453 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Misc/Visitable.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 12:14:59.545377 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/MsgPack/
--rw-r--r--   0 runner    (1001) docker     (122)    15856 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/MsgPack/MsgPackDeserializer.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     5241 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/MsgPack/MsgPackSerializer.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      972 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/MsgPack/endianess.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      489 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/MsgPack/ieee754.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1226 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Namespace.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 12:14:59.549378 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Numbers/
--rw-r--r--   0 runner    (1001) docker     (122)      345 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Numbers/Float.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2296 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Numbers/FloatParts.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     5880 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Numbers/FloatTraits.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      952 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Numbers/Integer.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3965 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Numbers/arithmeticCompare.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3763 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Numbers/convertNumber.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3682 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Numbers/parseNumber.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 12:14:59.549378 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Object/
--rw-r--r--   0 runner    (1001) docker     (122)     5644 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Object/MemberProxy.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1296 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Object/ObjectFunctions.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2155 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Object/ObjectImpl.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2309 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Object/ObjectIterator.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     7676 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Object/ObjectRef.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2440 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Object/ObjectShortcuts.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1001 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Object/Pair.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 12:14:59.553377 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/
--rw-r--r--   0 runner    (1001) docker     (122)      526 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/alias_cast.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      293 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/assert.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1309 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/attributes.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      370 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/ctype.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      471 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/integer.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      922 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/limits.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      491 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/math.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 12:14:59.553377 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/mpl/
--rw-r--r--   0 runner    (1001) docker     (122)      560 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/mpl/max.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1901 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/pgmspace.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      865 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/pgmspace_generic.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/preprocessor.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      583 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/safe_strcmp.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      889 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/static_array.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 12:14:59.557378 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/
--rw-r--r--   0 runner    (1001) docker     (122)      451 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/conditional.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      257 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/declval.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      423 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/enable_if.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      408 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/integral_constant.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      439 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_array.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      672 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_base_of.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      560 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_class.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      405 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_const.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      992 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_convertible.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      560 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_enum.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      490 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_floating_point.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1395 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_integral.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      335 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_pointer.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      411 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_same.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_signed.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      904 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_unsigned.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/make_unsigned.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      251 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/make_void.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      429 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/remove_const.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      508 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/remove_cv.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      437 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/remove_reference.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      283 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/type_identity.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      849 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/type_traits.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      535 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/utility.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 12:14:59.557378 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Serialization/
--rw-r--r--   0 runner    (1001) docker     (122)      608 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Serialization/CountingDecorator.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Serialization/Writer.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 12:14:59.557378 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Serialization/Writers/
--rw-r--r--   0 runner    (1001) docker     (122)      993 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Serialization/Writers/ArduinoStringWriter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Serialization/Writers/DummyWriter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      564 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Serialization/Writers/PrintWriter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      670 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Serialization/Writers/StaticStringWriter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      686 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Serialization/Writers/StdStreamWriter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      924 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Serialization/Writers/StdStringWriter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      452 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Serialization/measure.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1971 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Serialization/serialize.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 12:14:59.561378 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/StringStorage/
--rw-r--r--   0 runner    (1001) docker     (122)     1281 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/StringStorage/StringCopier.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      724 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/StringStorage/StringMover.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      616 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/StringStorage/StringStorage.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 12:14:59.561378 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Strings/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 12:14:59.561378 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Strings/Adapters/
--rw-r--r--   0 runner    (1001) docker     (122)     1159 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Strings/Adapters/ArduinoStringAdapter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Strings/Adapters/ConstRamStringAdapter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Strings/Adapters/FlashStringAdapter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      623 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Strings/Adapters/JsonStringAdapter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      844 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Strings/Adapters/RamStringAdapter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Strings/Adapters/SizedFlashStringAdapter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      855 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Strings/Adapters/SizedRamStringAdapter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      994 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Strings/Adapters/StdStringAdapter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      843 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Strings/Adapters/StringViewAdapter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      772 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Strings/IsWriteableString.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      328 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Strings/StoragePolicy.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Strings/String.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      798 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Strings/StringAdapter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      864 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Strings/StringAdapters.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 12:14:59.565378 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Variant/
--rw-r--r--   0 runner    (1001) docker     (122)      416 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Variant/Converter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     7215 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Variant/ConverterImpl.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1729 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Variant/SlotFunctions.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     5098 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Variant/VariantCompare.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1133 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Variant/VariantContent.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     9517 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Variant/VariantData.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2908 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Variant/VariantFunctions.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     4300 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Variant/VariantImpl.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     5651 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Variant/VariantOperators.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    10885 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Variant/VariantRef.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      750 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Variant/VariantShortcuts.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2995 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Variant/VariantSlot.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      316 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Variant/VariantTag.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      618 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Variant/VariantTo.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      988 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Variant/Visitor.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      827 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/compatibility.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      259 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/version.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      291 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson.h
--rw-r--r--   0 runner    (1001) docker     (122)     2717 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2157 2023-05-11 12:14:46.000000 TheengsDecoder-1.4.2/src/arduino_json/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)    29794 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/decoder.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3750 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/decoder.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 12:14:59.581378 TheengsDecoder-1.4.2/src/devices/
--rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/ABN03_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/ABTemp_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1642 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/APPLE_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/Amphiro_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2242 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/BC08_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1301 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/BM1IN1_json.h
--rw-r--r--   0 runner    (1001) docker     (122)      857 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/BM2_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2160 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/BM3IN1_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2048 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/BM4IN1_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2962 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/BPARASITE_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1178 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/BWBSDOO_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1380 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/CGD1_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     3733 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/CGDK2_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2319 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/CGDN1_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     6309 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/CGG1_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1308 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/CGH1_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1643 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/CGP1W_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2475 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/CGPR1_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/GAEN_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     4840 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/H5055_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1928 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/H5072_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1269 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/H5074_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2134 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/H5102_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2794 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/H5106_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2273 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/HHCCJCY01HHCC_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2128 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/HHCCJCY10_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1238 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/HHCCPOT002_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2271 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/IBS_THBP01B_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     3386 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/IBT_2X_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2802 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/IBT_4XS_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     3854 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/IBT_6XS_SOLIS6_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1293 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/JHT_F525_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2251 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/JQJCY01YM_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/LYWSD02_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2864 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/LYWSD03MMC_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1767 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/LYWSDCGQ_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     3892 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/MBXPRO_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     3409 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/MS_CDP_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/MUE4094RT_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1960 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/Miband_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1942 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/Mokobeacon_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     4425 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/Mopeka_json.h
--rw-r--r--   0 runner    (1001) docker     (122)      819 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/PH10_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     8958 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/RDL52832_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     3271 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/RuuviTag_RAWv1_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     4454 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/RuuviTag_RAWv2_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     3798 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/SBCS_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2440 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/SBCU_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     3468 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/SBMS_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2189 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/SBMT_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2150 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/SBOT_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1585 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/SBS1_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1794 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/SCD4X_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/SHT4X_json.h
--rw-r--r--   0 runner    (1001) docker     (122)      779 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/ServiceData_json.h
--rw-r--r--   0 runner    (1001) docker     (122)      864 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/Skale_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2193 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/SmartDry_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1196 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/T201_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1194 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/T301_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2445 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/TPMS_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1165 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/TPTH_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     4690 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/ThermoBeacon_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2129 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/XMTZC04HM_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/XMTZC05HM_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/common_props.h
--rw-r--r--   0 runner    (1001) docker     (122)     2646 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/iBeacon_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     3789 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/iNodeEM_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     3173 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices/tracker_json.h
--rw-r--r--   0 runner    (1001) docker     (122)     6414 2023-05-11 12:14:44.000000 TheengsDecoder-1.4.2/src/devices.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.259791 TheengsDecoder-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1434 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    35147 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2610 2023-06-09 00:04:46.259791 TheengsDecoder-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2389 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.235791 TheengsDecoder-1.5.0/TheengsDecoder/
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/TheengsDecoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2521 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/TheengsDecoder/_decoder.cpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.239791 TheengsDecoder-1.5.0/TheengsDecoder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2610 2023-06-09 00:04:46.000000 TheengsDecoder-1.5.0/TheengsDecoder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    11521 2023-06-09 00:04:46.000000 TheengsDecoder-1.5.0/TheengsDecoder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-09 00:04:46.000000 TheengsDecoder-1.5.0/TheengsDecoder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-09 00:04:46.000000 TheengsDecoder-1.5.0/TheengsDecoder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      123 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-09 00:04:46.259791 TheengsDecoder-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1395 2023-06-09 00:04:43.000000 TheengsDecoder-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.239791 TheengsDecoder-1.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.239791 TheengsDecoder-1.5.0/src/arduino_json/
+-rw-r--r--   0 runner    (1001) docker     (122)      283 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-06-09 00:04:31.000000 TheengsDecoder-1.5.0/src/arduino_json/.git
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (122)      241 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/.mbedignore
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/ArduinoJson.h
+-rw-r--r--   0 runner    (1001) docker     (122)    40084 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      265 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (122)    10845 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      871 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/SUPPORT.md
+-rw-r--r--   0 runner    (1001) docker     (122)      894 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/appveyor.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    32515 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/banner.svg
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/component.mk
+-rw-r--r--   0 runner    (1001) docker     (122)      932 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/keywords.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      852 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/library.json
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/library.properties
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.239791 TheengsDecoder-1.5.0/src/arduino_json/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.239791 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.243791 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Array/
+-rw-r--r--   0 runner    (1001) docker     (122)      807 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Array/ArrayFunctions.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      746 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Array/ArrayImpl.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2413 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Array/ArrayIterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5393 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Array/ArrayRef.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1308 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Array/ArrayShortcuts.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5295 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Array/ElementProxy.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3810 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Array/Utilities.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.243791 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Collection/
+-rw-r--r--   0 runner    (1001) docker     (122)     1960 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Collection/CollectionData.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5837 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Collection/CollectionImpl.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7657 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Configuration.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.243791 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/
+-rw-r--r--   0 runner    (1001) docker     (122)     3587 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/DeserializationError.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1197 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/Filter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      630 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/NestingLimit.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/Reader.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.243791 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/
+-rw-r--r--   0 runner    (1001) docker     (122)      700 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/ArduinoStreamReader.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      450 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/ArduinoStringReader.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1172 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/FlashReader.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/IteratorReader.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/RamReader.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      680 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/StdStreamReader.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/VariantReader.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3108 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/deserialize.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.243791 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Document/
+-rw-r--r--   0 runner    (1001) docker     (122)     4061 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Document/BasicJsonDocument.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      573 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Document/DynamicJsonDocument.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     9071 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Document/JsonDocument.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1230 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Document/StaticJsonDocument.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.243791 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Json/
+-rw-r--r--   0 runner    (1001) docker     (122)      828 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Json/EscapeSequence.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    18680 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Json/JsonDeserializer.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2946 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Json/JsonSerializer.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Json/Latch.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2233 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Json/PrettyJsonSerializer.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3937 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Json/TextFormatter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Json/Utf16.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1192 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Json/Utf8.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.243791 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Memory/
+-rw-r--r--   0 runner    (1001) docker     (122)     1165 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Memory/Alignment.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4855 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Memory/MemoryPool.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.243791 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Misc/
+-rw-r--r--   0 runner    (1001) docker     (122)     1370 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Misc/SerializedValue.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      453 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Misc/Visitable.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.243791 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/MsgPack/
+-rw-r--r--   0 runner    (1001) docker     (122)    15856 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/MsgPack/MsgPackDeserializer.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5241 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/MsgPack/MsgPackSerializer.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      972 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/MsgPack/endianess.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      489 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/MsgPack/ieee754.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1226 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Namespace.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.243791 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Numbers/
+-rw-r--r--   0 runner    (1001) docker     (122)      345 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Numbers/Float.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2296 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Numbers/FloatParts.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5880 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Numbers/FloatTraits.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      952 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Numbers/Integer.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3965 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Numbers/arithmeticCompare.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3763 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Numbers/convertNumber.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3682 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Numbers/parseNumber.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.247791 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Object/
+-rw-r--r--   0 runner    (1001) docker     (122)     5644 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Object/MemberProxy.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1296 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Object/ObjectFunctions.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2155 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Object/ObjectImpl.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2309 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Object/ObjectIterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7676 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Object/ObjectRef.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2440 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Object/ObjectShortcuts.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1001 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Object/Pair.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.247791 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/
+-rw-r--r--   0 runner    (1001) docker     (122)      526 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/alias_cast.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      293 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/assert.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1309 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/attributes.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      370 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/ctype.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      471 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/integer.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      922 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/limits.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      491 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/math.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.247791 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/mpl/
+-rw-r--r--   0 runner    (1001) docker     (122)      560 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/mpl/max.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1901 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/pgmspace.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      865 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/pgmspace_generic.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/preprocessor.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      583 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/safe_strcmp.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      889 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/static_array.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.251791 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/
+-rw-r--r--   0 runner    (1001) docker     (122)      451 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/conditional.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      257 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/declval.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      423 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/enable_if.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      408 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/integral_constant.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      439 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_array.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      672 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_base_of.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      560 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_class.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      405 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_const.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      992 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_convertible.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      560 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_enum.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      490 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_floating_point.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1395 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_integral.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      335 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_pointer.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      411 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_same.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_signed.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      904 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_unsigned.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/make_unsigned.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      251 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/make_void.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      429 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/remove_const.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      508 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/remove_cv.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      437 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/remove_reference.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      283 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/type_identity.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      849 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      535 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/utility.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.251791 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Serialization/
+-rw-r--r--   0 runner    (1001) docker     (122)      608 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Serialization/CountingDecorator.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Serialization/Writer.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.251791 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Serialization/Writers/
+-rw-r--r--   0 runner    (1001) docker     (122)      993 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Serialization/Writers/ArduinoStringWriter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Serialization/Writers/DummyWriter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      564 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Serialization/Writers/PrintWriter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      670 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Serialization/Writers/StaticStringWriter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      686 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Serialization/Writers/StdStreamWriter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      924 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Serialization/Writers/StdStringWriter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      452 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Serialization/measure.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1971 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Serialization/serialize.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.251791 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/StringStorage/
+-rw-r--r--   0 runner    (1001) docker     (122)     1281 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/StringStorage/StringCopier.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      724 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/StringStorage/StringMover.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      616 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/StringStorage/StringStorage.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.251791 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.251791 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/
+-rw-r--r--   0 runner    (1001) docker     (122)     1159 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/ArduinoStringAdapter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/ConstRamStringAdapter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/FlashStringAdapter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      623 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/JsonStringAdapter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      844 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/RamStringAdapter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/SizedFlashStringAdapter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      855 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/SizedRamStringAdapter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      994 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/StdStringAdapter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      843 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/StringViewAdapter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      772 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/IsWriteableString.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      328 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/StoragePolicy.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/String.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      798 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/StringAdapter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      864 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/StringAdapters.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.251791 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/
+-rw-r--r--   0 runner    (1001) docker     (122)      416 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/Converter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7215 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/ConverterImpl.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1729 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/SlotFunctions.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5098 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/VariantCompare.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1133 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/VariantContent.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     9517 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/VariantData.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2908 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/VariantFunctions.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4300 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/VariantImpl.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5651 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/VariantOperators.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    10885 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/VariantRef.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      750 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/VariantShortcuts.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2995 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/VariantSlot.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/VariantTag.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      618 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/VariantTo.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      988 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/Visitor.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      827 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/compatibility.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      259 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/version.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      291 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2717 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2157 2023-06-09 00:04:32.000000 TheengsDecoder-1.5.0/src/arduino_json/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    29875 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/decoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3790 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/decoder.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2025 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/decoder_c.cpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:04:46.259791 TheengsDecoder-1.5.0/src/devices/
+-rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/ABN03_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/ABTemp_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1642 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/APPLE_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/Amphiro_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2595 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/BC08_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1301 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/BM1IN1_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)      857 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/BM2_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2160 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/BM3IN1_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2048 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/BM4IN1_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2962 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/BPARASITE_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1178 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/BWBSDOO_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1380 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/CGD1_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3733 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/CGDK2_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2319 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/CGDN1_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     6179 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/CGG1_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1308 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/CGH1_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1643 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/CGP1W_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2475 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/CGPR1_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/GAEN_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4840 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/H5055_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1928 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/H5072_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1269 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/H5074_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2134 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/H5102_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2810 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/H5106_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2273 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/HHCCJCY01HHCC_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2128 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/HHCCJCY10_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1238 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/HHCCPOT002_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2271 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/IBS_THBP01B_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3386 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/IBT_2X_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2802 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/IBT_4XS_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3854 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/IBT_6XS_SOLIS6_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1293 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/JHT_F525_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2251 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/JQJCY01YM_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2271 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/KKM_K6P_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3522 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/KKM_K9_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/LYWSD02_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2864 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/LYWSD03MMC_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1767 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/LYWSDCGQ_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3892 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/MBXPRO_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)      785 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/MS_CDP_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/MUE4094RT_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1960 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/Miband_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1942 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/Mokobeacon_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4604 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/Mopeka_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)      819 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/PH10_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     8958 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/RDL52832_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3271 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/RuuviTag_RAWv1_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4454 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/RuuviTag_RAWv2_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1956 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/SBBT_002C_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3798 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/SBCS_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2440 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/SBCU_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3468 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/SBMS_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2189 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/SBMT_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2150 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/SBOT_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1585 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/SBS1_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1794 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/SCD4X_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/SHT4X_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)      779 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/ServiceData_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)      864 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/Skale_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2193 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/SmartDry_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1196 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/T201_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1194 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/T301_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2445 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/TPMS_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1165 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/TPTH_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4690 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/ThermoBeacon_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2129 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/XMTZC04HM_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/XMTZC05HM_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/common_props.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2646 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/iBeacon_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3789 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/iNodeEM_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3173 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices/tracker_json.h
+-rw-r--r--   0 runner    (1001) docker     (122)     6645 2023-06-09 00:04:30.000000 TheengsDecoder-1.5.0/src/devices.h
```

### Comparing `TheengsDecoder-1.4.2/CMakeLists.txt` & `TheengsDecoder-1.5.0/CMakeLists.txt`

 * *Files 5% similar despite different names*

```diff
@@ -20,20 +20,25 @@
     target_compile_features(_decoder PRIVATE cxx_std_11)
     install(TARGETS _decoder LIBRARY DESTINATION TheengsDecoder)
 
 else()
 
     add_library(decoder
                 src/decoder.cpp
+                src/decoder_c.cpp
                 )
 
+    set_target_properties(decoder PROPERTIES
+        PUBLIC_HEADER shared/theengs.h)
+
     target_include_directories(decoder
         PUBLIC
             $<INSTALL_INTERFACE:arduino_json>
             $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/src/arduino_json/src>
+            ${CMAKE_CURRENT_SOURCE_DIR}/include
             ${CMAKE_CURRENT_SOURCE_DIR}/src
     )
 
     target_compile_features(decoder PRIVATE cxx_std_11)
 
     if(CMAKE_PROJECT_NAME STREQUAL PROJECT_NAME)
         include(CTest)
```

### Comparing `TheengsDecoder-1.4.2/LICENSE.txt` & `TheengsDecoder-1.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/PKG-INFO` & `TheengsDecoder-1.5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: TheengsDecoder
-Version: 1.4.2
+Version: 1.5.0
 Summary: A message decoder for the Internet of Things
 Author: Theengs
 License:  GPL-3.0 License
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-Theengs Decoder project aims to provide an efficient, portable and lightweight library for Internet of Things messages decoding.
+Theengs Decoder project aims to provide an efficient, portable and lightweight library for BLE Internet of Things messages decoding.
 
 ![Iot](https://github.com/theengs/decoder/raw/development//docs/img/Theengs_decoder_iot_chain.jpg)
 
 Sensors and devices use chains of data to communicate to gateways, computers, servers. Enabling them to have lightweight and fast communication.
 On the other hand we have a huge diversity of communication methods, resulting in the sensors or devices being closed to one ecosystem or a few.
 
 Theengs decoder library translates these data chains into human readable data leveraging the well known data interchange format JSON. This format can easily be integrated into different systems or software.
@@ -31,9 +31,10 @@
 
 Projects using the Theengs Decoder library
 * [OpenMQTTGateway](https://github.com/1technophile/OpenMQTTGateway) - A BLE to MQTT bridge running on ESP8266, ESP32 or Arduino boards.
 * [Theengs Gateway](https://github.com/theengs/gateway) - A Python-based BLE to MQTT bridge running on Raspberry Pi, Windows or Linux.
 * [Theengs Explorer](https://github.com/theengs/explorer) - A text user interface to discover BLE devices, showing their raw advertisement alongside the decoded data; running on Linux, Windows or macOS.
 * [Theengs App](https://github.com/theengs/app) - A paid app for Android and iOS/iPadOS phones and tablets displaying decoded BLE sensor data and optionally acting as a BLE to MQTT bridge.
 * [BresserWeatherSensorTTN](https://github.com/matthias-bs/BresserWeatherSensorTTN) - Bresser 5-in-1/6-in-1/7-in-1 868 MHz Weather Sensor Radio Receiver based on ESP32 and RFM95W/SX1276 - sends data to a LoRaWAN Network.
+* [Platypush](https://github.com/BlackLight/platypush) - A versatile and extensible platform for home and life automation with hundreds of supported integrations.
 
 For more information view the [documentation](https://decoder.theengs.io/)
```

### Comparing `TheengsDecoder-1.4.2/README.md` & `TheengsDecoder-1.5.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Theengs Decoder project aims to provide an efficient, portable and lightweight library for Internet of Things messages decoding.
+Theengs Decoder project aims to provide an efficient, portable and lightweight library for BLE Internet of Things messages decoding.
 
 ![Iot](https://github.com/theengs/decoder/raw/development//docs/img/Theengs_decoder_iot_chain.jpg)
 
 Sensors and devices use chains of data to communicate to gateways, computers, servers. Enabling them to have lightweight and fast communication.
 On the other hand we have a huge diversity of communication methods, resulting in the sensors or devices being closed to one ecosystem or a few.
 
 Theengs decoder library translates these data chains into human readable data leveraging the well known data interchange format JSON. This format can easily be integrated into different systems or software.
@@ -22,9 +22,10 @@
 
 Projects using the Theengs Decoder library
 * [OpenMQTTGateway](https://github.com/1technophile/OpenMQTTGateway) - A BLE to MQTT bridge running on ESP8266, ESP32 or Arduino boards.
 * [Theengs Gateway](https://github.com/theengs/gateway) - A Python-based BLE to MQTT bridge running on Raspberry Pi, Windows or Linux.
 * [Theengs Explorer](https://github.com/theengs/explorer) - A text user interface to discover BLE devices, showing their raw advertisement alongside the decoded data; running on Linux, Windows or macOS.
 * [Theengs App](https://github.com/theengs/app) - A paid app for Android and iOS/iPadOS phones and tablets displaying decoded BLE sensor data and optionally acting as a BLE to MQTT bridge.
 * [BresserWeatherSensorTTN](https://github.com/matthias-bs/BresserWeatherSensorTTN) - Bresser 5-in-1/6-in-1/7-in-1 868 MHz Weather Sensor Radio Receiver based on ESP32 and RFM95W/SX1276 - sends data to a LoRaWAN Network.
+* [Platypush](https://github.com/BlackLight/platypush) - A versatile and extensible platform for home and life automation with hundreds of supported integrations.
 
 For more information view the [documentation](https://decoder.theengs.io/)
```

### Comparing `TheengsDecoder-1.4.2/TheengsDecoder/_decoder.cpp` & `TheengsDecoder-1.5.0/TheengsDecoder/_decoder.cpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/TheengsDecoder.egg-info/PKG-INFO` & `TheengsDecoder-1.5.0/TheengsDecoder.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: TheengsDecoder
-Version: 1.4.2
+Version: 1.5.0
 Summary: A message decoder for the Internet of Things
 Author: Theengs
 License:  GPL-3.0 License
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-Theengs Decoder project aims to provide an efficient, portable and lightweight library for Internet of Things messages decoding.
+Theengs Decoder project aims to provide an efficient, portable and lightweight library for BLE Internet of Things messages decoding.
 
 ![Iot](https://github.com/theengs/decoder/raw/development//docs/img/Theengs_decoder_iot_chain.jpg)
 
 Sensors and devices use chains of data to communicate to gateways, computers, servers. Enabling them to have lightweight and fast communication.
 On the other hand we have a huge diversity of communication methods, resulting in the sensors or devices being closed to one ecosystem or a few.
 
 Theengs decoder library translates these data chains into human readable data leveraging the well known data interchange format JSON. This format can easily be integrated into different systems or software.
@@ -31,9 +31,10 @@
 
 Projects using the Theengs Decoder library
 * [OpenMQTTGateway](https://github.com/1technophile/OpenMQTTGateway) - A BLE to MQTT bridge running on ESP8266, ESP32 or Arduino boards.
 * [Theengs Gateway](https://github.com/theengs/gateway) - A Python-based BLE to MQTT bridge running on Raspberry Pi, Windows or Linux.
 * [Theengs Explorer](https://github.com/theengs/explorer) - A text user interface to discover BLE devices, showing their raw advertisement alongside the decoded data; running on Linux, Windows or macOS.
 * [Theengs App](https://github.com/theengs/app) - A paid app for Android and iOS/iPadOS phones and tablets displaying decoded BLE sensor data and optionally acting as a BLE to MQTT bridge.
 * [BresserWeatherSensorTTN](https://github.com/matthias-bs/BresserWeatherSensorTTN) - Bresser 5-in-1/6-in-1/7-in-1 868 MHz Weather Sensor Radio Receiver based on ESP32 and RFM95W/SX1276 - sends data to a LoRaWAN Network.
+* [Platypush](https://github.com/BlackLight/platypush) - A versatile and extensible platform for home and life automation with hundreds of supported integrations.
 
 For more information view the [documentation](https://decoder.theengs.io/)
```

### Comparing `TheengsDecoder-1.4.2/TheengsDecoder.egg-info/SOURCES.txt` & `TheengsDecoder-1.5.0/TheengsDecoder.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 TheengsDecoder/_decoder.cpp
 TheengsDecoder.egg-info/PKG-INFO
 TheengsDecoder.egg-info/SOURCES.txt
 TheengsDecoder.egg-info/dependency_links.txt
 TheengsDecoder.egg-info/top_level.txt
 src/decoder.cpp
 src/decoder.h
+src/decoder_c.cpp
 src/devices.h
 src/arduino_json/.clang-format
 src/arduino_json/.git
 src/arduino_json/.gitattributes
 src/arduino_json/.gitignore
 src/arduino_json/.mbedignore
 src/arduino_json/.prettierignore
@@ -201,27 +202,30 @@
 src/devices/HHCCPOT002_json.h
 src/devices/IBS_THBP01B_json.h
 src/devices/IBT_2X_json.h
 src/devices/IBT_4XS_json.h
 src/devices/IBT_6XS_SOLIS6_json.h
 src/devices/JHT_F525_json.h
 src/devices/JQJCY01YM_json.h
+src/devices/KKM_K6P_json.h
+src/devices/KKM_K9_json.h
 src/devices/LYWSD02_json.h
 src/devices/LYWSD03MMC_json.h
 src/devices/LYWSDCGQ_json.h
 src/devices/MBXPRO_json.h
 src/devices/MS_CDP_json.h
 src/devices/MUE4094RT_json.h
 src/devices/Miband_json.h
 src/devices/Mokobeacon_json.h
 src/devices/Mopeka_json.h
 src/devices/PH10_json.h
 src/devices/RDL52832_json.h
 src/devices/RuuviTag_RAWv1_json.h
 src/devices/RuuviTag_RAWv2_json.h
+src/devices/SBBT_002C_json.h
 src/devices/SBCS_json.h
 src/devices/SBCU_json.h
 src/devices/SBMS_json.h
 src/devices/SBMT_json.h
 src/devices/SBOT_json.h
 src/devices/SBS1_json.h
 src/devices/SCD4X_json.h
```

### Comparing `TheengsDecoder-1.4.2/setup.py` & `TheengsDecoder-1.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     if version.parse(get_cmake_version()) < version.parse("3.4"):
         setup_requires.append("cmake")
 except SKBuildError:
     setup_requires.append("cmake")
 
 setup(
     name="TheengsDecoder",
-    version="v1.4.2",
+    version="v1.5.0",
     long_description=long_description,
     long_description_content_type="text/markdown",
     description="A message decoder for the Internet of Things",
     author='Theengs',
     license=" GPL-3.0 License",
     packages=['TheengsDecoder'],
     setup_requires=setup_requires,
```

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/CHANGELOG.md` & `TheengsDecoder-1.5.0/src/arduino_json/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/CMakeLists.txt` & `TheengsDecoder-1.5.0/src/arduino_json/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/LICENSE.md` & `TheengsDecoder-1.5.0/src/arduino_json/LICENSE.md`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/README.md` & `TheengsDecoder-1.5.0/src/arduino_json/README.md`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/SUPPORT.md` & `TheengsDecoder-1.5.0/src/arduino_json/SUPPORT.md`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/appveyor.yml` & `TheengsDecoder-1.5.0/src/arduino_json/appveyor.yml`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/banner.svg` & `TheengsDecoder-1.5.0/src/arduino_json/banner.svg`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/keywords.txt` & `TheengsDecoder-1.5.0/src/arduino_json/keywords.txt`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/library.json` & `TheengsDecoder-1.5.0/src/arduino_json/library.json`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/library.properties` & `TheengsDecoder-1.5.0/src/arduino_json/library.properties`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Array/ArrayFunctions.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Array/ArrayFunctions.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Array/ArrayImpl.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Array/ArrayImpl.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Array/ArrayIterator.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Array/ArrayIterator.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Array/ArrayRef.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Array/ArrayRef.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Array/ArrayShortcuts.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Array/ArrayShortcuts.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Array/ElementProxy.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Array/ElementProxy.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Array/Utilities.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Array/Utilities.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Collection/CollectionData.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Collection/CollectionData.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Collection/CollectionImpl.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Collection/CollectionImpl.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Configuration.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Configuration.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Deserialization/DeserializationError.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/DeserializationError.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Deserialization/Filter.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/Filter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Deserialization/NestingLimit.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/NestingLimit.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Deserialization/Reader.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/Reader.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Deserialization/Readers/ArduinoStreamReader.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/ArduinoStreamReader.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Deserialization/Readers/FlashReader.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/FlashReader.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Deserialization/Readers/IteratorReader.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/IteratorReader.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Deserialization/Readers/RamReader.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/RamReader.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Deserialization/Readers/StdStreamReader.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/StdStreamReader.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Deserialization/Readers/VariantReader.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/Readers/VariantReader.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Deserialization/deserialize.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Deserialization/deserialize.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Document/BasicJsonDocument.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Document/BasicJsonDocument.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Document/DynamicJsonDocument.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Document/DynamicJsonDocument.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Document/JsonDocument.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Document/JsonDocument.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Document/StaticJsonDocument.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Document/StaticJsonDocument.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Json/EscapeSequence.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Json/EscapeSequence.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Json/JsonDeserializer.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Json/JsonDeserializer.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Json/JsonSerializer.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Json/JsonSerializer.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Json/Latch.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Json/Latch.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Json/PrettyJsonSerializer.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Json/PrettyJsonSerializer.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Json/TextFormatter.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Json/TextFormatter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Json/Utf16.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Json/Utf16.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Json/Utf8.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Json/Utf8.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Memory/Alignment.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Memory/Alignment.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Memory/MemoryPool.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Memory/MemoryPool.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Misc/SerializedValue.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Misc/SerializedValue.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/MsgPack/MsgPackDeserializer.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/MsgPack/MsgPackDeserializer.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/MsgPack/MsgPackSerializer.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/MsgPack/MsgPackSerializer.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/MsgPack/endianess.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/MsgPack/endianess.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Namespace.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Namespace.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Numbers/FloatParts.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Numbers/FloatParts.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Numbers/FloatTraits.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Numbers/FloatTraits.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Numbers/Integer.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Numbers/Integer.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Numbers/arithmeticCompare.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Numbers/arithmeticCompare.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Numbers/convertNumber.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Numbers/convertNumber.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Numbers/parseNumber.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Numbers/parseNumber.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Object/MemberProxy.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Object/MemberProxy.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Object/ObjectFunctions.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Object/ObjectFunctions.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Object/ObjectImpl.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Object/ObjectImpl.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Object/ObjectIterator.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Object/ObjectIterator.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Object/ObjectRef.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Object/ObjectRef.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Object/ObjectShortcuts.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Object/ObjectShortcuts.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Object/Pair.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Object/Pair.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/alias_cast.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/alias_cast.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/attributes.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/attributes.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/limits.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/limits.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/mpl/max.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/mpl/max.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/pgmspace.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/pgmspace.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/pgmspace_generic.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/pgmspace_generic.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/preprocessor.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/preprocessor.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/safe_strcmp.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/safe_strcmp.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/static_array.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/static_array.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_base_of.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_base_of.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_class.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_class.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_convertible.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_convertible.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_enum.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_enum.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_integral.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_integral.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_signed.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_signed.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_unsigned.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/is_unsigned.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/make_unsigned.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits/make_unsigned.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/type_traits.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/type_traits.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Polyfills/utility.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Polyfills/utility.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Serialization/CountingDecorator.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Serialization/CountingDecorator.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Serialization/Writer.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Serialization/Writer.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Serialization/Writers/ArduinoStringWriter.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Serialization/Writers/ArduinoStringWriter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Serialization/Writers/PrintWriter.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Serialization/Writers/PrintWriter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Serialization/Writers/StaticStringWriter.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Serialization/Writers/StaticStringWriter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Serialization/Writers/StdStreamWriter.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Serialization/Writers/StdStreamWriter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Serialization/Writers/StdStringWriter.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Serialization/Writers/StdStringWriter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Serialization/serialize.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Serialization/serialize.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/StringStorage/StringCopier.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/StringStorage/StringCopier.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/StringStorage/StringMover.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/StringStorage/StringMover.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/StringStorage/StringStorage.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/StringStorage/StringStorage.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Strings/Adapters/ArduinoStringAdapter.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/ArduinoStringAdapter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Strings/Adapters/ConstRamStringAdapter.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/ConstRamStringAdapter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Strings/Adapters/FlashStringAdapter.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/FlashStringAdapter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Strings/Adapters/JsonStringAdapter.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/JsonStringAdapter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Strings/Adapters/RamStringAdapter.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/RamStringAdapter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Strings/Adapters/SizedFlashStringAdapter.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/SizedFlashStringAdapter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Strings/Adapters/SizedRamStringAdapter.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/SizedRamStringAdapter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Strings/Adapters/StdStringAdapter.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/StdStringAdapter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Strings/Adapters/StringViewAdapter.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/Adapters/StringViewAdapter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Strings/IsWriteableString.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/IsWriteableString.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Strings/String.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/String.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Strings/StringAdapter.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/StringAdapter.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Strings/StringAdapters.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Strings/StringAdapters.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Variant/ConverterImpl.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/ConverterImpl.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Variant/SlotFunctions.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/SlotFunctions.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Variant/VariantCompare.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/VariantCompare.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Variant/VariantContent.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/VariantContent.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Variant/VariantData.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/VariantData.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Variant/VariantFunctions.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/VariantFunctions.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Variant/VariantImpl.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/VariantImpl.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Variant/VariantOperators.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/VariantOperators.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Variant/VariantRef.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/VariantRef.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Variant/VariantShortcuts.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/VariantShortcuts.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Variant/VariantSlot.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/VariantSlot.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Variant/VariantTo.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/VariantTo.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/Variant/Visitor.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/Variant/Visitor.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson/compatibility.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson/compatibility.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/ArduinoJson.hpp` & `TheengsDecoder-1.5.0/src/arduino_json/src/ArduinoJson.hpp`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/arduino_json/src/CMakeLists.txt` & `TheengsDecoder-1.5.0/src/arduino_json/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/decoder.cpp` & `TheengsDecoder-1.5.0/src/decoder.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -560,14 +560,17 @@
             break;
           case 15:
             doc["type"] = "AIR"; // air environmental monitoring devices
             break;
           case 16:
             doc["type"] = "TRACK"; // Bluetooth tracker
             break;
+          case 17:
+            doc["type"] = "BTN"; // Button
+            break;
           case 254:
             doc["type"] = "RMAC"; // random MAC address devices
             break;
           case 255:
             doc["type"] = "UNIQ"; // unique devices
             break;
         }
```

### Comparing `TheengsDecoder-1.4.2/src/decoder.h` & `TheengsDecoder-1.5.0/src/decoder.h`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,16 @@
     IBT_2XS,
     IBT4XS,
     IBT6XS_SOLIS,
     MIBAND,
     XMTZC04HM,
     XMTZC05HM,
     TPMS,
+    KKM_K6P,
+    KKM_K9,
     LYWSD03MMC_ATC,
     LYWSD03MMC_PVVX,
     CGPR1,
     THERMOBEACON,
     H5055,
     H5072,
     H5074,
@@ -121,14 +123,15 @@
     TILE,
     TILEN,
     JHT_F525,
     IBEACON,
     APPLE_CONT,
     APPLE_CONTAT,
     SERVICE_DATA,
+    SBBT_002C,
     BLE_ID_MAX
   };
 
 private:
   void        reverse_hex_data(const char* in, char* out, int l);
   double      value_from_hex_string(const char* data_str, int offset, int data_length, bool reverse, bool canBeNegative = true, bool isFloat = false);
   double      bf_value_from_hex_string(const char* data_str, int offset, int data_length, bool reverse, bool canBeNegative = true, bool isFloat = false);
```

### Comparing `TheengsDecoder-1.4.2/src/devices/ABN03_json.h` & `TheengsDecoder-1.5.0/src/devices/ABN03_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/ABTemp_json.h` & `TheengsDecoder-1.5.0/src/devices/ABTemp_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/APPLE_json.h` & `TheengsDecoder-1.5.0/src/devices/APPLE_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/Amphiro_json.h` & `TheengsDecoder-1.5.0/src/devices/Amphiro_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/BC08_json.h` & `TheengsDecoder-1.5.0/src/devices/BC08_json.h`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,23 @@
-const char* _BC08_json = "{\"brand\":\"BlueCharm\",\"model\":\"Beacon 08/04P/021\",\"model_id\":\"KSensor\",\"tag\":\"0708\",\"condition\":[\"servicedata\",\"=\",26,\"&\",\"uuid\",\"index\",0,\"feaa\"],\"properties\":{\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",10,4,false,true],\"post_proc\":[\"/\",253]},\"accx\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",14,4,false,true]},\"accy\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",18,4,false,true]},\"accz\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",22,4,false,true]},\"volt\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",6,4,false,false],\"post_proc\":[\"/\",1000]}}}";
+const char* _BC08_json = "{\"brand\":\"BlueCharm\",\"model\":\"Beacon 08/04P/021\",\"model_id\":\"KSensor\",\"tag\":\"0708\",\"condition\":[\"servicedata\",\"=\",26,\"index\",0,\"21010b\",\"&\",\"uuid\",\"index\",0,\"feaa\"],\"properties\":{\".cal\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",12,2,false,false],\"post_proc\":[\"/\",256,\"*\",100,\">\",0,\"/\",100]},\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",10,2,false,true],\"post_proc\":[\"+\",\".cal\"]},\"accx\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",14,4,false,true]},\"accy\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",18,4,false,true]},\"accz\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",22,4,false,true]},\"volt\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",6,4,false,false],\"post_proc\":[\"/\",1000]}}}";
 /*R""""(
 {
    "brand":"BlueCharm",
    "model":"Beacon 08/04P/021",
    "model_id":"KSensor",
    "tag":"0708",
-   "condition":["servicedata", "=", 26, "&", "uuid", "index", 0, "feaa"],
+   "condition":["servicedata", "=", 26, "index", 0, "21010b", "&", "uuid", "index", 0, "feaa"],
    "properties":{
+      ".cal":{
+         "decoder":["value_from_hex_data", "servicedata", 12, 2, false, false],
+         "post_proc":["/", 256, "*", 100, ">", 0, "/", 100]
+      },
       "tempc":{
-         "decoder":["value_from_hex_data", "servicedata", 10, 4, false, true],
-         "post_proc":["/", 253]
+         "decoder":["value_from_hex_data", "servicedata", 10, 2, false, true],
+         "post_proc":["+", ".cal"]
       },
       "accx":{
          "decoder":["value_from_hex_data", "servicedata", 14, 4, false, true]
       },
       "accy":{
          "decoder":["value_from_hex_data", "servicedata", 18, 4, false, true]
       },
```

### Comparing `TheengsDecoder-1.4.2/src/devices/BM1IN1_json.h` & `TheengsDecoder-1.5.0/src/devices/BM1IN1_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/BM2_json.h` & `TheengsDecoder-1.5.0/src/devices/BM2_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/BM3IN1_json.h` & `TheengsDecoder-1.5.0/src/devices/BM3IN1_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/BM4IN1_json.h` & `TheengsDecoder-1.5.0/src/devices/BM4IN1_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/BPARASITE_json.h` & `TheengsDecoder-1.5.0/src/devices/BPARASITE_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/BWBSDOO_json.h` & `TheengsDecoder-1.5.0/src/devices/BWBSDOO_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/CGD1_json.h` & `TheengsDecoder-1.5.0/src/devices/CGD1_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/CGDK2_json.h` & `TheengsDecoder-1.5.0/src/devices/CGDK2_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/CGDN1_json.h` & `TheengsDecoder-1.5.0/src/devices/CGDN1_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/CGG1_json.h` & `TheengsDecoder-1.5.0/src/devices/CGG1_json.h`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,14 @@
    "brand":"ClearGrass/Qingping",
    "model":"Round TH",
    "model_id":"CGG1",
    "tag":"0102",
    "condition":["servicedata", "=", 30, "|", "servicedata", "=", 32, "|", "servicedata", "=", 36, "&", "name", "index", 0, "Qingping Temp & RH", "|", "name", "index", 0, "ClearGrass Temp & RH", "&","uuid", "index", 0, "fe95"],
    "properties":{
       "tempc":{
-         // "condition":["servicedata", "=", 32, "|", "servicedata", "=", 36, "&", "servicedata", 23, "!", "6"], // not working!!
          "condition":["servicedata", ">=", 32, "&", "servicedata", 23, "!", "6"],
          "decoder":["value_from_hex_data", "servicedata", 28, 4, true],
          "post_proc":["/", 10]
       },
       "hum":{
          "condition":["servicedata", "=", 36, "&", "servicedata", 23, "!", "6"],
          "decoder":["value_from_hex_data", "servicedata", 32, 4, true],
```

### Comparing `TheengsDecoder-1.4.2/src/devices/CGH1_json.h` & `TheengsDecoder-1.5.0/src/devices/CGH1_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/CGP1W_json.h` & `TheengsDecoder-1.5.0/src/devices/CGP1W_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/CGPR1_json.h` & `TheengsDecoder-1.5.0/src/devices/CGPR1_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/GAEN_json.h` & `TheengsDecoder-1.5.0/src/devices/GAEN_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/H5055_json.h` & `TheengsDecoder-1.5.0/src/devices/H5055_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/H5072_json.h` & `TheengsDecoder-1.5.0/src/devices/H5072_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/H5074_json.h` & `TheengsDecoder-1.5.0/src/devices/H5074_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/H5102_json.h` & `TheengsDecoder-1.5.0/src/devices/H5102_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/H5106_json.h` & `TheengsDecoder-1.5.0/src/devices/H5106_json.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-const char* _H5106_json = "{\"brand\":\"Govee\",\"model\":\"Smart Air Quality Monitor\",\"model_id\":\"H5106\",\"tag\":\"0f03\",\"condition\":[\"name\",\"index\",0,\"GVH5106\",\"&\",\"manufacturerdata\",\">=\",16,\"index\",0,\"0100\"],\"properties\":{\"tempc\":{\"condition\":[\"manufacturerdata\",8,\"bit\",3,0],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",8,8,false,false],\"post_proc\":[\"/\",1000000,\">\",0,\"/\",10]},\"_tempc\":{\"condition\":[\"manufacturerdata\",8,\"bit\",3,1],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",8,8,false,false],\"post_proc\":[\"&\",2147483647,\"/\",1000000,\">\",0,\"/\",10,\"*\",-1]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",8,8,false,false],\"post_proc\":[\"&\",2147483647,\"%\",1000000,\"/\",10000,\">\",0]},\".cal\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",8,8,false,false],\"post_proc\":[\"&\",2147483647,\"/\",1000,\">\",0,\"*\",1000]},\"pm25\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",8,8,false,false],\"post_proc\":[\"&\",2147483647,\"-\",\".cal\"]}}}";
+const char* _H5106_json = "{\"brand\":\"Govee\",\"model\":\"Smart Air Quality Monitor\",\"model_id\":\"H5106\",\"tag\":\"0f03\",\"condition\":[\"name\",\"index\",0,\"GVH5106\",\"&\",\"manufacturerdata\",\">=\",16,\"index\",0,\"0100\"],\"properties\":{\"tempc\":{\"condition\":[\"manufacturerdata\",8,\"bit\",3,0],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",8,8,false,false],\"post_proc\":[\"/\",1000000,\">\",0,\"/\",10]},\"_tempc\":{\"condition\":[\"manufacturerdata\",8,\"bit\",3,1],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",8,8,false,false],\"post_proc\":[\"&\",2147483647,\"/\",1000000,\">\",0,\"/\",10,\"*\",-1]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",8,8,false,false],\"post_proc\":[\"&\",2147483647,\"%\",1000000,\"/\",1000,\">\",0,\"/\",10]},\".cal\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",8,8,false,false],\"post_proc\":[\"&\",2147483647,\"/\",1000,\">\",0,\"*\",1000]},\"pm25\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",8,8,false,false],\"post_proc\":[\"&\",2147483647,\"-\",\".cal\"]}}}";
 /* R""""(
 {
    "brand":"Govee",
    "model":"Smart Air Quality Monitor",
    "model_id":"H5106",
    "tag":"0f03",
    "condition":["name", "index", 0, "GVH5106", "&", "manufacturerdata", ">=", 16, "index", 0, "0100"],
@@ -15,15 +15,15 @@
       "_tempc":{
          "condition":["manufacturerdata", 8, "bit", 3, 1],
          "decoder":["value_from_hex_data", "manufacturerdata", 8, 8, false, false],
          "post_proc":["&", 2147483647, "/", 1000000, ">", 0, "/", 10, "*", -1]
       },
       "hum":{
          "decoder":["value_from_hex_data", "manufacturerdata", 8, 8, false, false],
-         "post_proc":["&", 2147483647, "%", 1000000, "/", 10000, ">", 0]
+         "post_proc":["&", 2147483647, "%", 1000000, "/", 1000, ">", 0, "/", 10]
       },
       ".cal":{
          "decoder":["value_from_hex_data", "manufacturerdata", 8, 8, false, false],
          "post_proc":["&", 2147483647, "/", 1000, ">", 0, "*", 1000]
       },
       "pm25":{
          "decoder":["value_from_hex_data", "manufacturerdata", 8, 8, false, false],
```

### Comparing `TheengsDecoder-1.4.2/src/devices/HHCCJCY01HHCC_json.h` & `TheengsDecoder-1.5.0/src/devices/HHCCJCY01HHCC_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/HHCCJCY10_json.h` & `TheengsDecoder-1.5.0/src/devices/HHCCJCY10_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/HHCCPOT002_json.h` & `TheengsDecoder-1.5.0/src/devices/HHCCPOT002_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/IBS_THBP01B_json.h` & `TheengsDecoder-1.5.0/src/devices/IBS_THBP01B_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/IBT_2X_json.h` & `TheengsDecoder-1.5.0/src/devices/IBT_2X_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/IBT_4XS_json.h` & `TheengsDecoder-1.5.0/src/devices/IBT_4XS_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/IBT_6XS_SOLIS6_json.h` & `TheengsDecoder-1.5.0/src/devices/IBT_6XS_SOLIS6_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/JHT_F525_json.h` & `TheengsDecoder-1.5.0/src/devices/JHT_F525_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/JQJCY01YM_json.h` & `TheengsDecoder-1.5.0/src/devices/JQJCY01YM_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/LYWSD02_json.h` & `TheengsDecoder-1.5.0/src/devices/LYWSD02_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/LYWSD03MMC_json.h` & `TheengsDecoder-1.5.0/src/devices/LYWSD03MMC_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/LYWSDCGQ_json.h` & `TheengsDecoder-1.5.0/src/devices/LYWSDCGQ_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/MBXPRO_json.h` & `TheengsDecoder-1.5.0/src/devices/MBXPRO_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/MS_CDP_json.h` & `TheengsDecoder-1.5.0/src/devices/TPMS_json.h`

 * *Files 24% similar despite different names*

```diff
@@ -1,73 +1,57 @@
-const char* _MS_CDP_json = "{\"brand\":\"GENERIC\",\"model\":\"MS-CDP\",\"model_id\":\"MS-CDP\",\"tag\":\"fe\",\"condition\":[\"manufacturerdata\",\"index\",0,\"060001\"],\"properties\":{\"device\":{\"condition\":[\"manufacturerdata\",7,\"1\"],\"decoder\":[\"static_value\",\"Xbox One\"]},\"_device\":{\"condition\":[\"manufacturerdata\",7,\"6\"],\"decoder\":[\"static_value\",\"Apple iPhone\"]},\"__device\":{\"condition\":[\"manufacturerdata\",7,\"7\"],\"decoder\":[\"static_value\",\"Apple iPad\"]},\"___device\":{\"condition\":[\"manufacturerdata\",7,\"8\"],\"decoder\":[\"static_value\",\"Android device\"]},\"____device\":{\"condition\":[\"manufacturerdata\",7,\"9\"],\"decoder\":[\"static_value\",\"Windows 10 Desktop\"]},\"_____device\":{\"condition\":[\"manufacturerdata\",7,\"11\"],\"decoder\":[\"static_value\",\"Windows 10 Phone\"]},\"______device\":{\"condition\":[\"manufacturerdata\",7,\"12\"],\"decoder\":[\"static_value\",\"Linux device\"]},\"_______device\":{\"condition\":[\"manufacturerdata\",7,\"17\"],\"decoder\":[\"static_value\",\"Windows IoT\"]},\"________device\":{\"condition\":[\"manufacturerdata\",7,\"14\"],\"decoder\":[\"static_value\",\"Surface Hub\"]},\"salt\":{\"decoder\":[\"string_from_hex_data\",\"manufacturerdata\",12,8]},\"hash\":{\"decoder\":[\"string_from_hex_data\",\"manufacturerdata\",20,32]}}}}";
+const char* _TPMS_json = "{\"brand\":\"GENERIC\",\"model\":\"TPMS\",\"model_id\":\"TPMS\",\"tag\":\"0a01\",\"condition\":[\"manufacturerdata\",\"=\",36,\"index\",0,\"000\",\"&\",\"manufacturerdata\",\"mac@index\",4],\"conditionnomac\":[\"manufacturerdata\",\"=\",36,\"&\",\"name\",\"index\",0,\"TPMS\"],\"properties\":{\"count\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",5,1,false],\"post_proc\":[\"+\",1]},\"pres\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",16,8,true],\"post_proc\":[\"/\",100000]},\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",24,8,true],\"post_proc\":[\"/\",100]},\"batt\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",32,2,true]},\"alarm\":{\"decoder\":[\"bit_static_value\",\"manufacturerdata\",35,0,false,true]}}}";
 /*R""""(
 {
    "brand":"GENERIC",
-   "model":"MS-CDP",
-   "model_id":"MS-CDP",
-   "tag":"fe",
-   "condition":["manufacturerdata", "index", 0, "060001"],
+   "model":"TPMS",
+   "model_id":"TPMS",
+   "tag":"0a01",
+   "condition":["manufacturerdata", "=", 36, "index", 0, "000", "&", "manufacturerdata", "mac@index", 4],
+   "conditionnomac":["manufacturerdata", "=", 36, "&", "name", "index", 0, "TPMS"],
    "properties":{
-      "device":{
-         "condition":["manufacturerdata", 7, "1"],
-         "decoder":["static_value", "Xbox One"]
-      },
-      "_device":{
-         "condition":["manufacturerdata", 7, "6"],
-         "decoder":["static_value", "Apple iPhone"]
-      },
-      "__device":{
-         "condition":["manufacturerdata", 7, "7"],
-         "decoder":["static_value", "Apple iPad"]
-      },
-      "___device":{
-         "condition":["manufacturerdata", 7, "8"],
-         "decoder":["static_value", "Android device"]
-      },
-      "____device":{
-         "condition":["manufacturerdata", 7, "9"],
-         "decoder":["static_value", "Windows 10 Desktop"]
-      },
-      "_____device":{
-         "condition":["manufacturerdata", 7, "11"],
-         "decoder":["static_value", "Windows 10 Phone"]
-      },
-      "______device":{
-         "condition":["manufacturerdata", 7, "12"],
-         "decoder":["static_value", "Linux device"]
-      },
-      "_______device":{
-         "condition":["manufacturerdata", 7, "13"],
-         "decoder":["static_value", "Windows IoT"]
-      },
-      "________device":{
-         "condition":["manufacturerdata", 7, "14"],
-         "decoder":["static_value", "Surface Hub"]
+      "count":{
+         "decoder":["value_from_hex_data", "manufacturerdata", 5, 1, false],
+         "post_proc":["+", 1]
+      },
+      "pres":{
+         "decoder":["value_from_hex_data", "manufacturerdata", 16, 8, true],
+         "post_proc":["/", 100000]
+      },
+      "tempc":{
+         "decoder":["value_from_hex_data", "manufacturerdata", 24, 8, true],
+         "post_proc":["/", 100]
       },
-      "salt":{
-         "decoder":["string_from_hex_data", "manufacturerdata", 12, 8]
+      "batt":{
+         "decoder":["value_from_hex_data", "manufacturerdata", 32, 2, true]
       },
-      "hash":{
-         "decoder":["string_from_hex_data", "manufacturerdata", 20, 32]
+      "alarm":{
+         "decoder":["bit_static_value", "manufacturerdata", 35, 0, false, true]
       }
    }
 })"""";*/
 
-const char* _MS_CDP_json_props = "{\"properties\":{\"device\":{\"unit\":\"string\",\"name\":\"device type\"},\"salt\":{\"unit\":\"hex\",\"name\":\"salt\"},\"hash\":{\"unit\":\"hex\",\"name\":\"device hash\"}}}";
+const char* _TPMS_json_props = "{\"properties\":{\"batt\":{\"unit\":\"%\",\"name\":\"battery\"},\"tempc\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"pres\":{\"unit\":\"bar\",\"name\":\"pressure\"},\"count\":{\"unit\":\"int\",\"name\":\"count\"},\"alarm\":{\"unit\":\"status\",\"name\":\"alarm\"}}}";
 /*R""""(
 {
    "properties":{
-      "device":{
-         "unit":"string",
-         "name":"device type"
-      },
-      "salt":{
-         "unit":"hex",
-         "name":"salt"
-      },
-      "hash":{
-         "unit":"hex",
-         "name":"device hash"
+      "batt":{
+         "unit":"%",
+         "name":"battery"
+      },
+      "tempc":{
+         "unit":"°C",
+         "name":"temperature"
+      },
+      "pres":{
+         "unit":"bar",
+         "name":"pressure"
+      },
+      "count":{
+         "unit":"int",
+         "name":"count"
+      },
+      "alarm":{
+         "unit":"status",
+         "name":"alarm"
       }
-
    }
 })"""";*/
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `TheengsDecoder-1.4.2/src/devices/MUE4094RT_json.h` & `TheengsDecoder-1.5.0/src/devices/MUE4094RT_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/Miband_json.h` & `TheengsDecoder-1.5.0/src/devices/Miband_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/Mokobeacon_json.h` & `TheengsDecoder-1.5.0/src/devices/Mokobeacon_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/Mopeka_json.h` & `TheengsDecoder-1.5.0/src/devices/Mopeka_json.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,20 @@
-const char* _Mopeka_json = "{\"brand\":\"Mopeka\",\"model\":\"Pro Check Sensor\",\"model_id\":\"M1017\",\"tag\":\"ff01\",\"condition\":[\"manufacturerdata\",\"=\",24,\"index\",0,\"590003\"],\"properties\":{\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",8,2,false,true],\"post_proc\":[\"&\",127,\"-\",40,\"min\",-40]},\".cal\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",8,2,false,true],\"post_proc\":[\"&\",127]},\"_.cal\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",8,2,false,true],\"post_proc\":[\"&\",127,\"*\",\".cal\",\"*\",-0.00000535]},\"__.cal\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",8,2,false,true],\"post_proc\":[\"&\",127,\"*\",-0.002822,\"+\",0.573045,\"+\",\".cal\"]},\"lvl_cm\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",10,4,true,false],\"post_proc\":[\"&\",16383,\"*\",\".cal\",\"/\",10]},\"sync\":{\"decoder\":[\"bit_static_value\",\"manufacturerdata\",8,3,false,true]},\"volt\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",6,2,false,false],\"post_proc\":[\"&\",127,\"/\",32]},\"batt\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",6,2,false,false],\"post_proc\":[\"&\",127,\"/\",32,\"-\",2.2,\"/\",0.65,\"*\",100,\"max\",100,\"min\",0]},\"quality\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",12,2,false,false],\"post_proc\":[\">\",6,\"max\",3,\"min\",0]}}}";
+const char* _Mopeka_json = "{\"brand\":\"Mopeka\",\"model\":\"Pro Check Sensor\",\"model_id\":\"M1017\",\"tag\":\"ff01\",\"condition\":[\"manufacturerdata\",\"=\",24,\"index\",0,\"590003\"],\"properties\":{\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",8,2,false,true],\"post_proc\":[\"&\",127,\"-\",40,\"min\",-40]},\".cal\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",8,2,false,true],\"post_proc\":[\"&\",127]},\"_.cal\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",8,2,false,true],\"post_proc\":[\"&\",127,\"*\",\".cal\",\"*\",-0.00000535]},\"__.cal\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",8,2,false,true],\"post_proc\":[\"&\",127,\"*\",-0.002822,\"+\",0.573045,\"+\",\".cal\"]},\"lvl_cm\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",10,4,true,false],\"post_proc\":[\"&\",16383,\"*\",\".cal\",\"/\",10]},\"sync\":{\"decoder\":[\"bit_static_value\",\"manufacturerdata\",8,3,false,true]},\"volt\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",6,2,false,false],\"post_proc\":[\"&\",127,\"/\",32]},\"batt\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",6,2,false,false],\"post_proc\":[\"&\",127,\"/\",32,\"-\",2.2,\"/\",0.65,\"*\",100,\"max\",100,\"min\",0]},\"quality\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",12,2,false,false],\"post_proc\":[\">\",6,\"max\",3,\"min\",0]},\"accx\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",20,2,false,true]},\"accy\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",22,2,false,true]}}}";
 /* R""""(
 {
    "brand":"Mopeka",
    "model":"Pro Check Sensor",
    "model_id":"M1017",
    "tag":"ff01",
    "condition":["manufacturerdata", "=", 24, "index", 0, "590003"],
    "properties":{
-      // "tempraw":{
-      //    "decoder":["value_from_hex_data", "manufacturerdata", 8, 2, false, true],
-      //    "post_proc":["&", 127]
-      // },
       "tempc":{
          "decoder":["value_from_hex_data", "manufacturerdata", 8, 2, false, true],
          "post_proc":["&", 127, "-", 40, "min", -40]
       },
-      // "levl":{
-      //    "decoder":["value_from_hex_data", "manufacturerdata", 10, 4, true, false],
-      //    "post_proc":["&", 16383]
-      // },
       ".cal":{
          "decoder":["value_from_hex_data", "manufacturerdata", 8, 2, false, true],
          "post_proc":["&", 127]
       },
       "_.cal":{
          "decoder":["value_from_hex_data", "manufacturerdata", 8, 2, false, true],
          "post_proc":["&", 127, "*", ".cal", "*", -0.00000535]
@@ -45,34 +37,32 @@
       "batt":{
          "decoder":["value_from_hex_data", "manufacturerdata", 6, 2, false, false],
          "post_proc":["&", 127, "/", 32, "-", 2.2, "/", 0.65, "*", 100, "max", 100, "min", 0]
       },
       "quality":{
          "decoder":["value_from_hex_data", "manufacturerdata", 12, 2, false, false],
          "post_proc":[">", 6, "max", 3, "min", 0]
+      },
+      "accx":{
+         "decoder":["value_from_hex_data", "manufacturerdata", 20, 2, false, true]
+      },
+      "accy":{
+         "decoder":["value_from_hex_data", "manufacturerdata", 22, 2, false, true]
       }
    }
 })"""";*/
 
-const char* _Mopeka_json_props = "{\"properties\":{\"tempc\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"lvl_cm\":{\"unit\":\"cm\",\"name\":\"level in cm\"},\"sync\":{\"unit\":\"status\",\"name\":\"sync pressed\"},\"volt\":{\"unit\":\"V\",\"name\":\"voltage\"},\"batt\":{\"unit\":\"%\",\"name\":\"battery\"},\"quality\":{\"unit\":\"status\",\"name\":\"reading quality\"}}}";
+const char* _Mopeka_json_props = "{\"properties\":{\"tempc\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"lvl_cm\":{\"unit\":\"cm\",\"name\":\"level in cm\"},\"sync\":{\"unit\":\"status\",\"name\":\"sync pressed\"},\"volt\":{\"unit\":\"V\",\"name\":\"voltage\"},\"batt\":{\"unit\":\"%\",\"name\":\"battery\"},\"quality\":{\"unit\":\"status\",\"name\":\"reading quality\"},\"accx\":{\"unit\":\"m/s²\",\"name\":\"acceleration x\"},\"accy\":{\"unit\":\"m/s²\",\"name\":\"acceleration y\"}}}";
 /*R""""(
 {
    "properties":{
-      // "tempraw":{
-      //    "unit":"°C",
-      //    "name":"temperature"
-      // },
       "tempc":{
          "unit":"°C",
          "name":"temperature"
       },
-      // "levl":{
-      //    "unit":"int",
-      //    "name":"raw level"
-      // },
       "lvl_cm":{
          "unit":"cm",
          "name":"level in cm"
       },
       "sync":{
          "unit":"status",
          "name":"sync pressed"
@@ -84,10 +74,18 @@
       "batt":{
          "unit":"%",
          "name":"battery"
       },
       "quality":{
          "unit":"status",
          "name":"reading quality"
+      },
+      "accx":{
+         "unit":"m/s²",
+         "name":"acceleration x"
+      },
+      "accy":{
+         "unit":"m/s²",
+         "name":"acceleration y"
       }
    }
 })"""";*/
```

### Comparing `TheengsDecoder-1.4.2/src/devices/PH10_json.h` & `TheengsDecoder-1.5.0/src/devices/PH10_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/RDL52832_json.h` & `TheengsDecoder-1.5.0/src/devices/RDL52832_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/RuuviTag_RAWv1_json.h` & `TheengsDecoder-1.5.0/src/devices/RuuviTag_RAWv1_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/RuuviTag_RAWv2_json.h` & `TheengsDecoder-1.5.0/src/devices/RuuviTag_RAWv2_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/SBCS_json.h` & `TheengsDecoder-1.5.0/src/devices/SBCS_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/SBCU_json.h` & `TheengsDecoder-1.5.0/src/devices/SBCU_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/SBMS_json.h` & `TheengsDecoder-1.5.0/src/devices/SBMS_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/SBMT_json.h` & `TheengsDecoder-1.5.0/src/devices/SBMT_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/SBOT_json.h` & `TheengsDecoder-1.5.0/src/devices/SBOT_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/SBS1_json.h` & `TheengsDecoder-1.5.0/src/devices/SBS1_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/SCD4X_json.h` & `TheengsDecoder-1.5.0/src/devices/SCD4X_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/SHT4X_json.h` & `TheengsDecoder-1.5.0/src/devices/SHT4X_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/ServiceData_json.h` & `TheengsDecoder-1.5.0/src/devices/ServiceData_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/Skale_json.h` & `TheengsDecoder-1.5.0/src/devices/Skale_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/SmartDry_json.h` & `TheengsDecoder-1.5.0/src/devices/SmartDry_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/T201_json.h` & `TheengsDecoder-1.5.0/src/devices/T201_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/T301_json.h` & `TheengsDecoder-1.5.0/src/devices/T301_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/TPMS_json.h` & `TheengsDecoder-1.5.0/src/devices/iBeacon_json.h`

 * *Files 15% similar despite different names*

```diff
@@ -1,57 +1,64 @@
-const char* _TPMS_json = "{\"brand\":\"GENERIC\",\"model\":\"TPMS\",\"model_id\":\"TPMS\",\"tag\":\"0a01\",\"condition\":[\"manufacturerdata\",\"=\",36,\"index\",0,\"000\",\"&\",\"manufacturerdata\",\"mac@index\",4],\"conditionnomac\":[\"manufacturerdata\",\"=\",36,\"&\",\"name\",\"index\",0,\"TPMS\"],\"properties\":{\"count\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",5,1,false],\"post_proc\":[\"+\",1]},\"pres\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",16,8,true],\"post_proc\":[\"/\",100000]},\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",24,8,true],\"post_proc\":[\"/\",100]},\"batt\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",32,2,true]},\"alarm\":{\"decoder\":[\"bit_static_value\",\"manufacturerdata\",35,0,false,true]}}}";
+const char* _ibeacon_json = "{\"brand\":\"GENERIC\",\"model\":\"iBeacon\",\"model_id\":\"IBEACON\",\"tag\":\"06\",\"condition\":[\"manufacturerdata\",\"=\",50,\"index\",0,\"4c00\"],\"properties\":{\"mfid\":{\"decoder\":[\"string_from_hex_data\",\"manufacturerdata\",0,4]},\"uuid\":{\"decoder\":[\"string_from_hex_data\",\"manufacturerdata\",8,32]},\"major\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",40,4,false]},\"minor\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",44,4,false]},\"txpower\":{\"condition\":[\"manufacturerdata\",48,\"bit\",3,1],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",48,2,false]},\"volt\":{\"condition\":[\"manufacturerdata\",48,\"bit\",3,0],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",48,2,false],\"post_proc\":[\"/\",10]}}}";
+
 /*R""""(
 {
    "brand":"GENERIC",
-   "model":"TPMS",
-   "model_id":"TPMS",
-   "tag":"0a01",
-   "condition":["manufacturerdata", "=", 36, "index", 0, "000", "&", "manufacturerdata", "mac@index", 4],
-   "conditionnomac":["manufacturerdata", "=", 36, "&", "name", "index", 0, "TPMS"],
+   "model":"iBeacon",
+   "model_id":"IBEACON",
+   "tag":"06",
+   "condition":["manufacturerdata", "=", 50, "index", 0, "4c00"],
    "properties":{
-      "count":{
-         "decoder":["value_from_hex_data", "manufacturerdata", 5, 1, false],
-         "post_proc":["+", 1]
-      },
-      "pres":{
-         "decoder":["value_from_hex_data", "manufacturerdata", 16, 8, true],
-         "post_proc":["/", 100000]
-      },
-      "tempc":{
-         "decoder":["value_from_hex_data", "manufacturerdata", 24, 8, true],
-         "post_proc":["/", 100]
+      "mfid":{
+         "decoder":["string_from_hex_data", "manufacturerdata", 0, 4]
+      },
+      "uuid":{
+         "decoder":["string_from_hex_data", "manufacturerdata", 8, 32]
       },
-      "batt":{
-         "decoder":["value_from_hex_data", "manufacturerdata", 32, 2, true]
+      "major":{
+         "decoder":["value_from_hex_data", "manufacturerdata", 40, 4, false]
       },
-      "alarm":{
-         "decoder":["bit_static_value", "manufacturerdata", 35, 0, false, true]
+      "minor":{
+         "decoder":["value_from_hex_data", "manufacturerdata", 44, 4, false]
+      },
+      "txpower":{
+         "condition":["manufacturerdata", 48, "bit", 3, 1],
+         "decoder":["value_from_hex_data","manufacturerdata", 48, 2, false]
+      },
+      "volt":{
+         "condition":["manufacturerdata", 48, "bit", 3, 0],
+         "decoder":["value_from_hex_data","manufacturerdata", 48, 2, false],
+         "post_proc":["/", 10]
       }
    }
 })"""";*/
 
-const char* _TPMS_json_props = "{\"properties\":{\"batt\":{\"unit\":\"%\",\"name\":\"battery\"},\"tempc\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"pres\":{\"unit\":\"bar\",\"name\":\"pressure\"},\"count\":{\"unit\":\"int\",\"name\":\"count\"},\"alarm\":{\"unit\":\"status\",\"name\":\"alarm\"}}}";
+const char* _ibeacon_json_props = "{\"properties\":{\"mfid\":{\"unit\":\"hex\",\"name\":\"manufacturer id\"},\"uuid\":{\"unit\":\"hex\",\"name\":\"service uuid\"},\"major\":{\"unit\":\"hex\",\"name\":\"major value\"},\"minor\":{\"unit\":\"hex\",\"name\":\"minor value\"},\"txpower\":{\"unit\":\"dBm\",\"name\":\"tx power @ 1 m\"},\"volt\":{\"unit\":\"V\",\"name\":\"voltage\"}}}";
 /*R""""(
 {
    "properties":{
-      "batt":{
-         "unit":"%",
-         "name":"battery"
-      },
-      "tempc":{
-         "unit":"°C",
-         "name":"temperature"
-      },
-      "pres":{
-         "unit":"bar",
-         "name":"pressure"
-      },
-      "count":{
-         "unit":"int",
-         "name":"count"
-      },
-      "alarm":{
-         "unit":"status",
-         "name":"alarm"
+      "mfid":{
+         "unit":"hex",
+         "name":"manufacturer id"
+      },
+      "uuid":{
+         "unit":"hex",
+         "name":"service uuid"
+      },
+      "major":{
+         "unit":"hex",
+         "name":"major value"
+      },
+      "minor":{
+         "unit":"hex",
+         "name":"minor value"
+      },
+      "txpower":{
+         "unit":"dBm",
+         "name":"tx power @ 1 m"
+      },
+      "volt":{
+         "unit":"V",
+         "name":"voltage"
       }
    }
 })"""";*/
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `TheengsDecoder-1.4.2/src/devices/TPTH_json.h` & `TheengsDecoder-1.5.0/src/devices/TPTH_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/ThermoBeacon_json.h` & `TheengsDecoder-1.5.0/src/devices/ThermoBeacon_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/XMTZC04HM_json.h` & `TheengsDecoder-1.5.0/src/devices/XMTZC04HM_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/XMTZC05HM_json.h` & `TheengsDecoder-1.5.0/src/devices/XMTZC05HM_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/common_props.h` & `TheengsDecoder-1.5.0/src/devices/common_props.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/iBeacon_json.h` & `TheengsDecoder-1.5.0/src/devices/KKM_K6P_json.h`

 * *Files 23% similar despite different names*

```diff
@@ -1,64 +1,50 @@
-const char* _ibeacon_json = "{\"brand\":\"GENERIC\",\"model\":\"iBeacon\",\"model_id\":\"IBEACON\",\"tag\":\"06\",\"condition\":[\"manufacturerdata\",\"=\",50,\"index\",0,\"4c00\"],\"properties\":{\"mfid\":{\"decoder\":[\"string_from_hex_data\",\"manufacturerdata\",0,4]},\"uuid\":{\"decoder\":[\"string_from_hex_data\",\"manufacturerdata\",8,32]},\"major\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",40,4,false]},\"minor\":{\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",44,4,false]},\"txpower\":{\"condition\":[\"manufacturerdata\",48,\"bit\",3,1],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",48,2,false]},\"volt\":{\"condition\":[\"manufacturerdata\",48,\"bit\",3,0],\"decoder\":[\"value_from_hex_data\",\"manufacturerdata\",48,2,false],\"post_proc\":[\"/\",10]}}}";
-
+const char* _KKM_K6P_json = "{\"brand\":\"KKM\",\"model\":\"Long Range K6P\",\"model_id\":\"K6P\",\"tag\":\"01\",\"condition\":[\"servicedata\",\"=\",18,\"index\",0,\"210107\",\"&\",\"uuid\",\"index\",0,\"feaa\"],\"properties\":{\".cal\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",12,2,false,false],\"post_proc\":[\"/\",256,\"*\",100,\">\",0,\"/\",100]},\"tempc\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",10,2,false,true],\"post_proc\":[\"+\",\".cal\"]},\"_.cal\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",16,2,false,false],\"post_proc\":[\"/\",256,\"*\",100,\">\",0,\"/\",100]},\"hum\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",14,2,false,false],\"post_proc\":[\"+\",\".cal\"]},\"volt\":{\"decoder\":[\"value_from_hex_data\",\"servicedata\",6,4,false,false],\"post_proc\":[\"/\",1000]}}}";
 /*R""""(
 {
-   "brand":"GENERIC",
-   "model":"iBeacon",
-   "model_id":"IBEACON",
-   "tag":"06",
-   "condition":["manufacturerdata", "=", 50, "index", 0, "4c00"],
+   "brand":"KKM",
+   "model":"Long Range K6P",
+   "model_id":"K6P",
+   "tag":"01",
+   "condition":["servicedata", "=", 18, "index", 0, "210107", "&", "uuid", "index", 0, "feaa"],
    "properties":{
-      "mfid":{
-         "decoder":["string_from_hex_data", "manufacturerdata", 0, 4]
-      },
-      "uuid":{
-         "decoder":["string_from_hex_data", "manufacturerdata", 8, 32]
-      },
-      "major":{
-         "decoder":["value_from_hex_data", "manufacturerdata", 40, 4, false]
-      },
-      "minor":{
-         "decoder":["value_from_hex_data", "manufacturerdata", 44, 4, false]
-      },
-      "txpower":{
-         "condition":["manufacturerdata", 48, "bit", 3, 1],
-         "decoder":["value_from_hex_data","manufacturerdata", 48, 2, false]
+      ".cal":{
+         "decoder":["value_from_hex_data", "servicedata", 12, 2, false, false],
+         "post_proc":["/", 256, "*", 100, ">", 0, "/", 100]
+      },
+      "tempc":{
+         "decoder":["value_from_hex_data", "servicedata", 10, 2, false, true],
+         "post_proc":["+", ".cal"]
+      },
+      "_.cal":{
+         "decoder":["value_from_hex_data", "servicedata", 16, 2, false, false],
+         "post_proc":["/", 256, "*", 100, ">", 0, "/", 100]
+      },
+      "hum":{
+         "decoder":["value_from_hex_data", "servicedata", 14, 2, false, false],
+         "post_proc":["+", ".cal"]
       },
       "volt":{
-         "condition":["manufacturerdata", 48, "bit", 3, 0],
-         "decoder":["value_from_hex_data","manufacturerdata", 48, 2, false],
-         "post_proc":["/", 10]
+         "decoder":["value_from_hex_data", "servicedata", 6, 4, false, false],
+         "post_proc":["/", 1000]
       }
    }
 })"""";*/
 
-const char* _ibeacon_json_props = "{\"properties\":{\"mfid\":{\"unit\":\"hex\",\"name\":\"manufacturer id\"},\"uuid\":{\"unit\":\"hex\",\"name\":\"service uuid\"},\"major\":{\"unit\":\"hex\",\"name\":\"major value\"},\"minor\":{\"unit\":\"hex\",\"name\":\"minor value\"},\"txpower\":{\"unit\":\"dBm\",\"name\":\"tx power @ 1 m\"},\"volt\":{\"unit\":\"V\",\"name\":\"voltage\"}}}";
+const char* _KKM_K6P_json_props = "{\"properties\":{\"tempc\":{\"unit\":\"°C\",\"name\":\"temperature\"},\"hum\":{\"unit\":\"%\",\"name\":\"humidity\"},\"volt\":{\"unit\":\"V\",\"name\":\"voltage\"}}}";
 /*R""""(
 {
    "properties":{
-      "mfid":{
-         "unit":"hex",
-         "name":"manufacturer id"
-      },
-      "uuid":{
-         "unit":"hex",
-         "name":"service uuid"
-      },
-      "major":{
-         "unit":"hex",
-         "name":"major value"
-      },
-      "minor":{
-         "unit":"hex",
-         "name":"minor value"
-      },
-      "txpower":{
-         "unit":"dBm",
-         "name":"tx power @ 1 m"
+      "tempc":{
+         "unit":"°C",
+         "name":"temperature"
+      },
+      "hum":{
+         "unit":"%",
+         "name":"humidity"
       },
       "volt":{
          "unit":"V",
          "name":"voltage"
       }
    }
 })"""";*/
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `TheengsDecoder-1.4.2/src/devices/iNodeEM_json.h` & `TheengsDecoder-1.5.0/src/devices/iNodeEM_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices/tracker_json.h` & `TheengsDecoder-1.5.0/src/devices/tracker_json.h`

 * *Files identical despite different names*

### Comparing `TheengsDecoder-1.4.2/src/devices.h` & `TheengsDecoder-1.5.0/src/devices.h`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,16 @@
 #include "devices/SBOT_json.h"
 #include "devices/SBS1_json.h"
 #include "devices/SHT4X_json.h"
 #include "devices/SCD4X_json.h"
 #include "devices/Skale_json.h"
 #include "devices/SmartDry_json.h"
 #include "devices/TPMS_json.h"
+#include "devices/KKM_K6P_json.h"
+#include "devices/KKM_K9_json.h"
 #include "devices/ThermoBeacon_json.h"
 #include "devices/XMTZC04HM_json.h"
 #include "devices/XMTZC05HM_json.h"
 #include "devices/ABN03_json.h"
 #include "devices/ABTemp_json.h"
 #include "devices/Amphiro_json.h"
 #include "devices/PH10_json.h"
@@ -82,14 +84,15 @@
 #include "devices/BPARASITE_json.h"
 #include "devices/BWBSDOO_json.h"
 #include "devices/BM2_json.h"
 #include "devices/JHT_F525_json.h"
 #include "devices/iBeacon_json.h"
 #include "devices/APPLE_json.h"
 #include "devices/ServiceData_json.h"
+#include "devices/SBBT_002C_json.h"
 
 
 const char* _devices[][2] = {
     {_HHCCJCY01HHCC_json, _HHCCJCY01HHCC_json_props},
     {_LYWSD02_json, _LYWSD02_json_props},
     {_LYWSDCGQ_json, _LYWSDCGQ_json_props},
     {_CGP1W_json, _CGP1W_json_props},
@@ -109,14 +112,16 @@
     {_IBT_2X_json_2XS, _IBT_2X_json_props},
     {_IBT_4XS_json, _IBT_4XS_json_props},
     {_IBT_6XS_SOLIS6_json, _IBT_6XS_SOLIS6_json_props},
     {_Miband_json, _Miband_json_props},
     {_XMTZC04HM_json, _XMTZC04HM_json_props},
     {_XMTZC05HM_json, _XMTZC05HM_json_props},
     {_TPMS_json, _TPMS_json_props},
+    {_KKM_K6P_json, _KKM_K6P_json_props},
+    {_KKM_K9_json, _KKM_K9_json_props},
     {_LYWSD03MMC_json_ATC, _LYWSD03MMC_json_props},
     {_LYWSD03MMC_json_PVVX, _LYWSD03MMC_json_props},
     {_CGPR1_json, _CGPR1_json_props},
     {_ThermoBeacon_json, _ThermoBeacon_json_props},
     {_H5055_json, _H5055_json_props},
     {_H5072_json, _H5072_json_props},
     {_H5074_json, _H5074_json_props},
@@ -164,8 +169,9 @@
     {_tracker_json_tile, _tracker_json_props},
     {_tracker_json_tilename, _tracker_json_props},
     {_JHT_F525_json, _JHT_F525_json_props},
     {_ibeacon_json, _ibeacon_json_props},
     {_APPLE_json, _APPLE_json_props},
     {_APPLE_json_at, _APPLE_json_props},
     {_ServiceData_json, _ServiceData_json_props},
+    {_SBBT_002C_json, _SBBT_002C_json_props},
 };
```

