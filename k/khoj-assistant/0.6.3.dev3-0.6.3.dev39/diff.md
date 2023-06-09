# Comparing `tmp/khoj_assistant-0.6.3.dev3.tar.gz` & `tmp/khoj_assistant-0.6.3.dev39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun May 28 04:51:54 2023, max compression
+gzip compressed data, last modified: Fri Jun  9 00:32:53 2023, max compression
```

## Comparing `khoj_assistant-0.6.3.dev3.tar` & `khoj_assistant-0.6.3.dev39.tar`

### file list

```diff
@@ -1,62 +1,65 @@
--rw-r--r--   0        0        0        0 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/__init__.py
--rw-r--r--   0        0        0     9769 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/configure.py
--rw-r--r--   0        0        0     4929 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/main.py
--rw-r--r--   0        0        0        0 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/interface/desktop/__init__.py
--rw-r--r--   0        0        0     2904 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/interface/desktop/file_browser.py
--rw-r--r--   0        0        0      861 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/interface/desktop/labelled_text_field.py
--rw-r--r--   0        0        0    15746 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/interface/desktop/main_window.py
--rw-r--r--   0        0        0     1316 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/interface/desktop/system_tray.py
--rw-r--r--   0        0        0     9685 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/interface/web/chat.html
--rw-r--r--   0        0        0      546 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/interface/web/config.html
--rw-r--r--   0        0        0    11635 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/interface/web/index.html
--rw-r--r--   0        0        0      438 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/interface/web/khoj.webmanifest
--rw-r--r--   0        0        0      406 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/interface/web/khoj_chat.webmanifest
--rw-r--r--   0        0        0      437 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/interface/web/assets/config.css
--rw-r--r--   0        0        0     4515 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/interface/web/assets/config.js
--rw-r--r--   0        0        0   275822 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/interface/web/assets/markdown-it.min.js
--rw-r--r--   0        0        0    58507 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/interface/web/assets/org.min.js
--rw-r--r--   0        0        0    26348 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/interface/web/assets/icons/favicon-128x128.png
--rw-r--r--   0        0        0   162910 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/interface/web/assets/icons/favicon-144x144.ico
--rw-r--r--   0        0        0    29325 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/interface/web/assets/icons/favicon-144x144.png
--rw-r--r--   0        0        0   113060 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/interface/web/assets/icons/favicon.icns
--rw-r--r--   0        0        0        0 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/processor/__init__.py
--rw-r--r--   0        0        0     4216 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/processor/text_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/processor/conversation/__init__.py
--rw-r--r--   0        0        0     9530 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/processor/conversation/gpt.py
--rw-r--r--   0        0        0     5182 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/processor/conversation/utils.py
--rw-r--r--   0        0        0        0 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/processor/jsonl/__init__.py
--rw-r--r--   0        0        0     3930 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/processor/jsonl/jsonl_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/processor/ledger/__init__.py
--rw-r--r--   0        0        0     5701 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/processor/ledger/beancount_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/processor/markdown/__init__.py
--rw-r--r--   0        0        0     6577 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/processor/markdown/markdown_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/processor/org_mode/__init__.py
--rw-r--r--   0        0        0     6526 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/processor/org_mode/org_to_jsonl.py
--rw-r--r--   0        0        0    16789 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/processor/org_mode/orgnode.py
--rw-r--r--   0        0        0        0 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/routers/__init__.py
--rw-r--r--   0        0        0    10226 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/routers/api.py
--rw-r--r--   0        0        0     1941 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/routers/api_beta.py
--rw-r--r--   0        0        0      803 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/routers/web_client.py
--rw-r--r--   0        0        0        0 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/search_filter/__init__.py
--rw-r--r--   0        0        0      463 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/search_filter/base_filter.py
--rw-r--r--   0        0        0     7470 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/search_filter/date_filter.py
--rw-r--r--   0        0        0     2713 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/search_filter/file_filter.py
--rw-r--r--   0        0        0     3690 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/search_filter/word_filter.py
--rw-r--r--   0        0        0        0 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/search_type/__init__.py
--rw-r--r--   0        0        0    11375 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/search_type/image_search.py
--rw-r--r--   0        0        0    10930 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/search_type/text_search.py
--rw-r--r--   0        0        0        0 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/utils/__init__.py
--rw-r--r--   0        0        0     2012 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/utils/cli.py
--rw-r--r--   0        0        0     2379 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/utils/config.py
--rw-r--r--   0        0        0     2478 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/utils/constants.py
--rw-r--r--   0        0        0     6703 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/utils/helpers.py
--rw-r--r--   0        0        0     1607 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/utils/jsonl.py
--rw-r--r--   0        0        0     2463 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/utils/models.py
--rw-r--r--   0        0        0     3744 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/utils/rawconfig.py
--rw-r--r--   0        0        0     1047 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/utils/state.py
--rw-r--r--   0        0        0     1239 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/src/khoj/utils/yaml.py
--rw-r--r--   0        0        0      523 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/.gitignore
--rw-r--r--   0        0        0    32472 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/LICENSE
--rw-r--r--   0        0        0    21760 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/README.md
--rw-r--r--   0        0        0     2650 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/pyproject.toml
--rw-r--r--   0        0        0    23905 2023-05-28 04:51:54.000000 khoj_assistant-0.6.3.dev3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/__init__.py
+-rw-r--r--   0        0        0    10308 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/configure.py
+-rw-r--r--   0        0        0     4929 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/main.py
+-rw-r--r--   0        0        0        0 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/interface/desktop/__init__.py
+-rw-r--r--   0        0        0     2987 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/interface/desktop/file_browser.py
+-rw-r--r--   0        0        0      861 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/interface/desktop/labelled_text_field.py
+-rw-r--r--   0        0        0    15746 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/interface/desktop/main_window.py
+-rw-r--r--   0        0        0     1316 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/interface/desktop/system_tray.py
+-rw-r--r--   0        0        0     9685 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/interface/web/chat.html
+-rw-r--r--   0        0        0      546 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/interface/web/config.html
+-rw-r--r--   0        0        0    12168 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/interface/web/index.html
+-rw-r--r--   0        0        0      402 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/interface/web/khoj.webmanifest
+-rw-r--r--   0        0        0      418 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/interface/web/khoj_chat.webmanifest
+-rw-r--r--   0        0        0      437 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/interface/web/assets/config.css
+-rw-r--r--   0        0        0     4515 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/interface/web/assets/config.js
+-rw-r--r--   0        0        0   275822 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/interface/web/assets/markdown-it.min.js
+-rw-r--r--   0        0        0    58507 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/interface/web/assets/org.min.js
+-rw-r--r--   0        0        0    26348 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/interface/web/assets/icons/favicon-128x128.png
+-rw-r--r--   0        0        0   162910 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/interface/web/assets/icons/favicon-144x144.ico
+-rw-r--r--   0        0        0    29325 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/interface/web/assets/icons/favicon-144x144.png
+-rw-r--r--   0        0        0   113060 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/interface/web/assets/icons/favicon.icns
+-rw-r--r--   0        0        0        0 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/processor/__init__.py
+-rw-r--r--   0        0        0     4216 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/processor/text_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/processor/conversation/__init__.py
+-rw-r--r--   0        0        0     6053 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/processor/conversation/gpt.py
+-rw-r--r--   0        0        0     4386 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/processor/conversation/prompts.py
+-rw-r--r--   0        0        0     6478 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/processor/conversation/utils.py
+-rw-r--r--   0        0        0        0 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/processor/jsonl/__init__.py
+-rw-r--r--   0        0        0     3930 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/processor/jsonl/jsonl_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/processor/ledger/__init__.py
+-rw-r--r--   0        0        0     5701 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/processor/ledger/beancount_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/processor/markdown/__init__.py
+-rw-r--r--   0        0        0     6577 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/processor/markdown/markdown_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/processor/org_mode/__init__.py
+-rw-r--r--   0        0        0     6526 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/processor/org_mode/org_to_jsonl.py
+-rw-r--r--   0        0        0    16789 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/processor/org_mode/orgnode.py
+-rw-r--r--   0        0        0        0 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/processor/pdf/__init__.py
+-rw-r--r--   0        0        0     5153 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/processor/pdf/pdf_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/routers/__init__.py
+-rw-r--r--   0        0        0    11138 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/routers/api.py
+-rw-r--r--   0        0        0     1941 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/routers/api_beta.py
+-rw-r--r--   0        0        0      803 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/routers/web_client.py
+-rw-r--r--   0        0        0        0 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/search_filter/__init__.py
+-rw-r--r--   0        0        0      463 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/search_filter/base_filter.py
+-rw-r--r--   0        0        0     7470 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/search_filter/date_filter.py
+-rw-r--r--   0        0        0     2713 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/search_filter/file_filter.py
+-rw-r--r--   0        0        0     3690 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/search_filter/word_filter.py
+-rw-r--r--   0        0        0        0 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/search_type/__init__.py
+-rw-r--r--   0        0        0    11375 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/search_type/image_search.py
+-rw-r--r--   0        0        0    10930 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/search_type/text_search.py
+-rw-r--r--   0        0        0        0 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/utils/__init__.py
+-rw-r--r--   0        0        0     2012 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/utils/cli.py
+-rw-r--r--   0        0        0     2434 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/utils/config.py
+-rw-r--r--   0        0        0     2713 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/utils/constants.py
+-rw-r--r--   0        0        0     6703 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/utils/helpers.py
+-rw-r--r--   0        0        0     1607 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/utils/jsonl.py
+-rw-r--r--   0        0        0     2463 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/utils/models.py
+-rw-r--r--   0        0        0     3781 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/utils/rawconfig.py
+-rw-r--r--   0        0        0     1047 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/utils/state.py
+-rw-r--r--   0        0        0     1239 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/utils/yaml.py
+-rw-r--r--   0        0        0      523 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/.gitignore
+-rw-r--r--   0        0        0    32472 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/LICENSE
+-rw-r--r--   0        0        0    21788 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/README.md
+-rw-r--r--   0        0        0     2759 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/pyproject.toml
+-rw-r--r--   0        0        0    24096 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/PKG-INFO
```

### Comparing `khoj_assistant-0.6.3.dev3/src/khoj/configure.py` & `khoj_assistant-0.6.3.dev39/src/khoj/configure.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 # Internal Packages
 from khoj.processor.conversation.gpt import summarize
 from khoj.processor.ledger.beancount_to_jsonl import BeancountToJsonl
 from khoj.processor.jsonl.jsonl_to_jsonl import JsonlToJsonl
 from khoj.processor.markdown.markdown_to_jsonl import MarkdownToJsonl
 from khoj.processor.org_mode.org_to_jsonl import OrgToJsonl
