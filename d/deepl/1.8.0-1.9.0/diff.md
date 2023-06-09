# Comparing `tmp/deepl-1.8.0.tar.gz` & `tmp/deepl-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepl-1.8.0.tar", max compression
+gzip compressed data, was "deepl-1.9.0.tar", max compression
```

## Comparing `deepl-1.8.0.tar` & `deepl-1.9.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     7435 2022-06-10 07:14:38.635856 deepl-1.8.0/CHANGELOG.md
--rw-r--r--   0        0        0     1084 2022-06-10 06:57:30.533536 deepl-1.8.0/LICENSE
--rw-r--r--   0        0        0    20840 2022-06-10 06:57:30.533536 deepl-1.8.0/README.md
--rw-r--r--   0        0        0     3351 2022-06-10 06:57:30.533536 deepl-1.8.0/SECURITY.md
--rw-r--r--   0        0        0      873 2022-06-10 06:57:30.533536 deepl-1.8.0/deepl/__init__.py
--rw-r--r--   0        0        0    17349 2022-06-10 06:57:30.533536 deepl-1.8.0/deepl/__main__.py
--rw-r--r--   0        0        0     2047 2022-06-10 06:57:30.533536 deepl-1.8.0/deepl/exceptions.py
--rw-r--r--   0        0        0     7065 2022-06-10 06:57:30.533536 deepl-1.8.0/deepl/http_client.py
--rw-r--r--   0        0        0    44481 2022-06-10 06:57:30.533536 deepl-1.8.0/deepl/translator.py
--rw-r--r--   0        0        0     3803 2022-06-10 06:57:30.533536 deepl-1.8.0/deepl/util.py
--rw-r--r--   0        0        0      166 2022-06-10 07:14:38.635856 deepl-1.8.0/deepl/version.py
--rw-r--r--   0        0        0     1387 2022-06-10 07:14:38.635856 deepl-1.8.0/pyproject.toml
--rw-r--r--   0        0        0    22187 2022-06-10 07:15:36.162034 deepl-1.8.0/setup.py
--rw-r--r--   0        0        0    21922 2022-06-10 07:15:36.163201 deepl-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0     7667 2022-07-07 11:37:29.936253 deepl-1.9.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1084 2022-07-07 11:37:29.936253 deepl-1.9.0/LICENSE
+-rw-r--r--   0        0        0    21653 2022-07-07 11:37:29.936253 deepl-1.9.0/README.md
+-rw-r--r--   0        0        0     3351 2022-07-07 11:37:29.936253 deepl-1.9.0/SECURITY.md
+-rw-r--r--   0        0        0      873 2022-07-07 11:37:29.936253 deepl-1.9.0/deepl/__init__.py
+-rw-r--r--   0        0        0    18192 2022-07-07 11:37:29.936253 deepl-1.9.0/deepl/__main__.py
+-rw-r--r--   0        0        0     2047 2022-07-07 11:37:29.936253 deepl-1.9.0/deepl/exceptions.py
+-rw-r--r--   0        0        0     7065 2022-07-07 11:37:29.936253 deepl-1.9.0/deepl/http_client.py
+-rw-r--r--   0        0        0    46741 2022-07-07 11:37:29.936253 deepl-1.9.0/deepl/translator.py
+-rw-r--r--   0        0        0     3803 2022-07-07 11:37:29.936253 deepl-1.9.0/deepl/util.py
+-rw-r--r--   0        0        0      166 2022-07-07 11:37:29.936253 deepl-1.9.0/deepl/version.py
+-rw-r--r--   0        0        0     1387 2022-07-07 11:37:29.936253 deepl-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0    23025 2022-07-07 11:37:42.788293 deepl-1.9.0/setup.py
+-rw-r--r--   0        0        0    22735 2022-07-07 11:37:42.789444 deepl-1.9.0/PKG-INFO
```

### Comparing `deepl-1.8.0/CHANGELOG.md` & `deepl-1.9.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 
+## [1.9.0] - 2022-07-07
+### Added
+* Add `Translator.create_glossary_from_csv()` allowing glossaries downloaded
+  from website to be easily uploaded to API.
+
+
 ## [1.8.0] - 2022-06-10
 ### Added
 * Optional `filename` parameter added to `Translator.translate_document()`, only
   required if uploading string or bytes containing file content.
   * Pull request [#30](https://github.com/DeepLcom/deepl-python/pull/30)
     thanks to [seratch](https://github.com/seratch). 
 ### Changed
@@ -173,14 +179,15 @@
 * Fix examples in readme to match function interface changes.
 
 
 ## [0.1.0] - 2021-07-26
 Initial version.
 
 
+[1.9.0]: https://github.com/DeepLcom/deepl-python/compare/v1.8.0...v1.9.0
 [1.8.0]: https://github.com/DeepLcom/deepl-python/compare/v1.7.0...v1.8.0
 [1.7.0]: https://github.com/DeepLcom/deepl-python/compare/v1.6.0...v1.7.0
 [1.6.0]: https://github.com/DeepLcom/deepl-python/compare/v1.5.1...v1.6.0
 [1.5.1]: https://github.com/DeepLcom/deepl-python/compare/v1.5.0...v1.5.1
 [1.5.0]: https://github.com/DeepLcom/deepl-python/compare/v1.4.1...v1.5.0
 [1.4.1]: https://github.com/DeepLcom/deepl-python/compare/v1.4.0...v1.4.1
 [1.4.0]: https://github.com/DeepLcom/deepl-python/compare/v1.3.1...v1.4.0
```

### Comparing `deepl-1.8.0/LICENSE` & `deepl-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deepl-1.8.0/README.md` & `deepl-1.9.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -262,14 +262,33 @@
     f"Created '{my_glossary.name}' ({my_glossary.glossary_id}) "
     f"{my_glossary.source_lang}->{my_glossary.target_lang} "
     f"containing {my_glossary.entry_count} entries"
 )
 # Example: Created 'My glossary' (559192ed-8e23-...) EN->DE containing 2 entries
 ```
 
+You can also upload a glossary downloaded from the DeepL website using
+`create_glossary_from_csv()`. Instead of supplying the entries as a dictionary,
+specify the CSV data as `csv_data` either as a file-like object or string or
+bytes containing file content:
+
+```python
+with open('/path/to/glossary_file.csv', 'r') as csv_file:
+    csv_data = csv_file.read()  # Read the file contents as a string
+    my_csv_glossary = translator.create_glossary_from_csv(
+        "CSV glossary",
+        source_lang="EN",
+        target_lang="DE",
+        csv_data=csv_data,
+    )
+```
+
+The [API documentation][api-docs-csv-format] explains the expected CSV format in
+detail.
+
 #### Getting, listing and deleting stored glossaries
 
 Functions to get, list, and delete stored glossaries are also provided:
 
 - `get_glossary()` takes a glossary ID and returns a `GlossaryInfo` object for a
   stored glossary, or raises an exception if no such glossary is found.
 - `list_glossaries()` returns a list of `GlossaryInfo` objects corresponding to
@@ -518,14 +537,16 @@
 errors and test the client error-handling. To execute the tests using
 deepl-mock, run it in another terminal while executing the tests. Execute the
 tests using `pytest` with the `DEEPL_MOCK_SERVER_PORT` and `DEEPL_SERVER_URL`
 environment variables defined referring to the mock-server.
 
 [api-docs]: https://www.deepl.com/docs-api?utm_source=github&utm_medium=github-python-readme
 
+[api-docs-csv-format]: https://www.deepl.com/docs-api/managing-glossaries/supported-glossary-formats/?utm_source=github&utm_medium=github-python-readme
+
 [api-docs-xml-handling]: https://www.deepl.com/docs-api/handling-xml/?utm_source=github&utm_medium=github-python-readme
 
 [api-docs-lang-list]: https://www.deepl.com/docs-api/translating-text/?utm_source=github&utm_medium=github-python-readme
 
 [api-docs-glossary-lang-list]: https://www.deepl.com/docs-api/managing-glossaries/?utm_source=github&utm_medium=github-python-readme
 
 [create-account]: https://www.deepl.com/pro?utm_source=github&utm_medium=github-python-readme#developer
```

### Comparing `deepl-1.8.0/SECURITY.md` & `deepl-1.9.0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `deepl-1.8.0/deepl/__init__.py` & `deepl-1.9.0/deepl/__init__.py`

 * *Files identical despite different names*

### Comparing `deepl-1.8.0/deepl/__main__.py` & `deepl-1.9.0/deepl/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -82,30 +82,45 @@
 ):
     # Call action function corresponding to command with remaining args
     globals()[f"action_glossary_{subcommand}"](translator, **kwargs)
     pass
 
 
 def action_glossary_create(
-    translator: deepl.Translator, entry_list, file, **kwargs
+    translator: deepl.Translator, entry_list, file, csv, **kwargs
 ):
