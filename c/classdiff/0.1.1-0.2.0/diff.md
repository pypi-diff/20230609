# Comparing `tmp/classdiff-0.1.1.tar.gz` & `tmp/classdiff-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classdiff-0.1.1.tar", max compression
+gzip compressed data, was "classdiff-0.2.0.tar", max compression
```

## Comparing `classdiff-0.1.1.tar` & `classdiff-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1386 2023-05-09 14:50:06.267093 classdiff-0.1.1/README.md
--rw-r--r--   0        0        0       59 2023-05-09 13:58:40.964963 classdiff-0.1.1/classdiff/__init__.py
--rw-r--r--   0        0        0     7859 2023-05-29 11:55:55.933166 classdiff-0.1.1/classdiff/classdiff.py
--rw-r--r--   0        0        0     2706 2023-05-29 11:53:42.400335 classdiff-0.1.1/classdiff/examples/classdiff.py
--rw-r--r--   0        0        0      996 2023-05-09 13:58:40.976016 classdiff-0.1.1/classdiff/json.py
--rw-r--r--   0        0        0      638 2023-05-22 07:09:42.086138 classdiff-0.1.1/classdiff/utils.py
--rw-r--r--   0        0        0     1510 2023-05-29 12:05:06.670311 classdiff-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1861 1970-01-01 00:00:00.000000 classdiff-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2226 2023-06-09 18:09:47.217143 classdiff-0.2.0/README.md
+-rw-r--r--   0        0        0       59 2023-05-09 13:58:40.964963 classdiff-0.2.0/classdiff/__init__.py
+-rw-r--r--   0        0        0     8670 2023-06-09 18:14:21.550319 classdiff-0.2.0/classdiff/classdiff.py
+-rw-r--r--   0        0        0     3784 2023-06-09 18:18:11.579912 classdiff-0.2.0/classdiff/examples/classdiff.py
+-rw-r--r--   0        0        0      996 2023-05-09 13:58:40.976016 classdiff-0.2.0/classdiff/json.py
+-rw-r--r--   0        0        0      638 2023-05-22 07:09:42.086138 classdiff-0.2.0/classdiff/utils.py
+-rw-r--r--   0        0        0     1518 2023-06-09 18:18:23.134321 classdiff-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2701 1970-01-01 00:00:00.000000 classdiff-0.2.0/PKG-INFO
```

### Comparing `classdiff-0.1.1/classdiff/classdiff.py` & `classdiff-0.2.0/classdiff/classdiff.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,23 +72,26 @@
                 color = Font.ENDC
 
         indent = " " * (2 * self.indent)
 
         return f"{color}{self.diff_type.value} {indent}{key}{value}{Font.ENDC}"
 
 
-def enum_name(value: Enum):
+def enum_name(value: Enum) -> str:
+    """Return the name of the enum."""
     return value.name
 
 
-def enum_value(value: Enum):
+def enum_value(value: Enum) -> str:
+    """Return the value of the enum."""
     return value.value
 
 