+from khoj.processor.pdf.pdf_to_jsonl import PdfToJsonl
 from khoj.search_type import image_search, text_search
 from khoj.utils import constants, state
 from khoj.utils.config import SearchType, SearchModels, ProcessorConfigModel, ConversationProcessorConfigModel
 from khoj.utils.helpers import LRU, resolve_absolute_path, merge_dicts
 from khoj.utils.rawconfig import FullConfig, ProcessorConfig
 from khoj.search_filter.date_filter import DateFilter
 from khoj.search_filter.word_filter import WordFilter
@@ -128,14 +129,26 @@
             BeancountToJsonl,
             config.content_type.ledger,
             search_config=config.search_type.symmetric,
             regenerate=regenerate,
             filters=[DateFilter(), WordFilter(), FileFilter()],
         )
 
+    # Initialize PDF Search
+    if (t == state.SearchType.Pdf or t == None) and config.content_type.pdf:
+        logger.info("💸 Setting up search for pdf")
+        # Extract Entries, Generate PDF Embeddings
+        model.pdf_search = text_search.setup(
+            PdfToJsonl,
+            config.content_type.pdf,
+            search_config=config.search_type.asymmetric,
+            regenerate=regenerate,
+            filters=[DateFilter(), WordFilter(), FileFilter()],
+        )
+
     # Initialize Image Search
     if (t == state.SearchType.Image or t == None) and config.content_type.image:
         logger.info("🌄 Setting up search for images")
         # Extract Entries, Generate Image Embeddings
         model.image_search = image_search.setup(
             config.content_type.image, search_config=config.search_type.image, regenerate=regenerate
         )
