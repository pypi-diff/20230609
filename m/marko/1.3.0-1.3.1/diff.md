# Comparing `tmp/marko-1.3.0.tar.gz` & `tmp/marko-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marko-1.3.0.tar", last modified: Sat Jan 28 08:37:04 2023, max compression
+gzip compressed data, was "marko-1.3.1.tar", last modified: Fri Jun  9 08:55:13 2023, max compression
```

## Comparing `marko-1.3.0.tar` & `marko-1.3.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-01-28 08:36:56.916728 marko-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-01-28 08:36:56.916728 marko-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-01-28 08:36:56.916728 marko-1.3.0/marko/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-01-28 08:36:56.916728 marko-1.3.0/marko/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-01-28 08:36:56.916728 marko-1.3.0/marko/ast_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20371 2023-01-28 08:36:56.916728 marko-1.3.0/marko/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-01-28 08:36:56.916728 marko-1.3.0/marko/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-01-28 08:36:56.916728 marko-1.3.0/marko/element.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-01-28 08:36:56.916728 marko-1.3.0/marko/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-01-28 08:36:56.916728 marko-1.3.0/marko/ext/codehilite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-01-28 08:36:56.916728 marko-1.3.0/marko/ext/footnote.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-01-28 08:36:56.916728 marko-1.3.0/marko/ext/gfm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-01-28 08:36:56.916728 marko-1.3.0/marko/ext/gfm/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-01-28 08:36:56.916728 marko-1.3.0/marko/ext/latex_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-01-28 08:36:56.916728 marko-1.3.0/marko/ext/pangu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-01-28 08:36:56.916728 marko-1.3.0/marko/ext/toc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-01-28 08:36:56.916728 marko-1.3.0/marko/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-01-28 08:36:56.916728 marko-1.3.0/marko/html_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-01-28 08:36:56.916728 marko-1.3.0/marko/inline.py
--rw-r--r--   0 runner    (1001) docker     (123)    17688 2023-01-28 08:36:56.916728 marko-1.3.0/marko/inline_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-01-28 08:36:56.916728 marko-1.3.0/marko/md_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-01-28 08:36:56.916728 marko-1.3.0/marko/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-01-28 08:36:56.916728 marko-1.3.0/marko/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-28 08:36:56.916728 marko-1.3.0/marko/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-01-28 08:36:56.916728 marko-1.3.0/marko/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-01-28 08:36:56.916728 marko-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-01-28 08:36:56.916728 marko-1.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-01-28 08:36:56.916728 marko-1.3.0/tests/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-01-28 08:36:56.916728 marko-1.3.0/tests/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)    13117 2023-01-28 08:36:56.916728 marko-1.3.0/tests/samples/jquery.md
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-01-28 08:36:56.916728 marko-1.3.0/tests/samples/syntax.md
--rw-r--r--   0 runner    (1001) docker     (123)   204971 2023-01-28 08:36:56.920728 marko-1.3.0/tests/spec/commonmark.txt
--rw-r--r--   0 runner    (1001) docker     (123)   216867 2023-01-28 08:36:56.920728 marko-1.3.0/tests/spec/gfm.txt
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-01-28 08:36:56.916728 marko-1.3.0/tests/spec.sh
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-01-28 08:36:56.920728 marko-1.3.0/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-01-28 08:36:56.920728 marko-1.3.0/tests/test_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-01-28 08:36:56.920728 marko-1.3.0/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-01-28 08:36:56.920728 marko-1.3.0/tests/test_latex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-01-28 08:36:56.920728 marko-1.3.0/tests/test_spec.py
--rw-------   0 runner    (1001) docker     (123)     4343 2023-01-28 08:37:04.877029 marko-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-09 08:55:03.195424 marko-1.3.1/LICENSE
+-rw-r--r--   0        0        0     3505 2023-06-09 08:55:03.195424 marko-1.3.1/README.md
+-rw-r--r--   0        0        0     5127 2023-06-09 08:55:03.195424 marko-1.3.1/marko/__init__.py
+-rw-r--r--   0        0        0      333 2023-06-09 08:55:03.195424 marko-1.3.1/marko/__main__.py
+-rw-r--r--   0        0        0     3805 2023-06-09 08:55:03.195424 marko-1.3.1/marko/ast_renderer.py
+-rw-r--r--   0        0        0    20405 2023-06-09 08:55:03.195424 marko-1.3.1/marko/block.py
+-rw-r--r--   0        0        0     2500 2023-06-09 08:55:03.199424 marko-1.3.1/marko/cli.py
+-rw-r--r--   0        0        0      793 2023-06-09 08:55:03.199424 marko-1.3.1/marko/element.py
+-rw-r--r--   0        0        0      105 2023-06-09 08:55:03.199424 marko-1.3.1/marko/ext/__init__.py
+-rw-r--r--   0        0        0     1832 2023-06-09 08:55:03.199424 marko-1.3.1/marko/ext/codehilite.py
+-rw-r--r--   0        0        0     3159 2023-06-09 08:55:03.199424 marko-1.3.1/marko/ext/footnote.py
+-rw-r--r--   0        0        0     2758 2023-06-09 08:55:03.199424 marko-1.3.1/marko/ext/gfm/__init__.py
+-rw-r--r--   0        0        0     7120 2023-06-09 08:55:03.199424 marko-1.3.1/marko/ext/gfm/elements.py
+-rw-r--r--   0        0        0     5132 2023-06-09 08:55:03.199424 marko-1.3.1/marko/ext/latex_renderer.py
+-rw-r--r--   0        0        0      988 2023-06-09 08:55:03.199424 marko-1.3.1/marko/ext/pangu.py
+-rw-r--r--   0        0        0     2544 2023-06-09 08:55:03.199424 marko-1.3.1/marko/ext/toc.py
+-rw-r--r--   0        0        0     7670 2023-06-09 08:55:03.199424 marko-1.3.1/marko/helpers.py
+-rw-r--r--   0        0        0     5029 2023-06-09 08:55:03.199424 marko-1.3.1/marko/html_renderer.py
+-rw-r--r--   0        0        0     5542 2023-06-09 08:55:03.199424 marko-1.3.1/marko/inline.py
+-rw-r--r--   0        0        0    17695 2023-06-09 08:55:03.199424 marko-1.3.1/marko/inline_parser.py
+-rw-r--r--   0        0        0     5669 2023-06-09 08:55:03.199424 marko-1.3.1/marko/md_renderer.py
+-rw-r--r--   0        0        0     4562 2023-06-09 08:55:03.199424 marko-1.3.1/marko/parser.py
+-rw-r--r--   0        0        0     3308 2023-06-09 08:55:03.199424 marko-1.3.1/marko/patterns.py
+-rw-r--r--   0        0        0        0 2023-06-09 08:55:03.199424 marko-1.3.1/marko/py.typed
+-rw-r--r--   0        0        0     3392 2023-06-09 08:55:03.199424 marko-1.3.1/marko/renderer.py
+-rw-r--r--   0        0        0     1367 2023-06-09 08:55:03.199424 marko-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1844 2023-06-09 08:55:03.199424 marko-1.3.1/tests/__init__.py
+-rw-r--r--   0        0        0     2175 2023-06-09 08:55:03.199424 marko-1.3.1/tests/benchmark.py
+-rw-r--r--   0        0        0     6879 2023-06-09 08:55:03.199424 marko-1.3.1/tests/normalize.py
+-rw-r--r--   0        0        0    13117 2023-06-09 08:55:03.199424 marko-1.3.1/tests/samples/jquery.md
+-rw-r--r--   0        0        0     2566 2023-06-09 08:55:03.199424 marko-1.3.1/tests/samples/syntax.md
+-rw-r--r--   0        0        0   204971 2023-06-09 08:55:03.203425 marko-1.3.1/tests/spec/commonmark.txt
+-rw-r--r--   0        0        0   216867 2023-06-09 08:55:03.203425 marko-1.3.1/tests/spec/gfm.txt
+-rw-r--r--   0        0        0      483 2023-06-09 08:55:03.199424 marko-1.3.1/tests/spec.sh
+-rw-r--r--   0        0        0     4280 2023-06-09 08:55:03.203425 marko-1.3.1/tests/test_basic.py
+-rw-r--r--   0        0        0     3371 2023-06-09 08:55:03.203425 marko-1.3.1/tests/test_ext.py
+-rw-r--r--   0        0        0     1745 2023-06-09 08:55:03.203425 marko-1.3.1/tests/test_helpers.py
+-rw-r--r--   0        0        0     7590 2023-06-09 08:55:03.203425 marko-1.3.1/tests/test_latex.py
+-rw-r--r--   0        0        0     2619 2023-06-09 08:55:03.203425 marko-1.3.1/tests/test_spec.py
+-rw-r--r--   0        0        0     4343 1970-01-01 00:00:00.000000 marko-1.3.1/PKG-INFO
```

### Comparing `marko-1.3.0/LICENSE` & `marko-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `marko-1.3.0/README.md` & `marko-1.3.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 ![Build Status](https://github.com/frostming/marko/workflows/Tests/badge.svg)
 [![codecov](https://codecov.io/gh/frostming/marko/branch/master/graph/badge.svg)](https://codecov.io/gh/frostming/marko)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/b785f5b3fa7c4d93a02372d31b3f73b1)](https://www.codacy.com/app/frostming/marko?utm_source=github.com&utm_medium=referral&utm_content=frostming/marko&utm_campaign=Badge_Grade)
 
 Marko is a markdown parser written in pure Python that complies with [CommonMark's spec v0.30][spec].
 It is designed to be highly extensible, see [Extensions](#extensions) for details.
 
-Marko requires Python 3.6 or higher.
+Marko requires Python 3.7 or higher.
 
 ## Why Marko
 
 Among all implementations of Python's markdown parser, it is a common issue that user can't easily extend it to add his own features. Furthermore, [Python-Markdown][pymd] and [mistune][mistune] don't comply with CommonMark's spec. It is a good reason for me to develop a new markdown parser.
 
 Respecting that Marko complies with CommonMark's spec at the same time, which is a super complicated spec, Marko's performance will be affected. However, using a parser
 which doesn't comply with the CommonMark spec may give you unexpected rendered results from time to time.
```

