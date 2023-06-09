# Comparing `tmp/unstructured-0.7.2.tar.gz` & `tmp/unstructured-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured-0.7.2.tar", last modified: Wed Jun  7 18:12:05 2023, max compression
+gzip compressed data, was "unstructured-0.7.3.tar", last modified: Fri Jun  9 18:21:51 2023, max compression
```

## Comparing `unstructured-0.7.2.tar` & `unstructured-0.7.3.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:12:05.321691 unstructured-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-06-07 18:11:51.000000 unstructured-0.7.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-07 18:11:51.000000 unstructured-0.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17932 2023-06-07 18:12:05.321691 unstructured-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14544 2023-06-07 18:11:51.000000 unstructured-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:12:05.305690 unstructured-0.7.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-07 18:11:51.000000 unstructured-0.7.2/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-07 18:11:51.000000 unstructured-0.7.2/requirements/huggingface.in
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-07 18:11:51.000000 unstructured-0.7.2/requirements/ingest-azure.in
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-07 18:11:51.000000 unstructured-0.7.2/requirements/ingest-discord.in
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-07 18:11:51.000000 unstructured-0.7.2/requirements/ingest-github.in
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-07 18:11:51.000000 unstructured-0.7.2/requirements/ingest-gitlab.in
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-07 18:11:51.000000 unstructured-0.7.2/requirements/ingest-google-drive.in
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-07 18:11:51.000000 unstructured-0.7.2/requirements/ingest-reddit.in
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-07 18:11:51.000000 unstructured-0.7.2/requirements/ingest-s3.in
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-07 18:11:51.000000 unstructured-0.7.2/requirements/ingest-slack.in
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-07 18:11:51.000000 unstructured-0.7.2/requirements/ingest-wikipedia.in
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-07 18:11:51.000000 unstructured-0.7.2/requirements/local-inference.in
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-07 18:12:05.321691 unstructured-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-06-07 18:11:51.000000 unstructured-0.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:12:05.305690 unstructured-0.7.2/test_unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:11:51.000000 unstructured-0.7.2/test_unstructured/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:12:05.305690 unstructured-0.7.2/test_unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:11:51.000000 unstructured-0.7.2/test_unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-07 18:11:51.000000 unstructured-0.7.2/test_unstructured/nlp/mock_nltk.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-07 18:11:51.000000 unstructured-0.7.2/test_unstructured/nlp/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-07 18:11:51.000000 unstructured-0.7.2/test_unstructured/nlp/test_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-07 18:11:51.000000 unstructured-0.7.2/test_unstructured/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:12:05.305690 unstructured-0.7.2/unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:12:05.309691 unstructured-0.7.2/unstructured/cleaners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/cleaners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/cleaners/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/cleaners/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/cleaners/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:12:05.309691 unstructured-0.7.2/unstructured/documents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/documents/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/documents/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/documents/email_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/documents/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/documents/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:12:05.309691 unstructured-0.7.2/unstructured/file_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/file_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/file_utils/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/file_utils/exploration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/file_utils/file_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    14040 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/file_utils/filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/file_utils/google_filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/file_utils/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:12:05.309691 unstructured-0.7.2/unstructured/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/ingest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:12:05.309691 unstructured-0.7.2/unstructured/ingest/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/ingest/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/ingest/connector/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/ingest/connector/biomed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/ingest/connector/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/ingest/connector/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/ingest/connector/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/ingest/connector/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/ingest/connector/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/ingest/connector/google_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/ingest/connector/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/ingest/connector/reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/ingest/connector/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/ingest/connector/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/ingest/connector/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:12:05.309691 unstructured-0.7.2/unstructured/ingest/doc_processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/ingest/doc_processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/ingest/doc_processor/generalized.py
--rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/ingest/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/ingest/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24447 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/ingest/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:12:05.309691 unstructured-0.7.2/unstructured/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:12:05.317691 unstructured-0.7.2/unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/nlp/english-words.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/nlp/english_words.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/nlp/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/nlp/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/nlp/tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:12:05.321691 unstructured-0.7.2/unstructured/partition/
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8901 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/docx.py
--rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/epub.py
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/md.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/msg.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/odt.py
--rw-r--r--   0 runner    (1001) docker     (123)    12659 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/ppt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/pptx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/rtf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/text_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/xlsx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/partition/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:12:05.321691 unstructured-0.7.2/unstructured/staging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/staging/argilla.py
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/staging/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/staging/baseplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/staging/datasaur.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/staging/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/staging/label_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/staging/label_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/staging/prodigy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/staging/weaviate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-07 18:11:51.000000 unstructured-0.7.2/unstructured/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:12:05.305690 unstructured-0.7.2/unstructured.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17932 2023-06-07 18:12:05.000000 unstructured-0.7.2/unstructured.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-06-07 18:12:05.000000 unstructured-0.7.2/unstructured.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 18:12:05.000000 unstructured-0.7.2/unstructured.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-07 18:12:05.000000 unstructured-0.7.2/unstructured.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-07 18:12:05.000000 unstructured-0.7.2/unstructured.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-07 18:12:05.000000 unstructured-0.7.2/unstructured.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:51.852471 unstructured-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-06-09 18:21:39.000000 unstructured-0.7.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-09 18:21:39.000000 unstructured-0.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17932 2023-06-09 18:21:51.852471 unstructured-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14544 2023-06-09 18:21:39.000000 unstructured-0.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:51.832471 unstructured-0.7.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-09 18:21:39.000000 unstructured-0.7.3/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-09 18:21:39.000000 unstructured-0.7.3/requirements/huggingface.in
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-09 18:21:39.000000 unstructured-0.7.3/requirements/ingest-azure.in
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-09 18:21:39.000000 unstructured-0.7.3/requirements/ingest-discord.in
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-09 18:21:39.000000 unstructured-0.7.3/requirements/ingest-github.in
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-09 18:21:39.000000 unstructured-0.7.3/requirements/ingest-gitlab.in
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-09 18:21:39.000000 unstructured-0.7.3/requirements/ingest-google-drive.in
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-09 18:21:39.000000 unstructured-0.7.3/requirements/ingest-reddit.in
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-09 18:21:39.000000 unstructured-0.7.3/requirements/ingest-s3.in
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-09 18:21:39.000000 unstructured-0.7.3/requirements/ingest-slack.in
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-09 18:21:39.000000 unstructured-0.7.3/requirements/ingest-wikipedia.in
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-09 18:21:39.000000 unstructured-0.7.3/requirements/local-inference.in
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-09 18:21:51.856471 unstructured-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-06-09 18:21:39.000000 unstructured-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:51.832471 unstructured-0.7.3/test_unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:39.000000 unstructured-0.7.3/test_unstructured/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:51.832471 unstructured-0.7.3/test_unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:39.000000 unstructured-0.7.3/test_unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-09 18:21:39.000000 unstructured-0.7.3/test_unstructured/nlp/mock_nltk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-09 18:21:39.000000 unstructured-0.7.3/test_unstructured/nlp/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-09 18:21:39.000000 unstructured-0.7.3/test_unstructured/nlp/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-09 18:21:39.000000 unstructured-0.7.3/test_unstructured/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:51.832471 unstructured-0.7.3/unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:51.836471 unstructured-0.7.3/unstructured/cleaners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/cleaners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/cleaners/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/cleaners/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/cleaners/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:51.836471 unstructured-0.7.3/unstructured/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/documents/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/documents/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/documents/email_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/documents/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/documents/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:51.836471 unstructured-0.7.3/unstructured/file_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/file_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/file_utils/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/file_utils/exploration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/file_utils/file_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15494 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/file_utils/filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/file_utils/google_filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/file_utils/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:51.836471 unstructured-0.7.3/unstructured/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/ingest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:51.840471 unstructured-0.7.3/unstructured/ingest/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/ingest/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/ingest/connector/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/ingest/connector/biomed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/ingest/connector/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/ingest/connector/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/ingest/connector/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/ingest/connector/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/ingest/connector/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/ingest/connector/google_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/ingest/connector/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/ingest/connector/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/ingest/connector/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/ingest/connector/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/ingest/connector/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:51.840471 unstructured-0.7.3/unstructured/ingest/doc_processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/ingest/doc_processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/ingest/doc_processor/generalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/ingest/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/ingest/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24447 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/ingest/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:51.840471 unstructured-0.7.3/unstructured/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:51.848471 unstructured-0.7.3/unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/nlp/english-words.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/nlp/english_words.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/nlp/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/nlp/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/nlp/tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:51.852471 unstructured-0.7.3/unstructured/partition/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9232 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/docx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/epub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/odt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12797 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/ppt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/pptx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/rtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/text_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:51.852471 unstructured-0.7.3/unstructured/staging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/staging/argilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/staging/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/staging/baseplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/staging/datasaur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/staging/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/staging/label_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/staging/label_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/staging/prodigy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/staging/weaviate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:51.832471 unstructured-0.7.3/unstructured.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17932 2023-06-09 18:21:51.000000 unstructured-0.7.3/unstructured.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-06-09 18:21:51.000000 unstructured-0.7.3/unstructured.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:21:51.000000 unstructured-0.7.3/unstructured.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-09 18:21:51.000000 unstructured-0.7.3/unstructured.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-09 18:21:51.000000 unstructured-0.7.3/unstructured.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-09 18:21:51.000000 unstructured-0.7.3/unstructured.egg-info/top_level.txt
```

### Comparing `unstructured-0.7.2/LICENSE.md` & `unstructured-0.7.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/PKG-INFO` & `unstructured-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.7.2
+Version: 0.7.3
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.7.2 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.7.3 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
```

### Comparing `unstructured-0.7.2/README.md` & `unstructured-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/setup.py` & `unstructured-0.7.3/setup.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/test_unstructured/nlp/mock_nltk.py` & `unstructured-0.7.3/test_unstructured/nlp/mock_nltk.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/test_unstructured/nlp/test_tokenize.py` & `unstructured-0.7.3/test_unstructured/nlp/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/test_unstructured/test_utils.py` & `unstructured-0.7.3/test_unstructured/test_utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/cleaners/core.py` & `unstructured-0.7.3/unstructured/cleaners/core.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/cleaners/extract.py` & `unstructured-0.7.3/unstructured/cleaners/extract.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/cleaners/translate.py` & `unstructured-0.7.3/unstructured/cleaners/translate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/documents/base.py` & `unstructured-0.7.3/unstructured/documents/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/documents/elements.py` & `unstructured-0.7.3/unstructured/documents/elements.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,25 +2,41 @@
 
 import datetime
 import hashlib
 import os
 import pathlib
 from abc import ABC
 from dataclasses import dataclass