```

### Comparing `khoj_assistant-0.6.3.dev3/src/khoj/main.py` & `khoj_assistant-0.6.3.dev39/src/khoj/main.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev3/src/khoj/interface/desktop/file_browser.py` & `khoj_assistant-0.6.3.dev39/src/khoj/interface/desktop/file_browser.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,16 @@
     def getFileFilter(self, search_type):
         if search_type == SearchType.Org:
             return "Org-Mode Files (*.org)"
         elif search_type == SearchType.Ledger:
             return "Beancount Files (*.bean *.beancount)"
         elif search_type == SearchType.Markdown:
             return "Markdown Files (*.md *.markdown)"
+        elif search_type == SearchType.Pdf:
+            return "Pdf Files (*.pdf)"
         elif search_type == SearchType.Music:
             return "Org-Music Files (*.org)"
         elif search_type == SearchType.Image:
             return "Images (*.jp[e]g)"
 
     def storeFilesSelectedInFileDialog(self):
         filepaths = self.getPaths()
```

### Comparing `khoj_assistant-0.6.3.dev3/src/khoj/interface/desktop/labelled_text_field.py` & `khoj_assistant-0.6.3.dev39/src/khoj/interface/desktop/labelled_text_field.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev3/src/khoj/interface/desktop/main_window.py` & `khoj_assistant-0.6.3.dev39/src/khoj/interface/desktop/main_window.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev3/src/khoj/interface/desktop/system_tray.py` & `khoj_assistant-0.6.3.dev39/src/khoj/interface/desktop/system_tray.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev3/src/khoj/interface/web/chat.html` & `khoj_assistant-0.6.3.dev39/src/khoj/interface/web/chat.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev3/src/khoj/interface/web/config.html` & `khoj_assistant-0.6.3.dev39/src/khoj/interface/web/config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev3/src/khoj/interface/web/index.html` & `khoj_assistant-0.6.3.dev39/src/khoj/interface/web/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -40,25 +40,36 @@
 
         function render_ledger(query, data) {
             return `<div id="results-ledger">` + data.map(function (item) {
                 return `<p>${item.entry}</p>`
             }).join("\n") + `</div>`;
         }
 
+        function render_pdf(query, data) {
+            return `<div id="results-pdf">` + data.map(function (item) {
+                let compiled_lines = item.additional.compiled.split("\n");
+                let filename = compiled_lines.shift();
+                let text_match = compiled_lines.join("\n")
+                return `<h2>${filename}</h2>\n<p>${text_match}</p>`
+            }).join("\n") + `</div>`;
+        }
+
         function render_json(data, query, type) {
             if (type === "markdown") {
                 return render_markdown(query, data);
             } else if (type === "org") {
                 return render_org(query, data);
             } else if (type === "music") {
                 return render_org(query, data, "music-");
             } else if (type === "image") {
                 return data.map(render_image).join('');
             } else if (type === "ledger") {
                 return render_ledger(query, data);
+            } else if (type === "pdf") {
+                return render_pdf(query, data);
             } else {
                 return `<div id="results-plugin">`
                     + data.map((item) => `<p>${item.entry}</p>`).join("\n")
                     + `</div>`;
             }
         }
 
@@ -275,14 +286,15 @@
             width: 20vw;
             border-radius: 10px;
             border: 1px solid #475569;
         }
         #json {
             white-space: pre-wrap;
         }
+        #results-pdf,
         #results-plugin,
         #results-ledger {
             text-align: left;
             white-space: pre-line;
         }
          #results-markdown {
             text-align: left;
```

### Comparing `khoj_assistant-0.6.3.dev3/src/khoj/interface/web/assets/config.js` & `khoj_assistant-0.6.3.dev39/src/khoj/interface/web/assets/config.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev3/src/khoj/interface/web/assets/markdown-it.min.js` & `khoj_assistant-0.6.3.dev39/src/khoj/interface/web/assets/markdown-it.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev3/src/khoj/interface/web/assets/org.min.js` & `khoj_assistant-0.6.3.dev39/src/khoj/interface/web/assets/org.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev3/src/khoj/interface/web/assets/icons/favicon-128x128.png` & `khoj_assistant-0.6.3.dev39/src/khoj/interface/web/assets/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev3/src/khoj/interface/web/assets/icons/favicon-144x144.ico` & `khoj_assistant-0.6.3.dev39/src/khoj/interface/web/assets/icons/favicon-144x144.ico`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev3/src/khoj/interface/web/assets/icons/favicon-144x144.png` & `khoj_assistant-0.6.3.dev39/src/khoj/interface/web/assets/icons/favicon-144x144.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev3/src/khoj/interface/web/assets/icons/favicon.icns` & `khoj_assistant-0.6.3.dev39/src/khoj/interface/web/assets/icons/favicon.icns`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev3/src/khoj/processor/text_to_jsonl.py` & `khoj_assistant-0.6.3.dev39/src/khoj/processor/text_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev3/src/khoj/processor/conversation/utils.py` & `khoj_assistant-0.6.3.dev39/src/khoj/processor/conversation/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # Standard Packages
 import os
 import logging
 from datetime import datetime
 
 # External Packages
