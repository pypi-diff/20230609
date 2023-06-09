# Comparing `tmp/arguably-1.0.2.tar.gz` & `tmp/arguably-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arguably-1.0.2.tar", max compression
+gzip compressed data, was "arguably-1.1.0.tar", max compression
```

## Comparing `arguably-1.0.2.tar` & `arguably-1.1.0.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0     1538 2023-06-08 13:05:22.603853 arguably-1.0.2/LICENSE.txt
--rw-r--r--   0        0        0    72461 2023-06-08 13:05:22.603853 arguably-1.0.2/arguably/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 13:05:22.603853 arguably-1.0.2/arguably/py.typed
--rw-r--r--   0        0        0     5135 2023-06-08 13:05:22.603853 arguably-1.0.2/assets/PYPI_README.md
--rw-r--r--   0        0        0      917 2023-06-08 13:05:22.603853 arguably-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     5845 1970-01-01 00:00:00.000000 arguably-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1538 2023-06-09 14:58:02.626738 arguably-1.1.0/LICENSE.txt
+-rw-r--r--   0        0        0    75984 2023-06-09 14:58:02.626738 arguably-1.1.0/arguably/__init__.py
+-rw-r--r--   0        0        0     2200 2023-06-09 14:58:02.626738 arguably-1.1.0/arguably/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-09 14:58:02.626738 arguably-1.1.0/arguably/py.typed
+-rw-r--r--   0        0        0     4735 2023-06-09 14:58:02.626738 arguably-1.1.0/arguably/util.py
+-rw-r--r--   0        0        0     5177 2023-06-09 14:58:02.626738 arguably-1.1.0/assets/PYPI_README.md
+-rw-r--r--   0        0        0      917 2023-06-09 14:58:02.630738 arguably-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5887 1970-01-01 00:00:00.000000 arguably-1.1.0/PKG-INFO
```

### Comparing `arguably-1.0.2/LICENSE.txt` & `arguably-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `arguably-1.0.2/arguably/__init__.py` & `arguably-1.1.0/arguably/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,24 +58,26 @@
     Dict,
     Type,
     Tuple,
 )
 
 from docstring_parser import parse as docparse
 
+from arguably.util import warn, logger
+
 # Annotated is 3.9 and up
 if sys.version_info >= (3, 9):
     from typing import Annotated, get_type_hints, get_args, get_origin
-else:
+else:  # pragma: no cover
     from typing_extensions import Annotated, get_type_hints, get_args, get_origin
 
 # UnionType is the new type for the `A | B` type syntax, which is 3.10 and up
 if sys.version_info >= (3, 10):
     from types import UnionType
-else:
+else:  # pragma: no cover
 
     class UnionType:
         """Stub this out, we only use it for issubclass() checks"""
 
 
 ########################################################################################################################
 ########################################################################################################################
@@ -540,14 +542,15 @@
                 continue
             arg_description = doc_item.description or ""
 
             found = True
             break
 
         if not found and item.name in enum_member_docs:
+            # noinspection PyTypeChecker
             arg_description = enum_member_docs[item.name]
 
         # Extract the alias from the docstring for the flag item
         if alias_match := re.match(r"^\[-([a-zA-Z0-9])] ", arg_description):
             arg_description = arg_description[len(alias_match.group(0)) :]
             options.insert(0, f"-{alias_match.group(1)}")
 
@@ -584,28 +587,21 @@
 
 @dataclass
 class _CommandDecoratorInfo:
     """Used for keeping a reference to everything marked with @arguably.command"""
 
     function: Callable
     alias: Optional[str] = None
+    name: str = field(init=False)
 
-    @property
-    def name(self) -> str:
-        """
-        We need to know the name pretty early on, so the method to calculate it lives here. This calculates the name as
-        the user should see it. Rules:
-          * `__root__` is left as-is
-          * Leading or trailing `_` are stripped.
-          * `__` becomes space ` `
-          * `_` becomes `-`
-        """
+    def __post_init__(self) -> None:
         if self.function.__name__ == "__root__":
-            return "__root__"
-        return _normalize_name(self.function.__name__)
+            self.name = "__root__"
+        else:
+            self.name = _normalize_name(self.function.__name__)
 
 
 @dataclass
 class _SubtypeDecoratorInfo:
     """Used for keeping a reference to everything marked with @arguably.subtype"""
 
     type_: type
@@ -937,39 +933,44 @@
     Options for arguably
 
     :ivar name: Name of the script/program. Defaults to the filename or module name (depending on invocation method).
 
     :ivar call_ancestors: Normally false. If true, `git init` will first call `git()`, then `git__init()`. Calls all
         members of the hierarchy. This allows parents to handle options. Parents can determine if they are actually the
         target command (instead of being called through the heirarchy) through the `is_target()` method.
+    :ivar always_subcommand: Normally false. If true, will force a subcommand interface to be used, even if there's only
+        one command.
     :ivar auto_alias_cmds: Normally false. If true, will automatically create a short alias for every command. See
         `_find_alias` for implementation.
     :ivar auto_alias_params: Normally false. If true, will automatically create a short alias for every parameter
         (example: `-v` for `--verbose`). See `_find_alias` for implementation.
     :ivar version_flag: Normally false. If true, will set up version printing using `__version__` and add options to
         the root parser.
 
     :ivar show_defaults: Show default values for optional arguments.
+    :ivar show_types: Show the type of each argument.
     :ivar command_metavar: Allows you to change how the subcommand placeholder appears in the usage string.
     :ivar max_description_offset: The maximum number of columns before argument descriptions are printed. Equivalent to
         `max_help_position` in argparse.
     :ivar max_width: The total maximum width of text to be displayed in the terminal. Equivalent to `width` in argparse.
     :ivar output: Where argparse output should be written - can write to a file, stderr, or anything similar.
     """
 
     name: Optional[str]
 
     # Behavior options
     call_ancestors: bool
+    always_subcommand: bool
     auto_alias_cmds: bool
     auto_alias_params: bool
     version_flag: Union[bool, List[str]]
 
     # Formatting options
     show_defaults: bool
+    show_types: bool
     command_metavar: str
     max_description_offset: int
     max_width: int
     output: Optional[TextIO]
 
     def __post_init__(self) -> None:
         # When running as a module, show the script name as the module path.
@@ -1011,14 +1012,18 @@
 
         # These are really only set and used in the run() method
         self._commands: Dict[str, _Command] = dict()
         self._command_aliases: Dict[str, str] = dict()
         self._parsers: Dict[str, argparse.ArgumentParser] = dict()
         self._subparsers: Dict[str, Any] = dict()
 
+    def reset(self) -> None:
+        self.__dict__.clear()
+        self.__init__()  # type: ignore[misc]
+
     def add_command(self, **kwargs: Any) -> None:
         """Invoked by `@arguably.command`, saves info about a command to include when the parser is set up."""
         info = _CommandDecoratorInfo(**kwargs)
         self._command_decorator_info.append(info)
 
     def add_subtype(self, **kwargs: Any) -> None:
         """Invoked by `@arguably.subtype`, saves info about a how to construct a type."""
@@ -1045,24 +1050,29 @@
             prog, max_help_position=self._options.max_description_offset, width=self._options.max_width
         )
 
     def _process_decorator_info(self, info: _CommandDecoratorInfo) -> _Command:
         """Takes the decorator info and return a processed command"""
 
         processed_name = info.name
+        func = info.function.__init__ if isinstance(info.function, type) else info.function  # type: ignore[misc]
 
         # Get the description from the docstring
-        if info.function.__doc__ is None:
+        if func.__doc__ is None:
             docs = None
             processed_description = ""
         else:
-            docs = docparse(info.function.__doc__)
+            docs = docparse(func.__doc__)
             processed_description = "" if docs.short_description is None else docs.short_description
 
-        hints = get_type_hints(info.function, include_extras=True)
+        try:
+            hints = get_type_hints(func, include_extras=True)
+        except NameError as e:
+            hints = {}
+            warn(f"Unable to resolve type hints for function {processed_name}: {str(e)}", func)
 
         # Will be filled in as we loop over all parameters
         processed_args: List[_CommandArg] = list()
         used_arg_aliases: List[str] = list()
         has_positional_args = False
         variadic_positional_arg = None
 
@@ -1223,40 +1233,55 @@
                 if arg_.default is _NoDefault:
                     raise ArguablyException(
                         f"Function argument `{arg_.param_name}` in `{cmd.name}` is an enum.Flag. Due to implementation "
                         f"limitations, all enum.Flag parameters must have a default value."
                     )
                 parser.set_defaults(**{arg_.arg_name: arg_.default})
                 for entry in _info_for_flags(arg_.arg_name, arg_.arg_value_type):
+                    logger.debug(
+                        f'Parser({parser.prog.partition(" ")[2]!r}).add_argument('
+                        f"*{entry.option!r}, "
+                        f"action={_EnumFlagAction!r}, "
+                        f"const={entry!r}, "
+                        f"nargs={0!r}, "
+                        f"help={entry.description!r},)"
+                    )
                     parser.add_argument(
-                        *entry.option, action=_EnumFlagAction, const=entry, nargs=0, help=entry.description
+                        *entry.option,
+                        action=_EnumFlagAction,
+                        const=entry,
+                        nargs=0,
+                        help=entry.description,
                     )
                 continue
 
             # Optional kwargs for parser.add_argument
             add_arg_kwargs: Dict[str, Any] = dict(type=arg_.arg_value_type)
 
             arg_description = arg_.description
+            description_extras = []
+
+            # Show arg type?
+            if self._options.show_types:
+                description_extras.append(f"type: {arg_.arg_value_type.__name__}")
 
             # `default` value?
             if arg_.input_method.is_optional and arg_.default is not _NoDefault:
                 add_arg_kwargs.update(default=arg_.default)
                 if self._options.show_defaults:
-                    if len(arg_description) > 0:
-                        arg_description += " "
                     if isinstance(arg_.default, enum.Enum):
-                        arg_description += f"(default: {_normalize_name(arg_.default.name, spaces=False)})"
+                        description_extras.append(f"default: {_normalize_name(arg_.default.name, spaces=False)}")
                     elif isinstance(arg_.default, str):
                         str_default = arg_.default
                         # Use the string repr if it contains spaces, contains a newline, or is zero-length
                         if (" " in str_default) or ("\n" in str_default) or (len(str_default) == 0):
                             str_default = repr(str_default)
-                        arg_description += f"(default: {str_default})"
+                        description_extras.append(f"default: {str_default}")
                     else:
-                        arg_description += f"(default: {arg_.default})"
+                        description_extras.append(f"default: {arg_.default}")
 
             # Number of arguments `nargs`?
             if arg_.count is _CommandArg.ANY_COUNT:
                 add_arg_kwargs.update(nargs="*")
             elif arg_.input_method is _InputMethod.OPTIONAL_POSITIONAL:
                 add_arg_kwargs.update(nargs="?")
             elif arg_.count != 1:
@@ -1289,21 +1314,28 @@
                     )
                 # Use `store_true` or `store_false` for bools
                 add_arg_kwargs.update(action="store_true" if arg_.default is False else "store_false")
                 if "type" in add_arg_kwargs:
                     del add_arg_kwargs["type"]
 
             # Set the help description
+            if len(description_extras) > 0:
+                if len(arg_description) > 0:
+                    arg_description += " "
+                arg_description += f"({', '.join(description_extras)})"
             add_arg_kwargs.update(help=arg_description)
 
             # Run modifiers for this arg
             for modifier in arg_.modifiers:
                 modifier.modify_arg_dict(cmd, arg_, add_arg_kwargs)
 
             # Add the argument to the parser
+            logger.debug(
+                f'Parser({parser.prog.partition(" ")[2]!r}).add_argument(' f"*{arg_names!r}, " f"**{add_arg_kwargs!r})"
+            )
             parser.add_argument(*arg_names, **add_arg_kwargs)
 
     def _build_subparser_tree(self, command_decorator_info: _CommandDecoratorInfo) -> str:
         """Builds up the subparser tree for a given `_CommandDecoratorInfo`. Inserts dummy entries to `self._parsers`
         and `self._commands` if necessary. Returns the name of the parent for this command."""
 
         prev_ancestor = "__root__"
@@ -1314,24 +1346,41 @@
             required_subparser = False
             if ancestor not in self._commands:
                 # Dummy command - this ancestor doesn't have a function of its own, it's just a path.
                 self._commands[ancestor] = _Command(lambda *_, **__: None, ancestor)
             if ancestor not in self._parsers:
                 # Dummy parser - since there's nothing to run, require the subparser.
                 required_subparser = True
+                logger.debug(
+                    f"Subparsers({prev_ancestor!r}).add_parser("
+                    f'{ancestor.split(" ")[-1]!r}, '
+                    f'help={""!r}, '
+                    f"formatter_class={self._formatter!r}, "
+                    f"**{self._extra_argparser_options!r},)"
+                )
                 self._parsers[ancestor] = self._subparsers[prev_ancestor].add_parser(
-                    ancestor.split(" ")[-1], help="", formatter_class=self._formatter, **self._extra_argparser_options
+                    ancestor.split(" ")[-1],
+                    help="",
+                    formatter_class=self._formatter,
+                    **self._extra_argparser_options,
                 )
             if ancestor not in self._subparsers:
                 # Add subparser to the parent command's parser.
                 ancestor_cmd = self._commands[ancestor]
                 if ancestor_cmd.has_positional_args:
                     raise ArguablyException(
                         f"Command `{ancestor}` cannot have both subcommands and positional arguments."
                     )
+                logger.debug(
+                    f"Parser({ancestor!r}).add_subparsers("
+                    f"parser_class={_ArgumentParser!r}, "
+                    f"dest={ancestor_cmd.get_subcommand_metavar(self._options.command_metavar)!r}, "
+                    f"metavar={self._options.command_metavar!r}, "
+                    f"required={required_subparser!r},)"
+                )
                 self._subparsers[ancestor] = self._parsers[ancestor].add_subparsers(
                     parser_class=_ArgumentParser,
                     dest=ancestor_cmd.get_subcommand_metavar(self._options.command_metavar),
                     metavar=self._options.command_metavar,
                     required=required_subparser,
                 )
             prev_ancestor = ancestor
@@ -1346,18 +1395,20 @@
             raise ArguablyException("Unknown current parser.")
         self._current_parser.error(message)  # This will exit the script
 
     def run(
         self,
         name: Optional[str] = None,
         call_ancestors: bool = False,
+        always_subcommand: bool = False,
         auto_alias_cmds: bool = False,
         auto_alias_params: bool = False,
         version_flag: Union[bool, Tuple[str], Tuple[str, str]] = False,
         show_defaults: bool = True,
+        show_types: bool = False,
         max_description_offset: int = 60,
         max_width: int = 120,
         command_metavar: str = "command",
         output: Optional[TextIO] = None,
     ) -> Any:
         """Set up the argument parser, parse argv, and run the appropriate command(s)"""
 
@@ -1366,17 +1417,24 @@
         self._extra_argparser_options = dict(output=self._options.output)
 
         self._is_calling_target = False
 
         # Grab the description
         import __main__
 
-        description = "" if __main__.__doc__ is None else __main__.__doc__.partition("\n\n")[0]
+        description = "" if __main__.__doc__ is None else __main__.__doc__.partition("\n\n\n")[0]
 
         # Set up the root parser
+        logger.debug(
+            f'Initializing {"__root__"!r} parser: _ArgumentParser('
+            f"prog={self._options.name!r}, "
+            f"description={description!r}, "
+            f"formatter_class={self._formatter!r}, "
+            f"**{self._extra_argparser_options!r})"
+        )
         root_parser = _ArgumentParser(
             prog=self._options.name,
             description=description,
             formatter_class=self._formatter,
             **self._extra_argparser_options,
         )
         self._parsers["__root__"] = root_parser
@@ -1386,20 +1444,25 @@
         if self._options.version_flag:
             if not hasattr(__main__, "__version__"):
                 raise ArguablyException("__version__ must be defined if version_flag is set")
             if isinstance(self._options.version_flag, tuple):
                 argparse_version_flags = self._options.version_flag
             else:
                 argparse_version_flags = ("--version",)
-            root_parser.add_argument(
-                *argparse_version_flags, action="version", version=f"%(prog)s {__main__.__version__}"
+            version_string = f"%(prog)s {__main__.__version__}"
+            logger.debug(
+                f'Parser({"__root__"!r}).add_argument('
+                f"*{argparse_version_flags!r}, "
+                f'action={"version"!r}, '
+                f"version={version_string!r})"
             )
+            root_parser.add_argument(*argparse_version_flags, action="version", version=version_string)
 
         # Check the number of commands we have
-        only_one_cmd = len(self._command_decorator_info) == 1
+        only_one_cmd = (len(self._command_decorator_info) == 1) and not self._options.always_subcommand
         if len(self._command_decorator_info) == 0:
             raise ArguablyException("At least one command is required")
 
         for command_decorator_info in sorted(
             self._command_decorator_info, key=lambda v: (v.name != "__root__", v.name.count(" "))
         ):
             if only_one_cmd:
@@ -1425,14 +1488,23 @@
                         f"`{self._command_aliases[cmd.alias]}`"
                     )
                 self._command_aliases[cmd.alias] = cmd.name
             self._commands[cmd.name] = cmd
 
             # Add the parser for the command
             if not only_one_cmd and cmd.name != "__root__":
+                logger.debug(
+                    f"Subparsers({parent_name!r}).add_parser("
+                    f'{cmd.name.split(" ")[-1]!r}, '
+                    f"aliases={[cmd.alias] if cmd.alias is not None else []!r}, "
+                    f"help={cmd.description!r}, "
+                    f"description={cmd.description!r}, "
+                    f"formatter_class={self._formatter!r}, "
+                    f"**{self._extra_argparser_options!r})"
+                )
                 self._parsers[cmd.name] = self._subparsers[parent_name].add_parser(
                     cmd.name.split(" ")[-1],
                     aliases=[cmd.alias] if cmd.alias is not None else [],
                     help=cmd.description,
                     description=cmd.description,
                     formatter_class=self._formatter,
                     **self._extra_argparser_options,
@@ -1463,14 +1535,15 @@
 
         # Make the magic happen
         parsed_args = vars(root_parser.parse_args())
 
         # Resolve the command that needs to be called
         if only_one_cmd:
             cmd = next(iter(self._commands.values()))
+            self._current_parser = self._parsers["__root__"]
         else:
             # Find the actual command we need to execute by traversing the subparser tree. Call each stop along the way
             # if the call_ancestors option is set to True.
             path = "__root__"
             while path in self._subparsers:
                 # Find the variable name for this subparser's command metavar and read the value. If it's none, run the
                 # current stop of our path in the tree.
@@ -1578,16 +1651,20 @@
 
 
 ########################################################################################################################
 ########################################################################################################################
 # arguably API
 
 
+class ArguablyWarning(UserWarning):
+    """Raised when a decorated function is incorrectly set up in some way, but arguably can continue"""
+
+
 class ArguablyException(Exception):
-    """Raised when an annotated function is incorrectly set up in some way"""
+    """Raised when a decorated function is incorrectly set up in some way"""
 
 
 run = _context.run
 is_target = _context.is_calling_target
 error = _context.error
```

