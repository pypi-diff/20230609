# Comparing `tmp/castepinput-0.1.6.tar.gz` & `tmp/castepinput-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/castepinput-0.1.6.tar", last modified: Wed Dec 23 20:48:58 2020, max compression
+gzip compressed data, was "castepinput-0.1.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `castepinput-0.1.6.tar` & `castepinput-0.1.8.tar`

### file list

```diff
@@ -1,21 +1,8 @@
-drwxr-xr-x   0 bonan     (1000) bonan     (1000)        0 2020-12-23 20:48:58.426898 castepinput-0.1.6/
--rw-r--r--   0 bonan     (1000) bonan     (1000)     3428 2020-12-23 20:48:58.425896 castepinput-0.1.6/PKG-INFO
--rw-r--r--   0 bonan     (1000) bonan     (1000)     2338 2020-12-23 19:18:15.000000 castepinput-0.1.6/README.md
-drwxr-xr-x   0 bonan     (1000) bonan     (1000)        0 2020-12-23 20:48:58.415691 castepinput-0.1.6/castepinput/
--rw-r--r--   0 bonan     (1000) bonan     (1000)      103 2020-12-23 19:18:15.000000 castepinput-0.1.6/castepinput/__init__.py
--rw-r--r--   0 bonan     (1000) bonan     (1000)     1853 2020-05-21 11:01:18.000000 castepinput-0.1.6/castepinput/common.py
--rw-r--r--   0 bonan     (1000) bonan     (1000)     6601 2020-12-23 19:18:15.000000 castepinput-0.1.6/castepinput/inputs.py
--rw-r--r--   0 bonan     (1000) bonan     (1000)     8966 2020-12-23 19:18:15.000000 castepinput-0.1.6/castepinput/parser.py
-drwxr-xr-x   0 bonan     (1000) bonan     (1000)        0 2020-12-23 20:48:58.425437 castepinput-0.1.6/castepinput/tests/
--rw-r--r--   0 bonan     (1000) bonan     (1000)        0 2020-05-21 11:01:18.000000 castepinput-0.1.6/castepinput/tests/__init__.py
--rw-r--r--   0 bonan     (1000) bonan     (1000)      963 2020-05-21 11:01:18.000000 castepinput-0.1.6/castepinput/tests/test_common.py
--rw-r--r--   0 bonan     (1000) bonan     (1000)     5735 2020-12-23 20:32:13.000000 castepinput-0.1.6/castepinput/tests/test_inputs.py
--rw-r--r--   0 bonan     (1000) bonan     (1000)     2422 2020-12-23 20:37:54.000000 castepinput-0.1.6/castepinput/tests/test_parser.py
-drwxr-xr-x   0 bonan     (1000) bonan     (1000)        0 2020-12-23 20:48:58.421908 castepinput-0.1.6/castepinput.egg-info/
--rw-r--r--   0 bonan     (1000) bonan     (1000)     3428 2020-12-23 20:48:58.000000 castepinput-0.1.6/castepinput.egg-info/PKG-INFO
--rw-r--r--   0 bonan     (1000) bonan     (1000)      411 2020-12-23 20:48:58.000000 castepinput-0.1.6/castepinput.egg-info/SOURCES.txt
--rw-r--r--   0 bonan     (1000) bonan     (1000)        1 2020-12-23 20:48:58.000000 castepinput-0.1.6/castepinput.egg-info/dependency_links.txt
--rw-r--r--   0 bonan     (1000) bonan     (1000)       28 2020-12-23 20:48:58.000000 castepinput-0.1.6/castepinput.egg-info/requires.txt
--rw-r--r--   0 bonan     (1000) bonan     (1000)       12 2020-12-23 20:48:58.000000 castepinput-0.1.6/castepinput.egg-info/top_level.txt
--rw-r--r--   0 bonan     (1000) bonan     (1000)       38 2020-12-23 20:48:58.426898 castepinput-0.1.6/setup.cfg
--rw-r--r--   0 bonan     (1000) bonan     (1000)     1701 2020-12-23 20:47:43.000000 castepinput-0.1.6/setup.py
+-rw-r--r--   0        0        0     1066 2023-06-08 23:22:56.711438 castepinput-0.1.8/LICENSE
+-rw-r--r--   0        0        0     2333 2023-06-08 23:22:56.711438 castepinput-0.1.8/README.md
+-rw-r--r--   0        0        0      173 2023-06-08 23:22:56.711438 castepinput-0.1.8/castepinput/__init__.py
+-rw-r--r--   0        0        0     1855 2023-06-08 23:22:56.711438 castepinput-0.1.8/castepinput/common.py
+-rw-r--r--   0        0        0     6991 2023-06-08 23:22:56.711438 castepinput-0.1.8/castepinput/inputs.py
+-rw-r--r--   0        0        0     9001 2023-06-08 23:22:56.711438 castepinput-0.1.8/castepinput/parser.py
+-rw-r--r--   0        0        0      832 2023-06-08 23:22:56.711438 castepinput-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3189 1970-01-01 00:00:00.000000 castepinput-0.1.8/PKG-INFO
```