+from langchain.chat_models import ChatOpenAI
+from langchain.llms import OpenAI
+from langchain.schema import ChatMessage
 import openai
 import tiktoken
 from tenacity import (
     before_sleep_log,
     retry,
     retry_if_exception_type,
     stop_after_attempt,
@@ -27,80 +30,109 @@
     retry=(
         retry_if_exception_type(openai.error.Timeout)
         | retry_if_exception_type(openai.error.APIError)
         | retry_if_exception_type(openai.error.APIConnectionError)
         | retry_if_exception_type(openai.error.RateLimitError)
         | retry_if_exception_type(openai.error.ServiceUnavailableError)
     ),
-    wait=wait_random_exponential(min=1, max=30),
-    stop=stop_after_attempt(6),
+    wait=wait_random_exponential(min=1, max=10),
+    stop=stop_after_attempt(3),
     before_sleep=before_sleep_log(logger, logging.DEBUG),
     reraise=True,
 )
 def completion_with_backoff(**kwargs):
-    openai.api_key = kwargs["api_key"] if kwargs.get("api_key") else os.getenv("OPENAI_API_KEY")
-    return openai.Completion.create(**kwargs, request_timeout=60)
+    prompt = kwargs.pop("prompt")
+    if "api_key" in kwargs:
+        kwargs["openai_api_key"] = kwargs.get("api_key")
+    else:
+        kwargs["openai_api_key"] = os.getenv("OPENAI_API_KEY")
+    llm = OpenAI(**kwargs, request_timeout=20, max_retries=1)
+    return llm(prompt)
 
 
 @retry(
     retry=(
         retry_if_exception_type(openai.error.Timeout)
         | retry_if_exception_type(openai.error.APIError)
         | retry_if_exception_type(openai.error.APIConnectionError)
         | retry_if_exception_type(openai.error.RateLimitError)
         | retry_if_exception_type(openai.error.ServiceUnavailableError)
     ),
     wait=wait_exponential(multiplier=1, min=4, max=10),
-    stop=stop_after_attempt(6),
+    stop=stop_after_attempt(3),
     before_sleep=before_sleep_log(logger, logging.DEBUG),
     reraise=True,
 )
-def chat_completion_with_backoff(**kwargs):
-    openai.api_key = kwargs["api_key"] if kwargs.get("api_key") else os.getenv("OPENAI_API_KEY")
-    return openai.ChatCompletion.create(**kwargs, request_timeout=60)
+def chat_completion_with_backoff(messages, model_name, temperature, openai_api_key=None):
+    chat = ChatOpenAI(
+        model_name=model_name,
+        temperature=temperature,
+        openai_api_key=openai_api_key or os.getenv("OPENAI_API_KEY"),
+        request_timeout=10,
+        max_retries=1,
+    )
+    return chat(messages).content
 
 
 def generate_chatml_messages_with_context(
     user_message, system_message, conversation_log={}, model_name="gpt-3.5-turbo", lookback_turns=2
 ):
     """Generate messages for ChatGPT with context from previous conversation"""
     # Extract Chat History for Context
-    chat_logs = [f'{chat["message"]}\n\nNotes:\n{chat.get("context","")}' for chat in conversation_log.get("chat", [])]
+    chat_logs = []
+    for chat in conversation_log.get("chat", []):
+        chat_notes = f'\n\n Notes:\n{chat.get("context")}' if chat.get("context") else "\n"
+        chat_logs += [chat["message"] + chat_notes]
+
     rest_backnforths = []
     # Extract in reverse chronological order
     for user_msg, assistant_msg in zip(chat_logs[-2::-2], chat_logs[::-2]):
         if len(rest_backnforths) >= 2 * lookback_turns:
             break
         rest_backnforths += reciprocal_conversation_to_chatml([user_msg, assistant_msg])[::-1]
 
     # Format user and system messages to chatml format
-    system_chatml_message = [message_to_chatml(system_message, "system")]
-    user_chatml_message = [message_to_chatml(user_message, "user")]
+    system_chatml_message = [ChatMessage(content=system_message, role="system")]
+    user_chatml_message = [ChatMessage(content=user_message, role="user")]
 
-    messages = user_chatml_message + rest_backnforths[:2] + system_chatml_message + rest_backnforths[2:]
+    messages = user_chatml_message + rest_backnforths + system_chatml_message
 
     # Truncate oldest messages from conversation history until under max supported prompt size by model
-    encoder = tiktoken.encoding_for_model(model_name)
-    tokens = sum([len(encoder.encode(value)) for message in messages for value in message.values()])
-    while tokens > max_prompt_size[model_name]:
-        messages.pop()
-        tokens = sum([len(encoder.encode(value)) for message in messages for value in message.values()])
+    messages = truncate_messages(messages, max_prompt_size[model_name], model_name)
 
     # Return message in chronological order
     return messages[::-1]
 
 