### Comparing `arguably-1.0.2/assets/PYPI_README.md` & `arguably-1.1.0/assets/PYPI_README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 <p align="center">
       <img alt="arguably logo" src="https://raw.githubusercontent.com/treykeown/arguably/main/assets/arguably_black.png">
 </p>
 
 <p align="center">
     <em>
-        turns functions into command line interfaces
+        the best CLI library, arguably<br>
+        turns your functions into command line interfaces
     </em>
 </p>
 
 <p align="center">
     <a href="https://github.com/treykeown/arguably/actions/workflows/python-package.yml"><img src="https://github.com/treykeown/arguably/actions/workflows/python-package.yml/badge.svg" alt="Test status"></a>
-    <a href="https://github.com/treykeown/arguably/tree/main/test"><img src="https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/treykeown/f493b14288af4e8358ea8578c393213a/raw/arguably-coverage-badge.json" alt="Code coverage"></a>
+    <a href="https://treykeown.github.io/arguably/coverage/"><img src="https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/treykeown/f493b14288af4e8358ea8578c393213a/raw/arguably-coverage-badge.json" alt="Code coverage"></a>
     <a href="https://pypi.org/project/arguably/"><img src="https://shields.io/pypi/pyversions/arguably" alt="Supported Python versions"></a>
     <a href="https://pypi.org/project/arguably/"><img src="https://shields.io/pypi/v/arguably" alt="PyPI version"></a>
 </p>
 <hr>
 
 `arguably` solves this problem:
 1. You've written a Python script
 2. Now you want to pass in parameters from the command line
 3. You don't want to read the docs for your favorite argument parsing library *again*
 
 By leveraging as many Python idioms as possible, `arguably` keeps its API small and memorable without sacrificing