-from typing import Any, Callable, Dict, List, Optional, Tuple, Union
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union, cast
 
 
 class NoID(ABC):
     """Class to indicate that an element do not have an ID."""
 
     pass
 
 
 @dataclass
+class DataSourceMetadata:
+    """Metadata fields that pertain to the data source of the document."""
+
+    url: Optional[str] = None
+    version: Optional[str] = None
+    record_locator: Optional[Dict[str, Any]] = None  # Values must be JSON-serializable
+    date_created: Optional[str] = None
+    date_modified: Optional[str] = None
+    date_processed: Optional[str] = None
+
+    def to_dict(self):
+        return {key: value for key, value in self.__dict__.items() if value is not None}
+
+
+@dataclass
 class ElementMetadata:
+    data_source: Optional[DataSourceMetadata] = None
     filename: Optional[str] = None
     file_directory: Optional[str] = None
     date: Optional[str] = None
     filetype: Optional[str] = None
 
     # Page numbers currenlty supported for PDF, HTML and PPT documents
     page_number: Optional[int] = None
@@ -45,15 +61,18 @@
 
         if self.filename is not None:
             file_directory, filename = os.path.split(self.filename)
             self.file_directory = file_directory or None
             self.filename = filename
 
     def to_dict(self):
-        return {key: value for key, value in self.__dict__.items() if value is not None}
+        dict = {key: value for key, value in self.__dict__.items() if value is not None}
+        if self.data_source:
+            dict["data_source"] = cast(DataSourceMetadata, self.data_source).to_dict()
+        return dict
 
     @classmethod
     def from_dict(cls, input_dict):
         return cls(**input_dict)
 
     def merge(self, other: ElementMetadata):
         for k in self.__dict__:
```

### Comparing `unstructured-0.7.2/unstructured/documents/email_elements.py` & `unstructured-0.7.3/unstructured/documents/email_elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/documents/html.py` & `unstructured-0.7.3/unstructured/documents/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/documents/xml.py` & `unstructured-0.7.3/unstructured/documents/xml.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/file_utils/encoding.py` & `unstructured-0.7.3/unstructured/file_utils/encoding.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/file_utils/exploration.py` & `unstructured-0.7.3/unstructured/file_utils/exploration.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/file_utils/file_conversion.py` & `unstructured-0.7.3/unstructured/file_utils/file_conversion.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/file_utils/filetype.py` & `unstructured-0.7.3/unstructured/file_utils/filetype.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import re
 import zipfile
 from enum import Enum
 from functools import wraps
 from typing import IO, Callable, List, Optional
 
 from unstructured.documents.elements import Element, PageBreak
+from unstructured.file_utils.encoding import detect_file_encoding
 from unstructured.nlp.patterns import LIST_OF_DICTS_PATTERN
 from unstructured.partition.common import (
     _add_element_metadata,
     _remove_element_metadata,
     exactly_one,
 )
 
@@ -186,14 +187,15 @@
 
 
 def detect_filetype(
     filename: Optional[str] = None,
     content_type: Optional[str] = None,
     file: Optional[IO] = None,
     file_filename: Optional[str] = None,
+    encoding: Optional[str] = "utf-8",
 ) -> Optional[FileType]:
     """Use libmagic to determine a file's type. Helps determine which partition brick
     to use for a given file. A return value of None indicates a non-supported file type.
     """
     exactly_one(filename=filename, file=file)
 
     if content_type:
@@ -253,17 +255,20 @@
         elif extension and extension == ".md":
             return FileType.MD
         elif extension and extension == ".rtf":
             return FileType.RTF
         elif extension and extension == ".html":
             return FileType.HTML
 
-        if _is_text_file_a_json(file=file, filename=filename):
+        if _is_text_file_a_json(file=file, filename=filename, encoding=encoding):
             return FileType.JSON
 
+        if _is_text_file_a_csv(file=file, filename=filename, encoding=encoding):
+            return FileType.CSV
+
         if file and not extension and _check_eml_from_buffer(file=file) is True:
             return FileType.EML
 
         # Safety catch
         if mime_type in STR_TO_FILETYPE:
             return STR_TO_FILETYPE[mime_type]
 
@@ -323,47 +328,76 @@
 
     logger.warning(
         "Could not detect the filetype from application/octet-stream MIME type.",
     )
     return FileType.UNK
 
 
-def _is_text_file_a_json(
+def _read_file_start_for_type_check(
     filename: Optional[str] = None,
-    content_type: Optional[str] = None,
     file: Optional[IO] = None,
-):
-    """Detects if a file that has a text/plain MIME type is a JSON file."""
+    encoding: Optional[str] = "utf-8",
+) -> str:
+    """Reads the start of the file and returns the text content."""
     exactly_one(filename=filename, file=file)
-
     if file is not None:
         file.seek(0)
         file_content = file.read(4096)
         if isinstance(file_content, str):
             file_text = file_content
         else:
             file_text = file_content.decode(errors="ignore")
         file.seek(0)
-    elif filename is not None:
-        with open(filename) as f:
-            file_text = f.read()
+    if filename is not None:
+        try:
+            with open(filename, encoding=encoding) as f:
+                file_text = f.read(4096)
+        except UnicodeDecodeError:
+            encoding, _ = detect_file_encoding(filename=filename)
+            with open(filename, encoding=encoding) as f:
+                file_text = f.read(4096)
+    return file_text
+
 
+def _is_text_file_a_json(
+    filename: Optional[str] = None,
+    file: Optional[IO] = None,
+    encoding: Optional[str] = "utf-8",
+):
+    """Detects if a file that has a text/plain MIME type is a JSON file."""
+    file_text = _read_file_start_for_type_check(file=file, filename=filename, encoding=encoding)
     return re.match(LIST_OF_DICTS_PATTERN, file_text) is not None
 
 
+def _is_text_file_a_csv(
+    filename: Optional[str] = None,
+    file: Optional[IO] = None,
+    encoding: Optional[str] = "utf-8",
+):
+    """Detects if a file that has a text/plain MIME type is a CSV file."""
+    file_text = _read_file_start_for_type_check(file=file, filename=filename, encoding=encoding)
+    lines = file_text.strip().splitlines()
+    if len(lines) < 2:
+        return False
+    lines = lines[: len(lines)] if len(lines) < 10 else lines[:10]
+    header = lines[0].split(",")
+    if any("," not in line for line in lines):
+        return False
+    return all(len(line.split(",")) == len(header) for line in lines[:-1])
+
+
 def _check_eml_from_buffer(file: IO) -> bool:
     """Checks if a text/plain file is actually a .eml file. Uses a regex pattern to see if the
     start of the file matches the typical pattern for a .eml file."""
     file.seek(0)
     file_content = file.read(4096)
     if isinstance(file_content, bytes):
         file_head = file_content.decode("utf-8", errors="ignore")
     else:
         file_head = file_content
