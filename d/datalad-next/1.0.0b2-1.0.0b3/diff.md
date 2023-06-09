# Comparing `tmp/datalad_next-1.0.0b2.tar.gz` & `tmp/datalad_next-1.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datalad_next-1.0.0b2.tar", last modified: Fri Mar 17 17:02:39 2023, max compression
+gzip compressed data, was "datalad_next-1.0.0b3.tar", last modified: Fri Jun  9 08:45:49 2023, max compression
```

## Comparing `datalad_next-1.0.0b2.tar` & `datalad_next-1.0.0b3.tar`

### file list

```diff
@@ -1,162 +1,218 @@
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:39.699346 datalad_next-1.0.0b2/
--rw-rw-r--   0 mih       (1000) mih       (1000)       70 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/CONTRIBUTORS
--rw-rw-r--   0 mih       (1000) mih       (1000)     1300 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/LICENSE
--rw-rw-r--   0 mih       (1000) mih       (1000)      124 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/MANIFEST.in
--rw-rw-r--   0 mih       (1000) mih       (1000)     9668 2023-03-17 17:02:39.699346 datalad_next-1.0.0b2/PKG-INFO
--rw-rw-r--   0 mih       (1000) mih       (1000)     9147 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/README.md
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:39.691346 datalad_next-1.0.0b2/_datalad_buildsupport/
--rw-rw-r--   0 mih       (1000) mih       (1000)      529 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/_datalad_buildsupport/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    10698 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/_datalad_buildsupport/formatters.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     8520 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/_datalad_buildsupport/setup.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:39.699346 datalad_next-1.0.0b2/datalad_next/
--rw-rw-r--   0 mih       (1000) mih       (1000)     3041 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      499 2023-03-17 17:02:39.699346 datalad_next-1.0.0b2/datalad_next/_version.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:39.691346 datalad_next-1.0.0b2/datalad_next/annexbackends/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/annexbackends/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    10374 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/annexbackends/base.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:39.691346 datalad_next-1.0.0b2/datalad_next/annexbackends/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/annexbackends/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1984 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/annexbackends/tests/test_base.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2429 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/annexbackends/xdlra.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:39.691346 datalad_next-1.0.0b2/datalad_next/annexremotes/
--rw-rw-r--   0 mih       (1000) mih       (1000)      391 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/annexremotes/__init__.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:39.691346 datalad_next-1.0.0b2/datalad_next/annexremotes/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/annexremotes/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    16654 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/annexremotes/tests/test_uncurl.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    21823 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/annexremotes/uncurl.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:39.691346 datalad_next-1.0.0b2/datalad_next/commands/
--rw-rw-r--   0 mih       (1000) mih       (1000)     3212 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/commands/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    23896 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/commands/create_sibling_webdav.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    19234 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/commands/credentials.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    14003 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/commands/download.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:39.691346 datalad_next-1.0.0b2/datalad_next/commands/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/commands/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    13556 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/commands/tests/test_create_sibling_webdav.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     6055 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/commands/tests/test_credentials.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     8664 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/commands/tests/test_download.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    31590 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/commands/tests/test_tree.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    46815 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/commands/tree.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1104 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/conftest.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:39.691346 datalad_next-1.0.0b2/datalad_next/constraints/
--rw-rw-r--   0 mih       (1000) mih       (1000)      997 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/constraints/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     8628 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/constraints/base.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    15744 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/constraints/basic.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    18457 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/constraints/compound.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     4895 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/constraints/dataset.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    12533 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/constraints/exceptions.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     3879 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/constraints/formats.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2323 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/constraints/git.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    17072 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/constraints/parameter.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     7359 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/constraints/parameter_legacy.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:39.691346 datalad_next-1.0.0b2/datalad_next/constraints/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/constraints/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     4416 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/constraints/tests/test_base.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     9131 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/constraints/tests/test_basic.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    11396 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/constraints/tests/test_cmdarg_validation.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     9521 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/constraints/tests/test_compound.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1807 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/constraints/tests/test_exceptions.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    13462 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/constraints/tests/test_special_purpose.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2107 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/constraints/tests/test_tutorial.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1047 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/constraints/utils.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:39.691346 datalad_next-1.0.0b2/datalad_next/credman/
--rw-rw-r--   0 mih       (1000) mih       (1000)       39 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/credman/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    43760 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/credman/manager.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:39.695346 datalad_next-1.0.0b2/datalad_next/credman/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/credman/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    14808 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/credman/tests/test_credman.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:39.695346 datalad_next-1.0.0b2/datalad_next/datasets/
--rw-rw-r--   0 mih       (1000) mih       (1000)      465 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/datasets/__init__.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:39.695346 datalad_next-1.0.0b2/datalad_next/exceptions/
--rw-rw-r--   0 mih       (1000) mih       (1000)      423 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/exceptions/__init__.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:39.695346 datalad_next-1.0.0b2/datalad_next/gitremotes/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/gitremotes/__init__.py
--rwxrwxr-x   0 mih       (1000) mih       (1000)    49544 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/gitremotes/datalad_annex.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:39.695346 datalad_next-1.0.0b2/datalad_next/gitremotes/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/gitremotes/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    14678 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/gitremotes/tests/test_datalad_annex.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:39.695346 datalad_next-1.0.0b2/datalad_next/patches/
--rw-rw-r--   0 mih       (1000) mih       (1000)      194 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/patches/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     4196 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/patches/annexrepo.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      491 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/patches/common_cfg.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     6848 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/patches/configuration.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     5444 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/patches/create_sibling_ghlike.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1197 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/patches/distribution_dataset.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    10908 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/patches/interface_utils.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    16444 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/patches/push_optimize.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    10108 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/patches/push_to_export_remote.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2447 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/patches/siblings.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      827 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/patches/test_keyring.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:39.695346 datalad_next-1.0.0b2/datalad_next/patches/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/patches/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1824 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/patches/tests/test_configuration.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1488 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/patches/tests/test_create_sibling_ghlike.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1406 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/patches/tests/test_push.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     7834 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/patches/tests/test_push_to_export_remote.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:39.695346 datalad_next-1.0.0b2/datalad_next/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    12055 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/tests/fixtures.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      142 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/tests/test_common_cfg.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      120 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/tests/test_register.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      486 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/tests/test_testutils.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     4544 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/tests/utils.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:39.695346 datalad_next-1.0.0b2/datalad_next/uis/
--rw-rw-r--   0 mih       (1000) mih       (1000)      182 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/uis/__init__.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:39.695346 datalad_next-1.0.0b2/datalad_next/url_operations/
--rw-rw-r--   0 mih       (1000) mih       (1000)    16350 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/url_operations/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     8002 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/url_operations/any.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     9074 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/url_operations/file.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     9793 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/url_operations/http.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    14290 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/url_operations/ssh.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:39.695346 datalad_next-1.0.0b2/datalad_next/url_operations/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/url_operations/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2040 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/url_operations/tests/test_any.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     3442 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/url_operations/tests/test_file.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1544 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/url_operations/tests/test_http.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     4369 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/url_operations/tests/test_ssh.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:39.695346 datalad_next-1.0.0b2/datalad_next/utils/
--rw-rw-r--   0 mih       (1000) mih       (1000)     7069 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/utils/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      267 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/utils/consts.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      326 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/utils/credman.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2667 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/utils/http_helpers.py
--rw-rw-r--   0 mih       (1000) mih       (1000)       37 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/utils/log.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2013 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/utils/patch.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    12336 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/utils/requests_auth.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:39.695346 datalad_next-1.0.0b2/datalad_next/utils/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/datalad_next/utils/tests/__init__.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:39.691346 datalad_next-1.0.0b2/datalad_next.egg-info/
--rw-rw-r--   0 mih       (1000) mih       (1000)     9668 2023-03-17 17:02:39.000000 datalad_next-1.0.0b2/datalad_next.egg-info/PKG-INFO
--rw-rw-r--   0 mih       (1000) mih       (1000)     4573 2023-03-17 17:02:39.000000 datalad_next-1.0.0b2/datalad_next.egg-info/SOURCES.txt
--rw-rw-r--   0 mih       (1000) mih       (1000)        1 2023-03-17 17:02:39.000000 datalad_next-1.0.0b2/datalad_next.egg-info/dependency_links.txt
--rw-rw-r--   0 mih       (1000) mih       (1000)      272 2023-03-17 17:02:39.000000 datalad_next-1.0.0b2/datalad_next.egg-info/entry_points.txt
--rw-rw-r--   0 mih       (1000) mih       (1000)      153 2023-03-17 17:02:39.000000 datalad_next-1.0.0b2/datalad_next.egg-info/requires.txt
--rw-rw-r--   0 mih       (1000) mih       (1000)       13 2023-03-17 17:02:39.000000 datalad_next-1.0.0b2/datalad_next.egg-info/top_level.txt
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:39.695346 datalad_next-1.0.0b2/docs/
--rw-rw-r--   0 mih       (1000) mih       (1000)      469 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/docs/CODEOWNERS
--rw-rw-r--   0 mih       (1000) mih       (1000)     7496 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/docs/Makefile
--rw-rw-r--   0 mih       (1000) mih       (1000)     1755 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/docs/README.md
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:39.695346 datalad_next-1.0.0b2/docs/policy/
--rw-rw-r--   0 mih       (1000) mih       (1000)      826 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/docs/policy/release-management.md
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:39.695346 datalad_next-1.0.0b2/docs/source/
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:39.695346 datalad_next-1.0.0b2/docs/source/_static/
--rw-rw-r--   0 mih       (1000) mih       (1000)      958 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/docs/source/_static/datalad_logo.png
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:39.687346 datalad_next-1.0.0b2/docs/source/_templates/
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:39.699346 datalad_next-1.0.0b2/docs/source/_templates/autosummary/
--rw-rw-r--   0 mih       (1000) mih       (1000)      116 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/docs/source/_templates/autosummary/class.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)      436 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/docs/source/_templates/autosummary/module.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)      142 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/docs/source/annex-backends.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)      149 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/docs/source/annex-specialremotes.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)      181 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/docs/source/api.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)      225 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/docs/source/cmd.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)     4835 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/docs/source/conf.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-03-17 17:02:39.699346 datalad_next-1.0.0b2/docs/source/developer_guide/
--rw-rw-r--   0 mih       (1000) mih       (1000)     3439 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/docs/source/developer_guide/constraints.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)      497 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/docs/source/developer_guide/contributing.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)      357 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/docs/source/developer_guide/index.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)      140 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/docs/source/git-remote-helpers.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)     2135 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/docs/source/index.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)      296 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/docs/source/patches.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)      381 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/docs/source/pyutils.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)       60 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/pyproject.toml
--rw-rw-r--   0 mih       (1000) mih       (1000)     1332 2023-03-17 17:02:39.699346 datalad_next-1.0.0b2/setup.cfg
--rwxrwxr-x   0 mih       (1000) mih       (1000)      364 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/setup.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    68607 2023-03-17 17:02:34.000000 datalad_next-1.0.0b2/versioneer.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:49.374657 datalad_next-1.0.0b3/
+-rw-rw-r--   0 mih       (1000) mih       (1000)       70 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/CONTRIBUTORS
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1300 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/LICENSE
+-rw-rw-r--   0 mih       (1000) mih       (1000)      124 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/MANIFEST.in
+-rw-rw-r--   0 mih       (1000) mih       (1000)     9653 2023-06-09 08:45:49.374657 datalad_next-1.0.0b3/PKG-INFO
+-rw-rw-r--   0 mih       (1000) mih       (1000)     9132 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/README.md
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:49.366657 datalad_next-1.0.0b3/_datalad_buildsupport/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      529 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/_datalad_buildsupport/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    10699 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/_datalad_buildsupport/formatters.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     8520 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/_datalad_buildsupport/setup.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:49.378657 datalad_next-1.0.0b3/datalad_next/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3931 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      499 2023-06-09 08:45:49.378657 datalad_next-1.0.0b3/datalad_next/_version.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:49.366657 datalad_next-1.0.0b3/datalad_next/annexbackends/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/annexbackends/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    10375 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/annexbackends/base.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:49.366657 datalad_next-1.0.0b3/datalad_next/annexbackends/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/annexbackends/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1984 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/annexbackends/tests/test_base.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2429 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/annexbackends/xdlra.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:49.366657 datalad_next-1.0.0b3/datalad_next/annexremotes/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3639 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/annexremotes/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    24410 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/annexremotes/archivist.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:49.366657 datalad_next-1.0.0b3/datalad_next/annexremotes/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/annexremotes/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     9828 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/annexremotes/tests/test_archivist.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    16653 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/annexremotes/tests/test_uncurl.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    22301 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/annexremotes/uncurl.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:49.366657 datalad_next-1.0.0b3/datalad_next/archive_operations/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1881 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/archive_operations/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2426 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/archive_operations/tarfile.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:49.366657 datalad_next-1.0.0b3/datalad_next/commands/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3125 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/commands/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    23894 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/commands/create_sibling_webdav.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    19234 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/commands/credentials.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    14126 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/commands/download.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    13562 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/commands/ls_file_collection.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:49.366657 datalad_next-1.0.0b3/datalad_next/commands/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/commands/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    13556 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/commands/tests/test_create_sibling_webdav.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     6055 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/commands/tests/test_credentials.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     8665 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/commands/tests/test_download.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     6840 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/commands/tests/test_ls_file_collection.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    31590 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/commands/tests/test_tree.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    46816 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/commands/tree.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:49.366657 datalad_next-1.0.0b3/datalad_next/config/
+-rw-rw-r--   0 mih       (1000) mih       (1000)       41 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/config/__init__.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:49.366657 datalad_next-1.0.0b3/datalad_next/config/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/config/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      325 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/config/tests/test_core.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     5747 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/config/tests/test_utils.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3355 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/config/utils.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1399 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/conftest.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:49.370658 datalad_next-1.0.0b3/datalad_next/constraints/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2597 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/constraints/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     8627 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/constraints/base.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    16244 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/constraints/basic.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    18685 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/constraints/compound.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     4774 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/constraints/dataset.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    12979 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/constraints/exceptions.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3881 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/constraints/formats.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2371 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/constraints/git.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    18669 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/constraints/parameter.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     7361 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/constraints/parameter_legacy.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:49.370658 datalad_next-1.0.0b3/datalad_next/constraints/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/constraints/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     4416 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/constraints/tests/test_base.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     9112 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/constraints/tests/test_basic.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    12038 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/constraints/tests/test_cmdarg_validation.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     9522 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/constraints/tests/test_compound.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1807 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/constraints/tests/test_exceptions.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    13462 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/constraints/tests/test_special_purpose.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2107 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/constraints/tests/test_tutorial.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1047 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/constraints/utils.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:49.370658 datalad_next-1.0.0b3/datalad_next/credman/
+-rw-rw-r--   0 mih       (1000) mih       (1000)       39 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/credman/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    43830 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/credman/manager.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:49.370658 datalad_next-1.0.0b3/datalad_next/credman/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/credman/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    14813 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/credman/tests/test_credman.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:49.370658 datalad_next-1.0.0b3/datalad_next/datasets/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2714 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/datasets/__init__.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:49.370658 datalad_next-1.0.0b3/datalad_next/exceptions/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      429 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/exceptions/__init__.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:49.370658 datalad_next-1.0.0b3/datalad_next/gitremotes/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/gitremotes/__init__.py
+-rwxrwxr-x   0 mih       (1000) mih       (1000)    50583 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/gitremotes/datalad_annex.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:49.370658 datalad_next-1.0.0b3/datalad_next/gitremotes/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/gitremotes/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    14680 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/gitremotes/tests/test_datalad_annex.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:49.370658 datalad_next-1.0.0b3/datalad_next/iter_collections/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      822 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/iter_collections/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1859 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/iter_collections/directory.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     9169 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/iter_collections/gitworktree.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2669 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/iter_collections/tarfile.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:49.370658 datalad_next-1.0.0b3/datalad_next/iter_collections/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/iter_collections/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2841 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/iter_collections/tests/test_iterdir.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2691 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/iter_collections/tests/test_itergitworktree.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3357 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/iter_collections/tests/test_itertar.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2449 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/iter_collections/tests/test_iterzip.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2877 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/iter_collections/utils.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2215 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/iter_collections/zipfile.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:49.370658 datalad_next-1.0.0b3/datalad_next/patches/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2009 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/patches/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     4173 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/patches/annexrepo.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1836 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/patches/cli_configoverrides.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      334 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/patches/commanderror.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      491 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/patches/common_cfg.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     6848 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/patches/configuration.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     5443 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/patches/create_sibling_ghlike.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    16004 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/patches/create_sibling_gitlab.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     5037 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/patches/customremotes_main.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1174 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/patches/distribution_dataset.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      288 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/patches/enabled.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    11076 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/patches/interface_utils.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    16380 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/patches/push_optimize.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    10053 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/patches/push_to_export_remote.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2424 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/patches/siblings.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      827 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/patches/test_keyring.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:49.370658 datalad_next-1.0.0b3/datalad_next/patches/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/patches/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2271 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/patches/tests/test_annex_progress_logging.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      621 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/patches/tests/test_cli_configoverrides.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      339 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/patches/tests/test_commanderror.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1824 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/patches/tests/test_configuration.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1488 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/patches/tests/test_create_sibling_ghlike.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    17125 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/patches/tests/test_create_sibling_gitlab.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1406 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/patches/tests/test_push.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     7807 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/patches/tests/test_push_to_export_remote.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:49.374657 datalad_next-1.0.0b3/datalad_next/runners/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      684 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/runners/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      365 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/runners/exceptions.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      887 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/runners/protocols.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:49.374657 datalad_next-1.0.0b3/datalad_next/runners/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/runners/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      330 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/runners/tests/test_exceptions.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:49.374657 datalad_next-1.0.0b3/datalad_next/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    12892 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/tests/fixtures.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      142 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/tests/test_common_cfg.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      120 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/tests/test_register.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      486 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/tests/test_testutils.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     4544 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/tests/utils.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:49.374657 datalad_next-1.0.0b3/datalad_next/types/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/types/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1523 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/types/annexkey.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     5285 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/types/archivist.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      266 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/types/enums.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:49.374657 datalad_next-1.0.0b3/datalad_next/types/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/types/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      905 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/types/tests/test_annexkey.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1723 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/types/tests/test_archivist.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:49.374657 datalad_next-1.0.0b3/datalad_next/uis/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      182 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/uis/__init__.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:49.374657 datalad_next-1.0.0b3/datalad_next/url_operations/
+-rw-rw-r--   0 mih       (1000) mih       (1000)    15913 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/url_operations/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     8072 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/url_operations/any.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     9029 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/url_operations/file.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    11605 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/url_operations/http.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    13267 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/url_operations/ssh.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:49.374657 datalad_next-1.0.0b3/datalad_next/url_operations/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/url_operations/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2040 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/url_operations/tests/test_any.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3443 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/url_operations/tests/test_file.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     4141 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/url_operations/tests/test_http.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     4369 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/url_operations/tests/test_ssh.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:49.374657 datalad_next-1.0.0b3/datalad_next/utils/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     7092 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/utils/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      267 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/utils/consts.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      326 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/utils/credman.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3927 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/utils/deprecate.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2667 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/utils/http_helpers.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)       37 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/utils/log.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1737 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/utils/multihash.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)       61 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/utils/patch.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    12442 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/utils/requests_auth.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:49.374657 datalad_next-1.0.0b3/datalad_next/utils/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/utils/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     5634 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/utils/tests/test_deprecated.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      543 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/datalad_next/utils/tests/test_multihash.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:49.366657 datalad_next-1.0.0b3/datalad_next.egg-info/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     9653 2023-06-09 08:45:49.000000 datalad_next-1.0.0b3/datalad_next.egg-info/PKG-INFO
+-rw-rw-r--   0 mih       (1000) mih       (1000)     6543 2023-06-09 08:45:49.000000 datalad_next-1.0.0b3/datalad_next.egg-info/SOURCES.txt
+-rw-rw-r--   0 mih       (1000) mih       (1000)        1 2023-06-09 08:45:49.000000 datalad_next-1.0.0b3/datalad_next.egg-info/dependency_links.txt
+-rw-rw-r--   0 mih       (1000) mih       (1000)      342 2023-06-09 08:45:49.000000 datalad_next-1.0.0b3/datalad_next.egg-info/entry_points.txt
+-rw-rw-r--   0 mih       (1000) mih       (1000)      162 2023-06-09 08:45:49.000000 datalad_next-1.0.0b3/datalad_next.egg-info/requires.txt
+-rw-rw-r--   0 mih       (1000) mih       (1000)       13 2023-06-09 08:45:49.000000 datalad_next-1.0.0b3/datalad_next.egg-info/top_level.txt
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:49.374657 datalad_next-1.0.0b3/docs/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      469 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/docs/CODEOWNERS
+-rw-rw-r--   0 mih       (1000) mih       (1000)     7496 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/docs/Makefile
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1755 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/docs/README.md
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:49.374657 datalad_next-1.0.0b3/docs/policy/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      826 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/docs/policy/release-management.md
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:49.374657 datalad_next-1.0.0b3/docs/source/
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:49.374657 datalad_next-1.0.0b3/docs/source/_static/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      958 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/docs/source/_static/datalad_logo.png
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:49.366657 datalad_next-1.0.0b3/docs/source/_templates/
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:49.374657 datalad_next-1.0.0b3/docs/source/_templates/autosummary/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      116 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/docs/source/_templates/autosummary/class.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)      436 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/docs/source/_templates/autosummary/module.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)      142 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/docs/source/annex-backends.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)      179 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/docs/source/annex-specialremotes.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)      203 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/docs/source/api.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)      269 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/docs/source/cmd.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)     4698 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/docs/source/conf.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2023-06-09 08:45:49.374657 datalad_next-1.0.0b3/docs/source/developer_guide/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3439 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/docs/source/developer_guide/constraints.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)      497 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/docs/source/developer_guide/contributing.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)      357 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/docs/source/developer_guide/index.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)      140 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/docs/source/git-remote-helpers.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2135 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/docs/source/index.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)      318 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/docs/source/patches.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)      508 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/docs/source/pyutils.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)       60 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/pyproject.toml
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1413 2023-06-09 08:45:49.378657 datalad_next-1.0.0b3/setup.cfg
+-rwxrwxr-x   0 mih       (1000) mih       (1000)      364 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/setup.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    68607 2023-06-09 08:45:39.000000 datalad_next-1.0.0b3/versioneer.py
```

### Comparing `datalad_next-1.0.0b2/LICENSE` & `datalad_next-1.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `datalad_next-1.0.0b2/PKG-INFO` & `datalad_next-1.0.0b3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalad_next
-Version: 1.0.0b2
+Version: 1.0.0b3
 Summary: What is next in DataLad
 Home-page: https://github.com/datalad/datalad-next
 Author: The DataLad Team and Contributors
 Author-email: team@datalad.org
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
@@ -120,15 +120,15 @@
   command's logic only, while the former enables more uniform and more
   comprehensive validation and error reporting. Beyond per-parameter validation
   and type-conversion also inter-parameter dependency validation and value
   transformations are supported.
 - Improved composition of importable functionality. Key components for `commands`,
   `annexremotes`, `datasets` (etc) are collected in topical top-level modules that
   provide "all" necessary pieces in a single place.
-- `serve_path_via_webdav` test decorator that automatically deploys a local WebDAV
+- `webdav_server` fixture that automatically deploys a local WebDAV
   server.
 - Utilities for HTTP handling
   - `probe_url()` discovers redirects and authentication requirements for an HTTP
     URL
   - `get_auth_realm()` returns a label for an authentication realm that can be used
     to query for matching credentials
 - Utilities for special remote credential management:
```