### Comparing `marko-1.3.0/marko/__init__.py` & `marko-1.3.1/marko/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,27 +7,26 @@
  A markdown parser with high extensibility.
 
  Licensed under MIT.
  Created by Frost Ming<mianghong@gmail.com>
 """
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, cast
+from typing import TYPE_CHECKING, Iterable, cast
 
-from .helpers import load_extension_object
+from .helpers import load_extension
 from .html_renderer import HTMLRenderer
 from .parser import Parser
 from .renderer import Renderer
 
 if TYPE_CHECKING:
-
     from .block import Document
     from .parser import ElementType
 
-__version__ = "1.3.0"
+__version__ = "1.3.1"
 
 
 class SetupDone(Exception):
     def __str__(self) -> str:
         return "Unable to register more extensions after setup done."
 
 
@@ -44,55 +43,59 @@
         See document of :meth:`Markdown.use()`.
     """
 
     def __init__(
         self,
         parser: type[Parser] = Parser,
         renderer: type[Renderer] = HTMLRenderer,
-        extensions: Any | None = None,
+        extensions: Iterable[str | object] | None = None,
     ) -> None:
         if not issubclass(parser, Parser):
             raise TypeError("parser must be a subclass of Parser.")
         self._base_parser = parser
-        self._parser_mixins: list[Any] = []
+        self._parser_mixins: list[type] = []
 
         if not issubclass(renderer, Renderer):
             raise TypeError("renderer must be a subclass of Renderer.")
         self._base_renderer = renderer
