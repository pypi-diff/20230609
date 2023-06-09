# Comparing `tmp/pure_ocean_breeze-3.9.5.tar.gz` & `tmp/pure_ocean_breeze-3.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pure_ocean_breeze-3.9.5.tar", last modified: Tue May 16 13:39:02 2023, max compression
+gzip compressed data, was "pure_ocean_breeze-3.9.6.tar", last modified: Fri Jun  9 08:54:34 2023, max compression
```

## Comparing `pure_ocean_breeze-3.9.5.tar` & `pure_ocean_breeze-3.9.6.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.100108 pure_ocean_breeze-3.9.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-16 13:39:02.096108 pure_ocean_breeze-3.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.088107 pure_ocean_breeze-3.9.5/pure_ocean_breeze/
--rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.088107 pure_ocean_breeze-3.9.5/pure_ocean_breeze/data/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31742 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/data/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    29552 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    49960 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    49390 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.088107 pure_ocean_breeze-3.9.5/pure_ocean_breeze/future_version/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23637 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.088107 pure_ocean_breeze-3.9.5/pure_ocean_breeze/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.088107 pure_ocean_breeze-3.9.5/pure_ocean_breeze/labor/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)   240111 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.088107 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.088107 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v1/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)   192825 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.092108 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v1p10/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v1p10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v1p10/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)    85655 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.092108 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v2/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v2/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)   314704 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.092108 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.092108 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/data/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29395 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/data/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    43178 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.092108 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/future_version/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.092108 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.092108 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/labor/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)   138094 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.092108 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/mail/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.092108 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/state/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.096108 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/withs/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.096108 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/
--rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.096108 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/data/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29805 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/data/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    23214 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    29153 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    45478 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.096108 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/future_version/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.096108 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.096108 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/labor/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)   193541 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.096108 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/mail/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.096108 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/state/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.096108 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/withs/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.096108 pure_ocean_breeze-3.9.5/pure_ocean_breeze/mail/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.096108 pure_ocean_breeze-3.9.5/pure_ocean_breeze/state/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.096108 pure_ocean_breeze-3.9.5/pure_ocean_breeze/withs/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.088107 pure_ocean_breeze-3.9.5/pure_ocean_breeze.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-16 13:39:02.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-05-16 13:39:02.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:39:02.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-16 13:39:02.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-16 13:39:02.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:39:02.100108 pure_ocean_breeze-3.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.120399 pure_ocean_breeze-3.9.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-06-09 08:54:34.120399 pure_ocean_breeze-3.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.108399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/
+-rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.112399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31742 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29570 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65150 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49382 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.112399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/future_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23637 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.112399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.112399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/labor/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   227673 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.112399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.112399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v1/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)   192825 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.112399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v1p10/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v1p10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v1p10/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85655 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.112399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v2/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)   314704 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.112399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.116399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29395 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43178 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.116399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/future_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.116399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.116399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/labor/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   138094 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.116399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.116399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.116399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/withs/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.116399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/
+-rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.116399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29805 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23214 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29153 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45478 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.120399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/future_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.120399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.120399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/labor/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   193541 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.120399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.120399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.120399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/withs/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.120399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.120399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.120399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/withs/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.108399 pure_ocean_breeze-3.9.6/pure_ocean_breeze.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-06-09 08:54:34.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-06-09 08:54:34.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 08:54:34.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-09 08:54:34.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-09 08:54:34.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 08:54:34.120399 pure_ocean_breeze-3.9.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/setup.py
```

### Comparing `pure_ocean_breeze-3.9.5/LICENSE` & `pure_ocean_breeze-3.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/PKG-INFO` & `pure_ocean_breeze-3.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure_ocean_breeze
-Version: 3.9.5
+Version: 3.9.6
 Summary: stock factor test
 Home-page: https://github.com/chen-001/pure_ocean_breeze.git
 Author: chenzongwei
 Author-email: winterwinter999@163.com
 License: MIT
 Project-URL: Documentation, https://chen-001.github.io/pure_ocean_breeze/
 Requires-Python: >=3
```

### Comparing `pure_ocean_breeze-3.9.5/README.md` & `pure_ocean_breeze-3.9.6/README.md`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/__init__.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 一个量化多因子研究的框架，包含数据、回测、因子加工等方面的功能
 """
 
-__updated__ = "2023-05-13 09:20:38"
-__version__ = "3.9.5"
+__updated__ = "2023-05-18 18:47:05"
+__version__ = "3.9.6"
 __author__ = "chenzongwei"
 __author_email__ = "winterwinter999@163.com"
 __url__ = "https://github.com/chen-001/pure_ocean_breeze"
 __all__ = [
     "data",
     "labor",
     "state",
```

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/data/database.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/data/dicts.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/data/read_data.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/data/read_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,15 @@
             lows = pd.read_parquet(homeplace.daily_data_file + "lows.parquet")
             df = lows
         elif vwap:
             df = pd.read_parquet(
                 homeplace.daily_data_file + "vwaps.parquet"
             ) * read_daily(adjfactor=1, start=start)
         elif tr:
-            trs = pd.read_parquet(homeplace.daily_data_file + "trs.parquet")
+            trs = pd.read_parquet(homeplace.daily_data_file + "trs.parquet").replace(0,np.nan)
             df = trs
         elif sharenum:
             sharenums = pd.read_parquet(homeplace.daily_data_file + "sharenums.parquet")
             df = sharenums
         elif total_sharenum:
             df = pd.read_parquet(homeplace.daily_data_file + "total_sharenums.parquet")
         elif amount:
```

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/data/tools.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/data/tools.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 针对一些不常见的文件格式，读取数据文件的一些工具函数，以及其他数据工具
 """
 
-__updated__ = "2023-03-22 22:50:18"
+__updated__ = "2023-06-09 16:44:30"
 
 import os
 import pandas as pd
 import tqdm.auto
 import datetime
 import scipy.io as scio
 import numpy as np
 import numpy_ext as npext
+import knockknock as kk
 import scipy.stats as ss
 from functools import reduce, partial
 from loguru import logger
 from typing import Callable, Union, Dict, List, Tuple
 
 try:
     import rqdatac
@@ -22,14 +23,18 @@
     rqdatac.init()
 except Exception:
     print("暂时未连接米筐")
 from pure_ocean_breeze.state.homeplace import HomePlace
 import deprecation
 from pure_ocean_breeze import __version__
 from pure_ocean_breeze.state.decorators import do_on_dfs
+try:
+    homeplace = HomePlace()
+except Exception:
+    print("您暂未初始化，功能将受限")
 
 
 def is_notebook() -> bool:
     try:
         shell = get_ipython().__class__.__name__
         if shell == "ZMQInteractiveShell":
             return True  # Jupyter notebook or qtconsole
@@ -405,20 +410,317 @@
         i.rename(columns={list(i.columns)[-2]: "code", list(i.columns)[0]: "date"})
         for i in dfs
     ]
     df = reduce(lambda x, y: pd.merge(x, y, on=["date", "code"], how=how), dfs)
     return df
 
 
+class pure_dawn(object):
+    """
+    因子切割论的母框架，可以对两个因子进行类似于因子切割的操作
+    可用于派生任何"以两个因子生成一个因子"的子类
+    使用举例
+    cut函数里，必须带有输入变量df,df有两个columns，一个名为'fac1'，一个名为'fac2'，df是最近一个回看期内的数据
+    ```python
+    class Cut(pure_dawn):
+
+    def cut(self,df):
+        df=df.sort_values('fac1')
+        df=df.assign(fac3=df.fac1*df.fac2)
+        ret0=df.fac2.iloc[:4].mean()
+        ret1=df.fac2.iloc[4:8].mean()
+        ret2=df.fac2.iloc[8:12].mean()
+        ret3=df.fac2.iloc[12:16].mean()
+        ret4=df.fac2.iloc[16:].mean()
+        aret0=df.fac3.iloc[:4].mean()
+        aret1=df.fac3.iloc[4:8].mean()
+        aret2=df.fac3.iloc[8:12].mean()
+        aret3=df.fac3.iloc[12:16].mean()
+        aret4=df.fac3.iloc[16:].mean()
+        return ret0,ret1,ret2,ret3,ret4,aret0,aret1,aret2,aret3,aret4
+
+    cut=Cut(ct,ret_inday)
+    cut.run(cut.cut)
+
+    cut0=get_value(cut(),0)
+    cut1=get_value(cut(),1)
+    cut2=get_value(cut(),2)
+    cut3=get_value(cut(),3)
+    cut4=get_value(cut(),4)
+    ```
+    """
+
+    def __init__(self, fac1: pd.DataFrame, fac2: pd.DataFrame, *args: list) -> None:
+        """几个因子的操作，每个月操作一次
+
+        Parameters
+        ----------
+        fac1 : pd.DataFrame
+            因子值1，index为时间，columns为股票代码，values为因子值
+        fac2 : pd.DataFrame
+            因子2，index为时间，columns为股票代码，values为因子值
+        """
+        self.fac1 = fac1
+        self.fac1 = self.fac1.stack().reset_index()
+        self.fac1.columns = ["date", "code", "fac1"]
+        self.fac2 = fac2
+        self.fac2 = self.fac2.stack().reset_index()
+        self.fac2.columns = ["date", "code", "fac2"]
+        fac_all = pd.merge(self.fac1, self.fac2, on=["date", "code"])
+        for i, fac in enumerate(args):
+            fac = fac.stack().reset_index()
+            fac.columns = ["date", "code", f"fac{i+3}"]
+            fac_all = pd.merge(fac_all, fac, on=["date", "code"])
+        fac_all = fac_all.sort_values(["date", "code"])
+        self.fac = fac_all.copy()
+
+    def __call__(self) -> pd.DataFrame:
+        """返回最终月度因子值
+
+        Returns
+        -------
+        `pd.DataFrame`
+            最终因子值
+        """
+        return self.fac.copy()
+
+    def get_fac_long_and_tradedays(self):
+        """将两个因子的矩阵转化为长列表"""
+        self.tradedays = sorted(list(set(self.fac.date)))
+
+    def get_month_starts_and_ends(self, backsee=20):
+        """计算出每个月回看期间的起点日和终点日"""
+        self.month_ends = [
+            i
+            for i, j in zip(self.tradedays[:-1], self.tradedays[1:])
+            if i.month != j.month
+        ]
+        self.month_ends.append(self.tradedays[-1])
+        self.month_starts = [
+            self.find_begin(self.tradedays, i, backsee=backsee) for i in self.month_ends
+        ]
+        self.month_starts[0] = self.tradedays[0]
+
+    def find_begin(self, tradedays, end_day, backsee=20):
+        """找出回看若干天的开始日，默认为20"""
+        end_day_index = tradedays.index(end_day)
+        start_day_index = end_day_index - backsee + 1
+        start_day = tradedays[start_day_index]
+        return start_day
+
+    def make_monthly_factors_single_code(self, df, func, daily):
+        """
+        对单一股票来计算月度因子
+        func为单月执行的函数，返回值应为月度因子，如一个float或一个list
+        df为一个股票的四列表，包含时间、代码、因子1和因子2
+        """
+        res = {}
+        if daily:
+            ones = [self.find_begin(i) for i in self.tradedays[self.backsee - 1 :]]
+            twos = self.tradedays[self.backsee - 1 :]
+        else:
+            ones = self.month_starts
+            twos = self.month_ends
+        for start, end in zip(ones, twos):
+            this_month = df[(df.date >= start) & (df.date <= end)]
+            res[end] = func(this_month)
+        dates = list(res.keys())
+        corrs = list(res.values())
+        part = pd.DataFrame({"date": dates, "corr": corrs})
+        return part
+
+    @staticmethod
+    def for_cross_via_zip(func):
+        """返回值为多个pd.Series，每个pd.Series的index为股票代码，values为单个因子值
+        例如
+        ```python
+        return (
+                    pd.Series([1.54,8.77,9.99……],index=['000001.SZ','000002.SZ','000004.SZ'……]),
+                    pd.Series([3.54,6.98,9.01……],index=['000001.SZ','000002.SZ','000004.SZ'……]),
+                )
+        ```
+        上例中，每个股票一天返回两个因子值，每个pd.Series对应一个因子值
+        """
+
+        def full_run(df, *args, **kwargs):
+            res = func(df, *args, **kwargs)
+            if isinstance(res, pd.Series):
+                return res
+            else:
+                res = pd.concat(res, axis=1)
+                res.columns = [f"fac{i}" for i in range(len(res.columns))]
+                res = res.assign(fac=list(zip(*[res[i] for i in list(res.columns)])))
+                return res.fac
+
+        return full_run
+
+    def get_monthly_factor(
+        self, func, whole_cross: bool = 0, daily: bool = 0, history_file: str = None
+    ):
+        """运行自己写的函数，获得月度因子"""
+        if daily:
+            iter_item = self.tradedays[self.backsee - 1 :]
+        else:
+            iter_item = self.month_ends
+        res = []
+        if history_file is not None:
+            if os.path.exists(homeplace.update_data_file + history_file):
+                old = pd.read_parquet(homeplace.update_data_file + history_file)
+                old_date = old.index.max()
+                if old_date == self.fac.date.max():
+                    logger.info(f"本地文件已经是最新的了，无需计算")
+                else:
+                    try:
+                        new_date = self.find_begin(
+                            self.tradedays, old_date, self.backsee
+                        )
+                        fac = self.fac[self.fac.date > new_date]
+                        iter_item = [i for i in iter_item if i > new_date]
+                        if whole_cross:
+                            for end_date in tqdm.auto.tqdm(iter_item):
+                                start_date = self.find_begin(
+                                    self.tradedays, end_date, self.backsee
+                                )
+                                df = fac[
+                                    (fac.date >= start_date) & (fac.date <= end_date)
+                                ]
+                                df = func(df)
+                                df = df.to_frame().T
+                                df.index = [end_date]
+                                res.append(df)
+                            fac = pd.concat(res).resample("M").last()
+                            self.fac = pd.concat([old, fac])
+                        else:
+                            tqdm.auto.tqdm.pandas(
+                                desc="when the dawn comes, tonight will be a memory too."
+                            )
+                            fac = fac.groupby(["code"]).progress_apply(
+                                lambda x: self.make_monthly_factors_single_code(
+                                    x, func, daily=daily
+                                )
+                            )
+                            fac = (
+                                fac.reset_index(level=1, drop=True)
+                                .reset_index()
+                                .set_index(["date", "code"])
+                                .unstack()
+                            )
+                            fac.columns = [i[1] for i in list(fac.columns)]
+                            fac = fac.resample("M").last()
+                            self.fac = pd.concat([old, fac])
+                        self.fac.to_parquet(homeplace.update_data_file + history_file)
+                        logger.success(f"本地文件已经更新完成")
+                    except Exception:
+                        logger.info(f"本地文件已经是最新的了，无需计算")
+            else:
+                logger.info("第一次计算，请耐心等待……")
+                if whole_cross:
+                    for end_date in tqdm.auto.tqdm(iter_item):
+                        start_date = self.find_begin(
+                            self.tradedays, end_date, self.backsee
+                        )
+                        df = self.fac[
+                            (self.fac.date >= start_date) & (self.fac.date <= end_date)
+                        ]
+                        df = func(df)
+                        df = df.to_frame().T
+                        df.index = [end_date]
+                        res.append(df)
+                    self.fac = pd.concat(res).resample("M").last()
+                else:
+                    tqdm.auto.tqdm.pandas(
+                        desc="when the dawn comes, tonight will be a memory too."
+                    )
+                    self.fac = self.fac.groupby(["code"]).progress_apply(
+                        lambda x: self.make_monthly_factors_single_code(
+                            x, func, daily=daily
+                        )
+                    )
+                    self.fac = (
+                        self.fac.reset_index(level=1, drop=True)
+                        .reset_index()
+                        .set_index(["date", "code"])
+                        .unstack()
+                    )
+                    self.fac.columns = [i[1] for i in list(self.fac.columns)]
+                    self.fac = self.fac.resample("M").last()
+                self.fac.to_parquet(homeplace.update_data_file + history_file)
+                logger.success(f"本地文件已经写入完成")
+        else:
+            logger.warning("您本次计算没有指定任何本地文件路径，这很可能会导致大量的重复计算和不必要的时间浪费，请注意！")
+            if daily:
+                logger.warning("您指定的是日频计算，非月频计算，因此强烈建议您指定history_file参数！！")
+            if whole_cross:
+                for end_date in tqdm.auto.tqdm(iter_item):
+                    start_date = self.find_begin(self.tradedays, end_date, self.backsee)
+                    df = self.fac[
+                        (self.fac.date >= start_date) & (self.fac.date <= end_date)
+                    ]
+                    df = func(df)
+                    df = df.to_frame().T
+                    df.index = [end_date]
+                    res.append(df)
+                self.fac = pd.concat(res).resample("M").last()
+            else:
+                tqdm.auto.tqdm.pandas(
+                    desc="when the dawn comes, tonight will be a memory too."
+                )
+                self.fac = self.fac.groupby(["code"]).progress_apply(
+                    lambda x: self.make_monthly_factors_single_code(
+                        x, func, daily=daily
+                    )
+                )
+                self.fac = (
+                    self.fac.reset_index(level=1, drop=True)
+                    .reset_index()
+                    .set_index(["date", "code"])
+                    .unstack()
+                )
+                self.fac.columns = [i[1] for i in list(self.fac.columns)]
+                self.fac = self.fac.resample("M").last()
+
+    @kk.desktop_sender(title="嘿，切割完成啦🛁")
+    def run(
+        self,
+        func: Callable,
+        backsee: int = 20,
+        whole_cross: bool = 0,
+        daily: bool = 0,
+        history_file: str = None,
+    ) -> None:
+        """执行计算的框架，产生因子值
+
+        Parameters
+        ----------
+        func : Callable
+            每个月要进行的操作
+        backsee : int, optional
+            回看期，即每个月月底对过去多少天进行计算, by default 20
+        whole_cross : bool, optional
+            是否同时取横截面上所有股票进行计算, by default 20
+        daily : bool, optional
+            是否每日计算, by default 20
+        history_file : str, optional
+            存储历史数据的文件名, by default None
+        """
+        self.backsee = backsee
+        self.get_fac_long_and_tradedays()
+        self.get_month_starts_and_ends(backsee=backsee)
+        self.get_monthly_factor(
+            func, whole_cross=whole_cross, daily=daily, history_file=history_file
+        )
+
 def corr_two_daily(
     df1: pd.DataFrame,
     df2: pd.DataFrame,
     history: str = None,
     rolling_window: int = 20,
     n_jobs: int = 1,
+    daily: bool = 1,
+    method: str = 'pearson',
 ) -> pd.DataFrame:
     """求两个因子，在相同股票上，时序上滚动窗口下的相关系数
 
     Parameters
     ----------
     df1 : pd.DataFrame
         第一个因子，index为时间，columns为股票代码
@@ -426,40 +728,77 @@
         第二个因子，index为时间，columns为股票代码
     history : str, optional
         从某处读取计算好的历史文件
     rolling_window : int, optional
         滚动窗口, by default 20
     n_jobs : int, optional
         并行数量, by default 1
+    daily : bool, optional
+        是否每天计算, by default 1
+    method : str, optional
+        使用哪种方法计算相关系数, by default 'pearson'
 
     Returns
     -------
     pd.DataFrame
         相关系数后的结果，index为时间，columns为股票代码
     """
-
-    def corr_in(a, b, c):
-        return c.iloc[-1], np.corrcoef(a, b)[0, 1]
-
-    return func_two_daily(
-        df1=df1,
-        df2=df2,
-        func=corr_in,
-        history=history,
-        rolling_window=rolling_window,
-        n_jobs=n_jobs,
-    )
+    if daily:
+        if method=='pearson':
+            def corr_in(a, b, c):
+                return c.iloc[-1], np.corrcoef(a, b)[0, 1]
+
+            return func_two_daily(
+                df1=df1,
+                df2=df2,
+                func=corr_in,
+                history=history,
+                rolling_window=rolling_window,
+                n_jobs=n_jobs,
+            )
+        elif method=='spearman':
+            def corr_in(a, b, c):
+                return c.iloc[-1], np.corrcoef(np.argsort(a), np.argsort(b))[0, 1]
+
+            return func_two_daily(
+                df1=df1,
+                df2=df2,
+                func=corr_in,
+                history=history,
+                rolling_window=rolling_window,
+                n_jobs=n_jobs,
+            )
+        else:
+            raise ValueError('您输入的方法暂不支持')
+    else:
+        if method=='pearson':
+            class Cut(pure_dawn):
+                def cut(self,df:pd.DataFrame):
+                    return df[['fac1','fac2']].corr().iloc[0,1]
+            cut=Cut(df1,df2)
+            cut.run(cut.cut,backsee=rolling_window,history_file=history)
+            return cut()
+        elif method=='spearman':
+            class Cut(pure_dawn):
+                def cut(self,df:pd.DataFrame):
+                    return df[['fac1','fac2']].rank().corr().iloc[0,1]
+            cut=Cut(df1,df2)
+            cut.run(cut.cut,backsee=rolling_window,history_file=history)
+            return cut()
+        else:
+            raise ValueError('您输入的方法暂不支持')
 
 
 def cov_two_daily(
     df1: pd.DataFrame,
     df2: pd.DataFrame,
     history: str = None,
     rolling_window: int = 20,
     n_jobs: int = 1,
+    daily: bool = 1,
 ) -> pd.DataFrame:
     """求两个因子，在相同股票上，时序上滚动窗口下的协方差
 
     Parameters
     ----------
     df1 : pd.DataFrame
         第一个因子，index为时间，columns为股票代码
@@ -467,32 +806,41 @@
         第二个因子，index为时间，columns为股票代码
     history : str, optional
         从某处读取计算好的历史文件
     rolling_window : int, optional
         滚动窗口, by default 20
     n_jobs : int, optional
         并行数量, by default 1
+    daily : bool, optional
+        是否每天计算, by default 1
 
     Returns
     -------
     pd.DataFrame
         求协方差后的结果，index为时间，columns为股票代码
     """
-
-    def cov_in(a, b, c):
-        return c.iloc[-1], np.cov(a, b)[0, 1]
-
-    return func_two_daily(
-        df1=df1,
-        df2=df2,
-        func=cov_in,
-        history=history,
-        rolling_window=rolling_window,
-        n_jobs=n_jobs,
-    )
+    if daily:
+        def cov_in(a, b, c):
+            return c.iloc[-1], np.cov(a, b)[0, 1]
+
+        return func_two_daily(
+            df1=df1,
+            df2=df2,
+            func=cov_in,
+            history=history,
+            rolling_window=rolling_window,
+            n_jobs=n_jobs,
+        )
+    else:
+        class Cut(pure_dawn):
+            def cut(self,df:pd.DataFrame):
+                return df[['fac1','fac2']].cov().iloc[0,1]
+        cut=Cut(df1,df2)
+        cut.run(cut.cut,backsee=rolling_window,history_file=history)
+        return cut()
 
 
 def func_two_daily(
     df1: pd.DataFrame,
     df2: pd.DataFrame,
     func: Callable,
     history: str = None,
@@ -985,15 +1333,15 @@
     -------
     `pd.DataFrame`
         每天每只股票多个因子的标准差
     """
     delta_sts_mean = sum(delta_sts) / len(delta_sts)
     delta_sts_std = [(i - delta_sts_mean) ** 2 for i in delta_sts]
     delta_sts_std = sum(delta_sts_std)
-    delta_sts_std = delta_sts_std**0.5 / len(delta_sts)**0.5
+    delta_sts_std = delta_sts_std**0.5 / len(delta_sts) ** 0.5
     return delta_sts_std
 
 
 def get_list_std_weighted(delta_sts: List[pd.DataFrame], weights: list) -> pd.DataFrame:
     """对多个df对应位置上的值求加权标准差
 
     Parameters
@@ -1267,15 +1615,15 @@
                 dfs.append(df0)
             dfs = pd.concat(dfs, axis=1).T
             dfs = drop_duplicates_index(pd.concat([old, dfs]))
             dfs.to_parquet(homeplace.update_data_file + history_file)
             if daily:
                 return dfs
             else:
-                return dfs.resample('M').last()
+                return dfs.resample("M").last()
         else:
             logger.info("已经是最新的了")
             return old
     else:
         ends = list(df.index)
         ends = pd.Series(ends, index=ends)
         ends = ends.resample("M").last()
@@ -1326,15 +1674,15 @@
             dfs.append(df0)
         dfs = pd.concat(dfs, axis=1).T
         if history_file is not None:
             dfs.to_parquet(homeplace.update_data_file + history_file)
         if daily:
             return dfs
         else:
-            return dfs.resample('M').last()
+            return dfs.resample("M").last()
 
 
 @do_on_dfs
 def get_fac_cross_via_func(
     df: pd.DataFrame,
     func: Callable,
     history_file: str = None,
@@ -1505,23 +1853,37 @@
     pd.DataFrame
         变化后非负的因子值
     """
     return (df.T - df.T.min()).T
 
 
 @do_on_dfs
-def clip_mad(df: pd.DataFrame, n: float = 3) -> pd.DataFrame:
-    df0 = df.T
-    median = df0.quantile(0.5)
-    diff_median = ((df0 - median).abs()).quantile(0.5)
-    max_range = median + n * diff_median
-    min_range = median - n * diff_median
-    mid1 = (((df0 - min_range) >= 0) + 0).replace(0, np.nan)
-    mid2 = (((df0 - max_range) <= 0) + 0).replace(0, np.nan)
-    return (df0 * mid1 * mid2).T
+def clip_mad(df: pd.DataFrame, n: float = 3, replace: bool = 1) -> pd.DataFrame:
+    def clip_sing(x: pd.Series, n: float = 3):
+        median = x.quantile(0.5)
+        diff_median = ((x - median).abs()).quantile(0.5)
+        max_range = median + n * diff_median
+        min_range = median - n * diff_median
+        x = x.where(x < max_range, max_range)
+        x = x.where(x > min_range, min_range)
+        return x
+
+    if replace:
+        df1 = df.T.apply(lambda x: clip_sing(x, n)).T
+        df = np.abs(np.sign(df)) * df1
+        return df
+    else:
+        df0 = df.T
+        median = df0.quantile(0.5)
+        diff_median = ((df0 - median).abs()).quantile(0.5)
+        max_range = median + n * diff_median
+        min_range = median - n * diff_median
+        mid1 = (((df0 - min_range) >= 0) + 0).replace(0, np.nan)
+        mid2 = (((df0 - max_range) <= 0) + 0).replace(0, np.nan)
+        return (df0 * mid1 * mid2).T
 
 
 @do_on_dfs
 def clip_three_sigma(df: pd.DataFrame, n: float = 3) -> pd.DataFrame:
     df0 = df.T
     mean = df0.mean()
     std = df0.std()
```

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/data/write_data.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/data/write_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__updated__ = "2023-05-16 11:40:12"
+__updated__ = "2023-05-22 15:55:43"
 
 import time
 
 try:
     import rqdatac
 
     rqdatac.init()