+    term_separator = None
     if file:
         if entry_list:
             raise deepl.DeepLException(
                 "The --file argument cannot be used together with "
                 "command-line entries"
             )
-        file_contents = pathlib.Path(file).read_text("UTF-8")
-        entry_dict = deepl.convert_tsv_to_dict(file_contents)
+        content = pathlib.Path(file).read_text("UTF-8")
     elif entry_list and entry_list[0] == "-":
-        entry_dict = deepl.convert_tsv_to_dict(sys.stdin.read())
+        content = sys.stdin.read()
     else:
-        entry_dict = deepl.convert_tsv_to_dict("\n".join(entry_list), "=")
+        content = "\n".join(entry_list)
+        term_separator = "="
+        if csv:
+            raise Exception(
+                "csv option is not compatible with command-line entries"
+            )
+
+    if csv:
+        glossary = translator.create_glossary_from_csv(
+            csv_data=content, **kwargs
+        )
+    else:
+        if term_separator:
+            entry_dict = deepl.convert_tsv_to_dict(content, term_separator)
+        else:
+            entry_dict = deepl.convert_tsv_to_dict(content)
+        glossary = translator.create_glossary(entries=entry_dict, **kwargs)
 
-    glossary = translator.create_glossary(entries=entry_dict, **kwargs)
     print(f"Created {glossary}")
     print_glossaries([glossary])
 
 
 def print_glossaries(glossaries):
     headers = [
         "Glossary ID",
@@ -363,16 +378,16 @@
     # Note: add_subparsers param 'required' is not available in py36
     glossary_subparsers = parser_glossary.add_subparsers(
         metavar="subcommand", dest="subcommand"
     )
     parser_glossary_create = glossary_subparsers.add_parser(
         "create",
         help="create a new glossary",
-        description="create a new glossary using entries specified in "
-        "a TSV file, standard-input, or provided via command-line",
+        description="create a new glossary using entries provided via command-"
+        "line, standard-input, or specified in a TSV or CSV file",
     )
     parser_glossary_create.add_argument(
         "--name", required=True, help="name to be associated with glossary."
     )
     parser_glossary_create.add_argument(
         "--from",
         "--source-lang",
@@ -389,25 +404,33 @@
     )
     parser_glossary_create.add_argument(
         "entry_list",
         nargs="*",
         type=str,
         metavar="SOURCE=TARGET",
         help="one or more entries to add to glossary, may be repeated. "
-        'Alternatively, use "-" to read entries from standard-input in TSV '
-        "format (see --file argument). These arguments cannot be used "
-        "together with the --file argument.",
+        'Alternatively, use "-" to read entries from standard-input in TSV or '
+        "CSV format (see --file argument for formatting information). These "
+        "arguments cannot be used together with the --file argument.",
     )
     parser_glossary_create.add_argument(
         "--file",
         type=str,
-        help="file to read glossary entries from. File must be in "
-        "tab-separated values (TSV) format: one entry-pair per line, each "
-        "line contains the source entry, a tab, then the target entry. Empty "
-        "lines are ignored.",
+        help="file to read glossary entries from. Unless --csv is specified, "
+        "file format is expected to be tab-separated values (TSV) format: one "
+        "entry-pair per line, each line contains the source entry, a tab, "
+        "then the target entry. Empty lines are ignored.",
+    )
+    parser_glossary_create.add_argument(
+        "--csv",
+        action="store_true",
+        help="the provided --file option or standard-input should be "
+        "interpreted as a CSV file. Information about the expected CSV format "
+        "can be found in the API documentation: "
+        "https://www.deepl.com/docs-api/managing-glossaries/supported-glossary-formats/.",  # noqa
     )
 
     parser_glossary_list = glossary_subparsers.add_parser(
         "list",
         help="list available glossaries",
         description="list available glossaries",
     )
```

### Comparing `deepl-1.8.0/deepl/exceptions.py` & `deepl-1.9.0/deepl/exceptions.py`

 * *Files identical despite different names*

### Comparing `deepl-1.8.0/deepl/http_client.py` & `deepl-1.9.0/deepl/http_client.py`

 * *Files identical despite different names*

### Comparing `deepl-1.8.0/deepl/translator.py` & `deepl-1.9.0/deepl/translator.py`

 * *Files 2% similar despite different names*

```diff
@@ -626,14 +626,43 @@
             request_data["formality"] = str(formality).lower()
         if isinstance(glossary, GlossaryInfo):
             request_data["glossary_id"] = glossary.glossary_id
         elif glossary is not None:
             request_data["glossary_id"] = glossary
         return request_data
 
+    def _create_glossary(
+        self,
+        name: str,
+        source_lang: Union[str, Language],
+        target_lang: Union[str, Language],
+        entries_format: str,
+        entries: str,
+    ) -> GlossaryInfo:
+        # glossaries are only supported for base language types
+        source_lang = Language.remove_regional_variant(source_lang)
+        target_lang = Language.remove_regional_variant(target_lang)
+
+        if not name:
+            raise ValueError("glossary name must not be empty")
+
+        request_data = {
+            "name": name,
+            "source_lang": source_lang,
+            "target_lang": target_lang,
+            "entries_format": entries_format,
+            "entries": entries,
+        }
+
+        status, content, json = self._api_call(
+            "v2/glossaries", data=request_data
+        )
+        self._raise_for_status(status, content, json, glossary=True)
+        return GlossaryInfo.from_json(json)
+
     def close(self):
         if hasattr(self, "_client"):
             self._client.close()
 
     @property
     def server_url(self):
         return self._server_url
@@ -1129,36 +1158,67 @@
         :return: GlossaryInfo containing information about created glossary.
 
         :raises ValueError: If the glossary name is empty, or entries are
             empty or invalid.
         :raises DeepLException: If source and target language pair are not
             supported for glossaries.
         """
-        # glossaries are only supported for base language types
-        target_lang = Language.remove_regional_variant(target_lang)
-        source_lang = Language.remove_regional_variant(source_lang)
-
-        if not name:
-            raise ValueError("glossary name must not be empty")
         if not entries:
             raise ValueError("glossary entries must not be empty")
 
-        request_data = {
-            "name": name,
-            "source_lang": source_lang,
-            "target_lang": target_lang,
-            "entries_format": "tsv",
-            "entries": util.convert_dict_to_tsv(entries),
-        }
+        return self._create_glossary(
+            name,
+            source_lang,
+            target_lang,
+            "tsv",
+            util.convert_dict_to_tsv(entries),
+        )
 
-        status, content, json = self._api_call(
-            "v2/glossaries", data=request_data
+    def create_glossary_from_csv(
+        self,
+        name: str,
+        source_lang: Union[str, Language],
+        target_lang: Union[str, Language],
+        csv_data: Union[TextIO, BinaryIO, str, bytes, Any],
+    ) -> GlossaryInfo:
+        """Creates a glossary with given name for the source and target
+        languages, containing the entries in the given CSV data.
+        The glossary may be used in the translate_text functions.
+
+        Only certain language pairs are supported. The available language pairs
+        can be queried using get_glossary_languages(). Glossaries are not
+        regional specific: a glossary with target language EN may be used to
+        translate texts into both EN-US and EN-GB.
+
+        This function allows you to upload a glossary CSV file that you have
+        downloaded from the DeepL website.
+
+        Information about the expected CSV format can be found in the API
+        documentation: https://www.deepl.com/docs-api/managing-glossaries/supported-glossary-formats/  # noqa
+
+        :param name: user-defined name to attach to glossary.
+        :param source_lang: Language of source terms.
+        :param target_lang: Language of target terms.
+        :param csv_data: CSV data containing glossary entries, either as a
+            file-like object or string or bytes containing file content.
+        :return: GlossaryInfo containing information about created glossary.
+
+        :raises ValueError: If the glossary name is empty, or entries are
+            empty or invalid.
+        :raises DeepLException: If source and target language pair are not
+            supported for glossaries.
+        """
+
+        entries = (
+            csv_data if isinstance(csv_data, (str, bytes)) else csv_data.read()
+        )
+
+        return self._create_glossary(
+            name, source_lang, target_lang, "csv", entries
         )
-        self._raise_for_status(status, content, json, glossary=True)
-        return GlossaryInfo.from_json(json)
 
     def get_glossary(self, glossary_id: str) -> GlossaryInfo:
         """Retrieves GlossaryInfo for the glossary with specified ID.
 
         :param glossary_id: ID of glossary to retrieve.
         :return: GlossaryInfo with information about specified glossary.
         :raises GlossaryNotFoundException: If no glossary with given ID is
```

### Comparing `deepl-1.8.0/deepl/util.py` & `deepl-1.9.0/deepl/util.py`

 * *Files identical despite different names*

### Comparing `deepl-1.8.0/pyproject.toml` & `deepl-1.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.black]
 line-length = 79
 
 [tool.poetry]
 name = "deepl"