-        self._renderer_mixins: list[Any] = []
+        self._renderer_mixins: list[type] = []
 
         self._extra_elements: list[ElementType] = []
         self._setup_done = False
         if extensions:
             self.use(*extensions)
 
-    def use(self, *extensions: Any) -> None:
+    def use(self, *extensions: str | object) -> None:
         r"""Register extensions to Markdown object.
         An extension should be either an object providing ``elements``, `parser_mixins``
         , ``renderer_mixins`` or all attributes, or a string representing the
         corresponding extension in ``marko.ext`` module.
 
         :param \*extensions: extension object or string.
 
         .. note:: Marko uses a mixin based extension system, the order of extensions
             matters: An extension preceding in order will have higher priorty.
         """
         if self._setup_done:
             raise SetupDone()
         for extension in extensions:
             if isinstance(extension, str):
-                extension = load_extension_object(extension)()
+                extension = load_extension(extension)
 
             self._parser_mixins = (
-                getattr(extension, "parser_mixins", []) + self._parser_mixins
+                cast("list[type]", getattr(extension, "parser_mixins", []))
+                + self._parser_mixins
             )
             self._renderer_mixins = (
-                getattr(extension, "renderer_mixins", []) + self._renderer_mixins
+                cast("list[type]", getattr(extension, "renderer_mixins", []))
+                + self._renderer_mixins
+            )
+            self._extra_elements.extend(
+                cast("list[ElementType]", getattr(extension, "elements", []))
             )