-
     return EMAIL_HEAD_RE.match(file_head) is not None
 
 
 def document_to_element_list(
     document,
     include_page_breaks: bool = False,
 ) -> List[Element]:
```

### Comparing `unstructured-0.7.2/unstructured/file_utils/metadata.py` & `unstructured-0.7.3/unstructured/file_utils/metadata.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/ingest/connector/azure.py` & `unstructured-0.7.3/unstructured/ingest/connector/azure.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/ingest/connector/biomed.py` & `unstructured-0.7.3/unstructured/ingest/connector/biomed.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/ingest/connector/discord.py` & `unstructured-0.7.3/unstructured/ingest/connector/discord.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/ingest/connector/fsspec.py` & `unstructured-0.7.3/unstructured/ingest/connector/fsspec.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/ingest/connector/git.py` & `unstructured-0.7.3/unstructured/ingest/connector/git.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/ingest/connector/github.py` & `unstructured-0.7.3/unstructured/ingest/connector/github.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/ingest/connector/gitlab.py` & `unstructured-0.7.3/unstructured/ingest/connector/gitlab.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/ingest/connector/google_drive.py` & `unstructured-0.7.3/unstructured/ingest/connector/google_drive.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/ingest/connector/local.py` & `unstructured-0.7.3/unstructured/ingest/connector/local.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/ingest/connector/reddit.py` & `unstructured-0.7.3/unstructured/ingest/connector/reddit.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/ingest/connector/s3.py` & `unstructured-0.7.3/unstructured/ingest/connector/s3.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/ingest/connector/slack.py` & `unstructured-0.7.3/unstructured/ingest/connector/slack.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/ingest/connector/wikipedia.py` & `unstructured-0.7.3/unstructured/ingest/connector/wikipedia.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/ingest/doc_processor/generalized.py` & `unstructured-0.7.3/unstructured/ingest/doc_processor/generalized.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/ingest/main.py` & `unstructured-0.7.3/unstructured/ingest/main.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/nlp/english-words.txt` & `unstructured-0.7.3/unstructured/nlp/english-words.txt`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/nlp/english_words.py` & `unstructured-0.7.3/unstructured/nlp/english_words.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/nlp/patterns.py` & `unstructured-0.7.3/unstructured/nlp/patterns.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,7 +101,8 @@
 
 ENDS_IN_PUNCT_PATTERN = r"[^\w\s]\Z"
 ENDS_IN_PUNCT_RE = re.compile(ENDS_IN_PUNCT_PATTERN)
 
 # NOTE(robinson) - Used to detect if text is in the expected "list of dicts"
 # format for document elements
 LIST_OF_DICTS_PATTERN = r"\A\s*\[\s*{?"
+JSON_PATTERN = r"^(?:\{.*\}|\[.*\])$"
```

### Comparing `unstructured-0.7.2/unstructured/nlp/tokenize.py` & `unstructured-0.7.3/unstructured/nlp/tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/partition/__init__.py` & `unstructured-0.7.3/unstructured/partition/__init__.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/partition/api.py` & `unstructured-0.7.3/unstructured/partition/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import contextlib
-import json
 from typing import (
     IO,
     List,
     Optional,
 )
 
 import requests
 
 from unstructured.documents.elements import Element
 from unstructured.partition.common import exactly_one
-from unstructured.partition.json import partition_json
+from unstructured.staging.base import dict_to_elements, elements_from_json
 
 
 def partition_via_api(
     filename: Optional[str] = None,
     content_type: Optional[str] = None,
     file: Optional[IO] = None,
     file_filename: Optional[str] = None,
@@ -78,15 +77,15 @@
             )
         files = [
             ("files", (file_filename, file, content_type)),  # type: ignore
         ]
         response = requests.post(api_url, headers=headers, data=data, files=files)  # type: ignore
 
     if response.status_code == 200:
-        return partition_json(text=response.text)
+        return elements_from_json(text=response.text)
     else:
         raise ValueError(
             f"Receive unexpected status code {response.status_code} from the API.",
         )
 
 
 def partition_multiple_via_api(
@@ -168,14 +167,20 @@
             filename = file_filenames[i]
             _files.append(("files", (filename, _file, content_type)))
 
         response = requests.post(api_url, headers=headers, data=data, files=_files)  # type: ignore
 
     if response.status_code == 200:
         documents = []
-        for document in response.json():
-            documents.append(partition_json(text=json.dumps(document)))
+        response_list = response.json()
+        # NOTE(robinson) - this check is because if only one filename is passed, the return
+        # type from the API is a list of objects instead of a list of lists
+        if not isinstance(response_list[0], list):
+            response_list = [response_list]
+
+        for document in response_list:
+            documents.append(dict_to_elements(document))
         return documents
     else:
         raise ValueError(
             f"Receive unexpected status code {response.status_code} from the API.",
         )
```

### Comparing `unstructured-0.7.2/unstructured/partition/auto.py` & `unstructured-0.7.3/unstructured/partition/auto.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import io
 from typing import IO, Callable, Dict, Optional, Tuple
 
 import requests
 
+from unstructured.documents.elements import DataSourceMetadata
 from unstructured.file_utils.filetype import (
     FILETYPE_TO_MIMETYPE,
     STR_TO_FILETYPE,
     FileType,
     detect_filetype,
 )
 from unstructured.logger import logger
@@ -42,14 +43,15 @@
     encoding: Optional[str] = None,
     paragraph_grouper: Optional[Callable[[str], str]] = None,
     headers: Dict[str, str] = {},
     ssl_verify: bool = True,
     ocr_languages: str = "eng",
     pdf_infer_table_structure: bool = False,
     xml_keep_tags: bool = False,
+    data_source_metadata: Optional[DataSourceMetadata] = None,
 ):
     """Partitions a document into its constituent elements. Will use libmagic to determine
     the file's type and route it to the appropriate partitioning function. Applies the default
     parameters for each partitioning function. Use the document-type specific partitioning
     functions if you need access to additional kwarg options.
 
     Parameters
@@ -64,16 +66,16 @@
         When file is not None, the filename (string) to store in element metadata. E.g. "foo.txt"
     url
         The url for a remote document. Pass in content_type if you want partition to treat
         the document as a specific content_type.
     include_page_breaks
         If True, the output will include page breaks if the filetype supports it
     strategy
-        The strategy to use for partitioning the PDF. Uses a layout detection model if set
-        to 'hi_res', otherwise partition_pdf simply extracts the text from the document
+        The strategy to use for partitioning PDF/image. Uses a layout detection model if set
+        to 'hi_res', otherwise partition simply extracts the text from the document
         and processes it.
     encoding
         The encoding method used to decode the text input. If None, utf-8 will be used.
     headers
         The headers to be used in conjunction with the HTTP request if URL is set.
     ssl_verify
         If the URL parameter is set, determines whether or not partition uses SSL verification
@@ -106,14 +108,15 @@
                 "The headers kwarg will be ignored.",
             )
         filetype = detect_filetype(
             filename=filename,
             file=file,
             file_filename=file_filename,
             content_type=content_type,
+            encoding=encoding,
         )
 
     if file is not None:
         file.seek(0)
 
     if filetype == FileType.DOC:
         elements = partition_doc(filename=filename, file=file)
@@ -163,14 +166,15 @@
         )
     elif (filetype == FileType.PNG) or (filetype == FileType.JPG):
         elements = partition_image(
             filename=filename,  # type: ignore
             file=file,  # type: ignore
             url=None,
             include_page_breaks=include_page_breaks,
+            strategy=strategy,
             ocr_languages=ocr_languages,
         )
     elif filetype == FileType.TXT:
         elements = partition_text(
             filename=filename,
             file=file,
             encoding=encoding,
@@ -202,14 +206,15 @@
         elements = partition_csv(filename=filename, file=file)
     else:
         msg = "Invalid file" if not filename else f"Invalid file {filename}"
         raise ValueError(f"{msg}. The {filetype} file type is not supported in partition.")
 
     for element in elements:
         element.metadata.url = url
+        element.metadata.data_source = data_source_metadata
         if content_type is not None:
             out_filetype = STR_TO_FILETYPE.get(content_type)
             element.metadata.filetype = (
                 FILETYPE_TO_MIMETYPE[out_filetype] if out_filetype is not None else None
             )
         else:
             element.metadata.filetype = FILETYPE_TO_MIMETYPE[filetype]
@@ -223,9 +228,11 @@
     headers: Dict[str, str] = {},
     ssl_verify: bool = True,
 ) -> Tuple[io.BytesIO, Optional[FileType]]:
     response = requests.get(url, headers=headers, verify=ssl_verify)
     file = io.BytesIO(response.content)
 
     content_type = content_type or response.headers.get("Content-Type")
-    filetype = detect_filetype(file=file, content_type=content_type)
+    encoding = response.headers.get("Content-Encoding", "utf-8")
+
+    filetype = detect_filetype(file=file, content_type=content_type, encoding=encoding)
     return file, filetype
```

### Comparing `unstructured-0.7.2/unstructured/partition/common.py` & `unstructured-0.7.3/unstructured/partition/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     CheckBox,
     Element,
     ElementMetadata,
     ListItem,
     PageBreak,
     Text,
 )
+from unstructured.logger import logger
 from unstructured.nlp.patterns import ENUMERATED_BULLETS_RE, UNICODE_BULLETS_RE
 
 
 def normalize_layout_element(layout_element) -> Union[Element, List[Element]]:
     """Converts a list of unstructured_inference DocumentLayout objects to a list of
     unstructured Elements."""
 
@@ -135,36 +136,44 @@
 
 def convert_office_doc(input_filename: str, output_directory: str, target_format: str):
     """Converts a .doc file to a .docx file using the libreoffice CLI."""
     # NOTE(robinson) - In the future can also include win32com client as a fallback for windows
     # users who do not have LibreOffice installed
     # ref: https://stackoverflow.com/questions/38468442/
     #       multiple-doc-to-docx-file-conversion-using-python
+    command = [
+        "soffice",
+        "--headless",
+        "--convert-to",
+        target_format,
+        "--outdir",
+        output_directory,
+        input_filename,
+    ]
     try:
-        subprocess.call(
-            [
-                "soffice",
-                "--headless",
-                "--convert-to",
-                target_format,
-                "--outdir",
-                output_directory,
-                input_filename,
-            ],
+        process = subprocess.Popen(
+            command,
+            stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE,
         )
+        output, error = process.communicate()
     except FileNotFoundError:
         raise FileNotFoundError(
             """soffice command was not found. Please install libreoffice
 on your system and try again.
 
 - Install instructions: https://www.libreoffice.org/get-help/install-howto/
 - Mac: https://formulae.brew.sh/cask/libreoffice
 - Debian: https://wiki.debian.org/LibreOffice""",
         )
 
