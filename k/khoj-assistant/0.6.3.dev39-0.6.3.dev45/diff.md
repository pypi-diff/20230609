# Comparing `tmp/khoj_assistant-0.6.3.dev39.tar.gz` & `tmp/khoj_assistant-0.6.3.dev45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Fri Jun  9 00:32:53 2023, max compression
+gzip compressed data, last modified: Fri Jun  9 13:06:49 2023, max compression
```

## Comparing `khoj_assistant-0.6.3.dev39.tar` & `khoj_assistant-0.6.3.dev45.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0        0 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/__init__.py
--rw-r--r--   0        0        0    10308 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/configure.py
--rw-r--r--   0        0        0     4929 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/main.py
--rw-r--r--   0        0        0        0 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/interface/desktop/__init__.py
--rw-r--r--   0        0        0     2987 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/interface/desktop/file_browser.py
--rw-r--r--   0        0        0      861 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/interface/desktop/labelled_text_field.py
--rw-r--r--   0        0        0    15746 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/interface/desktop/main_window.py
--rw-r--r--   0        0        0     1316 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/interface/desktop/system_tray.py
--rw-r--r--   0        0        0     9685 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/interface/web/chat.html
--rw-r--r--   0        0        0      546 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/interface/web/config.html
--rw-r--r--   0        0        0    12168 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/interface/web/index.html
--rw-r--r--   0        0        0      402 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/interface/web/khoj.webmanifest
--rw-r--r--   0        0        0      418 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/interface/web/khoj_chat.webmanifest
--rw-r--r--   0        0        0      437 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/interface/web/assets/config.css
--rw-r--r--   0        0        0     4515 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/interface/web/assets/config.js
--rw-r--r--   0        0        0   275822 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/interface/web/assets/markdown-it.min.js
--rw-r--r--   0        0        0    58507 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/interface/web/assets/org.min.js
--rw-r--r--   0        0        0    26348 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/interface/web/assets/icons/favicon-128x128.png
--rw-r--r--   0        0        0   162910 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/interface/web/assets/icons/favicon-144x144.ico
--rw-r--r--   0        0        0    29325 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/interface/web/assets/icons/favicon-144x144.png
--rw-r--r--   0        0        0   113060 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/interface/web/assets/icons/favicon.icns
--rw-r--r--   0        0        0        0 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/processor/__init__.py
--rw-r--r--   0        0        0     4216 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/processor/text_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/processor/conversation/__init__.py
--rw-r--r--   0        0        0     6053 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/processor/conversation/gpt.py
--rw-r--r--   0        0        0     4386 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/processor/conversation/prompts.py
--rw-r--r--   0        0        0     6478 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/processor/conversation/utils.py
--rw-r--r--   0        0        0        0 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/processor/jsonl/__init__.py
--rw-r--r--   0        0        0     3930 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/processor/jsonl/jsonl_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/processor/ledger/__init__.py
--rw-r--r--   0        0        0     5701 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/processor/ledger/beancount_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/processor/markdown/__init__.py
--rw-r--r--   0        0        0     6577 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/processor/markdown/markdown_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/processor/org_mode/__init__.py
--rw-r--r--   0        0        0     6526 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/processor/org_mode/org_to_jsonl.py
--rw-r--r--   0        0        0    16789 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/processor/org_mode/orgnode.py
--rw-r--r--   0        0        0        0 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/processor/pdf/__init__.py
--rw-r--r--   0        0        0     5153 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/processor/pdf/pdf_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/routers/__init__.py
--rw-r--r--   0        0        0    11138 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/routers/api.py
--rw-r--r--   0        0        0     1941 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/routers/api_beta.py
--rw-r--r--   0        0        0      803 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/routers/web_client.py
--rw-r--r--   0        0        0        0 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/search_filter/__init__.py
--rw-r--r--   0        0        0      463 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/search_filter/base_filter.py
--rw-r--r--   0        0        0     7470 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/search_filter/date_filter.py
--rw-r--r--   0        0        0     2713 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/search_filter/file_filter.py
--rw-r--r--   0        0        0     3690 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/search_filter/word_filter.py
--rw-r--r--   0        0        0        0 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/search_type/__init__.py
--rw-r--r--   0        0        0    11375 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/search_type/image_search.py
--rw-r--r--   0        0        0    10930 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/search_type/text_search.py
--rw-r--r--   0        0        0        0 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/utils/__init__.py
--rw-r--r--   0        0        0     2012 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/utils/cli.py
--rw-r--r--   0        0        0     2434 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/utils/config.py
--rw-r--r--   0        0        0     2713 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/utils/constants.py
--rw-r--r--   0        0        0     6703 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/utils/helpers.py
--rw-r--r--   0        0        0     1607 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/utils/jsonl.py
--rw-r--r--   0        0        0     2463 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/utils/models.py
--rw-r--r--   0        0        0     3781 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/utils/rawconfig.py
--rw-r--r--   0        0        0     1047 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/utils/state.py
--rw-r--r--   0        0        0     1239 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/src/khoj/utils/yaml.py
--rw-r--r--   0        0        0      523 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/.gitignore
--rw-r--r--   0        0        0    32472 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/LICENSE
--rw-r--r--   0        0        0    21788 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/README.md
--rw-r--r--   0        0        0     2759 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/pyproject.toml
--rw-r--r--   0        0        0    24096 2023-06-09 00:32:53.000000 khoj_assistant-0.6.3.dev39/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/__init__.py
+-rw-r--r--   0        0        0    10308 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/configure.py
+-rw-r--r--   0        0        0     4929 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/main.py
+-rw-r--r--   0        0        0        0 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/interface/desktop/__init__.py
+-rw-r--r--   0        0        0     2987 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/interface/desktop/file_browser.py
+-rw-r--r--   0        0        0      861 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/interface/desktop/labelled_text_field.py
+-rw-r--r--   0        0        0    15746 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/interface/desktop/main_window.py
+-rw-r--r--   0        0        0     1316 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/interface/desktop/system_tray.py
+-rw-r--r--   0        0        0     9707 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/interface/web/chat.html
+-rw-r--r--   0        0        0      546 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/interface/web/config.html
+-rw-r--r--   0        0        0    12201 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/interface/web/index.html
+-rw-r--r--   0        0        0      402 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/interface/web/khoj.webmanifest
+-rw-r--r--   0        0        0      418 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/interface/web/khoj_chat.webmanifest
+-rw-r--r--   0        0        0      437 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/interface/web/assets/config.css
+-rw-r--r--   0        0        0     4526 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/interface/web/assets/config.js
+-rw-r--r--   0        0        0   275822 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/interface/web/assets/markdown-it.min.js
+-rw-r--r--   0        0        0    58507 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/interface/web/assets/org.min.js
+-rw-r--r--   0        0        0    26348 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/interface/web/assets/icons/favicon-128x128.png
+-rw-r--r--   0        0        0   162910 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/interface/web/assets/icons/favicon-144x144.ico
+-rw-r--r--   0        0        0    29325 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/interface/web/assets/icons/favicon-144x144.png
+-rw-r--r--   0        0        0   113060 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/interface/web/assets/icons/favicon.icns
+-rw-r--r--   0        0        0        0 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/processor/__init__.py
+-rw-r--r--   0        0        0     4216 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/processor/text_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/processor/conversation/__init__.py
+-rw-r--r--   0        0        0     6053 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/processor/conversation/gpt.py
+-rw-r--r--   0        0        0     4386 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/processor/conversation/prompts.py
+-rw-r--r--   0        0        0     6478 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/processor/conversation/utils.py
+-rw-r--r--   0        0        0        0 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/processor/jsonl/__init__.py
+-rw-r--r--   0        0        0     3930 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/processor/jsonl/jsonl_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/processor/ledger/__init__.py
+-rw-r--r--   0        0        0     5701 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/processor/ledger/beancount_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/processor/markdown/__init__.py
+-rw-r--r--   0        0        0     6577 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/processor/markdown/markdown_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/processor/org_mode/__init__.py
+-rw-r--r--   0        0        0     6526 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/processor/org_mode/org_to_jsonl.py
+-rw-r--r--   0        0        0    16789 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/processor/org_mode/orgnode.py
+-rw-r--r--   0        0        0        0 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/processor/pdf/__init__.py
+-rw-r--r--   0        0        0     5153 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/processor/pdf/pdf_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/routers/__init__.py
+-rw-r--r--   0        0        0    11299 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/routers/api.py
+-rw-r--r--   0        0        0     1941 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/routers/api_beta.py
+-rw-r--r--   0        0        0      803 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/routers/web_client.py
+-rw-r--r--   0        0        0        0 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/search_filter/__init__.py
+-rw-r--r--   0        0        0      463 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/search_filter/base_filter.py
+-rw-r--r--   0        0        0     7470 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/search_filter/date_filter.py
+-rw-r--r--   0        0        0     2713 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/search_filter/file_filter.py
+-rw-r--r--   0        0        0     3690 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/search_filter/word_filter.py
+-rw-r--r--   0        0        0        0 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/search_type/__init__.py
+-rw-r--r--   0        0        0    11375 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/search_type/image_search.py
+-rw-r--r--   0        0        0    10930 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/search_type/text_search.py
+-rw-r--r--   0        0        0        0 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/utils/__init__.py
+-rw-r--r--   0        0        0     2012 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/utils/cli.py
+-rw-r--r--   0        0        0     2434 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/utils/config.py
+-rw-r--r--   0        0        0     2713 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/utils/constants.py
+-rw-r--r--   0        0        0     6779 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/utils/helpers.py
+-rw-r--r--   0        0        0     1607 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/utils/jsonl.py
+-rw-r--r--   0        0        0     2463 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/utils/models.py
+-rw-r--r--   0        0        0     3781 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/utils/rawconfig.py
+-rw-r--r--   0        0        0     1047 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/utils/state.py
+-rw-r--r--   0        0        0     1239 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/src/khoj/utils/yaml.py
+-rw-r--r--   0        0        0      523 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/.gitignore
+-rw-r--r--   0        0        0    32472 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/LICENSE
+-rw-r--r--   0        0        0    21788 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/README.md
+-rw-r--r--   0        0        0     2759 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/pyproject.toml
+-rw-r--r--   0        0        0    24096 2023-06-09 13:06:49.000000 khoj_assistant-0.6.3.dev45/PKG-INFO
```

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/configure.py` & `khoj_assistant-0.6.3.dev45/src/khoj/configure.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/main.py` & `khoj_assistant-0.6.3.dev45/src/khoj/main.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/interface/desktop/file_browser.py` & `khoj_assistant-0.6.3.dev45/src/khoj/interface/desktop/file_browser.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/interface/desktop/labelled_text_field.py` & `khoj_assistant-0.6.3.dev45/src/khoj/interface/desktop/labelled_text_field.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/interface/desktop/main_window.py` & `khoj_assistant-0.6.3.dev45/src/khoj/interface/desktop/main_window.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/interface/desktop/system_tray.py` & `khoj_assistant-0.6.3.dev45/src/khoj/interface/desktop/system_tray.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/interface/web/chat.html` & `khoj_assistant-0.6.3.dev45/src/khoj/interface/web/chat.html`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
                 return;
 
             // Add message by user to chat body
             renderMessage(query, "you");
             document.getElementById("chat-input").value = "";
 
             // Generate backend API URL to execute query
