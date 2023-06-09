# Comparing `tmp/markpickle-1.5.1.tar.gz` & `tmp/markpickle-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markpickle-1.5.1.tar", max compression
+gzip compressed data, was "markpickle-1.6.0.tar", max compression
```

## Comparing `markpickle-1.5.1.tar` & `markpickle-1.6.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     1071 2023-06-08 18:02:09.907821 markpickle-1.5.1/LICENSE
--rw-r--r--   0        0        0     7182 2023-06-08 18:02:09.907821 markpickle-1.5.1/README.md
--rw-r--r--   0        0        0      574 2023-06-08 18:02:09.911821 markpickle-1.5.1/markpickle/__init__.py
--rw-r--r--   0        0        0     1437 2023-06-08 18:02:09.911821 markpickle-1.5.1/markpickle/__main__.py
--rw-r--r--   0        0        0     2005 2023-06-08 18:02:09.911821 markpickle-1.5.1/markpickle/atx_as_dictionary.py
--rw-r--r--   0        0        0     1614 2023-06-08 18:02:09.911821 markpickle-1.5.1/markpickle/binary_streams.py
--rw-r--r--   0        0        0       57 2023-06-08 18:02:09.911821 markpickle-1.5.1/markpickle/cli.py
--rw-r--r--   0        0        0     2299 2023-06-08 18:02:09.911821 markpickle-1.5.1/markpickle/config_class.py
--rw-r--r--   0        0        0    13725 2023-06-08 18:02:09.911821 markpickle-1.5.1/markpickle/deserialize.py
--rw-r--r--   0        0        0      412 2023-06-08 18:02:09.911821 markpickle-1.5.1/markpickle/meta.py
--rw-r--r--   0        0        0     1145 2023-06-08 18:02:09.911821 markpickle-1.5.1/markpickle/mypy_types.py
--rw-r--r--   0        0        0       80 2023-06-08 18:02:09.911821 markpickle-1.5.1/markpickle/py.typed
--rw-r--r--   0        0        0     5581 2023-06-08 18:02:09.911821 markpickle-1.5.1/markpickle/python_to_tables.py
--rw-r--r--   0        0        0    15441 2023-06-08 18:02:09.911821 markpickle-1.5.1/markpickle/serialize.py
--rw-r--r--   0        0        0      737 2023-06-08 18:02:09.911821 markpickle-1.5.1/markpickle/simplify_types.py
--rw-r--r--   0        0        0     1043 2023-06-08 18:02:09.911821 markpickle-1.5.1/markpickle/split_file_code.py
--rw-r--r--   0        0        0     1216 2023-06-08 18:02:09.911821 markpickle-1.5.1/markpickle/third_party_tables.py
--rw-r--r--   0        0        0     1760 2023-06-08 18:02:09.911821 markpickle-1.5.1/markpickle/tool.py
--rw-r--r--   0        0        0      813 2023-06-08 18:02:09.911821 markpickle-1.5.1/markpickle/unicode_formatting.py
--rw-r--r--   0        0        0     3725 2023-06-08 18:02:09.911821 markpickle-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     8706 1970-01-01 00:00:00.000000 markpickle-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-09 02:32:42.419553 markpickle-1.6.0/LICENSE
+-rw-r--r--   0        0        0     7355 2023-06-09 02:32:42.423553 markpickle-1.6.0/README.md
+-rw-r--r--   0        0        0      723 2023-06-09 02:32:42.423553 markpickle-1.6.0/markpickle/__init__.py
+-rw-r--r--   0        0        0     1437 2023-06-09 02:32:42.423553 markpickle-1.6.0/markpickle/__main__.py
+-rw-r--r--   0        0        0     2804 2023-06-09 02:32:42.423553 markpickle-1.6.0/markpickle/atx_as_dictionary.py
+-rw-r--r--   0        0        0     1614 2023-06-09 02:32:42.423553 markpickle-1.6.0/markpickle/binary_streams.py
+-rw-r--r--   0        0        0       57 2023-06-09 02:32:42.423553 markpickle-1.6.0/markpickle/cli.py
+-rw-r--r--   0        0        0     2539 2023-06-09 02:32:42.423553 markpickle-1.6.0/markpickle/config_class.py
+-rw-r--r--   0        0        0    14645 2023-06-09 02:32:42.423553 markpickle-1.6.0/markpickle/deserialize.py
+-rw-r--r--   0        0        0      412 2023-06-09 02:32:42.423553 markpickle-1.6.0/markpickle/meta.py
+-rw-r--r--   0        0        0     1406 2023-06-09 02:32:42.423553 markpickle-1.6.0/markpickle/mypy_types.py
+-rw-r--r--   0        0        0       80 2023-06-09 02:32:42.423553 markpickle-1.6.0/markpickle/py.typed
+-rw-r--r--   0        0        0     5581 2023-06-09 02:32:42.423553 markpickle-1.6.0/markpickle/python_to_tables.py
+-rw-r--r--   0        0        0    15443 2023-06-09 02:32:42.423553 markpickle-1.6.0/markpickle/serialize.py
+-rw-r--r--   0        0        0      737 2023-06-09 02:32:42.423553 markpickle-1.6.0/markpickle/simplify_types.py
+-rw-r--r--   0        0        0     1043 2023-06-09 02:32:42.423553 markpickle-1.6.0/markpickle/split_file_code.py
+-rw-r--r--   0        0        0      538 2023-06-09 02:32:42.423553 markpickle-1.6.0/markpickle/sugar.py
+-rw-r--r--   0        0        0     1216 2023-06-09 02:32:42.423553 markpickle-1.6.0/markpickle/third_party_tables.py
+-rw-r--r--   0        0        0     1760 2023-06-09 02:32:42.423553 markpickle-1.6.0/markpickle/tool.py
+-rw-r--r--   0        0        0      813 2023-06-09 02:32:42.423553 markpickle-1.6.0/markpickle/unicode_formatting.py
+-rw-r--r--   0        0        0     3886 2023-06-09 02:32:42.423553 markpickle-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     8879 1970-01-01 00:00:00.000000 markpickle-1.6.0/PKG-INFO
```

### Comparing `markpickle-1.5.1/LICENSE` & `markpickle-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `markpickle-1.5.1/README.md` & `markpickle-1.6.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # markpickle
 
 Markpickle is a Python library for lossy serialization of markdown to simple python data types and back. Imagine if markdown headers were used to define nested dictionaries and Markdown lists were python lists.
 
 It will create predictable markdown from a python object, but can't turn all markdown files into sensible python objects (for that use a markdown library that creates an AST). I created this because I wanted a way to turn json into Markdown. It is an accidental successor to [markdown-to-json](https://github.com/njvack/markdown-to-json).
 
-For example this
-
 ```markdown
 - 1
 - 2
 ```
 
 becomes the python list `[1, 2]`
 
@@ -21,15 +19,15 @@
 Felix
 ```
 
 becomes the python list `{"cat":{"Name":"Ringo","Species":"Felix"}`
 
 See [examples](https://github.com/matthewdeanmartin/markpickle/blob/main/docs/examples.md) for representable types.
 
-Almost all markdown libraries use it as intended, as a way to generate HTML fragments from untrusted sources for insertion into some other HTML template. We are using it to represent data. See [guidance](docs/choosing_a_library.md) for which library make sense for you.
+Almost all markdown libraries use it as a way to generate HTML fragments from untrusted sources for insertion into some other HTML template. We are using it to represent data. See [guidance](docs/choosing_a_library.md) for which library make sense for you.
 
 ![Libraries.io dependency status for latest release](https://img.shields.io/librariesio/release/pypi/markpickle) [![Downloads](https://pepy.tech/badge/markpickle/month)](https://pepy.tech/project/markpickle/month)
 
 ______________________________________________________________________
 
 ## Installation
 
@@ -89,15 +87,17 @@
 
 ```bash
 python -m markpickle "docs/individual/list of scalars.md"
 ```
 
 ## Prior Art
 
-People normally want to convert json to markdown. Json looks like python dict, so if you can do that you can probably do both.
+Imagine you have json and want to the same data as markdown. Json looks like python dict, so any python library that can convert json to markdown, probably can convert a python dict to markdown.
+
+Many tools turn tabular data into a markdown table.
 
 ### Serializing to Markdown
 
 [json2md](https://github.com/IonicaBizau/json2md), a node package, will turn json that looks like the HTML document object model into markdown, e.g.
 
 ```python
 {"h1": "Some Header",
@@ -108,31 +108,36 @@
 
 [pytablewriter](https://pytablewriter.readthedocs.io/en/latest/pages/reference/writers/text/markup/md.html) also, dict to table, but supports many tabular formats.
 
 ### Deserializing to Python
 
 Most libraries turn markdown into document object model. Markdown-to-json is the most similar to markpickle's goal of turning a markdown document into a python data types, in this case nested dicts.
 
-[markdown-to-json](https://github.com/njvack/markdown-to-json) is the library most similar to markpickle, but is somewhat broken, unmaintained and depends on the unmaintained commonmark library.
+[markdown-to-json](https://github.com/njvack/markdown-to-json) is the library most similar to markpickle and is now maintained. It handles only deserialization and conversion to json.
 
 [mistune](https://pypi.org/project/mistune/) will turn markdown into an Abstract Syntax Tree. The AST is faithful representation of the Markdown, including concepts that have no semantic equivalent to python datatypes.
 
 [beautifulsoup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/) will let you navigate the HTML DOM. So you can turn the markdown into HTML, then parse with Beautiful Soup.
 
 ## Representable Types
 
 There is one optional root dictionary representable with ATX headers, e.g. `#`, `##`, etc. Lists are nestable lists or dicts. For the most part, this looks like the types that JSON can represent.
 
 ```python
-from typing import Union, TypeAlias
-import datetime
-import PIL
-MarkSerializable: TypeAlias = Union[
-    dict[str, "MarkSerializable"],
-    list["MarkSerializable"], str, int, float, bool, datetime, PIL.image, bytes, None]
+SerializableTypes: TypeAlias = Union[
+    ColumnsValuesTableType,
+    dict[str, "SerializableTypes"],
+    list["SerializableTypes"],
+    str,
+    int,
+    float,
+    bool,
+    datetime.date,
+    None,
+]
 ```
 
 The deserialized types is the same except all Scalars are strings.
 
 ## Schema Validation for Markdown
 
 In the case of a serialization library, you'd want something that would indicate if your markdown file will successfully deserialize back into python.
@@ -150,9 +155,15 @@
 - [Choosing a Library](https://github.com/matthewdeanmartin/markpickle/blob/main/docs/choosing_a_library.md)
 - [Examples](https://github.com/matthewdeanmartin/markpickle/blob/main/docs/examples.md)
 - [TODO](https://github.com/matthewdeanmartin/markpickle/blob/main/docs/TODO.md)
 - [People solving similar problems on StackOverflow](https://github.com/matthewdeanmartin/markpickle/blob/main/docs/stackoverflow.md)
 
 ## Change Log
 
-- 1.1.0 - Basic functionality. See [examples](https://github.com/matthewdeanmartin/markpickle/blob/main/docs/examples.md) for what is supported.
+- 0.2.0 - Idea and reserve package name.
+- 1.0.0 - Basic functionality.
+- 1.1.0 - Basic functionality.
 - 1.2.0 - Add support for binary data, which is serialized as images with data URLs.
+- 1.3.0 - Improve CLI and more examples
+- 1.4.0 - ATX as dictionary now works
+- 1.5.0 - Tables less buggy
+- 1.5.1 - Fix mypy typing. Pin mistune to <3.0.0
```

### Comparing `markpickle-1.5.1/markpickle/__init__.py` & `markpickle-1.6.0/markpickle/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,8 +15,12 @@
     "loads_all",
     "dump",
     "dump_all",
     "dumps",
     "dumps_all",
     "Config",
     "split_file",
+    "convert_json_to_markdown",
+    "convert_markdown_to_json",
 ]
+
+from markpickle.sugar import convert_json_to_markdown, convert_markdown_to_json
```

### Comparing `markpickle-1.5.1/markpickle/__main__.py` & `markpickle-1.6.0/markpickle/__main__.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.5.1/markpickle/atx_as_dictionary.py` & `markpickle-1.6.0/markpickle/atx_as_dictionary.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,24 @@
     ATX headers, e.g. # Header, ## Subheader, can be used for a single set of nested dictionaries.
     """
     candidate = recursive_part(level, cast(MistuneTokenList, token_list))
 
     # recursive
     if isinstance(candidate, dict):
         for token_key, token_list in candidate.items():
-            candidate[token_key] = recursive_part(level + 1, cast(MistuneTokenList, token_list))
+            # Sometimes people skip a level!
+            the_sequence = [
+                item["level"] if item["type"] == "heading" else 10000000 for item in cast(MistuneTokenList, token_list)
+            ]
+            if not the_sequence:
+                next_level = level + 1
+            else:
+                next_level = min(the_sequence)
+
+            candidate[token_key] = recursive_part(next_level, cast(MistuneTokenList, token_list))
 
     if candidate:
         return candidate
     # no ATX dict-like structures here.
     # mypy doesn't like this, but this is really just a hack to hold a list.
     return cast(PossibleDictTypes, {None: token_list})
 
@@ -39,19 +48,33 @@
     for item in token_list:
         if item["type"] == "newline":
             # ignore whitespace
             continue
         if item["type"] == "heading" and item["level"] == level:
             if key:
                 candidate[key] = between_values
-            key = "".join(_["text"] for _ in item["children"])
+            key = strip_formatting(item)
             between_values = []
             continue
 
         between_values.append(cast(dict[Optional[str], Any], item))
 
     # left overs
     if key and between_values:
         candidate[key] = between_values
     if not candidate:
         return between_values
     return candidate
+
+
+def strip_formatting(item: dict[str, list[dict[str, Any]]], joiner: str = " "):
+    """For when we just don't have a good way to handle bold, underline, etc."""
+    parts: list[str] = []
+    for _ in item["children"]:
+        if "text" in _:
+            parts.append(_["text"])
+            continue
+        if "children" in _:
+            stripped = strip_formatting(_)
+            parts.append(stripped)
+    key = joiner.join(parts)
+    return key
```

### Comparing `markpickle-1.5.1/markpickle/binary_streams.py` & `markpickle-1.6.0/markpickle/binary_streams.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.5.1/markpickle/config_class.py` & `markpickle-1.6.0/markpickle/config_class.py`

 * *Files 12% similar despite different names*

```diff
@@ -55,7 +55,13 @@
 
     serialize_include_python_type: bool = False
     """Help deserializer find correct constructor"""
 
     serialize_images_to_pillow: bool = False
 
     default: Optional[Callable[[object], str]] = None
+
+    deserialized_add_missing_key: bool = True
+    """If document has ATX headers add missing initial ATX header"""
+
+    deserialized_missing_key_name: str = "Missing Key"
+    """Add `# Missing Key` to head of document if missing."""
```

### Comparing `markpickle-1.5.1/markpickle/deserialize.py` & `markpickle-1.6.0/markpickle/deserialize.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import textwrap
 import urllib.parse
 from typing import Any, Generator, Optional, cast
 
 import mistune
 
 import markpickle.python_to_tables as python_to_tables
-from markpickle.atx_as_dictionary import parse_outermost_dict
+from markpickle.atx_as_dictionary import parse_outermost_dict, strip_formatting
 from markpickle.binary_streams import extract_bytes
 from markpickle.config_class import Config
 from markpickle.mypy_types import (
     DictTypes,
     ListTypes,
     MistuneTokenList,
     PossibleDictTypes,
@@ -97,19 +97,19 @@
 
 def process_list(list_ast: Any, config: Config) -> ListTypes:
     """Deserialize a markdown list in AST form"""
     current_list: ListTypes = []
     for token in list_ast["children"]:
         if token["type"] == "list_item":
             for child in token["children"]:
-                if child["type"] == "block_text":
+                if child["type"] in ("block_text", "paragraph"):
                     block_text = child
                     if block_text["children"][0]["type"] == "text":
                         # This fails if not all text!
-                        current_value = ",".join(str(text.get("text")) for text in block_text["children"])
+                        current_value = strip_formatting(block_text, ",")
                         scalar = extract_scalar(current_value, config)
                         current_list.append(scalar)
                     elif block_text["children"][0]["type"] == "link":
                         # Doesn't handle title or text
                         url = urllib.parse.urlparse(block_text["children"][0]["link"])
                         # HACK: Turn off type checking
                         current_list.append(cast(Any, url))
@@ -170,39 +170,29 @@
         yield loads(part.read(), config, object_hook)
 
 
 def process_list_of_tokens(list_of_tokens: MistuneTokenList, config: Config) -> Optional[SerializableTypes]:
     """Process a list of tokens to lists and scalars and so on."""
     # Tokens that are not ATX-dict-like headers
     return_value: Optional[SerializableTypes] = None
+
+    accumulate_a_tuple: list[SerializableTypes] = []
     for token in list_of_tokens:
         if token["type"] == "newline":
             # Whitespace, no impact on datatype
             continue
 
-        # if token["type"] == "heading" and current_key is None:
-        #     # Dict key, value not found yet
-        #     if not all("text" in _ for _ in token["children"]):
-        #         print("uh oh")
-        #     current_key = ",".join([_["text"] for _ in token["children"]])
-        #     possible_dict[current_key] = None
-        # elif token["type"] == "heading" and current_key is not None:
-        #     # New dict key, value not found yet
-        #     if not all("text" in _ for _ in token["children"]):
-        #         print("uh oh")
-        #     current_key = ",".join([_["text"] for _ in token["children"]])
-        #     possible_dict[current_key] = None
         if token["type"] == "list":
             # Dict value of type list
             if token["children"][0]["type"] == "text":
-                return_value = cast(
-                    Optional[ListTypes], [",".join(_["text"] for _ in item["children"]) for item in token["children"]]
-                )
+                list_contents_as_text = cast(Optional[ListTypes], strip_formatting(token, ","))
+                accumulate_a_tuple.append(list_contents_as_text)
             elif token["children"][0]["type"] == "list_item":
-                return_value = process_list(token, config)
+                sublist = process_list(token, config)
+                accumulate_a_tuple.append(sublist)
             else:
                 raise NotImplementedError()
 
         elif (
             token["type"] == "paragraph"
             and token.get("children")
             and len(token["children"]) == 1
@@ -214,57 +204,85 @@
             # Root scalar
             current_text_value: str = token["children"][0]["text"]
             if current_text_value.count("|") >= 2 and config.tables_become_list_of_tuples:
                 return python_to_tables.parse_table_with_regex(current_text_value)
             elif current_text_value.count("|") >= 2:
                 return python_to_tables.parse_table_to_list_of_dict(current_text_value)
 
-            return extract_scalar(current_text_value, config)
+            some_scalar = extract_scalar(current_text_value, config)
+            accumulate_a_tuple.append(some_scalar)
 
         elif (
             token["type"] == "paragraph"
             and token.get("children")
+            and all(_.get("type") in ("text", "codespan", "strong") for _ in token["children"])
+        ):
+            # E.g. "Cat *and* Dog", which is 3 child tokens because of formatting
+            current_value: str = strip_formatting(token)
+            scalar = extract_scalar(current_value, config)
+            accumulate_a_tuple.append(scalar)
+        elif (
+            token["type"] == "paragraph"
+            and token.get("children")
             and len(token["children"]) == 1
             and token["children"][0]["type"] == "text"
         ):
-            # Root scalar
-            if token["children"][0]["type"] == "text":
-                current_value: str = token["children"][0]["text"]
-                scalar = extract_scalar(current_value, config)
-            elif token["children"][0]["type"] == "image":
+            # Handle images
+            if token["children"][0]["type"] == "image":
                 scalar = extract_bytes(token["children"][0]["src"], config)
             else:
                 raise NotImplementedError()
-            return_value = scalar
-        # what was this?
-        # elif (
-        #         token["type"] == "paragraph"
-        #         and token.get("children")
-        #         # and len(token["children"]) == 1
-        #         # and token["children"][0]["type"] == "text"
-        # ):
-        #     series_of_children = token["children"]
-        #     most_recent_key = handle_series_of_children(config, most_recent_key, outermost_dict, series_of_children)
-        #     current_key = None
+            accumulate_a_tuple.append(scalar)
         elif token["type"] == "block_code":
+            # See markmodule for treating block_code as code. Can't easily do it here.
             # Treat block code as just more text, no "styling"
             continuation_value: str = token["text"]
             scalar = extract_scalar(continuation_value, config)
             # continuation of text
             if return_value:
                 # mypy isn't sure if scalar is always a string.
-                return_value = str(return_value) + "\n\n" + str(scalar)
+                accumulate_a_tuple.append(str(return_value) + "\n\n" + str(scalar))
             else:
-                return_value = scalar
+                accumulate_a_tuple.append(scalar)
         elif token["type"] == "heading":
             # handled elsewhere?
-            pass
-        # else:
-        #     raise NotImplementedError(token["type"])
-    return return_value
+            raise TypeError("Unconsumed header... shouldn't be in AST by this point.")
+        else:
+            # This is probably mixed content.
+            # e.g. a paragraph + list + something + something
+            raise NotImplementedError(
+                f"Probably mixed content (tuple) where a single scalar/list/dict was expected. {token['type']}"
+            )
+    if len(accumulate_a_tuple) == 0:
+        # Found nothing.
+        return None
+    if len(accumulate_a_tuple) == 1:
+        # Found only 1 thing.
+        return accumulate_a_tuple[0]
+
+    # This probably means that the markdown is more of a DOM than a data structure.
+    # Found a mixture of things. I guess those are tuples.
+    return cast(SerializableTypes, tuple(accumulate_a_tuple))
+
+
+def missing_top_key(result: MistuneTokenList):
+    """The ATX-header root dictionary will discard the top part of the document without an starting key,
+    e.g. a h1/# token"""
+    found: list[dict[str, Any]] = []
+    for token in result:
+        if token["type"] == "newline":
+            continue
+        if token["type"] == "paragraph" and token.get("children"):
+            possible_whitespace = strip_formatting(token)
+            if possible_whitespace.strip() == "":
+                continue
+        if token["type"] == "heading" and found == []:
+            return False
+        found.append(token)
+    return True
 
 
 def load(value: io.StringIO, config: Optional[Config] = None, object_hook=None) -> SerializableTypes:
     """
     Convert certain markdown streams into simple Python types
 
     >>> import io
@@ -299,16 +317,20 @@
     # Process a list
     if len(result) == 1 and result[0]["type"] == "list":
         return process_list(result[0], config)
 
     dict_wrapper = False
     # handle ATX-dict-like headers
     has_headers = any(True if item["type"] == "heading" else False for item in result)
+
     if has_headers:
+        # handle people skipping to ## or ###
         minimum = min(item["level"] if item["type"] == "heading" else 100000000 for item in result)
+        if missing_top_key(result) and config.deserialized_add_missing_key:
+            result = parser.parse("#" * minimum + f" {config.deserialized_missing_key_name}\n\n" + string_value)
         outermost_dict = parse_outermost_dict(result, minimum)
         outermost_dict = walk_dict(cast(PossibleDictTypes, outermost_dict), config)
     else:
         dict_wrapper = True
         outermost_dict = {None: process_list_of_tokens(result, config)}
 
     # if possible_dict and possible_dict.get("python_type"):
```

### Comparing `markpickle-1.5.1/markpickle/mypy_types.py` & `markpickle-1.6.0/markpickle/mypy_types.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from __future__ import annotations
 
 import datetime
 from typing import Any, Optional, Union
 
 try:
     from typing_extensions import TypeAlias
+except ModuleNotFoundError:
+    from typing import TypeAlias  # type: ignore[no-redef,attr-defined]
 except ImportError:
     from typing import TypeAlias  # type: ignore[no-redef,attr-defined]
 
 
 # https://github.com/python/mypy/issues/14219#issuecomment-1528993478
 ScalarTypes = Union[
     None,
@@ -20,22 +22,29 @@
     float,
     datetime.date,
 ]
 # There are many ways to represent a table
 ColumnsValuesTableType = list[Union[tuple[str, ...], list[Any]]]
 SerializableTypes: TypeAlias = Union[
     ColumnsValuesTableType,
+    # ATX headers
     dict[str, "SerializableTypes"],
+    # lists and nested lists
     list["SerializableTypes"],
+    # series of paragraphs/lists/etc
+    tuple["SerializableTypes"],
     str,
     int,
     float,
     bool,
     datetime.date,
     None,
+    # bytes
+    # images
+    # urls
 ]
 DictTypes = dict[str, SerializableTypes]
 ListTypes = list[SerializableTypes]
 
 # Intermediate states for parsing AST
 MistuneTokenList = list[dict[str, Any]]  # list[dict[Optional[str], Any]]
 # for when the key is None because it is actually a list.
```

### Comparing `markpickle-1.5.1/markpickle/python_to_tables.py` & `markpickle-1.6.0/markpickle/python_to_tables.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.5.1/markpickle/serialize.py` & `markpickle-1.6.0/markpickle/serialize.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,15 +228,15 @@
                 seralialized_scalar = minibuilder.getvalue()
                 builder.write(f"{header_level * '#'} {key}\n" f"{seralialized_scalar}\n")
             else:
                 # This is ad hoc and not a markdown standard.
                 minibuilder = io.StringIO()
                 render_scalar(minibuilder, item, config)
                 seralialized_scalar = minibuilder.getvalue()
-                builder.write(f"{indent * ' '}{config.list_bullet_style} {key} : {seralialized_scalar}\n")
+                builder.write(f"{indent * '  '}{config.list_bullet_style} {key} : {seralialized_scalar}\n")
         elif isinstance(item, list):
             if item and isinstance(item[0], dict):
                 if config.serialize_headers_are_dict_keys and indent == 0:
                     # headers dict keys. Can't nest.
                     header = f"{header_level * '#'} {key}\n"
                     builder.write(header)
                 else:
@@ -309,15 +309,15 @@
 
     # The list is not of dictionaries or we don't want tables.
     for item in value:
         if not isinstance(item, (list, dict, set)):
             minibuilder = io.StringIO()
             render_scalar(minibuilder, item, config)
             seralialized_scalar = minibuilder.getvalue()
-            builder.write(f"{indent * ' '}{config.list_bullet_style} {seralialized_scalar}\n")
+            builder.write(f"{indent * '  '}{config.list_bullet_style} {seralialized_scalar}\n")
         elif isinstance(item, list):
             if item and isinstance(item[0], dict):
                 # assuming if the first is dict, they all are dict.
                 python_to_tables.list_of_dict_to_markdown(builder, cast(list[DictTypes], item), indent)
             else:
                 render_list(builder, cast(list[SerializableTypes], item), config, indent + 1, header_level)
         elif isinstance(item, dict):
```

### Comparing `markpickle-1.5.1/markpickle/simplify_types.py` & `markpickle-1.6.0/markpickle/simplify_types.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.5.1/markpickle/split_file_code.py` & `markpickle-1.6.0/markpickle/split_file_code.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.5.1/markpickle/third_party_tables.py` & `markpickle-1.6.0/markpickle/third_party_tables.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.5.1/markpickle/tool.py` & `markpickle-1.6.0/markpickle/tool.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.5.1/markpickle/unicode_formatting.py` & `markpickle-1.6.0/markpickle/unicode_formatting.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.5.1/pyproject.toml` & `markpickle-1.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "markpickle"
-version = "1.5.1"
+version = "1.6.0"
 description = "Lossy python to markdown serializer"
 authors = ["Matthew Martin <matthewdeanmartin@gmail.com>"]
 keywords = ["serializer", "deserializer", "markdown",]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
@@ -154,8 +154,17 @@
 
 #[tool.setuptools]
 ## find = {}
 #py-modules = ["markpickle",
 #    "markpickle.deserialize",
 #    "markpickle.python_to_tables",
 #    "markpickle.serialize",
-#]
+#]
+
+[mypy]
+warn_return_any = true
+warn_unused_configs = true
+strict = true
+
+[[tool.mypy.overrides]]
+module = ["mistune.*"]
+ignore_missing_imports = true
```

### Comparing `markpickle-1.5.1/PKG-INFO` & `markpickle-1.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markpickle
-Version: 1.5.1
+Version: 1.6.0
 Summary: Lossy python to markdown serializer
 Home-page: https://github.com/matthewdeanmartin/markpickle
 License: MIT
 Keywords: serializer,deserializer,markdown
 Author: Matthew Martin
 Author-email: matthewdeanmartin@gmail.com
 Classifier: Development Status :: 3 - Alpha
@@ -35,16 +35,14 @@
 
 # markpickle
 
 Markpickle is a Python library for lossy serialization of markdown to simple python data types and back. Imagine if markdown headers were used to define nested dictionaries and Markdown lists were python lists.
 
 It will create predictable markdown from a python object, but can't turn all markdown files into sensible python objects (for that use a markdown library that creates an AST). I created this because I wanted a way to turn json into Markdown. It is an accidental successor to [markdown-to-json](https://github.com/njvack/markdown-to-json).
 
-For example this
-
 ```markdown
 - 1
 - 2
 ```
 
 becomes the python list `[1, 2]`
 
@@ -56,15 +54,15 @@
 Felix
 ```
 
 becomes the python list `{"cat":{"Name":"Ringo","Species":"Felix"}`
 
 See [examples](https://github.com/matthewdeanmartin/markpickle/blob/main/docs/examples.md) for representable types.
 
-Almost all markdown libraries use it as intended, as a way to generate HTML fragments from untrusted sources for insertion into some other HTML template. We are using it to represent data. See [guidance](docs/choosing_a_library.md) for which library make sense for you.
+Almost all markdown libraries use it as a way to generate HTML fragments from untrusted sources for insertion into some other HTML template. We are using it to represent data. See [guidance](docs/choosing_a_library.md) for which library make sense for you.
 
 ![Libraries.io dependency status for latest release](https://img.shields.io/librariesio/release/pypi/markpickle) [![Downloads](https://pepy.tech/badge/markpickle/month)](https://pepy.tech/project/markpickle/month)
 
 ______________________________________________________________________
 
 ## Installation
 
@@ -124,15 +122,17 @@
 
 ```bash
 python -m markpickle "docs/individual/list of scalars.md"
 ```
 
 ## Prior Art
 
-People normally want to convert json to markdown. Json looks like python dict, so if you can do that you can probably do both.
+Imagine you have json and want to the same data as markdown. Json looks like python dict, so any python library that can convert json to markdown, probably can convert a python dict to markdown.
+
+Many tools turn tabular data into a markdown table.
 
 ### Serializing to Markdown
 
 [json2md](https://github.com/IonicaBizau/json2md), a node package, will turn json that looks like the HTML document object model into markdown, e.g.
 
 ```python
 {"h1": "Some Header",
@@ -143,31 +143,36 @@
 
 [pytablewriter](https://pytablewriter.readthedocs.io/en/latest/pages/reference/writers/text/markup/md.html) also, dict to table, but supports many tabular formats.
 
 ### Deserializing to Python
 
 Most libraries turn markdown into document object model. Markdown-to-json is the most similar to markpickle's goal of turning a markdown document into a python data types, in this case nested dicts.
 
-[markdown-to-json](https://github.com/njvack/markdown-to-json) is the library most similar to markpickle, but is somewhat broken, unmaintained and depends on the unmaintained commonmark library.
+[markdown-to-json](https://github.com/njvack/markdown-to-json) is the library most similar to markpickle and is now maintained. It handles only deserialization and conversion to json.
 
 [mistune](https://pypi.org/project/mistune/) will turn markdown into an Abstract Syntax Tree. The AST is faithful representation of the Markdown, including concepts that have no semantic equivalent to python datatypes.
 
 [beautifulsoup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/) will let you navigate the HTML DOM. So you can turn the markdown into HTML, then parse with Beautiful Soup.
 
 ## Representable Types
 
 There is one optional root dictionary representable with ATX headers, e.g. `#`, `##`, etc. Lists are nestable lists or dicts. For the most part, this looks like the types that JSON can represent.
 
 ```python
-from typing import Union, TypeAlias
-import datetime
-import PIL
-MarkSerializable: TypeAlias = Union[
-    dict[str, "MarkSerializable"],
-    list["MarkSerializable"], str, int, float, bool, datetime, PIL.image, bytes, None]
+SerializableTypes: TypeAlias = Union[
+    ColumnsValuesTableType,
+    dict[str, "SerializableTypes"],
+    list["SerializableTypes"],
+    str,
+    int,
+    float,
+    bool,
+    datetime.date,
+    None,
+]
 ```
 
 The deserialized types is the same except all Scalars are strings.
 
 ## Schema Validation for Markdown
 
 In the case of a serialization library, you'd want something that would indicate if your markdown file will successfully deserialize back into python.
@@ -185,10 +190,16 @@
 - [Choosing a Library](https://github.com/matthewdeanmartin/markpickle/blob/main/docs/choosing_a_library.md)
 - [Examples](https://github.com/matthewdeanmartin/markpickle/blob/main/docs/examples.md)
 - [TODO](https://github.com/matthewdeanmartin/markpickle/blob/main/docs/TODO.md)
 - [People solving similar problems on StackOverflow](https://github.com/matthewdeanmartin/markpickle/blob/main/docs/stackoverflow.md)
 
 ## Change Log
 
-- 1.1.0 - Basic functionality. See [examples](https://github.com/matthewdeanmartin/markpickle/blob/main/docs/examples.md) for what is supported.
+- 0.2.0 - Idea and reserve package name.
+- 1.0.0 - Basic functionality.
+- 1.1.0 - Basic functionality.
 - 1.2.0 - Add support for binary data, which is serialized as images with data URLs.
+- 1.3.0 - Improve CLI and more examples
+- 1.4.0 - ATX as dictionary now works
+- 1.5.0 - Tables less buggy
+- 1.5.1 - Fix mypy typing. Pin mistune to <3.0.0
```