-def reciprocal_conversation_to_chatml(message_pair):
-    """Convert a single back and forth between user and assistant to chatml format"""
-    return [message_to_chatml(message, role) for message, role in zip(message_pair, ["user", "assistant"])]
+def truncate_messages(messages, max_prompt_size, model_name):
+    """Truncate messages to fit within max prompt size supported by model"""
+    encoder = tiktoken.encoding_for_model(model_name)
+    tokens = sum([len(encoder.encode(message.content)) for message in messages])
+    while tokens > max_prompt_size and len(messages) > 1:
+        messages.pop()
+        tokens = sum([len(encoder.encode(message.content)) for message in messages])
+
+    # Truncate last message if still over max supported prompt size by model
+    if tokens > max_prompt_size:
+        last_message = "\n".join(messages[-1].content.split("\n")[:-1])
+        original_question = "\n".join(messages[-1].content.split("\n")[-1:])
+        original_question_tokens = len(encoder.encode(original_question))
+        remaining_tokens = max_prompt_size - original_question_tokens
+        truncated_message = encoder.decode(encoder.encode(last_message)[:remaining_tokens]).strip()
+        logger.debug(
+            f"Truncate last message to fit within max prompt size of {max_prompt_size} supported by {model_name} model:\n {truncated_message}"
+        )
+        messages = [ChatMessage(content=truncated_message + original_question, role=messages[-1].role)]
+
+    return messages
 
 
-def message_to_chatml(message, role="assistant"):
-    """Create chatml message from message and role"""
-    return {"role": role, "content": message}
+def reciprocal_conversation_to_chatml(message_pair):
+    """Convert a single back and forth between user and assistant to chatml format"""
+    return [ChatMessage(content=message, role=role) for message, role in zip(message_pair, ["user", "assistant"])]
 
 
 def message_to_prompt(
     user_message, conversation_history="", gpt_message=None, start_sequence="\nAI:", restart_sequence="\nHuman:"
 ):
     """Create prompt for GPT from messages and conversation history"""
     gpt_message = f" {gpt_message}" if gpt_message else ""
```

### Comparing `khoj_assistant-0.6.3.dev3/src/khoj/processor/jsonl/jsonl_to_jsonl.py` & `khoj_assistant-0.6.3.dev39/src/khoj/processor/jsonl/jsonl_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev3/src/khoj/processor/ledger/beancount_to_jsonl.py` & `khoj_assistant-0.6.3.dev39/src/khoj/processor/ledger/beancount_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev3/src/khoj/processor/markdown/markdown_to_jsonl.py` & `khoj_assistant-0.6.3.dev39/src/khoj/processor/markdown/markdown_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev3/src/khoj/processor/org_mode/org_to_jsonl.py` & `khoj_assistant-0.6.3.dev39/src/khoj/processor/org_mode/org_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev3/src/khoj/processor/org_mode/orgnode.py` & `khoj_assistant-0.6.3.dev39/src/khoj/processor/org_mode/orgnode.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev3/src/khoj/routers/api.py` & `khoj_assistant-0.6.3.dev39/src/khoj/routers/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,14 +105,25 @@
                 user_query, state.model.markdown_search, rank_results=r, score_threshold=score_threshold, dedupe=dedupe
             )
 
         # collate and return results
         with timer("Collating results took", logger):
             results = text_search.collate_results(hits, entries, results_count)
 
+    elif (t == SearchType.Pdf or t == None) and state.model.pdf_search:
+        # query pdf files
+        with timer("Query took", logger):
+            hits, entries = text_search.query(
+                user_query, state.model.pdf_search, rank_results=r, score_threshold=score_threshold, dedupe=dedupe
+            )
+
+        # collate and return results
+        with timer("Collating results took", logger):
+            results = text_search.collate_results(hits, entries, results_count)
+
     elif (t == SearchType.Ledger or t == None) and state.model.ledger_search:
         # query transactions
         with timer("Query took", logger):
             hits, entries = text_search.query(
                 user_query, state.model.ledger_search, rank_results=r, score_threshold=score_threshold, dedupe=dedupe
             )
 
@@ -213,36 +224,44 @@
         )
 
     # Initialize Variables
     api_key = state.processor_config.conversation.openai_api_key
     model = state.processor_config.conversation.model
     chat_model = state.processor_config.conversation.chat_model
     user_message_time = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
+    conversation_type = "general" if q.startswith("@general") else "notes"
+    compiled_references = []
+    inferred_queries = []
 
     # Load Conversation History
     chat_session = state.processor_config.conversation.chat_session
     meta_log = state.processor_config.conversation.meta_log
 
     # If user query is empty, return chat history
     if not q:
         if meta_log.get("chat"):
             return {"status": "ok", "response": meta_log["chat"]}
         else:
             return {"status": "ok", "response": []}
 
-    # Infer search queries from user message
-    with timer("Extracting search queries took", logger):
-        inferred_queries = extract_questions(q, model=model, api_key=api_key, conversation_log=meta_log)
-
-    # Collate search results as context for GPT
-    with timer("Searching knowledge base took", logger):
-        result_list = []
-        for query in inferred_queries:
-            result_list.extend(search(query, n=5, r=True, score_threshold=-5.0, dedupe=False))
-        compiled_references = [item.additional["compiled"] for item in result_list]
+    if conversation_type == "notes":
+        # Infer search queries from user message
+        with timer("Extracting search queries took", logger):
+            inferred_queries = extract_questions(q, model=model, api_key=api_key, conversation_log=meta_log)
+
+        # Collate search results as context for GPT
+        with timer("Searching knowledge base took", logger):
+            result_list = []
+            for query in inferred_queries:
+                result_list.extend(search(query, n=5, r=True, score_threshold=-5.0, dedupe=False))
+            compiled_references = [item.additional["compiled"] for item in result_list]
+
+    # Switch to general conversation type if no relevant notes found for the given query
+    conversation_type = "notes" if compiled_references else "general"
+    logger.debug(f"Conversation Type: {conversation_type}")
 
     try:
         with timer("Generating chat response took", logger):
             gpt_response = converse(compiled_references, q, meta_log, model=chat_model, api_key=api_key)
         status = "ok"
     except Exception as e:
         gpt_response = str(e)