@@ -288,15 +288,15 @@
         )
         # 换手率，流通股本，换手率要除以100，流通股本要乘以10000
         df2 = pro.daily_basic(
             trade_date=day,
             fields=[
                 "ts_code",
                 "trade_date",
-                "turnover_rate_f",
+                "turnover_rate",
                 "total_share",
                 "float_share",
                 "pe",
                 "pb",
             ],
         )
         time.sleep(1)
@@ -327,15 +327,15 @@
         )
         # 换手率，流通股本，换手率要除以100，流通股本要乘以10000
         df2 = pro.daily_basic(
             trade_date=day,
             fields=[
                 "ts_code",
                 "trade_date",
-                "turnover_rate_f",
+                "turnover_rate",
                 "total_share",
                 "float_share",
                 "pe",
                 "pb",
             ],
         )
         time.sleep(1)
@@ -478,16 +478,16 @@
         adjfactors = to_mat(part1, "adjfactor", "adjfactors")
         # 涨停价
         stop_ups = to_mat(part1, "limit", "stop_ups")
         # 跌停价
         stop_downs = to_mat(part1, "stopping", "stop_downs")
 
         # 换手率
-        part2 = df2s[["date", "code", "turnover_rate_f"]].pivot(
-            index="date", columns="code", values="turnover_rate_f"
+        part2 = df2s[["date", "code", "turnover_rate"]].pivot(
+            index="date", columns="code", values="turnover_rate"
         )
         part2 = part2 / 100
         part2_old = pd.read_parquet(homeplace.daily_data_file + "trs.parquet")
         part2_new = pd.concat([part2_old, part2])
         part2_new = part2_new.drop_duplicates()
         part2_new = part2_new[closes.columns]
         part2_new = part2_new[sorted(list(part2_new.columns))]
```

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/future_version/half_way.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/future_version/in_thoughts.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/initialize/initialize.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/labor/comment.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/labor/process.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/labor/process.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__updated__ = "2023-05-16 11:40:18"
+__updated__ = "2023-06-04 12:44:48"
 
 import warnings
 
 warnings.filterwarnings("ignore")
 import numpy as np
 import pandas as pd
 import knockknock as kk
@@ -1551,15 +1551,16 @@
             cls.closes = cls.closes.replace(0, np.nan)
 
     def set_factor_df_date_as_index(self, df: pd.DataFrame):
         """设置因子数据的dataframe，因子表列名应为股票代码，索引应为时间"""
         # week_here
         self.factors = df.resample(self.freq).last().dropna(how="all")
         self.factor_cover = np.sign(self.factors.abs() + 1).sum().sum()
-        total = np.sign(self.opens.resample(self.freq).last()).sum().sum()
+        opens = self.opens[self.opens.index >= self.factors.index.min()]
+        total = np.sign(opens.resample(self.freq).last()).sum().sum()
         self.factor_cover = min(self.factor_cover / total, 1)
         self.factor_cross_skew = self.factors.skew(axis=1).mean()
         pos_num = ((self.factors > 0) + 0).sum().sum()
         neg_num = ((self.factors < 0) + 0).sum().sum()
         self.pos_neg_rate = pos_num / (neg_num + pos_num)
         self.corr_itself = show_corr(self.factors, self.factors.shift(1), plt_plot=0)
         self.corr_itself_shift2 = show_corr(
@@ -3963,305 +3964,14 @@
         -------
         `pd.DataFrame`
             每个组的年化收益率
         """
         return self.square_rets.copy()
 
 
-class pure_dawn(object):
-    """
-    因子切割论的母框架，可以对两个因子进行类似于因子切割的操作
-    可用于派生任何"以两个因子生成一个因子"的子类
-    使用举例
-    cut函数里，必须带有输入变量df,df有两个columns，一个名为'fac1'，一个名为'fac2'，df是最近一个回看期内的数据
-    ```python
-    class Cut(pure_dawn):
-
-    def cut(self,df):
-        df=df.sort_values('fac1')
-        df=df.assign(fac3=df.fac1*df.fac2)
-        ret0=df.fac2.iloc[:4].mean()
-        ret1=df.fac2.iloc[4:8].mean()
-        ret2=df.fac2.iloc[8:12].mean()
-        ret3=df.fac2.iloc[12:16].mean()
-        ret4=df.fac2.iloc[16:].mean()
-        aret0=df.fac3.iloc[:4].mean()
-        aret1=df.fac3.iloc[4:8].mean()
-        aret2=df.fac3.iloc[8:12].mean()
-        aret3=df.fac3.iloc[12:16].mean()
-        aret4=df.fac3.iloc[16:].mean()
-        return ret0,ret1,ret2,ret3,ret4,aret0,aret1,aret2,aret3,aret4
-
-    cut=Cut(ct,ret_inday)
-    cut.run(cut.cut)
-
-    cut0=get_value(cut(),0)
-    cut1=get_value(cut(),1)
-    cut2=get_value(cut(),2)
-    cut3=get_value(cut(),3)
-    cut4=get_value(cut(),4)
-    ```
-    """
-
-    def __init__(self, fac1: pd.DataFrame, fac2: pd.DataFrame, *args: list) -> None:
-        """几个因子的操作，每个月操作一次
-
-        Parameters
-        ----------
-        fac1 : pd.DataFrame
-            因子值1，index为时间，columns为股票代码，values为因子值
-        fac2 : pd.DataFrame
-            因子2，index为时间，columns为股票代码，values为因子值
-        """
-        self.fac1 = fac1
-        self.fac1 = self.fac1.stack().reset_index()
-        self.fac1.columns = ["date", "code", "fac1"]
-        self.fac2 = fac2
-        self.fac2 = self.fac2.stack().reset_index()
-        self.fac2.columns = ["date", "code", "fac2"]
-        fac_all = pd.merge(self.fac1, self.fac2, on=["date", "code"])
-        for i, fac in enumerate(args):
-            fac = fac.stack().reset_index()
-            fac.columns = ["date", "code", f"fac{i+3}"]
-            fac_all = pd.merge(fac_all, fac, on=["date", "code"])
-        fac_all = fac_all.sort_values(["date", "code"])
-        self.fac = fac_all.copy()
-
-    def __call__(self) -> pd.DataFrame:
-        """返回最终月度因子值
-
-        Returns
-        -------
-        `pd.DataFrame`
-            最终因子值
-        """
-        return self.fac.copy()
-
-    def get_fac_long_and_tradedays(self):
-        """将两个因子的矩阵转化为长列表"""
-        self.tradedays = sorted(list(set(self.fac.date)))
-
-    def get_month_starts_and_ends(self, backsee=20):
-        """计算出每个月回看期间的起点日和终点日"""
-        self.month_ends = [
-            i
-            for i, j in zip(self.tradedays[:-1], self.tradedays[1:])
-            if i.month != j.month
-        ]
-        self.month_ends.append(self.tradedays[-1])
-        self.month_starts = [
-            self.find_begin(self.tradedays, i, backsee=backsee) for i in self.month_ends
-        ]
-        self.month_starts[0] = self.tradedays[0]
-
-    def find_begin(self, tradedays, end_day, backsee=20):
-        """找出回看若干天的开始日，默认为20"""
-        end_day_index = tradedays.index(end_day)
-        start_day_index = end_day_index - backsee + 1
-        start_day = tradedays[start_day_index]
-        return start_day
-
-    def make_monthly_factors_single_code(self, df, func, daily):
-        """
-        对单一股票来计算月度因子
-        func为单月执行的函数，返回值应为月度因子，如一个float或一个list
-        df为一个股票的四列表，包含时间、代码、因子1和因子2
-        """
-        res = {}
-        if daily:
-            ones = [self.find_begin(i) for i in self.tradedays[self.backsee - 1 :]]
-            twos = self.tradedays[self.backsee - 1 :]
-        else:
-            ones = self.month_starts
-            twos = self.month_ends
-        for start, end in zip(ones, twos):
-            this_month = df[(df.date >= start) & (df.date <= end)]
-            res[end] = func(this_month)
-        dates = list(res.keys())
-        corrs = list(res.values())
-        part = pd.DataFrame({"date": dates, "corr": corrs})
-        return part
-
-    @staticmethod
-    def for_cross_via_zip(func):
-        """返回值为多个pd.Series，每个pd.Series的index为股票代码，values为单个因子值
-        例如
-        ```python
-        return (
-                    pd.Series([1.54,8.77,9.99……],index=['000001.SZ','000002.SZ','000004.SZ'……]),
-                    pd.Series([3.54,6.98,9.01……],index=['000001.SZ','000002.SZ','000004.SZ'……]),
-                )
-        ```
-        上例中，每个股票一天返回两个因子值，每个pd.Series对应一个因子值
-        """
-
-        def full_run(df, *args, **kwargs):
-            res = func(df, *args, **kwargs)
-            if isinstance(res, pd.Series):
-                return res
-            else:
-                res = pd.concat(res, axis=1)
-                res.columns = [f"fac{i}" for i in range(len(res.columns))]
-                res = res.assign(fac=list(zip(*[res[i] for i in list(res.columns)])))
-                return res.fac
-
-        return full_run
-
-    def get_monthly_factor(
-        self, func, whole_cross: bool = 0, daily: bool = 0, history_file: str = None
-    ):
-        """运行自己写的函数，获得月度因子"""
-        if daily:
-            iter_item = self.tradedays[self.backsee - 1 :]
-        else:
-            iter_item = self.month_ends
-        res = []
-        if history_file is not None:
-            if os.path.exists(homeplace.update_data_file + history_file):
-                old = pd.read_parquet(homeplace.update_data_file + history_file)
-                old_date = old.index.max()
-                if old_date == self.fac.date.max():
-                    logger.info(f"本地文件已经是最新的了，无需计算")
-                else:
-                    try:
-                        new_date = self.find_begin(self.tradedays, old_date, self.backsee)
-                        fac = self.fac[self.fac.date > new_date]
-                        iter_item = [i for i in iter_item if i > new_date]
-                        if whole_cross:
-                            for end_date in tqdm.auto.tqdm(iter_item):
-                                start_date = self.find_begin(
-                                    self.tradedays, end_date, self.backsee
-                                )
-                                df = fac[(fac.date >= start_date) & (fac.date <= end_date)]
-                                df = func(df)
-                                df = df.to_frame().T
-                                df.index = [end_date]
-                                res.append(df)
-                            fac = pd.concat(res).resample("M").last()
-                            self.fac = pd.concat([old, fac])
-                        else:
-                            tqdm.auto.tqdm.pandas(
-                                desc="when the dawn comes, tonight will be a memory too."
-                            )
-                            fac = fac.groupby(["code"]).progress_apply(
-                                lambda x: self.make_monthly_factors_single_code(
-                                    x, func, daily=daily
-                                )
-                            )
-                            fac = (
-                                fac.reset_index(level=1, drop=True)
-                                .reset_index()
-                                .set_index(["date", "code"])
-                                .unstack()
-                            )
-                            fac.columns = [i[1] for i in list(fac.columns)]
-                            fac = fac.resample("M").last()
-                            self.fac = pd.concat([old, fac])
-                        self.fac.to_parquet(homeplace.update_data_file + history_file)
-                        logger.success(f"本地文件已经更新完成")
-                    except Exception:
-                        logger.info(f"本地文件已经是最新的了，无需计算")
-            else:
-                logger.info("第一次计算，请耐心等待……")
-                if whole_cross:
-                    for end_date in tqdm.auto.tqdm(iter_item):
-                        start_date = self.find_begin(
-                            self.tradedays, end_date, self.backsee
-                        )
-                        df = self.fac[
-                            (self.fac.date >= start_date) & (self.fac.date <= end_date)
-                        ]
-                        df = func(df)
-                        df = df.to_frame().T
-                        df.index = [end_date]
-                        res.append(df)
-                    self.fac = pd.concat(res).resample("M").last()
-                else:
-                    tqdm.auto.tqdm.pandas(
-                        desc="when the dawn comes, tonight will be a memory too."
-                    )
-                    self.fac = self.fac.groupby(["code"]).progress_apply(
-                        lambda x: self.make_monthly_factors_single_code(
-                            x, func, daily=daily
-                        )
-                    )
-                    self.fac = (
-                        self.fac.reset_index(level=1, drop=True)
-                        .reset_index()
-                        .set_index(["date", "code"])
-                        .unstack()
-                    )
-                    self.fac.columns = [i[1] for i in list(self.fac.columns)]
-                    self.fac = self.fac.resample("M").last()
-                self.fac.to_parquet(homeplace.update_data_file + history_file)
-                logger.success(f"本地文件已经写入完成")
-        else:
-            logger.warning("您本次计算没有指定任何本地文件路径，这很可能会导致大量的重复计算和不必要的时间浪费，请注意！")
-            if daily:
-                logger.warning("您指定的是日频计算，非月频计算，因此强烈建议您指定history_file参数！！")
-            if whole_cross:
-                for end_date in tqdm.auto.tqdm(iter_item):
-                    start_date = self.find_begin(self.tradedays, end_date, self.backsee)
-                    df = self.fac[
-                        (self.fac.date >= start_date) & (self.fac.date <= end_date)
-                    ]
-                    df = func(df)
-                    df = df.to_frame().T
-                    df.index = [end_date]
-                    res.append(df)
-                self.fac = pd.concat(res).resample("M").last()
-            else:
-                tqdm.auto.tqdm.pandas(
-                    desc="when the dawn comes, tonight will be a memory too."
-                )
-                self.fac = self.fac.groupby(["code"]).progress_apply(
-                    lambda x: self.make_monthly_factors_single_code(
-                        x, func, daily=daily
-                    )
-                )
-                self.fac = (
-                    self.fac.reset_index(level=1, drop=True)
-                    .reset_index()
-                    .set_index(["date", "code"])
-                    .unstack()
-                )
-                self.fac.columns = [i[1] for i in list(self.fac.columns)]
-                self.fac = self.fac.resample("M").last()
-
-    @kk.desktop_sender(title="嘿，切割完成啦🛁")
-    def run(
-        self,
-        func: Callable,
-        backsee: int = 20,
-        whole_cross: bool = 0,
-        daily: bool = 0,
-        history_file: str = None,
-    ) -> None:
-        """执行计算的框架，产生因子值
-
-        Parameters
-        ----------
-        func : Callable
-            每个月要进行的操作
-        backsee : int, optional
-            回看期，即每个月月底对过去多少天进行计算, by default 20
-        whole_cross : bool, optional
-            是否同时取横截面上所有股票进行计算, by default 20
-        daily : bool, optional
-            是否每日计算, by default 20
-        history_file : str, optional
-            存储历史数据的文件名, by default None
-        """
-        self.backsee = backsee
-        self.get_fac_long_and_tradedays()
-        self.get_month_starts_and_ends(backsee=backsee)
-        self.get_monthly_factor(
-            func, whole_cross=whole_cross, daily=daily, history_file=history_file
-        )
-
 
 @do_on_dfs
 def follow_tests(
     fac: pd.DataFrame,
     trade_cost_double_side_list: float = [0.001, 0.002, 0.003, 0.004, 0.005],
     index_member_value_weighted: bool = 1,
     comments_writer: pd.ExcelWriter = None,
@@ -4893,15 +4603,15 @@
         self.factors_group_long = [(i == 0) + 0 for i in self.factors_group]
         self.factors_group_short = [
             (i == (j - 1)) + 0 for i, j in zip(self.factors_group, self.minus_group)
         ]
         self.value_weighted = value_weighted
         if value_weighted:
             if total_cap:
-                self.cap=read_daily(total_cap=1,start=start)
+                self.cap = read_daily(total_cap=1, start=start)
             self.cap = read_daily(flow_cap=1, start=start)
             self.factors_group_long = [self.cap * i for i in self.factors_group_long]
             self.factors_group_short = [self.cap * i for i in self.factors_group_short]
             self.factors_group_long = [
                 (i.T / i.T.sum()).T for i in self.factors_group_long
             ]
             self.factors_group_short = [
@@ -5186,15 +4896,15 @@
     boxcox: bool = 0,
     hs300: bool = 0,
     zz500: bool = 0,
     zz1000: bool = 0,
     gz2000: bool = 0,
     iplot: bool = 1,
     opens_average_first_day: bool = 0,
-    total_cap: bool=0,
+    total_cap: bool = 0,
 ) -> pd.Series:
     """对因子在指数成分股内进行多空和多头测试
 
     Parameters
     ----------
     df : pd.DataFrame
         因子值，index为时间，columns为股票代码
```

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v1/initialize.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v1/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v1p10/initialize.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v1p10/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v2/initialize.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v2/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/__init__.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/data/database.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/data/tools.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/data/tools.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/labor/process.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/labor/process.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/mail/email.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/__init__.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/data/database.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/data/tools.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/data/tools.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/labor/process.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/labor/process.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/mail/email.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/state/states.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/state/states.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/mail/email.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/state/decorators.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/state/homeplace.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/state/states.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/state/states.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze/withs/requires.py` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze.egg-info/PKG-INFO` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure-ocean-breeze
-Version: 3.9.5
+Version: 3.9.6
 Summary: stock factor test
 Home-page: https://github.com/chen-001/pure_ocean_breeze.git
 Author: chenzongwei
 Author-email: winterwinter999@163.com
 License: MIT
 Project-URL: Documentation, https://chen-001.github.io/pure_ocean_breeze/
 Requires-Python: >=3
```

### Comparing `pure_ocean_breeze-3.9.5/pure_ocean_breeze.egg-info/SOURCES.txt` & `pure_ocean_breeze-3.9.6/pure_ocean_breeze.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.5/setup.py` & `pure_ocean_breeze-3.9.6/setup.py`

 * *Files identical despite different names*

