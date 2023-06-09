# Comparing `tmp/kiutils-1.4.1.tar.gz` & `tmp/kiutils-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiutils-1.4.1.tar", last modified: Sat Apr 22 16:16:26 2023, max compression
+gzip compressed data, was "kiutils-1.4.2.tar", last modified: Fri Jun  9 19:17:39 2023, max compression
```

## Comparing `kiutils-1.4.1.tar` & `kiutils-1.4.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 16:16:26.185885 kiutils-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-22 16:16:01.000000 kiutils-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-22 16:16:26.185885 kiutils-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-04-22 16:16:01.000000 kiutils-1.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-22 16:16:01.000000 kiutils-1.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-22 16:16:26.185885 kiutils-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-22 16:16:01.000000 kiutils-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 16:16:26.181885 kiutils-1.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 16:16:26.181885 kiutils-1.4.1/src/kiutils/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-22 16:16:01.000000 kiutils-1.4.1/src/kiutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14176 2023-04-22 16:16:01.000000 kiutils-1.4.1/src/kiutils/board.py
--rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-04-22 16:16:01.000000 kiutils-1.4.1/src/kiutils/dru.py
--rw-r--r--   0 runner    (1001) docker     (123)    46972 2023-04-22 16:16:01.000000 kiutils-1.4.1/src/kiutils/footprint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 16:16:26.181885 kiutils-1.4.1/src/kiutils/items/
--rw-r--r--   0 runner    (1001) docker     (123)    47460 2023-04-22 16:16:01.000000 kiutils-1.4.1/src/kiutils/items/brditems.py
--rw-r--r--   0 runner    (1001) docker     (123)    42864 2023-04-22 16:16:01.000000 kiutils-1.4.1/src/kiutils/items/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    13609 2023-04-22 16:16:01.000000 kiutils-1.4.1/src/kiutils/items/dimensions.py
--rw-r--r--   0 runner    (1001) docker     (123)    34336 2023-04-22 16:16:01.000000 kiutils-1.4.1/src/kiutils/items/fpitems.py
--rw-r--r--   0 runner    (1001) docker     (123)    31527 2023-04-22 16:16:01.000000 kiutils-1.4.1/src/kiutils/items/gritems.py
--rw-r--r--   0 runner    (1001) docker     (123)    72965 2023-04-22 16:16:01.000000 kiutils-1.4.1/src/kiutils/items/schitems.py
--rw-r--r--   0 runner    (1001) docker     (123)    21590 2023-04-22 16:16:01.000000 kiutils-1.4.1/src/kiutils/items/syitems.py
--rw-r--r--   0 runner    (1001) docker     (123)    27998 2023-04-22 16:16:01.000000 kiutils-1.4.1/src/kiutils/items/zones.py
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-04-22 16:16:01.000000 kiutils-1.4.1/src/kiutils/libraries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 16:16:26.185885 kiutils-1.4.1/src/kiutils/misc/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-22 16:16:01.000000 kiutils-1.4.1/src/kiutils/misc/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14321 2023-04-22 16:16:01.000000 kiutils-1.4.1/src/kiutils/schematic.py
--rw-r--r--   0 runner    (1001) docker     (123)    25567 2023-04-22 16:16:01.000000 kiutils-1.4.1/src/kiutils/symbol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 16:16:26.185885 kiutils-1.4.1/src/kiutils/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-22 16:16:01.000000 kiutils-1.4.1/src/kiutils/utils/sexpr.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-22 16:16:01.000000 kiutils-1.4.1/src/kiutils/utils/strings.py
--rw-r--r--   0 runner    (1001) docker     (123)    38203 2023-04-22 16:16:01.000000 kiutils-1.4.1/src/kiutils/wks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 16:16:26.181885 kiutils-1.4.1/src/kiutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-22 16:16:26.000000 kiutils-1.4.1/src/kiutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-22 16:16:26.000000 kiutils-1.4.1/src/kiutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 16:16:26.000000 kiutils-1.4.1/src/kiutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-22 16:16:26.000000 kiutils-1.4.1/src/kiutils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 16:16:26.185885 kiutils-1.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-04-22 16:16:01.000000 kiutils-1.4.1/tests/test_board.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-22 16:16:01.000000 kiutils-1.4.1/tests/test_designrules.py
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-04-22 16:16:01.000000 kiutils-1.4.1/tests/test_footprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-22 16:16:01.000000 kiutils-1.4.1/tests/test_libtable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-22 16:16:01.000000 kiutils-1.4.1/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-04-22 16:16:01.000000 kiutils-1.4.1/tests/test_schematic.py
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-04-22 16:16:01.000000 kiutils-1.4.1/tests/test_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-22 16:16:01.000000 kiutils-1.4.1/tests/test_worksheets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-04-22 16:16:01.000000 kiutils-1.4.1/tests/testfunctions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:17:39.747579 kiutils-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-06-09 19:17:12.000000 kiutils-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-06-09 19:17:39.747579 kiutils-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-09 19:17:12.000000 kiutils-1.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-09 19:17:12.000000 kiutils-1.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-09 19:17:39.747579 kiutils-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-09 19:17:12.000000 kiutils-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:17:39.739578 kiutils-1.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:17:39.743578 kiutils-1.4.2/src/kiutils/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-09 19:17:12.000000 kiutils-1.4.2/src/kiutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14176 2023-06-09 19:17:12.000000 kiutils-1.4.2/src/kiutils/board.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-06-09 19:17:12.000000 kiutils-1.4.2/src/kiutils/dru.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46972 2023-06-09 19:17:12.000000 kiutils-1.4.2/src/kiutils/footprint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:17:39.743578 kiutils-1.4.2/src/kiutils/items/
+-rw-r--r--   0 runner    (1001) docker     (123)    47460 2023-06-09 19:17:12.000000 kiutils-1.4.2/src/kiutils/items/brditems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42864 2023-06-09 19:17:12.000000 kiutils-1.4.2/src/kiutils/items/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13609 2023-06-09 19:17:12.000000 kiutils-1.4.2/src/kiutils/items/dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34336 2023-06-09 19:17:12.000000 kiutils-1.4.2/src/kiutils/items/fpitems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31527 2023-06-09 19:17:12.000000 kiutils-1.4.2/src/kiutils/items/gritems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75394 2023-06-09 19:17:12.000000 kiutils-1.4.2/src/kiutils/items/schitems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21590 2023-06-09 19:17:12.000000 kiutils-1.4.2/src/kiutils/items/syitems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27998 2023-06-09 19:17:12.000000 kiutils-1.4.2/src/kiutils/items/zones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-06-09 19:17:12.000000 kiutils-1.4.2/src/kiutils/libraries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:17:39.743578 kiutils-1.4.2/src/kiutils/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-09 19:17:12.000000 kiutils-1.4.2/src/kiutils/misc/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14716 2023-06-09 19:17:12.000000 kiutils-1.4.2/src/kiutils/schematic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25567 2023-06-09 19:17:12.000000 kiutils-1.4.2/src/kiutils/symbol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:17:39.743578 kiutils-1.4.2/src/kiutils/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-09 19:17:12.000000 kiutils-1.4.2/src/kiutils/utils/sexpr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-09 19:17:12.000000 kiutils-1.4.2/src/kiutils/utils/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38203 2023-06-09 19:17:12.000000 kiutils-1.4.2/src/kiutils/wks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:17:39.743578 kiutils-1.4.2/src/kiutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-06-09 19:17:39.000000 kiutils-1.4.2/src/kiutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-09 19:17:39.000000 kiutils-1.4.2/src/kiutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 19:17:39.000000 kiutils-1.4.2/src/kiutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-09 19:17:39.000000 kiutils-1.4.2/src/kiutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:17:39.747579 kiutils-1.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-06-09 19:17:12.000000 kiutils-1.4.2/tests/test_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-09 19:17:12.000000 kiutils-1.4.2/tests/test_designrules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-06-09 19:17:12.000000 kiutils-1.4.2/tests/test_footprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-09 19:17:12.000000 kiutils-1.4.2/tests/test_libtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-09 19:17:12.000000 kiutils-1.4.2/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-06-09 19:17:12.000000 kiutils-1.4.2/tests/test_schematic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-06-09 19:17:12.000000 kiutils-1.4.2/tests/test_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-09 19:17:12.000000 kiutils-1.4.2/tests/test_worksheets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-06-09 19:17:12.000000 kiutils-1.4.2/tests/testfunctions.py
```

### Comparing `kiutils-1.4.1/LICENSE` & `kiutils-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.1/PKG-INFO` & `kiutils-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiutils
-Version: 1.4.1
+Version: 1.4.2
 Summary: Simple and SCM-friendly KiCad file parser for KiCad 6.0 and up
 Home-page: https://github.com/mvnmgrx/kiutils
 Author: Marvin Mager
 Author-email: 99667992+mvnmgrx@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/mvnmgrx/kiutils/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `kiutils-1.4.1/README.md` & `kiutils-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.1/setup.cfg` & `kiutils-1.4.2/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = kiutils
-version = 1.4.1
+version = 1.4.2
 author = Marvin Mager
 author_email = 99667992+mvnmgrx@users.noreply.github.com
 description = Simple and SCM-friendly KiCad file parser for KiCad 6.0 and up
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mvnmgrx/kiutils
 project_urls =
```