-            let url = `/api/chat?q=${encodeURIComponent(query)}`;
+            let url = `/api/chat?q=${encodeURIComponent(query)}&client=web`;
 
             // Call specified Khoj API
             fetch(url)
                 .then(response => response.json())
                 .then(data => {
                     // Render message by Khoj to chat body
                     console.log(data.response);
@@ -78,15 +78,15 @@
             // Send chat message on 'Enter'
             if (event.key === 'Enter') {
                 chat();
             }
         }
 
         window.onload = function () {
-            fetch('/api/chat')
+            fetch('/api/chat?client=web')
                 .then(response => response.json())
                 .then(data => data.response)
                 .then(chat_logs => {
                     // Render conversation history, if any
                     chat_logs.forEach(chat_log => {
                         renderMessageWithReference(chat_log.message, chat_log.by, chat_log.context, new Date(chat_log.created));
                     });
```

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/interface/web/config.html` & `khoj_assistant-0.6.3.dev45/src/khoj/interface/web/config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/interface/web/index.html` & `khoj_assistant-0.6.3.dev45/src/khoj/interface/web/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -86,16 +86,16 @@
 
             // If set query field in url query param on rerank
             if (rerank)
                 setQueryFieldInUrl(query);
 
             // Generate Backend API URL to execute Search
             url = type === "image"
-                ? `/api/search?q=${encodeURIComponent(query)}&t=${type}&n=${results_count}`
-                : `/api/search?q=${encodeURIComponent(query)}&t=${type}&n=${results_count}&r=${rerank}`;
+                ? `/api/search?q=${encodeURIComponent(query)}&t=${type}&n=${results_count}&client=web`
+                : `/api/search?q=${encodeURIComponent(query)}&t=${type}&n=${results_count}&r=${rerank}&client=web`;
 
             // Execute Search and Render Results
             fetch(url)
                 .then(response => response.json())
                 .then(data => {
                     console.log(data);
                     document.getElementById("results").innerHTML =
@@ -103,15 +103,15 @@
                         + render_json(data, query, type)
                         + `</div>`;
                 });
         }
 
         function updateIndex() {
             type = document.getElementById("type").value;
-            fetch(`/api/update?t=${type}`)
+            fetch(`/api/update?t=${type}&client=web`)
                 .then(response => response.json())
                 .then(data => {
                     console.log(data);
                     document.getElementById("results").innerHTML =
                         render_json(data);
                 });
         }
```

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/interface/web/assets/config.js` & `khoj_assistant-0.6.3.dev45/src/khoj/interface/web/assets/config.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -42,15 +42,15 @@
 /**
  * The click handler for the Regenerate button.
  */
 regenerateButton.addEventListener("click", (event) => {
     event.preventDefault();
     regenerateButton.style.cursor = "progress";
     regenerateButton.disabled = true;
-    fetch("/api/update?force=true")
+    fetch("/api/update?force=true&client=web")
         .then(response => response.json())
         .then(data => {
             regenerateButton.style.cursor = "pointer";
             regenerateButton.disabled = false;
             console.log(data);
         });
 })
```

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/interface/web/assets/markdown-it.min.js` & `khoj_assistant-0.6.3.dev45/src/khoj/interface/web/assets/markdown-it.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/interface/web/assets/org.min.js` & `khoj_assistant-0.6.3.dev45/src/khoj/interface/web/assets/org.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/interface/web/assets/icons/favicon-128x128.png` & `khoj_assistant-0.6.3.dev45/src/khoj/interface/web/assets/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/interface/web/assets/icons/favicon-144x144.ico` & `khoj_assistant-0.6.3.dev45/src/khoj/interface/web/assets/icons/favicon-144x144.ico`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/interface/web/assets/icons/favicon-144x144.png` & `khoj_assistant-0.6.3.dev45/src/khoj/interface/web/assets/icons/favicon-144x144.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/interface/web/assets/icons/favicon.icns` & `khoj_assistant-0.6.3.dev45/src/khoj/interface/web/assets/icons/favicon.icns`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/processor/text_to_jsonl.py` & `khoj_assistant-0.6.3.dev45/src/khoj/processor/text_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/processor/conversation/gpt.py` & `khoj_assistant-0.6.3.dev45/src/khoj/processor/conversation/gpt.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/processor/conversation/prompts.py` & `khoj_assistant-0.6.3.dev45/src/khoj/processor/conversation/prompts.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/processor/conversation/utils.py` & `khoj_assistant-0.6.3.dev45/src/khoj/processor/conversation/utils.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/processor/jsonl/jsonl_to_jsonl.py` & `khoj_assistant-0.6.3.dev45/src/khoj/processor/jsonl/jsonl_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/processor/ledger/beancount_to_jsonl.py` & `khoj_assistant-0.6.3.dev45/src/khoj/processor/ledger/beancount_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/processor/markdown/markdown_to_jsonl.py` & `khoj_assistant-0.6.3.dev45/src/khoj/processor/markdown/markdown_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/processor/org_mode/org_to_jsonl.py` & `khoj_assistant-0.6.3.dev45/src/khoj/processor/org_mode/org_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/processor/org_mode/orgnode.py` & `khoj_assistant-0.6.3.dev45/src/khoj/processor/org_mode/orgnode.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/processor/pdf/pdf_to_jsonl.py` & `khoj_assistant-0.6.3.dev45/src/khoj/processor/pdf/pdf_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/routers/api.py` & `khoj_assistant-0.6.3.dev45/src/khoj/routers/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 def search(
     q: str,
     n: Optional[int] = 5,
     t: Optional[SearchType] = None,
     r: Optional[bool] = False,
     score_threshold: Optional[Union[float, None]] = None,
     dedupe: Optional[bool] = True,
+    client: Optional[str] = None,
 ):
     results: List[SearchResponse] = []
     if q is None or q == "":
         logger.warn(f"No query param (q) passed in API call to initiate search")
         return results
 
     # initialize variables
@@ -177,22 +178,24 @@
             results = text_search.collate_results(hits, entries, results_count)
 
     # Cache results
     state.query_cache[query_cache_key] = results
 
     # Only log telemetry if query is new and not a continuation of previous query
     if state.previous_query is None or state.previous_query not in user_query:
-        state.telemetry += [log_telemetry(telemetry_type="api", api="search", app_config=state.config.app)]
+        state.telemetry += [
+            log_telemetry(telemetry_type="api", api="search", client=client, app_config=state.config.app)
+        ]
     state.previous_query = user_query
 
     return results
 
 
 @api.get("/update")
-def update(t: Optional[SearchType] = None, force: Optional[bool] = False):
+def update(t: Optional[SearchType] = None, force: Optional[bool] = False, client: Optional[str] = None):
     try:
         state.search_index_lock.acquire()
         state.model = configure_search(state.model, state.config, regenerate=force, t=t)
         state.search_index_lock.release()
     except ValueError as e:
         logger.error(e)
         raise HTTPException(status_code=500, detail=str(e))
@@ -203,21 +206,21 @@
         state.processor_config = configure_processor(state.config.processor)
     except ValueError as e:
         logger.error(e)
         raise HTTPException(status_code=500, detail=str(e))
     else:
         logger.info("📬 Processor reconfigured via API")
 
-    state.telemetry += [log_telemetry(telemetry_type="api", api="update", app_config=state.config.app)]
+    state.telemetry += [log_telemetry(telemetry_type="api", api="update", client=client, app_config=state.config.app)]
 
     return {"status": "ok", "message": "khoj reloaded"}
 
 
 @api.get("/chat")
-def chat(q: Optional[str] = None):
+def chat(q: Optional[str] = None, client: Optional[str] = None):
     if (
         state.processor_config is None
         or state.processor_config.conversation is None
         or state.processor_config.conversation.openai_api_key is None
     ):
         raise HTTPException(
             status_code=500, detail="Chat processor not configured. Configure OpenAI API key on server and restart it."
@@ -273,10 +276,10 @@
         q,
         gpt_response,
         user_message_metadata={"created": user_message_time},
         khoj_message_metadata={"context": compiled_references, "intent": {"inferred-queries": inferred_queries}},
         conversation_log=meta_log.get("chat", []),
     )
 
-    state.telemetry += [log_telemetry(telemetry_type="api", api="chat", app_config=state.config.app)]
+    state.telemetry += [log_telemetry(telemetry_type="api", api="chat", client=client, app_config=state.config.app)]
 
     return {"status": status, "response": gpt_response, "context": compiled_references}
```

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/routers/api_beta.py` & `khoj_assistant-0.6.3.dev45/src/khoj/routers/api_beta.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/routers/web_client.py` & `khoj_assistant-0.6.3.dev45/src/khoj/routers/web_client.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/search_filter/date_filter.py` & `khoj_assistant-0.6.3.dev45/src/khoj/search_filter/date_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/search_filter/file_filter.py` & `khoj_assistant-0.6.3.dev45/src/khoj/search_filter/file_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/search_filter/word_filter.py` & `khoj_assistant-0.6.3.dev45/src/khoj/search_filter/word_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/search_type/image_search.py` & `khoj_assistant-0.6.3.dev45/src/khoj/search_type/image_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/search_type/text_search.py` & `khoj_assistant-0.6.3.dev45/src/khoj/search_type/text_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/utils/cli.py` & `khoj_assistant-0.6.3.dev45/src/khoj/utils/cli.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/utils/config.py` & `khoj_assistant-0.6.3.dev45/src/khoj/utils/config.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/utils/constants.py` & `khoj_assistant-0.6.3.dev45/src/khoj/utils/constants.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/utils/helpers.py` & `khoj_assistant-0.6.3.dev45/src/khoj/utils/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Standard Packages
 from __future__ import annotations  # to avoid quoting type hints
 from collections import OrderedDict
 import datetime
 from importlib import import_module
+from importlib.metadata import version
 import logging
 from os import path
 from pathlib import Path
 import platform
-import requests
 import sys
 from time import perf_counter
 import torch
 from typing import Optional, Union, TYPE_CHECKING
 import uuid
 
 # Internal Packages
@@ -180,14 +180,15 @@
     if not app_config or not app_config.should_log_telemetry:
         return []
 
     # Populate telemetry data to log
     request_body = {
         "telemetry_type": telemetry_type,
         "server_id": get_server_id(),
+        "server_version": version("khoj-assistant"),
         "os": platform.system(),
         "timestamp": datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
     }
     if api:
         # API endpoint on server called by client
         request_body["api"] = api
     if client:
```

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/utils/jsonl.py` & `khoj_assistant-0.6.3.dev45/src/khoj/utils/jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/utils/models.py` & `khoj_assistant-0.6.3.dev45/src/khoj/utils/models.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/utils/rawconfig.py` & `khoj_assistant-0.6.3.dev45/src/khoj/utils/rawconfig.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/utils/state.py` & `khoj_assistant-0.6.3.dev45/src/khoj/utils/state.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev39/src/khoj/utils/yaml.py` & `khoj_assistant-0.6.3.dev45/src/khoj/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev39/.gitignore` & `khoj_assistant-0.6.3.dev45/.gitignore`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev39/LICENSE` & `khoj_assistant-0.6.3.dev45/LICENSE`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev39/README.md` & `khoj_assistant-0.6.3.dev45/README.md`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev39/pyproject.toml` & `khoj_assistant-0.6.3.dev45/pyproject.toml`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev39/PKG-INFO` & `khoj_assistant-0.6.3.dev45/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khoj-assistant
-Version: 0.6.3.dev39
+Version: 0.6.3.dev45
 Summary: A natural language search engine for your personal notes, transactions and images
 Project-URL: Homepage, https://github.com/debanjum/khoj#readme
 Project-URL: Issues, https://github.com/debanjum/khoj/issues
 Project-URL: Discussions, https://github.com/debanjum/khoj/discussions
 Project-URL: Releases, https://github.com/debanjum/khoj/releases
 Author: Debanjum Singh Solanky, Saba Imran
 License-Expression: GPL-3.0-or-later
```