### Comparing `datalad_next-1.0.0b2/README.md` & `datalad_next-1.0.0b3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
   command's logic only, while the former enables more uniform and more
   comprehensive validation and error reporting. Beyond per-parameter validation
   and type-conversion also inter-parameter dependency validation and value
   transformations are supported.
 - Improved composition of importable functionality. Key components for `commands`,
   `annexremotes`, `datasets` (etc) are collected in topical top-level modules that
   provide "all" necessary pieces in a single place.
-- `serve_path_via_webdav` test decorator that automatically deploys a local WebDAV
+- `webdav_server` fixture that automatically deploys a local WebDAV
   server.
 - Utilities for HTTP handling
   - `probe_url()` discovers redirects and authentication requirements for an HTTP
     URL
   - `get_auth_realm()` returns a label for an authentication realm that can be used
     to query for matching credentials
 - Utilities for special remote credential management:
```

### Comparing `datalad_next-1.0.0b2/_datalad_buildsupport/__init__.py` & `datalad_next-1.0.0b3/_datalad_buildsupport/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.0.0b2/_datalad_buildsupport/formatters.py` & `datalad_next-1.0.0b3/_datalad_buildsupport/formatters.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     def _mk_title(self, prog):
         name_version = "{0} {1}".format(prog, self._version)
         return '.TH "{0}" "{1}" "{2}" "{3}"\n'.format(
             prog, self._section, self._today, name_version)
 
     def _mk_name(self, prog, desc):
         """
-        this method is in consitent with others ... it relies on
+        this method is in consistent with others ... it relies on
         distribution
         """
         desc = desc.splitlines()[0] if desc else 'it is in the name'
         # ensure starting lower case
         desc = desc[0].lower() + desc[1:]
         return '.SH NAME\n%s \\- %s\n' % (self._bold(prog), desc)
```

### Comparing `datalad_next-1.0.0b2/_datalad_buildsupport/setup.py` & `datalad_next-1.0.0b3/_datalad_buildsupport/setup.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.0.0b2/datalad_next/annexbackends/base.py` & `datalad_next-1.0.0b3/datalad_next/annexbackends/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,15 +251,15 @@
     backend : Backend
         A class implementing the Backend interface to which this master
         is linked.
     """
 
     def __init__(self, output=sys.stdout):
         """
-        Initialize the Master with an ouput.
+        Initialize the Master with an output.
 
         Parameters
         ----------
         output : io.TextIOBase
             Where to send replies and backend messages
             Default: sys.stdout
         """
```

### Comparing `datalad_next-1.0.0b2/datalad_next/annexbackends/tests/test_base.py` & `datalad_next-1.0.0b3/datalad_next/annexbackends/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.0.0b2/datalad_next/annexbackends/xdlra.py` & `datalad_next-1.0.0b3/datalad_next/annexbackends/xdlra.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.0.0b2/datalad_next/annexremotes/tests/test_uncurl.py` & `datalad_next-1.0.0b3/datalad_next/annexremotes/tests/test_uncurl.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
     ds = existing_dataset
     dsca = ds.repo.call_annex
     # same set as in `test_uncurl_checkurl()`
     dsca(['initremote', 'myuncurl'] + std_initargs + [
         'match=.*(?P<origurl>https?://.*)$',
         f'url={hbsurl}/redirect-to?url={{origurl}}',
     ])
-    # feed it a broken URL, which must be getting fixed by the rewritting
+    # feed it a broken URL, which must be getting fixed by the rewriting
     # (pulls 24 bytes)
     testurl = f'garbled{hbsurl}/bytes/24'
     dsca(['addurl', '--file=dummy', testurl])
     # we got what we expected
     assert ds.status(
         'dummy', annex='basic', return_type='item-or-list', **res_kwargs
         )['bytesize'] == 24
```

### Comparing `datalad_next-1.0.0b2/datalad_next/annexremotes/uncurl.py` & `datalad_next-1.0.0b3/datalad_next/annexremotes/uncurl.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
 Requirements
 ------------
 
 This special remote implementation requires git-annex version 8.20210127 (or
 later) to be available.
 
-Download helper with credential management support
---------------------------------------------------
+Download helper
+---------------
 
 The simplest way to use this remote is to initialize it without any particular
 configuration::
 
     $ git annex initremote uncurl type=external externaltype=uncurl encryption=none
     initremote uncurl ok
     (recording state in git...)
@@ -35,15 +35,32 @@
 with the *uncurl* remote whether it can handle a particular URL, and will let
 the remote perform the download in case of positive response. By default, the
 remote will claim any URLs with a scheme that the local datalad-next
 installation supports. This always includes ``file://``, ``http://``, and
 ``https://``, but is extensible, and a particular installation may also support
 ``ssh://`` (by default when openssh is installed), or other schemes.
 
-With this setup, download requests now use DataLad's credential system for
+This additional URL support is also available for other commands. Here is an
+example how ``datalad addurls`` can be given any uncurl-supported URLs
+(here an SSH-URL) directly, provided that the ``uncurl`` remote was initialized
+for a dataset (as shown above)::
+
+    $ echo '[{"url":"ssh://my.server.org/home/me/file", "file":"dummy"}]' \\
+        | datalad addurls - '{url}' {'file'}
+
+This makes legacy commands (e.g., ``datalad download-url``), unnecessary, and
+facilitates the use of more advanced ``datalad addurls`` features (e.g.,
+automatic creation of subdatasets) that are not provided by lower-level
+commands like ``git annex addurl``.
+
+
+Download helper with credential management support
+--------------------------------------------------
+
+With this setup, download requests now also use DataLad's credential system for
 authentication. DataLad will automatically lookup matching credentials, prompt
 for manual entry if none are found, and offer to store them securely for later
 use after having used them successfully::
 
     $ git annex addurl http://httpbin.org/basic-auth/myuser/mypassword
     Credential needed for access to http://httpbin.org/basic-auth/myuser/mypassword
     user: myuser
@@ -206,15 +223,15 @@
 from pathlib import Path
 import re
 
 # we intentionally limit ourselves to the most basic interface
 # and even that we only need to get a `ConfigManager` instance.
 # If that class would support a plain path argument, we could
 # avoid it entirely
-from datalad_next.datasets import LeanGitRepo
+from datalad_next.datasets import LeanAnnexRepo
 
 from datalad_next.exceptions import (
     CapturedException,
     UrlOperationsRemoteError,
     UrlOperationsResourceUnknown,
 )
 from datalad_next.url_operations.any import AnyUrlOperations
@@ -231,15 +248,14 @@
     """ """
     def __init__(self, annex):
         super().__init__(annex)
         self.configs.update(
             url='Python format language template composing an access URL',
             match='(whitespace-separated list of) regular expression(s) to match particular components in supported URL via named groups',
         )
-        self.repo = None
         self.url_tmpl = None
         self.match = None
         self.url_handler = None
         # cache of properties that do not vary within a session
         # or across annex keys
         self.persistent_tmpl_props = {}
 
@@ -247,59 +263,55 @@
         # at present there is nothing that needs to be done on init/enable.
         # the remote is designed to work without any specific setup too
         pass
 
     def prepare(self):
         # we need the git remote name to be able to look up config about
         # that remote
-        remotename = self.annex.getgitremotename()
-        # get the repo to gain access to its config
-        self.repo = LeanGitRepo(self.annex.getgitdir())
         # check the config for a URL template setting
-        self.url_tmpl = self.repo.cfg.get(
-            f'remote.{remotename}.uncurl-url', '')
+        self.url_tmpl = self.get_remote_gitcfg('uncurl', 'url', '')
         # only if we have no local, overriding, configuration ask git-annex
         # for the committed special remote config on the URL template
         if not self.url_tmpl:
             # ask for the commit config, could still be empty
             self.url_tmpl = self.annex.getconfig('url')
             # TODO test the case of a fully absent URL template
             # that would be fine and only verbatim recorded URLs could
             # be sent to a downloader
 
         # unconditionally ask git-annex for a match-url setting, any local
-        # config ammends, and does not override
+        # config amends, and does not override
         self.match = self.annex.getconfig('match')
         if self.match:
             self.match = self.match.split()
             # TODO implement sanity checks, but running it through re.compile()
             # might just be enough
             self.match = [re.compile(m) for m in self.match]
-        # extend with additonal matchers from local config
+        # extend with additional matchers from local config
         self.match = (self.match or []) + [
             re.compile(m)
-            for m in ensure_list(self.repo.cfg.get(
-                f'remote.{remotename}.uncurl-match', [], get_all=True))
+            for m in ensure_list(self.get_remote_gitcfg(
+                'uncurl', 'match', default=[], get_all=True))
         ]
 
         self.message(
             f'URL rewriting template: {self.url_tmpl!r}', type='debug')
         self.message(
             f'Active URL match expressions: {[e.pattern for e in self.match]!r}',
             type='debug')
 
-        # let the URL hander use the repo's config
+        # let the URL handler use the repo's config
         self.url_handler = AnyUrlOperations(cfg=self.repo.cfg)
 
         # cache template properties
         # using function arg name syntax, we need the identifiers to be valid
         # Python symbols to work in `format()`
         self.persistent_tmpl_props.update(
             datalad_dsid=self.repo.cfg.get('datalad.dataset.id', ''),
-            git_remotename=remotename,
+            git_remotename=self.remotename,
             annex_remoteuuid=self.annex.getuuid(),
         )
 
     def claimurl(self, url):
         """Needs to check if want to handle a given URL
 
         If match expressions are configured, matches the URL against all known