+    logger.info(output.decode().strip())
+    if error:
+        logger.error(error.decode().strip())
+
 
 def exactly_one(**kwargs) -> None:
     """
     Verify arguments; exactly one of all keyword arguments must not be None.
 
     Example:
         >>> exactly_one(filename=filename, file=file, text=text, url=url)
```

### Comparing `unstructured-0.7.2/unstructured/partition/csv.py` & `unstructured-0.7.3/unstructured/partition/csv.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/partition/doc.py` & `unstructured-0.7.3/unstructured/partition/doc.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/partition/docx.py` & `unstructured-0.7.3/unstructured/partition/docx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/partition/email.py` & `unstructured-0.7.3/unstructured/partition/email.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/partition/epub.py` & `unstructured-0.7.3/unstructured/partition/epub.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/partition/html.py` & `unstructured-0.7.3/unstructured/partition/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/partition/image.py` & `unstructured-0.7.3/unstructured/partition/image.py`

 * *Files 20% similar despite different names*

```diff
@@ -31,18 +31,20 @@
         be used.
     token
         A string defining the authentication token for a self-host url, if applicable.
     ocr_languages
         The languages to use for the Tesseract agent. To use a language, you'll first need
         to install the appropriate Tesseract language pack.
     strategy
-        The strategy to use for partitioning the PDF. Valid strategies are "hi_res" and
+        The strategy to use for partitioning the image. Valid strategies are "hi_res" and
         "ocr_only". When using the "hi_res" strategy, the function uses a layout detection
         model if to identify document elements. When using the "ocr_only" strategy,
         partition_image simply extracts the text from the document using OCR and processes it.
+        The default strategy `auto` will determine when a image can be extracted using
+        `ocr_only` mode, otherwise it will fall back to `hi_res`.
     """
     exactly_one(filename=filename, file=file)
 
     if template is None:
         template = "layout/image"
 
     return partition_pdf_or_image(
```

### Comparing `unstructured-0.7.2/unstructured/partition/json.py` & `unstructured-0.7.3/unstructured/partition/json.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/partition/md.py` & `unstructured-0.7.3/unstructured/partition/md.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/partition/msg.py` & `unstructured-0.7.3/unstructured/partition/msg.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/partition/odt.py` & `unstructured-0.7.3/unstructured/partition/odt.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/partition/pdf.py` & `unstructured-0.7.3/unstructured/partition/pdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,17 +53,18 @@
         be used.
     token
         A string defining the authentication token for a self-host url, if applicable.
     strategy
         The strategy to use for partitioning the PDF. Valid strategies are "hi_res",
         "ocr_only", and "fast". When using the "hi_res" strategy, the function uses
         a layout detection model to identify document elements. When using the
-        "ocr_only" strategy, partition_image simply extracts the text from the
+        "ocr_only" strategy, partition_pdf simply extracts the text from the
         document using OCR and processes it. If the "fast" strategy is used, the text
-        is extracted directly from the PDF.
+        is extracted directly from the PDF. The default strategy `auto` will determine
+        when a page can be extracted using `fast` mode, otherwise it will fall back to `hi_res`.
     infer_table_structure
         Only applicable if `strategy=hi_res`.
         If True, any Table elements that are extracted will also have a metadata field
         named "text_as_html" where the table's text content is rendered into an html string.
         I.e., rows and cells are preserved.
         Whether True or False, the "text" field is always present in any Table element
         and is the text content of the table (no structure).
```

### Comparing `unstructured-0.7.2/unstructured/partition/ppt.py` & `unstructured-0.7.3/unstructured/partition/ppt.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/partition/pptx.py` & `unstructured-0.7.3/unstructured/partition/pptx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/partition/rtf.py` & `unstructured-0.7.3/unstructured/partition/rtf.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/partition/strategies.py` & `unstructured-0.7.3/unstructured/partition/strategies.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/partition/text.py` & `unstructured-0.7.3/unstructured/partition/text.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/partition/text_type.py` & `unstructured-0.7.3/unstructured/partition/text_type.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/partition/xlsx.py` & `unstructured-0.7.3/unstructured/partition/xlsx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/partition/xml.py` & `unstructured-0.7.3/unstructured/partition/xml.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/staging/argilla.py` & `unstructured-0.7.3/unstructured/staging/argilla.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/staging/base.py` & `unstructured-0.7.3/unstructured/staging/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/staging/baseplate.py` & `unstructured-0.7.3/unstructured/staging/baseplate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/staging/datasaur.py` & `unstructured-0.7.3/unstructured/staging/datasaur.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/staging/huggingface.py` & `unstructured-0.7.3/unstructured/staging/huggingface.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/staging/label_box.py` & `unstructured-0.7.3/unstructured/staging/label_box.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/staging/label_studio.py` & `unstructured-0.7.3/unstructured/staging/label_studio.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/staging/prodigy.py` & `unstructured-0.7.3/unstructured/staging/prodigy.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured/staging/weaviate.py` & `unstructured-0.7.3/unstructured/staging/weaviate.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,22 +49,25 @@
         },
         {
             "name": "category",
             "dataType": ["text"],
         },
     ]
 
+    exclude_metadata_keys = ["data_source"]
+
     for name, annotation in ElementMetadata.__annotations__.items():
-        data_type = _annotation_to_weaviate_data_type(annotation)
-        properties.append(
-            {
-                "name": name,
-                "dataType": data_type,
-            },
-        )
+        if name not in exclude_metadata_keys:
+            data_type = _annotation_to_weaviate_data_type(annotation)
+            properties.append(
+                {
+                    "name": name,
+                    "dataType": data_type,
+                },
+            )
 
     class_dict = {
         "class": class_name,
         "properties": properties,
     }
 
     return class_dict
```

### Comparing `unstructured-0.7.2/unstructured/utils.py` & `unstructured-0.7.3/unstructured/utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.2/unstructured.egg-info/PKG-INFO` & `unstructured-0.7.3/unstructured.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.7.2
+Version: 0.7.3
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.7.2 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.7.3 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
```

### Comparing `unstructured-0.7.2/unstructured.egg-info/SOURCES.txt` & `unstructured-0.7.3/unstructured.egg-info/SOURCES.txt`

 * *Files identical despite different names*