-funcitonality. `arguably` uses functions and their docstrings to automatically set up argparse. Notably, `arguably`
+functionality. `arguably` uses functions and their docstrings to automatically set up argparse. Notably, `arguably`
 maps your function signature to a command-line interface like this:
 
 ```python
 @arguably.command
 def some_function(required, not_required="foo", *others, option="bar"):
     ...
 ```
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
                                 [arguably logo]
-                 turns functions into command line interfaces
+                        the best CLI library, arguably
+               turns your functions into command line interfaces
    [Test_status] [Code_coverage] [Supported_Python_versions] [PyPI_version]
 ===============================================================================
 `arguably` solves this problem: 1. You've written a Python script 2. Now you
 want to pass in parameters from the command line 3. You don't want to read the
 docs for your favorite argument parsing library *again* By leveraging as many
 Python idioms as possible, `arguably` keeps its API small and memorable without
-sacrificing funcitonality. `arguably` uses functions and their docstrings to
+sacrificing functionality. `arguably` uses functions and their docstrings to
 automatically set up argparse. Notably, `arguably` maps your function signature
 to a command-line interface like this: ```python @arguably.command def
 some_function(required, not_required="foo", *others, option="bar"): ... ```
                                     becomes
 ```text usage: script [--option OPTION] required [not-required] [others ...]
 ``` In short, `arguably` turns your function's **positional parameters** into
 **positional command-line arguments**, and your function's **keyword-only