-def enum_full(value: Enum):
+def enum_full(value: Enum) -> str:
+    """Return full enum name including class."""
     return f"{value.__class__.__name__}.{value.name}"
 
 
 def diff(  # noqa: PLR0915
     a: IsDataclass | object | None,
     b: IsDataclass | object | None,
     *,
@@ -100,36 +103,37 @@
     Diff two dataclasses.
 
     Calculate the diff between two passed (data)classes or dictionaries.
 
     Arguments:
         a: The first dataclass
         b: The second dataclass
+        enum_formatter: Function used to format enum output
         indent: The current level in the dataclass
         class_key: The key in a parent dict where the class was found
 
     Returns:
         A list of `DiffInfo`
     """
     if a is None and b is None:
         return []
 
     if isinstance(a, dict):
         a_dict = a
-    elif a is None:
-        a_dict = {}
-    else:
+    elif hasattr(a, "__dict__"):
         a_dict = a.__dict__
+    else:
+        a_dict = {}
 
     if isinstance(b, dict):
         b_dict = b
-    elif b is None:
-        b_dict = {}
-    else:
+    elif hasattr(b, "__dict__"):
         b_dict = b.__dict__
+    else:
+        b_dict = {}
 
     changeset = {}
     if a is not None and b is not None:
         if type(a) != type(b):
             return diff(
                 a,
                 None,
@@ -207,23 +211,36 @@
             value=f"{Font.BOLD}{Font.UNDERLINE}{class_name}{Font.NO_UNDERLINE}{Font.NO_BOLD}{class_opening}",
             previous_value=None,
         )
     ]
 
     for key, change_type in all_keys:
         if change_type == "deleted":
-            class_diff.extend(
-                diff(
-                    None,
-                    secondary_data[key],
-                    enum_formatter=enum_formatter,
-                    indent=indent + 1,
-                    class_key=key,
+            sd = secondary_data[key]
+            if isinstance(sd, dict) or hasattr(sd, "__dict__"):
+                class_diff.extend(
+                    diff(
+                        None,
+                        secondary_data[key],
+                        enum_formatter=enum_formatter,
+                        indent=indent + 1,
+                        class_key=key,
+                    )
                 )
-            )
+            else:
+                class_diff.append(
+                    DiffInfo(
+                        indent=indent,
+                        diff_type=DiffType.REMOVED,
+                        key=key,
+                        value=sd,
+                        previous_value=None,
+                    )
+                )
+
             continue
 
         value = primary_data[key]
 
         if isinstance(value, Enum):
             value = enum_formatter(value)
 
@@ -264,15 +281,17 @@
                 )
             )
             continue
 
         class_diff.append(
             DiffInfo(
                 indent=indent,
-                diff_type=diff_type,
+                diff_type=diff_type
+                if key in secondary_data or diff_type != DiffType.UNCHANGED
+                else DiffType.ADDED,
                 key=key,
                 value=value,
                 previous_value=None,
             )
         )
 
     class_diff.append(
```

### Comparing `classdiff-0.1.1/classdiff/examples/classdiff.py` & `classdiff-0.2.0/classdiff/examples/classdiff.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,22 +15,65 @@
     quantity: int
     dangerous: bool
     other: OtherClass
     not_changed: OtherClass
 
 
 def main():
+    added_removed_changed()
     changed_keys()
     missing_keys()
     with_dict()
     with_dataclasses()
     enum()
 
 
-def enum():
+def added_removed_changed() -> None:
+    a1 = {
+        "parent": {
+            "unchanged": "unchanged",
+            "changed": 1,
+            "changed_list": [1, 2, 3],
+            "changed_dict": {
+                "added": "added",
+                "unchanged": "unchanged",
+                "changed": "a",
+            },
+            "added": "added",
+            "added_list": [1, 2, 3],
+            "added_dict": {
+                "first": 1,
+            },
+        }
+    }
+    a2 = {
+        "parent": {
+            "unchanged": "unchanged",
+            "changed": 2,
+            "changed_list": [4, 5, 6],
+            "changed_dict": {
+                "removed": "removed",
+                "unchanged": "unchanged",
+                "changed": "b",
+            },
+            "removed": "removed",
+            "removed_list": [1, 2, 3],
+            "removed_dict": {
+                "second": 2,
+            },
+        }
+    }
+
+    for l in classdiff.diff(a1, a2):
+        print(l)
+
+    print("-" * 40)
+
+
+def enum() -> None:
     from enum import Enum
 
     class YesOrNo(Enum):
         YES = "y"
         NO = "n"
 
     @dataclass
@@ -44,15 +87,15 @@
     for fn in [classdiff.enum_name, classdiff.enum_value, classdiff.enum_full]:
         for l in classdiff.diff(a1, a2, enum_formatter=fn):
             print(l)
 
         print("-" * 40)
 
 
-def changed_keys():
+def changed_keys() -> None:
     @dataclass
     class A:
         a: str
 
     @dataclass
     class B:
         b: str
@@ -62,25 +105,25 @@
 
     for l in classdiff.diff(a, b):
         print(l)
 
     print("-" * 40)
 
 
-def missing_keys():
+def missing_keys() -> None:
     a = {"foo": {"x": 1, "baz": {"a": "baz-a", "b": "baz-b"}}}
     b = {"foo": {"x": 1, "biz": {"a": "biz-a", "b": "biz-b"}}}
 
     for l in classdiff.diff(a, b):
         print(l)
 
     print("-" * 40)
 
 
-def with_dict():
+def with_dict() -> None:
     class Bar:
         def __init__(self, b):
             self.a = "a"
             self.b = b
 
     class Foo:
         def __init__(self, n, b):
@@ -91,15 +134,15 @@
     result = classdiff.diff(Foo(43, "b"), Foo(44, "c"))
     for l in result:
         print(l)
 
     print("-" * 40)
 
 
-def with_dataclasses():
+def with_dataclasses() -> None:
     defined_in_code = SomeResource(
         name="my-data",
         price=2.3,
         quantity=4,
         dangerous=True,
         other=OtherClass(name="OA"),
         not_changed=OtherClass(name="Same"),
```

### Comparing `classdiff-0.1.1/classdiff/json.py` & `classdiff-0.2.0/classdiff/json.py`

 * *Files identical despite different names*

### Comparing `classdiff-0.1.1/classdiff/utils.py` & `classdiff-0.2.0/classdiff/utils.py`

 * *Files identical despite different names*

### Comparing `classdiff-0.1.1/pyproject.toml` & `classdiff-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "classdiff"
-version = "0.1.1"
+version = "0.2.0"
 description = "Utility to diff classes"
 authors = ["Validio <support@validio.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "classdiff"}]
 
 [tool.poetry.dependencies]
@@ -57,12 +57,12 @@
 "__init__.py" = [
     # We don't need docstrings in __init__
     "D104",
 ]
 
 # No need for documentation in binaries, examples or generated code
 "*/bin/*.py" = [ "D" ]
-"*/examples/*.py" = [ "D" ]
+"*/examples/*.py" = [ "D", "E741" ]
 "tests/*.py" = [ "D" ]
 
 [tool.ruff.pydocstyle]
 convention = "google"
```