@@ -340,15 +352,15 @@
             )
         except KeyError as e:
             self.message(
                 'URL rewriting template requires unavailable component '
                 f'{e}, continuing with original URL',
                 type='debug',
             )
-            # otherwise go ahead with the orginal URL. the template might
+            # otherwise go ahead with the original URL. the template might
             # just be here to aid structured uploads
         try:
             urlprops = self.url_handler.stat(url)
             return True
         except UrlOperationsRemoteError as e:
             # leave a trace in the logs
             CapturedException(e)
@@ -443,15 +455,15 @@
     def extract_tmpl_props(self, tmpl, *, urls=None, key=None):
         # look up all the standard
         allprops = dict(self.persistent_tmpl_props)
         if key:
             allprops['annex_key'] = key
             # if we are working on a specific key, check the template if it
             # needs more key-specific properties. The conditionals below
-            # are intentionally unprecise to avoid false-negatives given the
+            # are intentionally imprecise to avoid false-negatives given the
             # flexibility of the format-string-syntax
             if 'annex_dirhash' in tmpl:
                 allprops['annex_dirhash'] = self.annex.dirhash(key)
             if 'annex_dirhash_lower' in tmpl:
                 allprops['annex_dirhash_lower'] = self.annex.dirhash_lower(key)
         # try all URLs against all matchers
         for url in ensure_list(urls):
```

### Comparing `datalad_next-1.0.0b2/datalad_next/commands/__init__.py` & `datalad_next-1.0.0b3/datalad_next/commands/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,20 +5,15 @@
 
 from datalad.interface.base import (
     Interface,
     build_doc,
 )
 from datalad.interface.results import get_status_dict
 from datalad.interface.utils import generic_result_renderer
-try:
-    # datalad 0.17.10+
-    from datalad.interface.base import eval_results
-except ImportError:
-    # older datalad
-    from datalad.interface.utils import eval_results
+from datalad.interface.base import eval_results
 from datalad.support.param import Parameter
 
 from datalad_next.constraints.parameter import (
     EnsureCommandParameterization,
     ParameterConstraintContext,
 )
 from datalad_next.datasets import datasetmethod
@@ -48,15 +43,15 @@
 
     To transition a command from ``Interface`` to ``ValidatedInterface``,
     replace the base class declaration and declare a ``_validator_`` class
     member. Any ``constraints=`` declaration for ``Parameter`` instances
     should either be removed, or moved to the corresponding entry in
     ``_validator_``.
     """
-    _validator_ = None
+    _validator_: EnsureCommandParameterization | None = None
 
     @classmethod
     def get_parameter_validator(cls) -> EnsureCommandParameterization | None:
         """Returns a validator for the entire parameter set of a command
 
         If parameter validation shall be performed, this method must return an
         instance of
```

### Comparing `datalad_next-1.0.0b2/datalad_next/commands/create_sibling_webdav.py` & `datalad_next-1.0.0b3/datalad_next/commands/create_sibling_webdav.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,19 +158,19 @@
             code_py="clone('datalad-annex::?type=webdav&encryption=none&url=https://webdav.example.com/myds')",
             code_cmd='datalad clone "datalad-annex::?type=webdav&encryption=none&url=https://webdav.example.com/myds"'),
        dict(
            text="A sibling can also be created with a human-readable file "
                  "tree, suitable for data exchange with non-DataLad users, "
                  "but only able to host a single version of each file",
            code_py="create_sibling_webdav(url='https://example.com/browseable', mode='filetree')",
-           code_cmd='datalad create-sibling-webdav --mode filetree "https://example.com/browseable"'),
+           code_cmd='datalad create-sibling-webdav --mode filetree "https://example.com/browsable"'),
        dict(text="Cloning such dataset siblings is possible via a convenience "
                  "URL",
             code_py="clone('webdavs://example.com/browseable')",
-            code_cmd='datalad clone "webdavs://example.com/browseable"'),
+            code_cmd='datalad clone "webdavs://example.com/browsable"'),
        dict(text="In all cases, the storage sibling needs to explicitly "
                  "enabled prior to file content retrieval",
             code_py="siblings('enable', name='example.com-storage')",
             code_cmd='datalad siblings enable --name example.com-storage'),
     ]
 
     _params_ = dict(
@@ -504,15 +504,15 @@
     name: str
     credential_name: str
     credential: tuple
     export: bool
     existing: {skip, error, reconfigure}
     known: bool
         Flag whether the sibling is a known remote (no implied
-        necessary existance of content on the remote).
+        necessary existence of content on the remote).
     publish_depends: str or None
         publication dependency to set
     """
     if known and existing == 'skip':
         yield _get_skip_sibling_result(name, ds, 'git')
         return
 
@@ -562,15 +562,15 @@
     name: str
     credential: tuple
     export: bool
     existing: {skip, error, reconfigure}
         (Presently unused)
     known: bool
         Flag whether the sibling is a known remote (no implied
-        necessary existance of content on the remote).
+        necessary existence of content on the remote).
     """
     if known and existing == 'skip':
         yield _get_skip_sibling_result(name, ds, 'storage')
         return
 
     cmd_args = [
         'enableremote' if known and existing == 'reconfigure'
```

### Comparing `datalad_next-1.0.0b2/datalad_next/commands/credentials.py` & `datalad_next-1.0.0b3/datalad_next/commands/credentials.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.0.0b2/datalad_next/commands/download.py` & `datalad_next-1.0.0b3/datalad_next/commands/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     downloads from a variety of URL schemes. Built-in support for the schemes
     'http', 'https', 'file', and 'ssh' is provided. Extension packages
     may add additional support.
 
     In contrast to other downloader tools, this command integrates with the
     DataLad credential management and is able to auto-discover credentials.
     If no credential is available, it automatically prompts for them, and
-    offers to store them for re-use after a successfull authentication.
+    offers to store them for re-use after a successful authentication.
 
     Simultaneous hashing (checksumming) of downloaded content is supported
     with user-specified algorithms.
 
     The command can process any number of downloads (serially). it can read
     download specifications from (command line) arguments, files, or STDIN.
     It can deposit downloads to individual files, or stream to STDOUT.
@@ -85,15 +85,15 @@
     Implementation and extensibility
 
     Each URL scheme is processed by a dedicated handler. Additional
     schemes can be supported by sub-classing
     :class:`datalad_next.url_operations.UrlOperations` and implementing
     the `download()` method. Extension packages can register new handlers,
     by patching them into the `datalad_next.download._urlscheme_handlers`
-    registery dict.
+    registry dict.
     """
     #
     # argument format specifications
     #
     # any URL that we would take must have a scheme, because we switch
     # protocol handling based on that. It is also crucial for distinguishing
     # stuff like local paths and file names from URLs
@@ -242,14 +242,16 @@
          'code_cmd':
          'datalad download --hash sha256 http://example.com/data.xml"',
          'code_py':
          'download("http://example.com/data.xml", hash=["sha256"])'},
         {'text': 'Download from SSH server',
          'code_cmd': 'datalad download "ssh://example.com/home/user/data.xml"',
          'code_py': 'download("ssh://example.com/home/user/data.xml")'},
+        {'text': 'Stream a download to STDOUT',
+         'code_cmd': 'datalad -f disabled download "http://example.com -"'},
     ]
 
     @staticmethod
     @datasetmethod(name="download")
     @eval_results
     def __call__(spec, *, dataset=None, force=None, credential=None,
                  hash=None):
```

### Comparing `datalad_next-1.0.0b2/datalad_next/commands/tests/test_create_sibling_webdav.py` & `datalad_next-1.0.0b3/datalad_next/commands/tests/test_create_sibling_webdav.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.0.0b2/datalad_next/commands/tests/test_credentials.py` & `datalad_next-1.0.0b3/datalad_next/commands/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.0.0b2/datalad_next/commands/tests/test_download.py` & `datalad_next-1.0.0b3/datalad_next/commands/tests/test_download.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,15 +156,15 @@
         assert json.loads(capsys.readouterr().out) == auth_ok_response
         # repeated reads do not accumulate
         assert capsys.readouterr().out == ''
 
 
 def test_download_explicit_credential(credman, capsys, hbscred, hbsurl):
     # the provided credential has the wrong 'realm' for auto-detection.
-    # but chosing it explicitly must put things to work
+    # but choosing it explicitly must put things to work
     credman.set(hbscred[0], **hbscred[1])
     # consume stdout to make test self-contained
     capsys.readouterr()
     download({f'{hbsurl}/digest-auth/auth/mike/dummy': '-'},
              credential=hbscred[0])
     assert json.loads(capsys.readouterr().out) == auth_ok_response
```

### Comparing `datalad_next-1.0.0b2/datalad_next/commands/tests/test_tree.py` & `datalad_next-1.0.0b3/datalad_next/commands/tests/test_tree.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.0.0b2/datalad_next/commands/tree.py` & `datalad_next-1.0.0b3/datalad_next/commands/tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 lgr = logging.getLogger('datalad.local.tree')
 
 
 @build_doc
 class TreeCommand(ValidatedInterface):
     """Visualize directory and dataset hierarchies
 
-    This command mimics the UNIX/MSDOS 'tree' utility to generate and
+    This command mimics the UNIX/MS-DOS 'tree' utility to generate and
     display a directory tree, with DataLad-specific enhancements.
 
     It can serve the following purposes:
 
     1. Glorified 'tree' command
     2. Dataset discovery
     3. Programmatic directory traversal
```

### Comparing `datalad_next-1.0.0b2/datalad_next/conftest.py` & `datalad_next-1.0.0b3/datalad_next/conftest.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,14 +20,21 @@
     existing_noannex_dataset,
     # session-scope, standard http credential (full dict)
     http_credential,
     # function-scope, auth-less HTTP server
     http_server,
     # function-scope, HTTP server with required authentication
     http_server_with_basicauth,
-    # session-scope HTTPBIN URLs
+    # function-scope relay httpbin_service, unless undesired and skips instead
     httpbin,
+    # session-scope HTTPBIN instance startup and URLs
+    httpbin_service,
     # session-scope, standard webdav credential (full dict)
     webdav_credential,
     # function-scope, serve a local temp-path via WebDAV
     webdav_server,
 )
+from datalad_next.iter_collections.tests.test_itertar import (
+    # session-scope, downloads a tarball with a set of standard
+    # file/dir/link types
+    sample_tar_xz,
+)
```

### Comparing `datalad_next-1.0.0b2/datalad_next/constraints/base.py` & `datalad_next-1.0.0b3/datalad_next/constraints/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 __all__ = ['Constraint', 'AllOf', 'AnyOf', 'DatasetParameter']
 
 from .exceptions import ConstraintError
 
 
 class DatasetParameter:
-    """Utitlity class to report an original and resolve dataset parameter value
+    """Utility class to report an original and resolve dataset parameter value
 
     This is used by `EnsureDataset` to be able to report the original argument
     semantics of a dataset parameter to a receiving command. It is consumed
     by any ``Constraint.for_dataset()``.
 
     The original argument is provided via the `original` property.
     A corresponding `Dataset` instance is provided via the `ds` property.
```

### Comparing `datalad_next-1.0.0b2/datalad_next/constraints/basic.py` & `datalad_next-1.0.0b3/datalad_next/constraints/basic.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     Constraint,
     DatasetParameter,
 )
 from .utils import _type_str
 
 
 class NoConstraint(Constraint):
-    """A contraint that represents no constraints"""
+    """A constraint that represents no constraints"""
     def short_description(self):
         return ''
 
     def __call__(self, value):
         return value
 
 
@@ -39,15 +39,19 @@
         super().__init__()
         self._target_value = value
 
     def __call__(self, value):
         if value == self._target_value:
             return value
         else:
-            raise ValueError(f"value must be {self._target_value!r}")
+            self.raise_for(
+                value,
+                "must be {target_value!r}",
+                target_value=self._target_value,
+            )
 
     def short_description(self):
         return f'{self._target_value!r}'
 
     def long_description(self):
         return f'value must be {self.short_description()}'
 
@@ -116,17 +120,15 @@
             return value
         elif isinstance(value, (bytes, str)):
             value = value.lower()
             if value in ('0', 'no', 'off', 'disable', 'false'):
                 return False
             elif value in ('1', 'yes', 'on', 'enable', 'true'):
                 return True
-        raise ValueError(
-            "value '{}' must be convertible to boolean".format(
-                value))
+        self.raise_for(value, "must be convertible to boolean")
 
     def long_description(self):
         return 'value must be convertible to type bool'
 
     def short_description(self):
         return 'bool'
 
@@ -158,22 +160,25 @@
             self._match = re.compile(match)
 
     def __call__(self, value) -> str:
         if not isinstance(value, (bytes, str)):
             # do not perform a blind conversion ala str(), as almost
             # anything can be converted and the result is most likely
             # unintended
-            raise ValueError("%s is not a string" % repr(value))
+            self.raise_for(value, "must be a string")
         if len(value) < self._min_len:
-            raise ValueError("%r is shorter than of minimal length %d"
-                             % (value, self._min_len))
+            self.raise_for(value, "must have minimum length {len}",
+                                 len=self._min_len)
         if self._match:
             if not self._match.match(value):
-                raise ValueError(
-                    f'{value} does not match {self._match.pattern}')
+                self.raise_for(
+                    value,
+                    'does not match {pattern}',
+                    pattern=self._match.pattern,
+                )
         return value
 
     def long_description(self):
         return 'must be a string{}'.format(
             f' and match {self._match.pattern}' if self._match else '',
         )
 
@@ -199,16 +204,19 @@
         """
         self._prefix = prefix
         super().__init__()
 
     def __call__(self, value):
         super().__call__(value)
         if not value.startswith(self._prefix):
-            raise ValueError("%r does not start with '%s'"
-                             % (value, self._prefix))
+            self.raise_for(
+                value,
+                "does not start with {prefix!r}",
+                prefix=self._prefix,
+            )
         return value
 
     def long_description(self):
         return "value must start with '{}'".format(self._prefix)
 
     def short_description(self):
         return '{}...'.format(self._prefix)
@@ -222,15 +230,15 @@
 
 class EnsureCallable(Constraint):
     """Ensure an input is a callable object"""
     def __call__(self, value):
         if hasattr(value, '__call__'):
             return value
         else:
-            raise ValueError("value must be a callable")
+            self.raise_for(value, "must be a callable")
 
     def short_description(self):
         return 'callable'
 
     def long_description(self):
         return 'value must be a callable'
 
@@ -281,15 +289,15 @@
            Possible accepted values.
         """
         self._key = key
         super(EnsureKeyChoice, self).__init__(*values)
 
     def __call__(self, value):
         if self._key not in value:
-            raise ValueError("value not dict-like")
+            self.raise_for(value, "must be dict-like")
         super(EnsureKeyChoice, self).__call__(value[self._key])
         return value
 
     def long_description(self):
         return "value in '%s' must be one of %s" % (self._key, str(self._allowed),)
 
     def short_description(self):
@@ -369,24 +377,24 @@
           instantiated on all platforms, and not all checks are possible with
           all path types.
         is_format: {'absolute', 'relative'} or None
           If not None, the path is tested whether it matches being relative or
           absolute.
         lexists:
           If not None, the path is tested to confirmed exists or not. A symlink
-          need not point to an existing path to fullfil the "exists" condition.
+          need not point to an existing path to fulfil the "exists" condition.
         is_mode:
           If set, this callable will receive the path's `.lstat().st_mode`,
           and an exception is raised, if the return value does not evaluate
           to `True`. Typical callables for this feature are provided by the
           `stat` module, e.g. `S_ISDIR()`
         ref:
           If set, defines a reference Path any given path is compared to. The
           comparison operation is given by `ref_is`.
-        ref_is: {'parent-or-identical'}
+        ref_is: {'parent-or-same-as', 'parent-of'}
           Comparison operation to perform when `ref` is given.
         dsarg: DatasetParameter, optional
           If given, incoming paths are resolved in the following fashion:
           If, and only if, the original "dataset" parameter was a
           ``Dataset`` object instance, relative paths are interpreted as
           relative to the given dataset. In all other cases, relative paths
           are treated as relative to the current working directory.
@@ -395,28 +403,30 @@
         self._path_type = path_type
         self._is_format = is_format
         self._lexists = lexists
         self._is_mode = is_mode
         self._ref = ref
         self._ref_is = ref_is
         self._dsarg = dsarg
+        assert self._ref_is in ('parent-or-same-as', 'parent-of'), \
+            'Unrecognized `ref_is` operation label'
 
     def __call__(self, value):
         # turn it into the target type to make everything below
         # more straightforward
         path = self._path_type(value)
 
         # we are testing the format first, because resolve_path()
         # will always turn things into absolute paths
         if self._is_format is not None:
             is_abs = path.is_absolute()
             if self._is_format == 'absolute' and not is_abs:
-                raise ValueError(f'{path} is not an absolute path')
+                self.raise_for(path, 'is not an absolute path')
             elif self._is_format == 'relative' and is_abs:
-                raise ValueError(f'{path} is not a relative path')
+                self.raise_for(path, 'is not a relative path')
 
         # resolve relative paths against a dataset, if given
         if self._dsarg:
             path = resolve_path(
                 path,
                 self._dsarg.original,
                 self._dsarg.ds)
@@ -426,32 +436,38 @@
             try:
                 mode = path.lstat().st_mode
             except FileNotFoundError:
                 # this is fine, handled below
                 pass
         if self._lexists is not None:
             if self._lexists and mode is None:
-                raise ValueError(f'{path} does not exist')
+                self.raise_for(path, 'does not exist')
             elif not self._lexists and mode is not None:
-                raise ValueError(f'{path} does (already) exist')
+                self.raise_for(path, 'does (already) exist')
         if self._is_mode is not None:
             if not self._is_mode(mode):
-                raise ValueError(f'{path} does not match desired mode')
+                self.raise_for(path, 'does not match desired mode')
         if self._ref:
             ok = True
             if self._ref_is == 'parent-or-same-as':
                 ok = (path == self._ref or self._ref in path.parents)
             elif self._ref_is == 'parent-of':
                 ok = self._ref in path.parents
-            else:
-                raise ValueError('Unknown `ref_is` operation label')
+            else:  # pragma: nocover
+                # this code cannot be reached with normal usage.
+                # it is prevented by an assertion in __init__()
+                raise RuntimeError('Unknown `ref_is` operation label')
 
             if not ok:
-                raise ValueError(
-                    f'{self._ref} is not {self._ref_is} {path}')
+                self.raise_for(
+                    path,
+                    '{ref} is not {ref_is} {path}',
+                    ref=self._ref,
+                    ref_is=self._ref_is,
+                )
         return path
 
     def for_dataset(self, dataset: DatasetParameter) -> Constraint:
         """Return an similarly parametrized variant that resolves
         paths against a given dataset (argument)
```

### Comparing `datalad_next-1.0.0b2/datalad_next/constraints/compound.py` & `datalad_next-1.0.0b3/datalad_next/constraints/compound.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,29 +69,40 @@
         )
 
     @property
     def item_constraint(self):
         return self._item_constraint
 
     def __call__(self, value):
-        iter = self._iter_type(
-            self._item_constraint(i) for i in value
-        )
+        try:
+            iter = self._iter_type(
+                self._item_constraint(i) for i in value
+            )
+        except TypeError as e:
+            self.raise_for(
+                value,
+                "cannot coerce to target (item) type",
+                __caused_by__=e,
+            )
         if self._min_len is not None or self._max_len is not None:
             # only do this if necessary, generators will not support
             # __len__, for example
             iter_len = len(iter)
             if self._min_len is not None and iter_len < self._min_len:
-                raise ValueError(
-                    f'Length-{iter_len} iterable is shorter than '
-                    f'required minmum length {self._min_len}')
+                self.raise_for(
+                    iter,
+                    'must have minimum length {len}',
+                    len=self._min_len,
+                )
             if self._max_len is not None and iter_len > self._max_len:
-                raise ValueError(
-                    f'Length-{iter_len} iterable is longer than '
-                    f'required maximum length {self._max_len}')
+                self.raise_for(
+                    iter,
+                    'must not exceed maximum length {len}',
+                    len=self._max_len,
+                )
         return iter
 
     def short_description(self):
         return f'{self._iter_type}({self._item_constraint})'
 
 
 class EnsureListOf(EnsureIterableOf):
@@ -260,15 +271,15 @@
 
     def short_description(self):
         return \
             f'items of type "{self._item_constraint.short_description()}" ' \
             'read from a file-like'
 
     def __call__(self, value) -> Generator[Any, None, None]:
-        # we only support a single file-like source. If we happend to get
+        # we only support a single file-like source. If we happened to get
         # a length-1 sequence (for technical reasons, such as argparse
         # having collected the value), we unpack it.
         if isinstance(value, (list, tuple)) and len(value) == 1:
             value = value[0]
         opened_file = False
         if value == '-':
             value = sys.stdin
@@ -300,15 +311,15 @@
                         yield CapturedException(e)
         finally:
             if close_file:
                 fp.close()
 
 
 class ConstraintWithPassthrough(Constraint):
-    """Regular contraint, but with a "pass-through" value that is not processed
+    """Regular constraint, but with a "pass-through" value that is not processed
 
     This is different from a `Constraint() | EnsureValue(...)` construct,
     because the pass-through value is not communicated. This can be useful
     when a particular value must be supported for technical reasons, but
     need not, or must not be included in (error) messages.
 
     The pass-through is returned as-is, and is not processed except for an
@@ -375,15 +386,15 @@
         return self._constraint.long_description()
 
     def short_description(self) -> str:
         return self._constraint.short_description()
 
 
 class WithDescription(Constraint):
-    """Contraint that wraps another constraint and replaces its description
+    """Constraint that wraps another constraint and replaces its description
 
     Whenever a constraint's self-description does not fit an application
     context, it can be wrapped with this class. The given synopsis and
     description of valid inputs replaces those of the wrapped constraint.
     """
     def __init__(self,
                  constraint: Constraint,
```

### Comparing `datalad_next-1.0.0b2/datalad_next/constraints/dataset.py` & `datalad_next-1.0.0b3/datalad_next/constraints/dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -66,29 +66,28 @@
     def __call__(self, value) -> DatasetParameter:
         # good-enough test to recognize a dataset instance cheaply
         if hasattr(value, 'repo') and hasattr(value, 'pathobj'):
             ds = value
         # anticipate what require_dataset() could handle and fail if we got
         # something else
         elif not isinstance(value, (str, PurePath, type(None))):
-            raise TypeError(f"Cannot create Dataset from {type(value)}")
+            self.raise_for(
+                value, "cannot create Dataset from {type}", type=type(value)
+            )
         else:
             ds = self._require_dataset(value)
         assert ds
         if self._installed is not None:
             is_installed = ds.is_installed()
             if self._installed is False and is_installed:
-                raise ValueError(f'{ds} already exists locally')
+                self.raise_for(ds, 'already exists locally')
             if self._installed and not is_installed:
-                # for uniformity with require_dataset() below, use
-                # this custom exception
-                raise NoDatasetFound(f'{ds} is not installed')
+                self.raise_for(ds, 'not installed')
         if self._require_id and not ds.id:
-            raise NoDatasetFound(f'{ds} does not have a valid '
-                                 f'datalad-id')
+            self.raise_for(ds, 'does not have a valid datalad-id')
         return DatasetParameter(value, ds)
 
     def short_description(self) -> str:
         return "(path to) {}Dataset".format(
             'an existing ' if self._installed is True
             else 'a non-existing ' if self._installed is False else 'a ')
```

### Comparing `datalad_next-1.0.0b2/datalad_next/constraints/exceptions.py` & `datalad_next-1.0.0b3/datalad_next/constraints/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,32 +55,32 @@
           is used to interpolate a message, but may also contain additional
           key-value mappings. A recognized key is ``'__caused_by__'``, with
           a value of one exception (or a list of exceptions) that led to a
           ``ConstraintError`` being raised.
         """
         # the msg/ctx setup is inspired by pydantic
         # we put `msg` in the `.args` container first to match where
-        # `ValueError` would have it. Everthing else goes after it.
+        # `ValueError` would have it. Everything else goes after it.
         super().__init__(msg, constraint, value, ctx)
 
     @property
     def msg(self):
-        """Obtain an (interpolated) message on the contraint violation
+        """Obtain an (interpolated) message on the constraint violation
 
         The error message template can be interpolated with any information
         available in the error context dict (``ctx``). In addition to the
         information provided by the ``Constraint`` that raised the error,
         the following additional placeholders are provided:
 
         - ``__value__``: the value reported to have caused the error
         - ``__itemized_causes__``: an indented bullet list str with on
           item for each error in the ``caused_by`` report of the error.
 
         Message template can use any feature of the Python format mini
-        lanuage. For example ``{__value__!r}`` to get a ``repr()``-style
+        language. For example ``{__value__!r}`` to get a ``repr()``-style
         representation of the offending value.
         """
         msg_tmpl = self.args[0]
         # get interpolation values for message formatting
         # we need a copy, because we need to mutate the dict
         ctx = dict(self.context)
         # support a few standard placeholders
@@ -96,16 +96,24 @@
 
     @property
     def constraint(self):
         """Get the instance of the constraint that was violated"""
         return self.args[1]
 
     @property
-    def caused_by(self):
-        return self.context.get('__caused_by__', None)
+    def caused_by(self) -> Tuple[Exception] | None:
+        """Returns a tuple of any underlying exceptions that caused a violation
+        """
+        cb = self.context.get('__caused_by__', None)
+        if cb is None:
+            return
+        elif isinstance(cb, Exception):
+            return (cb,)
+        else:
+            return tuple(cb)
 
     @property
     def value(self):
         """Get the value that violated the constraint"""
         return self.args[2]
 
     @property
@@ -129,15 +137,15 @@
         )
 
 
 class ConstraintErrors(ConstraintError):
     """Exception representing context-specific ConstraintError instances
 
     This class enables the association of a context in which any particular
-    contraint was violated. This is done by passing a mapping, of a context
+    constraint was violated. This is done by passing a mapping, of a context
     identifier (e.g., a label) to the particular ``ConstraintError`` that
     occurred in this context, to the constructor.
 
     This is a generic implementation with no requirements regarding the
     nature of the context identifiers (expect for being hashable). See
     ``CommandParametrizationError`` for a specialization.
     """
@@ -261,25 +269,31 @@
             descr=f" ({self.description})" if self.description else '',
         )
 
     def get_label_with_parameter_values(self, values: dict) -> str:
         """Like ``.label`` but each parameter will also state a value"""
         # TODO truncate the values after repr() to ensure a somewhat compact
         # output
+        from .parameter import NoValue
         return '{param}{descr}'.format(
-            param=", ".join(f'{p}={values[p]!r}' for p in self.parameters),
+            param=", ".join(
+                f'{p}=<no value>'
+                if isinstance(values[p], NoValue)
+                else f'{p}={values[p]!r}'
+                for p in self.parameters
+            ),
             descr=f" ({self.description})" if self.description else '',
         )
 
 
 class ParametrizationErrors(ConstraintErrors):
     """Exception type raised on violating parameter constraints
 
     This is a ``ConstraintErrors`` variant that uses parameter names (i.e,
-    ``str`` labels) as context identifiers. In addition to individal
+    ``str`` labels) as context identifiers. In addition to individual
     parameter names an additional ``__all__`` identifier is recognized. It
     can be used to record a ``ConstraintError`` arising from high-order
     constraints, such as the violation of "mutually exclusive" requirements
     across more than one parameter.
     """
     def __init__(
             self,
```

### Comparing `datalad_next-1.0.0b2/datalad_next/constraints/formats.py` & `datalad_next-1.0.0b3/datalad_next/constraints/formats.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     ParseResult,
 )
 
 from .base import Constraint
 
 
 class EnsureJSON(Constraint):
-    """Ensures that string is JSON formated and can be deserialized.
+    """Ensures that string is JSON formatted and can be deserialized.
     """
     def __init__(self):
         super().__init__()
 
     def __call__(self, value: str):
         try:
             return loads(value)
@@ -37,15 +37,15 @@
 
     and/or:
 
     - does not contain certain components
     - matches a particular regular expression
 
     Given that a large variety of strings are also a valid URL, a typical use
-    of this contraint would involve using a `required=['scheme']` setting.
+    of this constraint would involve using a `required=['scheme']` setting.
 
     All URL attribute names supported by `urllib.parse.urlparse()` are also
     supported here: scheme, netloc, path, params, query, fragment, username,
     password, hostname, port.
 
     .. seealso::
       https://docs.python.org/3/library/urllib.parse.html#urllib.parse.urlparse
```

### Comparing `datalad_next-1.0.0b2/datalad_next/constraints/git.py` & `datalad_next-1.0.0b3/datalad_next/constraints/git.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 """Constraints for Git-related concepts and parameters"""
 
+from datalad_next.runners import (
+    CommandError,
+    GitRunner,
+    StdOutCapture,
+)
+
 from .base import Constraint
 
 
 class EnsureGitRefName(Constraint):
     """Ensures that a reference name is well formed
 
-    Validation is peformed by calling `git check-ref-format`.
+    Validation is performed by calling `git check-ref-format`.
     """
     def __init__(self,
                  allow_onelevel: bool = True,
                  normalize: bool = True,
                  refspec_pattern: bool = False):
         """
         Parameters
@@ -31,18 +37,16 @@
         self._allow_onelevel = allow_onelevel
         self._normalize = normalize
         self._refspec_pattern = refspec_pattern
 
     def __call__(self, value: str) -> str:
         if not value:
             # simple, do here
-            raise ValueError('refname must not be empty')
+            self.raise_for(value, 'refname must not be empty')
 
-        from datalad.runner import GitRunner, StdOutCapture
-        from datalad_next.exceptions import CommandError
         runner = GitRunner()
         cmd = ['git', 'check-ref-format']
         cmd.append('--allow-onelevel'
                    if self._allow_onelevel
                    else '--no-allow-onelevel')
         if self._refspec_pattern:
             cmd.append('--refspec-pattern')
@@ -50,15 +54,19 @@
             cmd.append('--normalize')
 
         cmd.append(value)
 
         try:
             out = runner.run(cmd, protocol=StdOutCapture)
         except CommandError as e:
-            raise ValueError(f'{value} is not a valid refname') from e
+            self.raise_for(
+                value,
+                'is not a valid refname',
+                __caused_by__=e,
+            )
 
         if self._normalize:
             return out['stdout'].strip()
         else:
             return value
 
     def short_description(self):
```

### Comparing `datalad_next-1.0.0b2/datalad_next/constraints/parameter.py` & `datalad_next-1.0.0b3/datalad_next/constraints/parameter.py`

 * *Files 3% similar despite different names*

```diff
@@ -158,23 +158,34 @@
 
           _joint_validators_ = {
               ParameterConstraintContext(('p1', 'p2'), 'sum'):
                   MyValidator._check_sum,
           }
 
           def _checksum(self, p1, p2):
-              EnsureRange(min=3)(p1 + p2)
+              if (p1 + p2) < 3:
+                  self.raise_for(
+                     dict(p1=p1, p2=p2),
+                     'parameter sum is too large',
+                  )
 
         The callable will be passed the arguments named in the
         ``ParameterConstraintContext`` as keyword arguments, using the same
-        names as originally given to ``EnsureCommandParameterization``. Any
-        raised ``ConstraintError`` is caught and reported together with the
-        respective ``ParameterConstraintContext``. If the callable anyhow
-        modifies the passed arguments, it must return them as a kwargs-like
-        mapping.  If nothing is modified, it is OK to return ``None``.
+        names as originally given to ``EnsureCommandParameterization``.
+
+        Any raised ``ConstraintError`` is caught and reported together with the
+        respective ``ParameterConstraintContext``. The violating value reported
+        in such a ``ConstraintError`` must be a mapping of parameter name to
+        value, comprising the full parameter set (i.e., keys matching the
+        ``ParameterConstraintContext``).  The use of ``self.raise_for()`` is
+        encouraged.
+
+        If the callable anyhow modifies the passed arguments, it must return
+        them as a kwargs-like mapping.  If nothing is modified, it is OK to
+        return ``None``.
 
         Returns
         -------
         dict
           The returned dict must have a value for each item passed in via
           ``params``.
         on_error: {'raise-early', 'raise-at-end'}
@@ -204,14 +215,23 @@
                 # call the validator with the parameters given in the context
                 # and only with those, to make sure the context is valid
                 # and not an underspecification.
                 # pull the values form `validated` to be able to benefit
                 # from incremental coercing done in individual checks
                 res = validator(**{p: validated[p] for p in ctx.parameters})
             except ConstraintError as e:
+                if not isinstance(e.value, dict) \
+                        or set(ctx.parameters) != e.value.keys():  # pragma: no cover
+                    raise RuntimeError(
+                        'on raising a ConstraintError the joint validator '
+                        f'{validator} did not report '
+                        'a mapping of parameter name to (violating) value '
+                        'comprising all constraint context parameters. '
+                        'This is a software defect of the joint validator. '
+                        'Please report!')
                 exceptions[ctx] = e
                 if on_error == 'raise-early':
                     raise CommandParametrizationError(exceptions)
             if res is not None:
                 validated.update(**res)
 
         if exceptions:
@@ -219,27 +239,30 @@
 
         return validated
 
     def __call__(
         self,
         kwargs,
         at_default=None,
+        required=None,
         on_error='raise-early',
     ) -> Dict:
         """
         Parameters
         ----------
         kwargs: dict
           Parameter name (``str``)) to value (any) mapping of the parameter
           set.
         at_default: set or None
           Set of parameter names where the respective values in ``kwargs``
           match their respective defaults. This is used for deciding whether
           or not to process them with an associated value constraint (see the
           ``validate_defaults`` constructor argument).
+        required: set or None
+          Set of parameter names that are known to be required.
         on_error: {'raise-early', 'raise-at-end'}
           Flag how to handle constraint violation. By default, validation is
           stopped at the first error and an exception is raised. When an
           exhaustive validation is performed, an eventual exception contains
           information on all constraint violations. Regardless of this mode
           more than one error can be reported (in case (future) implementation
           perform independent validations in parallel).
@@ -249,14 +272,26 @@
         CommandParametrizationError
           Raised whenever one (or more) ``ConstraintError`` exceptions are
           caught during validation. Other exception types are not caught and
           pass through.
         """
         assert on_error in ('raise-early', 'raise-at-end')
 
+        exceptions = {}
+        missing_args = tuple(a for a in (required or []) if a not in kwargs)
+        if missing_args:
+            exceptions[ParameterConstraintContext(missing_args)] = \
+                ConstraintError(
+                    self,
+                    dict(zip(missing_args, [NoValue()] * len(missing_args))),
+                    'missing required arguments',
+                )
+            if on_error == 'raise-early':
+                raise CommandParametrizationError(exceptions)
+
         # validators to work with. make a copy of the dict to be able to tailor
         # them for this run only
         # TODO copy likely not needed
         param_constraints = self._param_constraints.copy()
 
         # names of parameters we need to process
         to_validate = set(kwargs)
@@ -266,15 +301,14 @@
         # to process them first.
         # the approach is to simply sort them first, but otherwise apply standard
         # handling
         to_validate.difference_update(ds_provider_params)
         # strip all args provider args that have not been provided
         ds_provider_params.intersection_update(kwargs)
 
-        exceptions = {}
         validated = {}
         # process all parameters. starts with those that are needed as
         # dependencies for others.
         # this dependency-based sorting is very crude for now. it does not
         # consider possible dependencies within `ds_provider_params` at all
         for argname in chain(ds_provider_params, to_validate):
             arg = kwargs[argname]
```

### Comparing `datalad_next-1.0.0b2/datalad_next/constraints/parameter_legacy.py` & `datalad_next-1.0.0b3/datalad_next/constraints/parameter_legacy.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         ----------
         spec: Parameter
           Instance of a datalad-core Parameter. If not overwritten by values
           given to the other arguments of this method, item constraints,
           number of arguments and other argparse-specific information
           is taken from this object and processed to built a comprehensive
           constraint that handles all aspects of the specification in a
-          homogenous fashion via the Constraint interface.
+          homogeneous fashion via the Constraint interface.
         default: Any
           A parameter's default value. It is configured as a "pass-through"
           value that will not be subjected to validation.
         item_constraint:
           If given, it override any constraint declared in the Parameter
           instance given to `spec`
         nargs:
@@ -162,15 +162,15 @@
             constraint = EnsureBool()
         elif param_spec.cmd_kwargs.get('choices'):
             constraint = EnsureChoice(*param_spec.cmd_kwargs.get('choices'))
         else:
             # always have one for simplicity
             constraint = NoConstraint()
 
-    # we must addtionally consider the following nargs spec for
+    # we must additionally consider the following nargs spec for
     # a complete constraint specification
     # (int, '*', '+'), plus action=
     # - 'store_const' TODO
     # - 'store_true' and 'store_false' TODO
     # - 'append'
     # - 'append_const' TODO
     # - 'count' TODO
```

### Comparing `datalad_next-1.0.0b2/datalad_next/constraints/tests/test_base.py` & `datalad_next-1.0.0b3/datalad_next/constraints/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.0.0b2/datalad_next/constraints/tests/test_basic.py` & `datalad_next-1.0.0b3/datalad_next/constraints/tests/test_basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,17 +294,16 @@
     with pytest.raises(ValueError):
         assert c(target.parent)
     c = EnsurePath(ref=target, ref_is='parent-of')
     assert c(target / 'some') == target / 'some'
     with pytest.raises(ValueError):
         assert c(target)
     assert c.short_description() == f'path that is parent-of {target}'
-    c = EnsurePath(ref=target, ref_is='stupid')
-    with pytest.raises(ValueError):
-        c('doesnotmatter')
+    with pytest.raises(AssertionError):
+        c = EnsurePath(ref=target, ref_is='stupid')
 
 
 def test_EnsurePath_fordataset(existing_dataset):
     P = pathlib.Path
     ds = existing_dataset
     # standard: relative in, relative out
     c = EnsurePath()
```

### Comparing `datalad_next-1.0.0b2/datalad_next/constraints/tests/test_cmdarg_validation.py` & `datalad_next-1.0.0b3/datalad_next/constraints/tests/test_cmdarg_validation.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,18 +65,30 @@
             ),
             **kwargs
         )
 
 
 class SophisticatedCmdValidator(BasicCmdValidator):
     def _check_unique_values(self, **kwargs):
-        EnsureAllUnique()(kwargs.values())
+        try:
+            EnsureAllUnique()(kwargs.values())
+        except ConstraintError as e:
+            self.raise_for(
+                kwargs,
+                e.msg,
+            )
 
     def _check_sum_range(self, p1, p2):
-        EnsureRange(min=3)(p1 + p2)
+        try:
+            EnsureRange(min=3)(p1 + p2)
+        except ConstraintError:
+            self.raise_for(
+                dict(p1=p1, p2=p2),
+                "it's too small"
+            )
 
     def _limit_sum_range(self, p1, p2):
         # random example of a joint constraint that modifies the parameter
         # set it is given
         return dict(p1=p1, p2=min(p2, 100 - p1 - p2))
 
     def __init__(self):
@@ -246,14 +258,23 @@
     # https://github.com/datalad/datalad/issues/7167
     with pytest.raises(ValueError):
         CmdWithValidation.__call__(
             'unsupported',
             return_type='item-or-list', result_renderer='disabled',
         )
 
+    # no call with a required argument missing
+    with pytest.raises(ValueError) as e:
+        CmdWithValidation.__call__()
+    exc_rendering = str(e.value)
+    # must label the issue correctly
+    assert 'missing required argument' in exc_rendering
+    # must identify the missing argument
+    assert 'spec=<no value>' in exc_rendering
+
 
 #
 # test dataset tailoring
 #
 
 class EnsureUUID(Constraint):
     def __call__(self, value):
```

### Comparing `datalad_next-1.0.0b2/datalad_next/constraints/tests/test_compound.py` & `datalad_next-1.0.0b3/datalad_next/constraints/tests/test_compound.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         EnsureIterableOf(list, bool, max_len=2)((1, 0, 1))
     with pytest.raises(ValueError):
         # too few items
         EnsureIterableOf(list, bool, min_len=4)((1, 0, 1))
     with pytest.raises(ValueError):
         # invalid specification min>max
         EnsureIterableOf(list, bool, min_len=1, max_len=0)
-    with pytest.raises(TypeError):
+    with pytest.raises(ValueError):
         # item_constraint fails
         EnsureIterableOf(list, dict)([5.6, 3.2])
     with pytest.raises(ValueError):
         # item_constraint fails
         EnsureIterableOf(list, EnsureBool())([5.6, 3.2])
 
     seq = [3.3, 1, 2.6]
```

### Comparing `datalad_next-1.0.0b2/datalad_next/constraints/tests/test_exceptions.py` & `datalad_next-1.0.0b3/datalad_next/constraints/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.0.0b2/datalad_next/constraints/tests/test_special_purpose.py` & `datalad_next-1.0.0b3/datalad_next/constraints/tests/test_special_purpose.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     # default is valid too
     assert c({'choice': None}) == dict(choice=None)
     # multi-item values
     c = EnsureParameterConstraint.from_parameter(
         Parameter(nargs=2),
         (None, None))
     assert c({'some': [3, 4]}) == dict(some=[3, 4])
-    with pytest.raises(TypeError):
+    with pytest.raises(ValueError):
         c({'some': 3})
     with pytest.raises(ValueError):
         c({'some': [3, 4, 5]})
     # one or more items
     c = EnsureParameterConstraint.from_parameter(
         Parameter(nargs='*'),
         None)
@@ -115,17 +115,17 @@
     assert c({'some': []}) == dict(some=[])
     assert c({'some': [[3, 2]]}) == dict(some=[[3, 2]])
     assert c({'some': [[3, 2], [5, 4]]}) == dict(some=[[3, 2], [5, 4]])
     # length mismatch
     with pytest.raises(ValueError):
         c({'some': [[3, 2], [1]]})
     # no iterable
-    with pytest.raises(TypeError):
+    with pytest.raises(ValueError):
         c({'some': [3, [1, 2]]})
-    with pytest.raises(TypeError):
+    with pytest.raises(ValueError):
         c({'some': 3})
     # overwrite an item constraint and nargs
     c = EnsureParameterConstraint.from_parameter(
         Parameter(nargs=2, constraints=EnsureInt(), action='append'),
         None,
         item_constraint=EnsureStr(),
         nargs=1)
@@ -293,15 +293,15 @@
             'https://s.kg.eb.eu/i/a8932c7e-063c-4131-ab96-996d843998e9',
             'ssh://4ac9f0bc-560d-47e0-8916-7b24da9bb0ce.com/home',
     ):
         c(url)
 
 
 def test_EnsureDataset(tmp_path):
-    with pytest.raises(TypeError):
+    with pytest.raises(ValueError):
         # will not return a Dataset from sensless input
         EnsureDataset()(5)
     # by default the installation state is not checked
     # this matches the behavior of the original implementation
     # from datalad-core
     assert EnsureDataset()(tmp_path).ds.pathobj == tmp_path
 
@@ -363,9 +363,9 @@
     # smoke test for idcheck:
     assert EnsureDataset(require_id=True)(ds).ds == ds
     assert EnsureDataset(require_id=False)(ds).ds == ds
     # unset the dataset ID to test whether an ID check would raise, but
     # bring it back later in case future tests need it
     id = ds.config.get('datalad.dataset.id')
     ds.config.unset('datalad.dataset.id', scope='branch')
-    with pytest.raises(NoDatasetFound):
+    with pytest.raises(ValueError):
         EnsureDataset(require_id=True)(tmp_path)
```

### Comparing `datalad_next-1.0.0b2/datalad_next/constraints/tests/test_tutorial.py` & `datalad_next-1.0.0b3/datalad_next/constraints/tests/test_tutorial.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.0.0b2/datalad_next/constraints/utils.py` & `datalad_next-1.0.0b3/datalad_next/constraints/utils.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.0.0b2/datalad_next/credman/manager.py` & `datalad_next-1.0.0b3/datalad_next/credman/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from typing import (
     Dict,
     List,
     Tuple,
 )
 
 import datalad
+from datalad_next.config import ConfigManager
 from datalad_next.exceptions import (
     CapturedException,
     CommandError,
 )
 from datalad_next.uis import ui_switcher as ui
 
 lgr = logging.getLogger('datalad.credman')
@@ -66,23 +67,23 @@
     properties from method parameters. The one exception is the ``name``
     parameter, which is used as a primary identifier (albeit being optional
     for some operations).
 
     The ``obtain()`` method is provided as an additional convenience, and
     implements a standard workflow for obtaining a credential in a wide variety
     of scenarios (credential name, credential properties, secret either
-    respectively already known or yet unkown).
+    respectively already known or yet unknown).
     """
     valid_property_names_regex = re.compile(r'[a-z0-9]+[a-z0-9-]*$')
 
     secret_names = {
         'user_password': 'password',
     }
 
-    def __init__(self, cfg=None):
+    def __init__(self, cfg: ConfigManager | None = None):
         """
 
         Parameters
         ----------
         cfg: ConfigManager, optional
           If given, all configuration queries are performed using this
           ``ConfigManager`` instance. Otherwise ``datalad.cfg`` is used.