### Comparing `castepinput-0.1.6/PKG-INFO` & `castepinput-0.1.8/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,82 +1,89 @@
 Metadata-Version: 2.1
 Name: castepinput
-Version: 0.1.6
-Summary: A general reader/writer for CASTEP inputs
-Home-page: https://github.com/zhubonan/castepinput
-Author: Bonan Zhu
-Author-email: zhubonan@outlook.com
-License: MIT License
-Description: A simple CASTEP input files parser/writer
-        ==========================
-        This package provide a basic framework for read/write input files of CASTEP.
-        There is already a excellent reader/writer implemented in [ase](https://gitlab.com/ase/ase) 
-        but they are ortentated to work with the `Atoms` and `Calculator` classes in `ase`. 
-        It also requires a CASTEP binary to exist to work.
-        This package aim to provide a more generic framework with minimum dependency for 
-        simple (but important) tasks of writing and reading inputs files of CASTEP.  
-        
-        
-        Usage
-        ------
-        The two classes to be used for reading/writing inputs are `ParamInput` and `CellInput`.
-        Keyword-value pairs can be set the same as dictionaries.
-        For example:
-        
-        ```python
-        from castepinput import CellInput, ParamInput, Block
-        # ParamInput is in fact just a subclass of OrderedDict
-        param = ParamInput(cut_off_energy=300, task="singlepoint")
-        param["opt_strategy"] = "speed"
-        
-        # Use the Block class to signal that it is a BLOCK
-        # The following line sets the positions_abs
-        cell = CellInput(positions_abs=Block(["C 0 0 0", "C 1 0 0"])
-        ```
-        
-        The two classes use simple string formatting when writing out the content.
-        See the following code as example.
-        ```python
-        cell = CellInput(snap_to_symmetry=True)
-        
-        # Should give 'snap_to_symmetry : True'
-        cell.get_string()
-        
-        # Should give 'symmetry_genreate : true'
-        cell['snap_to_symmetry'] = 'true'
-        cell.get_string()
-        
-        # Not all CASTEP keyword requires a value
-        # Use "" as the value will result just a keyword on a line
-        cell['symmetry_generate'] = ''
-        # Should give a string with a line 'symmetry_generate'
-        cell.get_string()
-        
-        # Set cell and positions use the set methods
-        cell.set_cell([10 ,10 , 10])
-        cell.set_positions(["O", "O"], [[0, 0, 0], [1.4, 0, 0]])
-        # Save to file
-        cell.save("O2.cell")
-        ```
-        
-        To initialize from a existing param/cell file, use the `ParamInput.from_file` method.
-        ```python
-        cell = CellInput.from_file("O2.cell")
-        # This should give [[10, 0, 0], [0, 10, 0], [0, 0, 10]]
-        cell.get_cell()
-        
-        # The value returned should be "" to be consistent with setting
-        cell["symmetry_generate"]
-        ```
-        
-        We also try to be smart and convert string into python types where it is possible.
-        Supported types are integer, floats and 1-d arrays made of integer/floats.
-        These coversions can be avoided by using `ParamInput.from_file(filename, plain=True)` when loading files.
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Version: 0.1.8
+Summary: Base module of castepinput
+Author-email: Bonan Zhu <zhubonan@outlook.com>
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 4 - Beta
-Description-Content-Type: text/markdown
-Provides-Extra: testing
+Requires-Dist: numpy
+Requires-Dist: pre-commit ; extra == "pre-commit"
+Requires-Dist: pylint-pytest ; extra == "pre-commit"
+Requires-Dist: pytest ; extra == "test"
+Requires-Dist: pytest-cov ; extra == "test"
+Requires-Dist: coverage ; extra == "test"
+Project-URL: Home, https://github.com/zhubonan/castepinput
+Provides-Extra: pre-commit
+Provides-Extra: test
+
+A simple CASTEP input files parser/writer
+==========================
+This package provide a basic framework for read/write input files of CASTEP.
+There is already a excellent reader/writer implemented in [ase](https://gitlab.com/ase/ase)
+but they are ortentated to work with the `Atoms` and `Calculator` classes in `ase`.
+It also requires a CASTEP binary to exist to work.
+This package aim to provide a more generic framework with minimum dependency for
+simple (but important) tasks of writing and reading inputs files of CASTEP.
+
+
+Usage
+------
+The two classes to be used for reading/writing inputs are `ParamInput` and `CellInput`.
+Keyword-value pairs can be set the same as dictionaries.
+For example:
+
+```python
+from castepinput import CellInput, ParamInput, Block
+# ParamInput is in fact just a subclass of OrderedDict
+param = ParamInput(cut_off_energy=300, task="singlepoint")
+param["opt_strategy"] = "speed"
+
+# Use the Block class to signal that it is a BLOCK
+# The following line sets the positions_abs
+cell = CellInput(positions_abs=Block(["C 0 0 0", "C 1 0 0"])
+```
+
+The two classes use simple string formatting when writing out the content.
+See the following code as example.
+```python
+cell = CellInput(snap_to_symmetry=True)
+
+# Should give 'snap_to_symmetry : True'
+cell.get_string()
+
+# Should give 'symmetry_genreate : true'
+cell['snap_to_symmetry'] = 'true'
+cell.get_string()
+
+# Not all CASTEP keyword requires a value
+# Use "" as the value will result just a keyword on a line
+cell['symmetry_generate'] = ''
+# Should give a string with a line 'symmetry_generate'
+cell.get_string()
+
+# Set cell and positions use the set methods
+cell.set_cell([10 ,10 , 10])
+cell.set_positions(["O", "O"], [[0, 0, 0], [1.4, 0, 0]])
+# Save to file
+cell.save("O2.cell")
+```
+
+To initialize from a existing param/cell file, use the `ParamInput.from_file` method.
+```python
+cell = CellInput.from_file("O2.cell")
+# This should give [[10, 0, 0], [0, 10, 0], [0, 0, 10]]
+cell.get_cell()
+
+# The value returned should be "" to be consistent with setting
+cell["symmetry_generate"]
+```
+
+We also try to be smart and convert string into python types where it is possible.
+Supported types are integer, floats and 1-d arrays made of integer/floats.
+These coversions can be avoided by using `ParamInput.from_file(filename, plain=True)` when loading files.
+
```

### Comparing `castepinput-0.1.6/README.md` & `castepinput-0.1.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 A simple CASTEP input files parser/writer
 ==========================
 This package provide a basic framework for read/write input files of CASTEP.
-There is already a excellent reader/writer implemented in [ase](https://gitlab.com/ase/ase) 
-but they are ortentated to work with the `Atoms` and `Calculator` classes in `ase`. 
+There is already a excellent reader/writer implemented in [ase](https://gitlab.com/ase/ase)
+but they are ortentated to work with the `Atoms` and `Calculator` classes in `ase`.
 It also requires a CASTEP binary to exist to work.
-This package aim to provide a more generic framework with minimum dependency for 
-simple (but important) tasks of writing and reading inputs files of CASTEP.  
+This package aim to provide a more generic framework with minimum dependency for
+simple (but important) tasks of writing and reading inputs files of CASTEP.
 
 
 Usage
 ------
 The two classes to be used for reading/writing inputs are `ParamInput` and `CellInput`.
 Keyword-value pairs can be set the same as dictionaries.
 For example:
```

### Comparing `castepinput-0.1.6/castepinput/common.py` & `castepinput-0.1.8/castepinput/common.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,39 +3,39 @@
 """
 from __future__ import division, print_function
 from __future__ import absolute_import
 from math import sin, cos, pi, sqrt
 
 import numpy as np
 
+# pylint: disable=invalid-name
+
 
 class FormatError(RuntimeError):
     pass
 
 
 class Block(list):
     """
     A class for blocks in CASTEP inputs files stored as a list of strings
     """
-
     def __repr__(self):
-        r = super(Block, self).__repr__()
-        return "Block(" + r + ")"
+        r = super().__repr__()
+        return 'Block(' + r + ')'
 
     def compact(self, inplace=False):
         """
         Remove any blank lines
         """
         f = [s.strip() for s in self if s]
         if inplace:
             del self[:]
             self.extend(f)
             return self
-        else:
-            return f
+        return f
 
 
 def cell_abcs_to_vec(abcs):
     """
     Convert fractional cell format to vectors.
     The result a vector is along [1, 0, 0] and the normal of a,b plane
     is along [0, 0, 1] direction.
```

### Comparing `castepinput-0.1.6/castepinput/inputs.py` & `castepinput-0.1.8/castepinput/inputs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 Classes for .param and .cell files
 """
-from __future__ import absolute_import
+import os
+import tempfile
+import re
 from collections import OrderedDict
+
 import numpy as np
 from .parser import Parser, PlainParser
 from .common import Block, cell_abcs_to_vec
-from six.moves import map
-from six.moves import zip
-
 
 
 class CastepInput(OrderedDict):
     """
     Class for storing key - values pairs of CASTEP inputs
     This class can be used for .param, .cell and also other CASTEP style
     inputs such as OptaDos's odi file
@@ -24,117 +24,123 @@
     to ``write`` function of a file-like object
 
     sepecial properties:
     * ``header`` a list of lines to be put into the header
     * ``units`` a dictionary of the units
     """
     def __init__(self, *args, **kwargs):
-        super(CastepInput, self).__init__(*args, **kwargs)
+        """Instantiate the object"""
+        super().__init__(*args, **kwargs)
         self.header = []
         self.units = {}
 
     def get_file_lines(self):
         """
         Return a list of strings to be write out to the files
         """
         lines = []
-        for h in self.header:
-            if not h.startswith("#"):
-                lines.append("# " + h)
+        for hline in self.header:
+            if not hline.startswith('#'):
+                lines.append('# ' + hline)
             else:
-                lines.append(h)
+                lines.append(hline)
 
         for key, value in self.items():
             if isinstance(value, Block):
-                lines.append("%BLOCK {}".format(key))
+                lines.append(f'%BLOCK {key}')
+                # Add units
                 if key in self.units:
-                    lines.append("{}".format(self.units[key]))
-                for v in value:
-                    lines.append(v)
-                lines.append("%ENDBLOCK {}".format(key))
+                    lines.append(str(self.units[key]))
+                # Append each line
+                for val in value:
+                    lines.append(val)
+                lines.append(f'%ENDBLOCK {key}\n')
             else:
                 # If a list/tuple is passed join into a string
                 if isinstance(value, (tuple, list)):
-                    value = " ".join(map(str, value))
-                if value is not None and value is not "":
-                    l = "{:<20}: {}".format(key, value)
+                    value = ' '.join(map(str, value))
+                # None and "" are treats as simple flag line e.g. SYMMETRY_GENERATE
+                if value is not None and value != '':
+                    this_line = f'{key:<20}: {value}'
                 else:
-                    l = key
+                    this_line = key
                 if key in self.units:
-                    l = l + " " + self.units[key]
-                lines.append(l)
+                    this_line = this_line + ' ' + self.units[key]
+                lines.append(this_line)
 
         return lines
 
     def get_string(self):
-        return "\n".join(self.get_file_lines())
+        """Return the string representing the input file"""
+        return '\n'.join(self.get_file_lines()) + '\n'
 
-    def save(self, fh):
-        with open(fh, "w") as fh:
-            fh.write(self.get_string())
+    def save(self, fname):
+        """Save the input as a file"""
+        with open(fname, 'w', encoding='utf-8') as fhandle:
+            fhandle.write(self.get_string())
 
     @classmethod
-    def from_file(cls, fn, plain=False):
+    def from_file(cls, fname, plain=False):
         """
         Constrant an instance from the file
         """
         out = cls()
-        out.load_file(fn, plain)
+        out.load_file(fname, plain)
         return out
 
-    def load_file(self, fn, plain=False):
+    def load_file(self, fname, plain=False):
         """
         Load from the file
         """
-        with open(fn) as fh:
-            lines = fh.readlines()
+        with open(fname, encoding='utf-8') as fhandle:
+            lines = fhandle.readlines()
         if plain:
-            p = PlainParser(lines)
+            parser = PlainParser(lines)
         else:
-            p = Parser(lines)
-        dict_out = p.get_dict()
+            parser = Parser(lines)
+        dict_out = parser.get_dict()
         for k, value in dict_out.items():
             self.__setitem__(k, value)
 
     def test_read_write(self, basic_input):
         """
         Adhoc test of readin and writing
         """
-        import tempfile
-        import os
-        outname = os.path.join(tempfile.mkdtemp(), "test.in")
+        outname = os.path.join(tempfile.mkdtemp(), 'test.in')
         self.save(outname)
         input2 = type(self)()
         input2.load_file(outname)
         assert dict(input2) == dict(basic_input)
 
 
 class ParamInput(CastepInput):
     pass
 
 
 class CellInput(CastepInput):
-
+    """
+    Representation for the content in `<seed>.cell` file.
+    """
     def get_cell(self):
         """Return cell vectors"""
 
         cell = []
-        if "lattice_cart" in self:
+        if 'lattice_cart' in self:
             cell_lines = self['lattice_cart']
 
-            for l in cell_lines:
-                cell.append([float(v) for v in l.split()])
+            for line in cell_lines:
+                cell.append([float(val) for val in line.split()])
 
-        elif "lattice_abc" in self:
+        elif 'lattice_abc' in self:
             abc_lines = self['lattice_abc']
 
             abc = []
-            for l in abc_lines:
-                abc.extend([float(v) for v in l.split()])
-            assert len(abc) == 6, "Problem in lattice_abc block"
+            for line in abc_lines:
+                abc.extend([float(val) for val in line.split()])
+            assert len(abc) == 6, 'Problem in lattice_abc block'
 
             cell = cell_abcs_to_vec(abc)
 
         return np.asarray(cell)
 
     def get_positions(self):
         """
@@ -146,95 +152,89 @@
         """
         is_frac = False
         pos_lines = self.get('positions_abs')
         if not pos_lines:
             pos_lines = self.get('positions_frac')
             is_frac = True
         if not pos_lines:
-            raise RuntimeError("No positions defined")
-
+            raise RuntimeError('No positions defined')
 
         elems = []
         pos = []
         tags = []
-        for l in pos_lines:
-            e, p, t = parse_pos_line(l)
-            elems.append(e)
-            pos.append(p)
-            tags.append(t)
+        for line in pos_lines:
+            elem, parser, tag = parse_pos_line(line)
+            elems.append(elem)
+            pos.append(parser)
+            tags.append(tag)
 
         pos = np.array(pos)
 
         if is_frac:
             # We need to multiple the positions with cells
             cell = self.get_cell()
             pos = np.dot(cell, pos.T).T
 
         return elems, pos, tags
 
-
     def set_cell(self, cell):
         """
         Set cell. Accept a length 3 list/array or 3x3 list/array.
         """
         cell_lines = Block()
         cell = np.asarray(cell)
-        if cell.shape == (3,):
+        if cell.shape == (3, ):
             cell = np.diag(cell)
         if cell.shape != (3, 3):
-            raise ValueError("Cell must be a 3x3 matrix. But {} is given".format(cell))
-
-        for x in cell:
-            cell_lines.append("{:.10f}  {:.10f}  {:.10f}".format(*x))
+            raise ValueError(f'Cell must be a 3x3 matrix. But {cell} is given')
 
-        self.__setitem__("lattice_cart", Block(cell_lines))
+        for coord in cell:
+            cell_lines.append(
+                f'{coord[0]:.10f}  {coord[1]:.10f}  {coord[2]:.10f}')
 
+        self['lattice_cart'] = Block(cell_lines)
 
     def set_positions(self, elements, positions, tags=None, frac=False):
         """
         Set positions
         """
         if frac:
-            bname = "positions_frac"
+            bname = 'positions_frac'
         else:
-            bname = "positions_abs"
+            bname = 'positions_abs'
 
         pos_lines = Block()
         if not tags:
-            tags = [""] * len(elements)
-        for e, p, t in zip(elements, positions, tags):
-            pos_lines.append(construct_pos_line(e, p, t))
+            tags = [''] * len(elements)
+        for elem, parser, tag in zip(elements, positions, tags):
+            pos_lines.append(construct_pos_line(elem, parser, tag))
 
-        self.__setitem__(bname, Block(pos_lines))
+        self[bname] = Block(pos_lines)
 
 
 def parse_pos_line(cell_line):
     """
     Parse single line in the cell block.
     Return element, coorindates and a dictionary of tags
     """
 
-    import re
     cell_line = cell_line.strip()
-    s = re.split(r"[\s]+", cell_line, maxsplit=4)
-    if len(s) < 4:
-        raise ValueError("Cannot understand line: {}".format(cell_line))
-    if len(s) == 5:
-        tags = s[-1]
+    tokens = re.split(r'[\s]+', cell_line, maxsplit=4)
+    if len(tokens) < 4:
+        raise ValueError(f'Cannot understand line: {cell_line}')
+    # There are trailing tags here
+    if len(tokens) == 5:
+        tags = tokens[-1]
     else:
-        tags = ""
+        tags = ''
 
-    elem = s[0].capitalize()
-    coor = list(map(float, s[1:4]))
+    elem = tokens[0].capitalize()
+    coor = list(map(float, tokens[1:4]))
 
     return elem, coor, tags
 
 
 def construct_pos_line(elem, coor, tags):
     """
     Do the opposite of the parse_pos_line
     """
-    line = "{elem}  {x:.10f} {y:.10f} {z:.10f} {tags}"
-
-    return line.format(elem=elem, x=coor[0], y=coor[1], z=coor[2],
-                       tags=tags)
-
+    return f'{elem}  {coor[0]:.10f} {coor[1]:.10f} {coor[2]:.10f} {tags}'
```

### Comparing `castepinput-0.1.6/castepinput/parser.py` & `castepinput-0.1.8/castepinput/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,52 +7,45 @@
 CASTEP input does not destinguish between low and upper case, but python does.
 To stardardise data parsed. Output follows the convension
 1. all keys will be in lower case
 2. all block names will be in lower case
 3. case of the values themselves are not affected
 4. content of the blocks are not affected
 """
-
-from __future__ import print_function
-from __future__ import division
-
-from __future__ import absolute_import
 import re
 from .common import Block, FormatError
-from six.moves import map
 
-COMMENT_SYMBOLS = ["#", "!"]
+COMMENT_SYMBOLS = ('#', '!')
 
 # RE for separating blocks
-block_start = re.compile(r"%block (\w+)", flags=re.IGNORECASE)
-block_finish = re.compile(r"%endblock (\w+)", flags=re.IGNORECASE)
-kw_split = re.compile(r"[ \t:=]+")
+block_start = re.compile(r'%block (\w+)', flags=re.IGNORECASE)
+block_finish = re.compile(r'%endblock (\w+)', flags=re.IGNORECASE)
+kw_split = re.compile(r'[ \t:=]+')
 
 
-class PlainParser(object):
+class PlainParser:
     """
     Base parser class
     Does nothing fancy, basic text processing
     """
-
     def __init__(self, lines):
         """
         Parser for cell/param files for castep.
         May also be useful for OptaDos/CASTEPConv that shares similar
         format.
         Parameters:
         :params lines: A list of the file content or name of a file to be read
         """
 
         if isinstance(lines, (list, tuple)):
             self._raw_lines = lines  # Raw input lines
         else:
-            with open(lines) as fh:
+            with open(lines, encoding='utf-8') as fhandle:
                 lin = []
-                for line in fh:
+                for line in fhandle:
                     lin.append(line.strip())
             self._raw_lines = lin
 
         self._lines = []  # Processed lines
         self._kwlines = []  # key-value paired lines
         self._blocks = {}  # A dictionary of blocks
         self._keywords = {}  # A dictionary of key value pairs
@@ -70,17 +63,16 @@
     def content(self):
         """A list of lines as inputs for parsing"""
         return self._raw_lines
 
     @property
     def comments(self):
         if self._comments is None:
-            raise RuntimeError("File is not parsed")
-        else:
-            return self._comments
+            raise RuntimeError('File is not parsed')
+        return self._comments
 
     def _clean_up_lines(self):
         """
         Filter out comments
         Save cleaned lines in self._lines and
         comments in self._comments
         Make everything not comment in lower case
@@ -97,22 +89,21 @@
 
             # We first check for comment
             if line[0] in COMMENT_SYMBOLS:
                 comments.append(line[1:].strip())
                 continue
 
             # Check if there is any trailing comments
-            for s in COMMENT_SYMBOLS:
-                pos = line.find(s)
+            for symbol in COMMENT_SYMBOLS:
+                pos = line.find(symbol)
                 if pos != -1:
                     comments.append(line[pos + 1:].strip())
                     cld_line = line[:pos].strip()  # Remove trailing space
                     break
-                else:
-                    cld_line = line
+                cld_line = line
             cleaned_lines.append(cld_line)
 
         self._lines = cleaned_lines
         self._comments = comments
         return cleaned_lines, comments
 
     def _split_block_kw(self):
@@ -131,43 +122,42 @@
         kwlines = []
         start_name = None
         for i, line in enumerate(self._lines):
 
             start_match = block_start.match(line)
             if start_match:
                 if in_block is True:
-                    raise FormatError("End of block {}"
-                                      " is not detected".format(start_name))
+                    raise FormatError(f'End of block {start_name}'
+                                      ' is not detected')
                 start = i
                 in_block = True
                 start_name = start_match.group(1).lower()
                 continue
 
             end_match = block_finish.match(line)
             if end_match:
                 finish = i
                 end_name = end_match.group(1).lower()
                 if in_block is False:
-                    raise FormatError("Start of block {} not"
-                                      " found".format(end_name))
-                elif end_name != start_name:
-                    raise FormatError("Mismatch block names, start: {}"
-                                      " finish: {}".format(
-                                          start_name, end_name))
-                else:
-                    block_indices[start_name] = (start, finish)
-                    in_block = False
+                    raise FormatError(f'Start of block {end_name} not'
+                                      ' found')
+                if end_name != start_name:
+                    raise FormatError(
+                        f'Mismatch block names, start: {start_name}'
+                        f' finish: {end_name}')
+                # Push the content of the push into the main container
+                block_indices[start_name] = (start, finish)
+                in_block = False
                 continue
 
             if not in_block:
                 kwlines.append(line)
 
         if in_block is True:
-            raise FormatError("End of block {}"
-                              " not detected".format(start_name))
+            raise FormatError(f'End of block {start_name}' ' not detected')
 
         # Now extract block contents
         blocks = {}
         for key, index in block_indices.items():
             lines = self._lines[index[0] + 1:index[1]]
             blocks[key.lower()] = Block(lines)
 
@@ -175,25 +165,25 @@
         self._kwlines = kwlines
         return blocks, kwlines
 
     def _parse_keywords(self):
         """Parse keyword, value pairs"""
         out_dict = {}
         for line in self._kwlines:
-            s = kw_split.split(line, 1)
-            if len(s) == 2:
-                key, value = s
-            elif len(s) == 1:
-                key = s[0]
-                value = ""  # Empty string for key without values
+            tokens = kw_split.split(line, 1)
+            if len(tokens) == 2:
+                key, value = tokens
+            elif len(tokens) == 1:
+                key = tokens[0]
+                value = ''  # Empty string for key without values
             else:
-                raise FormatError("Cannot parse into key-value"
-                                  " pair {}".format(line))
+                raise FormatError(
+                    f'Cannot parse into key-value pair in: {line}')
             if not value:
-                value = ""
+                value = ''
 
             out_dict[key.lower()] = value
         self._keywords = out_dict
         return out_dict
 
     def get_dict(self):
         """
@@ -209,106 +199,112 @@
 
 class Parser(PlainParser):
     """
     General parser class
     Try to convert data types
     bool >> int >> float >> plain text
     """
-    _CONVERT_TYPE = True
-
     def __init__(self, lines, convert_type=True):
         """
         Initialize the parser by passing either:
         - A list of lines to be parsed
         - A path to the file to be parsed
 
         :param convert_type: Either try to convert the types or not
         """
-        super(Parser, self).__init__(lines)
-        self._CONVERT_TYPE = convert_type
+        super().__init__(lines)
+        self._convert_type = convert_type
 
     def parse(self):
         """
         Parse the contents
         Also will try to convert the types if requested
         """
-        super(Parser, self).parse()
-        if self._CONVERT_TYPE is False:
+        super().parse()
+        if self._convert_type is False:
             return self._keywords
 
         old_keywords = self._keywords
 
         new_keywords = {}
         for key, value in old_keywords.items():
             new_keywords[key] = convert_type_kw(value, key)
 
         self._keywords = new_keywords
+        return None
 
 
-class CannotConverError(ValueError):
+class CannotConvertError(ValueError):
     pass
 
 
-class Converter(object):
+class Converter:
     """
     Class for convert that convert types
     """
     ACCEPTED_ERRORS = (ValueError, )
 
     def __init__(self, func):
         """
         Initialized by passing the conversion function
         """
         self.convert_func = func
 
     def convert(self, value):
+        """
+        Convert a string into python object
+
+        Return a tuple of (success, output)
+        """
+
         assert isinstance(value, str)
         try:
             out = self.convert_func(value)
         except self.ACCEPTED_ERRORS:
             success = False
             out = value
         else:
             success = True
 
         return success, out
 
 
 def booltest(value):
-    if value.lower().strip() == "true":
+    """Test if a string value is a Bool"""
+    if value.lower().strip() == 'true':
         return True
-    elif value.lower().strip() == "false":
+    if value.lower().strip() == 'false':
         return False
-    else:
-        raise CannotConverError
+    raise CannotConvertError
 
 
 def emptystrtest(value):
     """Rule for empty string to be empty string"""
-    if value == "":
+    if value == '':
         return value
-    else:
-        raise CannotConverError
+    raise CannotConvertError
 
 
 intconv = Converter(int)
 floatconv = Converter(float)
 intarrayconv = Converter(lambda x: list(map(int, x.split())))
 floatarrayconv = Converter(lambda x: list(map(float, x.split())))
 boolconv = Converter(booltest)
 emptyconv = Converter(emptystrtest)
 
 
 def convert_type_kw(value, key=None):
     """
     Try to convert type of the value
     """
+    # the key argument is not used for now - reserve for per-key treatment
+    _ = key
 
-    # Check if it is bool
+    # Note that the order of which these converters are call matters
     convs = [
         emptyconv, boolconv, intconv, floatconv, intarrayconv, floatarrayconv
     ]
-    for c in convs:
-        success, out = c.convert(value)
+    for converter in convs:
+        success, out = converter.convert(value)
         if success:
             return out
     return value
```