### Comparing `kiutils-1.4.1/src/kiutils/board.py` & `kiutils-1.4.2/src/kiutils/board.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.1/src/kiutils/dru.py` & `kiutils-1.4.2/src/kiutils/dru.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.1/src/kiutils/footprint.py` & `kiutils-1.4.2/src/kiutils/footprint.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.1/src/kiutils/items/brditems.py` & `kiutils-1.4.2/src/kiutils/items/brditems.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.1/src/kiutils/items/common.py` & `kiutils-1.4.2/src/kiutils/items/common.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.1/src/kiutils/items/dimensions.py` & `kiutils-1.4.2/src/kiutils/items/dimensions.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.1/src/kiutils/items/fpitems.py` & `kiutils-1.4.2/src/kiutils/items/fpitems.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.1/src/kiutils/items/gritems.py` & `kiutils-1.4.2/src/kiutils/items/gritems.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.1/src/kiutils/items/schitems.py` & `kiutils-1.4.2/src/kiutils/items/schitems.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,14 +210,79 @@
         expression += self.stroke.to_sexpr(indent+2)
         if self.uuid is not None:
             expression += f'{indents}  (uuid {self.uuid})\n'
         expression += f'{indents}){endline}'
         return expression
 
 @dataclass
+class BusAlias():
+    """The ``bus_alias`` token defines a bus entry in the schematic
+
+    Documentation:
+        https://gitlab.com/kicad/services/kicad-dev-docs/-/merge_requests/53/diffs
+    """
+
+    name: str = ""
+    """The ``name`` of the bus."""
+
+    members: List[str] = field(default_factory=list)
+    """The list of ``members`` defined in the bus. Note that when you tap out a bus entry
+    from a bus using one these members a label will be created with the selected member name"""
+
+    @classmethod
+    def from_sexpr(cls, exp: list) -> BusAlias:
+        """Convert the given S-Expresstion into a BusAlias object
+
+        Args:
+            - exp (list): Part of parsed S-Expression ``(bus_alias ...)``
+
+        Raises:
+            - Exception: When given parameter's type is not a list
+            - Exception: When the first item of the list is not bus_alias
+            - Exception: When the S-Expression is not exactly three items long
+            - Exception: When the ``members`` token is missing
+
+        Returns:
+            - BusAlias: Object of the class initialized with the given S-Expression
+        """
+        if not isinstance(exp, list):
+            raise Exception("Expression does not have the correct type")
+
+        if exp[0] != 'bus_alias':
+            raise Exception("Expression does not have the correct type")
+
+        if len(exp) != 3:
+            raise Exception("Exactly three items are expected in a bus_alias S-Expression.")
+        
+        if not isinstance(exp[2], list) or exp[2][0] != 'members':
+            raise Exception("bus_alias needs to contain a list of members")
+        
+        object = cls()
+        object.name = exp[1]
+        object.members = [x for x in exp[2][1:]]
+        return object
+
+    def to_sexpr(self, indent=2, newline=True) -> str:
+        """Generate the S-Expression representing this object
+
+        Args:
+            - indent (int): Number of whitespaces used to indent the output. Defaults to 2.
+            - newline (bool): Adds a newline to the end of the output. Defaults to True.
+
+        Returns:
+            - str: S-Expression of this object
+        """
+        indents = ' '*indent
+        endline = '\n' if newline else ''
+
+        members = [f'"{dequote(member)}"' for member in self.members]
+        expression =  f'{indents}(bus_alias "{dequote(self.name)}" (members {" ".join(members)})){endline}'
+        return expression
+
+@dataclass
 class Connection():
     """The ``wire`` and ``bus`` tokens define wires and buses in the schematic
 
     Documentation:
         https://dev-docs.kicad.org/en/file-formats/sexpr-schematic/#_wire_and_bus_section
     """