@@ -591,15 +592,15 @@
                *,
                prompt: str | None = None,
                type_hint: str | None = None,
                query_props: Dict | None = None,
                expected_props: List | Tuple | None = None):
         """Obtain a credential by query or prompt (if needed)
 
-        This convienence method implements a standard workflow to obtain a
+        This convenience method implements a standard workflow to obtain a
         credential.  It supports credential selection by credential
         name/identifier, and falls back onto querying for a credential matching
         a set of specified properties (as key-value mappings). If no suitable
         credential is known, a user is prompted to enter one interactively (if
         possible in the current session).
 
         If a credential was entered manually, any given ``type_hint`` will
@@ -1038,15 +1039,15 @@
 
     # ATTN: from Providers.from_config_files() is sensitive to the PWD
     # it will only read legacy credentials from datasets whenever
     # PWD is inside a dataset
     legacy_credentials = set(
         (p.credential.name, type(p.credential))
         # without reload, no changes in files since the last call
-        # will be considered. That last call might have happended
+        # will be considered. That last call might have happened
         # in datalad-core, and may have been in another directory
         for p in Providers.from_config_files(reload=True)
         if p.credential
     )
     for name, type_ in legacy_credentials:
         yield (name, type_hints.get(type_))
```

### Comparing `datalad_next-1.0.0b2/datalad_next/credman/tests/test_credman.py` & `datalad_next-1.0.0b3/datalad_next/credman/tests/test_credman.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # ## ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ##
 """
 
 """
 import pytest
 
-from datalad.config import ConfigManager
+from datalad_next.config import ConfigManager
 from ..manager import (
     CredentialManager,
     _get_cred_cfg_var,
 )
 from datalad_next.tests.utils import (
     assert_in,
     assert_raises,
```

### Comparing `datalad_next-1.0.0b2/datalad_next/gitremotes/datalad_annex.py` & `datalad_next-1.0.0b3/datalad_next/gitremotes/datalad_annex.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,27 +193,26 @@
 from unittest.mock import patch
 from urllib.parse import (
     unquote,
     urlparse,
 )
 
 from datalad.core.local.repo import repo_from_path
-from datalad.runner import (
-    NoCapture,
-    StdOutCapture,
-)
+
+from datalad_next.constraints import EnsureInt
 from datalad_next.datasets import (
     LegacyAnnexRepo as AnnexRepo,
     LegacyGitRepo as GitRepo,
 )
-from datalad_next.exceptions import (
-    CapturedException,
+from datalad_next.exceptions import CapturedException
+from datalad_next.runners import (
     CommandError,
+    NoCapture,
+    StdOutCapture,
 )
-from datalad_next.constraints import EnsureInt
 from datalad_next.uis import ui_switcher as ui
 from datalad_next.utils import (
     external_versions,
     on_windows,
     rmtree,
 )
 
@@ -608,14 +607,24 @@
         # (re-)create an instance
         mr = GitRepo(
             self._mirrorrepodir,
             # if the remote had no refs, there would still be no repo
             create=not existing_repo,
             bare=True)
 
+        if not existing_repo:
+            # align HEAD symbolic ref between source and mirror repo
+            # IF WE CREATED IT LOCALLY JUST NOW, otherwise take whatever
+            # we got.
+            # otherwise we can end up in a conflict situation where the mirror
+            # points to 'master' (or something else) and the source actually
+            # has 'main' (or something different)
+            src_head_ref = self.repo.call_git(['symbolic-ref', 'HEAD']).strip()
+            mr.call_git(['symbolic-ref', 'HEAD', src_head_ref])
+
         self.log('Established mirror')
         self._mirrorrepo = mr
         return mr
 
     def log(self, *args, level=2):
         """Send log messages to the errstream"""
         # A value of 0 for <n> means that processes operate quietly,
@@ -671,17 +680,17 @@
                     # the mirror is out-of-sync with the remote (could be a
                     # slightly more expensive test)
                     # we must upload it.
                     try:
                         self.replace_remote_deposit_from_mirrorrepo()
                     except Exception:
                         # the bad thing is that we have no way of properly
-                        # signaling to git that this happended,
+                        # signaling to git that this happened,
                         # the refs for this remote will look as if the upload
-                        # was successfull
+                        # was successful
 
                         # we do not need to roll-back the refs in the
                         # mirrorrepo as it will be rsync'ed to the remote on
                         # next access
                         self.log('Remote update failed, flagging refs',
                                  post_refs)
                         for ref in post_refs:
@@ -708,15 +717,15 @@
                 self._store_credential()
                 return
             elif line == 'connect git-upload-pack\n':
                 self.log('Connecting git-upload-pack\n')
                 self.send('\n')
                 # must not capture -- git is talking to it directly from here.
                 # the `self.mirrorrepo` access will ensure that the mirror
-                # is uptodate
+                # is up-to-date
                 self.mirrorrepo._git_runner.run(
                     ['git', 'upload-pack', self.mirrorrepo.path],
                     protocol=NoCapture,
                 )
                 # everything has worked, if we used a credential, update it
                 self._store_credential()
                 return
@@ -887,23 +896,35 @@
         if self._mirrorrepodir.exists():
             # if we extract, we cannot tollerate left-overs
             rmtree(str(self._mirrorrepodir), ignore_errors=True)
             # null the repohandle to be reconstructed later on-demand
             self._mirrorrepo = None
 
         self.log('Extracting repository archive')
+        legacy_deposit = False
         with zipfile.ZipFile(repoexportkeyloc) as zip:
+            try:
+                zip.getinfo('repo/')
+                legacy_deposit = True
+                safe_content = [f'repo/{i}' for i in self.safe_content]
+            except KeyError:
+                safe_content = self.safe_content
+
             zip.extractall(
                 self._mirrorrepodir,
                 # a bit of a safety-net, exclude all unexpected content
                 members=[
                     m for m in zip.namelist()
                     if any(m.startswith(prefix)
-                           for prefix in self.safe_content)],
+                           for prefix in safe_content)],
             )
+        if legacy_deposit:
+            legacy_basedir = self._mirrorrepodir / 'repo'
+            for p in legacy_basedir.iterdir():
+                p.rename(self._mirrorrepodir / p.relative_to(legacy_basedir))
 
     def get_remote_refs(self):
         """Report remote refs
 
         The underlying special remote is asked whether it has the key
         containing the refs list for the remote. If it does, it is retrieved
         and reported.
@@ -1211,19 +1232,19 @@
     error_operations = (
         'no-match', 'rejected', 'remote-rejected', 'remote-failure',
         'error',
     )
     return any(o in operations for o in error_operations)
 
 
-def main():
+def main(gitremote_cls=RepoAnnexGitRemote):
     """git-remote helper executable entrypoint"""
     try:
         if len(sys.argv) < 3:
-            raise ValueError("Usage: git-remote-datalad-annex REMOTE-NAME URL")
+            raise ValueError(f"Usage: {sys.argv[0]} REMOTE-NAME URL")
 
         remote, url = sys.argv[1:3]
         # provided by Git
         gitdir = os.environ.pop('GIT_DIR')
         # no fallback, must be present
         if gitdir is None:
             raise RuntimeError('GIT_DIR environment variable not defined')
@@ -1232,15 +1253,15 @@
         # the 'annex' backend really doesn't do much annex-specific
         # albeit maybe progress reporting (unclear to MIH right now)
         # but it does make credential entry possible here, despite the
         # remote helper process being connected to Git with its stdin/stdout
         ui.set_backend('annex')
 
         # lock and load
-        remote = RepoAnnexGitRemote(gitdir, remote, url)
+        remote = gitremote_cls(gitdir, remote, url)
         remote.communicate()
         # there is no value in keeping around the downloads
         # we either have things in the mirror repo or have to
         # redownload anyways
         # leaving the table clean and always bootstrap from scratch
         # has the advantage that we always automatically react to any
         # git-remote reconfiguration between runs
```

### Comparing `datalad_next-1.0.0b2/datalad_next/gitremotes/tests/test_datalad_annex.py` & `datalad_next-1.0.0b3/datalad_next/gitremotes/tests/test_datalad_annex.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,15 +210,15 @@
 
     # wipe out the remote
     rmtree(remotepath)
     assert not remotepath.exists()
     remotepath.mkdir(parents=True)
 
     # helper must detect the discrepancy and re-push, despite the local mirror
-    # repo already being uptodate
+    # repo already being up-to-date
     dsrepo.call_git(['push', 'dla'])
     eq_dla_branch_state(dsrepo.get_hexsha(DEFAULT_BRANCH), remotepath)
 
 
 def test_params_from_url():
     f = get_initremote_params_from_url
     # just the query part being used
```

### Comparing `datalad_next-1.0.0b2/datalad_next/patches/annexrepo.py` & `datalad_next-1.0.0b3/datalad_next/patches/annexrepo.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     CredentialManager,
     ensure_list,
     get_specialremote_credential_envpatch,
     get_specialremote_param_dict,
     get_specialremote_credential_properties,
     needs_specialremote_credential_envpatch,
 )
-from datalad_next.utils.patch import apply_patch
+from . import apply_patch
 
 
 # reuse logger from -core, despite the unconventional name
 lgr = logging.getLogger('datalad.annex')
 
 
 # This function is taken from datalad-core@2ed709613ecde8218a215dcb7d74b4a352825685
```

### Comparing `datalad_next-1.0.0b2/datalad_next/patches/configuration.py` & `datalad_next-1.0.0b3/datalad_next/patches/configuration.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.0.0b2/datalad_next/patches/create_sibling_ghlike.py` & `datalad_next-1.0.0b3/datalad_next/patches/create_sibling_ghlike.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 candidates of suitable credentials without having to specific
 their name, similar to a request context url used by the old
 providers setup.
 
 This automatic realm-based credential lookup is now also implemented.
 When no credential name is specified, the most recently used
 credential matching the API realm will be used automatically.
-If determined like this, it will be tested for successfull
+If determined like this, it will be tested for successful
 authorization, and will then be stored again with an updated
 ``last-used`` timestamp.
 """
 
 import logging
 from urllib.parse import urlparse
```

### Comparing `datalad_next-1.0.0b2/datalad_next/patches/distribution_dataset.py` & `datalad_next-1.0.0b3/datalad_next/patches/distribution_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 This patch ensure the traditional handling of "dataset instance from
 a string-type parameter in this context.
 """
 
 import logging
 
-from datalad_next.utils.patch import apply_patch
+from . import apply_patch
 
 # use same logger as -core, looks weird but is correct
 lgr = logging.getLogger('datalad.dataset')
 
 
 def resolve_path(path, ds=None, ds_resolved=None):
     if hasattr(ds, 'auto_instance_from_path'):
```

### Comparing `datalad_next-1.0.0b2/datalad_next/patches/interface_utils.py` & `datalad_next-1.0.0b3/datalad_next/patches/interface_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     get_result_filter,
     keep_result,
     render_action_summary,
     xfm_result,
     _process_results,
 )
 from datalad_next.exceptions import IncompleteResultsError
-from datalad_next.utils.patch import apply_patch
+from . import apply_patch
 from datalad_next.constraints.dataset import DatasetParameter
 
 # use same logger as -core
 lgr = logging.getLogger('datalad.interface.utils')
 
 
 # this is a replacement for datalad.interface.base.get_allargs_as_kwargs
@@ -46,20 +46,22 @@
 
     Basically resolving the argnames for all positional arguments, and
     resolving the defaults for all kwargs that are not given in a kwargs
     dict
 
     Returns
     -------
-    (dict, set)
+    (dict, set, set)
       The first return value is a mapping of argument names to their respective
       values.
       The second return value in the tuple is a set of argument names for
       which the effective value is identical to the default declared in the
       signature of the callable.
+      The third value is a set with names of all mandatory arguments, whether
+      or not they are included in the returned mapping.
     """
     from datalad_next.utils import getargspec
     argspec = getargspec(call, include_kwonlyargs=True)
     defaults = argspec.defaults
     nargs = len(argspec.args)
     defaults = defaults or []  # ensure it is a list and not None
     assert (nargs >= len(defaults))
@@ -79,15 +81,22 @@
         k for k in kwargs_
         if k in default_map and default_map[k] == kwargs_[k]
     )
     # XXX we cannot assert the following, because our own highlevel
     # API commands support more kwargs than what is discoverable
     # from their signature...
     #assert (nargs == len(kwargs_))
-    return kwargs_, at_default
+    return (
+        # argument name/value mapping
+        kwargs_,
+        # names of arguments that are at their default
+        at_default,
+        # names of mandatory arguments (set for uniformity)
+        set(argspec.args),
+    )
 
 
 # This function interface is taken from
 # datalad-core@209bc319db8f34cceae4fee86493bf41927676fd
 def _execute_command_(
     *,
     interface: anInterface,
@@ -112,15 +121,15 @@
     exec_kwargs:
       Keyword argument affecting the result handling.
       See `datalad.interface.common_opts.eval_params`.
     """
     # for result filters and validation
     # we need to produce a dict with argname/argvalue pairs for all args
     # incl. defaults and args given as positionals
-    allkwargs, at_default = get_allargs_as_kwargs(
+    allkwargs, at_default, required_args = get_allargs_as_kwargs(
         cmd,
         cmd_args,
         {**cmd_kwargs, **exec_kwargs},
     )
 
     # validate the complete parameterization
     param_validator = interface.get_parameter_validator() \
@@ -129,14 +138,15 @@
         lgr.debug(
             'Command parameter validation skipped. %s declares no validator',
             interface)
     else:
         lgr.debug('Command parameter validation for %s', interface)
         validator_kwargs = dict(
             at_default=at_default,
+            required=required_args or None,
         )
         # make immediate vs exhaustive parameter validation
         # configurable
         raise_on_error = dlcfg.get(
             'datalad.runtime.parameter-violation', None)
         if raise_on_error:
             validator_kwargs['on_error'] = raise_on_error
@@ -278,14 +288,9 @@
             failed=incomplete_results,
             msg="Command did not complete successfully")
 
 
 # apply patch
 patch_msg = \
     'Apply datalad-next patch to interface.(utils|base).py:_execute_command_'
-try:
-    apply_patch('datalad.interface.utils', None, '_execute_command_',
-                _execute_command_, msg=patch_msg)
-except AttributeError:
-    # we have datalad 0.17.10+ and the target has moved
-    apply_patch('datalad.interface.base', None, '_execute_command_',
-                _execute_command_, msg=patch_msg)
+apply_patch('datalad.interface.base', None, '_execute_command_',
+            _execute_command_, msg=patch_msg)
```

### Comparing `datalad_next-1.0.0b2/datalad_next/patches/push_optimize.py` & `datalad_next-1.0.0b3/datalad_next/patches/push_optimize.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,24 +39,23 @@
 """
 
 from itertools import chain
 import logging
 import re
 
 import datalad.core.distributed.push as mod_push
-from datalad.runner.exception import CommandError
 from datalad_next.utils import (
     ensure_list,
     log_progress,
 )
 from datalad_next.datasets import (
     LegacyAnnexRepo as AnnexRepo,
     Dataset,
 )
-from datalad_next.utils.patch import apply_patch
+from . import apply_patch
 
 
 lgr = logging.getLogger('datalad.core.distributed.push')
 
 
 def _push(dspath, content, target, data, force, jobs, res_kwargs, pbars,
           got_path_arg=False):
@@ -436,15 +435,15 @@
                 'availability update.')
         repo.call_git(fetch_cmd)
         # If no CommandError was raised, it means that remote has git-annex
         # but local repo might not be an annex yet. Since there is nothing to "sync"
         # from us, we just skip localsync without mutating repo into an AnnexRepo
         if is_annex_repo:
             repo.localsync(target)
-    except CommandError as e:
+    except mod_push.CommandError as e:
         # it is OK if the remote doesn't have a git-annex branch yet
         # (e.g. fresh repo)
         # TODO is this possible? we just copied? Maybe check if anything
         # was actually copied?
         if "fatal: couldn't find remote ref git-annex" not in e.stderr.lower():
             raise
         lgr.debug('Remote does not have a git-annex branch: %s', e)
```

### Comparing `datalad_next-1.0.0b2/datalad_next/patches/push_to_export_remote.py` & `datalad_next-1.0.0b3/datalad_next/patches/push_to_export_remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,29 +14,28 @@
     Iterable,
     Optional,
     Union,
 )
 from unittest.mock import patch
 
 import datalad.core.distributed.push as mod_push
-from datalad.runner.exception import CommandError
 from datalad_next.constraints import EnsureChoice
 from datalad_next.exceptions import CapturedException
 from datalad_next.commands import Parameter
 from datalad_next.datasets import (
     LegacyAnnexRepo as AnnexRepo,
     Dataset,
 )
 from datalad_next.utils import (
     CredentialManager,
     get_specialremote_credential_envpatch,
     get_specialremote_credential_properties,
     needs_specialremote_credential_envpatch,
 )
-from datalad_next.utils.patch import apply_patch
+from . import apply_patch
 
 
 lgr = logging.getLogger('datalad.core.distributed.push')
 
 
 def _is_export_remote(remote_info: Optional[Dict]) -> bool:
     """Check if remote_info is valid and has exporttree set to "yes"
