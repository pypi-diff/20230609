# Comparing `tmp/metldata-0.1.0.tar.gz` & `tmp/metldata-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metldata-0.1.0.tar", last modified: Thu Apr 13 09:36:20 2023, max compression
+gzip compressed data, was "metldata-0.2.0.tar", last modified: Fri Jun  9 09:19:36 2023, max compression
```

## Comparing `metldata-0.1.0.tar` & `metldata-0.2.0.tar`

### file list

```diff
@@ -1,102 +1,187 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:36:20.820966 metldata-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-04-13 09:36:11.000000 metldata-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-04-13 09:36:20.820966 metldata-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-04-13 09:36:11.000000 metldata-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:36:20.812966 metldata-0.1.0/metldata/
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-13 09:36:11.000000 metldata-0.1.0/metldata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-13 09:36:11.000000 metldata-0.1.0/metldata/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:36:20.812966 metldata-0.1.0/metldata/accession_registry/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-13 09:36:11.000000 metldata-0.1.0/metldata/accession_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-04-13 09:36:11.000000 metldata-0.1.0/metldata/accession_registry/accession_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-04-13 09:36:11.000000 metldata-0.1.0/metldata/accession_registry/accession_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-13 09:36:11.000000 metldata-0.1.0/metldata/accession_registry/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:36:20.812966 metldata-0.1.0/metldata/builtin_transformations/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-13 09:36:11.000000 metldata-0.1.0/metldata/builtin_transformations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:36:20.812966 metldata-0.1.0/metldata/builtin_transformations/infer_references/
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-13 09:36:11.000000 metldata-0.1.0/metldata/builtin_transformations/infer_references/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-04-13 09:36:11.000000 metldata-0.1.0/metldata/builtin_transformations/infer_references/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-13 09:36:11.000000 metldata-0.1.0/metldata/builtin_transformations/infer_references/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-04-13 09:36:11.000000 metldata-0.1.0/metldata/builtin_transformations/infer_references/metadata_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-04-13 09:36:11.000000 metldata-0.1.0/metldata/builtin_transformations/infer_references/model_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:36:20.812966 metldata-0.1.0/metldata/builtin_transformations/infer_references/path/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-13 09:36:11.000000 metldata-0.1.0/metldata/builtin_transformations/infer_references/path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-04-13 09:36:11.000000 metldata-0.1.0/metldata/builtin_transformations/infer_references/path/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-13 09:36:11.000000 metldata-0.1.0/metldata/builtin_transformations/infer_references/path/path_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-04-13 09:36:11.000000 metldata-0.1.0/metldata/builtin_transformations/infer_references/path/path_str.py
--rw-r--r--   0 runner    (1001) docker     (123)     8788 2023-04-13 09:36:11.000000 metldata-0.1.0/metldata/builtin_transformations/infer_references/path/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-04-13 09:36:11.000000 metldata-0.1.0/metldata/builtin_transformations/infer_references/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-13 09:36:11.000000 metldata-0.1.0/metldata/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-13 09:36:11.000000 metldata-0.1.0/metldata/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-04-13 09:36:11.000000 metldata-0.1.0/metldata/metadata_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:36:20.816966 metldata-0.1.0/metldata/model_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-13 09:36:11.000000 metldata-0.1.0/metldata/model_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-04-13 09:36:11.000000 metldata-0.1.0/metldata/model_utils/anchors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-04-13 09:36:11.000000 metldata-0.1.0/metldata/model_utils/assumptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-13 09:36:11.000000 metldata-0.1.0/metldata/model_utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-04-13 09:36:11.000000 metldata-0.1.0/metldata/model_utils/essentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-13 09:36:11.000000 metldata-0.1.0/metldata/model_utils/identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-04-13 09:36:11.000000 metldata-0.1.0/metldata/model_utils/manipulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-13 09:36:11.000000 metldata-0.1.0/metldata/model_utils/metadata_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:36:20.816966 metldata-0.1.0/metldata/submission_registry/
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-13 09:36:11.000000 metldata-0.1.0/metldata/submission_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-13 09:36:11.000000 metldata-0.1.0/metldata/submission_registry/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-13 09:36:11.000000 metldata-0.1.0/metldata/submission_registry/event_publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-04-13 09:36:11.000000 metldata-0.1.0/metldata/submission_registry/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-04-13 09:36:11.000000 metldata-0.1.0/metldata/submission_registry/submission_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-04-13 09:36:11.000000 metldata-0.1.0/metldata/submission_registry/submission_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-13 09:36:11.000000 metldata-0.1.0/metldata/submission_registry/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:36:20.816966 metldata-0.1.0/metldata/transform/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-13 09:36:11.000000 metldata-0.1.0/metldata/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-04-13 09:36:11.000000 metldata-0.1.0/metldata/transform/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-04-13 09:36:11.000000 metldata-0.1.0/metldata/transform/handling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:36:20.812966 metldata-0.1.0/metldata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-04-13 09:36:20.000000 metldata-0.1.0/metldata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-13 09:36:20.000000 metldata-0.1.0/metldata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 09:36:20.000000 metldata-0.1.0/metldata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-13 09:36:20.000000 metldata-0.1.0/metldata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 09:36:20.000000 metldata-0.1.0/metldata.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-13 09:36:20.000000 metldata-0.1.0/metldata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-13 09:36:20.000000 metldata-0.1.0/metldata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-13 09:36:20.820966 metldata-0.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-04-13 09:36:11.000000 metldata-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:36:20.816966 metldata-0.1.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:36:20.816966 metldata-0.1.0/tests/accession_registry/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-13 09:36:11.000000 metldata-0.1.0/tests/accession_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-13 09:36:11.000000 metldata-0.1.0/tests/accession_registry/test_accession_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-13 09:36:11.000000 metldata-0.1.0/tests/accession_registry/test_accession_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:36:20.816966 metldata-0.1.0/tests/builtin_tranformations/
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-13 09:36:11.000000 metldata-0.1.0/tests/builtin_tranformations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:36:20.816966 metldata-0.1.0/tests/builtin_tranformations/infer_references/
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-13 09:36:11.000000 metldata-0.1.0/tests/builtin_tranformations/infer_references/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:36:20.816966 metldata-0.1.0/tests/builtin_tranformations/infer_references/path/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-13 09:36:11.000000 metldata-0.1.0/tests/builtin_tranformations/infer_references/path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-13 09:36:11.000000 metldata-0.1.0/tests/builtin_tranformations/infer_references/path/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-04-13 09:36:11.000000 metldata-0.1.0/tests/builtin_tranformations/infer_references/path/test_path.py
--rw-r--r--   0 runner    (1001) docker     (123)    10545 2023-04-13 09:36:11.000000 metldata-0.1.0/tests/builtin_tranformations/infer_references/path/test_path_str.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-04-13 09:36:11.000000 metldata-0.1.0/tests/builtin_tranformations/infer_references/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:36:20.820966 metldata-0.1.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-13 09:36:11.000000 metldata-0.1.0/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-13 09:36:11.000000 metldata-0.1.0/tests/fixtures/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-13 09:36:11.000000 metldata-0.1.0/tests/fixtures/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-13 09:36:11.000000 metldata-0.1.0/tests/fixtures/metadata_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-13 09:36:11.000000 metldata-0.1.0/tests/fixtures/transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-13 09:36:11.000000 metldata-0.1.0/tests/fixtures/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:36:20.820966 metldata-0.1.0/tests/model_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-13 09:36:11.000000 metldata-0.1.0/tests/model_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-04-13 09:36:11.000000 metldata-0.1.0/tests/model_utils/test_anchor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-13 09:36:11.000000 metldata-0.1.0/tests/model_utils/test_assumptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-13 09:36:11.000000 metldata-0.1.0/tests/model_utils/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-13 09:36:11.000000 metldata-0.1.0/tests/model_utils/test_essentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-13 09:36:11.000000 metldata-0.1.0/tests/model_utils/test_identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-04-13 09:36:11.000000 metldata-0.1.0/tests/model_utils/test_manipulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-13 09:36:11.000000 metldata-0.1.0/tests/model_utils/test_metadata_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:36:20.820966 metldata-0.1.0/tests/submission_registry/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-13 09:36:11.000000 metldata-0.1.0/tests/submission_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-13 09:36:11.000000 metldata-0.1.0/tests/submission_registry/test_event_publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-13 09:36:11.000000 metldata-0.1.0/tests/submission_registry/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6832 2023-04-13 09:36:11.000000 metldata-0.1.0/tests/submission_registry/test_submission_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-13 09:36:11.000000 metldata-0.1.0/tests/submission_registry/test_submission_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-04-13 09:36:11.000000 metldata-0.1.0/tests/test_metadata_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:36:20.820966 metldata-0.1.0/tests/transform/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-13 09:36:11.000000 metldata-0.1.0/tests/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-04-13 09:36:11.000000 metldata-0.1.0/tests/transform/test_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:19:36.777880 metldata-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-06-09 09:19:23.000000 metldata-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15169 2023-06-09 09:19:36.777880 metldata-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14473 2023-06-09 09:19:23.000000 metldata-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:19:36.745879 metldata-0.2.0/metldata/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:19:36.745879 metldata-0.2.0/metldata/accession_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/accession_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/accession_registry/accession_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/accession_registry/accession_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/accession_registry/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:19:36.745879 metldata-0.2.0/metldata/artifacts_rest/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/artifacts_rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/artifacts_rest/api_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/artifacts_rest/artifact_dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/artifacts_rest/artifact_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/artifacts_rest/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/artifacts_rest/load_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/artifacts_rest/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/artifacts_rest/query_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:19:36.749879 metldata-0.2.0/metldata/builtin_transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/builtin_transformations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:19:36.749879 metldata-0.2.0/metldata/builtin_transformations/add_accessions/
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/builtin_transformations/add_accessions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/builtin_transformations/add_accessions/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/builtin_transformations/add_accessions/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/builtin_transformations/add_accessions/metadata_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/builtin_transformations/add_accessions/model_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:19:36.749879 metldata-0.2.0/metldata/builtin_transformations/custom_embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/builtin_transformations/custom_embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/builtin_transformations/custom_embeddings/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/builtin_transformations/custom_embeddings/embedding_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/builtin_transformations/custom_embeddings/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/builtin_transformations/custom_embeddings/metadata_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/builtin_transformations/custom_embeddings/model_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:19:36.753879 metldata-0.2.0/metldata/builtin_transformations/delete_slots/
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/builtin_transformations/delete_slots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/builtin_transformations/delete_slots/assumptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/builtin_transformations/delete_slots/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/builtin_transformations/delete_slots/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/builtin_transformations/delete_slots/metadata_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/builtin_transformations/delete_slots/model_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:19:36.757879 metldata-0.2.0/metldata/builtin_transformations/infer_references/
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/builtin_transformations/infer_references/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/builtin_transformations/infer_references/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/builtin_transformations/infer_references/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/builtin_transformations/infer_references/metadata_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/builtin_transformations/infer_references/model_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:19:36.757879 metldata-0.2.0/metldata/builtin_transformations/infer_references/path/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/builtin_transformations/infer_references/path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/builtin_transformations/infer_references/path/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/builtin_transformations/infer_references/path/path_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/builtin_transformations/infer_references/path/path_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8736 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/builtin_transformations/infer_references/path/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/builtin_transformations/infer_references/reference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:19:36.761879 metldata-0.2.0/metldata/builtin_transformations/merge_slots/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/builtin_transformations/merge_slots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/builtin_transformations/merge_slots/assumptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/builtin_transformations/merge_slots/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/builtin_transformations/merge_slots/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/builtin_transformations/merge_slots/metadata_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/builtin_transformations/merge_slots/model_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/builtin_transformations/merge_slots/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:19:36.761879 metldata-0.2.0/metldata/builtin_workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/builtin_workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/builtin_workflows/ghga_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/custom_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:19:36.761879 metldata-0.2.0/metldata/event_handling/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/event_handling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/event_handling/artifact_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/event_handling/event_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/event_handling/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/event_handling/submission_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:19:36.765879 metldata-0.2.0/metldata/load/
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/load/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/load/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/load/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/load/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/load/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/load/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/load/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/load/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/metadata_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:19:36.769879 metldata-0.2.0/metldata/model_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/model_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/model_utils/anchors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/model_utils/assumptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/model_utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/model_utils/essentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/model_utils/identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/model_utils/manipulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/model_utils/metadata_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:19:36.769879 metldata-0.2.0/metldata/submission_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/submission_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/submission_registry/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/submission_registry/event_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/submission_registry/identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/submission_registry/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/submission_registry/submission_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/submission_registry/submission_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:19:36.769879 metldata-0.2.0/metldata/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/transform/artifact_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/transform/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/transform/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9449 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/transform/handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/transform/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-09 09:19:23.000000 metldata-0.2.0/metldata/transform/source_event_subscriber.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:19:36.745879 metldata-0.2.0/metldata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15169 2023-06-09 09:19:36.000000 metldata-0.2.0/metldata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-06-09 09:19:36.000000 metldata-0.2.0/metldata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 09:19:36.000000 metldata-0.2.0/metldata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-09 09:19:36.000000 metldata-0.2.0/metldata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 09:19:36.000000 metldata-0.2.0/metldata.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-09 09:19:36.000000 metldata-0.2.0/metldata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-09 09:19:36.000000 metldata-0.2.0/metldata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-09 09:19:36.777880 metldata-0.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-06-09 09:19:23.000000 metldata-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:19:36.769879 metldata-0.2.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:19:36.773880 metldata-0.2.0/tests/accession_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/accession_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/accession_registry/test_accession_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/accession_registry/test_accession_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:19:36.773880 metldata-0.2.0/tests/artifact_rest/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/artifact_rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/artifact_rest/test_api_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/artifact_rest/test_artifact_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/artifact_rest/test_load_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/artifact_rest/test_query_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:19:36.773880 metldata-0.2.0/tests/builtin_tranformations/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/builtin_tranformations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:19:36.773880 metldata-0.2.0/tests/builtin_tranformations/infer_references/
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/builtin_tranformations/infer_references/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:19:36.773880 metldata-0.2.0/tests/builtin_tranformations/infer_references/path/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/builtin_tranformations/infer_references/path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/builtin_tranformations/infer_references/path/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/builtin_tranformations/infer_references/path/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10233 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/builtin_tranformations/infer_references/path/test_path_str.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:19:36.773880 metldata-0.2.0/tests/builtin_tranformations/merge_slots/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/builtin_tranformations/merge_slots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/builtin_tranformations/merge_slots/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/builtin_tranformations/merge_slots/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/builtin_tranformations/test_happy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:19:36.773880 metldata-0.2.0/tests/builtin_workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/builtin_workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/builtin_workflows/test_happy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:19:36.773880 metldata-0.2.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/fixtures/artifact_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/fixtures/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/fixtures/event_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/fixtures/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/fixtures/metadata_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/fixtures/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/fixtures/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/fixtures/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:19:36.773880 metldata-0.2.0/tests/load/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/load/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/load/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:19:36.777880 metldata-0.2.0/tests/model_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/model_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/model_utils/test_anchor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/model_utils/test_assumptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/model_utils/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/model_utils/test_essentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/model_utils/test_identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/model_utils/test_manipulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/model_utils/test_metadata_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:19:36.777880 metldata-0.2.0/tests/submission_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/submission_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/submission_registry/test_event_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/submission_registry/test_identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/submission_registry/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/submission_registry/test_submission_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/submission_registry/test_submission_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/test_event_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/test_metadata_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:19:36.777880 metldata-0.2.0/tests/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/transform/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/transform/test_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-09 09:19:23.000000 metldata-0.2.0/tests/transform/test_main.py
```

### Comparing `metldata-0.1.0/LICENSE` & `metldata-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metldata-0.1.0/metldata/__init__.py` & `metldata-0.2.0/metldata/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Short description of package"""  # Please adapt to package
 
-__version__ = "0.1.0"
+__version__ = "0.2.0"
```

### Comparing `metldata-0.1.0/metldata/__main__.py` & `metldata-0.2.0/metldata/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Entrypoint of the package"""
 