```

### Comparing `kiutils-1.4.1/src/kiutils/items/syitems.py` & `kiutils-1.4.2/src/kiutils/items/syitems.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.1/src/kiutils/items/zones.py` & `kiutils-1.4.2/src/kiutils/items/zones.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.1/src/kiutils/libraries.py` & `kiutils-1.4.2/src/kiutils/libraries.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.1/src/kiutils/schematic.py` & `kiutils-1.4.2/src/kiutils/schematic.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,17 @@
 
     noConnects: List[NoConnect] = field(default_factory=list)
     """The ``noConnect`` token defines a list of no_connect markers used in the schematic"""
 
     busEntries: List[BusEntry] = field(default_factory=list)
     """The ``busEntries`` token defines a list of bus_entry used in the schematic"""
 
+    busAliases: List[BusAlias] = field(default_factory=list)
+    """The ``busAliases`` token defines a list of bus_alias used in the schematic"""
+
     graphicalItems: List[Union[Connection, PolyLine]] = field(default_factory=list)
     """The ``graphicalItems`` token defines a list of ``bus``, ``wire`` or ``polyline`` elements 
     used in the schematic"""
 
     shapes: List[Union[Arc, Circle, Rectangle]] = field(default_factory=list)
     """The ``shapes`` token defines a list of graphical shapes (``Arc``, ``Rectangle`` or 
     ``Circle``) used in the schematic.
@@ -140,14 +143,15 @@
             if item[0] == 'title_block': object.titleBlock = TitleBlock().from_sexpr(item)
             if item[0] == 'lib_symbols':
                 for symbol in item[1:]:
                     object.libSymbols.append(Symbol().from_sexpr(symbol))
             if item[0] == 'junction': object.junctions.append(Junction().from_sexpr(item))
             if item[0] == 'no_connect': object.noConnects.append(NoConnect().from_sexpr(item))
             if item[0] == 'bus_entry': object.busEntries.append(BusEntry().from_sexpr(item))
+            if item[0] == 'bus_alias': object.busAliases.append(BusAlias().from_sexpr(item))
             if item[0] == 'wire': object.graphicalItems.append(Connection().from_sexpr(item))
             if item[0] == 'bus': object.graphicalItems.append(Connection().from_sexpr(item))
             if item[0] == 'polyline': object.graphicalItems.append(PolyLine().from_sexpr(item))
             if item[0] == 'arc': object.shapes.append(Arc.from_sexpr(item))
             if item[0] == 'circle': object.shapes.append(Circle.from_sexpr(item))
             if item[0] == 'rectangle': object.shapes.append(Rectangle.from_sexpr(item))
             if item[0] == 'image': object.images.append(Image().from_sexpr(item))
@@ -265,14 +269,19 @@
                 expression += item.to_sexpr(indent+2)
 
         if self.busEntries:
             expression += '\n'
             for item in self.busEntries:
                 expression += item.to_sexpr(indent+2)
 
+        if self.busAliases:
+            expression += '\n'
+            for item in self.busAliases:
+                expression += item.to_sexpr(indent+2)
+
         if self.graphicalItems:
             expression += '\n'
             for item in self.graphicalItems:
                 expression += item.to_sexpr(indent+2)
 
         if self.shapes:
             expression += '\n'
```

### Comparing `kiutils-1.4.1/src/kiutils/symbol.py` & `kiutils-1.4.2/src/kiutils/symbol.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.1/src/kiutils/utils/sexpr.py` & `kiutils-1.4.2/src/kiutils/utils/sexpr.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.1/src/kiutils/utils/strings.py` & `kiutils-1.4.2/src/kiutils/utils/strings.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.1/src/kiutils/wks.py` & `kiutils-1.4.2/src/kiutils/wks.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.1/src/kiutils.egg-info/PKG-INFO` & `kiutils-1.4.2/src/kiutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiutils
-Version: 1.4.1
+Version: 1.4.2
 Summary: Simple and SCM-friendly KiCad file parser for KiCad 6.0 and up
 Home-page: https://github.com/mvnmgrx/kiutils
 Author: Marvin Mager
 Author-email: 99667992+mvnmgrx@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/mvnmgrx/kiutils/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `kiutils-1.4.1/src/kiutils.egg-info/SOURCES.txt` & `kiutils-1.4.2/src/kiutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.1/tests/test_board.py` & `kiutils-1.4.2/tests/test_board.py`

 * *Files 6% similar despite different names*

```diff
@@ -88,14 +88,22 @@
     def test_pcbPlotParams(self):
         """Tests the parsing of board plot params"""
         self.testData.compareToTestFile = True
         self.testData.pathToTestFile = path.join(BOARD_BASE, 'test_pcbPlotParams')
         board = Board().from_file(self.testData.pathToTestFile)
         self.assertTrue(to_file_and_compare(board, self.testData))
 
+    def test_zoneOnOuterLayersOnly(self):
+        """Tests the parsing of a zone that is only on the outer board layers (F.Cu and B.Cu). 
+        Regression test for bug in PR #89."""
+        self.testData.compareToTestFile = True
+        self.testData.pathToTestFile = path.join(BOARD_BASE, 'test_zoneOnOuterLayersOnly')
+        board = Board().from_file(self.testData.pathToTestFile)
+        self.assertTrue(to_file_and_compare(board, self.testData))
+
 class Tests_Board_Since_V7(unittest.TestCase):
     """Test cases for Boards since KiCad 7"""
 
     def setUp(self) -> None:
         prepare_test(self)
         return super().setUp()