@@ -107,15 +106,15 @@
                     "destination-annex-uuid",
                     "treeish"
                 ],
                 line.replace(":", " ").split()
             ))
             result_dict["timestamp"] = float(result_dict["timestamp"][:-1])
             yield result_dict
-    except CommandError as command_error:
+    except mod_push.CommandError as command_error:
         # Some errors indicate that there was no export yet.
         # May depend on Git version
         expected_errors = (
             "fatal: Not a valid object name git-annex:export.log",
             "fatal: path 'export.log' does not exist in 'git-annex'", # v2.36
         )
         if command_error.stderr.strip() in expected_errors:
@@ -238,15 +237,15 @@
                     annexjson2result(result, ds, **res_kwargs)
                 # annexjson2result overwrites 'action' with annex' 'command',
                 # even if we provided our 'action' within res_kwargs. Therefore,
                 # change afterwards instead:
                 result_adjusted['action'] = "copy"
                 yield result_adjusted
 
-        except CommandError as cmd_error:
+        except mod_push.CommandError as cmd_error:
             ce = CapturedException(cmd_error)
             yield {
                 **res_kwargs,
                 "action": "copy",
                 "status": "error",
                 "message": str(ce),
                 "exception": ce
```

### Comparing `datalad_next-1.0.0b2/datalad_next/patches/siblings.py` & `datalad_next-1.0.0b3/datalad_next/patches/siblings.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from datalad_next.datasets import LegacyAnnexRepo as AnnexRepo
 from datalad.support.exceptions import (
     AccessDeniedError,
     AccessFailedError,
     CapturedException,
 )
-from datalad_next.utils.patch import apply_patch
+from . import apply_patch
 
 
 # use same logger as -core
 lgr = logging.getLogger('datalad.distribution.siblings')
 
 
 # This function is taken from datalad-core@2ed709613ecde8218a215dcb7d74b4a352825685
```

### Comparing `datalad_next-1.0.0b2/datalad_next/patches/test_keyring.py` & `datalad_next-1.0.0b3/datalad_next/patches/test_keyring.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.0.0b2/datalad_next/patches/tests/test_configuration.py` & `datalad_next-1.0.0b3/datalad_next/patches/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.0.0b2/datalad_next/patches/tests/test_create_sibling_ghlike.py` & `datalad_next-1.0.0b3/datalad_next/patches/tests/test_create_sibling_ghlike.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.0.0b2/datalad_next/patches/tests/test_push.py` & `datalad_next-1.0.0b3/datalad_next/patches/tests/test_push.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.0.0b2/datalad_next/patches/tests/test_push_to_export_remote.py` & `datalad_next-1.0.0b3/datalad_next/patches/tests/test_push_to_export_remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 from typing import Generator
 from unittest.mock import (
     MagicMock,
     call,
     patch,
 )
 
-from datalad.runner.exception import CommandError
 from datalad_next.tests.utils import (
     SkipTest,
     assert_in,
     assert_in_results,
     eq_,
 )
 
 from datalad_next.patches.push_to_export_remote import (
     _get_export_log_entry,
     _is_export_remote,
     _is_valid_treeish,
     _transfer_data,
     get_export_records,
+    mod_push,
 )
 
 
 module_name = "datalad_next.patches.push_to_export_remote"
 
 
 class MockRepo:
@@ -172,15 +172,15 @@
         tuple(_call_transfer("no-target", False, False))
         eq_(pd_mock.call_count, 1)
 
 
 def test_get_export_records_no_exports():
     class NoExportRepo:
         def call_git_items_(self, *args, **kwargs):
-            raise CommandError(
+            raise mod_push.CommandError(
                 stderr="fatal: Not a valid object name git-annex:export.log")
 
     results = tuple(get_export_records(NoExportRepo()))
     eq_(results, ())
 
 
 def test_get_export_records():
```

### Comparing `datalad_next-1.0.0b2/datalad_next/tests/fixtures.py` & `datalad_next-1.0.0b3/datalad_next/tests/fixtures.py`

 * *Files 4% similar despite different names*

```diff
@@ -283,38 +283,38 @@
         # overwrite path with Path object for convenience
         server.path = path
         yield server
 
 
 @pytest.fixture(autouse=False, scope="function")
 def http_server_with_basicauth(tmp_path_factory, http_credential):
-    """Like ``http_server`` but requiering authenticat with ``http_credential``
+    """Like ``http_server`` but requiring authenticat with ``http_credential``
     """
     path = tmp_path_factory.mktemp("webdav")
     server = HTTPPath(
         path, use_ssl=False,
         auth=(http_credential['user'], http_credential['secret']),
     )
     with server:
         # overwrite path with Path object for convenience
         server.path = path
         yield server
 
 
 @pytest.fixture(scope="session")
-def httpbin():
-    """Return cannonical access URLs for the HTTPBIN service
+def httpbin_service():
+    """Return canonical access URLs for the HTTPBIN service
 
     This fixture tries to spin up a httpbin Docker container at localhost:8765;
     if successful, it returns this URL as the 'standard' URL.  If the attempt
-    fails, a URL pointing to the cannonical instance is returned.
+    fails, a URL pointing to the canonical instance is returned.
 
     For tests that need to have the service served via a specific
     protocol (https vs http), the corresponding URLs are returned
-    too. They always point to the cannonical deployment, as some
+    too. They always point to the canonical deployment, as some
     tests require both protocols simultaneously and a local deployment
     generally won't have https.
     """
     hburl = 'http://httpbin.org'
     hbsurl = 'https://httpbin.org'
     ciurl = 'http://localhost:8765'
     if os.name == "posix":
@@ -348,7 +348,26 @@
             "standard": ciurl if container_id is not None else hbsurl,
             "http": hburl,
             "https": hbsurl,
         }
     finally:
         if container_id is not None:
             subprocess.run(["docker", "rm", "-f", container_id], check=True)
+
+
+@pytest.fixture(scope="function")
+def httpbin(httpbin_service):
+    """Does the same thing as ``httpbin_service``, but skips on function-scope
+
+    ``httpbin_service`` always returns access URLs for HTTPBIN. However,
+    in some cases it is simply not desirable to run a test. For example,
+    the appveyor workers are more or less constantly unable to access the
+    public service. This fixture is evaluated at function-scope and
+    raises ``SkipTest`` whenever any of these undesired conditions is
+    detected. Otherwise it just relays ``httpbin_service``.
+    """
+    if 'APPVEYOR' in os.environ and 'DEPLOY_HTTPBIN_IMAGE' not in os.environ:
+        raise SkipTest(
+            "Not running httpbin-based test on appveyor without "
+            "docker-deployed instance -- too unreliable"
+        )
+    yield httpbin_service
```

### Comparing `datalad_next-1.0.0b2/datalad_next/tests/utils.py` & `datalad_next-1.0.0b3/datalad_next/tests/utils.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.0.0b2/datalad_next/url_operations/__init__.py` & `datalad_next-1.0.0b3/datalad_next/url_operations/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,20 @@
 from pathlib import Path
 from typing import (
     Any,
     Dict,
 )
 
 import datalad
+from datalad_next.config import ConfigManager
 from datalad_next.utils import log_progress
+from datalad_next.utils.multihash import (
+    MultiHash,
+    NoOpHash,
+)
 
 lgr = logging.getLogger('datalad.ext.next.url_operations')
 
 
 class UrlOperations:
     """Abstraction for operations on URLs
 
@@ -27,26 +32,26 @@
 
     - When downloads are to be supported, implement the `download()` method
       and comply with the behavior described in its documentation.
 
     This class provides a range of helper methods to aid computation of
     hashes and progress reporting.
     """
-    def __init__(self, *, cfg=None):
+    def __init__(self, *, cfg: ConfigManager | None = None):
         """
         Parameters
         ----------
         cfg: ConfigManager, optional
           A config manager instance that implementations will consult for
           any configuration items they may support.
         """
         self._cfg = cfg
 
     @property
-    def cfg(self):
+    def cfg(self) -> ConfigManager:
 
         if self._cfg is None:
             self._cfg = datalad.cfg
         return self._cfg
 
     def stat(self,
              url: str,
@@ -315,36 +320,17 @@
 
     def _progress_report_stop(self, pid: str, log_msg: tuple):
         log_progress(
             lgr.info, pid, *log_msg,
             noninteractive_level=logging.DEBUG,
         )
 
-    def _get_hasher(self, hash: list[str] | None) -> list[callable]:
-        if not hash:
-            return []
-
-        import hashlib
-        # yes, this will crash, if an invalid hash algorithm name
-        # is given
-        _hasher = []
-        for h in hash:
-            hr = getattr(hashlib, h.lower(), None)
-            if hr is None:
-                raise ValueError(f'unsupported hash algorithm {h}')
-            _hasher.append(hr())
-        return _hasher
-
-    def _get_hash_report(self,
-                         hash_names: list[str] | None,
-                         hashers: list) -> Dict:
-        if not hash_names:
-            return {}
-        else:
-            return dict(zip(hash_names, [h.hexdigest() for h in hashers]))
+    def _get_hasher(self, hash: list[str] | None) -> NoOpHash | MultiHash:
+        return MultiHash(hash) if hash is not None else NoOpHash()
+
 
 #
 # Exceptions to be used by all handlers
 #
 
 
 class UrlOperationsRemoteError(Exception):
```

### Comparing `datalad_next-1.0.0b2/datalad_next/url_operations/any.py` & `datalad_next-1.0.0b3/datalad_next/url_operations/any.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from importlib import import_module
 import json
 import logging
 from pathlib import Path
 import re
 from typing import Dict
 
+from datalad_next.config import ConfigManager
 from datalad_next.exceptions import CapturedException
 
 from . import UrlOperations
 
 lgr = logging.getLogger('datalad.ext.next.url_operations.any')
 
 
@@ -55,15 +56,15 @@
     Parameter identity and semantics are unchanged with respect to the
     underlying implementations. See their documentation for details.
 
     An instance retains and reuses URL scheme handler instances for subsequent
     operations, such that held connections or cached credentials can be reused
     efficiently.
     """
-    def __init__(self, cfg=None):
+    def __init__(self, cfg: ConfigManager | None = None):
         """
         Parameters
         ----------
         cfg: ConfigManager, optional
           A config manager instance that is consulted for any configuration
           filesystem configuration individual handlers may support.
         """
```

### Comparing `datalad_next-1.0.0b2/datalad_next/url_operations/file.py` & `datalad_next-1.0.0b3/datalad_next/url_operations/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,18 +246,17 @@
                 if not chunk:
                     break
                 dst_fp_write(chunk)
                 chunk_size = len(chunk)
                 self._progress_report_update(
                     progress_id, update_log, chunk_size)
                 # compute hash simultaneously
-                for h in hasher:
-                    h.update(chunk)
+                hasher.update(chunk)
                 copy_size += chunk_size
-            props.update(self._get_hash_report(hash, hasher))
+            props.update(hasher.get_hexdigest())
             # return how much was copied. we could compare with
             # `expected_size` and error on mismatch, but not all
             # sources can provide that (e.g. stdin)
             props['content-length'] = copy_size
             return props
         finally:
             self._progress_report_stop(progress_id, finish_log)
```

### Comparing `datalad_next-1.0.0b2/datalad_next/url_operations/http.py` & `datalad_next-1.0.0b3/datalad_next/url_operations/http.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 import logging
 from pathlib import Path
 import sys
 from typing import Dict
 import requests
 from requests_toolbelt import user_agent
-from requests_toolbelt.downloadutils.tee import tee as requests_tee
 import www_authenticate
 
 import datalad
 
 from datalad_next.utils.requests_auth import DataladAuth
 from . import (
     UrlOperations,
@@ -32,21 +31,36 @@
 
     This handler is built on the `requests` package. For authentication, it
     employes :class:`datalad_next.utils.requests_auth.DataladAuth`, an adaptor
     that consults the DataLad credential system in order to fulfill HTTP
     authentication challenges.
     """
 
-    _headers = {
-        'user-agent': user_agent('datalad', datalad.__version__),
-    }
+    def __init__(self, cfg=None, headers: Dict | None = None):
+        """
+        Parameters
+        ----------
+        cfg: ConfigManager, optional
+          A config manager instance that is consulted for any configuration
+          filesystem configuration individual handlers may support.
+        headers: dict, optional
+          Additional or alternative headers to add to a request. The default
+          headers contain a ``user-agent`` declaration. Any headers provided
+          here override corresponding defaults.
+        """
+        super().__init__(cfg=cfg)
+        self._headers = {
+            'user-agent': user_agent('datalad', datalad.__version__),
+        }
+        if headers:
+            self._headers.update(headers)
 
     def get_headers(self, headers: Dict | None = None) -> Dict:
         # start with the default
-        hdrs = dict(HttpUrlOperations._headers)
+        hdrs = dict(self._headers)
         if headers is not None:
             hdrs.update(headers)
         return hdrs
 
     def stat(self,
              url: str,
              *,
@@ -99,15 +113,15 @@
             context=f"for accessing {url}"
         )
         if 'content-length' in props:
             # make an effort to return size in bytes as int
             try:
                 props['content-length'] = int(props['content-length'])
             except (TypeError, ValueError):
-                # but be resonably robust against unexpected responses
+                # but be reasonably robust against unexpected responses
                 pass
         return props
 
     def download(self,
                  from_url: str,
                  to_path: Path | None,
                  *,
@@ -228,34 +242,59 @@
     def _stream_download_from_request(
             self, r, to_path, hash: list[str] | None = None) -> Dict:
         from_url = r.url
         hasher = self._get_hasher(hash)
         progress_id = self._get_progress_id(from_url, to_path)
         # get download size, but not every server provides it
         try:
+            # for compressed downloads the content length refers to the
+            # compressed content
             expected_size = int(r.headers.get('content-length'))
         except (ValueError, TypeError):
+            # some responses do not have a `content-length` header,
+            # even though they HTTP200 and deliver the content.
+            # example:
+            # https://github.com/datalad/datalad-next/pull/365#issuecomment-1557114109
             expected_size = None
         self._progress_report_start(
             progress_id,
             ('Download %s to %s', from_url, to_path),
             'downloading',
+            # can be None, and that is OK
             expected_size,
         )
 
         fp = None
         props = {}
         try:
+            # we can only write to file-likes opened in bytes mode
             fp = sys.stdout.buffer if to_path is None else open(to_path, 'wb')
-            # TODO make chunksize a config item
-            for chunk in requests_tee(r, fp):
+            # we need to track how much came down the pipe for progress
+            # reporting
+            downloaded_bytes = 0
+            # TODO make chunksize a config item, 65536 is the default in
+            # requests_toolbelt
+            for chunk in r.raw.stream(amt=65536, decode_content=True):
+                # update how much data was transferred from the remote server,
+                # but we cannot use the size of the chunk for that,
+                # because content might be downloaded with transparent
+                # (de)compression. ask the download stream itself for its
+                # "position"
+                if expected_size:
+                    tell = r.raw.tell()
+                else:
+                    tell = downloaded_bytes + len(chunk)
                 self._progress_report_update(
-                    progress_id, ('Downloaded chunk',), len(chunk))
+                    progress_id,
+                    ('Downloaded chunk',),
+                    tell - downloaded_bytes,
+                )
+                fp.write(chunk)
+                downloaded_bytes = tell
                 # compute hash simultaneously
-                for h in hasher:
-                    h.update(chunk)
-            props.update(self._get_hash_report(hash, hasher))
+                hasher.update(chunk)
+            props.update(hasher.get_hexdigest())
             return props
         finally:
             if fp and to_path is not None:
                 fp.close()
             self._progress_report_stop(progress_id, ('Finished download',))
```

### Comparing `datalad_next-1.0.0b2/datalad_next/url_operations/ssh.py` & `datalad_next-1.0.0b3/datalad_next/url_operations/ssh.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,22 +19,23 @@
     Any,
     Dict,
     Generator,
     IO,
 )
 from urllib.parse import urlparse
 
-from datalad.runner.protocol import WitlessProtocol
-from datalad.runner.coreprotocols import NoCapture
-
-from datalad.runner import StdOutCapture
-from datalad.runner.protocol import GeneratorMixIn
-from datalad.runner.nonasyncrunner import ThreadedRunner
+from datalad_next.runners import (
+    GeneratorMixIn,
+    NoCaptureGeneratorProtocol,
+    Protocol as RunnerProtocol,
+    StdOutCaptureGeneratorProtocol,
+    ThreadedRunner,
+    CommandError,
+)
 
-from datalad_next.exceptions import CommandError
 from datalad_next.utils.consts import COPY_BUFSIZE
 
 from . import (
     UrlOperations,
     UrlOperationsRemoteError,
     UrlOperationsResourceUnknown,
 )
@@ -59,15 +60,15 @@
        likely to be removed in the future, and connection multiplexing
        supported where possible (non-Windows platforms).
     """
     # first try ls'ing the path, and catch a missing path with a dedicated 244
     # exit code, to be able to distinguish the original exit=2 that ls-call
     # from a later exit=2 from awk in case of a "fatal error".
     # when executed through ssh, only a missing file would yield 244, while
-    # a conenction error or other problem unrelated to the present of a file
+    # a connection error or other problem unrelated to the present of a file
     # would a different error code (255 in case of a connection error)
     _stat_cmd = "printf \"\1\2\3\"; ls '{fpath}' &> /dev/null " \
                 "&& ls -nl '{fpath}' | awk 'BEGIN {{ORS=\"\1\"}} {{print $5}}' " \
                 "|| exit 244"
     _cat_cmd = "cat '{fpath}'"
 
     def stat(self,
@@ -101,15 +102,15 @@
         # to-be-downloaded file in bytes, followed by another magic
         # b'\1', and the file content after that
         need_magic = b'\1\2\3'
         expected_size_str = b''
         expected_size = None
 
         ssh_cat = _SshCat(url)
-        stream = ssh_cat.run(cmd, protocol=_StdOutCaptureGeneratorProtocol)
+        stream = ssh_cat.run(cmd, protocol=StdOutCaptureGeneratorProtocol)
         for chunk in stream:
             if need_magic:
                 expected_magic = need_magic[:min(len(need_magic),
                                                  len(chunk))]
                 incoming_magic = chunk[:len(need_magic)]
                 # does the incoming data have the remaining magic bytes?
                 if incoming_magic != expected_magic:
@@ -181,19 +182,18 @@
                 'downloading',
                 expected_size,
             )
             for chunk in stream:
                 # write data
                 dst_fp_write(chunk)
                 # compute hash simultaneously
-                for h in hasher:
-                    h.update(chunk)
+                hasher.update(chunk)
                 self._progress_report_update(
                     progress_id, ('Downloaded chunk',), len(chunk))
-            props.update(self._get_hash_report(hash, hasher))
+            props.update(hasher.get_hexdigest())
             return props
         except CommandError as e:
             if e.code == 244:
                 # this is the special code for a file-not-found
                 raise UrlOperationsResourceUnknown(from_url) from e
             else:
                 # wrap this into the datalad-standard, but keep the
@@ -258,15 +258,15 @@
         upload_queue = Queue(maxsize=2)
 
         ssh_cat = _SshCat(to_url)
         ssh_runner_generator = ssh_cat.run(
             # leave special exit code when writing fails, but not the
             # general SSH access
             "( mkdir -p '{fdir}' && cat > '{fpath}' ) || exit 244",
-            protocol=_NoCaptureGeneratorProtocol,
+            protocol=NoCaptureGeneratorProtocol,
             stdin=upload_queue,
             timeout=timeout,
         )
 
         # file is open, we can start progress tracking
         progress_id = self._get_progress_id(source_name, to_url)
         self._progress_report_start(
@@ -279,16 +279,15 @@
             upload_size = 0
             while ssh_runner_generator.runner.process.poll() is None:
                 chunk = src_fp.read(COPY_BUFSIZE)
                 if chunk == b'':
                     break
                 chunk_size = len(chunk)
                 # compute hash simultaneously
-                for h in hasher:
-                    h.update(chunk)
+                hasher.update(chunk)
                 # we are just putting stuff in the queue, and rely on
                 # its maxsize to cause it to block the next call to
                 # have the progress reports be anyhow valid
                 upload_queue.put(chunk, timeout=timeout)
                 self._progress_report_update(
                     progress_id, ('Uploaded chunk',), chunk_size)
                 upload_size += chunk_size
@@ -309,15 +308,15 @@
         finally:
             self._progress_report_stop(progress_id, ('Finished upload',))
 
         assert ssh_runner_generator.return_code == 0, "Unexpected ssh " \
             f"return value: {ssh_runner_generator.return_code}"
 
         return {
-            **self._get_hash_report(hash_names, hasher),
+            **hasher.get_hexdigest(),
             # return how much was copied. we could compare with
             # `expected_size` and error on mismatch, but not all
             # sources can provide that (e.g. stdin)
             'content-length': upload_size
         }
 
 
@@ -327,15 +326,15 @@
         # make sure the essential pieces exist
         assert self._parsed.hostname
         assert self._parsed.path
         self.ssh_args: list[str] = list(additional_ssh_args)
 
     def run(self,
             payload_cmd: str,
-            protocol: type[WitlessProtocol],
+            protocol: type[RunnerProtocol],
             stdin: Queue | None = None,
             timeout: float | None = None) -> Any | Generator:
         fpath = self._parsed.path
         cmd = ['ssh']
         cmd.extend(self.ssh_args)
         cmd.extend([
             '-e', 'none',
@@ -347,33 +346,7 @@
         ])
         return ThreadedRunner(
             cmd=cmd,
             protocol_class=protocol,
             stdin=subprocess.DEVNULL if stdin is None else stdin,
             timeout=timeout,
         ).run()
-
-
-#
-# Below are generic generator protocols that should be provided
-# upstream
-#
-class _NoCaptureGeneratorProtocol(NoCapture, GeneratorMixIn):
-    def __init__(self, done_future=None, encoding=None):
-        NoCapture.__init__(self, done_future, encoding)
-        GeneratorMixIn.__init__(self)
-
-    def timeout(self, fd):
-        raise TimeoutError(f"Runner timeout: process has not terminated yet")
-
-
-class _StdOutCaptureGeneratorProtocol(StdOutCapture, GeneratorMixIn):
-    def __init__(self, done_future=None, encoding=None):
-        StdOutCapture.__init__(self, done_future, encoding)
-        GeneratorMixIn.__init__(self)
-
-    def pipe_data_received(self, fd: int, data: bytes):
-        assert fd == 1
-        self.send_result(data)
-
-    def timeout(self, fd):
-        raise TimeoutError(f"Runner timeout {fd}")
```

### Comparing `datalad_next-1.0.0b2/datalad_next/url_operations/tests/test_any.py` & `datalad_next-1.0.0b3/datalad_next/url_operations/tests/test_any.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.0.0b2/datalad_next/url_operations/tests/test_file.py` & `datalad_next-1.0.0b3/datalad_next/url_operations/tests/test_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         m.setattr(sys, 'stdin',
                   io.TextIOWrapper(io.BytesIO(
                       bytes(payload, encoding='utf-8'))))
         props = ops.upload(None, from_stdin_url, hash=['md5'])
         assert props['md5'] == '321c3cf486ed509164edec1e1981fec8'
         assert props['content-length'] == len(payload)
 
-    # TODO test missing write permissons
+    # TODO test missing write permissions
 
 def test_file_url_delete(tmp_path):
     payload = 'payload'
     test_path = tmp_path / 'subdir' / 'myfile'
     test_path.parent.mkdir()
     test_url = test_path.as_uri()
     ops = FileUrlOperations()
```

### Comparing `datalad_next-1.0.0b2/datalad_next/url_operations/tests/test_ssh.py` & `datalad_next-1.0.0b3/datalad_next/url_operations/tests/test_ssh.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.0.0b2/datalad_next/utils/__init__.py` & `datalad_next-1.0.0b3/datalad_next/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     Path,
     check_symlink_capability,
     chpwd,
     ensure_bool,
     ensure_list,
     get_dataset_root,
     getargspec,
+    get_wrapped_class,
     knows_annex,
     on_linux,
     on_windows,
     rmtemp,
     rmtree,
     swallow_outputs,
 )
```

### Comparing `datalad_next-1.0.0b2/datalad_next/utils/http_helpers.py` & `datalad_next-1.0.0b3/datalad_next/utils/http_helpers.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.0.0b2/datalad_next/utils/patch.py` & `datalad_next-1.0.0b3/datalad_next/patches/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from importlib import import_module
 import logging
 from typing import Any
 
-lgr = logging.getLogger('datalad.ext.next.utils.patch')
+lgr = logging.getLogger('datalad.ext.next.patches')
 
 
 def apply_patch(
         modname: str,
         objname: str | None,
         attrname: str,
         patch: Any,
```

### Comparing `datalad_next-1.0.0b2/datalad_next/utils/requests_auth.py` & `datalad_next-1.0.0b3/datalad_next/utils/requests_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import logging
 from typing import Dict
 from urllib.parse import urlparse
 import requests
 import www_authenticate
 
+from datalad_next.config import ConfigManager
 from datalad_next.utils import CredentialManager
 from datalad_next.utils.http_helpers import get_auth_realm
 
 lgr = logging.getLogger('datalad.ext.next.utils.requests_auth')
 
 
 __all__ = ['DataladAuth', 'HTTPBearerTokenAuth']
@@ -34,20 +35,20 @@
     """
     _supported_auth_schemes = {
         'basic': 'user_password',
         'digest': 'user_password',
         'bearer': 'token',
     }
 
-    def __init__(self, cfg: CredentialManager, credential: str | None = None):
+    def __init__(self, cfg: ConfigManager, credential: str | None = None):
         """
         Parameters
         ----------
-        cfg: CredentialManager
-          Credentials are looked up in this instance.
+        cfg: ConfigManager
+          Is passed to CredentialManager() as `cfg`-parameter.
         credential: str, optional
           Name of a particular credential to be used for any operations.
         """
         self._credman = CredentialManager(cfg)
         self._credential = credential
         self._entered_credential = None
 
@@ -148,24 +149,25 @@
                 'Only unsupported HTTP auth schemes offered '
                 f'{list(auth_schemes.keys())!r}')
         # go with the first supported scheme
         ascheme = ascheme[0]
         ctype = DataladAuth._supported_auth_schemes[ascheme]
 
         try:
+            realm = get_auth_realm(url, auth_schemes)
             cred = self._credman.get(
                 name=None,
-                _prompt=f'Credential needed for access to {url}',
+                _prompt=f'Credential needed for accessing {url} (authentication realm {realm!r})',
                 _type_hint=ctype,
                 type=ctype,
                 # include the realm in the credential to avoid asking for it
                 # interactively (it is a server-specified property
                 # users would generally not know, if they do, they can use the
                 # `credentials` command upfront.
-                realm=get_auth_realm(url, auth_schemes)
+                realm=realm
             )
             self._entered_credential = cred
             return ascheme, None, cred
         except Exception as e:
             lgr.debug('Credential retrieval failed: %s', e)
             return ascheme, None, None
```

### Comparing `datalad_next-1.0.0b2/datalad_next.egg-info/PKG-INFO` & `datalad_next-1.0.0b3/datalad_next.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalad-next
-Version: 1.0.0b2
+Version: 1.0.0b3
 Summary: What is next in DataLad
 Home-page: https://github.com/datalad/datalad-next
 Author: The DataLad Team and Contributors
 Author-email: team@datalad.org
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
@@ -120,15 +120,15 @@
   command's logic only, while the former enables more uniform and more
   comprehensive validation and error reporting. Beyond per-parameter validation
   and type-conversion also inter-parameter dependency validation and value
   transformations are supported.
 - Improved composition of importable functionality. Key components for `commands`,
   `annexremotes`, `datasets` (etc) are collected in topical top-level modules that
   provide "all" necessary pieces in a single place.
-- `serve_path_via_webdav` test decorator that automatically deploys a local WebDAV
+- `webdav_server` fixture that automatically deploys a local WebDAV
   server.
 - Utilities for HTTP handling
   - `probe_url()` discovers redirects and authentication requirements for an HTTP
     URL
   - `get_auth_realm()` returns a label for an authentication realm that can be used
     to query for matching credentials
 - Utilities for special remote credential management:
```

### Comparing `datalad_next-1.0.0b2/docs/Makefile` & `datalad_next-1.0.0b3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `datalad_next-1.0.0b2/docs/README.md` & `datalad_next-1.0.0b3/docs/README.md`

 * *Files identical despite different names*

### Comparing `datalad_next-1.0.0b2/docs/policy/release-management.md` & `datalad_next-1.0.0b3/docs/policy/release-management.md`

 * *Files identical despite different names*

### Comparing `datalad_next-1.0.0b2/docs/source/_static/datalad_logo.png` & `datalad_next-1.0.0b3/docs/source/_static/datalad_logo.png`

 * *Files identical despite different names*

### Comparing `datalad_next-1.0.0b2/docs/source/conf.py` & `datalad_next-1.0.0b3/docs/source/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -111,17 +111,14 @@
 
 # The name of the Pygments (syntax highlighting) style to use.
 pygments_style = 'sphinx'
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = True
 
-# Example configuration for intersphinx: refer to the Python standard library.
-intersphinx_mapping = {'https://docs.python.org/': None}
-
 # -- Options for HTML output ----------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 html_theme = 'sphinx_rtd_theme'
 
 # The name of an image file (relative to this directory) to place at the top
```

### Comparing `datalad_next-1.0.0b2/docs/source/developer_guide/constraints.rst` & `datalad_next-1.0.0b3/docs/source/developer_guide/constraints.rst`

 * *Files identical despite different names*

### Comparing `datalad_next-1.0.0b2/docs/source/index.rst` & `datalad_next-1.0.0b3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `datalad_next-1.0.0b2/setup.cfg` & `datalad_next-1.0.0b3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -11,16 +11,17 @@
 	License :: OSI Approved :: BSD License
 	Programming Language :: Python :: 3
 
 [options]
 python_requires = >= 3.7
 install_requires = 
 	annexremote
-	datalad >= 0.18.1
+	datalad >= 0.18.4
 	www-authenticate
+	humanize
 packages = find_namespace:
 include_package_data = True
 
 [options.packages.find]
 include = datalad_next*
 
 [options.extras_require]
@@ -38,14 +39,15 @@
 [options.entry_points]
 datalad.extensions = 
 	next = datalad_next:command_suite
 console_scripts = 
 	git-annex-backend-XDLRA = datalad_next.annexbackends.xdlra:main
 	git-remote-datalad-annex = datalad_next.gitremotes.datalad_annex:main
 	git-annex-remote-uncurl = datalad_next.annexremotes.uncurl:main
+	git-annex-remote-archivist = datalad_next.annexremotes.archivist:main
 
 [versioneer]
 VCS = git
 style = pep440
 versionfile_source = datalad_next/_version.py
 versionfile_build = datalad_next/_version.py
 tag_prefix =
```

### Comparing `datalad_next-1.0.0b2/versioneer.py` & `datalad_next-1.0.0b3/versioneer.py`

 * *Files identical despite different names*