```

### Comparing `khoj_assistant-0.6.3.dev3/src/khoj/routers/api_beta.py` & `khoj_assistant-0.6.3.dev39/src/khoj/routers/api_beta.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev3/src/khoj/routers/web_client.py` & `khoj_assistant-0.6.3.dev39/src/khoj/routers/web_client.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev3/src/khoj/search_filter/date_filter.py` & `khoj_assistant-0.6.3.dev39/src/khoj/search_filter/date_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev3/src/khoj/search_filter/file_filter.py` & `khoj_assistant-0.6.3.dev39/src/khoj/search_filter/file_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev3/src/khoj/search_filter/word_filter.py` & `khoj_assistant-0.6.3.dev39/src/khoj/search_filter/word_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev3/src/khoj/search_type/image_search.py` & `khoj_assistant-0.6.3.dev39/src/khoj/search_type/image_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev3/src/khoj/search_type/text_search.py` & `khoj_assistant-0.6.3.dev39/src/khoj/search_type/text_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev3/src/khoj/utils/cli.py` & `khoj_assistant-0.6.3.dev39/src/khoj/utils/cli.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev3/src/khoj/utils/config.py` & `khoj_assistant-0.6.3.dev39/src/khoj/utils/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 class SearchType(str, Enum):
     Org = "org"
     Ledger = "ledger"
     Music = "music"
     Markdown = "markdown"
     Image = "image"
+    Pdf = "pdf"
 
 
 class ProcessorType(str, Enum):
     Conversation = "conversation"
 
 
 class TextSearchModel:
@@ -57,14 +58,15 @@
 
 @dataclass
 class SearchModels:
     orgmode_search: TextSearchModel = None
     ledger_search: TextSearchModel = None
     music_search: TextSearchModel = None
     markdown_search: TextSearchModel = None
+    pdf_search: TextSearchModel = None
     image_search: ImageSearchModel = None
     plugin_search: Dict[str, TextSearchModel] = None
 
 
 class ConversationProcessorConfigModel:
     def __init__(self, processor_config: ConversationProcessorConfig):
         self.openai_api_key = processor_config.openai_api_key
```

### Comparing `khoj_assistant-0.6.3.dev3/src/khoj/utils/constants.py` & `khoj_assistant-0.6.3.dev39/src/khoj/utils/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,20 @@
         },
         "ledger": {
             "input-files": None,
             "input-filter": None,
             "compressed-jsonl": "~/.khoj/content/ledger/ledger.jsonl.gz",
             "embeddings-file": "~/.khoj/content/ledger/ledger_embeddings.pt",
         },
+        "pdf": {
+            "input-files": None,
+            "input-filter": None,
+            "compressed-jsonl": "~/.khoj/content/pdf/pdf.jsonl.gz",
+            "embeddings-file": "~/.khoj/content/pdf/pdf_embeddings.pt",
+        },
         "image": {
             "input-directories": None,
             "input-filter": None,
             "embeddings-file": "~/.khoj/content/image/image_embeddings.pt",
             "batch-size": 50,
             "use-xmp-metadata": False,
         },
```

### Comparing `khoj_assistant-0.6.3.dev3/src/khoj/utils/helpers.py` & `khoj_assistant-0.6.3.dev39/src/khoj/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev3/src/khoj/utils/jsonl.py` & `khoj_assistant-0.6.3.dev39/src/khoj/utils/jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev3/src/khoj/utils/models.py` & `khoj_assistant-0.6.3.dev39/src/khoj/utils/models.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev3/src/khoj/utils/rawconfig.py` & `khoj_assistant-0.6.3.dev39/src/khoj/utils/rawconfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 
 class ContentConfig(ConfigBase):
     org: Optional[TextContentConfig]
     ledger: Optional[TextContentConfig]
     image: Optional[ImageContentConfig]
     music: Optional[TextContentConfig]
     markdown: Optional[TextContentConfig]
+    pdf: Optional[TextContentConfig]
     plugins: Optional[Dict[str, TextContentConfig]]
 
 
 class TextSearchConfig(ConfigBase):
     encoder: str
     cross_encoder: str
     encoder_type: Optional[str]