+from metldata.cli import cli
+
 
 def run():
     """Run the service"""
-    ...
+    cli()
 
 
 if __name__ == "__main__":
     run()
```

### Comparing `metldata-0.1.0/metldata/accession_registry/__init__.py` & `metldata-0.2.0/metldata/builtin_transformations/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-"""Generates and persists accession numbers."""
+"""Built-in transformations"""
```

### Comparing `metldata-0.1.0/metldata/accession_registry/accession_handler.py` & `metldata-0.2.0/metldata/accession_registry/accession_registry.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from typing import Iterable
 
 from pydantic import BaseSettings, Field
 
 from metldata.accession_registry.accession_store import AccessionStore
 
 
-class AccessionHandlerConfig(BaseSettings):
+class AccessionRegistryConfig(BaseSettings):
     """Config parameters and their defaults."""
 
     prefix_mapping: dict[str, str] = Field(
         ...,
         description="Specifies the ID prefix (values) per resource type (keys).",
         example={
             "file": "GHGAF",
@@ -37,16 +37,16 @@
             "dataset": "GHGAD",
         },
     )
 
     suffix_length: int = Field(8, description="Length of the numeric ID suffix.")
 
 
-class AccessionHandler:
-    """Main class handling the accession handler."""
+class AccessionRegistry:
+    """Main class handling the accession registry."""
 
     class UnkownResourceTypeError(RuntimeError):
         """Raised when a resource type is specified that is unkown."""
 
         def __init__(self, *, specified_type: str, expected_types: Iterable[str]):
             """Specify the given as well as the expected resource types."""
 
@@ -57,15 +57,15 @@
             )
             super().__init__(message)
 
     class AccessionGenerationError(RuntimeError):
         """Raised when a the generation of a new accession failed."""
 
     def __init__(
-        self, *, config: AccessionHandlerConfig, accession_store: AccessionStore
+        self, *, config: AccessionRegistryConfig, accession_store: AccessionStore
     ):
         """Initialize with config."""
 
         self._config = config
         self._accession_store = accession_store
 
     def _assert_resource_type_exists(self, *, resource_type: str) -> None:
```

### Comparing `metldata-0.1.0/metldata/accession_registry/accession_store.py` & `metldata-0.2.0/metldata/accession_registry/accession_store.py`

 * *Files identical despite different names*

### Comparing `metldata-0.1.0/metldata/accession_registry/config.py` & `metldata-0.2.0/metldata/accession_registry/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,13 +11,13 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Config Parameter Modeling and Parsing"""
 
-from metldata.accession_registry.accession_handler import AccessionHandlerConfig
+from metldata.accession_registry.accession_registry import AccessionRegistryConfig
 from metldata.accession_registry.accession_store import AccessionStoreConfig
 
 
-class Config(AccessionHandlerConfig, AccessionStoreConfig):
+class Config(AccessionRegistryConfig, AccessionStoreConfig):
     """Config parameters and their defaults."""
```

### Comparing `metldata-0.1.0/metldata/builtin_transformations/__init__.py` & `metldata-0.2.0/metldata/builtin_workflows/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-"""Built-in transformations"""
+"""Built in transformation workflows."""
```

### Comparing `metldata-0.1.0/metldata/builtin_transformations/infer_references/__init__.py` & `metldata-0.2.0/metldata/builtin_transformations/infer_references/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,10 +16,10 @@
 
 """A transformation to infer references based on existing ones in the metadata model."""
 
 
 # shortcuts:
 # pylint: disable=unused-import
 from metldata.builtin_transformations.infer_references.main import (  # noqa: F401
+    REFERENCE_INFERENCE_TRANSFORMATION,
     ReferenceInferenceConfig,
-    reference_inference_transformation,
 )
```

### Comparing `metldata-0.1.0/metldata/builtin_transformations/infer_references/config.py` & `metldata-0.2.0/metldata/builtin_transformations/infer_references/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -36,26 +36,26 @@
             + " on existing references. On the first level keys refer to classes to"
             + " which inferred references should be added. On the second level, keys"
             + " refer to the names of the new slots of classes that hold the inferred"
             + " references. The values refer to the actual references details."
         ),
         example={
             "class_a": {
-                "has_class_d": {
-                    "path": "class_a(has_class_b)>class_b(has_class_d)>class_d",
+                "class_d": {
+                    "path": "class_a(class_b)>class_b(class_d)>class_d",
                     "multivalued": False,
                 },
-                "has_class_c": {
-                    "path": "class_a(has_class_b)>class_b<(has_class_c)class_c",
+                "class_c": {
+                    "path": "class_a(class_b)>class_b<(class_c)class_c",
                     "multivalued": True,
                 },
             },
             "class_b": {
-                "has_class_c": {
-                    "path": "class_b<(has_class_c)class_c",
+                "class_c": {
+                    "path": "class_b<(class_c)class_c",
                     "multivalued": True,
                 }
             },
         },
     )
 
     @property
@@ -74,7 +74,12 @@
                         path=reference_details.path,
                         new_slot=new_slot,
                         multivalued=reference_details.multivalued,
                     )
                 )
 
         return inferred_refs
+
+    class Config:
+        """Pydantic config."""
+
+        extra = "forbid"
```

### Comparing `metldata-0.1.0/metldata/builtin_transformations/infer_references/main.py` & `metldata-0.2.0/metldata/builtin_transformations/infer_references/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -21,36 +21,60 @@
 )
 from metldata.builtin_transformations.infer_references.metadata_transform import (
     add_references_to_metadata,
 )
 from metldata.builtin_transformations.infer_references.model_transform import (
     add_references_to_model,
 )
+from metldata.event_handling.models import SubmissionAnnotation
+from metldata.model_utils.anchors import get_anchors_points_by_target
 from metldata.model_utils.assumptions import check_basic_model_assumption
 from metldata.model_utils.essentials import MetadataModel
 from metldata.transform.base import Json, MetadataTransformer, TransformationDefinition
 
 
 class ReferenceInferenceMetadataTransformer(
     MetadataTransformer[ReferenceInferenceConfig]
 ):
-    """A transformer that infers references in metadata based on existing once."""
+    """A transformer that infers references in metadata based on existing ones."""
 
-    def transform(self, *, metadata: Json) -> Json:
+    def __init__(
+        self,
+        config: ReferenceInferenceConfig,
+        original_model: MetadataModel,
+        transformed_model: MetadataModel,
+    ):
+        """Initialize the transformer."""
+
+        super().__init__(
+            config=config,
+            original_model=original_model,
+            transformed_model=transformed_model,
+        )
+
+        self._anchor_points_by_target = get_anchors_points_by_target(
+            model=self._original_model
+        )
+
+    def transform(self, *, metadata: Json, annotation: SubmissionAnnotation) -> Json:
         """Transforms metadata.
 
+        Args:
+            metadata: The metadata to be transformed.
+            annotation: The annotation on the metadata.
+
         Raises:
             MetadataTransformationError:
                 if the transformation fails.
         """
 
         return add_references_to_metadata(
             metadata=metadata,
-            model=self._original_model,
             references=self._config.inferred_references,
+            anchor_points_by_target=self._anchor_points_by_target,
         )
 
 
 def check_model_assumptions(
     model: MetadataModel,
     config: ReferenceInferenceConfig,  # pylint: disable=unused-argument
 ) -> None:
@@ -76,13 +100,13 @@
 
     return add_references_to_model(
         model=model,
         references=config.inferred_references,
     )
 
 
-reference_inference_transformation = TransformationDefinition[ReferenceInferenceConfig](
-    config=ReferenceInferenceConfig,
+REFERENCE_INFERENCE_TRANSFORMATION = TransformationDefinition[ReferenceInferenceConfig](
+    config_cls=ReferenceInferenceConfig,
     check_model_assumptions=check_model_assumptions,
     transform_model=transform_model,
     metadata_transformer_factory=ReferenceInferenceMetadataTransformer,
 )
```

### Comparing `metldata-0.1.0/metldata/builtin_transformations/infer_references/metadata_transform.py` & `metldata-0.2.0/metldata/builtin_transformations/custom_embeddings/metadata_transform.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,190 +12,204 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """Logic for transforming metadata."""
 
+from typing import Union, cast
 
-from metldata.builtin_transformations.infer_references.path.resolve import (
-    resolve_reference_for_metadata_resource,
+from metldata.builtin_transformations.custom_embeddings.embedding_profile import (
+    EmbeddingProfile,
 )
-from metldata.builtin_transformations.infer_references.reference import (
-    InferredReference,
+from metldata.builtin_transformations.custom_embeddings.model_transform import (
+    get_embedding_profile_root_slot,
 )
 from metldata.metadata_utils import (
     MetadataResourceNotFoundError,
-    SelfIdLookUpError,
-    convert_list_to_inlined_dict,
+    get_resource_dict_of_class,
     lookup_resource_by_identifier,
-    lookup_self_id,
-)
-from metldata.model_utils.anchors import (
-    AnchorPoint,
-    AnchorPointNotFoundError,
-    get_anchors_points_by_target,
-    lookup_anchor_point,
+    upsert_resources_in_metadata,
 )
+from metldata.model_utils.anchors import AnchorPoint, lookup_anchor_point
 from metldata.model_utils.essentials import MetadataModel
-from metldata.transform.base import (
-    Json,
-    MetadataModelTransformationError,
-    MetadataTransformationError,
-)
+from metldata.transform.base import Json, MetadataTransformationError
+
+
+def is_slot_multivalued(
+    *, slot_name: str, class_name: str, model: MetadataModel
+) -> bool:
+    """Checks whether a slot is multivalued."""
 
+    slot_definition = model.schema_view.induced_slot(
+        slot_name=slot_name, class_name=class_name
+    )
+
+    if not slot_definition:
+        raise RuntimeError(  # this should never happen
+            f"Slot '{slot_name}' not found in class '{class_name}'"
+        )
 
-def add_reference_to_metadata_resource(
-    resource: Json,
+    return bool(slot_definition.multivalued)
+
+
+def resolve_target_resource(
+    target_resource_id: str,
+    target: Union[str, EmbeddingProfile],
     global_metadata: Json,
-    reference: InferredReference,
-    anchor_points_by_target: dict[str, AnchorPoint],
+    model: MetadataModel,
+    anchor_points_by_target: dict,
 ) -> Json:
-    """Add an inferred reference to an individual metadata resource.
-
-    Args:
-        resource: The metadata resource to modify.
-        global_metadata: The global metadata context to look up references in.
-        reference: The inferred reference.
-        anchor_points: The anchor points of the metadata model.
+    """Resolves a target resource.
 
     Raises:
-        MetadataTransformationError:
-            if the transformation of the metadata fails.
+        MetadataTransformationError: If the target resource could not be found.
     """
 
+    if isinstance(target, EmbeddingProfile):
+        return generate_embedded_resource(
+            resource_id=target_resource_id,
+            embedding_profile=target,
+            global_metadata=global_metadata,
+            model=model,
+            anchor_points_by_target=anchor_points_by_target,
+        )
+
     try:
-        target_anchor_point = lookup_anchor_point(
-            class_name=reference.target, anchor_points_by_target=anchor_points_by_target
+        return lookup_resource_by_identifier(
+            class_name=target,
+            identifier=target_resource_id,
+            global_metadata=global_metadata,
+            anchor_points_by_target=anchor_points_by_target,
         )
-    except AnchorPointNotFoundError as error:
-        raise MetadataModelTransformationError(
-            f"Cannot add reference '{reference}' to metadata resource '{resource}'"
-            + " because the target anchor point could not be found."
+    except MetadataResourceNotFoundError as error:
+        raise MetadataTransformationError(
+            f"Could not find resource '{target_resource_id}' of class '{target}'"
         ) from error
 
-    if reference.new_slot in resource:
-        raise MetadataModelTransformationError(
-            f"Cannot add reference '{reference}' to metadata resource '{resource}'"
-            + f" because the target slot '{reference.new_slot}' already exists."
-        )
 
-    target_resources = resolve_reference_for_metadata_resource(
-        resource=resource,
+def generate_embedded_resource(
+    resource_id: str,
+    embedding_profile: EmbeddingProfile,
+    global_metadata: Json,
+    model: MetadataModel,
+    anchor_points_by_target: dict,
+) -> Json:
+    """Generates an embedded version of the specified resource. This is done recursively
+    for all embedded references that are linked to this resource."""
+
+    resource = lookup_resource_by_identifier(
+        class_name=embedding_profile.source_class,
+        identifier=resource_id,
         global_metadata=global_metadata,
-        reference_path=reference.path,
         anchor_points_by_target=anchor_points_by_target,
     )
 
-    # get IDs of final target resources:
-    target_ids: set[str] = set()
-    for target_resource in target_resources:
-        try:
-            target_ids.add(
-                lookup_self_id(
-                    resource=target_resource,
-                    identifier_slot=target_anchor_point.identifier_slot,
+    for reference_slot_name, target in embedding_profile.embedded_references.items():
+        if is_slot_multivalued(
+            slot_name=reference_slot_name,
+            class_name=embedding_profile.source_class,
+            model=model,
+        ):
+            target_resource_ids = cast(list[str], resource[reference_slot_name])
+            target_resources = [
+                resolve_target_resource(
+                    target_resource_id=target_resource_id,
+                    target=target,
+                    global_metadata=global_metadata,
+                    model=model,
+                    anchor_points_by_target=anchor_points_by_target,
                 )
+                for target_resource_id in target_resource_ids
+            ]
+            resource[reference_slot_name] = target_resources
+        else:
+            target_resource_id = cast(str, resource[reference_slot_name])
+            target_resource = resolve_target_resource(
+                target_resource_id=target_resource_id,
+                target=target,
+                global_metadata=global_metadata,
+                model=model,
+                anchor_points_by_target=anchor_points_by_target,
             )
-        except SelfIdLookUpError as error:
-            raise MetadataTransformationError(
-                f"Cannot add reference '{reference}' to metadata resource '{resource}'"
-                + f" because the target resource '{target_resource}' does not have"
-                + f" an identifier in slot '{target_anchor_point.identifier_slot}'."
-            ) from error
-
-    # add the target IDs to the source resource:
-    resource_copy = resource.copy()
-    resource_copy[reference.new_slot] = sorted(target_ids)
+            resource[reference_slot_name] = target_resource
 
-    return resource_copy
+    return resource
 
 
-def add_reference_to_metadata(
+def add_custom_embedding_to_metadata(
     *,
     metadata: Json,
-    reference: InferredReference,
+    embedding_profile: EmbeddingProfile,
+    model: MetadataModel,
     anchor_points_by_target: dict[str, AnchorPoint],
 ) -> Json:
-    """Transform metadata by adding an inferred reference.
+    """Add custom embedding to the metadata.
 
     Raises:
-            MetadataTransformationError:
-                if the transformation of the metadata fails.
+        MetadataTransformationError:
+            if the transformation of the metadata fails.
     """
 
-    try:
-        source_anchor_point = lookup_anchor_point(
-            class_name=reference.source, anchor_points_by_target=anchor_points_by_target
-        )
-    except AnchorPointNotFoundError as error:
-        raise MetadataTransformationError(
-            f"Cannot add reference '{reference}' to metadata because the source anchor"
-            + " point could not be found."
-        ) from error
-
-    source_ids = metadata.get(source_anchor_point.root_slot)
-
-    if not source_ids:
-        raise MetadataTransformationError(
-            f"Cannot add reference '{reference}' to metadata because the source anchor"
-            + f" point '{source_anchor_point.root_slot}' does not exist in the"
-            + " metadata."
-        )
-
-    try:
-        source_resources = [
-            lookup_resource_by_identifier(
-                class_name=reference.source,
-                global_metadata=metadata,
-                identifier=source_id,
-                anchor_points_by_target=anchor_points_by_target,
-            )
-            for source_id in source_ids
-        ]
-    except MetadataResourceNotFoundError as error:
-        raise MetadataTransformationError(
-            f"Cannot add reference '{reference}' to metadata because not all source"
-            + " resources could be found in the metadata."
-        ) from error
+    resource_ids = get_resource_dict_of_class(
+        class_name=embedding_profile.source_class,
+        global_metadata=metadata,
+        anchor_points_by_target=anchor_points_by_target,
+    ).keys()
 
-    modified_resources_as_list = [
-        add_reference_to_metadata_resource(
-            resource=source_resource,
+    resources = [
+        generate_embedded_resource(
+            resource_id=resource_id,
+            embedding_profile=embedding_profile,
             global_metadata=metadata,
-            reference=reference,
+            model=model,
             anchor_points_by_target=anchor_points_by_target,
         )
-        for source_resource in source_resources
+        for resource_id in resource_ids
     ]
 
-    modified_resources_as_dict = convert_list_to_inlined_dict(
-        resources=modified_resources_as_list,
-        identifier_slot=source_anchor_point.identifier_slot,
+    # add anchor point for embedding profile:
+    source_class_anchor_point = lookup_anchor_point(
+        class_name=embedding_profile.source_class,
+        anchor_points_by_target=anchor_points_by_target,
+    )
+    embedded_class_anchor_point = AnchorPoint(
+        target_class=embedding_profile.target_class,
+        identifier_slot=source_class_anchor_point.identifier_slot,
+        root_slot=get_embedding_profile_root_slot(embedding_profile=embedding_profile),
+    )
+    anchor_points_by_target_modified = anchor_points_by_target.copy()
+    anchor_points_by_target_modified[
+        embedding_profile.target_class
+    ] = embedded_class_anchor_point
+
+    return upsert_resources_in_metadata(
+        resources=resources,
+        class_name=embedding_profile.target_class,
+        global_metadata=metadata,
+        anchor_points_by_target=anchor_points_by_target_modified,
     )
-
-    metadata_copy = metadata.copy()
-    metadata_copy[source_anchor_point.root_slot] = modified_resources_as_dict
-
-    return metadata_copy
 
 
-def add_references_to_metadata(
-    *, metadata: Json, model: MetadataModel, references: list[InferredReference]
+def add_custom_embeddings_to_metadata(
+    *,
+    metadata: Json,
+    embedding_profiles: list[EmbeddingProfile],
+    model: MetadataModel,
+    anchor_points_by_target: dict[str, AnchorPoint],
 ) -> Json:
-    """Transform metadata and return the transformed one.
+    """Add custom embeddings to the metadata.
 
     Raises:
         MetadataTransformationError:
             if the transformation of the metadata fails.
     """
 
-    anchor_points_by_target = get_anchors_points_by_target(model=model)
-
-    for reference in references:
-        metadata = add_reference_to_metadata(
+    for embedding_profile in embedding_profiles:
+        metadata = add_custom_embedding_to_metadata(
             metadata=metadata,
-            reference=reference,
+            embedding_profile=embedding_profile,
+            model=model,
             anchor_points_by_target=anchor_points_by_target,
         )
 
     return metadata
```

### Comparing `metldata-0.1.0/metldata/builtin_transformations/infer_references/model_transform.py` & `metldata-0.2.0/metldata/builtin_transformations/infer_references/model_transform.py`

 * *Files identical despite different names*

### Comparing `metldata-0.1.0/metldata/builtin_transformations/infer_references/path/__init__.py` & `metldata-0.2.0/metldata/builtin_transformations/infer_references/path/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.1.0/metldata/builtin_transformations/infer_references/path/path.py` & `metldata-0.2.0/metldata/builtin_transformations/infer_references/path/path.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,36 +30,36 @@
     The reference path has two available representation. A string-based ("path_str"
     attribute) and an element-based ("elements" attribute) one.
 
     In the string-based representation ("path_string" attribute), the first and the last
     word correspond the name of the source and target class, respectively. ">" and "<"
     means indicate active (left class references the right one) and passive (the left
     class is referenced by the right one). Parentheses attached to these angles thereby
-    indicate the slot name of the referencing class. E.g. "class_a(has_class_b)>class_b"
-    means that the source class "class_a" has a slot "has_class_b" that references the
-    target class "class_b". Or "class_a<(has_class_a)class_b" means that the source
+    indicate the slot name of the referencing class. E.g. "class_a(class_b)>class_b"
+    means that the source class "class_a" has a slot "class_b" that references the
+    target class "class_b". Or "class_a<(class_a)class_b" means that the source
     class "class_a" is reference by the target class "class_b" via its slots
-    "has_class_a". Reference paths can also involve additional classes. E.g. a string of
-    "class_a<(has_class_a)class_b(has_class_c)>class_c" means that
+    "class_a". Reference paths can also involve additional classes. E.g. a string of
+    "class_a<(class_a)class_b(class_c)>class_c" means that
     a reference from the source class "class_a" to the target class "class_c" can be
     established via an additional class "class_b". Any inserted spaces or newlines will
     be ignored. So the following paths are equivalent:
-        - "class_a (has_class_b)> class_b"
+        - "class_a (class_b)> class_b"
         - "class_a
-            (has_class_b)>
+            (class_b)>
             class_b"
 
     A reference path consists of one or more elements. An element is a relationship
     between two classes. Reference paths that establish a direct relationship between
     source and target classes without the use of additional classes have only one
-    element (e.g. in string reprentations "class_a(has_class_b)>class_b" or
-    "class_a<(has_class_a)class_b"). More complex paths consist of multiple elements.
-    E.g. the path "class_a<(has_class_a)class_b(has_class_c)>class_c" can be decomposed
-    into the elements: "class_a<(has_class_a)class_b" and
-    "class_b(has_class_c)>class_c".
+    element (e.g. in string reprentations "class_a(class_b)>class_b" or
+    "class_a<(class_a)class_b"). More complex paths consist of multiple elements.
+    E.g. the path "class_a<(class_a)class_b(class_c)>class_c" can be decomposed
+    into the elements: "class_a<(class_a)class_b" and
+    "class_b(class_c)>class_c".
 
     The elements of a ReferencePath are stored in the "elements" attribute as a list
     of ReferencePathElement objects that are optimized for programmatic use.
 
     The "source" attribute provides the source class of the path while the
     "target" attribute provides the target class of the path.
     """
```

### Comparing `metldata-0.1.0/metldata/builtin_transformations/infer_references/path/path_elements.py` & `metldata-0.2.0/metldata/builtin_transformations/infer_references/path/path_elements.py`

 * *Files identical despite different names*

### Comparing `metldata-0.1.0/metldata/builtin_transformations/infer_references/path/path_str.py` & `metldata-0.2.0/metldata/builtin_transformations/infer_references/path/path_str.py`

 * *Files identical despite different names*

### Comparing `metldata-0.1.0/metldata/builtin_transformations/infer_references/path/resolve.py` & `metldata-0.2.0/metldata/builtin_transformations/infer_references/path/resolve.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,29 +131,33 @@
             identifier_slot=source_anchor_point.identifier_slot,
         )
     except SelfIdLookUpError as error:
         raise PathElementResolutionError(
             f"Cannot resolve path element: '{error}'"
         ) from error
 
-    target_resources_by_dict = global_metadata.get(target_anchor_point.root_slot)
-    if target_resources_by_dict is None:
+    target_resources = global_metadata.get(target_anchor_point.root_slot)
+    if target_resources is None:
         raise PathElementResolutionError(
             "Cannot resolve path element: No target resources found for"
             + f" root slot '{target_anchor_point.root_slot}'."
         )
 
     # lookup the target resources:
     target_ids_of_interest: set[str] = set()
-    for target_id, target_resource in target_resources_by_dict.items():
+    for target_resource in target_resources:
         referenced_source_ids = lookup_foreign_ids(
             resource=target_resource, slot=path_element.slot
         )
 
         if source_identifier in referenced_source_ids:
+            target_id = lookup_self_id(
+                resource=target_resource,
+                identifier_slot=target_anchor_point.identifier_slot,
+            )
             target_ids_of_interest.add(target_id)
 
     return target_ids_of_interest
 
 
 def resolve_path_element(
     *,
@@ -181,18 +185,15 @@
             source_resource=source_resource,
             path_element=path_element,
             global_metadata=global_metadata,
             anchor_points_by_target=anchor_points_by_target,
         )
 
     if not target_ids:
-        raise PathElementResolutionError(
-            f"Cannot resolve path element for source resource '{source_resource}'"
-            + " because no target resources were found."
-        )
+        return []
 
     target_resources: list[Json] = []
     for target_id in target_ids:
         try:
             target_resource = lookup_resource_by_identifier(
                 class_name=path_element.target,
                 identifier=target_id,
```

### Comparing `metldata-0.1.0/metldata/builtin_transformations/infer_references/reference.py` & `metldata-0.2.0/metldata/builtin_transformations/infer_references/reference.py`

 * *Files identical despite different names*

### Comparing `metldata-0.1.0/metldata/config.py` & `metldata-0.2.0/metldata/submission_registry/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,17 +11,19 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Config Parameter Modeling and Parsing"""
 
-from hexkit.config import config_from_yaml
-
-from metldata.accession_registry.config import Config as AccessionRegistryConfig
-from metldata.submission_registry.config import Config as SubmissionRegistryConfig
+from metldata.submission_registry.event_publisher import SourceEventPublisherConfig
+from metldata.submission_registry.submission_registry import SubmissionRegistryConfig
+from metldata.submission_registry.submission_store import SubmissionStoreConfig
 
 
 # pylint: disable=too-many-ancestors
-@config_from_yaml(prefix="metldata")
-class Config(AccessionRegistryConfig, SubmissionRegistryConfig):
+class Config(
+    SubmissionStoreConfig,
+    SubmissionRegistryConfig,
+    SourceEventPublisherConfig,
+):
     """Config parameters and their defaults."""
```

### Comparing `metldata-0.1.0/metldata/custom_types.py` & `metldata-0.2.0/tests/transform/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,12 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-"""A collection of custom types."""
-
-from typing import Any
-
-Json = dict[str, Any]
+"""Test the transform sub-package."""
```

### Comparing `metldata-0.1.0/metldata/model_utils/__init__.py` & `metldata-0.2.0/metldata/model_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.1.0/metldata/model_utils/anchors.py` & `metldata-0.2.0/metldata/model_utils/anchors.py`

 * *Files 18% similar despite different names*

```diff
@@ -31,14 +31,18 @@
     """Raised when an anchor point defined in a model is invalid."""
 
 
 class AnchorPointNotFoundError(RuntimeError):
     """Raised when no anchor point was found for a specific class."""
 
 
+class ClassNotAnchoredError(RuntimeError):
+    """Raised when a class is not anchored."""
+
+
 class AnchorPoint(BaseModel):
     """A model for describing an anchor point for the specified target class."""
 
     target_class: str = Field(..., description="The name of the class to be targeted.")
     identifier_slot: str = Field(
         ...,
         description=(
@@ -78,18 +82,18 @@
 
     if not slot.inlined:
         raise InvalidAnchorPointError(
             f"The inlined attribute for slot '{slot.name}' is set to False,"
             + " however, slots in the root class must be inlined."
         )
 
-    if slot.inlined_as_list:
+    if not slot.inlined_as_list:
         raise InvalidAnchorPointError(
-            f"The inlined_as_list attribute for slot '{slot.name}' is set to True,"
-            + " however, slots in the root class may not be inlined."
+            f"The inlined_as_list attribute for slot '{slot.name}' is set to False,"
+            + " however, slots in the root class must be inlined as list."
         )
 
     if not slot.required:
         raise InvalidAnchorPointError(
             f"The anchor point at the slot '{slot.name}' is not required."
         )
 
@@ -136,15 +140,15 @@
                 f"The class '{target_class}' has no identifier defined."
             )
 
         anchor_point.add(
             AnchorPoint(
                 target_class=target_class,
                 identifier_slot=identifier,
-                root_slot=root_slot.name,
+                root_slot=str(root_slot.name),
             )
         )
 
     return anchor_point
 
 
 def get_anchors_points_by_target(*, model: MetadataModel) -> dict[str, AnchorPoint]:
@@ -155,15 +159,19 @@
 
     return {anchor_point.target_class: anchor_point for anchor_point in anchor_points}
 
 
 def filter_anchor_points(
     *, anchor_points_by_target: dict[str, AnchorPoint], classes_of_interest: set[str]
 ) -> dict[str, AnchorPoint]:
-    """Filter the provided anchor points by a list of classes of interest."""
+    """Filter the provided anchor points by a list of classes of interest.
+
+    Raises:
+        AnchorPointNotFoundError: if no anchor point was found for a class of interest.
+    """
 
     # check if anchor points exists for all classes:
     classes_without_anchor_points = classes_of_interest.difference(
         anchor_points_by_target.keys()
     )
     if classes_without_anchor_points:
         raise AnchorPointNotFoundError(
@@ -187,7 +195,45 @@
 
     if anchor_point is None:
         raise AnchorPointNotFoundError(
             f"Cannot find anchor point class '{class_name}'."
         )
 
     return anchor_point
+
+
+def invert_anchor_points_by_target(
+    anchor_points_by_target: dict[str, AnchorPoint]
+) -> dict[str, str]:
+    """Convert the anchor points by target dict into an class by anchor point dict."""
+
+    return {
+        anchor_point.root_slot: class_name
+        for class_name, anchor_point in anchor_points_by_target.items()
+    }
+
+
+def get_target_by_anchor_point(*, model: MetadataModel) -> dict[str, str]:
+    """Get a mapping from the root slot where a class is anchored to the corresponding
+    class."""
+
+    anchor_points = get_anchor_points(model=model)
+
+    return {
+        anchor_point.root_slot: anchor_point.target_class
+        for anchor_point in anchor_points
+    }
+
+
+def lookup_class_by_anchor_point(
+    *, root_slot: str, target_by_anchor_point: dict[str, str]
+) -> str:
+    """Lookup the class for the given anchor point."""
+
+    class_name = target_by_anchor_point.get(root_slot)
+
+    if class_name is None:
+        raise ClassNotAnchoredError(
+            f"Cannot find class for anchor point with root slot '{root_slot}'."
+        )
+
+    return class_name
```

### Comparing `metldata-0.1.0/metldata/model_utils/assumptions.py` & `metldata-0.2.0/metldata/model_utils/assumptions.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,22 +11,73 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """Logic to check basic assumptions about the metadata model."""
-from metldata.model_utils.anchors import InvalidAnchorPointError, get_anchor_points
+from typing import Optional
+
+from metldata.model_utils.anchors import (
+    AnchorPointNotFoundError,
+    InvalidAnchorPointError,
+    filter_anchor_points,
+    get_anchors_points_by_target,
+)
 from metldata.model_utils.essentials import ROOT_CLASS, MetadataModel
 
 
 class MetadataModelAssumptionError(RuntimeError):
     """Raised when the assumptions about the metadata model are not met."""
 
 
+def check_class_exists(model: MetadataModel, class_name: str) -> None:
+    """Check that a class with the given name exists.
+
+    Raises:
+        MetadataModelAssumptionError: if validation fails.
+    """
+
+    # has a class called class_name:
+    class_ = model.schema_view.get_class(class_name=class_name)
+
+    if class_ is None:
+        raise MetadataModelAssumptionError(
+            f"A class called '{class_name}' is required but does not exist."
+        )
+
+
+def check_class_slot_exists(
+    model: MetadataModel, class_name: str, slot_name: str, ignore_parents: bool = False
+) -> None:
+    """Check that a class with the given name exists and that it has a slot with the
+    given name. If ignore_parents is set to True, slots that are inherited from parent
+    classes or mixins are ignored.
+
+    Raises:
+        MetadataModelAssumptionError: if validation fails.
+    """
+
+    check_class_exists(model=model, class_name=class_name)
+
+    all_slots = model.schema_view.class_slots(
+        class_name=class_name, direct=ignore_parents
+    )
+
+    if slot_name not in all_slots:
+        raise MetadataModelAssumptionError(
+            f"A slot called '{slot_name}' is required but does not exist"
+            + f" in the '{class_name}' class."
+            " Inherited slots are ignored."
+            if ignore_parents
+            else f"A slot called '{slot_name}' is required but does not exist"
+            + f" in the '{class_name}' class or its parents classes and mixins."
+        )
+
+
 def check_root_class_existence(model: MetadataModel) -> None:
     """Check the existence of a root class that is called as defined in ROOT_CLASS.
 
     Raises:
         MetadataModelAssumptionError: if validation fails.
     """
 
@@ -39,28 +90,42 @@
         )
     if not root_class.tree_root:
         raise MetadataModelAssumptionError(
             f"The {ROOT_CLASS} class must have the tree_root property set to true."
         )
 
 
-def check_anchor_points(model: MetadataModel) -> None:
-    """Checks the anchor points of the root class.
+def check_anchor_points(
+    model: MetadataModel, classes: Optional[list[str]] = None
+) -> None:
+    """Checks the anchor points of the root class. If classes is specified, also checks
+    that anchor points for the classes exist.
 
     Raises:
         MetadataModelAssumptionError: if validation fails.
     """
 
     try:
-        _ = get_anchor_points(model=model)
+        anchor_points_by_target = get_anchors_points_by_target(model=model)
     except InvalidAnchorPointError as error:
         raise MetadataModelAssumptionError(
             f"The model has invalid anchor points: {error}"
         ) from error
 
+    if classes is not None:
+        try:
+            _ = filter_anchor_points(
+                anchor_points_by_target=anchor_points_by_target,
+                classes_of_interest=set(classes),
+            )
+        except AnchorPointNotFoundError as error:
+            raise MetadataModelAssumptionError(
+                f"The model is missing anchor points: {error}"
+            ) from error
+
 
 def check_basic_model_assumption(model: MetadataModel) -> None:
     """Check that the basic assumptions that metldata makes about the metadata model
     are met. Raises a MetadataModelAssumptionError otherwise.
 
     Raises:
         MetadataModelAssumptionError: if validation fails.
```

### Comparing `metldata-0.1.0/metldata/model_utils/config.py` & `metldata-0.2.0/metldata/model_utils/config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.1.0/metldata/model_utils/essentials.py` & `metldata-0.2.0/metldata/model_utils/essentials.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,27 +17,36 @@
 """Basic constants and logic related to models."""
 
 from __future__ import annotations
 
 import dataclasses
 import json
 from contextlib import contextmanager
-from copy import deepcopy
+from copy import copy, deepcopy
+from functools import lru_cache
 from pathlib import Path
 from tempfile import NamedTemporaryFile
-from typing import Generator
+from typing import Any, Generator
 
+import jsonasobj2
 import yaml
 from linkml_runtime import SchemaView
 from linkml_runtime.linkml_model import SchemaDefinition
 
 # The name of the root class of a model:
 ROOT_CLASS = "Submission"
 
 
+@lru_cache
+def schema_view_from_model(model: MetadataModel) -> SchemaView:
+    """Get a schema view instance from the metadata model."""
+
+    return ExportableSchemaView(model)
+
+
 class MetadataModel(SchemaDefinition):
     """A dataclass for describing metadata models."""
 
     @classmethod
     def init_from_path(cls, model_path: Path) -> MetadataModel:
         """Initialize from a model file in yaml format."""
 
@@ -46,15 +55,15 @@
 
         return cls(**model_json)
 
     @property
     def schema_view(self) -> ExportableSchemaView:
         """Get a schema view instance from the metadata model."""
 
-        return ExportableSchemaView(self)
+        return schema_view_from_model(self)
 
     def copy(self) -> MetadataModel:
         """Copy the model."""
 
         return deepcopy(self)
 
     def __eq__(self, other: object):
@@ -74,15 +83,24 @@
 
         if essential:
             if "classes" in model_dict:
                 for class_ in model_dict["classes"].values():
                     if "from_schema" in class_:
                         del class_["from_schema"]
                     if "slot_usage" in class_:
-                        for slot in class_["slot_usage"].values():
+                        slot_usage: Any = (
+                            jsonasobj2.as_dict(class_["slot_usage"])
+                            if isinstance(class_["slot_usage"], jsonasobj2.JsonObj)
+                            else class_["slot_usage"]
+                        )
+                        for slot in slot_usage.values():
+                            if "alias" in slot:
+                                del slot["alias"]
+                            if "from_schema" in slot:
+                                del slot["from_schema"]
                             if "domain_of" in slot:
                                 del slot["domain_of"]
             if "slots" in model_dict:
                 for slot in model_dict["slots"].values():
                     if "from_schema" in slot:
                         del slot["from_schema"]
             if "enums" in model_dict:
@@ -128,13 +146,34 @@
 
         return hash(self.as_json())
 
 
 class ExportableSchemaView(SchemaView):
     """Extend the SchemaView by adding a method for exporting a MetadataModel."""
 
+    def __copy__(self):
+        """Return a copy of the model.
+
+        Please note, the copy will have a new uuid used for hashing.
+        """
+
+        return ExportableSchemaView(
+            schema=copy(self.schema),
+            importmap=copy(self.importmap),
+        )
+
+    def __deepcopy__(self, memo: Any):
+        """Return a deepcopy of the model.
+
+        Please note, the copy will have a new uuid used for hashing.
+        """
+
+        return ExportableSchemaView(
+            schema=deepcopy(self.schema), importmap=copy(self.importmap)
+        )
+
     def export_model(self) -> MetadataModel:
         """Export a MetadataModel."""
 
-        model_json = dataclasses.asdict(self.copy_schema())
+        model_json = dataclasses.asdict(deepcopy(self.schema))
 
         return MetadataModel(**model_json)
```

### Comparing `metldata-0.1.0/metldata/model_utils/identifiers.py` & `metldata-0.2.0/metldata/model_utils/identifiers.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,26 +17,45 @@
 """Handling identifiers of classes in a metadata model."""
 
 from typing import Optional
 
 from metldata.model_utils.essentials import ROOT_CLASS, MetadataModel
 
 
+def get_class_identifier(model: MetadataModel, class_name: str) -> Optional[str]:
+    """Get the identifier of a class in a metadata model.
+
+    Returns:
+        The identifier of the class, or None if the class does not have an identifier.
+    """
+
+    schema_view = model.schema_view
+
+    for slot_name in schema_view.class_slots(class_name=class_name):
+        slot_def = schema_view.induced_slot(slot_name=slot_name, class_name=class_name)
+        if slot_def.identifier:
+            return str(slot_def.name)
+
+    return None
+
+
 def get_class_identifiers(model: MetadataModel) -> dict[str, Optional[str]]:
     """Get the identifiers of all classes in a metadata model.
 
     Returns:
         A dictionary with the class names as keys and the identifiers as values. If a
         class does not have an identifier, the value is None.
     """
 
     schema_view = model.schema_view
 
     identifiers_by_class: dict[str, Optional[str]] = {}
     for class_name in schema_view.all_classes():
         if class_name == ROOT_CLASS:
             continue  # Root class does not have an identifier
-        identifier_slot_def = schema_view.get_identifier_slot(class_name)
-        identifier = identifier_slot_def.name if identifier_slot_def else None
+        class_def = schema_view.get_class(class_name=class_name)
+        if class_def.mixin or class_def.abstract:
+            continue  # Mixins and abstract classes do not have an identifier
+        identifier = get_class_identifier(model=model, class_name=class_name)
         identifiers_by_class[class_name] = identifier
 
     return identifiers_by_class
```

### Comparing `metldata-0.1.0/metldata/model_utils/metadata_validator.py` & `metldata-0.2.0/metldata/model_utils/metadata_validator.py`

 * *Files identical despite different names*

### Comparing `metldata-0.1.0/metldata/submission_registry/__init__.py` & `metldata-0.2.0/tests/builtin_tranformations/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,9 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-"""Manages submissions and acts as a source of truth for all derived transformations
-and artifacts."""
+"""Test the builtin_transformations sub-package."""
```

### Comparing `metldata-0.1.0/metldata/submission_registry/config.py` & `metldata-0.2.0/metldata/config.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,18 +11,29 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Config Parameter Modeling and Parsing"""
 
-from metldata.submission_registry.event_publisher import EventPublisherConfig
-from metldata.submission_registry.submission_registry import SubmissionRegistryConfig
-from metldata.submission_registry.submission_store import SubmissionStoreConfig
+from hexkit.config import config_from_yaml
 
+# pylint: disable=unused-import
+from metldata.accession_registry.config import Config as AccessionRegistryConfig
+from metldata.load.config import ArtifactLoaderAPIConfig as ArtifactLoaderAPIConfig_
+from metldata.load.config import ArtifactLoaderClientConfig  # noqa: F401
+from metldata.submission_registry.config import Config as SubmissionRegistryConfig
 
-class Config(
-    SubmissionStoreConfig,
-    SubmissionRegistryConfig,
-    EventPublisherConfig,
-):
+
+# pylint: disable=too-many-ancestors
+@config_from_yaml(prefix="metl_sub")
+class SubmissionConfig(AccessionRegistryConfig, SubmissionRegistryConfig):
+    """Config parameters and their defaults."""
+
+
+# Alias for the main config:
+Config = SubmissionConfig  # noqa: N806
+
+
+@config_from_yaml(prefix="metl_load")
+class ArtifactLoaderAPIConfig(ArtifactLoaderAPIConfig_):
     """Config parameters and their defaults."""
```

### Comparing `metldata-0.1.0/metldata/submission_registry/event_publisher.py` & `metldata-0.2.0/metldata/submission_registry/event_publisher.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,52 +12,46 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """Logic for the publication of source events."""
 
-from pathlib import Path
+import asyncio
+import json
 
-from pydantic import BaseSettings, Field
+from hexkit.protocols.eventpub import EventPublisherProtocol
 
+from metldata.event_handling.submission_events import SourceEventConfig
 from metldata.submission_registry import models
-from metldata.submission_registry.utils import save_submission_as_json
 
 
-class EventPublisherConfig(BaseSettings):
+class SourceEventPublisherConfig(SourceEventConfig):
     """Config parameters and their defaults."""
 
-    source_events_dir: Path = Field(
-        ..., description="The directory where source events will be stored as JSON."
-    )
 
-
-def get_source_event_path(*, submission_id: str, source_events_dir: Path) -> Path:
-    """Get the path for a source event."""
-
-    return source_events_dir / f"{submission_id}.json"
-
-
-class EventPublisher:
+class SourceEventPublisher:
     """Handles publication of source events."""
 
     def __init__(
-        self,
-        *,
-        config: EventPublisherConfig,
+        self, *, config: SourceEventPublisherConfig, provider: EventPublisherProtocol
     ):
         """Initialize with config parameters."""
 
         self._config = config
+        self._provider = provider
 
     def publish_submission(self, submission: models.Submission):
         """Publish the current submission as source event"""
 
         if submission.content is None:
             raise ValueError("Submission content must be defined.")
 
-        json_path = get_source_event_path(
-            submission_id=submission.id,
-            source_events_dir=self._config.source_events_dir,
+        payload = json.loads(submission.json())
+        asyncio.run(
+            self._provider.publish(
+                topic=self._config.source_event_topic,
+                type_=self._config.source_event_type,
+                key=submission.id,
+                payload=payload,
+            )
         )
-        save_submission_as_json(submission=submission, json_path=json_path)
```

### Comparing `metldata-0.1.0/metldata/submission_registry/models.py` & `metldata-0.2.0/tests/submission_registry/test_submission_store.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,78 +8,78 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-#
-
-"""Data models"""
-
-from enum import Enum
-from operator import attrgetter
-from typing import Any, Optional
-
-from ghga_service_chassis_lib.utils import DateTimeUTC, now_as_utc
-from pydantic import BaseModel, Field
-
-
-class SubmissionStatus(Enum):
-    """Statuses a submission may have."""
-
-    PENDING = "pending"
-    IN_REVIEW = "in-review"
-    CANCELED = "canceled"
-    COMPLETED = "completed"
-    DEPRECATED_PREPUBLICATION = "deprecated-prepublication"
-    EMPTIED_PREPUBLICATION = "emptyied-prepublication"
-    PUBLISHED = "published"
-    DEPRECATED_POSTPUBLICATION = "deprecated-postpublication"
-    HIDDEN_POSTPUBLICATION = "hidden-postpublication"
-    EMPTIED_POSTPUBLICATION = "emptied-postpublication"
-
 
-class StatusChange(BaseModel):
-    """A model for describing status changes of submissions."""
+"""Testing the submission store."""
 
-    timestamp: DateTimeUTC
-    new_status: SubmissionStatus
+import pytest
+from ghga_service_commons.utils.utc_dates import now_as_utc
 
-
-class SubmissionHeader(BaseModel):
-    """Basic information provided for a submission."""
-
-    title: str = Field(..., description="A descriptive title for this submission.")
-    description: Optional[str] = Field(None, description="An optional description.")
-
-
-class SubmissionCreation(SubmissionHeader):
-    """Essential data for creating a submission."""
-
-    content: Optional[dict[str, Any]] = Field(
-        None, description="The metadata content of the submission. "
+from metldata.config import SubmissionConfig
+from metldata.submission_registry.models import (
+    StatusChange,
+    Submission,
+    SubmissionStatus,
+)
+from metldata.submission_registry.submission_store import SubmissionStore
+from tests.fixtures.config import config_sub_fixture  # noqa: F401
+
+EXAMPLE_SUBMISSION = Submission(
+    title="test",
+    description="test",
+    content={"test_class": [{"alias": "test_alias1"}]},
+    accession_map={"test_class": {"test_alias1": "test_accession1"}},
+    id="testsubmission001",
+    status_history=(
+        StatusChange(
+            timestamp=now_as_utc(),
+            new_status=SubmissionStatus.COMPLETED,
+        ),
+    ),
+)
+
+
+def test_happy(config_sub_fixture: SubmissionConfig):  # noqa: F811
+    """Test the happy path of inserting, querying, and updating a submission using
+    the submission store."""
+
+    submission_store = SubmissionStore(config=config_sub_fixture)
+
+    # make sure that sumbission does not exist:
+    assert not submission_store.exists(submission_id=EXAMPLE_SUBMISSION.id)
+
+    # create new submission:
+    submission_store.insert_new(submission=EXAMPLE_SUBMISSION)
+
+    # make sure that sumbission exists:
+    assert submission_store.exists(submission_id=EXAMPLE_SUBMISSION.id)
+
+    # query newly created submission:
+    submission_queried = submission_store.get_by_id(submission_id=EXAMPLE_SUBMISSION.id)
+    assert EXAMPLE_SUBMISSION == submission_queried
+
+    # update the submision:
+    submission_updated = EXAMPLE_SUBMISSION.copy(
+        update={"title": "updated test submission"}
     )
+    submission_store.update_existing(submission=submission_updated)
 
-
-class Submission(SubmissionCreation):
-    """A model for describing a submission."""
-
-    id: str
-
-    status_history: list[StatusChange] = Field(
-        default_factory=lambda: [
-            StatusChange(timestamp=now_as_utc(), new_status=SubmissionStatus.PENDING)
-        ],
-        description="A history of status changes.",
+    # query updated submission:
+    submission_updated_queried = submission_store.get_by_id(
+        submission_id=submission_updated.id
     )
+    assert submission_updated_queried == submission_updated
 
-    @property
-    def current_status(self) -> SubmissionStatus:
-        """Extract the current submission status from the status history."""
 
-        if len(self.status_history) == 0:
-            raise RuntimeError("Status history is empty.")
+def test_query_non_existing(
+    config_sub_fixture: SubmissionConfig,  # noqa: F811
+):
+    """Test querying for a non-existing submission."""
 
-        sorted_history = sorted(self.status_history, key=attrgetter("timestamp"))
+    submission_store = SubmissionStore(config=config_sub_fixture)
 
-        return sorted_history[-1].new_status
+    with pytest.raises(SubmissionStore.SubmissionDoesNotExistError):
+        _ = submission_store.get_by_id(submission_id="non-exisitng-id")
```

### Comparing `metldata-0.1.0/metldata/submission_registry/submission_registry.py` & `metldata-0.2.0/metldata/submission_registry/submission_registry.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,22 +12,28 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """Logic for handling submissions."""
 
-from typing import Any
 
-from ghga_service_chassis_lib.utils import now_as_utc
+from ghga_service_commons.utils.utc_dates import now_as_utc
 
+from metldata.accession_registry.accession_registry import AccessionRegistry
+from metldata.custom_types import SubmissionContent
+from metldata.model_utils.anchors import get_anchors_points_by_target
 from metldata.model_utils.config import MetadataModelConfig
 from metldata.model_utils.metadata_validator import MetadataValidator
 from metldata.submission_registry import models
-from metldata.submission_registry.event_publisher import EventPublisher
+from metldata.submission_registry.event_publisher import SourceEventPublisher
+from metldata.submission_registry.identifiers import (
+    generate_accession_map,
+    generate_submission_id,
+)
 from metldata.submission_registry.submission_store import SubmissionStore
 
 
 class SubmissionRegistryConfig(MetadataModelConfig):
     """Config parameters and their defaults."""
 
 
@@ -61,21 +67,26 @@
             super().__init__(message)
 
     def __init__(
         self,
         *,
         config: SubmissionRegistryConfig,
         submission_store: SubmissionStore,
-        event_publisher: EventPublisher,
+        event_publisher: SourceEventPublisher,
+        accession_registry: AccessionRegistry,
     ):
         """Initialize with dependencies and config parameters."""
 
         self._submission_store = submission_store
         self._metadata_validator = MetadataValidator(model=config.metadata_model)
         self._event_publisher = event_publisher
+        self._accession_registry = accession_registry
+        self._anchor_points_by_target = get_anchors_points_by_target(
+            model=config.metadata_model
+        )
 
     def _get_submission_with_status(
         self, *, id_: str, expected_status: models.SubmissionStatus
     ) -> models.Submission:
         """Get details for a submission that is assumed to have the specified status.
 
         Raises:
@@ -95,33 +106,35 @@
                 expected_status=str(expected_status),
             )
 
         return submission
 
     def init_submission(self, *, header: models.SubmissionHeader) -> str:
         """Initialize a new submission by providing header information. Returns the
-        ID of the created submission."""
+        ID of the created submission. No source event is published, yet, since the
+        submission content is still empty."""
 
-        submission_creation = models.SubmissionCreation(**header.dict())
-        submission = self._submission_store.insert_new(submission=submission_creation)
+        id_ = generate_submission_id()
+        submission_creation = models.Submission(id=id_, **header.dict())
+        self._submission_store.insert_new(submission=submission_creation)
 
-        return submission.id
+        return id_
 
     def get_submission(self, *, id_: str) -> models.Submission:
         """Get details on the existing submission with the specified id.
 
         Raises:
             SubmissionRegistry.SubmissionDoesNotExistError:
                 when no submission with the specified ID exists.
         """
 
         return self._submission_store.get_by_id(id_)
 
     def upsert_submission_content(
-        self, *, submission_id: str, content: dict[str, Any]
+        self, *, submission_id: str, content: SubmissionContent
     ) -> None:
         """Insert or update the content of a pending submission.
         The metadata is validated against the model, persisted in the submission store,
         and finally published as source event.
 
         Raises:
             SubmissionRegistry.SubmissionDoesNotExistError:
@@ -129,25 +142,33 @@
             SubmissionRegistry.ValidationError:
                 when the provided content failed validation against the metadata model.
             SubmissionRegistry.StatusError:
                 when the status of the specified submission is not pending.
         """
 
         submission = self._get_submission_with_status(
-            id_=submission_id, expected_status=models.SubmissionStatus.PENDING
+            id_=submission_id,
+            expected_status=models.SubmissionStatus.PENDING,
         )
 
         # raises ValidationError if not valid:
         self._metadata_validator.validate(content)
 
-        # update the submission object in the store:
-        updated_submission = submission.copy(update={"content": content})
+        updated_accession_map = generate_accession_map(
+            content=content,
+            existing_accession_map=submission.accession_map,
+            accession_registry=self._accession_registry,
+            anchor_points_by_target=self._anchor_points_by_target,
+        )
+
+        updated_submission = submission.copy(
+            update={"content": content, "accession_map": updated_accession_map}
+        )
         self._submission_store.update_existing(submission=updated_submission)
 
-        # publish updated submission as source event:
         self._event_publisher.publish_submission(updated_submission)
 
     def complete_submission(self, *, id_: str) -> None:
         """Declare an existing submission as complete. The content of the submission
         cannot change anymore afterwards.
 
 
@@ -163,17 +184,16 @@
         submission = self._get_submission_with_status(
             id_=id_, expected_status=models.SubmissionStatus.PENDING
         )
 
         if submission.content is None:
             raise self.ContentEmptyError(submission_id=id_)
 
-        updated_submission = submission.copy()
-        updated_submission.status_history.append(
-            models.StatusChange(
-                timestamp=now_as_utc(), new_status=models.SubmissionStatus.COMPLETED
-            )
+        status_change = models.StatusChange(
+            timestamp=now_as_utc(), new_status=models.SubmissionStatus.COMPLETED
+        )
+        updated_submission = submission.copy(
+            update={"status_history": submission.status_history + (status_change,)}
         )
         self._submission_store.update_existing(submission=updated_submission)
 
-        # publish updated submission as source event:
         self._event_publisher.publish_submission(updated_submission)
```

### Comparing `metldata-0.1.0/metldata/submission_registry/utils.py` & `metldata-0.2.0/metldata/load/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,19 +10,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-"""Uility Collection"""
+"""Data models."""
 
-from pathlib import Path
+from typing_extensions import TypeAlias
 
-from metldata.submission_registry import models
+from metldata.custom_types import Json
 
-
-def save_submission_as_json(*, submission: models.Submission, json_path: Path) -> None:
-    """Save a submission as JSON."""
-
-    with open(json_path, "w", encoding="utf-8") as file:
-        file.write(submission.json(indent=4))
+# A dictionary of an artifact. The keys on the first correspond to artifact names.
+# The values are lists of resources for different submissions.
+ArtifactResourceDict: TypeAlias = dict[str, list[Json]]
```

### Comparing `metldata-0.1.0/metldata/transform/__init__.py` & `metldata-0.2.0/metldata/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.1.0/metldata/transform/base.py` & `metldata-0.2.0/metldata/builtin_transformations/delete_slots/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,90 +10,87 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-"""Models to describe transformations."""
+"""A tranformation for deleting slots from classes in a metadata model."""
 
-from abc import ABC, abstractmethod
-from dataclasses import dataclass
-from typing import Callable, Generic, TypeVar
-
-from pydantic import BaseModel, Field
-
-from metldata.custom_types import Json
-
-# shortcuts:
-# pylint: disable=unused-import
-from metldata.model_utils.assumptions import MetadataModelAssumptionError  # noqa: F401
+from metldata.builtin_transformations.delete_slots.assumptions import (
+    check_model_class_slots,
+)
+from metldata.builtin_transformations.delete_slots.config import SlotDeletionConfig
+from metldata.builtin_transformations.delete_slots.metadata_transform import (
+    delete_class_slots,
+)
+from metldata.builtin_transformations.delete_slots.model_transform import (
+    delete_class_slots_from_model,
+)
+from metldata.event_handling.models import SubmissionAnnotation
+from metldata.model_utils.anchors import get_anchors_points_by_target
+from metldata.model_utils.assumptions import check_anchor_points
 from metldata.model_utils.essentials import MetadataModel
+from metldata.transform.base import Json, MetadataTransformer, TransformationDefinition
 
 
-class MetadataModelTransformationError(RuntimeError):
-    """Raised when a transformation failed when applied to the metadata model."""
+def check_model_assumptions(model: MetadataModel, config: SlotDeletionConfig):
+    """Check that the classes and slots specified in the config exist in the model."""
 
+    check_model_class_slots(model=model, class_slots=config.slots_to_delete)
+    check_anchor_points(model=model, classes=list(config.slots_to_delete))
 
-class MetadataTransformationError(RuntimeError):
-    """Raised when a transformation failed when applied to metadata."""
 
+def transform_model(model: MetadataModel, config: SlotDeletionConfig) -> MetadataModel:
+    """Delete slots from classes in the model."""
 
-Config = TypeVar("Config", bound=BaseModel)
+    return delete_class_slots_from_model(
+        model=model, class_slots=config.slots_to_delete
+    )
 
 
-class MetadataTransformer(ABC, Generic[Config]):
-    """A base class for a metadata transformer."""
+class SlotDeletionMetadataTransformer(MetadataTransformer[SlotDeletionConfig]):
+    """Transformer for deleting slots from classes in a metadata model."""
 
     def __init__(
         self,
-        *,
-        config: Config,
+        config: SlotDeletionConfig,
         original_model: MetadataModel,
-        transformed_model: MetadataModel
+        transformed_model: MetadataModel,
     ):
-        """Initialize the transformer with config params, the original model, and the
-        transformed model."""
+        """Initialize the transformer."""
 
-        self._config = config
-        self._original_model = original_model
-        self._transformed_model = transformed_model
+        super().__init__(
+            config=config,
+            original_model=original_model,
+            transformed_model=transformed_model,
+        )
+
+        self._anchor_points_by_target = get_anchors_points_by_target(
+            model=self._original_model
+        )
 
-    @abstractmethod
-    def transform(self, *, metadata: Json) -> Json:
+    def transform(self, *, metadata: Json, annotation: SubmissionAnnotation) -> Json:
         """Transforms metadata.
 
+        Args:
+            metadata: The metadata to be transformed.
+            annotation: The annotation on the metadata.
+
         Raises:
             MetadataTransformationError:
                 if the transformation fails.
         """
-        ...
 
+        return delete_class_slots(
+            metadata=metadata,
+            slots_to_delete=self._config.slots_to_delete,
+            anchor_points_by_target=self._anchor_points_by_target,
+        )
 
-@dataclass(frozen=True)
-class TransformationDefinition(Generic[Config]):
-    """A model for describing a transformation."""
 
-    config: type[Config] = Field(
-        ..., description="The config model of the transformation."
-    )
-    check_model_assumptions: Callable[[MetadataModel, Config], None] = Field(
-        ...,
-        description=(
-            "A function that checks the assumptions made about the input model."
-            "Raises a MetadataModelAssumptionError if the assumptions are not met."
-        ),
-    )
-    transform_model: Callable[[MetadataModel, Config], MetadataModel] = Field(
-        ...,
-        description=(
-            "A function to transform the model. Raises a"
-            + " MetadataModelTransformationError if the transformation fails."
-        ),
-    )
-    metadata_transformer_factory: type[MetadataTransformer[Config]] = Field(
-        ...,
-        description=(
-            "A class for transforming metadata. Raises a MetadataTransformationError"
-            "if the transformation fails."
-        ),
-    )
+SLOT_DELETION_TRANSFORMATION = TransformationDefinition[SlotDeletionConfig](
+    config_cls=SlotDeletionConfig,
+    check_model_assumptions=check_model_assumptions,
+    transform_model=transform_model,
+    metadata_transformer_factory=SlotDeletionMetadataTransformer,
+)
```

### Comparing `metldata-0.1.0/setup.cfg` & `metldata-0.2.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 	Topic :: Scientific/Engineering :: Bio-Informatics
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = 
-	hexkit[mongodb]==0.9.2
-	ghga-service-chassis-lib==0.17.7
+	hexkit[mongodb]==0.9.3
+	ghga-service-commons[api,auth]==0.3.2
 	linkml-runtime==1.4.2
 	linkml-validator==0.4.5
 python_requires = >= 3.9
 
 [options.entry_points]
 console_scripts = 
 	metldata = metldata.__main__:run
```

### Comparing `metldata-0.1.0/setup.py` & `metldata-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `metldata-0.1.0/tests/accession_registry/__init__.py` & `metldata-0.2.0/tests/accession_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.1.0/tests/accession_registry/test_accession_handler.py` & `metldata-0.2.0/tests/accession_registry/test_accession_registry.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,38 +9,40 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Testing the accession handler."""
+"""Testing the accession registry."""
 
-from metldata.accession_registry.accession_handler import AccessionHandler
+from metldata.accession_registry.accession_registry import AccessionRegistry
 from metldata.accession_registry.accession_store import AccessionStore
-from metldata.config import Config
-from tests.fixtures.config import config_fixture  # noqa: F401
+from metldata.config import SubmissionConfig
+from tests.fixtures.config import config_sub_fixture  # noqa: F401
 
 
-def test_get_accession_happy(config_fixture: Config):  # noqa: F811
+def test_get_accession_happy(
+    config_sub_fixture: SubmissionConfig,  # noqa: F811
+):
     """Test the happy path of getting 10 accession for each resource type."""
 
-    accession_store = AccessionStore(config=config_fixture)
-    accession_handler = AccessionHandler(
-        config=config_fixture, accession_store=accession_store
+    accession_store = AccessionStore(config=config_sub_fixture)
+    accession_registry = AccessionRegistry(
+        config=config_sub_fixture, accession_store=accession_store
     )
 
     accessions = []
-    for resource_type in config_fixture.prefix_mapping:
+    for resource_type in config_sub_fixture.prefix_mapping:
         for _ in range(10):
             # generate 10 accessions for each resource type
-            expected_prefix = config_fixture.prefix_mapping[resource_type]
-            expected_length = len(expected_prefix) + config_fixture.suffix_length
+            expected_prefix = config_sub_fixture.prefix_mapping[resource_type]
+            expected_length = len(expected_prefix) + config_sub_fixture.suffix_length
 
-            accession = accession_handler.get_accession(resource_type=resource_type)
+            accession = accession_registry.get_accession(resource_type=resource_type)
 
             assert accession.startswith(expected_prefix)
             assert len(accession) == expected_length
 
             accessions.append(accession)
 
     # check whether all theses accessions have been stored:
```

### Comparing `metldata-0.1.0/tests/accession_registry/test_accession_store.py` & `metldata-0.2.0/tests/accession_registry/test_accession_store.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,34 +12,38 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Testing the accession handler."""
 
 from metldata.accession_registry.accession_store import AccessionStore
-from metldata.config import Config
-from tests.fixtures.config import config_fixture  # noqa: F401
+from metldata.config import SubmissionConfig
+from tests.fixtures.config import config_sub_fixture  # noqa: F401
 
 
-def test_accession_store_happy(config_fixture: Config):  # noqa: F811
+def test_accession_store_happy(
+    config_sub_fixture: SubmissionConfig,  # noqa: F811
+):
     """Test accession store happy path."""
 
     expected_accessions = ["accession001", "accession002"]
 
-    accession_store = AccessionStore(config=config_fixture)
+    accession_store = AccessionStore(config=config_sub_fixture)
 
     # save accessions
     for expected_accession in expected_accessions:
         accession_store.save(accession=expected_accession)
 
     # check that the expected accessions exist:
     for expected_accession in expected_accessions:
         assert accession_store.exists(accession=expected_accession)
 
 
-def test_accession_store_unkown_accession(config_fixture: Config):  # noqa: F811
+def test_accession_store_unkown_accession(
+    config_sub_fixture: SubmissionConfig,  # noqa: F811
+):
     """Test accession store happy path."""
 
     unknown_accession = "accession003"
 
-    accession_store = AccessionStore(config=config_fixture)
+    accession_store = AccessionStore(config=config_sub_fixture)
     assert not accession_store.exists(accession=unknown_accession)
```

### Comparing `metldata-0.1.0/tests/builtin_tranformations/__init__.py` & `metldata-0.2.0/tests/builtin_tranformations/infer_references/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-"""Test the builtin_transformations sub-package."""
+"""Test the infer_references sub-package."""
```

### Comparing `metldata-0.1.0/tests/builtin_tranformations/infer_references/__init__.py` & `metldata-0.2.0/tests/artifact_rest/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-"""Test the infer_references sub-package."""
+"""Test the artifact_rest sub-package."""
```

### Comparing `metldata-0.1.0/tests/builtin_tranformations/infer_references/path/__init__.py` & `metldata-0.2.0/tests/builtin_tranformations/infer_references/path/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.1.0/tests/builtin_tranformations/infer_references/path/test_config.py` & `metldata-0.2.0/tests/builtin_tranformations/infer_references/path/test_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,54 +26,50 @@
 
 
 def test_config():
     """Test the ReferenceInferenceConfig class."""
 
     inferred_ref_map = {
         "class_a": {
-            "has_class_d": {
-                "path": "class_a(has_class_b)>class_b(has_class_d)>class_d",
+            "class_d": {
+                "path": "class_a(class_b)>class_b(class_d)>class_d",
                 "multivalued": False,
             },
-            "has_class_c": {
-                "path": "class_a(has_class_b)>class_b<(has_class_c)class_c",
+            "class_c": {
+                "path": "class_a(class_b)>class_b<(class_c)class_c",
                 "multivalued": True,
             },
         },
         "class_b": {
-            "has_class_c": {
-                "path": "class_b<(has_class_c)class_c",
+            "class_c": {
+                "path": "class_b<(class_c)class_c",
                 "multivalued": True,
             }
         },
     }
     expected_refs = [
         InferredReference(
             source="class_a",
             target="class_d",
-            path=ReferencePath(
-                path_str="class_a(has_class_b)>class_b(has_class_d)>class_d"
-            ),
-            new_slot="has_class_d",
+            path=ReferencePath(path_str="class_a(class_b)>class_b(class_d)>class_d"),
+            new_slot="class_d",
             multivalued=False,
         ),
         InferredReference(
             source="class_a",
             target="class_c",
-            path=ReferencePath(
-                path_str="class_a(has_class_b)>class_b<(has_class_c)class_c"
-            ),
-            new_slot="has_class_c",
+            path=ReferencePath(path_str="class_a(class_b)>class_b<(class_c)class_c"),
+            new_slot="class_c",
             multivalued=True,
         ),
         InferredReference(
             source="class_b",
             target="class_c",
-            path=ReferencePath(path_str="class_b<(has_class_c)class_c"),
-            new_slot="has_class_c",
+            path=ReferencePath(path_str="class_b<(class_c)class_c"),
+            new_slot="class_c",
             multivalued=True,
         ),
     ]
 
     config = ReferenceInferenceConfig(inferred_ref_map=inferred_ref_map)
     observed_refs = config.inferred_references
     assert expected_refs == observed_refs
```

### Comparing `metldata-0.1.0/tests/builtin_tranformations/infer_references/path/test_path.py` & `metldata-0.2.0/tests/builtin_tranformations/infer_references/path/test_path.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,86 +28,86 @@
 )
 
 
 @pytest.mark.parametrize(
     "path_str, expected_elements, expected_source, expected_target",
     [
         (
-            "class_a(has_class_b)>class_b",
+            "class_a(class_b)>class_b",
             [
                 ReferencePathElement(
                     type_=ReferencePathElementType.ACTIVE,
                     source="class_a",
-                    slot="has_class_b",
+                    slot="class_b",
                     target="class_b",
                 )
             ],
             "class_a",
             "class_b",
         ),
         (
             """class_a
-                (has_class_b) >
+                (class_b) >
                 class_b""",  # containing whitespaces
             [
                 ReferencePathElement(
                     type_=ReferencePathElementType.ACTIVE,
                     source="class_a",
-                    slot="has_class_b",
+                    slot="class_b",
                     target="class_b",
                 )
             ],
             "class_a",
             "class_b",
         ),
         (
-            "class_a<(has_class_a)class_b",
+            "class_a<(class_a)class_b",
             [
                 ReferencePathElement(
                     type_=ReferencePathElementType.PASSIVE,
                     source="class_a",
-                    slot="has_class_a",
+                    slot="class_a",
                     target="class_b",
                 )
             ],
             "class_a",
             "class_b",
         ),
         (
-            "class_a(has_class_b)>class_b(has_class_c)>class_c",
+            "class_a(class_b)>class_b(class_c)>class_c",
             [
                 ReferencePathElement(
                     type_=ReferencePathElementType.ACTIVE,
                     source="class_a",
-                    slot="has_class_b",
+                    slot="class_b",
                     target="class_b",
                 ),
                 ReferencePathElement(
                     type_=ReferencePathElementType.ACTIVE,
                     source="class_b",
-                    slot="has_class_c",
+                    slot="class_c",
                     target="class_c",
                 ),
             ],
             "class_a",
             "class_c",
         ),
         (
-            "class_a(has_class_b)>class_b<(has_class_b)class_c",
+            "class_a(class_b)>class_b<(class_b)class_c",
             [
                 ReferencePathElement(
                     type_=ReferencePathElementType.ACTIVE,
                     source="class_a",
-                    slot="has_class_b",
+                    slot="class_b",
                     target="class_b",
                 ),
                 ReferencePathElement(
                     type_=ReferencePathElementType.PASSIVE,
                     source="class_b",
-                    slot="has_class_b",
+                    slot="class_b",
                     target="class_c",
                 ),
             ],
             "class_a",
             "class_c",
         ),
     ],
@@ -125,20 +125,20 @@
     assert observed_path.source == expected_source
     assert observed_path.target == expected_target
 
 
 @pytest.mark.parametrize(
     "path_str, is_valid",
     [
-        ("class_a(has_class_b)>class_b", True),
-        ("class_a<(has_class_a)class_b", True),
-        ("class_a(has_class_b)>class_b(has_class_c)>class_c", True),
+        ("class_a(class_b)>class_b", True),
+        ("class_a<(class_a)class_b", True),
+        ("class_a(class_b)>class_b(class_c)>class_c", True),
         (12312, False),
-        ("class_a<(has_class_b)>class_b", False),
-        ("(has_class_b)>class_b(has_class_c)>class_c", False),
+        ("class_a<(class_b)>class_b", False),
+        ("(class_b)>class_b(class_c)>class_c", False),
     ],
 )
 def test_reference_path_pydantic(path_str: str, is_valid: bool):
     """Test the ReferencePath class when used with pydantic."""
 
     class ExampleModel(BaseModel):
         """Some example model."""
```

### Comparing `metldata-0.1.0/tests/builtin_tranformations/infer_references/path/test_path_str.py` & `metldata-0.2.0/tests/builtin_tranformations/infer_references/path/test_path_str.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,102 +40,102 @@
     validate_string_element,
 )
 
 
 @pytest.mark.parametrize(
     "path_str, is_valid",
     [
-        ("class_a(has_class_b)>class_b", True),
-        ("class_a<(has_class_a)class_b", True),
-        ("class_1(has_class_2)>class_2", True),
-        ("ClassA(has_class_b)>ClassB", True),
+        ("class_a(class_b)>class_b", True),
+        ("class_a<(class_a)class_b", True),
+        ("class_1(class_2)>class_2", True),
+        ("ClassA(class_b)>ClassB", True),
         ("class-a(has-class_b)>class-b", False),
-        ("class_a.has_class_b>class_b", False),
+        ("class_a.class_b>class_b", False),
     ],
 )
 def test_validate_path_str_characters(path_str: str, is_valid: bool):
     """Test the validate_path_str_characters method."""
 
     with nullcontext() if is_valid else pytest.raises(ValidationError):  # type: ignore
         validate_path_str_characters(path_str)
 
 
 @pytest.mark.parametrize(
     "path_str, is_valid",
     [
-        ("class_a(has_class_b)>class_b", True),
-        ("class_a<(has_class_a)class_b", True),
-        ("class_a(has_class_b)>class_b(has_class_c)>class_c", True),
-        ("class_a<(has_class_a)class_b(has_class_c)>class_c", True),
-        ("class_a<(has_class_a)class_b<(has_class_b)class_c", True),
+        ("class_a(class_b)>class_b", True),
+        ("class_a<(class_a)class_b", True),
+        ("class_a(class_b)>class_b(class_c)>class_c", True),
+        ("class_a<(class_a)class_b(class_c)>class_c", True),
+        ("class_a<(class_a)class_b<(class_b)class_c", True),
         (
-            "class_a(has_class_b)>class_b(has_class_c)>class_c(has_class_d)>class_d",
+            "class_a(class_b)>class_b(class_c)>class_c(class_d)>class_d",
             True,
         ),
-        ("class_a<(has_class_b)>class_b", False),
+        ("class_a<(class_b)>class_b", False),
         ("class_a>class_b", False),
-        ("class_a>(has_class_a)class_b", False),
-        ("class_a(has_class_b)<class_b", False),
-        ("class_a(has_class_b)>class_b(has_class_c)>", False),
-        ("(has_class_b)>class_b(has_class_c)>class_c", False),
-        ("class_a(has_class_b>class_b", False),
+        ("class_a>(class_a)class_b", False),
+        ("class_a(class_b)<class_b", False),
+        ("class_a(class_b)>class_b(class_c)>", False),
+        ("(class_b)>class_b(class_c)>class_c", False),
+        ("class_a(class_b>class_b", False),
     ],
 )
 def test_validate_path_str_format(path_str: str, is_valid: bool):
     """Test the validate_path_str_format method."""
 
     with nullcontext() if is_valid else pytest.raises(ValidationError):  # type: ignore
         validate_path_str_format(path_str)
 
 
 @pytest.mark.parametrize(
     "path_str, expected_first_element",
     [
-        ("class_a(has_class_b)>class_b", "class_a(has_class_b)>class_b"),
-        ("class_a<(has_class_a)class_b", "class_a<(has_class_a)class_b"),
+        ("class_a(class_b)>class_b", "class_a(class_b)>class_b"),
+        ("class_a<(class_a)class_b", "class_a<(class_a)class_b"),
         (
-            "class_a(has_class_b)>class_b(has_class_c)>class_c",
-            "class_a(has_class_b)>class_b",
+            "class_a(class_b)>class_b(class_c)>class_c",
+            "class_a(class_b)>class_b",
         ),
     ],
 )
 def test_extract_first_element(path_str: str, expected_first_element: str):
     """Test the extract_first_element method."""
 
     observed_first_element = extract_first_element(path_str=path_str)
     assert observed_first_element == expected_first_element
 
 
 @pytest.mark.parametrize(
     "path_str, expected_target_class",
     [
-        ("class_a(has_class_b)>class_b", "class_b"),
-        ("class_a<(has_class_a)class_b", "class_b"),
+        ("class_a(class_b)>class_b", "class_b"),
+        ("class_a<(class_a)class_b", "class_b"),
         (
-            "class_a(has_class_b)>class_b(has_class_c)>class_c",
+            "class_a(class_b)>class_b(class_c)>class_c",
             "class_c",
         ),
     ],
 )
 def test_get_target_class(path_str: str, expected_target_class: str):
     """Test the get_target_class method."""
 
     observed_target_class = get_target_class(path_str=path_str)
     assert observed_target_class == expected_target_class
 
 
 @pytest.mark.parametrize(
     "path_str, expected_first_element, expected_remaining_path",
     [
-        ("class_a(has_class_b)>class_b", "class_a(has_class_b)>class_b", None),
-        ("class_a<(has_class_a)class_b", "class_a<(has_class_a)class_b", None),
+        ("class_a(class_b)>class_b", "class_a(class_b)>class_b", None),
+        ("class_a<(class_a)class_b", "class_a<(class_a)class_b", None),
         (
-            "class_a(has_class_b)>class_b(has_class_c)>class_c",
-            "class_a(has_class_b)>class_b",
-            "class_b(has_class_c)>class_c",
+            "class_a(class_b)>class_b(class_c)>class_c",
+            "class_a(class_b)>class_b",
+            "class_b(class_c)>class_c",
         ),
     ],
 )
 def test_split_first_element(
     path_str: str, expected_first_element: str, expected_remaining_path: Optional[str]
 ):
     """Test the split_first_element method."""
@@ -146,68 +146,68 @@
     assert observed_first_element == expected_first_element
     assert observed_remaining_path == expected_remaining_path
 
 
 @pytest.mark.parametrize(
     "path_str, expected_elements",
     [
-        ("class_a(has_class_b)>class_b", ["class_a(has_class_b)>class_b"]),
-        ("class_a<(has_class_a)class_b", ["class_a<(has_class_a)class_b"]),
+        ("class_a(class_b)>class_b", ["class_a(class_b)>class_b"]),
+        ("class_a<(class_a)class_b", ["class_a<(class_a)class_b"]),
         (
-            "class_a(has_class_b)>class_b(has_class_c)>class_c",
+            "class_a(class_b)>class_b(class_c)>class_c",
             [
-                "class_a(has_class_b)>class_b",
-                "class_b(has_class_c)>class_c",
+                "class_a(class_b)>class_b",
+                "class_b(class_c)>class_c",
             ],
         ),
     ],
 )
 def test_get_string_elements(path_str: str, expected_elements: list[str]):
     """Test the get_string_elements method."""
 
     observed_elements = get_string_elements(path_str=path_str)
     assert observed_elements == expected_elements
 
 
 @pytest.mark.parametrize(
     "string_element, is_valid",
     [
-        ("class_a(has_class_b)>class_b", True),
-        ("class_a<(has_class_a)class_b", True),
-        ("class_a<(has_class_a)>class_b", False),
+        ("class_a(class_b)>class_b", True),
+        ("class_a<(class_a)class_b", True),
+        ("class_a<(class_a)>class_b", False),
         ("class_a>class_b", False),
-        ("class_a(has_class_b)>class_b(has_class_c)>class_c", False),
+        ("class_a(class_b)>class_b(class_c)>class_c", False),
     ],
 )
 def test_validate_string_element(string_element: str, is_valid: bool):
     """Test the validate_string_element method."""
 
     with nullcontext() if is_valid else pytest.raises(ValidationError):  # type: ignore
         validate_string_element(string_element)
 
 
 @pytest.mark.parametrize(
     "string_element, expected_type",
     [
-        ("class_a(has_class_b)>class_b", ReferencePathElementType.ACTIVE),
-        ("class_a<(has_class_a)class_b", ReferencePathElementType.PASSIVE),
+        ("class_a(class_b)>class_b", ReferencePathElementType.ACTIVE),
+        ("class_a<(class_a)class_b", ReferencePathElementType.PASSIVE),
     ],
 )
 def test_get_element_type(string_element: str, expected_type: ReferencePathElementType):
     """Test the get_element_type method."""
 
     observed_type = get_element_type(string_element=string_element)
     assert observed_type == expected_type
 
 
 @pytest.mark.parametrize(
     "string_element, expected_source, expected_slot, expected_target",
     [
-        ("class_a(has_class_b)>class_b", "class_a", "has_class_b", "class_b"),
-        ("class_a<(has_class_a)class_b", "class_a", "has_class_a", "class_b"),
+        ("class_a(class_b)>class_b", "class_a", "class_b", "class_b"),
+        ("class_a<(class_a)class_b", "class_a", "class_a", "class_b"),
     ],
 )
 def test_get_element_components(
     string_element: str, expected_source: str, expected_slot: str, expected_target: str
 ):
     """Test the get_element_components method."""
 
@@ -219,28 +219,28 @@
     assert observed_target == expected_target
 
 
 @pytest.mark.parametrize(
     "string_element, expected_object",
     [
         (
-            "class_a(has_class_b)>class_b",
+            "class_a(class_b)>class_b",
             ReferencePathElement(
                 type_=ReferencePathElementType.ACTIVE,
                 source="class_a",
-                slot="has_class_b",
+                slot="class_b",
                 target="class_b",
             ),
         ),
         (
-            "class_a<(has_class_a)class_b",
+            "class_a<(class_a)class_b",
             ReferencePathElement(
                 type_=ReferencePathElementType.PASSIVE,
                 source="class_a",
-                slot="has_class_a",
+                slot="class_a",
                 target="class_b",
             ),
         ),
     ],
 )
 def test_string_element_to_object(
     string_element: str, expected_object: ReferencePathElement
@@ -251,65 +251,65 @@
     assert observed_object == expected_object
 
 
 @pytest.mark.parametrize(
     "path_str, expected_elements",
     [
         (
-            "class_a(has_class_b)>class_b",
+            "class_a(class_b)>class_b",
             [
                 ReferencePathElement(
                     type_=ReferencePathElementType.ACTIVE,
                     source="class_a",
-                    slot="has_class_b",
+                    slot="class_b",
                     target="class_b",
                 )
             ],
         ),
         (
-            "class_a<(has_class_a)class_b",
+            "class_a<(class_a)class_b",
             [
                 ReferencePathElement(
                     type_=ReferencePathElementType.PASSIVE,
                     source="class_a",
-                    slot="has_class_a",
+                    slot="class_a",
                     target="class_b",
                 )
             ],
         ),
         (
-            "class_a(has_class_b)>class_b(has_class_c)>class_c",
+            "class_a(class_b)>class_b(class_c)>class_c",
             [
                 ReferencePathElement(
                     type_=ReferencePathElementType.ACTIVE,
                     source="class_a",
-                    slot="has_class_b",
+                    slot="class_b",
                     target="class_b",
                 ),
                 ReferencePathElement(
                     type_=ReferencePathElementType.ACTIVE,
                     source="class_b",
-                    slot="has_class_c",
+                    slot="class_c",
                     target="class_c",
                 ),
             ],
         ),
         (
-            "class_a(has_class_b)>class_b<(has_class_b)class_c",
+            "class_a(class_b)>class_b<(class_b)class_c",
             [
                 ReferencePathElement(
                     type_=ReferencePathElementType.ACTIVE,
                     source="class_a",
-                    slot="has_class_b",
+                    slot="class_b",
                     target="class_b",
                 ),
                 ReferencePathElement(
                     type_=ReferencePathElementType.PASSIVE,
                     source="class_b",
-                    slot="has_class_b",
+                    slot="class_b",
                     target="class_c",
                 ),
             ],
         ),
     ],
 )
 def test_path_str_to_object_elements(
```

### Comparing `metldata-0.1.0/tests/fixtures/__init__.py` & `metldata-0.2.0/tests/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.1.0/tests/fixtures/config.py` & `metldata-0.2.0/tests/fixtures/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,32 +15,30 @@
 #
 
 from tempfile import NamedTemporaryFile, TemporaryDirectory
 from typing import Generator
 
 import pytest
 
-from metldata.config import Config
+from metldata.config import SubmissionConfig
 from tests.fixtures.metadata_models import VALID_MINIMAL_MODEL_EXAMPLE_PATH
 
 PREFIX_MAPPING = {
-    "file": "GHGAF",
-    "experiment": "GHGAE",
-    "sample": "GHGAS",
-    "dataset": "GHGAD",
+    "File": "GHGAF",
+    "Experiment": "GHGAE",
+    "Sample": "GHGAS",
+    "Dataset": "GHGAD",
 }
 
 
 @pytest.fixture
-def config_fixture() -> Generator[Config, None, None]:
+def config_sub_fixture() -> Generator[SubmissionConfig, None, None]:
     """Generate a test config."""
 
     with TemporaryDirectory() as submission_store_dir:
-        with TemporaryDirectory() as source_events_dir:
-            with NamedTemporaryFile() as accession_store_path:
-                yield Config(
-                    metadata_model_path=VALID_MINIMAL_MODEL_EXAMPLE_PATH,
-                    submission_store_dir=submission_store_dir,
-                    source_events_dir=source_events_dir,
-                    accession_store_path=accession_store_path.name,
-                    prefix_mapping=PREFIX_MAPPING,
-                )
+        with NamedTemporaryFile() as accession_store_path:
+            yield SubmissionConfig(
+                metadata_model_path=VALID_MINIMAL_MODEL_EXAMPLE_PATH,
+                submission_store_dir=submission_store_dir,
+                accession_store_path=accession_store_path.name,
+                prefix_mapping=PREFIX_MAPPING,
+            )
```

### Comparing `metldata-0.1.0/tests/fixtures/metadata.py` & `metldata-0.2.0/tests/fixtures/metadata.py`

 * *Files identical despite different names*

### Comparing `metldata-0.1.0/tests/fixtures/metadata_models.py` & `metldata-0.2.0/tests/fixtures/metadata_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 
 def _get_example_model(name: str) -> MetadataModel:
     """Get example model."""
 
     return MetadataModel.init_from_path(EXAMPLE_MODEL_DIR / f"{name}.yaml")
 
 
-MINIMAL_VALID_METADATA_MODEL = _get_example_model("minimal_model")
-ADVANCED_VALID_METADATA_MODEL = _get_example_model("advanced_model")
-VALID_METADATA_MODELS = [MINIMAL_VALID_METADATA_MODEL, ADVANCED_VALID_METADATA_MODEL]
+VALID_MINIMAL_METADATA_MODEL = _get_example_model("minimal_model")
+VALID_ADVANCED_METADATA_MODEL = _get_example_model("advanced_model")
+VALID_METADATA_MODELS = [VALID_MINIMAL_METADATA_MODEL, VALID_ADVANCED_METADATA_MODEL]
 
 ROOT_CLASS_INVALID_MODELS = [
     _get_example_model(f"minimal_model_root_class_missing{idx}") for idx in range(1, 3)
 ]
 
 ANCHORS_INVALID_MODELS = [
     _get_example_model(f"minimal_model_anchors_invalid{idx}") for idx in range(1, 5)
```

### Comparing `metldata-0.1.0/tests/fixtures/transformations.py` & `metldata-0.2.0/metldata/builtin_transformations/merge_slots/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,85 +10,91 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-"""Transformation test cases."""
+"""A tranformation for merging multiple slots of a class into a single one."""
 
-from dataclasses import dataclass
-from pathlib import Path
-from typing import Generic, TypeVar
-
-import yaml
-from pydantic import BaseModel
-
-from metldata.builtin_transformations.infer_references import ReferenceInferenceConfig
-from metldata.custom_types import Json
+from metldata.builtin_transformations.merge_slots.assumptions import (
+    check_model_class_slots,
+)
+from metldata.builtin_transformations.merge_slots.config import SlotMergingConfig
+from metldata.builtin_transformations.merge_slots.metadata_transform import (
+    apply_merge_instructions_to_metadata,
+)
+from metldata.builtin_transformations.merge_slots.model_transform import (
+    merge_slots_in_model,
+)
+from metldata.event_handling.models import SubmissionAnnotation
+from metldata.model_utils.anchors import get_anchors_points_by_target
+from metldata.model_utils.assumptions import check_anchor_points
 from metldata.model_utils.essentials import MetadataModel
-from tests.fixtures.utils import BASE_DIR
+from metldata.transform.base import Json, MetadataTransformer, TransformationDefinition
 
-Config = TypeVar("Config", bound=BaseModel)
 
+def check_model_assumptions(model: MetadataModel, config: SlotMergingConfig):
+    """Check that the classes and slots specified in the config exist in the model."""
 
-@dataclass(frozen=True)
-class TransformationTestCase(Generic[Config]):
-    """A test case for a transformation."""
+    check_model_class_slots(model=model, merge_instructions=config.merge_instructions)
 
-    config: Config
-    original_model: MetadataModel
-    original_metadata: Json
-    transformed_model: MetadataModel
-    transformed_metadata: Json
+    classe_names = {
+        merge_instruction.class_name for merge_instruction in config.merge_instructions
+    }
+    check_anchor_points(model=model, classes=list(classe_names))
 
 
-def _read_yaml(path: Path) -> Json:
-    """Read a YAML file."""
+def transform_model(model: MetadataModel, config: SlotMergingConfig) -> MetadataModel:
+    """Merge slots of classes in the model."""
 
-    with open(path, "r", encoding="utf-8") as file:
-        return yaml.safe_load(file)
+    return merge_slots_in_model(
+        model=model, merge_instructions=config.merge_instructions
+    )
 
 
-def _read_test_case(
-    config_class: type[Config], transformation_name: str, case_name: str
-) -> TransformationTestCase[Config]:
-    """Read a test case for a transformation."""
+class SlotMergingMetadataTransformer(MetadataTransformer[SlotMergingConfig]):
+    """Transformer for merging slots of classes in a metadata model."""
 
-    case_dir = BASE_DIR / "transformations" / transformation_name / case_name
-    config_path = case_dir / "config.yaml"
-    original_model_path = case_dir / "original_model.yaml"
-    original_metadata_path = case_dir / "original_metadata.yaml"
-    transformed_model_path = case_dir / "transformed_model.yaml"
-    transformed_metadata_path = case_dir / "transformed_metadata.yaml"
+    def __init__(
+        self,
+        config: SlotMergingConfig,
+        original_model: MetadataModel,
+        transformed_model: MetadataModel,
+    ):
+        """Initialize the transformer."""
+
+        super().__init__(
+            config=config,
+            original_model=original_model,
+            transformed_model=transformed_model,
+        )
 
-    return TransformationTestCase(
-        config=config_class(**_read_yaml(config_path)),
-        original_model=MetadataModel.init_from_path(original_model_path),
-        original_metadata=_read_yaml(original_metadata_path),
-        transformed_model=MetadataModel.init_from_path(transformed_model_path),
-        transformed_metadata=_read_yaml(transformed_metadata_path),
-    )
+        self._anchor_points_by_target = get_anchors_points_by_target(
+            model=self._original_model
+        )
 
+    def transform(self, *, metadata: Json, annotation: SubmissionAnnotation) -> Json:
+        """Transforms metadata.
 
-def _read_all_test_cases(
-    config_class: type[Config], transformation_name: str
-) -> list[TransformationTestCase[Config]]:
-    """Read all test cases for a transformation."""
-
-    base_dir = BASE_DIR / "transformations" / transformation_name
-    case_names = [path.name for path in base_dir.iterdir() if path.is_dir()]
-
-    return [
-        _read_test_case(
-            config_class=config_class,
-            transformation_name=transformation_name,
-            case_name=case_name,
+        Args:
+            metadata: The metadata to be transformed.
+            annotation: The annotation on the metadata.
+
+        Raises:
+            MetadataTransformationError:
+                if the transformation fails.
+        """
+
+        return apply_merge_instructions_to_metadata(
+            metadata=metadata,
+            merge_instructions=self._config.merge_instructions,
+            anchor_points_by_target=self._anchor_points_by_target,
         )
-        for case_name in case_names
-    ]
 
 
-INFERRED_REFERENCE_TEST_CASES = _read_all_test_cases(
-    config_class=ReferenceInferenceConfig,
-    transformation_name="infer_references",
+SLOT_MERGING_TRANSFORMATION = TransformationDefinition[SlotMergingConfig](
+    config_cls=SlotMergingConfig,
+    check_model_assumptions=check_model_assumptions,
+    transform_model=transform_model,
+    metadata_transformer_factory=SlotMergingMetadataTransformer,
 )
```

### Comparing `metldata-0.1.0/tests/model_utils/__init__.py` & `metldata-0.2.0/tests/model_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.1.0/tests/model_utils/test_anchor.py` & `metldata-0.2.0/tests/model_utils/test_anchor.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,40 +27,38 @@
     get_anchor_points,
     get_anchors_points_by_target,
     lookup_anchor_point,
 )
 from metldata.model_utils.essentials import MetadataModel
 from tests.fixtures.metadata_models import (
     ANCHORS_INVALID_MODELS,
-    MINIMAL_VALID_METADATA_MODEL,
+    VALID_MINIMAL_METADATA_MODEL,
 )
 
 EXAMPLE_ANCHOR_POINTS = {
-    AnchorPoint(target_class="File", identifier_slot="alias", root_slot="has_file"),
-    AnchorPoint(
-        target_class="Dataset", identifier_slot="alias", root_slot="has_dataset"
-    ),
+    AnchorPoint(target_class="File", identifier_slot="alias", root_slot="files"),
+    AnchorPoint(target_class="Dataset", identifier_slot="alias", root_slot="datasets"),
 }
 
 EXAMPLE_ANCHOR_POINTS_BY_TARGET = {
     "File": AnchorPoint(
-        target_class="File", identifier_slot="alias", root_slot="has_file"
+        target_class="File", identifier_slot="alias", root_slot="files"
     ),
     "Dataset": AnchorPoint(
-        target_class="Dataset", identifier_slot="alias", root_slot="has_dataset"
+        target_class="Dataset", identifier_slot="alias", root_slot="datasets"
     ),
 }
 
 
 def test_get_anchor_points_happy():
     """Test the happy path of using the get_anchor_points function."""
 
     expected_anchor_points = EXAMPLE_ANCHOR_POINTS
 
-    observed_anchor_points = get_anchor_points(model=MINIMAL_VALID_METADATA_MODEL)
+    observed_anchor_points = get_anchor_points(model=VALID_MINIMAL_METADATA_MODEL)
 
     assert observed_anchor_points == expected_anchor_points
 
 
 @pytest.mark.parametrize("invalid_model", ANCHORS_INVALID_MODELS)
 def test_get_anchor_points_invalid(invalid_model: MetadataModel):
     """Test the get_anchor_points function for models with invalid anchor points."""
@@ -71,15 +69,15 @@
 
 def test_get_anchor_points_by_target_happy():
     """Test the happy path of using the get_anchors_by_target function."""
 
     expected_anchor_points = EXAMPLE_ANCHOR_POINTS_BY_TARGET
 
     observed_anchor_points = get_anchors_points_by_target(
-        model=MINIMAL_VALID_METADATA_MODEL
+        model=VALID_MINIMAL_METADATA_MODEL
     )
 
     assert observed_anchor_points == expected_anchor_points
 
 
 def test_filter_anchor_points_happy():
     """Test the happy path of using the filter_anchor_points function."""
```

### Comparing `metldata-0.1.0/tests/model_utils/test_assumptions.py` & `metldata-0.2.0/tests/model_utils/test_assumptions.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,19 +18,22 @@
 from contextlib import nullcontext
 
 import pytest
 
 from metldata.model_utils.assumptions import (
     MetadataModelAssumptionError,
     check_basic_model_assumption,
+    check_class_exists,
+    check_class_slot_exists,
 )
 from metldata.model_utils.essentials import MetadataModel
 from tests.fixtures.metadata_models import (
     INVALID_METADATA_MODELS,
     VALID_METADATA_MODELS,
+    VALID_MINIMAL_METADATA_MODEL,
 )
 
 
 @pytest.mark.parametrize(
     "model, is_valid",
     [(valid_model, True) for valid_model in VALID_METADATA_MODELS]
     + [(invalid_model, False) for invalid_model in INVALID_METADATA_MODELS],
@@ -38,7 +41,53 @@
 def test_metadata_model_assumption_checking(model: MetadataModel, is_valid: bool):
     """Test the assumptions regarding the metadata model are correctly checked."""
 
     with nullcontext() if is_valid else pytest.raises(  # type:ignore
         MetadataModelAssumptionError
     ):
         check_basic_model_assumption(model)
+
+
+@pytest.mark.parametrize(
+    "model, class_name, exists",
+    [
+        (VALID_MINIMAL_METADATA_MODEL, "Dataset", True),
+        (VALID_MINIMAL_METADATA_MODEL, "NotExistingClass", False),
+    ],
+)
+def test_check_class_exists(model: MetadataModel, class_name: str, exists: bool):
+    """Test the check_class_exists function."""
+
+    with nullcontext() if exists else pytest.raises(  # type:ignore
+        MetadataModelAssumptionError
+    ):
+        check_class_exists(model=model, class_name=class_name)
+
+
+@pytest.mark.parametrize(
+    "model, class_name, slot_name, ignore_parents, exists",
+    [
+        (VALID_MINIMAL_METADATA_MODEL, "Dataset", "alias", False, True),
+        (VALID_MINIMAL_METADATA_MODEL, "Dataset", "alias", True, False),
+        (VALID_MINIMAL_METADATA_MODEL, "Dataset", "files", True, True),
+        (VALID_MINIMAL_METADATA_MODEL, "Dataset", "not_existing_slot", False, False),
+        (VALID_MINIMAL_METADATA_MODEL, "NotExistingClass", "name", False, False),
+    ],
+)
+def test_check_class_slot_exists(
+    model: MetadataModel,
+    class_name: str,
+    slot_name: str,
+    ignore_parents: bool,
+    exists: bool,
+):
+    """Test the check_class_slot_exists function."""
+
+    with nullcontext() if exists else pytest.raises(  # type:ignore
+        MetadataModelAssumptionError
+    ):
+        check_class_slot_exists(
+            model=model,
+            class_name=class_name,
+            slot_name=slot_name,
+            ignore_parents=ignore_parents,
+        )
```

### Comparing `metldata-0.1.0/tests/model_utils/test_config.py` & `metldata-0.2.0/tests/model_utils/test_config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.1.0/tests/model_utils/test_essentials.py` & `metldata-0.2.0/tests/model_utils/test_essentials.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from copy import deepcopy
 
 from linkml_runtime import SchemaView
 
 from metldata.model_utils.essentials import MetadataModel
 from tests.fixtures.metadata_models import (
-    MINIMAL_VALID_METADATA_MODEL,
+    VALID_MINIMAL_METADATA_MODEL,
     VALID_MINIMAL_MODEL_EXAMPLE_PATH,
 )
 
 
 def test_metadata_model_from_path():
     """Test the MetadataModel creation from path."""
 
@@ -34,23 +34,23 @@
 
     assert model.name == "Minimal-Model"
 
 
 def test_metadata_model_get_schema_view():
     """Test getting a schema view from a MetadataModel."""
 
-    schema_view = MINIMAL_VALID_METADATA_MODEL.schema_view
+    schema_view = VALID_MINIMAL_METADATA_MODEL.schema_view
 
     assert isinstance(schema_view, SchemaView)
 
 
 def test_metadata_model_temporary_yaml():
     """Test getting a temporary yaml file from a MetadataModel."""
 
-    model = deepcopy(MINIMAL_VALID_METADATA_MODEL)
+    model = deepcopy(VALID_MINIMAL_METADATA_MODEL)
 
     # modify the model:
     model.name = "Test-Model-Modified"
 
     # get a temporary yaml file:
     with model.temporary_yaml_path() as model_path:
         # load a copy of that file into a new model instance:
```

### Comparing `metldata-0.1.0/tests/model_utils/test_identifiers.py` & `metldata-0.2.0/tests/model_utils/test_identifiers.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """Test the identifiers module."""
 
 from metldata.model_utils.identifiers import get_class_identifiers
-from tests.fixtures.metadata_models import MINIMAL_VALID_METADATA_MODEL
+from tests.fixtures.metadata_models import VALID_MINIMAL_METADATA_MODEL
 
 
 def test_get_class_identifiers_happy():
     """Test the happy path of using the get_class_identifiers function."""
 
     expected_identifiers = {"File": "alias", "Dataset": "alias"}
 
-    observed_identifiers = get_class_identifiers(model=MINIMAL_VALID_METADATA_MODEL)
+    observed_identifiers = get_class_identifiers(model=VALID_MINIMAL_METADATA_MODEL)
 
     assert observed_identifiers == expected_identifiers
```

### Comparing `metldata-0.1.0/tests/model_utils/test_metadata_validator.py` & `metldata-0.2.0/tests/model_utils/test_metadata_validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,27 +21,27 @@
 import pytest
 
 from metldata.model_utils.metadata_validator import MetadataValidator
 from tests.fixtures.metadata import (
     INVALID_MINIMAL_METADATA_EXAMPLES,
     VALID_MINIMAL_METADATA_EXAMPLES,
 )
-from tests.fixtures.metadata_models import MINIMAL_VALID_METADATA_MODEL
+from tests.fixtures.metadata_models import VALID_MINIMAL_METADATA_MODEL
 
 
 @pytest.mark.parametrize(
     "metadata, is_valid",
     [(valid_metadata, True) for valid_metadata in VALID_MINIMAL_METADATA_EXAMPLES]
     + [
         (invalid_metadata, False)
         for invalid_metadata in INVALID_MINIMAL_METADATA_EXAMPLES
     ],
 )
 def test_validate_against_model(metadata: dict[str, Any], is_valid: bool):
     """Test the validation of metadata against a model."""
 
-    validator = MetadataValidator(model=MINIMAL_VALID_METADATA_MODEL)
+    validator = MetadataValidator(model=VALID_MINIMAL_METADATA_MODEL)
 
     with nullcontext() if is_valid else pytest.raises(  # type:ignore
         MetadataValidator.ValidationError
     ):
         validator.validate(metadata)
```

### Comparing `metldata-0.1.0/tests/submission_registry/__init__.py` & `metldata-0.2.0/tests/submission_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.1.0/tests/submission_registry/test_event_publisher.py` & `metldata-0.2.0/tests/submission_registry/test_models.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,43 +8,47 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+#
 
-"""Testing the event publisher."""
+"""Test model functionality."""
 
-from ghga_service_chassis_lib.utils import now_as_utc
+from datetime import timedelta
 
-from metldata.config import Config
-from metldata.submission_registry import models
-from metldata.submission_registry.event_publisher import EventPublisher
-from tests.fixtures.config import config_fixture  # noqa:402
-from tests.fixtures.utils import check_source_event
+from ghga_service_commons.utils.utc_dates import now_as_utc
 
+from metldata.submission_registry.models import (
+    StatusChange,
+    Submission,
+    SubmissionStatus,
+)
 
-def test_happy(config_fixture: Config):  # noqa: F811
-    """Test the happy path of publishing a submission."""
 
-    event_publisher = EventPublisher(config=config_fixture)
+def test_submission_current_status():
+    """Test whether the current status property returns the latest status."""
 
-    # publish a submission:
-    submission = models.Submission(
-        id="submission001",
+    submission = Submission(
         title="test",
         description="test",
-        content={"test": "test"},
-        status_history=[
-            models.StatusChange(
-                timestamp=now_as_utc(), new_status=models.SubmissionStatus.PENDING
-            )
-        ],
+        content={"test_class": [{"alias": "test_alias1"}]},
+        accession_map={"test_class": {"test_alias1": "test_accession1"}},
+        id="testsubmission001",
+        status_history=(
+            StatusChange(
+                timestamp=now_as_utc(), new_status=SubmissionStatus.IN_REVIEW  # second
+            ),
+            StatusChange(
+                timestamp=now_as_utc() + timedelta(days=10),  # third
+                new_status=SubmissionStatus.COMPLETED,
+            ),
+            StatusChange(
+                timestamp=now_as_utc() - timedelta(days=10),  # first
+                new_status=SubmissionStatus.PENDING,
+            ),
+        ),
     )
-    event_publisher.publish_submission(submission)
 
-    # check published source event:
-    check_source_event(
-        expected_content=submission,
-        source_events_dir=config_fixture.source_events_dir,
-    )
+    assert submission.current_status == SubmissionStatus.COMPLETED
```

### Comparing `metldata-0.1.0/tests/transform/__init__.py` & `metldata-0.2.0/tests/builtin_workflows/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-"""Test the transform sub-package."""
+"""Test builtin_workflows subpackage."""
```

### Comparing `metldata-0.1.0/tests/transform/test_handling.py` & `metldata-0.2.0/tests/transform/test_handling.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,31 +16,31 @@
 
 """Test the handling module. Only edge cases that are not covered by tests
 with builtin transformations are tested here."""
 
 import pytest
 
 from metldata.builtin_transformations.infer_references.main import (
+    REFERENCE_INFERENCE_TRANSFORMATION,
     ReferenceInferenceConfig,
-    reference_inference_transformation,
 )
 from metldata.model_utils.essentials import MetadataModel
 from metldata.transform.base import (
     MetadataModelAssumptionError,
     MetadataModelTransformationError,
     TransformationDefinition,
 )
 from metldata.transform.handling import TransformationHandler
-from tests.fixtures.metadata_models import ADVANCED_VALID_METADATA_MODEL
+from tests.fixtures.metadata_models import VALID_ADVANCED_METADATA_MODEL
 
 VALID_EXAMPLE_CONFIG = ReferenceInferenceConfig(
     inferred_ref_map={
         "Experiment": {
-            "has_file": {
-                "path": "Experiment(has_sample)>Sample(has_file)>File",
+            "files": {
+                "path": "Experiment(samples)>Sample(files)>File",
                 "multivalued": True,
             }
         }
     }
 )
 
 
@@ -51,44 +51,44 @@
     def always_failing_assumptions(
         model: MetadataModel, config: ReferenceInferenceConfig
     ):
         """A function that always raises a MetadataModelAssumptionError."""
         raise MetadataModelAssumptionError
 
     transformation = TransformationDefinition(
-        config=reference_inference_transformation.config,
+        config_cls=REFERENCE_INFERENCE_TRANSFORMATION.config_cls,
         check_model_assumptions=always_failing_assumptions,
-        transform_model=reference_inference_transformation.transform_model,
-        metadata_transformer_factory=reference_inference_transformation.metadata_transformer_factory,
+        transform_model=REFERENCE_INFERENCE_TRANSFORMATION.transform_model,
+        metadata_transformer_factory=REFERENCE_INFERENCE_TRANSFORMATION.metadata_transformer_factory,
     )
 
     with pytest.raises(MetadataModelAssumptionError):
         _ = TransformationHandler(
             transformation_definition=transformation,
             transformation_config=VALID_EXAMPLE_CONFIG,
-            original_model=ADVANCED_VALID_METADATA_MODEL,
+            original_model=VALID_ADVANCED_METADATA_MODEL,
         )
 
 
 def test_transformation_handler_model_transformation_error():
     """Test using the TransformationHandling when model transformation fails."""
 
     # make transformation definition always raise an MetadataModelAssumptionError:
     def always_failing_transformation(
         original_model: MetadataModel, config: ReferenceInferenceConfig
     ):
         """A function that always raises a MetadataModelTransformationError."""
         raise MetadataModelTransformationError
 
     transformation = TransformationDefinition(
-        config=reference_inference_transformation.config,
-        check_model_assumptions=reference_inference_transformation.check_model_assumptions,
+        config_cls=REFERENCE_INFERENCE_TRANSFORMATION.config_cls,
+        check_model_assumptions=REFERENCE_INFERENCE_TRANSFORMATION.check_model_assumptions,
         transform_model=always_failing_transformation,
-        metadata_transformer_factory=reference_inference_transformation.metadata_transformer_factory,
+        metadata_transformer_factory=REFERENCE_INFERENCE_TRANSFORMATION.metadata_transformer_factory,
     )
 
     with pytest.raises(MetadataModelTransformationError):
         _ = TransformationHandler(
             transformation_definition=transformation,
             transformation_config=VALID_EXAMPLE_CONFIG,
-            original_model=ADVANCED_VALID_METADATA_MODEL,
+            original_model=VALID_ADVANCED_METADATA_MODEL,
         )
```

