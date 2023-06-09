# Comparing `tmp/bldr-0.0.8.tar.gz` & `tmp/bldr-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bldr-0.0.8.tar", last modified: Wed Jan 11 15:52:35 2023, max compression
+gzip compressed data, was "dist/bldr-0.0.9.tar", last modified: Thu Jan 19 12:49:35 2023, max compression
```

## Comparing `bldr-0.0.8.tar` & `bldr-0.0.9.tar`

### file list

```diff
@@ -1,259 +1,259 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-01-11 15:52:02.000000 bldr-0.0.8/requirements.in
--rw-r--r--   0 runner    (1001) docker     (122)      182 2023-01-11 15:52:02.000000 bldr-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      536 2023-01-11 15:52:02.000000 bldr-0.0.8/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/
--rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-01-11 15:52:02.000000 bldr-0.0.8/test/testutil.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/e2e/
--rw-r--r--   0 runner    (1001) docker     (122)     3049 2023-01-11 15:52:02.000000 bldr-0.0.8/test/e2e/test_shell.py
--rw-r--r--   0 runner    (1001) docker     (122)     5013 2023-01-11 15:52:02.000000 bldr-0.0.8/test/e2e/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:02.000000 bldr-0.0.8/test/e2e/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/depend-test/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/depend-test/debian/
--rw-r--r--   0 runner    (1001) docker     (122)      328 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/depend-test/debian/control
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/depend-test/debian/depend-test.install
--rwxr-xr-x   0 runner    (1001) docker     (122)       76 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/depend-test/debian/rules
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/depend-test/debian/changelog
--rw-r--r--   0 runner    (1001) docker     (122)        2 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/depend-test/debian/compat
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/depend-test/src/
--rwxr-xr-x   0 runner    (1001) docker     (122)       73 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/depend-test/src/run-depend-test
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/depend-test/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      163 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/expected.example-lang-c.contents
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/test-quilt-proj/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/test-quilt-proj/debian-newer/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/test-quilt-proj/debian-newer/debian/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/test-quilt-proj/debian-newer/debian/patches/
--rw-r--r--   0 runner    (1001) docker     (122)      238 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-quilt-proj/debian-newer/debian/patches/hidden-file-typo-fix
--rw-r--r--   0 runner    (1001) docker     (122)      427 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-quilt-proj/debian-newer/debian/patches/new-false-bugfix
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-quilt-proj/debian-newer/debian/patches/series
--rw-r--r--   0 runner    (1001) docker     (122)      384 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-quilt-proj/debian-newer/debian/changelog
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/test-quilt-proj/upstream-newer/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-quilt-proj/upstream-newer/.hidden-file
--rwxr-xr-x   0 runner    (1001) docker     (122)      143 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-quilt-proj/upstream-newer/am-i-quilted
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/test-quilt-proj/debian/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/test-quilt-proj/debian/debian/
--rw-r--r--   0 runner    (1001) docker     (122)      267 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-quilt-proj/debian/debian/control
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/test-quilt-proj/debian/debian/patches/
--rw-r--r--   0 runner    (1001) docker     (122)      420 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-quilt-proj/debian/debian/patches/false-bugfix
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-quilt-proj/debian/debian/patches/series
--rwxr-xr-x   0 runner    (1001) docker     (122)       76 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-quilt-proj/debian/debian/rules
--rw-r--r--   0 runner    (1001) docker     (122)      179 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-quilt-proj/debian/debian/changelog
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/test-quilt-proj/debian/debian/source/
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-quilt-proj/debian/debian/source/format
--rw-r--r--   0 runner    (1001) docker     (122)        2 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-quilt-proj/debian/debian/compat
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-quilt-proj/debian/debian/quilt-proj.install
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/test-quilt-proj/master/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/test-quilt-proj/master/debian/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/test-quilt-proj/master/debian/patches/
--rw-r--r--   0 runner    (1001) docker     (122)      434 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-quilt-proj/master/debian/patches/new-false-bugfix
--rw-r--r--   0 runner    (1001) docker     (122)      574 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-quilt-proj/master/debian/changelog
--rwxr-xr-x   0 runner    (1001) docker     (122)      150 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-quilt-proj/master/am-i-quilted
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/test-quilt-proj/upstream/
--rw-r--r--   0 runner    (1001) docker     (122)       94 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-quilt-proj/upstream/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (122)      136 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-quilt-proj/upstream/am-i-quilted
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/symlinks/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/symlinks/debian/
--rw-r--r--   0 runner    (1001) docker     (122)      314 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/symlinks/debian/control
--rwxr-xr-x   0 runner    (1001) docker     (122)       30 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/symlinks/debian/rules
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/symlinks/debian/changelog
--rw-r--r--   0 runner    (1001) docker     (122)        2 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/symlinks/debian/compat
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/symlinks/src/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/symlinks/src/i_exist
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/symlinks/src/im_right
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/symlinks/src/im_doubly_right
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/symlinks/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/test-reindex-data/
--rw-r--r--   0 runner    (1001) docker     (122)     1652 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-reindex-data/Sources.correct
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/test-reindex-data/depend-test/
--rw-r--r--   0 runner    (1001) docker     (122)      524 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-reindex-data/depend-test/README
--rw-r--r--   0 runner    (1001) docker     (122)     5782 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-reindex-data/depend-test/depend-test_2.3-4_amd64.buildinfo
--rw-r--r--   0 runner    (1001) docker     (122)      727 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-reindex-data/depend-test/depend-test_2.3-4.tar.gz
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/test-reindex-data/depend-test/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/test-reindex-data/depend-test/src/depend-test/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/test-reindex-data/depend-test/src/depend-test/debian/
--rw-r--r--   0 runner    (1001) docker     (122)      328 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-reindex-data/depend-test/src/depend-test/debian/control
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-reindex-data/depend-test/src/depend-test/debian/depend-test.install
--rwxr-xr-x   0 runner    (1001) docker     (122)       76 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-reindex-data/depend-test/src/depend-test/debian/rules
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-reindex-data/depend-test/src/depend-test/debian/changelog
--rw-r--r--   0 runner    (1001) docker     (122)        2 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-reindex-data/depend-test/src/depend-test/debian/compat
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/test-reindex-data/depend-test/src/depend-test/src/
--rwxr-xr-x   0 runner    (1001) docker     (122)       73 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-reindex-data/depend-test/src/depend-test/src/run-depend-test
--rw-r--r--   0 runner    (1001) docker     (122)       87 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-reindex-data/depend-test/src/depend-test/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      358 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-reindex-data/depend-test/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      545 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-reindex-data/depend-test/depend-test_2.3-4.dsc
--rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-reindex-data/depend-test/depend-test_2.3-4_amd64.changes
--rw-r--r--   0 runner    (1001) docker     (122)     1196 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-reindex-data/depend-test/depend-test_2.3-4_amd64.deb
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/test-reindex-data/nonstandard-dir/
--rw-r--r--   0 runner    (1001) docker     (122)      524 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-reindex-data/nonstandard-dir/README
--rw-r--r--   0 runner    (1001) docker     (122)     1192 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-reindex-data/nonstandard-dir/libdependable_2.3-4_amd64.deb
--rw-r--r--   0 runner    (1001) docker     (122)     1890 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-reindex-data/nonstandard-dir/libdependable_2.3-4_amd64.changes
--rw-r--r--   0 runner    (1001) docker     (122)      603 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-reindex-data/nonstandard-dir/libdependable_2.3-4.dsc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/test-reindex-data/nonstandard-dir/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/test-reindex-data/nonstandard-dir/src/libdependable/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/test-reindex-data/nonstandard-dir/src/libdependable/debian/
--rw-r--r--   0 runner    (1001) docker     (122)      475 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-reindex-data/nonstandard-dir/src/libdependable/debian/control
--rwxr-xr-x   0 runner    (1001) docker     (122)       30 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-reindex-data/nonstandard-dir/src/libdependable/debian/rules
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-reindex-data/nonstandard-dir/src/libdependable/debian/libdependable.install
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-reindex-data/nonstandard-dir/src/libdependable/debian/libdependable-dev.install
--rw-r--r--   0 runner    (1001) docker     (122)      157 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-reindex-data/nonstandard-dir/src/libdependable/debian/changelog
--rw-r--r--   0 runner    (1001) docker     (122)        2 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-reindex-data/nonstandard-dir/src/libdependable/debian/compat
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/test-reindex-data/nonstandard-dir/src/libdependable/src/
--rwxr-xr-x   0 runner    (1001) docker     (122)       47 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-reindex-data/nonstandard-dir/src/libdependable/src/depend-on-me-buildtime
--rwxr-xr-x   0 runner    (1001) docker     (122)       44 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-reindex-data/nonstandard-dir/src/libdependable/src/depend-on-me-runtime
--rw-r--r--   0 runner    (1001) docker     (122)       87 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-reindex-data/nonstandard-dir/src/libdependable/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      340 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-reindex-data/nonstandard-dir/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)     6075 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-reindex-data/nonstandard-dir/libdependable_2.3-4_amd64.buildinfo
--rw-r--r--   0 runner    (1001) docker     (122)     1216 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-reindex-data/nonstandard-dir/libdependable-dev_2.3-4_amd64.deb
--rw-r--r--   0 runner    (1001) docker     (122)      786 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-reindex-data/nonstandard-dir/libdependable_2.3-4.tar.gz
--rw-r--r--   0 runner    (1001) docker     (122)     1416 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-reindex-data/Packages.correct
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/test-quilt-proj-onedir/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/test-quilt-proj-onedir/debian/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/test-quilt-proj-onedir/debian/debian/
--rw-r--r--   0 runner    (1001) docker     (122)      282 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-quilt-proj-onedir/debian/debian/control
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/test-quilt-proj-onedir/debian/debian/patches/
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-quilt-proj-onedir/debian/debian/patches/series
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-quilt-proj-onedir/debian/debian/patches/proper-welcome
--rwxr-xr-x   0 runner    (1001) docker     (122)      154 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-quilt-proj-onedir/debian/debian/rules
--rw-r--r--   0 runner    (1001) docker     (122)      186 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-quilt-proj-onedir/debian/debian/changelog
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/test-quilt-proj-onedir/debian/debian/source/
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-quilt-proj-onedir/debian/debian/source/format
--rw-r--r--   0 runner    (1001) docker     (122)        2 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-quilt-proj-onedir/debian/debian/compat
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/test-quilt-proj-onedir/upstream/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/test-quilt-proj-onedir/upstream/feeling/
--rw-r--r--   0 runner    (1001) docker     (122)        4 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-quilt-proj-onedir/upstream/feeling/alone
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-quilt-proj-onedir/upstream/feeling/lonely
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/embed-build-opts/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/embed-build-opts/debian/
--rw-r--r--   0 runner    (1001) docker     (122)      287 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/embed-build-opts/debian/control
--rwxr-xr-x   0 runner    (1001) docker     (122)       30 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/embed-build-opts/debian/rules
--rw-r--r--   0 runner    (1001) docker     (122)      158 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/embed-build-opts/debian/changelog
--rw-r--r--   0 runner    (1001) docker     (122)        2 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/embed-build-opts/debian/compat
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/embed-build-opts/debian/embed-build-opts.docs
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/embed-build-opts/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/test-hooks/
--rwxr-xr-x   0 runner    (1001) docker     (122)       62 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-hooks/post-install-deps
--rwxr-xr-x   0 runner    (1001) docker     (122)       88 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-hooks/pre-build
--rwxr-xr-x   0 runner    (1001) docker     (122)       61 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-hooks/pre-install-deps
--rwxr-xr-x   0 runner    (1001) docker     (122)       53 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-hooks/pre-init
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/quilt-no-patch/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/quilt-no-patch/debian/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/quilt-no-patch/debian/debian/
--rw-r--r--   0 runner    (1001) docker     (122)      323 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/quilt-no-patch/debian/debian/control
--rwxr-xr-x   0 runner    (1001) docker     (122)       30 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/quilt-no-patch/debian/debian/rules
--rw-r--r--   0 runner    (1001) docker     (122)      164 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/quilt-no-patch/debian/debian/changelog
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/quilt-no-patch/debian/debian/quilt-no-patch.docs
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/quilt-no-patch/debian/debian/source/
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/quilt-no-patch/debian/debian/source/format
--rw-r--r--   0 runner    (1001) docker     (122)        2 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/quilt-no-patch/debian/debian/compat
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/quilt-no-patch/master/
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/quilt-no-patch/master/README
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/quilt-no-patch/upstream/
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/quilt-no-patch/upstream/README
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/example-lang-C/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/example-lang-C/debian/
--rw-r--r--   0 runner    (1001) docker     (122)      304 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/example-lang-C/debian/control
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/example-lang-C/debian/copyright
--rwxr-xr-x   0 runner    (1001) docker     (122)       30 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/example-lang-C/debian/rules
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/example-lang-C/debian/changelog
--rw-r--r--   0 runner    (1001) docker     (122)        2 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/example-lang-C/debian/compat
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/example-lang-C/debian/dummy.dirs
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/example-lang-C/src/
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/example-lang-C/src/main.c
--rw-r--r--   0 runner    (1001) docker     (122)       47 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/example-lang-C/src/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/example-lang-C/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/test-git-proj/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/test-git-proj/debian/
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-git-proj/debian/git-proj.install
--rw-r--r--   0 runner    (1001) docker     (122)      209 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-git-proj/debian/control
--rwxr-xr-x   0 runner    (1001) docker     (122)       76 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-git-proj/debian/rules
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-git-proj/debian/changelog
--rw-r--r--   0 runner    (1001) docker     (122)        2 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-git-proj/debian/compat
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/test-git-proj/src/
--rwxr-xr-x   0 runner    (1001) docker     (122)       39 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-git-proj/src/run-git-proj-test
--rw-r--r--   0 runner    (1001) docker     (122)       87 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/test-git-proj/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/libdependable/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/libdependable/debian/
--rw-r--r--   0 runner    (1001) docker     (122)      475 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/libdependable/debian/control
--rwxr-xr-x   0 runner    (1001) docker     (122)       30 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/libdependable/debian/rules
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/libdependable/debian/libdependable.install
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/libdependable/debian/libdependable-dev.install
--rw-r--r--   0 runner    (1001) docker     (122)      157 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/libdependable/debian/changelog
--rw-r--r--   0 runner    (1001) docker     (122)        2 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/libdependable/debian/compat
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/libdependable/src/
--rwxr-xr-x   0 runner    (1001) docker     (122)       47 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/libdependable/src/depend-on-me-buildtime
--rwxr-xr-x   0 runner    (1001) docker     (122)       44 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/libdependable/src/depend-on-me-runtime
--rw-r--r--   0 runner    (1001) docker     (122)       87 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/libdependable/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/never-builds/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/never-builds/debian/
--rw-r--r--   0 runner    (1001) docker     (122)      360 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/never-builds/debian/control
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/example/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/asset/example/debian/
--rw-r--r--   0 runner    (1001) docker     (122)     1142 2023-01-11 15:52:02.000000 bldr-0.0.8/test/asset/example/debian/control
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/unit/
--rw-r--r--   0 runner    (1001) docker     (122)     3537 2023-01-11 15:52:02.000000 bldr-0.0.8/test/unit/test_config.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:02.000000 bldr-0.0.8/test/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:02.000000 bldr-0.0.8/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/test/integration/
--rw-r--r--   0 runner    (1001) docker     (122)     2302 2023-01-11 15:52:02.000000 bldr-0.0.8/test/integration/test_quilt_no_patch.py
--rw-r--r--   0 runner    (1001) docker     (122)     5399 2023-01-11 15:52:02.000000 bldr-0.0.8/test/integration/test_quilt_proj_build.py
--rw-r--r--   0 runner    (1001) docker     (122)     2634 2023-01-11 15:52:02.000000 bldr-0.0.8/test/integration/test_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     6206 2023-01-11 15:52:02.000000 bldr-0.0.8/test/integration/test_debian_build.py
--rw-r--r--   0 runner    (1001) docker     (122)     1575 2023-01-11 15:52:02.000000 bldr-0.0.8/test/integration/test_git_project_build.py
--rw-r--r--   0 runner    (1001) docker     (122)      795 2023-01-11 15:52:02.000000 bldr-0.0.8/test/integration/test_reindex.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:02.000000 bldr-0.0.8/test/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2221 2023-01-11 15:52:02.000000 bldr-0.0.8/test/integration/test_quilt_proj_build_onedir.py
--rw-r--r--   0 runner    (1001) docker     (122)      325 2023-01-11 15:52:02.000000 bldr-0.0.8/test/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-01-11 15:52:02.000000 bldr-0.0.8/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)      608 2023-01-11 15:52:35.000000 bldr-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      732 2023-01-11 15:52:02.000000 bldr-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1483 2023-01-11 15:52:02.000000 bldr-0.0.8/requirements-dev.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/bldr/
--rw-r--r--   0 runner    (1001) docker     (122)      325 2023-01-11 15:52:02.000000 bldr-0.0.8/bldr/version.py
--rw-r--r--   0 runner    (1001) docker     (122)     1208 2023-01-11 15:52:02.000000 bldr-0.0.8/bldr/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5423 2023-01-11 15:52:02.000000 bldr-0.0.8/bldr/docker_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    11718 2023-01-11 15:52:02.000000 bldr-0.0.8/bldr/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)    10618 2023-01-11 15:52:02.000000 bldr-0.0.8/bldr/bldr.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/bldr/data/
--rw-r--r--   0 runner    (1001) docker     (122)      449 2023-01-11 15:52:02.000000 bldr-0.0.8/bldr/data/Dockerfile.tpl
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/bldr/data/files/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/bldr/data/files/etc/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/bldr/data/files/etc/apt/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/bldr/data/files/etc/apt/sources.list.d/
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-01-11 15:52:02.000000 bldr-0.0.8/bldr/data/files/etc/apt/sources.list.d/local-apt.list
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/bldr/data/files/etc/apt/preferences.d/
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-01-11 15:52:02.000000 bldr-0.0.8/bldr/data/files/etc/apt/preferences.d/pin_local
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/bldr/data/files/etc/apt/apt.conf.d/
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-01-11 15:52:02.000000 bldr-0.0.8/bldr/data/files/etc/apt/apt.conf.d/99-debug
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-01-11 15:52:02.000000 bldr-0.0.8/bldr/data/files/etc/apt/apt.conf.d/91-debconf
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/bldr/data/files/etc/sudoers.d/
--rw-r--r--   0 runner    (1001) docker     (122)       55 2023-01-11 15:52:02.000000 bldr-0.0.8/bldr/data/files/etc/sudoers.d/keep_env
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/bldr/data/files/usr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/bldr/data/files/usr/local/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/bldr/data/files/usr/local/bin/
--rwxr-xr-x   0 runner    (1001) docker     (122)      649 2023-01-11 15:52:02.000000 bldr-0.0.8/bldr/data/files/usr/local/bin/install-build-deps
--rwxr-xr-x   0 runner    (1001) docker     (122)     2482 2023-01-11 15:52:02.000000 bldr-0.0.8/bldr/data/files/usr/local/bin/prepare-quilt-package
--rwxr-xr-x   0 runner    (1001) docker     (122)     1028 2023-01-11 15:52:02.000000 bldr-0.0.8/bldr/data/files/usr/local/bin/init-docker-image
--rwxr-xr-x   0 runner    (1001) docker     (122)      178 2023-01-11 15:52:02.000000 bldr-0.0.8/bldr/data/files/usr/local/bin/reindex
--rwxr-xr-x   0 runner    (1001) docker     (122)     2809 2023-01-11 15:52:02.000000 bldr-0.0.8/bldr/data/files/usr/local/bin/build-deb
--rwxr-xr-x   0 runner    (1001) docker     (122)      175 2023-01-11 15:52:02.000000 bldr-0.0.8/bldr/data/files/usr/local/bin/noninteractive-apt-get
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/bldr/data/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (122)       12 2023-01-11 15:52:02.000000 bldr-0.0.8/bldr/data/hooks/post-install-deps
--rwxr-xr-x   0 runner    (1001) docker     (122)       12 2023-01-11 15:52:02.000000 bldr-0.0.8/bldr/data/hooks/pre-build
--rwxr-xr-x   0 runner    (1001) docker     (122)      562 2023-01-11 15:52:02.000000 bldr-0.0.8/bldr/data/hooks/pre-install-deps
--rwxr-xr-x   0 runner    (1001) docker     (122)       12 2023-01-11 15:52:02.000000 bldr-0.0.8/bldr/data/hooks/pre-init
--rw-r--r--   0 runner    (1001) docker     (122)     2818 2023-01-11 15:52:02.000000 bldr-0.0.8/bldr/config.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:02.000000 bldr-0.0.8/bldr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-01-11 15:52:02.000000 bldr-0.0.8/bldr/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-01-11 15:52:02.000000 bldr-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      142 2023-01-11 15:52:02.000000 bldr-0.0.8/requirements-dev.in
--rw-r--r--   0 runner    (1001) docker     (122)     2518 2023-01-11 15:52:02.000000 bldr-0.0.8/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (122)     1739 2023-01-11 15:52:02.000000 bldr-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-11 15:52:35.000000 bldr-0.0.8/bldr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-01-11 15:52:35.000000 bldr-0.0.8/bldr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       40 2023-01-11 15:52:35.000000 bldr-0.0.8/bldr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      628 2023-01-11 15:52:35.000000 bldr-0.0.8/bldr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)     8047 2023-01-11 15:52:35.000000 bldr-0.0.8/bldr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-11 15:52:35.000000 bldr-0.0.8/bldr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1716 2023-01-11 15:52:35.000000 bldr-0.0.8/bldr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1716 2023-01-11 15:52:35.000000 bldr-0.0.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-01-19 12:49:06.000000 bldr-0.0.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:06.000000 bldr-0.0.9/test/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3537 2023-01-19 12:49:06.000000 bldr-0.0.9/test/unit/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/example-lang-C/
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/example-lang-C/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/example-lang-C/debian/
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/example-lang-C/debian/changelog
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/example-lang-C/debian/copyright
+-rwxr-xr-x   0 runner    (1001) docker     (122)       30 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/example-lang-C/debian/rules
+-rw-r--r--   0 runner    (1001) docker     (122)        2 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/example-lang-C/debian/compat
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/example-lang-C/debian/dummy.dirs
+-rw-r--r--   0 runner    (1001) docker     (122)      304 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/example-lang-C/debian/control
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/example-lang-C/src/
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/example-lang-C/src/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/example-lang-C/src/main.c
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/never-builds/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/never-builds/debian/
+-rw-r--r--   0 runner    (1001) docker     (122)      360 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/never-builds/debian/control
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/libdependable/
+-rw-r--r--   0 runner    (1001) docker     (122)       87 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/libdependable/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/libdependable/debian/
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/libdependable/debian/changelog
+-rwxr-xr-x   0 runner    (1001) docker     (122)       30 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/libdependable/debian/rules
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/libdependable/debian/libdependable.install
+-rw-r--r--   0 runner    (1001) docker     (122)        2 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/libdependable/debian/compat
+-rw-r--r--   0 runner    (1001) docker     (122)      475 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/libdependable/debian/control
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/libdependable/debian/libdependable-dev.install
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/libdependable/src/
+-rwxr-xr-x   0 runner    (1001) docker     (122)       47 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/libdependable/src/depend-on-me-buildtime
+-rwxr-xr-x   0 runner    (1001) docker     (122)       44 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/libdependable/src/depend-on-me-runtime
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/expected.example-lang-c.contents
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/embed-build-opts/
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/embed-build-opts/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/embed-build-opts/debian/
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/embed-build-opts/debian/embed-build-opts.docs
+-rw-r--r--   0 runner    (1001) docker     (122)      158 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/embed-build-opts/debian/changelog
+-rwxr-xr-x   0 runner    (1001) docker     (122)       30 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/embed-build-opts/debian/rules
+-rw-r--r--   0 runner    (1001) docker     (122)        2 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/embed-build-opts/debian/compat
+-rw-r--r--   0 runner    (1001) docker     (122)      287 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/embed-build-opts/debian/control
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/depend-test/
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/depend-test/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/depend-test/debian/
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/depend-test/debian/changelog
+-rwxr-xr-x   0 runner    (1001) docker     (122)       76 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/depend-test/debian/rules
+-rw-r--r--   0 runner    (1001) docker     (122)        2 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/depend-test/debian/compat
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/depend-test/debian/depend-test.install
+-rw-r--r--   0 runner    (1001) docker     (122)      328 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/depend-test/debian/control
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/depend-test/src/
+-rwxr-xr-x   0 runner    (1001) docker     (122)       73 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/depend-test/src/run-depend-test
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/test-git-proj/
+-rw-r--r--   0 runner    (1001) docker     (122)       87 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-git-proj/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/test-git-proj/debian/
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-git-proj/debian/changelog
+-rwxr-xr-x   0 runner    (1001) docker     (122)       76 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-git-proj/debian/rules
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-git-proj/debian/git-proj.install
+-rw-r--r--   0 runner    (1001) docker     (122)        2 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-git-proj/debian/compat
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-git-proj/debian/control
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/test-git-proj/src/
+-rwxr-xr-x   0 runner    (1001) docker     (122)       39 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-git-proj/src/run-git-proj-test
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/test-quilt-proj-onedir/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/test-quilt-proj-onedir/debian/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/test-quilt-proj-onedir/debian/debian/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/test-quilt-proj-onedir/debian/debian/patches/
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-quilt-proj-onedir/debian/debian/patches/series
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-quilt-proj-onedir/debian/debian/patches/proper-welcome
+-rw-r--r--   0 runner    (1001) docker     (122)      186 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-quilt-proj-onedir/debian/debian/changelog
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/test-quilt-proj-onedir/debian/debian/source/
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-quilt-proj-onedir/debian/debian/source/format
+-rwxr-xr-x   0 runner    (1001) docker     (122)      154 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-quilt-proj-onedir/debian/debian/rules
+-rw-r--r--   0 runner    (1001) docker     (122)        2 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-quilt-proj-onedir/debian/debian/compat
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-quilt-proj-onedir/debian/debian/control
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/test-quilt-proj-onedir/upstream/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/test-quilt-proj-onedir/upstream/feeling/
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-quilt-proj-onedir/upstream/feeling/lonely
+-rw-r--r--   0 runner    (1001) docker     (122)        4 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-quilt-proj-onedir/upstream/feeling/alone
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/test-hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (122)       53 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-hooks/pre-init
+-rwxr-xr-x   0 runner    (1001) docker     (122)       62 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-hooks/post-install-deps
+-rwxr-xr-x   0 runner    (1001) docker     (122)       61 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-hooks/pre-install-deps
+-rwxr-xr-x   0 runner    (1001) docker     (122)       88 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-hooks/pre-build
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/test-reindex-data/
+-rw-r--r--   0 runner    (1001) docker     (122)     1652 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-reindex-data/Sources.correct
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/test-reindex-data/nonstandard-dir/
+-rw-r--r--   0 runner    (1001) docker     (122)      524 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-reindex-data/nonstandard-dir/README
+-rw-r--r--   0 runner    (1001) docker     (122)      786 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-reindex-data/nonstandard-dir/libdependable_2.3-4.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (122)      340 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-reindex-data/nonstandard-dir/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     1216 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-reindex-data/nonstandard-dir/libdependable-dev_2.3-4_amd64.deb
+-rw-r--r--   0 runner    (1001) docker     (122)     6075 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-reindex-data/nonstandard-dir/libdependable_2.3-4_amd64.buildinfo
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/test-reindex-data/nonstandard-dir/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/test-reindex-data/nonstandard-dir/src/libdependable/
+-rw-r--r--   0 runner    (1001) docker     (122)       87 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-reindex-data/nonstandard-dir/src/libdependable/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/test-reindex-data/nonstandard-dir/src/libdependable/debian/
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-reindex-data/nonstandard-dir/src/libdependable/debian/changelog
+-rwxr-xr-x   0 runner    (1001) docker     (122)       30 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-reindex-data/nonstandard-dir/src/libdependable/debian/rules
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-reindex-data/nonstandard-dir/src/libdependable/debian/libdependable.install
+-rw-r--r--   0 runner    (1001) docker     (122)        2 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-reindex-data/nonstandard-dir/src/libdependable/debian/compat
+-rw-r--r--   0 runner    (1001) docker     (122)      475 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-reindex-data/nonstandard-dir/src/libdependable/debian/control
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-reindex-data/nonstandard-dir/src/libdependable/debian/libdependable-dev.install
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/test-reindex-data/nonstandard-dir/src/libdependable/src/
+-rwxr-xr-x   0 runner    (1001) docker     (122)       47 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-reindex-data/nonstandard-dir/src/libdependable/src/depend-on-me-buildtime
+-rwxr-xr-x   0 runner    (1001) docker     (122)       44 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-reindex-data/nonstandard-dir/src/libdependable/src/depend-on-me-runtime
+-rw-r--r--   0 runner    (1001) docker     (122)     1192 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-reindex-data/nonstandard-dir/libdependable_2.3-4_amd64.deb
+-rw-r--r--   0 runner    (1001) docker     (122)      603 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-reindex-data/nonstandard-dir/libdependable_2.3-4.dsc
+-rw-r--r--   0 runner    (1001) docker     (122)     1890 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-reindex-data/nonstandard-dir/libdependable_2.3-4_amd64.changes
+-rw-r--r--   0 runner    (1001) docker     (122)     1416 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-reindex-data/Packages.correct
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/test-reindex-data/depend-test/
+-rw-r--r--   0 runner    (1001) docker     (122)      524 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-reindex-data/depend-test/README
+-rw-r--r--   0 runner    (1001) docker     (122)     5782 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-reindex-data/depend-test/depend-test_2.3-4_amd64.buildinfo
+-rw-r--r--   0 runner    (1001) docker     (122)      545 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-reindex-data/depend-test/depend-test_2.3-4.dsc
+-rw-r--r--   0 runner    (1001) docker     (122)      727 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-reindex-data/depend-test/depend-test_2.3-4.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (122)     1196 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-reindex-data/depend-test/depend-test_2.3-4_amd64.deb
+-rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-reindex-data/depend-test/depend-test_2.3-4_amd64.changes
+-rw-r--r--   0 runner    (1001) docker     (122)      358 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-reindex-data/depend-test/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/test-reindex-data/depend-test/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/test-reindex-data/depend-test/src/depend-test/
+-rw-r--r--   0 runner    (1001) docker     (122)       87 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-reindex-data/depend-test/src/depend-test/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/test-reindex-data/depend-test/src/depend-test/debian/
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-reindex-data/depend-test/src/depend-test/debian/changelog
+-rwxr-xr-x   0 runner    (1001) docker     (122)       76 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-reindex-data/depend-test/src/depend-test/debian/rules
+-rw-r--r--   0 runner    (1001) docker     (122)        2 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-reindex-data/depend-test/src/depend-test/debian/compat
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-reindex-data/depend-test/src/depend-test/debian/depend-test.install
+-rw-r--r--   0 runner    (1001) docker     (122)      328 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-reindex-data/depend-test/src/depend-test/debian/control
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/test-reindex-data/depend-test/src/depend-test/src/
+-rwxr-xr-x   0 runner    (1001) docker     (122)       73 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-reindex-data/depend-test/src/depend-test/src/run-depend-test
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/quilt-no-patch/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/quilt-no-patch/master/
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/quilt-no-patch/master/README
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/quilt-no-patch/debian/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/quilt-no-patch/debian/debian/
+-rw-r--r--   0 runner    (1001) docker     (122)      164 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/quilt-no-patch/debian/debian/changelog
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/quilt-no-patch/debian/debian/source/
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/quilt-no-patch/debian/debian/source/format
+-rwxr-xr-x   0 runner    (1001) docker     (122)       30 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/quilt-no-patch/debian/debian/rules
+-rw-r--r--   0 runner    (1001) docker     (122)        2 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/quilt-no-patch/debian/debian/compat
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/quilt-no-patch/debian/debian/quilt-no-patch.docs
+-rw-r--r--   0 runner    (1001) docker     (122)      323 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/quilt-no-patch/debian/debian/control
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/quilt-no-patch/upstream/
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/quilt-no-patch/upstream/README
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/test-quilt-proj/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/test-quilt-proj/debian-newer/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/test-quilt-proj/debian-newer/debian/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/test-quilt-proj/debian-newer/debian/patches/
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-quilt-proj/debian-newer/debian/patches/series
+-rw-r--r--   0 runner    (1001) docker     (122)      427 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-quilt-proj/debian-newer/debian/patches/new-false-bugfix
+-rw-r--r--   0 runner    (1001) docker     (122)      238 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-quilt-proj/debian-newer/debian/patches/hidden-file-typo-fix
+-rw-r--r--   0 runner    (1001) docker     (122)      384 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-quilt-proj/debian-newer/debian/changelog
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/test-quilt-proj/upstream-newer/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      143 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-quilt-proj/upstream-newer/am-i-quilted
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-quilt-proj/upstream-newer/.hidden-file
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/test-quilt-proj/master/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      150 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-quilt-proj/master/am-i-quilted
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/test-quilt-proj/master/debian/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/test-quilt-proj/master/debian/patches/
+-rw-r--r--   0 runner    (1001) docker     (122)      434 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-quilt-proj/master/debian/patches/new-false-bugfix
+-rw-r--r--   0 runner    (1001) docker     (122)      574 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-quilt-proj/master/debian/changelog
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/test-quilt-proj/debian/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/test-quilt-proj/debian/debian/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/test-quilt-proj/debian/debian/patches/
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-quilt-proj/debian/debian/patches/series
+-rw-r--r--   0 runner    (1001) docker     (122)      420 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-quilt-proj/debian/debian/patches/false-bugfix
+-rw-r--r--   0 runner    (1001) docker     (122)      179 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-quilt-proj/debian/debian/changelog
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/test-quilt-proj/debian/debian/source/
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-quilt-proj/debian/debian/source/format
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-quilt-proj/debian/debian/quilt-proj.install
+-rwxr-xr-x   0 runner    (1001) docker     (122)       76 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-quilt-proj/debian/debian/rules
+-rw-r--r--   0 runner    (1001) docker     (122)        2 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-quilt-proj/debian/debian/compat
+-rw-r--r--   0 runner    (1001) docker     (122)      267 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-quilt-proj/debian/debian/control
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/test-quilt-proj/upstream/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      136 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-quilt-proj/upstream/am-i-quilted
+-rw-r--r--   0 runner    (1001) docker     (122)       94 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/test-quilt-proj/upstream/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/example/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/example/debian/
+-rw-r--r--   0 runner    (1001) docker     (122)     1142 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/example/debian/control
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/symlinks/
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/symlinks/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/symlinks/debian/
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/symlinks/debian/changelog
+-rwxr-xr-x   0 runner    (1001) docker     (122)       30 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/symlinks/debian/rules
+-rw-r--r--   0 runner    (1001) docker     (122)        2 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/symlinks/debian/compat
+-rw-r--r--   0 runner    (1001) docker     (122)      314 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/symlinks/debian/control
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/asset/symlinks/src/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/symlinks/src/i_exist
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/symlinks/src/im_right
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:06.000000 bldr-0.0.9/test/asset/symlinks/src/im_doubly_right
+-rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-01-19 12:49:06.000000 bldr-0.0.9/test/testutil.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/e2e/
+-rw-r--r--   0 runner    (1001) docker     (122)     3049 2023-01-19 12:49:06.000000 bldr-0.0.9/test/e2e/test_shell.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5013 2023-01-19 12:49:06.000000 bldr-0.0.9/test/e2e/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:06.000000 bldr-0.0.9/test/e2e/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:06.000000 bldr-0.0.9/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/test/integration/
+-rw-r--r--   0 runner    (1001) docker     (122)      795 2023-01-19 12:49:06.000000 bldr-0.0.9/test/integration/test_reindex.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2221 2023-01-19 12:49:06.000000 bldr-0.0.9/test/integration/test_quilt_proj_build_onedir.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5399 2023-01-19 12:49:06.000000 bldr-0.0.9/test/integration/test_quilt_proj_build.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1575 2023-01-19 12:49:06.000000 bldr-0.0.9/test/integration/test_git_project_build.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6206 2023-01-19 12:49:06.000000 bldr-0.0.9/test/integration/test_debian_build.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:06.000000 bldr-0.0.9/test/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2302 2023-01-19 12:49:06.000000 bldr-0.0.9/test/integration/test_quilt_no_patch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2634 2023-01-19 12:49:06.000000 bldr-0.0.9/test/integration/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      325 2023-01-19 12:49:06.000000 bldr-0.0.9/test/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-01-19 12:49:06.000000 bldr-0.0.9/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)      182 2023-01-19 12:49:06.000000 bldr-0.0.9/MANIFEST.in
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1739 2023-01-19 12:49:06.000000 bldr-0.0.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)      536 2023-01-19 12:49:06.000000 bldr-0.0.9/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/bldr/
+-rw-r--r--   0 runner    (1001) docker     (122)     2818 2023-01-19 12:49:06.000000 bldr-0.0.9/bldr/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      325 2023-01-19 12:49:06.000000 bldr-0.0.9/bldr/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/bldr/data/
+-rw-r--r--   0 runner    (1001) docker     (122)      763 2023-01-19 12:49:06.000000 bldr-0.0.9/bldr/data/Dockerfile.tpl
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/bldr/data/files/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/bldr/data/files/usr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/bldr/data/files/usr/local/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/bldr/data/files/usr/local/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      175 2023-01-19 12:49:06.000000 bldr-0.0.9/bldr/data/files/usr/local/bin/noninteractive-apt-get
+-rwxr-xr-x   0 runner    (1001) docker     (122)      178 2023-01-19 12:49:06.000000 bldr-0.0.9/bldr/data/files/usr/local/bin/reindex
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2809 2023-01-19 12:49:06.000000 bldr-0.0.9/bldr/data/files/usr/local/bin/build-deb
+-rwxr-xr-x   0 runner    (1001) docker     (122)      649 2023-01-19 12:49:06.000000 bldr-0.0.9/bldr/data/files/usr/local/bin/install-build-deps
+-rwxr-xr-x   0 runner    (1001) docker     (122)      858 2023-01-19 12:49:06.000000 bldr-0.0.9/bldr/data/files/usr/local/bin/init-docker-image
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2482 2023-01-19 12:49:06.000000 bldr-0.0.9/bldr/data/files/usr/local/bin/prepare-quilt-package
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/bldr/data/files/etc/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/bldr/data/files/etc/sudoers.d/
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-01-19 12:49:06.000000 bldr-0.0.9/bldr/data/files/etc/sudoers.d/keep_env
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/bldr/data/files/etc/apt/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/bldr/data/files/etc/apt/preferences.d/
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-01-19 12:49:06.000000 bldr-0.0.9/bldr/data/files/etc/apt/preferences.d/pin_local
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/bldr/data/files/etc/apt/apt.conf.d/
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-01-19 12:49:06.000000 bldr-0.0.9/bldr/data/files/etc/apt/apt.conf.d/99-debug
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-01-19 12:49:06.000000 bldr-0.0.9/bldr/data/files/etc/apt/apt.conf.d/91-debconf
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/bldr/data/files/etc/apt/sources.list.d/
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-01-19 12:49:06.000000 bldr-0.0.9/bldr/data/files/etc/apt/sources.list.d/local-apt.list
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/bldr/data/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      542 2023-01-19 12:49:06.000000 bldr-0.0.9/bldr/data/hooks/pre-init
+-rwxr-xr-x   0 runner    (1001) docker     (122)       12 2023-01-19 12:49:06.000000 bldr-0.0.9/bldr/data/hooks/post-install-deps
+-rwxr-xr-x   0 runner    (1001) docker     (122)       12 2023-01-19 12:49:06.000000 bldr-0.0.9/bldr/data/hooks/pre-install-deps
+-rwxr-xr-x   0 runner    (1001) docker     (122)       12 2023-01-19 12:49:06.000000 bldr-0.0.9/bldr/data/hooks/pre-build
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-01-19 12:49:06.000000 bldr-0.0.9/bldr/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)     1208 2023-01-19 12:49:06.000000 bldr-0.0.9/bldr/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:06.000000 bldr-0.0.9/bldr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10618 2023-01-19 12:49:06.000000 bldr-0.0.9/bldr/bldr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11718 2023-01-19 12:49:06.000000 bldr-0.0.9/bldr/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5423 2023-01-19 12:49:06.000000 bldr-0.0.9/bldr/docker_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2518 2023-01-19 12:49:06.000000 bldr-0.0.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-01-19 12:49:06.000000 bldr-0.0.9/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1483 2023-01-19 12:49:06.000000 bldr-0.0.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      142 2023-01-19 12:49:06.000000 bldr-0.0.9/requirements-dev.in
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 12:49:35.000000 bldr-0.0.9/bldr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-01-19 12:49:35.000000 bldr-0.0.9/bldr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-01-19 12:49:35.000000 bldr-0.0.9/bldr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     8047 2023-01-19 12:49:35.000000 bldr-0.0.9/bldr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-19 12:49:35.000000 bldr-0.0.9/bldr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1716 2023-01-19 12:49:35.000000 bldr-0.0.9/bldr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      628 2023-01-19 12:49:35.000000 bldr-0.0.9/bldr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      608 2023-01-19 12:49:35.000000 bldr-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      732 2023-01-19 12:49:06.000000 bldr-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1716 2023-01-19 12:49:35.000000 bldr-0.0.9/PKG-INFO
```

### Comparing `bldr-0.0.8/requirements.txt` & `bldr-0.0.9/requirements.txt`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/test/testutil.py` & `bldr-0.0.9/test/testutil.py`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/test/e2e/test_shell.py` & `bldr-0.0.9/test/e2e/test_shell.py`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/test/e2e/test_cli.py` & `bldr-0.0.9/test/e2e/test_cli.py`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/test/asset/test-quilt-proj/master/debian/changelog` & `bldr-0.0.9/test/asset/test-quilt-proj/master/debian/changelog`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/test/asset/test-reindex-data/Sources.correct` & `bldr-0.0.9/test/asset/test-reindex-data/Sources.correct`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/test/asset/test-reindex-data/depend-test/README` & `bldr-0.0.9/test/asset/test-reindex-data/nonstandard-dir/README`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/test/asset/test-reindex-data/depend-test/depend-test_2.3-4_amd64.buildinfo` & `bldr-0.0.9/test/asset/test-reindex-data/depend-test/depend-test_2.3-4_amd64.buildinfo`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/test/asset/test-reindex-data/depend-test/depend-test_2.3-4.tar.gz` & `bldr-0.0.9/test/asset/test-reindex-data/depend-test/depend-test_2.3-4.tar.gz`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/test/asset/test-reindex-data/depend-test/depend-test_2.3-4.dsc` & `bldr-0.0.9/test/asset/test-reindex-data/depend-test/depend-test_2.3-4.dsc`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/test/asset/test-reindex-data/depend-test/depend-test_2.3-4_amd64.changes` & `bldr-0.0.9/test/asset/test-reindex-data/depend-test/depend-test_2.3-4_amd64.changes`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/test/asset/test-reindex-data/depend-test/depend-test_2.3-4_amd64.deb` & `bldr-0.0.9/test/asset/test-reindex-data/depend-test/depend-test_2.3-4_amd64.deb`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/test/asset/test-reindex-data/nonstandard-dir/README` & `bldr-0.0.9/test/asset/test-reindex-data/depend-test/README`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/test/asset/test-reindex-data/nonstandard-dir/libdependable_2.3-4_amd64.deb` & `bldr-0.0.9/test/asset/test-reindex-data/nonstandard-dir/libdependable_2.3-4_amd64.deb`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/test/asset/test-reindex-data/nonstandard-dir/libdependable_2.3-4_amd64.changes` & `bldr-0.0.9/test/asset/test-reindex-data/nonstandard-dir/libdependable_2.3-4_amd64.changes`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/test/asset/test-reindex-data/nonstandard-dir/libdependable_2.3-4.dsc` & `bldr-0.0.9/test/asset/test-reindex-data/nonstandard-dir/libdependable_2.3-4.dsc`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/test/asset/test-reindex-data/nonstandard-dir/libdependable_2.3-4_amd64.buildinfo` & `bldr-0.0.9/test/asset/test-reindex-data/nonstandard-dir/libdependable_2.3-4_amd64.buildinfo`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/test/asset/test-reindex-data/nonstandard-dir/libdependable-dev_2.3-4_amd64.deb` & `bldr-0.0.9/test/asset/test-reindex-data/nonstandard-dir/libdependable-dev_2.3-4_amd64.deb`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/test/asset/test-reindex-data/nonstandard-dir/libdependable_2.3-4.tar.gz` & `bldr-0.0.9/test/asset/test-reindex-data/nonstandard-dir/libdependable_2.3-4.tar.gz`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/test/asset/test-reindex-data/Packages.correct` & `bldr-0.0.9/test/asset/test-reindex-data/Packages.correct`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/test/asset/example/debian/control` & `bldr-0.0.9/test/asset/example/debian/control`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/test/unit/test_config.py` & `bldr-0.0.9/test/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/test/integration/test_quilt_no_patch.py` & `bldr-0.0.9/test/integration/test_quilt_no_patch.py`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/test/integration/test_quilt_proj_build.py` & `bldr-0.0.9/test/integration/test_quilt_proj_build.py`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/test/integration/test_config.py` & `bldr-0.0.9/test/integration/test_config.py`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/test/integration/test_debian_build.py` & `bldr-0.0.9/test/integration/test_debian_build.py`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/test/integration/test_git_project_build.py` & `bldr-0.0.9/test/integration/test_git_project_build.py`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/test/integration/test_reindex.py` & `bldr-0.0.9/test/integration/test_reindex.py`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/test/integration/test_quilt_proj_build_onedir.py` & `bldr-0.0.9/test/integration/test_quilt_proj_build_onedir.py`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/test/conftest.py` & `bldr-0.0.9/test/conftest.py`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/setup.cfg` & `bldr-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/README.md` & `bldr-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/requirements-dev.txt` & `bldr-0.0.9/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/bldr/utils.py` & `bldr-0.0.9/bldr/utils.py`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/bldr/docker_utils.py` & `bldr-0.0.9/bldr/docker_utils.py`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/bldr/cli.py` & `bldr-0.0.9/bldr/cli.py`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/bldr/bldr.py` & `bldr-0.0.9/bldr/bldr.py`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/bldr/data/files/usr/local/bin/install-build-deps` & `bldr-0.0.9/bldr/data/files/usr/local/bin/install-build-deps`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/bldr/data/files/usr/local/bin/prepare-quilt-package` & `bldr-0.0.9/bldr/data/files/usr/local/bin/prepare-quilt-package`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/bldr/data/files/usr/local/bin/init-docker-image` & `bldr-0.0.9/bldr/data/files/usr/local/bin/init-docker-image`

 * *Files 14% similar despite different names*