```

### Comparing `arguably-1.0.2/pyproject.toml` & `arguably-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arguably"
-version = "1.0.2"
+version = "1.1.0"
 description = "turns functions into command line interfaces"
 authors = ["treykeown <2755914+treykeown@users.noreply.github.com>"]
 readme = "assets/PYPI_README.md"
 homepage = "https://github.com/treykeown/arguably"
 repository = "https://github.com/treykeown/arguably"
 
 [tool.poetry.dependencies]
```

### Comparing `arguably-1.0.2/PKG-INFO` & `arguably-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arguably
-Version: 1.0.2
+Version: 1.1.0
 Summary: turns functions into command line interfaces
 Home-page: https://github.com/treykeown/arguably
 Author: treykeown
 Author-email: 2755914+treykeown@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -18,33 +18,34 @@
 
 <p align="center">
       <img alt="arguably logo" src="https://raw.githubusercontent.com/treykeown/arguably/main/assets/arguably_black.png">
 </p>
 
 <p align="center">
     <em>
-        turns functions into command line interfaces
+        the best CLI library, arguably<br>
+        turns your functions into command line interfaces
     </em>
 </p>
 
 <p align="center">
     <a href="https://github.com/treykeown/arguably/actions/workflows/python-package.yml"><img src="https://github.com/treykeown/arguably/actions/workflows/python-package.yml/badge.svg" alt="Test status"></a>