```

### Comparing `khoj_assistant-0.6.3.dev3/src/khoj/utils/state.py` & `khoj_assistant-0.6.3.dev39/src/khoj/utils/state.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev3/src/khoj/utils/yaml.py` & `khoj_assistant-0.6.3.dev39/src/khoj/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev3/.gitignore` & `khoj_assistant-0.6.3.dev39/.gitignore`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev3/LICENSE` & `khoj_assistant-0.6.3.dev39/LICENSE`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev3/README.md` & `khoj_assistant-0.6.3.dev39/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Khoj 🦅
 [![test](https://github.com/debanjum/khoj/actions/workflows/test.yml/badge.svg)](https://github.com/debanjum/khoj/actions/workflows/test.yml)
 [![dockerize](https://github.com/debanjum/khoj/actions/workflows/dockerize.yml/badge.svg)](https://github.com/debanjum/khoj/pkgs/container/khoj)
 [![pypi](https://github.com/debanjum/khoj/actions/workflows/pypi.yml/badge.svg)](https://pypi.org/project/khoj-assistant/)
 
-*A search assistant for your second brain*
+*An AI personal assistant for your digital brain*
 
 **Supported Plugins**
 
 [![Khoj on Obsidian](https://img.shields.io/badge/Obsidian-%23483699.svg?style=for-the-badge&logo=obsidian&logoColor=white)](https://github.com/debanjum/khoj/tree/master/src/interface/obsidian#readme)
 [![Khoj on Emacs](https://img.shields.io/badge/Emacs-%237F5AB6.svg?&style=for-the-badge&logo=gnu-emacs&logoColor=white)](https://github.com/debanjum/khoj/tree/master/src/interface/emacs#readme)
 
 ## Table of Contents
@@ -59,27 +59,27 @@
 - **Chat**
   - **Faster answers**: Find answers faster, smoother than search. No need to manually scan through your notes to find answers.
   - **Iterative discovery**: Iteratively explore and (re-)discover your notes
   - **Assisted creativity**: Smoothly weave across answers retrieval and content generation
 - **General**
   - **Natural**: Advanced natural language understanding using Transformer based ML Models
   - **Pluggable**: Modular architecture makes it easy to plug in new data sources, frontends and ML models
-  - **Multiple Sources**: Index your Org-mode and Markdown notes, Beancount transactions and Photos
+  - **Multiple Sources**: Index your Org-mode and Markdown notes, Beancount transactions, PDF files and Photos
   - **Multiple Interfaces**: Interact from your [Web Browser](./src/khoj/interface/web/index.html), [Emacs](./src/interface/emacs/khoj.el) or [Obsidian](./src/interface/obsidian/)
 
 ## Demos
 ### Khoj in Obsidian
 https://github.com/debanjum/khoj/assets/6413477/3e33d8ea-25bb-46c8-a3bf-c92f78d0f56b
 
 <details><summary>Description</summary>
 
 - Install Khoj via `pip` and start Khoj backend in non-gui mode
 - Install Khoj plugin via Community Plugins settings pane on Obsidian app
 - Check the new Khoj plugin settings
-- Let Khoj backend index the markdown files in the current Vault
+- Let Khoj backend index the markdown, pdf files in the current Vault
 - Open Khoj plugin on Obsidian via Search button on Left Pane
 - Search \"*Announce plugin to folks*\" in the [Obsidian Plugin docs](https://marcus.se.net/obsidian-plugin-docs/)
 - Jump to the [search result](https://marcus.se.net/obsidian-plugin-docs/publishing/submit-your-plugin)
 </details>
 
 ### Khoj in Emacs, Browser
 https://user-images.githubusercontent.com/6413477/184735169-92c78bf1-d827-4663-9087-a1ea194b8f4b.mp4
@@ -392,15 +392,15 @@
 
 ```shell
 git clone https://github.com/debanjum/khoj && cd khoj
 ```
 
 ##### 2. Configure
 
-- **Required**: Update [docker-compose.yml](./docker-compose.yml) to mount your images, (org-mode or markdown) notes and beancount directories
+- **Required**: Update [docker-compose.yml](./docker-compose.yml) to mount your images, (org-mode or markdown) notes, pdf and beancount directories
 - **Optional**: Edit application configuration in [khoj_docker.yml](./config/khoj_docker.yml)
 
 ##### 3. Run
 
 ```shell
 docker-compose up -d
 ```
```

### Comparing `khoj_assistant-0.6.3.dev3/pyproject.toml` & `khoj_assistant-0.6.3.dev39/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     "productivity",
     "NLP",
     "AI",
     "org-mode",
     "markdown",
     "beancount",
     "images",
+    "pdf",
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
@@ -40,23 +41,25 @@
     "defusedxml == 0.7.1",
     "fastapi == 0.77.1",
     "jinja2 == 3.1.2",
     "openai >= 0.27.0",
     "tiktoken >= 0.3.0",
     "tenacity >= 8.2.2",
     "pillow == 9.3.0",
-    "pydantic == 1.9.1",
+    "pydantic >= 1.9.1",
     "pyqt6 == 6.3.1",
     "pyyaml == 6.0",
     "rich >= 13.3.1",
     "schedule == 1.1.0",
     "sentence-transformers == 2.2.2",
     "torch == 1.13.1",
     "uvicorn == 0.17.6",
     "aiohttp == 3.8.4",
+    "langchain >= 0.0.187",
+    "pypdf >= 3.9.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/debanjum/khoj#readme"
 Issues = "https://github.com/debanjum/khoj/issues"
 Discussions = "https://github.com/debanjum/khoj/discussions"
@@ -71,14 +74,16 @@
 ]
 dev = [
     "khoj-assistant[test]",
     "mypy >= 1.0.1",
     "black >= 23.1.0",
     "pre-commit >= 3.0.4",
     "freezegun >= 1.2.0",
+    "factory-boy==3.2.1",
+    "Faker==18.10.1",
 ]
 
 [tool.hatch.version]
 source = "vcs"
 raw-options.local_scheme = "no-local-version"  # PEP440 compliant version for PyPi
 
 [tool.hatch.build.targets.sdist]
```

### Comparing `khoj_assistant-0.6.3.dev3/PKG-INFO` & `khoj_assistant-0.6.3.dev39/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: khoj-assistant
-Version: 0.6.3.dev3
+Version: 0.6.3.dev39
 Summary: A natural language search engine for your personal notes, transactions and images
 Project-URL: Homepage, https://github.com/debanjum/khoj#readme
 Project-URL: Issues, https://github.com/debanjum/khoj/issues
 Project-URL: Discussions, https://github.com/debanjum/khoj/discussions
 Project-URL: Releases, https://github.com/debanjum/khoj/releases
 Author: Debanjum Singh Solanky, Saba Imran
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
-Keywords: AI,NLP,beancount,images,markdown,org-mode,productivity,search,semantic-search
+Keywords: AI,NLP,beancount,images,markdown,org-mode,pdf,productivity,search,semantic-search
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -23,42 +23,46 @@
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Python: <3.11,>=3.8
 Requires-Dist: aiohttp==3.8.4
 Requires-Dist: dateparser==1.1.1
 Requires-Dist: defusedxml==0.7.1
 Requires-Dist: fastapi==0.77.1
 Requires-Dist: jinja2==3.1.2
+Requires-Dist: langchain>=0.0.187
 Requires-Dist: openai>=0.27.0
 Requires-Dist: pillow==9.3.0
-Requires-Dist: pydantic==1.9.1
+Requires-Dist: pydantic>=1.9.1
+Requires-Dist: pypdf>=3.9.0
 Requires-Dist: pyqt6==6.3.1
 Requires-Dist: pyyaml==6.0
 Requires-Dist: rich>=13.3.1
 Requires-Dist: schedule==1.1.0
 Requires-Dist: sentence-transformers==2.2.2
 Requires-Dist: tenacity>=8.2.2
 Requires-Dist: tiktoken>=0.3.0
 Requires-Dist: torch==1.13.1
 Requires-Dist: uvicorn==0.17.6
 Provides-Extra: dev
 Requires-Dist: black>=23.1.0; extra == 'dev'
+Requires-Dist: factory-boy==3.2.1; extra == 'dev'
+Requires-Dist: faker==18.10.1; extra == 'dev'
 Requires-Dist: freezegun>=1.2.0; extra == 'dev'
 Requires-Dist: khoj-assistant[test]; extra == 'dev'
 Requires-Dist: mypy>=1.0.1; extra == 'dev'
 Requires-Dist: pre-commit>=3.0.4; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: pytest>=7.1.2; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Khoj 🦅
 [![test](https://github.com/debanjum/khoj/actions/workflows/test.yml/badge.svg)](https://github.com/debanjum/khoj/actions/workflows/test.yml)
 [![dockerize](https://github.com/debanjum/khoj/actions/workflows/dockerize.yml/badge.svg)](https://github.com/debanjum/khoj/pkgs/container/khoj)
 [![pypi](https://github.com/debanjum/khoj/actions/workflows/pypi.yml/badge.svg)](https://pypi.org/project/khoj-assistant/)
 
-*A search assistant for your second brain*
+*An AI personal assistant for your digital brain*
 
 **Supported Plugins**
 
 [![Khoj on Obsidian](https://img.shields.io/badge/Obsidian-%23483699.svg?style=for-the-badge&logo=obsidian&logoColor=white)](https://github.com/debanjum/khoj/tree/master/src/interface/obsidian#readme)
 [![Khoj on Emacs](https://img.shields.io/badge/Emacs-%237F5AB6.svg?&style=for-the-badge&logo=gnu-emacs&logoColor=white)](https://github.com/debanjum/khoj/tree/master/src/interface/emacs#readme)
 
 ## Table of Contents
@@ -110,27 +114,27 @@
 - **Chat**
   - **Faster answers**: Find answers faster, smoother than search. No need to manually scan through your notes to find answers.
   - **Iterative discovery**: Iteratively explore and (re-)discover your notes
   - **Assisted creativity**: Smoothly weave across answers retrieval and content generation
 - **General**
   - **Natural**: Advanced natural language understanding using Transformer based ML Models
   - **Pluggable**: Modular architecture makes it easy to plug in new data sources, frontends and ML models
-  - **Multiple Sources**: Index your Org-mode and Markdown notes, Beancount transactions and Photos
+  - **Multiple Sources**: Index your Org-mode and Markdown notes, Beancount transactions, PDF files and Photos
   - **Multiple Interfaces**: Interact from your [Web Browser](./src/khoj/interface/web/index.html), [Emacs](./src/interface/emacs/khoj.el) or [Obsidian](./src/interface/obsidian/)
 
 ## Demos
 ### Khoj in Obsidian
 https://github.com/debanjum/khoj/assets/6413477/3e33d8ea-25bb-46c8-a3bf-c92f78d0f56b
 
 <details><summary>Description</summary>
 
 - Install Khoj via `pip` and start Khoj backend in non-gui mode
 - Install Khoj plugin via Community Plugins settings pane on Obsidian app
 - Check the new Khoj plugin settings
-- Let Khoj backend index the markdown files in the current Vault
+- Let Khoj backend index the markdown, pdf files in the current Vault
 - Open Khoj plugin on Obsidian via Search button on Left Pane
 - Search \"*Announce plugin to folks*\" in the [Obsidian Plugin docs](https://marcus.se.net/obsidian-plugin-docs/)
 - Jump to the [search result](https://marcus.se.net/obsidian-plugin-docs/publishing/submit-your-plugin)
 </details>
 
 ### Khoj in Emacs, Browser
 https://user-images.githubusercontent.com/6413477/184735169-92c78bf1-d827-4663-9087-a1ea194b8f4b.mp4
@@ -443,15 +447,15 @@
 
 ```shell
 git clone https://github.com/debanjum/khoj && cd khoj
 ```
 
 ##### 2. Configure
 
-- **Required**: Update [docker-compose.yml](./docker-compose.yml) to mount your images, (org-mode or markdown) notes and beancount directories
+- **Required**: Update [docker-compose.yml](./docker-compose.yml) to mount your images, (org-mode or markdown) notes, pdf and beancount directories
 - **Optional**: Edit application configuration in [khoj_docker.yml](./config/khoj_docker.yml)
 
 ##### 3. Run
 
 ```shell
 docker-compose up -d
 ```
```

