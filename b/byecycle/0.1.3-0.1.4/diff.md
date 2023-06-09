# Comparing `tmp/byecycle-0.1.3.tar.gz` & `tmp/byecycle-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byecycle-0.1.3.tar", last modified: Thu Jun  1 15:08:35 2023, max compression
+gzip compressed data, was "byecycle-0.1.4.tar", last modified: Fri Jun  9 15:40:06 2023, max compression
```

## Comparing `byecycle-0.1.3.tar` & `byecycle-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1069 2023-06-01 15:07:04.217387 byecycle-0.1.3/LICENSE
--rw-r--r--   0        0        0     4870 2023-06-01 15:07:04.217387 byecycle-0.1.3/README.md
--rw-r--r--   0        0        0     1651 2023-06-01 15:08:35.780552 byecycle-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      147 2023-06-01 15:07:04.221387 byecycle-0.1.3/src/byecycle/__init__.py
--rw-r--r--   0        0        0       79 2023-06-01 15:07:04.221387 byecycle-0.1.3/src/byecycle/__main__.py
--rw-r--r--   0        0        0     4097 2023-06-01 15:07:04.221387 byecycle-0.1.3/src/byecycle/cli.py
--rw-r--r--   0        0        0     2583 2023-06-01 15:07:04.221387 byecycle-0.1.3/src/byecycle/draw/__init__.py
--rw-r--r--   0        0        0    12763 2023-06-01 15:07:04.221387 byecycle-0.1.3/src/byecycle/graph.py
--rw-r--r--   0        0        0     8113 2023-06-01 15:07:04.221387 byecycle-0.1.3/src/byecycle/misc.py
--rw-r--r--   0        0        0        0 2023-06-01 15:07:04.221387 byecycle-0.1.3/src/byecycle/py.typed
--rw-r--r--   0        0        0        0 2023-06-01 15:07:04.221387 byecycle-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0     3295 2023-06-01 15:07:04.221387 byecycle-0.1.3/tests/conftest.py
--rw-r--r--   0        0        0      299 2023-06-01 15:07:04.221387 byecycle-0.1.3/tests/test_module_imports.py
--rw-r--r--   0        0        0        0 2023-06-01 15:07:04.221387 byecycle-0.1.3/tests/test_scenarios/__init__.py
--rw-r--r--   0        0        0    11315 2023-06-01 15:07:04.221387 byecycle-0.1.3/tests/test_scenarios/test_basics.py
--rw-r--r--   0        0        0        0 2023-06-01 15:07:04.221387 byecycle-0.1.3/tests/test_scenarios/test_drawings.py
--rw-r--r--   0        0        0        0 2023-06-01 15:07:04.221387 byecycle-0.1.3/tests/unit/__init__.py
--rw-r--r--   0        0        0      592 2023-06-01 15:07:04.221387 byecycle-0.1.3/tests/unit/test_graph.py
--rw-r--r--   0        0        0     5533 1970-01-01 00:00:00.000000 byecycle-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-09 15:38:10.455547 byecycle-0.1.4/LICENSE
+-rw-r--r--   0        0        0     4864 2023-06-09 15:38:10.455547 byecycle-0.1.4/README.md
+-rw-r--r--   0        0        0     1651 2023-06-09 15:40:06.192963 byecycle-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      907 2023-06-09 15:38:10.455547 byecycle-0.1.4/src/byecycle/__init__.py
+-rw-r--r--   0        0        0       79 2023-06-09 15:38:10.455547 byecycle-0.1.4/src/byecycle/__main__.py
+-rw-r--r--   0        0        0     4163 2023-06-09 15:38:10.455547 byecycle-0.1.4/src/byecycle/cli.py
+-rw-r--r--   0        0        0     2993 2023-06-09 15:38:10.455547 byecycle-0.1.4/src/byecycle/draw/__init__.py
+-rw-r--r--   0        0        0    14207 2023-06-09 15:38:10.455547 byecycle-0.1.4/src/byecycle/graph.py
+-rw-r--r--   0        0        0     8428 2023-06-09 15:38:10.455547 byecycle-0.1.4/src/byecycle/misc.py
+-rw-r--r--   0        0        0        0 2023-06-09 15:38:10.455547 byecycle-0.1.4/src/byecycle/py.typed
+-rw-r--r--   0        0        0        0 2023-06-09 15:38:10.455547 byecycle-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0     2971 2023-06-09 15:38:10.459547 byecycle-0.1.4/tests/conftest.py
+-rw-r--r--   0        0        0      299 2023-06-09 15:38:10.459547 byecycle-0.1.4/tests/test_module_imports.py
+-rw-r--r--   0        0        0        0 2023-06-09 15:38:10.459547 byecycle-0.1.4/tests/test_scenarios/__init__.py
+-rw-r--r--   0        0        0    11463 2023-06-09 15:38:10.459547 byecycle-0.1.4/tests/test_scenarios/test_basics.py
+-rw-r--r--   0        0        0        0 2023-06-09 15:38:10.459547 byecycle-0.1.4/tests/test_scenarios/test_drawings.py
+-rw-r--r--   0        0        0        0 2023-06-09 15:38:10.459547 byecycle-0.1.4/tests/unit/__init__.py
+-rw-r--r--   0        0        0     1840 2023-06-09 15:38:10.459547 byecycle-0.1.4/tests/unit/test_graph.py
+-rw-r--r--   0        0        0     5527 1970-01-01 00:00:00.000000 byecycle-0.1.4/PKG-INFO
```

### Comparing `byecycle-0.1.3/LICENSE` & `byecycle-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `byecycle-0.1.3/README.md` & `byecycle-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
  - python 3.11 or higher
  - [pipx](https://pypa.github.io/pipx/installation/)
 ```shell
 pipx install byecycle
 ```
 ---
 
-### From Source / Dev Setup
+### Development Setup
 #### Requirements:
  - python 3.11 or higher
  - [pdm](https://pdm.fming.dev/)
  - git
 ```shell
 git clone https://github.com/a-recknagel/byecycle.git
 cd byecycle