-    <a href="https://github.com/treykeown/arguably/tree/main/test"><img src="https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/treykeown/f493b14288af4e8358ea8578c393213a/raw/arguably-coverage-badge.json" alt="Code coverage"></a>
+    <a href="https://treykeown.github.io/arguably/coverage/"><img src="https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/treykeown/f493b14288af4e8358ea8578c393213a/raw/arguably-coverage-badge.json" alt="Code coverage"></a>
     <a href="https://pypi.org/project/arguably/"><img src="https://shields.io/pypi/pyversions/arguably" alt="Supported Python versions"></a>
     <a href="https://pypi.org/project/arguably/"><img src="https://shields.io/pypi/v/arguably" alt="PyPI version"></a>
 </p>
 <hr>
 
 `arguably` solves this problem:
 1. You've written a Python script
 2. Now you want to pass in parameters from the command line
 3. You don't want to read the docs for your favorite argument parsing library *again*
 
 By leveraging as many Python idioms as possible, `arguably` keeps its API small and memorable without sacrificing
-funcitonality. `arguably` uses functions and their docstrings to automatically set up argparse. Notably, `arguably`
+functionality. `arguably` uses functions and their docstrings to automatically set up argparse. Notably, `arguably`
 maps your function signature to a command-line interface like this:
 
 ```python
 @arguably.command
 def some_function(required, not_required="foo", *others, option="bar"):
     ...
 ```