```diff
@@ -2,19 +2,14 @@
 
 set -e
 echo "Preparing BLDR deb builder docker image"
 
 echo "Adding non-privileged user ${NONPRIV_USER_NAME} with uid ${NONPRIV_USER_UID}"
 useradd -u ${NONPRIV_USER_UID} ${NONPRIV_USER_NAME} -m
 
-echo "Creating local apt repo, so that the supplied /etc/apt/sources.list works in this context too"
-mkdir /local-apt
-touch /local-apt/Packages
-touch /local-apt/Sources
-
 echo "Downloading and installing packages required by BLDR"
 noninteractive-apt-get update
 noninteractive-apt-get install eatmydata
 noninteractive-apt-get install nano joe vim-tiny \
     rsync sudo build-essential \
     pkg-config devscripts equivs git
 if [[ $(lsb_release --codename --short) = 'xenial' ]]
```

### Comparing `bldr-0.0.8/bldr/data/files/usr/local/bin/build-deb` & `bldr-0.0.9/bldr/data/files/usr/local/bin/build-deb`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/bldr/data/hooks/pre-install-deps` & `bldr-0.0.9/bldr/data/hooks/pre-init`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 #!/bin/bash
 
 perform_unminimization() {
-    local unminimize_cmd=$(command -v unminimize)
+    local unminimize_cmd="$(command -v unminimize)"
 
-    if [[ ${unminimize_cmd} != "" ]]; then
+    if [[ "${unminimize_cmd}" != "" ]]; then
         echo
         cat <<"END"
 Performing an image unminimization, because we experienced that more and more
 packages have tests depending on data which is not present on a minimized
 image.
 
 If this unminimization bothers you, please remove the
-'perform_unminimization' function from the 'pre-install-deps' hook.
+'perform_unminimization' function from the 'pre-init' hook.
 END
         echo
 
-        set -e
-        yes | $unminimize_cmd
-        set +e
+        yes | "${unminimize_cmd}" || exit 1
 
     fi
 }
 
 
 perform_unminimization
```

### Comparing `bldr-0.0.8/bldr/config.py` & `bldr-0.0.9/bldr/config.py`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/LICENSE` & `bldr-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/Makefile` & `bldr-0.0.9/Makefile`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/setup.py` & `bldr-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/bldr.egg-info/requires.txt` & `bldr-0.0.9/bldr.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/bldr.egg-info/SOURCES.txt` & `bldr-0.0.9/bldr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bldr-0.0.8/bldr.egg-info/PKG-INFO` & `bldr-0.0.9/bldr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bldr
-Version: 0.0.8
+Version: 0.0.9
 Summary: Build debian packages in a clean docker environment
 Home-page: https://www.github.com/OneIdentity/bldr
 Author: BLDR Developers
 Author-email: noreply@oneidentity.com
 License: MIT
 Description: BLDR
         ====
```

### Comparing `bldr-0.0.8/PKG-INFO` & `bldr-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bldr
-Version: 0.0.8
+Version: 0.0.9
 Summary: Build debian packages in a clean docker environment
 Home-page: https://www.github.com/OneIdentity/bldr
 Author: BLDR Developers
 Author-email: noreply@oneidentity.com
 License: MIT
 Description: BLDR
         ====
```