-            self._extra_elements.extend(getattr(extension, "elements", []))
 
     def _setup_extensions(self) -> None:
         """Install all extensions and set things up."""
         if self._setup_done:
             return
         self.parser: Parser = type(
             "MarkdownParser", tuple(self._parser_mixins) + (self._base_parser,), {}
```

### Comparing `marko-1.3.0/marko/ast_renderer.py` & `marko-1.3.1/marko/ast_renderer.py`

 * *Files identical despite different names*

### Comparing `marko-1.3.0/marko/block.py` & `marko-1.3.1/marko/block.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Block level elements
 """
 from __future__ import annotations
 
 import re
-from typing import Any, Match, cast
+from typing import Any, Match, Pattern, cast
 
 from . import inline, inline_parser, patterns
 from .element import Element
 from .helpers import Source, find_next, normalize_label, partition_by_spaces
 from .parser import Parser
 
 __all__ = (
@@ -39,24 +39,24 @@
     #: Whether children are parsed as inline elements.
     inline_children = False
     #: If true, will replace the element which it derives from.
     override = False
     _prefix = ""
 
     @classmethod
-    def match(self, source: Source) -> Any:
+    def match(cls, source: Source) -> Any:
         """Test if the source matches the element at current position.
         The source should not be consumed in the method unless you have to.
 
         :param source: the ``Source`` object of the content to be parsed
         """
         raise NotImplementedError()
 
     @classmethod
-    def parse(self, source: Source) -> Any:
+    def parse(cls, source: Source) -> Any:
         """Parses the source. This is a proper place to consume the source body and
         return an element or information to build one. The information tuple will be
         passed to ``__init__`` method afterwards. Inline parsing, if any, should also
         be performed here.
 
         :param source: the ``Source`` object of the content to be parsed
         """
@@ -119,24 +119,24 @@
     priority = 6
     pattern = re.compile(
         r" {0,3}(#{1,6})((?=\s)[^\n]*?|[^\n\S]*)(?:(?<=\s)(?<!\\)#+)?[^\n\S]*$\n?",
         flags=re.M,
     )
     inline_children = True
 
-    def __init__(self, match: Match) -> None:
+    def __init__(self, match: Match[str]) -> None:
         self.level = len(match.group(1))
         self.children = match.group(2).strip()
 
     @classmethod
-    def match(cls, source: Source) -> Match | None:
+    def match(cls, source: Source) -> Match[str] | None:
         return source.expect_re(cls.pattern)
 
     @classmethod
-    def parse(cls, source: Source) -> Match | None:
+    def parse(cls, source: Source) -> Match[str] | None:
         m = source.match
         source.consume()
         return m
 
 
 class SetextHeading(BlockElement):
     """Setext heading: (Hello\n===\n)
@@ -220,15 +220,15 @@
 
     def __init__(self, match: tuple[str, str, str]) -> None:
         self.lang = inline.Literal.strip_backslash(match[0])
         self.extra = match[1]
         self.children = [inline.RawText(match[2], False)]
 
     @classmethod
-    def match(cls, source: Source) -> Match | None:
+    def match(cls, source: Source) -> Match[str] | None:
         m = source.expect_re(cls.pattern)
         if not m:
             return None
         prefix, leading, info = m.groups()
         if leading[0] == "`" and "`" in info:
             return None
         lang, _, extra = partition_by_spaces(info)
@@ -277,15 +277,15 @@
         return cls()
 
 
 class HTMLBlock(BlockElement):
     """HTML blocks, parsed as it is"""
 
     priority = 5
-    _end_cond = None  # Optional[Match]
+    _end_cond: Pattern[str] | None = None
 
     def __init__(self, lines: str) -> None:
         self.children = lines
 
     @classmethod
     def match(cls, source: Source) -> int | bool:
         if source.expect_re(r"(?i) {,3}<(script|pre|style|textarea)[>\s]"):
@@ -423,15 +423,15 @@
 class Quote(BlockElement):
     """block quote element: (> hello world)"""
 
     priority = 6
     _prefix = r" {,3}>[^\n\S]?"
 
     @classmethod
-    def match(cls, source: Source) -> Match | None:
+    def match(cls, source: Source) -> Match[str] | None:
         return source.expect_re(r" {,3}>")
 
     @classmethod
     def parse(cls, source: Source) -> Quote:
         state = cls()
         with source.under_state(state):
             state.children = parser.parse(source)  # type: ignore
```

### Comparing `marko-1.3.0/marko/cli.py` & `marko-1.3.1/marko/cli.py`

 * *Files identical despite different names*

### Comparing `marko-1.3.0/marko/element.py` & `marko-1.3.1/marko/element.py`

 * *Files identical despite different names*

### Comparing `marko-1.3.0/marko/ext/codehilite.py` & `marko-1.3.1/marko/ext/codehilite.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,28 +10,37 @@
     All arguments are passed to ``pygments.formatters.html.HtmlFormatter``.
 
 Usage::
 
     from marko import Markdown
 
     markdown = Markdown(extensions=['codehilite'])
-    markdown.convert(```python my_script.py\nprint('hello world')\n```)
+    markdown.convert('```python filename="my_script.py"\nprint('hello world')\n```')
 """
 import json
 
 from pygments import highlight
 from pygments.formatters import html
 from pygments.lexers import get_lexer_by_name, guess_lexer
 from pygments.util import ClassNotFound
 
 
 def _parse_extras(line):
     if not line:
         return {}
-    return {k: json.loads(v) for part in line.split(",") for k, v in [part.split("=")]}
+    extras = {}
+    for token in line.split(","):
+        k, has_eq, v = token.partition("=")
+        if has_eq:
+            try:
+                parsed_v = json.loads(v)
+                extras[k] = parsed_v
+            except json.JSONDecodeError:
+                continue
+    return extras
 
 
 class CodeHiliteRendererMixin:
     options = {}  # type: dict
 
     def render_fenced_code(self, element):
         code = element.children[0].children
```

### Comparing `marko-1.3.0/marko/ext/footnote.py` & `marko-1.3.1/marko/ext/footnote.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 class Document(block.Document):
     def __init__(self, text):
         self.footnotes = {}
         super().__init__(text)
 
 
 class FootnoteDef(block.BlockElement):
-
     pattern = re.compile(r" {,3}\[\^([^\]]+)\]:[^\n\S]*(?=\S| {4})")
     priority = 6
 
     def __init__(self, match):
         self.label = helpers.normalize_label(match.group(1))
         self._prefix = re.escape(match.group())
         self._second_prefix = r" {1,4}"
@@ -44,15 +43,14 @@
         with source.under_state(state):
             state.children = block.parser.parse(source)
         source.root.footnotes[state.label] = state
         return state
 
 
 class FootnoteRef(inline.InlineElement):
-
     pattern = re.compile(r"\[\^([^\]]+)\]")
     priority = 6
 
     def __init__(self, match):
         self.label = helpers.normalize_label(match.group(1))
 
     @classmethod
```

### Comparing `marko-1.3.0/marko/ext/gfm/__init__.py` & `marko-1.3.1/marko/ext/gfm/__init__.py`

 * *Files identical despite different names*

### Comparing `marko-1.3.0/marko/ext/gfm/elements.py` & `marko-1.3.1/marko/ext/gfm/elements.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import itertools
 import re
 
 from marko import block, inline, patterns
 
 
 class Paragraph(block.Paragraph):
-
     _task_list_item_pattern = re.compile(r"(\[[\sxX]\])\s+\S")
     override = True
 
     def __init__(self, lines):
         super().__init__(lines)
         m = self._task_list_item_pattern.match(self.children)
         if m:
@@ -29,15 +28,14 @@
         r"|<![A-Z]+ +[\s\S]*?>"  # declaration
         r"|<!\[CDATA\[[\s\S]*?\]\]>)"  # CDATA section
         % (patterns.tag_name, patterns.attribute, patterns.tag_name)
     )
 
 
 class Strikethrough(inline.InlineElement):
-
     pattern = re.compile(r"(?<!~)(~|~~)([^~]+)\1(?!~)")
     priority = 5
     parse_children = True
     parse_group = 2
 
 
 class _MatchObj:
@@ -64,15 +62,14 @@
         return self._match.group(n)[start:end]
 
     def __getattr__(self, name):
         return getattr(self._match, name)
 
 
 class Url(inline.AutoLink):
-
     www_pattern = re.compile(
         r"(?:^|(?<=[\s*_~(\uff00-\uffef]))(www\.([\w.\-]*?\.[\w.\-]+)[^<\s]*)"
     )
     email_pattern = r"[\w.\-+]+@[\w.\-]*?\.[\w.\-]*[a-zA-Z0-9]"
     bare_pattern = re.compile(
         r"(?:^|(?<=[\s*_~(\uff00-\uffef]))((?:https?|ftp)://([\w.\-]*?\.[\w.\-]+)"
         r"[^<\s]*|%s(?=[\s.<]|\Z))" % email_pattern
@@ -104,15 +101,14 @@
                 m = re.search(r"&[a-zA-Z]+;$", link_text)
                 if m:
                     match = _MatchObj(match, end_shift=-len(m.group()))
             yield match
 
 
 class ListItem(block.ListItem):
-
     pattern = re.compile(r" {,3}(\d{1,9}[.)]|[*\-+])[ \t\n\r\f]")
     override = True
 
 
 class Table(block.BlockElement):
     """A table element."""
```

### Comparing `marko-1.3.0/marko/ext/latex_renderer.py` & `marko-1.3.1/marko/ext/latex_renderer.py`

 * *Files identical despite different names*

### Comparing `marko-1.3.0/marko/ext/pangu.py` & `marko-1.3.1/marko/ext/pangu.py`

 * *Files identical despite different names*

### Comparing `marko-1.3.0/marko/ext/toc.py` & `marko-1.3.1/marko/ext/toc.py`

 * *Files identical despite different names*

### Comparing `marko-1.3.0/marko/helpers.py` & `marko-1.3.1/marko/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,26 +3,17 @@
 """
 from __future__ import annotations
 
 import functools
 import re
 from contextlib import contextmanager
 from importlib import import_module
-from typing import (
-    TYPE_CHECKING,
-    Callable,
-    Container,
-    Generator,
-    Iterable,
-    Match,
-    Pattern,
-)
+from typing import TYPE_CHECKING, Container, Generator, Iterable, Match, Pattern
 
 if TYPE_CHECKING:
-
     from .block import BlockElement
 
 
 def camel_to_snake_case(name: str) -> str:
     """Takes a camelCased string and converts to snake_case."""
     pattern = r"[A-Z][a-z]+|[A-Z]+(?![a-z])"
     return "_".join(map(str.lower, re.findall(pattern, name)))
@@ -233,15 +224,15 @@
     if start < 0:
         return text, "", ""
     if end < 0:
         return text[:start], text[start:], ""
     return text[:start], text[start:end], text[end:]
 
 
-def load_extension_object(name: str) -> Callable:
+def load_extension(name: str) -> object:
     """Load extension object from a string.
     First try `marko.ext.<name>` if possible
     """
     module = None
     if "." not in name:
         try:
             module = import_module(f"marko.ext.{name}")
@@ -250,12 +241,12 @@
     if module is None:
         try:
             module = import_module(name)
         except ImportError as e:
             raise ImportError(f"Extension {name} cannot be imported") from e
 
     try:
-        return module.make_extension
+        return module.make_extension()
     except AttributeError:
         raise AttributeError(
             f"Module {name} does not have 'make_extension' attributte."
         ) from None
```

### Comparing `marko-1.3.0/marko/html_renderer.py` & `marko-1.3.1/marko/html_renderer.py`

 * *Files identical despite different names*

### Comparing `marko-1.3.0/marko/inline.py` & `marko-1.3.1/marko/inline.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,14 @@
 
     def __init__(self, match: _Match) -> None:
         self.soft = not match.group(1).startswith(("  ", "\\"))
         self.children = "\n"
 
 
 class InlineHTML(InlineElement):
-
     priority = 7
     pattern = re.compile(
         r"(<%s(?:%s)* */?>"  # open tag
         r"|</%s *>"  # closing tag
         r"|<!--(?!>|->|[\s\S]*?--[\s\S]*?-->)[\s\S]*?(?<!-)-->"  # HTML comment
         r"|<\?[\s\S]*?\?>"  # processing instruction
         r"|<![A-Z]+ +[\s\S]*?>"  # declaration
```

### Comparing `marko-1.3.0/marko/inline_parser.py` & `marko-1.3.1/marko/inline_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
 
 def make_elements(
     tokens: list[Token],
     text: str,
     start: int = 0,
     end: int | None = None,
-    fallback: ElementType = None,
+    fallback: ElementType | None = None,
 ) -> list[InlineElement]:
     """Make elements from a list of parsed tokens.
     It will turn all unmatched holes into fallback elements.
 
     :param tokens: a list of parsed tokens.
     :param text: the original tet.
     :param start: the offset of where parsing starts. Defaults to the start of text.
```

### Comparing `marko-1.3.0/marko/md_renderer.py` & `marko-1.3.1/marko/md_renderer.py`

 * *Files identical despite different names*

### Comparing `marko-1.3.0/marko/parser.py` & `marko-1.3.1/marko/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Base parser
 """
 from __future__ import annotations
 
 import itertools
-from typing import TYPE_CHECKING, AnyStr, Type
+from typing import TYPE_CHECKING, Type
 
 from .helpers import Source
 
 
 class Parser:
     r"""
     All elements defined in CommonMark's spec are included in the parser
@@ -51,15 +51,15 @@
             raise TypeError(
                 "The element should be a subclass of either `BlockElement` or "
                 "`InlineElement`."
             )
         dest[element.get_type()] = element
 
     def parse(
-        self, source_or_text: Source | AnyStr
+        self, source_or_text: Source | str
     ) -> list[block.BlockElement] | block.BlockElement:
         """Do the actual parsing and returns an AST or parsed element.
 
         :param source_or_text: the text or source object.
             Based on the type, it will do following:
             - text: returns the parsed Document element.
             - source: parse the source and returns the parsed children as a list.
```

### Comparing `marko-1.3.0/marko/patterns.py` & `marko-1.3.1/marko/patterns.py`

 * *Files identical despite different names*

### Comparing `marko-1.3.0/marko/renderer.py` & `marko-1.3.1/marko/renderer.py`

 * *Files identical despite different names*

### Comparing `marko-1.3.0/pyproject.toml` & `marko-1.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
-version = "1.3.0"
+version = "1.3.1"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/frostming/marko"
 Documentation = "https://marko-py.readthedocs.io"
```

### Comparing `marko-1.3.0/tests/__init__.py` & `marko-1.3.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `marko-1.3.0/tests/benchmark.py` & `marko-1.3.1/tests/benchmark.py`

 * *Files identical despite different names*

### Comparing `marko-1.3.0/tests/normalize.py` & `marko-1.3.1/tests/normalize.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
             self.output = self.output.rstrip()
         self.output += "<" + tag
         # For now we don't strip out 'extra' attributes, because of
         # raw HTML test cases.
         # attrs = filter(lambda attr: attr[0] in significant_attrs, attrs)
         if attrs:
             attrs.sort()
-            for (k, v) in attrs:
+            for k, v in attrs:
                 self.output += " " + k
                 if v in ["href", "src"]:
                     self.output += (
                         "=" + '"' + urllib.quote(urllib.unquote(v), safe="/") + '"'
                     )
                 elif v is not None:
                     self.output += "=" + '"' + escape(v, quote=True) + '"'
```

### Comparing `marko-1.3.0/tests/samples/jquery.md` & `marko-1.3.1/tests/samples/jquery.md`

 * *Files identical despite different names*

### Comparing `marko-1.3.0/tests/samples/syntax.md` & `marko-1.3.1/tests/samples/syntax.md`

 * *Files identical despite different names*

### Comparing `marko-1.3.0/tests/spec/commonmark.txt` & `marko-1.3.1/tests/spec/commonmark.txt`

 * *Files identical despite different names*

### Comparing `marko-1.3.0/tests/spec/gfm.txt` & `marko-1.3.1/tests/spec/gfm.txt`

 * *Files identical despite different names*

### Comparing `marko-1.3.0/tests/test_basic.py` & `marko-1.3.1/tests/test_basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,23 +41,21 @@
         assert normalize_html(marko.convert(rerendered)) == normalize_html(
             marko.convert(text)
         )
 
 
 class TestExtension:
     def test_extension_use(self):
-
         markdown = marko.Markdown(extensions=["footnote", "toc"])
 
         assert len(markdown._extra_elements) == 3
         assert len(markdown._renderer_mixins) == 2
         assert hasattr(markdown._renderer_mixins[1], "render_footnote_def")
 
     def test_extension_setup(self):
-
         markdown = marko.Markdown()
         markdown.use("footnote")
 
         markdown.convert("abc")
         with pytest.raises(marko.SetupDone, match="Unable to register more extensions"):
             markdown.use("toc")
```

### Comparing `marko-1.3.0/tests/test_ext.py` & `marko-1.3.1/tests/test_ext.py`

 * *Files identical despite different names*

### Comparing `marko-1.3.0/tests/test_helpers.py` & `marko-1.3.1/tests/test_helpers.py`

 * *Files 23% similar despite different names*

```diff
@@ -37,30 +37,30 @@
         source.root
 
     with pytest.raises(RuntimeError, match="Need to push a state first"):
         source.state
 
 
 def test_load_extension_object():
-    ext = helpers.load_extension_object("pangu")()
+    ext = helpers.load_extension("pangu")
     assert len(ext.renderer_mixins) == 1
 
-    ext = helpers.load_extension_object("marko.ext.pangu")()
+    ext = helpers.load_extension("marko.ext.pangu")
     assert len(ext.renderer_mixins) == 1
 
     with pytest.raises(ImportError, match="Extension foobar cannot be imported"):
-        helpers.load_extension_object("foobar")()
+        helpers.load_extension("foobar")
 
 
 def test_load_illegal_extension_object():
     with pytest.raises(
         AttributeError,
         match="Module marko.block does not have 'make_extension' attributte",
     ):
-        helpers.load_extension_object("marko.block")()
+        helpers.load_extension("marko.block")
 
 
 @pytest.mark.parametrize(
     "text, expected",
     [
         ("hello world", ("hello", " ", "world")),
         ("hello", ("hello", "", "")),
```

### Comparing `marko-1.3.0/tests/test_latex.py` & `marko-1.3.1/tests/test_latex.py`

 * *Files identical despite different names*

### Comparing `marko-1.3.0/tests/test_spec.py` & `marko-1.3.1/tests/test_spec.py`

 * *Files identical despite different names*

### Comparing `marko-1.3.0/PKG-INFO` & `marko-1.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marko
-Version: 1.3.0
+Version: 1.3.1
 Summary: A markdown parser with high extensibility.
 License: MIT
 Author-email: Frost Ming <mianghong@gmail.com>
 Requires-Python: >=3.7
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -32,15 +32,15 @@
 ![Build Status](https://github.com/frostming/marko/workflows/Tests/badge.svg)
 [![codecov](https://codecov.io/gh/frostming/marko/branch/master/graph/badge.svg)](https://codecov.io/gh/frostming/marko)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/b785f5b3fa7c4d93a02372d31b3f73b1)](https://www.codacy.com/app/frostming/marko?utm_source=github.com&utm_medium=referral&utm_content=frostming/marko&utm_campaign=Badge_Grade)
 
 Marko is a markdown parser written in pure Python that complies with [CommonMark's spec v0.30][spec].
 It is designed to be highly extensible, see [Extensions](#extensions) for details.
 
-Marko requires Python 3.6 or higher.
+Marko requires Python 3.7 or higher.
 
 ## Why Marko
 
 Among all implementations of Python's markdown parser, it is a common issue that user can't easily extend it to add his own features. Furthermore, [Python-Markdown][pymd] and [mistune][mistune] don't comply with CommonMark's spec. It is a good reason for me to develop a new markdown parser.
 
 Respecting that Marko complies with CommonMark's spec at the same time, which is a super complicated spec, Marko's performance will be affected. However, using a parser
 which doesn't comply with the CommonMark spec may give you unexpected rendered results from time to time.
```