```

#### html2text {}

```diff
@@ -1,26 +1,27 @@
-Metadata-Version: 2.1 Name: arguably Version: 1.0.2 Summary: turns functions
+Metadata-Version: 2.1 Name: arguably Version: 1.1.0 Summary: turns functions
 into command line interfaces Home-page: https://github.com/treykeown/arguably
 Author: treykeown Author-email: 2755914+treykeown@users.noreply.github.com
 Requires-Python: >=3.8,<4.0 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: docstring-
 parser (>=0.15,<0.16) Requires-Dist: typing-extensions (>=4.6.3,<5.0.0)
 Project-URL: Repository, https://github.com/treykeown/arguably Description-
 Content-Type: text/markdown
                                 [arguably logo]
-                 turns functions into command line interfaces
+                        the best CLI library, arguably
+               turns your functions into command line interfaces
    [Test_status] [Code_coverage] [Supported_Python_versions] [PyPI_version]
 ===============================================================================
 `arguably` solves this problem: 1. You've written a Python script 2. Now you
 want to pass in parameters from the command line 3. You don't want to read the
 docs for your favorite argument parsing library *again* By leveraging as many
 Python idioms as possible, `arguably` keeps its API small and memorable without
-sacrificing funcitonality. `arguably` uses functions and their docstrings to
+sacrificing functionality. `arguably` uses functions and their docstrings to
 automatically set up argparse. Notably, `arguably` maps your function signature
 to a command-line interface like this: ```python @arguably.command def
 some_function(required, not_required="foo", *others, option="bar"): ... ```
                                     becomes
 ```text usage: script [--option OPTION] required [not-required] [others ...]
 ``` In short, `arguably` turns your function's **positional parameters** into
 **positional command-line arguments**, and your function's **keyword-only
```