```

### Comparing `byecycle-0.1.3/pyproject.toml` & `byecycle-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "byecycle"
-version = "0.1.3"
+version = "0.1.4"
 description = "Find and expose cyclic imports in python projects."
 requires-python = ">=3.11"
 readme = "README.md"
 authors = [
     { name = "Arne Caratti", email = "arne.recknagel@hotmail.com" },
 ]
 classifiers = [
```

### Comparing `byecycle-0.1.3/src/byecycle/cli.py` & `byecycle-0.1.4/src/byecycle/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import importlib.util
 import json
 import os.path
 from pathlib import Path
 
-import networkx as nx  # type: ignore
+import networkx as nx  # type: ignore[import]
 import typer
 from rich import print, print_json
 
 from byecycle.graph import Module, build_digraph
 from byecycle.misc import EdgeKind, GraphDict
 from byecycle.misc import _default_cycle_severity as severity
 from byecycle.misc import (
@@ -92,25 +92,28 @@
         A dictionary-representation of the import graph.
         The actual import graph.
         The name of the package.
     """
     if os.path.isdir(project):
         project_path = Path(project)
     else:
-        spec = importlib.util.find_spec(project)
+        try:
+            spec = importlib.util.find_spec(project)
+        except ImportError:
+            spec = None
         if spec is None or spec.origin is None:
             raise RuntimeError(
                 f"Failed trying to resolve {project=} as a package, please pass the "
                 f"source code location as proper path."
             )
         project_path = Path(spec.origin).parent.resolve()
 
-    Module.populate(project_path)
+    root = Module.parse(project_path)
     graph = build_digraph(
-        [*Module.modules()],
+        root,
         dynamic=dynamic,
         conditional=conditional,
         typing=typing,
         parent=parent,
         vanilla=vanilla,
     )
     return {key: {**graph[key]} for key in graph}, graph, project_path.name
```

### Comparing `byecycle-0.1.3/src/byecycle/draw/__init__.py` & `byecycle-0.1.4/src/byecycle/draw/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,26 @@
+"""
+This code can be taken as a template for implementing a visualization of a module-import-
+graph. This attempt here using matplotlib is something of a bare minimum, lacking key
+features like the ability to zoom, editing, or any kind of rich inspection.
+
+But it should give an idea of how a `networkx.DiGraph` can be used, and what kind of
+metadata was put on its edges.
+"""
+
 from chextra import warn
 
 warn()
 
 from pathlib import Path
 
-import matplotlib.colors as clrs  # type: ignore
-import matplotlib.patches as ptc  # type: ignore
-import matplotlib.pyplot as plt  # type: ignore
-import networkx as nx  # type: ignore
+import matplotlib.colors as clrs  # type: ignore[import]
+import matplotlib.patches as ptc  # type: ignore[import]
+import matplotlib.pyplot as plt  # type: ignore[import]
+import networkx as nx  # type: ignore[import]
 
 DEFAULT_COLORS = {
     "no_cycle": "black",
     "good": "green",
     "bad": "red",
     "complicated": "yellow",
 }
```

### Comparing `byecycle-0.1.3/src/byecycle/graph.py` & `byecycle-0.1.4/src/byecycle/graph.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,153 +1,168 @@
+"""
+All algorithms that are concerned with generating the import graph live in this module.
+On a high level, the following takes place:
+
+1. Given an absolute path to a directory, recursively collect all python files in it
+2. Compile the [AST](https://docs.python.org/3/library/ast.html#module-ast) of each file
+3. Collect all import statements from the ASTs, retain those that successfully match
+   against any of the parsed files (a _module_)
+4. From the context of the import-node within its AST, categorize each import statement
+5. Distribute the imports onto the modules they took place in, merge their categories if
+   there were multiple
+6. From these `module -> modules` mappings, generate a di-graph where the nodes are all
+   parsed modules, and the edges are the imports that take place between them
+7. A bidirectional edge implies an import cycle, and each edge retains the import
+   categories as metadata to help interpret the severity of the cycle
+"""
 from __future__ import annotations
 
 import ast
+import itertools
 from collections import defaultdict
+from operator import attrgetter
 from pathlib import Path
 from typing import Iterable, Self, Unpack
 
-import networkx as nx  # type: ignore
+import networkx as nx  # type: ignore[import]
 
 from byecycle.misc import (
     EdgeKind,
     ImportKind,
+    ImportStatement,
     SeverityMap,
     cycle_severity,
     path_to_module_name,
 )
 
 
 class Module:
-    """Represent a python module and the modules it imports."""
+    """Represent a python module and the modules it imports.
 
-    _modules: list[Module] = []
-    _sorted: bool = False
+    Every module has links to both its parent and children modules, as well as a
+    collection of modules that it imports in some way or another.
 
-    def __init__(self, name: str):
+    Parent-module imports are a bit of a special case, as their name doesn't actually
+    exist in the child module's namespace. But since any import like
+    `from foo.bar import baz` will, before `baz` is resolved, import `foo.bar` (which in
+    turn needs an import of `foo` before that), they are registered first thing anyway.
+
+    Treating their reliance chain as _imports_ models their relationship accurately for
+    the most part, but does create the impression of cycles if a parent imports names from
+    a child, which is a popular pattern for simplifying/exposing a public API. As a
+    consequence, these child-parent imports should be treated differently during
+    analysis.
+
+    See Also:
+        [discuss.python.org: Partial Modules](https://discuss.python.org/t/question-understanding-imports-a-bit-better-how-are-cycles-avoided/26647/2)
+        for a technical explanation of how parent and child modules interact during
+        imports.
+    """
+
+    def __init__(self, name: str, parent: Module | None):
         self.name: str = name
-        Module._modules.append(self)
+        self.parent: Module | None = parent
+        self.children: dict[str, Module] = {}
         self.imports: dict[Module, set[ImportKind]] = defaultdict(set)
+        if self.parent is not None:
+            self.imports[self.parent] = {"parent"}
+            self.parent.children[self.name] = self
 
-    def add(self, other: Module | str, tag: ImportKind):
-        """Add an import to this Module.
+    def __getitem__(self, item: str) -> Module:
+        return self.children[item]
 
-        This method can only be called once all Modules have been instantiated.
-
-        Args:
-            other: A modules, either as an object or as a string that will be evaluated as
-                its longest match from all valid module names. Valid strings are fully
-                qualified import arguments, i.e. `"foo.bar"` from `import foo.bar` or
-                `"foo.bar.baz"` from `from foo.bar import baz`. If `foo.bar` is a
-                registered module with name `baz` in it, both strings would add the module
-                `foo.bar` as an import.
-            tag: Describes the kind of import, e.g. import of module `foo` has the
-                tags `typing`, meaning it is the import of a parent module within an
-                `if typing.TYPE_CHECKING` block, which will be important information once
-                we want to visualize the severity of certain cyclic imports.
-
-        Raises:
-            RuntimeError: If bad arguments are passed.
-        """
-        if not Module._sorted:
-            # sort in descending alphabetical order, so that the longest match is found
-            # first
-            Module._modules.sort(key=lambda n: n.name, reverse=True)
-            Module._sorted = True
-
-        if isinstance(other, Module):
-            target = other
-        elif isinstance(other, str):
-            for node in Module.modules():
-                if other.startswith(node.name):
-                    target = node
-                    break
-            else:
-                # when calling this function, filter with `startswith(package)` to avoid
-                # this exception
-                raise RuntimeError(f"Tried to add non-local import {other=}.")
+    def __str__(self):
+        if self.children:
+            children = ", ".join(map(str, self.children.values()))
+            return f"{{{self.name} -> {children}}}"
         else:
-            # bad parameter type
-            raise RuntimeError(f"Tried to use invalid type {type(other)} as module.")
+            return self.name
 
-        self.imports[target].add(tag)
+    def __repr__(self):
+        return f"Module('{self.name}')"
 
     def __hash__(self):
         """Setting the hash of a module to be equal to its name's hash.
 
         That way, module objects can be found in hash maps by searching for their name
-        as a string. Also means that you can't mix strings and modules in said hash maps
-        without getting very confusing bugs. But, you know, why would you ever want to do
-        that anyway, right?
+        as a string. This also means that you can't mix strings and modules in said hash
+        maps without getting very confusing bugs. But, you know, why would you ever want
+        to do that anyway, right?
         """
         return self.name.__hash__()
 
-    def __str__(self):
-        imports = {
-            k.name: v
-            for k, v in sorted(
-                self.imports.items(), key=lambda x: x[0].name, reverse=True
-            )
-        }
-        return f"'{self.name}' -> {imports}"
+    def __eq__(self, other):
+        """Modules of the same name should always be equal to each other.
 
-    @classmethod
-    def reset(cls):
-        cls._modules = []
-        cls._sorted = False
+        A module comparing equal with its name enables searching for them in hash maps by
+        their name.
+        """
+        return self.name == other or self.name == other.name
 
-    @classmethod
-    def modules(cls) -> Iterable[Module]:
-        """Accessor for all registered modules."""
-        yield from cls._modules
+    def add_import(self, import_: ImportStatement, tag: ImportKind, root: Module):
+        """Register a local import statement and its tag to this Module.
 
-    @classmethod
-    def add_parent_imports(cls):
-        """Make modules with parent packages import them explicitly.
+        Args:
+            import_: Equivalent to an import statement. If the name is set, it may or may
+                not refer to a module.
+            tag: Describes the kind of import, e.g. import of module `foo` has the
+                tags `typing`, meaning it is the import of a parent module within an
+                `if typing.TYPE_CHECKING` block, which will be important information once
+                we want to visualize the severity of certain cyclic imports.
+            root: The root module, which is used to find the other module. It must point
+                to the root module of the fully parsed source tree in order to produce
+                correct results.
+
+        !!! warning
+            Given that an import statement of the form `from foo.bar import baz` can't be
+            reasonably resolved in a static approach, a little guessing has to take place.
+            The current idea is to try and import the full normalized statement
+            `foo.bar.baz` as a module. If that fails (read, no python file was parsed
+            which corresponds to the module name), only the part between `from` and
+            `import`, i.e. `foo.bar` is attempted, assuming that `baz` is an attribute
+            within `foo.bar`.
 
-        While the parent package's name doesn't automatically exist in a module's
-        namespace, any import like `from foo.bar import baz` will, before `baz` is
-        resolved, import `foo.bar` -- which in turn needs an import of `foo` before that.
-
-        Treating their reliance chain as _imports_ models this link accurately for the
-        most part, but does create the impression of cycles if a parent imports names from
-        a child, which is a popular pattern for simplifying/exposing a public API. As a
-        consequence, these child-parent imports should be treated differently during
-        analysis.
-
-        See Also:
-            [discuss.python.org: Partial Modules](https://discuss.python.org/t/question-understanding-imports-a-bit-better-how-are-cycles-avoided/26647/2)
-            for a technical explanation of how parent and child modules interact during
-            imports.
-
-        Notes:
-            This method wil only produce accurate results once all Nodes have been
-            initialised.
+            As long as the import statements would not raise an `ImportError`, this
+            _should_ always produce correct results.
         """
-        nodes: dict[str, Module] = {node.name: node for node in cls.modules()}
-        for node in [*cls.modules()]:  # node.add() may shuffle cls.modules
-            package = node.name.rsplit(".", 1)[0]  # only direct parent, not grandparents
-            if package in nodes and package != node.name:
-                node.add(nodes[package], "parent")
+        target: dict[str, Module] | Module = {root.name: root}  # seed
+        for sub_module in itertools.accumulate(
+            import_["module"].split("."), lambda a, b: f"{a}.{b}"
+        ):
+            target = target[sub_module]
+        if import_["name"] is not None:
+            try:
+                target = target[f"{import_['module']}.{import_['name']}"]
+            except KeyError:
+                pass  # "name" was not a module -- that's ok
+        self.imports[target].add(tag)  # type: ignore[index]
+
+    @staticmethod
+    def walk(module: Module) -> Iterable[Module]:
+        yield module
+        for recursion in map(Module.walk, module.children.values()):
+            yield from recursion
 
     @classmethod
-    def populate(cls, source_path: Path):
+    def parse(cls, source_path: Path) -> Module:
         """Walks down a source tree and registers each python file as a [`Module`][byecycle.graph.Module].
 
         After parsing all files recursively, all import statements in each file that
-        import a module that resolves to any of the files just recursed are listed
-        on their respective [`Module`][byecycle.graph.Module]. Additionally, some metadata from the context of the
-        import is retained. Specifically, the import-kind defintions are:
+        import a module that resolves to any of the files that we just parsed are listed
+        on their respective [`Module`][byecycle.graph.Module]. Additionally, some metadata
+        from the context of the import is retained. Specifically, the import-kind
+        definitions are:
 
         ___`vanilla`___
 
         :   A regular import at the top-level of the module
 
         ___`typing`___
 
-        :   Only executed during static type analyis
+        :   Only executed during static type analysis
 
         ___`dynamic`___
 
         :   Scoped in a function, which might not be executed on module load
 
         ___`conditional`___
 
@@ -157,71 +172,75 @@
 
         :   Due to the module in question being a parent of the current module (in python,
             parent modules are imported before their children)
 
         If a module is imported multiple times in different ways, all their metadata is
         aggregated on the same entry.
 
-        Once this method was executed, the [`Module.modules`][byecycle.graph.Module.modules]
-        class-method can be called to produce all created modules.
-
-        Note:
-            Since `populate` takes place at the class-level, calling this funtion multiple
-            times will clear the data from a previous call.
-
         Args:
             source_path: Location of the source tree of the package that should be walked.
                 The `.name` attribute of this parameter is assumed to be the name of the
                 package in order to identify which imports are local imports.
+
+        Returns:
+            The top level, aka "root", module.
         """
-        cls.reset()
-        node_data: dict[Module, list[tuple[str, ImportKind]]] = {}
-        package_name = source_path.name
+        root_name = source_path.name
+        node_data: dict[Module, list[tuple[ImportStatement, ImportKind]]] = {}
+        module_map: dict[str, Module] = {}
 
         # walk the project, compile all python files, collect their import statements
-        for path in source_path.rglob("*"):
-            if not path.name.endswith(".py"):
-                continue
-            name = path_to_module_name(str(path), str(source_path), package_name)
-
+        # package modules need to be parsed first to make parent-child-linkage work
+        for path in sorted(
+            source_path.rglob("*.py"),
+            key=lambda x: x.parent if x.name == "__init__.py" else x,
+        ):
+            name = path_to_module_name(str(path), str(source_path), root_name)
             with open(path) as f:
                 ast_ = ast.parse(f.read())
 
-            # add a link to parent modules to make `Module.add_parent_imports` work
-            # and a link to their assumed module path to resolve imports
+            # add a link to the parent module and their qualname
             for node in ast.walk(ast_):
                 for child in ast.iter_child_nodes(node):
                     child._parent = node  # type: ignore[attr-defined]
                     child._module = (  # type: ignore[attr-defined]
                         name.split(".") + ["."]
                         if path.name == "__init__.py"
                         else name.split(".")
                     )
             visitor = ImportVisitor()
             visitor.visit(ast_)
-            node_data[cls(name)] = [
-                (m, t) for m, t in visitor.imports if m.startswith(package_name)
+
+            parent = module_map.get(name.rsplit(".", 1)[0])
+            module = cls(name, parent)
+            module_map[name] = module
+            node_data[module] = [
+                (m, t) for m, t in visitor.imports if m["module"].startswith(root_name)
             ]
-        cls.add_parent_imports()
 
-        # add all found imports to their respective module
+        # all source files parsed
+        root = module_map[root_name]
+
+        # link up import data with their respective module
         for module, imports in node_data.items():
             for import_, kind in imports:
-                module.add(import_, kind)
+                module.add_import(import_, kind, root)
+
+        return root
 
 
 class ImportVisitor(ast.NodeVisitor):
     """Collect import statements in a module and assign them an [`ImportKind`][byecycle.misc.ImportKind] category.
 
     Relies on a non-standard `_parent` field being present in each node which contains
-    a link to its parent node.
+    a link to its parent node, and `_module` to resolve relative imports.
     """
 
     def __init__(self):
-        self.imports: list[tuple[str, ImportKind]] = []
+        self.imports: list[tuple[ImportStatement, ImportKind]] = []
 
     @classmethod
     def find_import_kind(cls, node: ast.Import | ast.ImportFrom) -> ImportKind:
         """Find the [`ImportKind`][byecycle.misc.ImportKind] of an import statement.
 
         A single import statement can only have a single [`ImportKind`][byecycle.misc.ImportKind].
         This function uses information in the `ast.AST`-node to identify if it was
@@ -244,63 +263,63 @@
             case ast.If(_parent=ast.Module()):  # type: ignore[misc]
                 # probably guarded by `if sys.version >= (x, y, z):`, but doesn't actually
                 # matter -- anything but TYPE_CHECKING is env-dependent during runtime or
                 # too obtuse to consider (I'm not writing code that checks for `if True:`)
                 return "conditional"
             case _:
                 while True:
-                    # test if the import happens somewhere in a function
                     if isinstance(parent, (ast.FunctionDef, ast.AsyncFunctionDef)):
+                        # the import happens somewhere in a function
                         return "dynamic"
                     try:
                         parent = parent._parent  # type: ignore[attr-defined]
                     except AttributeError:
                         # any nodes that reach this point are treated as regular toplevel
                         # imports, like imports that happen in a class body
                         return "vanilla"
 
     def visit_Import(self, node: ast.Import):
         kind = self.find_import_kind(node)
         for alias in node.names:
-            self.imports.append((alias.name, kind))
+            self.imports.append(({"module": alias.name, "name": None}, kind))
 
     def visit_ImportFrom(self, node: ast.ImportFrom):
         kind = self.find_import_kind(node)
         # handle relative imports
         if node.level:
             path = node._module[: -node.level]  # type: ignore[attr-defined]
             if node.module:
                 path.append(node.module)
             module = ".".join(path)
         else:
-            assert node.module is not None  # iff None when node.level > 0 # nosec
-            module = node.module
+            # if node.level is 0, node.module can't be None
+            module = node.module  # type: ignore[assignment]
 
         for alias in node.names:
-            self.imports.append((f"{module}.{alias.name}", kind))
+            self.imports.append(({"module": module, "name": alias.name}, kind))
 
 
-def build_digraph(modules: list[Module], **kwargs: Unpack[SeverityMap]) -> nx.DiGraph:
-    """Turns a module-imports-mapping into a smart graph object.
+def build_digraph(root: Module, **kwargs: Unpack[SeverityMap]) -> nx.DiGraph:
+    """Turns module-import-mappings into a smart graph object.
 
     Args:
-        modules: [`Module`][byecycle.graph.Module] objects that know what other local
-            modules they import, and how.
+        root: Gets walked to produce all [`Module`][byecycle.graph.Module] objects that
+            know what other local modules they import, and how.
         **kwargs: Override the default settings for the severity of the "how" when imports
             in local modules might cause import cycles.
 
     Returns:
-        A graph object which allows the kind of operations that you'd want when working
-        with graph-like structures. Every edge in the graph has a `tags` and a `cycle`
-        entry (accessible with `getitem()`) holding metadata that can help interpret how
-        much of an issue a particular cyclic import might be.
+        A graph object which supports the kind of operations that you'd want when working
+            with graph-like structures. Every edge in the graph has a `tags` and a `cycle`
+            entry (accessible with `getitem()`) holding metadata that can help interpret
+            how much of an issue a particular cyclic import might be.
     """
     g = nx.DiGraph()
-    g.add_nodes_from([m.name for m in modules])
-    for module in modules:
+    g.add_nodes_from(map(attrgetter("name"), Module.walk(root)))
+    for module in Module.walk(root):
         for import_, tags in module.imports.items():
             g.add_edge(module.name, import_.name, tags=tags)
     for e_0, e_1 in g.edges():
         if g.has_edge(e_1, e_0):
             g[e_0][e_1]["cycle"] = cycle_severity(
                 g[e_0][e_1]["tags"], g[e_1][e_0]["tags"], **kwargs
             )
```

### Comparing `byecycle-0.1.3/src/byecycle/misc.py` & `byecycle-0.1.4/src/byecycle/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+Collection of shared structures, types, and functions.
+"""
+
 import enum
 from typing import (
     Annotated,
     Iterable,
     Literal,
     Optional,
     TypeAlias,
@@ -34,15 +38,15 @@
 The keys on the first level are the qualnames of importing modules, the keys on the second 
 level are the qualnames of imported modules, and the values on the second level contain
 the metadata dictionary of their keyed imports ([`ImportMetaData`][byecycle.misc.ImportMetaData]).
 Metadata consists of a `tags`-list of [`ImportKind`][byecycle.misc.ImportKind]s and a
 `cycle` which is either an [`EdgeKind`][byecycle.misc.EdgeKind] if there is a cycle, or
 `None` if there isn't.
 
-Example:
+??? example
     ```py
     {
         "foo": {
             "foo.a": {
                 "tags": ["vanilla"],
                 "cycle": "complicated"
             }
@@ -88,14 +92,24 @@
     dynamic: EdgeKind
     conditional: EdgeKind
     typing: EdgeKind
     parent: EdgeKind
     vanilla: EdgeKind
 
 
+class ImportStatement(TypedDict):
+    """Container for the information that we need from an AST import node.
+
+    The module-value is always non-empty, the name-value is only set by `ast.ImportFrom`.
+    """
+
+    module: str
+    name: str | None
+
+
 class _Edge(str, enum.Enum):
     """Proxy of the [`EdgeKind`][byecycle.misc.ImportKind] type alias.
 
     Necessary for typer due to https://github.com.tiangolo/typer/issues/76. I really hate
     it, also makes mypy sad.
     """
```

### Comparing `byecycle-0.1.3/tests/conftest.py` & `byecycle-0.1.4/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 @pytest.fixture
 def pip():
     """Not actually pip.
 
     But for testing purposes it's close enough.
     """
     old_modules = sys.modules.copy()
+    old_path = sys.path.copy()
     tmp_dir: tempfile.TemporaryDirectory | None = None
-    installed: Path | None = None
 
     def pseudo_installer(source: dict, *, install=True) -> str:
         def files_from_dict(path: Path, files: dict[str, str | dict]):
             for file_name, file_content in files.items():
                 if isinstance(file_content, str):
                     with open(path / f"{file_name}.py", "w") as f:
                         f.write(file_content)
@@ -56,45 +56,37 @@
                 else:
                     raise RuntimeError(
                         f"Bad format for {files=}, keys should be valid module names "
                         f"and values should be python file contents or a recursion."
                     )
 
         nonlocal tmp_dir
-        nonlocal installed
 
         # create source trees
         if len(source) != 1:
             raise RuntimeError("Exactly one top-level import-package required.")
         name = [*source][0]
         tmp_dir = tempfile.TemporaryDirectory(prefix=f"{name}_")
         files_from_dict(Path(tmp_dir.name), source)
 
-        # look ma, I'm a packager now!
         if install:
-            site_path = Path(site.getsitepackages()[-1])
-            dst = site_path / name
-            installed = shutil.copytree(Path(tmp_dir.name) / name, dst)
+            sys.path.append(tmp_dir.name)
 
         return str(Path(tmp_dir.name) / name)
 
     try:
         yield pseudo_installer
     finally:
         # cleanup of tmp files
         if tmp_dir:
             tmp_dir.cleanup()
 
-        # cleanup of "installed" modules
-        if installed:
-            shutil.rmtree(installed)
-            # ... was that so hard, easy_install?
-
-    # restoring module cache
+    # restoring system
     sys.modules = old_modules
+    sys.path = old_path
 
 
 @pytest.fixture(scope="session", autouse=True)
 def termination_handler():
     """Sends a SIGINT in case SIGTERM was sent to the current process.
 
     By default, fixture cleanup won't run on SIGTERM, which is unfortunately the default
```

### Comparing `byecycle-0.1.3/tests/test_scenarios/test_basics.py` & `byecycle-0.1.4/tests/test_scenarios/test_basics.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,405 +1,361 @@
 import json
 import subprocess
 import sys
 
+import pytest
+
 
 def test_version(cli):
     result = cli("--version")
 
     assert "version: " in result.output
 
 
-def test_package_no_imports(cli, pip):
-    pip(
-        {
-            "foo": {
-                "__init__": "",
-                "bar": "",
-                "baz": {
+@pytest.mark.parametrize(
+    "install", [pytest.param(True, id="package"), pytest.param(False, id="source tree")]
+)
+class TestMainEntrypoint:
+    def test_no_imports(self, cli, pip, install):
+        source = pip(
+            {
+                "foo": {
                     "__init__": "",
-                    "qux": "",
-                    "quux": "",
-                },
-            }
-        }
-    )
-
-    result = cli("foo")
-
-    assert result.exit_code == 0
-    assert result.json == {
-        "foo": {},
-        "foo.bar": {"foo": {"cycle": None, "tags": ["parent"]}},
-        "foo.baz": {"foo": {"cycle": None, "tags": ["parent"]}},
-        "foo.baz.qux": {"foo.baz": {"cycle": None, "tags": ["parent"]}},
-        "foo.baz.quux": {"foo.baz": {"cycle": None, "tags": ["parent"]}},
-    }
+                    "bar": "",
+                    "baz": {
+                        "__init__": "",
+                        "qux": "",
+                        "quux": "",
+                    },
+                }
+            },
+            install=install,
+        )
 
+        result = cli("foo" if install else source)
 
-def test_package_with_imports(cli, pip):
-    pip(
-        {
-            "foo": {
-                "__init__": "from foo import bar",
-                "bar": "from foo.baz import qux",
-                "baz": {
-                    "__init__": "",
-                    "qux": "from foo.baz.quux import x",
-                    "quux": "x = 1",
-                },
-            }
+        assert result.exit_code == 0
+        assert result.json == {
+            "foo": {},
+            "foo.bar": {"foo": {"cycle": None, "tags": ["parent"]}},
+            "foo.baz": {"foo": {"cycle": None, "tags": ["parent"]}},
+            "foo.baz.qux": {"foo.baz": {"cycle": None, "tags": ["parent"]}},
+            "foo.baz.quux": {"foo.baz": {"cycle": None, "tags": ["parent"]}},
         }
-    )
-
-    result = cli("foo")
 
-    assert result.exit_code == 0
-    assert result.json == {
-        "foo": {"foo.bar": {"cycle": "complicated", "tags": ["vanilla"]}},
-        "foo.bar": {
-            "foo": {"cycle": "complicated", "tags": ["parent"]},
-            "foo.baz.qux": {"cycle": None, "tags": ["vanilla"]},
-        },
-        "foo.baz": {"foo": {"cycle": None, "tags": ["parent"]}},
-        "foo.baz.qux": {
-            "foo.baz": {"cycle": None, "tags": ["parent"]},
-            "foo.baz.quux": {"cycle": None, "tags": ["vanilla"]},
-        },
-        "foo.baz.quux": {"foo.baz": {"cycle": None, "tags": ["parent"]}},
-    }
+    def test_imports(self, cli, pip, install):
+        source = pip(
+            {
+                "foo": {
+                    "__init__": "import foo.bar",
+                    "bar": "import foo.baz.qux",
+                    "baz": {
+                        "__init__": "",
+                        "qux": "import foo.baz.quux",
+                        "quux": "x = 1",
+                    },
+                }
+            },
+            install=install,
+        )
 
+        result = cli("foo" if install else source)
 
-def test_package_with_relative_imports(cli, pip):
-    pip(
-        {
-            "foo": {
-                "__init__": "from . import bar",
-                "bar": "from .baz import qux",
-                "baz": {
-                    "__init__": "",
-                    "qux": "from .quux import x",
-                    "quux": "x = 1",
-                    "quuux": "from ..foo.quux import x",
-                },
-            }
+        assert result.exit_code == 0
+        assert result.json == {
+            "foo": {"foo.bar": {"cycle": "complicated", "tags": ["vanilla"]}},
+            "foo.bar": {
+                "foo": {"cycle": "complicated", "tags": ["parent"]},
+                "foo.baz.qux": {"cycle": None, "tags": ["vanilla"]},
+            },
+            "foo.baz": {"foo": {"cycle": None, "tags": ["parent"]}},
+            "foo.baz.qux": {
+                "foo.baz": {"cycle": None, "tags": ["parent"]},
+                "foo.baz.quux": {"cycle": None, "tags": ["vanilla"]},
+            },
+            "foo.baz.quux": {"foo.baz": {"cycle": None, "tags": ["parent"]}},
         }
-    )
 
-    result = cli("foo")
-
-    assert result.exit_code == 0
-    assert result.json == {
-        "foo": {"foo.bar": {"cycle": "complicated", "tags": ["vanilla"]}},
-        "foo.bar": {
-            "foo": {"cycle": "complicated", "tags": ["parent"]},
-            "foo.baz.qux": {"cycle": None, "tags": ["vanilla"]},
-        },
-        "foo.baz": {"foo": {"cycle": None, "tags": ["parent"]}},
-        "foo.baz.qux": {
-            "foo.baz": {"cycle": None, "tags": ["parent"]},
-            "foo.baz.quux": {"cycle": None, "tags": ["vanilla"]},
-        },
-        "foo.baz.quux": {"foo.baz": {"cycle": None, "tags": ["parent"]}},
-        "foo.baz.quuux": {
-            "foo": {"cycle": None, "tags": ["vanilla"]},
-            "foo.baz": {"cycle": None, "tags": ["parent"]},
-        },
-    }
+    def test_imports_from(self, cli, pip, install):
+        source = pip(
+            {
+                "foo": {
+                    "__init__": "from foo import bar",
+                    "bar": "from foo.baz import qux",
+                    "baz": {
+                        "__init__": "",
+                        "qux": "from foo.baz.quux import x",
+                        "quux": "x = 1",
+                    },
+                }
+            },
+            install=install,
+        )
 
+        result = cli("foo" if install else source)
 
-def test_source_tree_no_imports(cli, pip):
-    source = pip(
-        {
-            "foo": {
-                "__init__": "",
-                "bar": "",
-                "baz": {
-                    "__init__": "",
-                    "qux": "",
-                    "quux": "",
-                },
-            }
-        },
-        install=False,
-    )
+        assert result.exit_code == 0
+        assert result.json == {
+            "foo": {"foo.bar": {"cycle": "complicated", "tags": ["vanilla"]}},
+            "foo.bar": {
+                "foo": {"cycle": "complicated", "tags": ["parent"]},
+                "foo.baz.qux": {"cycle": None, "tags": ["vanilla"]},
+            },
+            "foo.baz": {"foo": {"cycle": None, "tags": ["parent"]}},
+            "foo.baz.qux": {
+                "foo.baz": {"cycle": None, "tags": ["parent"]},
+                "foo.baz.quux": {"cycle": None, "tags": ["vanilla"]},
+            },
+            "foo.baz.quux": {"foo.baz": {"cycle": None, "tags": ["parent"]}},
+        }
 
-    result = cli(source)
+    def test_relative_imports_from(self, cli, pip, install):
+        source = pip(
+            {
+                "foo": {
+                    "__init__": "from . import bar",
+                    "bar": "from .baz import qux",
+                    "baz": {
+                        "__init__": "",
+                        "qux": "from .quux import x",
+                        "quux": "x = 1",
+                        "quuux": "from ..baz.quux import x",
+                    },
+                }
+            },
+            install=install,
+        )
 
-    assert result.exit_code == 0
-    assert result.json == {
-        "foo": {},
-        "foo.bar": {"foo": {"cycle": None, "tags": ["parent"]}},
-        "foo.baz": {"foo": {"cycle": None, "tags": ["parent"]}},
-        "foo.baz.qux": {"foo.baz": {"cycle": None, "tags": ["parent"]}},
-        "foo.baz.quux": {"foo.baz": {"cycle": None, "tags": ["parent"]}},
-    }
+        result = cli("foo" if install else source)
 
+        assert result.exit_code == 0
+        assert result.json == {
+            "foo": {"foo.bar": {"cycle": "complicated", "tags": ["vanilla"]}},
+            "foo.bar": {
+                "foo": {"cycle": "complicated", "tags": ["parent"]},
+                "foo.baz.qux": {"cycle": None, "tags": ["vanilla"]},
+            },
+            "foo.baz": {"foo": {"cycle": None, "tags": ["parent"]}},
+            "foo.baz.qux": {
+                "foo.baz": {"cycle": None, "tags": ["parent"]},
+                "foo.baz.quux": {"cycle": None, "tags": ["vanilla"]},
+            },
+            "foo.baz.quux": {"foo.baz": {"cycle": None, "tags": ["parent"]}},
+            "foo.baz.quuux": {
+                "foo.baz": {"cycle": None, "tags": ["parent"]},
+                "foo.baz.quux": {"cycle": None, "tags": ["vanilla"]},
+            },
+        }
 
-def test_source_tree_with_imports(cli, pip):
-    source = pip(
-        {
-            "foo": {
-                "__init__": "from foo import bar",
-                "bar": "from foo.baz import qux",
-                "baz": {
+    def test_vanilla_cycle(self, cli, pip, install):
+        source = pip(
+            {
+                "foo": {
                     "__init__": "",
-                    "qux": "from foo.baz.quux import x",
-                    "quux": "x = 1",
+                    "bar": "import foo.baz",
+                    "baz": "import foo.bar",
                 },
-            }
-        },
-        install=False,
-    )
+            },
+            install=install,
+        )
 
-    result = cli(source)
-
-    assert result.exit_code == 0
-    assert result.json == {
-        "foo": {"foo.bar": {"cycle": "complicated", "tags": ["vanilla"]}},
-        "foo.bar": {
-            "foo": {"cycle": "complicated", "tags": ["parent"]},
-            "foo.baz.qux": {"cycle": None, "tags": ["vanilla"]},
-        },
-        "foo.baz": {"foo": {"cycle": None, "tags": ["parent"]}},
-        "foo.baz.qux": {
-            "foo.baz": {"cycle": None, "tags": ["parent"]},
-            "foo.baz.quux": {"cycle": None, "tags": ["vanilla"]},
-        },
-        "foo.baz.quux": {"foo.baz": {"cycle": None, "tags": ["parent"]}},
-    }
+        result = cli("foo" if install else source)
 
+        assert result.exit_code == 0
+        assert result.json == {
+            "foo": {},
+            "foo.bar": {
+                "foo": {"cycle": None, "tags": ["parent"]},
+                "foo.baz": {"cycle": "bad", "tags": ["vanilla"]},
+            },
+            "foo.baz": {
+                "foo": {"cycle": None, "tags": ["parent"]},
+                "foo.bar": {"cycle": "bad", "tags": ["vanilla"]},
+            },
+        }
 
-def test_source_tree_with_relative_imports(cli, pip):
-    source = pip(
-        {
-            "foo": {
-                "__init__": "from . import bar",
-                "bar": "from .baz import qux",
-                "baz": {
+    def test_typing_cycle(self, cli, pip, install):
+        source = pip(
+            {
+                "foo": {
                     "__init__": "",
-                    "qux": "from .quux import x",
-                    "quux": "x = 1",
-                    "quuux": "from ..foo.quux import x",
+                    "bar": (
+                        "import typing\n" "if typing.TYPE_CHECKING:\n" "   import foo.baz"
+                    ),
+                    "baz": "import foo.bar",
                 },
-            }
-        },
-        install=False,
-    )
-
-    result = cli(source)
-
-    assert result.exit_code == 0
-    assert result.json == {
-        "foo": {"foo.bar": {"cycle": "complicated", "tags": ["vanilla"]}},
-        "foo.bar": {
-            "foo": {"cycle": "complicated", "tags": ["parent"]},
-            "foo.baz.qux": {"cycle": None, "tags": ["vanilla"]},
-        },
-        "foo.baz": {"foo": {"cycle": None, "tags": ["parent"]}},
-        "foo.baz.qux": {
-            "foo.baz": {"cycle": None, "tags": ["parent"]},
-            "foo.baz.quux": {"cycle": None, "tags": ["vanilla"]},
-        },
-        "foo.baz.quux": {"foo.baz": {"cycle": None, "tags": ["parent"]}},
-        "foo.baz.quuux": {
-            "foo": {"cycle": None, "tags": ["vanilla"]},
-            "foo.baz": {"cycle": None, "tags": ["parent"]},
-        },
-    }
-
-
-def test_package_vanilla_cycle(cli, pip):
-    pip(
-        {
-            "foo": {
-                "__init__": "",
-                "bar": "import foo.baz",
-                "baz": "import foo.bar",
             },
-        }
-    )
-
-    result = cli("foo")
-
-    assert result.exit_code == 0
-    assert result.json == {
-        "foo": {},
-        "foo.bar": {
-            "foo": {"cycle": None, "tags": ["parent"]},
-            "foo.baz": {"cycle": "bad", "tags": ["vanilla"]},
-        },
-        "foo.baz": {
-            "foo": {"cycle": None, "tags": ["parent"]},
-            "foo.bar": {"cycle": "bad", "tags": ["vanilla"]},
-        },
-    }
+            install=install,
+        )
 
+        result = cli("foo" if install else source)
 
-def test_package_typing_cycle(cli, pip):
-    pip(
-        {
-            "foo": {
-                "__init__": "",
-                "bar": (
-                    "import typing\n" "if typing.TYPE_CHECKING:\n" "   import foo.baz"
-                ),
-                "baz": "import foo.bar",
+        assert result.exit_code == 0
+        assert result.json == {
+            "foo": {},
+            "foo.bar": {
+                "foo": {"cycle": None, "tags": ["parent"]},
+                "foo.baz": {"cycle": "skip", "tags": ["typing"]},
+            },
+            "foo.baz": {
+                "foo": {"cycle": None, "tags": ["parent"]},
+                "foo.bar": {"cycle": "skip", "tags": ["vanilla"]},
             },
         }
-    )
-    result = cli("foo")
 
-    assert result.exit_code == 0
-    assert result.json == {
-        "foo": {},
-        "foo.bar": {
-            "foo": {"cycle": None, "tags": ["parent"]},
-            "foo.baz": {"cycle": "skip", "tags": ["typing"]},
-        },
-        "foo.baz": {
-            "foo": {"cycle": None, "tags": ["parent"]},
-            "foo.bar": {"cycle": "skip", "tags": ["vanilla"]},
-        },
-    }
+    def test_conditional_cycle(self, cli, pip, install):
+        source = pip(
+            {
+                "foo": {
+                    "__init__": "",
+                    "bar": (
+                        "import sys\n"
+                        "if sys.version >= (3, 10, 0):\n"
+                        "   import foo.baz"
+                    ),
+                    "baz": "import foo.bar",
+                },
+            },
+            install=install,
+        )
 
+        result = cli("foo" if install else source)
 
-def test_package_conditional_cycle(cli, pip):
-    pip(
-        {
-            "foo": {
-                "__init__": "",
-                "bar": (
-                    "import sys\n" "if sys.version >= (3, 10, 0):\n" "   import foo.baz"
-                ),
-                "baz": "import foo.bar",
+        assert result.exit_code == 0
+        assert result.json == {
+            "foo": {},
+            "foo.bar": {
+                "foo": {"cycle": None, "tags": ["parent"]},
+                "foo.baz": {"cycle": "complicated", "tags": ["conditional"]},
+            },
+            "foo.baz": {
+                "foo": {"cycle": None, "tags": ["parent"]},
+                "foo.bar": {"cycle": "complicated", "tags": ["vanilla"]},
             },
         }
-    )
-    result = cli("foo")
 
-    assert result.exit_code == 0
-    assert result.json == {
-        "foo": {},
-        "foo.bar": {
-            "foo": {"cycle": None, "tags": ["parent"]},
-            "foo.baz": {"cycle": "complicated", "tags": ["conditional"]},
-        },
-        "foo.baz": {
-            "foo": {"cycle": None, "tags": ["parent"]},
-            "foo.bar": {"cycle": "complicated", "tags": ["vanilla"]},
-        },
-    }
+    def test_dynamic_cycle(self, cli, pip, install):
+        source = pip(
+            {
+                "foo": {
+                    "__init__": "",
+                    "bar": ("def qux():\n" "   import foo.baz"),
+                    "baz": "import foo.bar",
+                },
+            },
+            install=install,
+        )
 
+        result = cli("foo" if install else source)
 
-def test_package_dynamic_cycle(cli, pip):
-    pip(
-        {
-            "foo": {
-                "__init__": "",
-                "bar": ("def qux():\n" "   import foo.baz"),
-                "baz": "import foo.bar",
+        assert result.exit_code == 0
+        assert result.json == {
+            "foo": {},
+            "foo.bar": {
+                "foo": {"cycle": None, "tags": ["parent"]},
+                "foo.baz": {"cycle": "complicated", "tags": ["dynamic"]},
+            },
+            "foo.baz": {
+                "foo": {"cycle": None, "tags": ["parent"]},
+                "foo.bar": {"cycle": "complicated", "tags": ["vanilla"]},
             },
         }
-    )
-    result = cli("foo")
 
-    assert result.exit_code == 0
-    assert result.json == {
-        "foo": {},
-        "foo.bar": {
-            "foo": {"cycle": None, "tags": ["parent"]},
-            "foo.baz": {"cycle": "complicated", "tags": ["dynamic"]},
-        },
-        "foo.baz": {
-            "foo": {"cycle": None, "tags": ["parent"]},
-            "foo.bar": {"cycle": "complicated", "tags": ["vanilla"]},
-        },
-    }
+    def test_class_scope_is_toplevel_cycle(self, cli, pip, install):
+        source = pip(
+            {
+                "foo": {
+                    "__init__": "",
+                    "bar": ("class Qux:\n" "   import foo.baz"),
+                    "baz": "import foo.bar",
+                },
+            },
+            install=install,
+        )
 
+        result = cli("foo" if install else source)
 
-def test_package_class_scope_is_toplevel_cycle(cli, pip):
-    pip(
-        {
-            "foo": {
-                "__init__": "",
-                "bar": ("class Qux:\n" "   import foo.baz"),
-                "baz": "import foo.bar",
+        assert result.exit_code == 0
+        assert result.json == {
+            "foo": {},
+            "foo.bar": {
+                "foo": {"cycle": None, "tags": ["parent"]},
+                "foo.baz": {"cycle": "bad", "tags": ["vanilla"]},
+            },
+            "foo.baz": {
+                "foo": {"cycle": None, "tags": ["parent"]},
+                "foo.bar": {"cycle": "bad", "tags": ["vanilla"]},
             },
         }
-    )
-    result = cli("foo")
 
-    assert result.exit_code == 0
-    assert result.json == {
-        "foo": {},
-        "foo.bar": {
-            "foo": {"cycle": None, "tags": ["parent"]},
-            "foo.baz": {"cycle": "bad", "tags": ["vanilla"]},
-        },
-        "foo.baz": {
-            "foo": {"cycle": None, "tags": ["parent"]},
-            "foo.bar": {"cycle": "bad", "tags": ["vanilla"]},
-        },
-    }
-
-
-def test_package_does_not_exist(cli):
-    result = cli("foo")
-
-    assert result.exit_code == 1
-    assert "Failed trying to resolve project='foo'" in result.exception.args[0]
-
-
-def test_package_print_plain(cli, pip):
-    pip(
-        {
-            "foo": {
-                "__init__": "",
-                "bar": "",
-                "baz": {
+    def test_print_plain(self, cli, pip, install):
+        source = pip(
+            {
+                "foo": {
                     "__init__": "",
-                    "qux": "",
-                    "quux": "",
-                },
-            }
-        }
-    )
+                    "bar": "",
+                    "baz": {
+                        "__init__": "",
+                        "qux": "",
+                        "quux": "",
+                    },
+                }
+            },
+            install=install,
+        )
 
-    result = cli("foo", "--no-rich")
+        result = cli("foo" if install else source, "--no-rich")
 
-    assert result.exit_code == 0
-    assert result.json == {
-        "foo": {},
-        "foo.bar": {"foo": {"cycle": None, "tags": ["parent"]}},
-        "foo.baz": {"foo": {"cycle": None, "tags": ["parent"]}},
-        "foo.baz.qux": {"foo.baz": {"cycle": None, "tags": ["parent"]}},
-        "foo.baz.quux": {"foo.baz": {"cycle": None, "tags": ["parent"]}},
-    }
+        assert result.exit_code == 0
+        assert result.json == {
+            "foo": {},
+            "foo.bar": {"foo": {"cycle": None, "tags": ["parent"]}},
+            "foo.baz": {"foo": {"cycle": None, "tags": ["parent"]}},
+            "foo.baz.qux": {"foo.baz": {"cycle": None, "tags": ["parent"]}},
+            "foo.baz.quux": {"foo.baz": {"cycle": None, "tags": ["parent"]}},
+        }
 
 
-def test_source_tree_byecycle_as_subprocess_module(pip):
+def test_byecycle_as_subprocess_module(pip):
     source = pip(
         {
             "foo": {
                 "__init__": "",
                 "bar": "",
                 "baz": {
                     "__init__": "",
                     "qux": "",
                     "quux": "",
                 },
             }
-        }
+        },
+        install=False,
     )
 
     result = subprocess.run(
-        [sys.executable, "-m", "byecycle", source], capture_output=True
+        [sys.executable, "-m", "byecycle", source],
+        capture_output=True,
     )
 
+    assert result.returncode == 0
     assert json.loads(result.stdout) == {
         "foo": {},
         "foo.bar": {"foo": {"cycle": None, "tags": ["parent"]}},
         "foo.baz": {"foo": {"cycle": None, "tags": ["parent"]}},
         "foo.baz.qux": {"foo.baz": {"cycle": None, "tags": ["parent"]}},
         "foo.baz.quux": {"foo.baz": {"cycle": None, "tags": ["parent"]}},
     }
+
+
+def test_package_not_installed(cli):
+    result = cli("foo")
+
+    assert result.exit_code == 1
+    assert "Failed trying to resolve project" in result.exception.args[0]
+
+
+@pytest.mark.parametrize("path", ["/foo", "./foo", "/home/dev/foo"])
+def test_path_not_found(cli, path):
+    result = cli(path)
+
+    assert result.exit_code == 1
+    assert "Failed trying to resolve project" in result.exception.args[0]
```

### Comparing `byecycle-0.1.3/PKG-INFO` & `byecycle-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byecycle
-Version: 0.1.3
+Version: 0.1.4
 Summary: Find and expose cyclic imports in python projects.
 Author-Email: Arne Caratti <arne.recknagel@hotmail.com>
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Typing :: Typed
 Classifier: Programming Language :: Python :: 3.11
@@ -43,15 +43,15 @@
  - python 3.11 or higher
  - [pipx](https://pypa.github.io/pipx/installation/)
 ```shell
 pipx install byecycle
 ```
 ---
 
-### From Source / Dev Setup
+### Development Setup
 #### Requirements:
  - python 3.11 or higher
  - [pdm](https://pdm.fming.dev/)
  - git
 ```shell
 git clone https://github.com/a-recknagel/byecycle.git
 cd byecycle
```