-version = "1.8.0"
+version = "1.9.0"
 description = "Python library for the DeepL API."
 authors = ["DeepL SE <python-api@deepl.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/DeepLcom/deepl-python"
 documentation = "https://www.deepl.com/docs-api/"
 classifiers = [
```

### Comparing `deepl-1.8.0/setup.py` & `deepl-1.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['requests>=2,<3']
 
 entry_points = \
 {'console_scripts': ['deepl = deepl.__main__:main']}
 
 setup_kwargs = {
     'name': 'deepl',
-    'version': '1.8.0',
+    'version': '1.9.0',
     'description': 'Python library for the DeepL API.',
-    'long_description': '# DeepL Python Library\n\n[![PyPI version](https://img.shields.io/pypi/v/deepl.svg)](https://pypi.org/project/deepl/)\n[![Supported Python versions](https://img.shields.io/pypi/pyversions/deepl.svg)](https://pypi.org/project/deepl/)\n[![License: MIT](https://img.shields.io/badge/license-MIT-blueviolet.svg)](https://github.com/DeepLcom/deepl-python/blob/main/LICENSE)\n\nThe [DeepL API][api-docs] is a language translation API that allows other\ncomputer programs to send texts and documents to DeepL\'s servers and receive\nhigh-quality translations. This opens a whole universe of opportunities for\ndevelopers: any translation product you can imagine can now be built on top of\nDeepL\'s best-in-class translation technology.\n\nThe DeepL Python library offers a convenient way for applications written in\nPython to interact with the DeepL API. We intend to support all API functions\nwith the library, though support for new features may be added to the library\nafter they’re added to the API.\n\n## Getting an authentication key\n\nTo use the DeepL Python Library, you\'ll need an API authentication key. To get a\nkey, [please create an account here][create-account]. With a DeepL API Free\naccount you can translate up to 500,000 characters/month for free.\n\n## Installation\n\nThe library can be installed from [PyPI][pypi-project] using pip:\n\n```shell\npip install --upgrade deepl\n```\n\nIf you need to modify this source code, install the dependencies using poetry:\n\n```shell\npoetry install\n```\n\n### Requirements\n\nThe library is tested with Python versions 3.6 to 3.10.\n\nThe `requests` module is used to perform HTTP requests; the minimum is version\n2.0.\n\n## Usage\n\nImport the package and construct a `Translator`. The first argument is a string\ncontaining your API authentication key as found in your\n[DeepL Pro Account][pro-account].\n\nBe careful not to expose your key, for example when sharing source code.\n\n```python\nimport deepl\n\nauth_key = "f63c02c5-f056-..."  # Replace with your key\ntranslator = deepl.Translator(auth_key)\n\nresult = translator.translate_text("Hello, world!", target_lang="FR")\nprint(result.text)  # "Bonjour, le monde !"\n```\n\nThis example is for demonstration purposes only. In production code, the\nauthentication key should not be hard-coded, but instead fetched from a\nconfiguration file or environment variable.\n\n`Translator` accepts additional options, see [Configuration](#configuration)\nfor more information.\n\n### Translating text\n\nTo translate text, call `translate_text()`. The first argument is a string\ncontaining the text you want to translate, or a list of strings if you want to\ntranslate multiple texts.\n\n`source_lang` and `target_lang` specify the source and target language codes\nrespectively. The `source_lang` is optional, if it is unspecified the source\nlanguage will be auto-detected.\n\nLanguage codes are **case-insensitive** strings according to ISO 639-1, for\nexample `\'DE\'`, `\'FR\'`, `\'JA\'\'`. Some target languages also include the regional\nvariant according to ISO 3166-1, for example `\'EN-US\'`, or `\'PT-BR\'`. The full\nlist of supported languages is in the\n[API documentation][api-docs-lang-list].\n\nThere are additional optional arguments to control translation, see\n[Text translation options](#text-translation-options) below.\n\n`translate_text()` returns a `TextResult`, or a list of `TextResult`s\ncorresponding to your input text(s). `TextResult` has two properties: `text` is\nthe translated text, and `detected_source_lang` is the detected source language\ncode.\n\n```python\n# Translate text into a target language, in this case, French:\nresult = translator.translate_text("Hello, world!", target_lang="FR")\nprint(result.text)  # "Bonjour, le monde !"\n\n# Translate multiple texts into British English\nresult = translator.translate_text(\n    ["お元気ですか？", "¿Cómo estás?"], target_lang="EN-GB"\n)\nprint(result[0].text)  # "How are you?"\nprint(result[0].detected_source_lang)  # "JA" the language code for Japanese\nprint(result[1].text)  # "How are you?"\nprint(result[1].detected_source_lang)  # "ES" the language code for Spanish\n\n# Translate into German with less and more Formality:\nprint(\n    translator.translate_text(\n        "How are you?", target_lang="DE", formality="less"\n    )\n)  # \'Wie geht es dir?\'\nprint(\n    translator.translate_text(\n        "How are you?", target_lang="DE", formality="more"\n    )\n)  # \'Wie geht es Ihnen?\'\n```\n\n#### Text translation options\n\nIn addition to the input text(s) argument, the available `translate_text()`\narguments are:\n\n- `source_lang`: Specifies the source language code, but may be omitted to\n  auto-detect the source language.\n- `target_lang`: Required. Specifies the target language code.\n- `split_sentences`: specify how input text should be split into sentences,\n  default: `\'on\'`.\n    - `\'on\'\'` (`SplitSentences.ON`): input text will be split into sentences\n      using both newlines and punctuation.\n    - `\'off\'` (`SplitSentences.OFF`): input text will not be split into\n      sentences. Use this for applications where each input text contains only\n      one sentence.\n    - `\'nonewlines\'` (`SplitSentences.NO_NEWLINES`): input text will be split\n      into sentences using punctuation but not newlines.\n- `preserve_formatting`: controls automatic-formatting-correction. Set to `True`\n  to prevent automatic-correction of formatting, default: `False`.\n- `formality`: controls whether translations should lean toward informal or\n  formal language. This option is only available for some target languages, see\n  [Listing available languages](#listing-available-languages).\n    - `\'less\'` (`Formality.LESS`): use informal language.\n    - `\'more\'` (`Formality.MORE`): use formal, more polite language.\n- `glossary`: specifies a glossary to use with translation, either as a string\n  containing the glossary ID, or a `GlossaryInfo` as returned by\n  `get_glossary()`.\n- `tag_handling`: type of tags to parse before translation, options are `\'html\'`\n  and `\'xml\'`.\n\nThe following options are only used if `tag_handling` is `\'xml\'`:\n\n- `outline_detection`: specify `False` to disable automatic tag detection,\n  default is `True`.\n- `splitting_tags`: list of XML tags that should be used to split text into\n  sentences. Tags may be specified as an array of strings (`[\'tag1\', \'tag2\']`),\n  or a comma-separated list of strings (`\'tag1,tag2\'`). The default is an empty\n  list.\n- `non_splitting_tags`: list of XML tags that should not be used to split text\n  into sentences. Format and default are the same as for `splitting_tags`.\n- `ignore_tags`: list of XML tags that containing content that should not be\n  translated. Format and default are the same as for `splitting_tags`.\n\nFor a detailed explanation of the XML handling options, see the\n[API documentation][api-docs-xml-handling].\n\n### Translating documents\n\nTo translate documents, you may call either `translate_document()` using file IO\nobjects, or `translate_document_from_filepath()` using file paths. For both\nfunctions, the first and second arguments correspond to the input and output\nfiles respectively.\n\nJust as for the `translate_text()` function, the `source_lang` and\n`target_lang` arguments specify the source and target language codes.\n\nThere are additional optional arguments to control translation, see\n[Document translation options](#document-translation-options) below.\n\n```python\n# Translate a formal document from English to German\ninput_path = "/path/to/Instruction Manual.docx"\noutput_path = "/path/to/Bedienungsanleitung.docx"\ntry:\n    # Using translate_document_from_filepath() with file paths \n    translator.translate_document_from_filepath(\n        input_path,\n        output_path,\n        target_lang="DE",\n        formality="more"\n    )\n\n    # Alternatively you can use translate_document() with file IO objects\n    with open(input_path, "rb") as in_file, open(output_path, "wb") as out_file:\n        translator.translate_document(\n            in_file,\n            out_file,\n            target_lang="DE",\n            formality="more"\n        )\n\nexcept deepl.DocumentTranslationException as error:\n    # If an error occurs during document translation after the document was\n    # already uploaded, a DocumentTranslationException is raised. The\n    # document_handle property contains the document handle that may be used to\n    # later retrieve the document from the server, or contact DeepL support.\n    doc_id = error.document_handle.id\n    doc_key = error.document_handle.key\n    print(f"Error after uploading ${error}, id: ${doc_id} key: ${doc_key}")\nexcept deepl.DeepLException as error:\n    # Errors during upload raise a DeepLException\n    print(error)\n```\n\n`translate_document()` and `translate_document_from_filepath()` are convenience\nfunctions that wrap multiple API calls: uploading, polling status until the\ntranslation is complete, and downloading. If your application needs to execute\nthese steps individually, you can instead use the following functions directly:\n\n- `translate_document_upload()`,\n- `translate_document_get_status()` (or\n  `translate_document_wait_until_done()`), and\n- `translate_document_download()`\n\n#### Document translation options\n\nIn addition to the input file, output file, `source_lang` and `target_lang`\narguments, the available `translate_document()` and\n`translate_document_from_filepath()` arguments are:\n\n- `formality`: same as in [Text translation options](#text-translation-options).\n- `glossary`: same as in [Text translation options](#text-translation-options).\n\n### Glossaries\n\nGlossaries allow you to customize your translations using user-defined terms.\nMultiple glossaries can be stored with your account, each with a user-specified\nname and a uniquely-assigned ID.\n\n#### Creating a glossary\n\nYou can create a glossary with your desired terms and name using\n`create_glossary()`. Each glossary applies to a single source-target language\npair. Note: Glossaries are only supported for some language pairs, see\n[Listing available glossary languages](#listing-available-glossary-languages)\nfor more information. The entries should be specified as a dictionary.\n\nIf successful, the glossary is created and stored with your DeepL account, and\na `GlossaryInfo` object is returned including the ID, name, languages and entry\ncount.\n\n```python\n# Create an English to German glossary with two terms:\nentries = {"artist": "Maler", "prize": "Gewinn"}\nmy_glossary = translator.create_glossary(\n    "My glossary",\n    source_lang="EN",\n    target_lang="DE",\n    entries=entries,\n)\nprint(\n    f"Created \'{my_glossary.name}\' ({my_glossary.glossary_id}) "\n    f"{my_glossary.source_lang}->{my_glossary.target_lang} "\n    f"containing {my_glossary.entry_count} entries"\n)\n# Example: Created \'My glossary\' (559192ed-8e23-...) EN->DE containing 2 entries\n```\n\n#### Getting, listing and deleting stored glossaries\n\nFunctions to get, list, and delete stored glossaries are also provided:\n\n- `get_glossary()` takes a glossary ID and returns a `GlossaryInfo` object for a\n  stored glossary, or raises an exception if no such glossary is found.\n- `list_glossaries()` returns a list of `GlossaryInfo` objects corresponding to\n  all of your stored glossaries.\n- `delete_glossary()` takes a glossary ID or `GlossaryInfo` object and deletes\n  the stored glossary from the server, or raises an exception if no such\n  glossary is found.\n\n```python\n# Retrieve a stored glossary using the ID\nglossary_id = "559192ed-8e23-..."\nmy_glossary = translator.get_glossary(glossary_id)\n\n# Find and delete glossaries named \'Old glossary\'\nglossaries = translator.list_glossaries()\nfor glossary in glossaries:\n    if glossary.name == "Old glossary":\n        translator.delete_glossary(glossary)\n```\n\n#### Listing entries in a stored glossary\n\nThe `GlossaryInfo` object does not contain the glossary entries, but instead\nonly the number of entries in the `entry_count` property.\n\nTo list the entries contained within a stored glossary, use\n`get_glossary_entries()` providing either the `GlossaryInfo` object or glossary\nID:\n\n```python\nentries = translator.get_glossary_entries(my_glossary)\nprint(entries)  # "{\'artist\': \'Maler\', \'prize\': \'Gewinn\'}"\n```\n\n#### Using a stored glossary\n\nYou can use a stored glossary for text translation by setting the `glossary`\nargument to either the glossary ID or `GlossaryInfo` object. You must also\nspecify the `source_lang` argument (it is required when using a glossary):\n\n```python\ntext = "The artist was awarded a prize."\nwith_glossary = translator.translate_text(\n    text, source_lang="EN", target_lang="DE", glossary=my_glossary,\n)\nprint(with_glossary)  # "Der Maler wurde mit einem Gewinn ausgezeichnet."\n\n# For comparison, the result without a glossary:\nwithout_glossary = translator.translate_text(text, target_lang="DE")\nprint(without_glossary)  # "Der Künstler wurde mit einem Preis ausgezeichnet."\n```\n\nUsing a stored glossary for document translation is the same: set the `glossary`\nargument and specify the `source_lang` argument:\n\n```python\ntranslator.translate_document(\n    in_file, out_file, source_lang="EN", target_lang="DE", glossary=my_glossary,\n)\n```\n\nThe `translate_document()`, `translate_document_from_filepath()` and\n`translate_document_upload()` functions all support the `glossary` argument.\n\n### Checking account usage\n\nTo check account usage, use the `get_usage()` function.\n\nThe returned `Usage` object contains three usage subtypes: `character`,\n`document` and `team_document`. Depending on your account type, some usage\nsubtypes may be invalid; this can be checked using the `valid` property. For API\naccounts:\n\n- `usage.character.valid` is `True`,\n- `usage.document.valid` and `usage.team_document.valid` are `False`.\n\nEach usage subtype (if valid) has `count` and `limit` properties giving the\namount used and maximum amount respectively, and the `limit_reached` property\nthat checks if the usage has reached the limit. The top level `Usage` object has\nthe `any_limit_reached` property to check all usage subtypes.\n\n```python\nusage = translator.get_usage()\nif usage.any_limit_reached:\n    print(\'Translation limit reached.\')\nif usage.character.valid:\n    print(\n        f"Character usage: {usage.character.count} of {usage.character.limit}")\nif usage.document.valid:\n    print(f"Document usage: {usage.document.count} of {usage.document.limit}")\n```\n\n### Listing available languages\n\nYou can request the list of languages supported by DeepL for text and documents\nusing the `get_source_languages()` and `get_target_languages()` functions. They\nboth return a list of `Language` objects.\n\nThe `name` property gives the name of the language in English, and the `code`\nproperty gives the language code. The `supports_formality` property only appears\nfor target languages, and indicates whether the target language supports the\noptional `formality` parameter.\n\n```python\nprint("Source languages:")\nfor language in translator.get_source_languages():\n    print(f"{language.name} ({language.code})")  # Example: "German (DE)"\n\nprint("Target languages:")\nfor language in translator.get_target_languages():\n    if language.supports_formality:\n        print(f"{language.name} ({language.code}) supports formality")\n        # Example: "Italian (IT) supports formality"\n    else:\n        print(f"{language.name} ({language.code})")\n        # Example: "Lithuanian (LT)"\n```\n\n#### Listing available glossary languages\n\nGlossaries are supported for a subset of language pairs. To retrieve those\nlanguages use the `get_glossary_languages()` function, which returns an array\nof `GlossaryLanguagePair` objects. Each has `source_lang` and `target_lang`\nproperties indicating that that pair of language codes is supported.\n\n```python\nglossary_languages = translator.get_glossary_languages()\nfor language_pair in glossary_languages:\n    print(f"{language_pair.source_lang} to {language_pair.target_lang}")\n    # Example: "EN to DE", "DE to EN", etc.\n```\n\nYou can also find the list of supported glossary language pairs in the\n[API documentation][api-docs-glossary-lang-list].\n\nNote that glossaries work for all target regional-variants: a glossary for the\ntarget language English (`"EN"`) supports translations to both American English\n(`"EN-US"`) and British English (`"EN-GB""`).\n\n### Exceptions\n\nAll module functions may raise `deepl.DeepLException` or one of its subclasses.\nIf invalid arguments are provided, they may raise the standard exceptions\n`ValueError` and `TypeError`.\n\n### Configuration\n\n#### Logging\n\nLogging can be enabled to see the HTTP requests sent and responses received by\nthe library. Enable and control logging using Python\'s `logging` module, for\nexample:\n\n```python\nimport logging\n\nlogging.basicConfig()\nlogging.getLogger(\'deepl\').setLevel(logging.DEBUG)\n```\n\n#### Server URL configuration\n\nYou can override the URL of the DeepL API by specifying the `server_url`\nargument when constructing a `deepl.Translator`. This may be useful for testing\npurposes. You **do not** need to specify the URL to distinguish API Free and API\nPro accounts, the library selects the correct URL automatically.\n\n```python\nserver_url = "http://user:pass@localhost:3000"\ntranslator = deepl.Translator(..., server_url=server_url)\n```\n\n#### Proxy configuration\n\nYou can configure a proxy by specifying the `proxy` argument when constructing a\n`deepl.Translator`:\n\n```python\nproxy = "http://user:pass@10.10.1.10:3128"\ntranslator = deepl.Translator(..., proxy=proxy)\n```\n\nThe proxy argument is passed to the underlying `requests` session, see the\n[documentation for requests][requests-proxy-docs]; a dictionary of schemes to\nproxy URLs is also accepted.\n\n## Command Line Interface\n\nThe library can be run on the command line supporting all API functions. Use the\n`--help` option for usage information:\n\n```shell\npython3 -m deepl --help\n```\n\nThe CLI requires your DeepL authentication key specified either as the\n`DEEPL_AUTH_KEY` environment variable, or using the `--auth-key` option, for\nexample:\n\n```shell\npython3 -m deepl --auth-key=YOUR_AUTH_KEY usage\n```\n\nNote that the `--auth-key` argument must appear *before* the command argument.\nThe recognized commands are:\n\n| Command   | Description                                            |\n| :-------- | :----------------------------------------------------- |\n| text      | translate text(s)                                      |\n| document  | translate document(s)                                  |\n| usage     | print usage information for the current billing period |\n| languages | print available languages                              |\n| glossary  | create, list, and remove glossaries                    |\n\nFor example, to translate text:\n\n```shell\npython3 -m deepl --auth-key=YOUR_AUTH_KEY text --to=DE "Text to be translated."\n```\n\nWrap text arguments in quotes to prevent the shell from splitting sentences into\nwords.\n\n## Issues\n\nIf you experience problems using the library, or would like to request a new\nfeature, please open an [issue][issues].\n\n## Development\n\nWe welcome Pull Requests, please read the\n[contributing guidelines](CONTRIBUTING.md).\n\n### Tests\n\nExecute the tests using `pytest`. The tests communicate with the DeepL API using\nthe auth key defined by the `DEEPL_AUTH_KEY` environment variable.\n\nBe aware that the tests make DeepL API requests that contribute toward your API\nusage.\n\nThe test suite may instead be configured to communicate with the mock-server\nprovided by [deepl-mock][deepl-mock]. Although most test cases work for either,\nsome test cases work only with the DeepL API or the mock-server and will be\notherwise skipped. The test cases that require the mock-server trigger server\nerrors and test the client error-handling. To execute the tests using\ndeepl-mock, run it in another terminal while executing the tests. Execute the\ntests using `pytest` with the `DEEPL_MOCK_SERVER_PORT` and `DEEPL_SERVER_URL`\nenvironment variables defined referring to the mock-server.\n\n[api-docs]: https://www.deepl.com/docs-api?utm_source=github&utm_medium=github-python-readme\n\n[api-docs-xml-handling]: https://www.deepl.com/docs-api/handling-xml/?utm_source=github&utm_medium=github-python-readme\n\n[api-docs-lang-list]: https://www.deepl.com/docs-api/translating-text/?utm_source=github&utm_medium=github-python-readme\n\n[api-docs-glossary-lang-list]: https://www.deepl.com/docs-api/managing-glossaries/?utm_source=github&utm_medium=github-python-readme\n\n[create-account]: https://www.deepl.com/pro?utm_source=github&utm_medium=github-python-readme#developer\n\n[deepl-mock]: https://www.github.com/DeepLcom/deepl-mock\n\n[issues]: https://www.github.com/DeepLcom/deepl-python/issues\n\n[pypi-project]: https://pypi.org/project/deepl/\n\n[pro-account]: https://www.deepl.com/pro-account/?utm_source=github&utm_medium=github-python-readme\n\n[requests-proxy-docs]: https://docs.python-requests.org/en/latest/user/advanced/#proxies\n',
+    'long_description': '# DeepL Python Library\n\n[![PyPI version](https://img.shields.io/pypi/v/deepl.svg)](https://pypi.org/project/deepl/)\n[![Supported Python versions](https://img.shields.io/pypi/pyversions/deepl.svg)](https://pypi.org/project/deepl/)\n[![License: MIT](https://img.shields.io/badge/license-MIT-blueviolet.svg)](https://github.com/DeepLcom/deepl-python/blob/main/LICENSE)\n\nThe [DeepL API][api-docs] is a language translation API that allows other\ncomputer programs to send texts and documents to DeepL\'s servers and receive\nhigh-quality translations. This opens a whole universe of opportunities for\ndevelopers: any translation product you can imagine can now be built on top of\nDeepL\'s best-in-class translation technology.\n\nThe DeepL Python library offers a convenient way for applications written in\nPython to interact with the DeepL API. We intend to support all API functions\nwith the library, though support for new features may be added to the library\nafter they’re added to the API.\n\n## Getting an authentication key\n\nTo use the DeepL Python Library, you\'ll need an API authentication key. To get a\nkey, [please create an account here][create-account]. With a DeepL API Free\naccount you can translate up to 500,000 characters/month for free.\n\n## Installation\n\nThe library can be installed from [PyPI][pypi-project] using pip:\n\n```shell\npip install --upgrade deepl\n```\n\nIf you need to modify this source code, install the dependencies using poetry:\n\n```shell\npoetry install\n```\n\n### Requirements\n\nThe library is tested with Python versions 3.6 to 3.10.\n\nThe `requests` module is used to perform HTTP requests; the minimum is version\n2.0.\n\n## Usage\n\nImport the package and construct a `Translator`. The first argument is a string\ncontaining your API authentication key as found in your\n[DeepL Pro Account][pro-account].\n\nBe careful not to expose your key, for example when sharing source code.\n\n```python\nimport deepl\n\nauth_key = "f63c02c5-f056-..."  # Replace with your key\ntranslator = deepl.Translator(auth_key)\n\nresult = translator.translate_text("Hello, world!", target_lang="FR")\nprint(result.text)  # "Bonjour, le monde !"\n```\n\nThis example is for demonstration purposes only. In production code, the\nauthentication key should not be hard-coded, but instead fetched from a\nconfiguration file or environment variable.\n\n`Translator` accepts additional options, see [Configuration](#configuration)\nfor more information.\n\n### Translating text\n\nTo translate text, call `translate_text()`. The first argument is a string\ncontaining the text you want to translate, or a list of strings if you want to\ntranslate multiple texts.\n\n`source_lang` and `target_lang` specify the source and target language codes\nrespectively. The `source_lang` is optional, if it is unspecified the source\nlanguage will be auto-detected.\n\nLanguage codes are **case-insensitive** strings according to ISO 639-1, for\nexample `\'DE\'`, `\'FR\'`, `\'JA\'\'`. Some target languages also include the regional\nvariant according to ISO 3166-1, for example `\'EN-US\'`, or `\'PT-BR\'`. The full\nlist of supported languages is in the\n[API documentation][api-docs-lang-list].\n\nThere are additional optional arguments to control translation, see\n[Text translation options](#text-translation-options) below.\n\n`translate_text()` returns a `TextResult`, or a list of `TextResult`s\ncorresponding to your input text(s). `TextResult` has two properties: `text` is\nthe translated text, and `detected_source_lang` is the detected source language\ncode.\n\n```python\n# Translate text into a target language, in this case, French:\nresult = translator.translate_text("Hello, world!", target_lang="FR")\nprint(result.text)  # "Bonjour, le monde !"\n\n# Translate multiple texts into British English\nresult = translator.translate_text(\n    ["お元気ですか？", "¿Cómo estás?"], target_lang="EN-GB"\n)\nprint(result[0].text)  # "How are you?"\nprint(result[0].detected_source_lang)  # "JA" the language code for Japanese\nprint(result[1].text)  # "How are you?"\nprint(result[1].detected_source_lang)  # "ES" the language code for Spanish\n\n# Translate into German with less and more Formality:\nprint(\n    translator.translate_text(\n        "How are you?", target_lang="DE", formality="less"\n    )\n)  # \'Wie geht es dir?\'\nprint(\n    translator.translate_text(\n        "How are you?", target_lang="DE", formality="more"\n    )\n)  # \'Wie geht es Ihnen?\'\n```\n\n#### Text translation options\n\nIn addition to the input text(s) argument, the available `translate_text()`\narguments are:\n\n- `source_lang`: Specifies the source language code, but may be omitted to\n  auto-detect the source language.\n- `target_lang`: Required. Specifies the target language code.\n- `split_sentences`: specify how input text should be split into sentences,\n  default: `\'on\'`.\n    - `\'on\'\'` (`SplitSentences.ON`): input text will be split into sentences\n      using both newlines and punctuation.\n    - `\'off\'` (`SplitSentences.OFF`): input text will not be split into\n      sentences. Use this for applications where each input text contains only\n      one sentence.\n    - `\'nonewlines\'` (`SplitSentences.NO_NEWLINES`): input text will be split\n      into sentences using punctuation but not newlines.\n- `preserve_formatting`: controls automatic-formatting-correction. Set to `True`\n  to prevent automatic-correction of formatting, default: `False`.\n- `formality`: controls whether translations should lean toward informal or\n  formal language. This option is only available for some target languages, see\n  [Listing available languages](#listing-available-languages).\n    - `\'less\'` (`Formality.LESS`): use informal language.\n    - `\'more\'` (`Formality.MORE`): use formal, more polite language.\n- `glossary`: specifies a glossary to use with translation, either as a string\n  containing the glossary ID, or a `GlossaryInfo` as returned by\n  `get_glossary()`.\n- `tag_handling`: type of tags to parse before translation, options are `\'html\'`\n  and `\'xml\'`.\n\nThe following options are only used if `tag_handling` is `\'xml\'`:\n\n- `outline_detection`: specify `False` to disable automatic tag detection,\n  default is `True`.\n- `splitting_tags`: list of XML tags that should be used to split text into\n  sentences. Tags may be specified as an array of strings (`[\'tag1\', \'tag2\']`),\n  or a comma-separated list of strings (`\'tag1,tag2\'`). The default is an empty\n  list.\n- `non_splitting_tags`: list of XML tags that should not be used to split text\n  into sentences. Format and default are the same as for `splitting_tags`.\n- `ignore_tags`: list of XML tags that containing content that should not be\n  translated. Format and default are the same as for `splitting_tags`.\n\nFor a detailed explanation of the XML handling options, see the\n[API documentation][api-docs-xml-handling].\n\n### Translating documents\n\nTo translate documents, you may call either `translate_document()` using file IO\nobjects, or `translate_document_from_filepath()` using file paths. For both\nfunctions, the first and second arguments correspond to the input and output\nfiles respectively.\n\nJust as for the `translate_text()` function, the `source_lang` and\n`target_lang` arguments specify the source and target language codes.\n\nThere are additional optional arguments to control translation, see\n[Document translation options](#document-translation-options) below.\n\n```python\n# Translate a formal document from English to German\ninput_path = "/path/to/Instruction Manual.docx"\noutput_path = "/path/to/Bedienungsanleitung.docx"\ntry:\n    # Using translate_document_from_filepath() with file paths \n    translator.translate_document_from_filepath(\n        input_path,\n        output_path,\n        target_lang="DE",\n        formality="more"\n    )\n\n    # Alternatively you can use translate_document() with file IO objects\n    with open(input_path, "rb") as in_file, open(output_path, "wb") as out_file:\n        translator.translate_document(\n            in_file,\n            out_file,\n            target_lang="DE",\n            formality="more"\n        )\n\nexcept deepl.DocumentTranslationException as error:\n    # If an error occurs during document translation after the document was\n    # already uploaded, a DocumentTranslationException is raised. The\n    # document_handle property contains the document handle that may be used to\n    # later retrieve the document from the server, or contact DeepL support.\n    doc_id = error.document_handle.id\n    doc_key = error.document_handle.key\n    print(f"Error after uploading ${error}, id: ${doc_id} key: ${doc_key}")\nexcept deepl.DeepLException as error:\n    # Errors during upload raise a DeepLException\n    print(error)\n```\n\n`translate_document()` and `translate_document_from_filepath()` are convenience\nfunctions that wrap multiple API calls: uploading, polling status until the\ntranslation is complete, and downloading. If your application needs to execute\nthese steps individually, you can instead use the following functions directly:\n\n- `translate_document_upload()`,\n- `translate_document_get_status()` (or\n  `translate_document_wait_until_done()`), and\n- `translate_document_download()`\n\n#### Document translation options\n\nIn addition to the input file, output file, `source_lang` and `target_lang`\narguments, the available `translate_document()` and\n`translate_document_from_filepath()` arguments are:\n\n- `formality`: same as in [Text translation options](#text-translation-options).\n- `glossary`: same as in [Text translation options](#text-translation-options).\n\n### Glossaries\n\nGlossaries allow you to customize your translations using user-defined terms.\nMultiple glossaries can be stored with your account, each with a user-specified\nname and a uniquely-assigned ID.\n\n#### Creating a glossary\n\nYou can create a glossary with your desired terms and name using\n`create_glossary()`. Each glossary applies to a single source-target language\npair. Note: Glossaries are only supported for some language pairs, see\n[Listing available glossary languages](#listing-available-glossary-languages)\nfor more information. The entries should be specified as a dictionary.\n\nIf successful, the glossary is created and stored with your DeepL account, and\na `GlossaryInfo` object is returned including the ID, name, languages and entry\ncount.\n\n```python\n# Create an English to German glossary with two terms:\nentries = {"artist": "Maler", "prize": "Gewinn"}\nmy_glossary = translator.create_glossary(\n    "My glossary",\n    source_lang="EN",\n    target_lang="DE",\n    entries=entries,\n)\nprint(\n    f"Created \'{my_glossary.name}\' ({my_glossary.glossary_id}) "\n    f"{my_glossary.source_lang}->{my_glossary.target_lang} "\n    f"containing {my_glossary.entry_count} entries"\n)\n# Example: Created \'My glossary\' (559192ed-8e23-...) EN->DE containing 2 entries\n```\n\nYou can also upload a glossary downloaded from the DeepL website using\n`create_glossary_from_csv()`. Instead of supplying the entries as a dictionary,\nspecify the CSV data as `csv_data` either as a file-like object or string or\nbytes containing file content:\n\n```python\nwith open(\'/path/to/glossary_file.csv\', \'r\') as csv_file:\n    csv_data = csv_file.read()  # Read the file contents as a string\n    my_csv_glossary = translator.create_glossary_from_csv(\n        "CSV glossary",\n        source_lang="EN",\n        target_lang="DE",\n        csv_data=csv_data,\n    )\n```\n\nThe [API documentation][api-docs-csv-format] explains the expected CSV format in\ndetail.\n\n#### Getting, listing and deleting stored glossaries\n\nFunctions to get, list, and delete stored glossaries are also provided:\n\n- `get_glossary()` takes a glossary ID and returns a `GlossaryInfo` object for a\n  stored glossary, or raises an exception if no such glossary is found.\n- `list_glossaries()` returns a list of `GlossaryInfo` objects corresponding to\n  all of your stored glossaries.\n- `delete_glossary()` takes a glossary ID or `GlossaryInfo` object and deletes\n  the stored glossary from the server, or raises an exception if no such\n  glossary is found.\n\n```python\n# Retrieve a stored glossary using the ID\nglossary_id = "559192ed-8e23-..."\nmy_glossary = translator.get_glossary(glossary_id)\n\n# Find and delete glossaries named \'Old glossary\'\nglossaries = translator.list_glossaries()\nfor glossary in glossaries:\n    if glossary.name == "Old glossary":\n        translator.delete_glossary(glossary)\n```\n\n#### Listing entries in a stored glossary\n\nThe `GlossaryInfo` object does not contain the glossary entries, but instead\nonly the number of entries in the `entry_count` property.\n\nTo list the entries contained within a stored glossary, use\n`get_glossary_entries()` providing either the `GlossaryInfo` object or glossary\nID:\n\n```python\nentries = translator.get_glossary_entries(my_glossary)\nprint(entries)  # "{\'artist\': \'Maler\', \'prize\': \'Gewinn\'}"\n```\n\n#### Using a stored glossary\n\nYou can use a stored glossary for text translation by setting the `glossary`\nargument to either the glossary ID or `GlossaryInfo` object. You must also\nspecify the `source_lang` argument (it is required when using a glossary):\n\n```python\ntext = "The artist was awarded a prize."\nwith_glossary = translator.translate_text(\n    text, source_lang="EN", target_lang="DE", glossary=my_glossary,\n)\nprint(with_glossary)  # "Der Maler wurde mit einem Gewinn ausgezeichnet."\n\n# For comparison, the result without a glossary:\nwithout_glossary = translator.translate_text(text, target_lang="DE")\nprint(without_glossary)  # "Der Künstler wurde mit einem Preis ausgezeichnet."\n```\n\nUsing a stored glossary for document translation is the same: set the `glossary`\nargument and specify the `source_lang` argument:\n\n```python\ntranslator.translate_document(\n    in_file, out_file, source_lang="EN", target_lang="DE", glossary=my_glossary,\n)\n```\n\nThe `translate_document()`, `translate_document_from_filepath()` and\n`translate_document_upload()` functions all support the `glossary` argument.\n\n### Checking account usage\n\nTo check account usage, use the `get_usage()` function.\n\nThe returned `Usage` object contains three usage subtypes: `character`,\n`document` and `team_document`. Depending on your account type, some usage\nsubtypes may be invalid; this can be checked using the `valid` property. For API\naccounts:\n\n- `usage.character.valid` is `True`,\n- `usage.document.valid` and `usage.team_document.valid` are `False`.\n\nEach usage subtype (if valid) has `count` and `limit` properties giving the\namount used and maximum amount respectively, and the `limit_reached` property\nthat checks if the usage has reached the limit. The top level `Usage` object has\nthe `any_limit_reached` property to check all usage subtypes.\n\n```python\nusage = translator.get_usage()\nif usage.any_limit_reached:\n    print(\'Translation limit reached.\')\nif usage.character.valid:\n    print(\n        f"Character usage: {usage.character.count} of {usage.character.limit}")\nif usage.document.valid:\n    print(f"Document usage: {usage.document.count} of {usage.document.limit}")\n```\n\n### Listing available languages\n\nYou can request the list of languages supported by DeepL for text and documents\nusing the `get_source_languages()` and `get_target_languages()` functions. They\nboth return a list of `Language` objects.\n\nThe `name` property gives the name of the language in English, and the `code`\nproperty gives the language code. The `supports_formality` property only appears\nfor target languages, and indicates whether the target language supports the\noptional `formality` parameter.\n\n```python\nprint("Source languages:")\nfor language in translator.get_source_languages():\n    print(f"{language.name} ({language.code})")  # Example: "German (DE)"\n\nprint("Target languages:")\nfor language in translator.get_target_languages():\n    if language.supports_formality:\n        print(f"{language.name} ({language.code}) supports formality")\n        # Example: "Italian (IT) supports formality"\n    else:\n        print(f"{language.name} ({language.code})")\n        # Example: "Lithuanian (LT)"\n```\n\n#### Listing available glossary languages\n\nGlossaries are supported for a subset of language pairs. To retrieve those\nlanguages use the `get_glossary_languages()` function, which returns an array\nof `GlossaryLanguagePair` objects. Each has `source_lang` and `target_lang`\nproperties indicating that that pair of language codes is supported.\n\n```python\nglossary_languages = translator.get_glossary_languages()\nfor language_pair in glossary_languages:\n    print(f"{language_pair.source_lang} to {language_pair.target_lang}")\n    # Example: "EN to DE", "DE to EN", etc.\n```\n\nYou can also find the list of supported glossary language pairs in the\n[API documentation][api-docs-glossary-lang-list].\n\nNote that glossaries work for all target regional-variants: a glossary for the\ntarget language English (`"EN"`) supports translations to both American English\n(`"EN-US"`) and British English (`"EN-GB""`).\n\n### Exceptions\n\nAll module functions may raise `deepl.DeepLException` or one of its subclasses.\nIf invalid arguments are provided, they may raise the standard exceptions\n`ValueError` and `TypeError`.\n\n### Configuration\n\n#### Logging\n\nLogging can be enabled to see the HTTP requests sent and responses received by\nthe library. Enable and control logging using Python\'s `logging` module, for\nexample:\n\n```python\nimport logging\n\nlogging.basicConfig()\nlogging.getLogger(\'deepl\').setLevel(logging.DEBUG)\n```\n\n#### Server URL configuration\n\nYou can override the URL of the DeepL API by specifying the `server_url`\nargument when constructing a `deepl.Translator`. This may be useful for testing\npurposes. You **do not** need to specify the URL to distinguish API Free and API\nPro accounts, the library selects the correct URL automatically.\n\n```python\nserver_url = "http://user:pass@localhost:3000"\ntranslator = deepl.Translator(..., server_url=server_url)\n```\n\n#### Proxy configuration\n\nYou can configure a proxy by specifying the `proxy` argument when constructing a\n`deepl.Translator`:\n\n```python\nproxy = "http://user:pass@10.10.1.10:3128"\ntranslator = deepl.Translator(..., proxy=proxy)\n```\n\nThe proxy argument is passed to the underlying `requests` session, see the\n[documentation for requests][requests-proxy-docs]; a dictionary of schemes to\nproxy URLs is also accepted.\n\n## Command Line Interface\n\nThe library can be run on the command line supporting all API functions. Use the\n`--help` option for usage information:\n\n```shell\npython3 -m deepl --help\n```\n\nThe CLI requires your DeepL authentication key specified either as the\n`DEEPL_AUTH_KEY` environment variable, or using the `--auth-key` option, for\nexample:\n\n```shell\npython3 -m deepl --auth-key=YOUR_AUTH_KEY usage\n```\n\nNote that the `--auth-key` argument must appear *before* the command argument.\nThe recognized commands are:\n\n| Command   | Description                                            |\n| :-------- | :----------------------------------------------------- |\n| text      | translate text(s)                                      |\n| document  | translate document(s)                                  |\n| usage     | print usage information for the current billing period |\n| languages | print available languages                              |\n| glossary  | create, list, and remove glossaries                    |\n\nFor example, to translate text:\n\n```shell\npython3 -m deepl --auth-key=YOUR_AUTH_KEY text --to=DE "Text to be translated."\n```\n\nWrap text arguments in quotes to prevent the shell from splitting sentences into\nwords.\n\n## Issues\n\nIf you experience problems using the library, or would like to request a new\nfeature, please open an [issue][issues].\n\n## Development\n\nWe welcome Pull Requests, please read the\n[contributing guidelines](CONTRIBUTING.md).\n\n### Tests\n\nExecute the tests using `pytest`. The tests communicate with the DeepL API using\nthe auth key defined by the `DEEPL_AUTH_KEY` environment variable.\n\nBe aware that the tests make DeepL API requests that contribute toward your API\nusage.\n\nThe test suite may instead be configured to communicate with the mock-server\nprovided by [deepl-mock][deepl-mock]. Although most test cases work for either,\nsome test cases work only with the DeepL API or the mock-server and will be\notherwise skipped. The test cases that require the mock-server trigger server\nerrors and test the client error-handling. To execute the tests using\ndeepl-mock, run it in another terminal while executing the tests. Execute the\ntests using `pytest` with the `DEEPL_MOCK_SERVER_PORT` and `DEEPL_SERVER_URL`\nenvironment variables defined referring to the mock-server.\n\n[api-docs]: https://www.deepl.com/docs-api?utm_source=github&utm_medium=github-python-readme\n\n[api-docs-csv-format]: https://www.deepl.com/docs-api/managing-glossaries/supported-glossary-formats/?utm_source=github&utm_medium=github-python-readme\n\n[api-docs-xml-handling]: https://www.deepl.com/docs-api/handling-xml/?utm_source=github&utm_medium=github-python-readme\n\n[api-docs-lang-list]: https://www.deepl.com/docs-api/translating-text/?utm_source=github&utm_medium=github-python-readme\n\n[api-docs-glossary-lang-list]: https://www.deepl.com/docs-api/managing-glossaries/?utm_source=github&utm_medium=github-python-readme\n\n[create-account]: https://www.deepl.com/pro?utm_source=github&utm_medium=github-python-readme#developer\n\n[deepl-mock]: https://www.github.com/DeepLcom/deepl-mock\n\n[issues]: https://www.github.com/DeepLcom/deepl-python/issues\n\n[pypi-project]: https://pypi.org/project/deepl/\n\n[pro-account]: https://www.deepl.com/pro-account/?utm_source=github&utm_medium=github-python-readme\n\n[requests-proxy-docs]: https://docs.python-requests.org/en/latest/user/advanced/#proxies\n',
     'author': 'DeepL SE',
     'author_email': 'python-api@deepl.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/DeepLcom/deepl-python',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `deepl-1.8.0/PKG-INFO` & `deepl-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepl
-Version: 1.8.0
+Version: 1.9.0
 Summary: Python library for the DeepL API.
 Home-page: https://github.com/DeepLcom/deepl-python
 License: MIT
 Author: DeepL SE
 Author-email: python-api@deepl.com
 Requires-Python: >=3.6.2,<4
 Classifier: Development Status :: 5 - Production/Stable
@@ -288,14 +288,33 @@
     f"Created '{my_glossary.name}' ({my_glossary.glossary_id}) "
     f"{my_glossary.source_lang}->{my_glossary.target_lang} "
     f"containing {my_glossary.entry_count} entries"
 )
 # Example: Created 'My glossary' (559192ed-8e23-...) EN->DE containing 2 entries
 ```
 
+You can also upload a glossary downloaded from the DeepL website using
+`create_glossary_from_csv()`. Instead of supplying the entries as a dictionary,
+specify the CSV data as `csv_data` either as a file-like object or string or
+bytes containing file content:
+
+```python
+with open('/path/to/glossary_file.csv', 'r') as csv_file:
+    csv_data = csv_file.read()  # Read the file contents as a string
+    my_csv_glossary = translator.create_glossary_from_csv(
+        "CSV glossary",
+        source_lang="EN",
+        target_lang="DE",
+        csv_data=csv_data,
+    )
+```
+
+The [API documentation][api-docs-csv-format] explains the expected CSV format in
+detail.
+
 #### Getting, listing and deleting stored glossaries
 
 Functions to get, list, and delete stored glossaries are also provided:
 
 - `get_glossary()` takes a glossary ID and returns a `GlossaryInfo` object for a
   stored glossary, or raises an exception if no such glossary is found.
 - `list_glossaries()` returns a list of `GlossaryInfo` objects corresponding to
@@ -544,14 +563,16 @@
 errors and test the client error-handling. To execute the tests using
 deepl-mock, run it in another terminal while executing the tests. Execute the
 tests using `pytest` with the `DEEPL_MOCK_SERVER_PORT` and `DEEPL_SERVER_URL`
 environment variables defined referring to the mock-server.
 
 [api-docs]: https://www.deepl.com/docs-api?utm_source=github&utm_medium=github-python-readme
 
+[api-docs-csv-format]: https://www.deepl.com/docs-api/managing-glossaries/supported-glossary-formats/?utm_source=github&utm_medium=github-python-readme
+
 [api-docs-xml-handling]: https://www.deepl.com/docs-api/handling-xml/?utm_source=github&utm_medium=github-python-readme
 
 [api-docs-lang-list]: https://www.deepl.com/docs-api/translating-text/?utm_source=github&utm_medium=github-python-readme
 
 [api-docs-glossary-lang-list]: https://www.deepl.com/docs-api/managing-glossaries/?utm_source=github&utm_medium=github-python-readme
 
 [create-account]: https://www.deepl.com/pro?utm_source=github&utm_medium=github-python-readme#developer
```