```

### Comparing `kiutils-1.4.1/tests/test_designrules.py` & `kiutils-1.4.2/tests/test_designrules.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.1/tests/test_footprint.py` & `kiutils-1.4.2/tests/test_footprint.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.1/tests/test_libtable.py` & `kiutils-1.4.2/tests/test_libtable.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.1/tests/test_misc.py` & `kiutils-1.4.2/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.1/tests/test_schematic.py` & `kiutils-1.4.2/tests/test_schematic.py`

 * *Files 4% similar despite different names*

```diff
@@ -157,7 +157,15 @@
     def test_strokeOptionalTokens(self):
         """Tests the parsing of the optional tokens on strokes since KiCad v7.
         Came up in PR #73."""
         self.testData.compareToTestFile = True
         self.testData.pathToTestFile = path.join(SCHEMATIC_BASE, 'since_v7', 'test_strokeOptionalTokens')
         schematic = Schematic().from_file(self.testData.pathToTestFile)
         self.assertTrue(to_file_and_compare(schematic, self.testData))
+
+    def test_busAliases(self):
+        """Tests the parsing of bus aliases since KiCad v7.
+        Came up in PR #92."""
+        self.testData.compareToTestFile = True
+        self.testData.pathToTestFile = path.join(SCHEMATIC_BASE, 'since_v7', 'test_busAliases')
+        schematic = Schematic().from_file(self.testData.pathToTestFile)
+        self.assertTrue(to_file_and_compare(schematic, self.testData))
```

### Comparing `kiutils-1.4.1/tests/test_symbol.py` & `kiutils-1.4.2/tests/test_symbol.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.1/tests/test_worksheets.py` & `kiutils-1.4.2/tests/test_worksheets.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.1/tests/testfunctions.py` & `kiutils-1.4.2/tests/testfunctions.py`

 * *Files identical despite different names*

