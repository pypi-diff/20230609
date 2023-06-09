# Comparing `tmp/charex-0.1.0.tar.gz` & `tmp/charex-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charex-0.1.0.tar", last modified: Tue May 23 13:08:01 2023, max compression
+gzip compressed data, was "charex-0.2.0.tar", last modified: Fri Jun  9 13:08:03 2023, max compression
```

## Comparing `charex-0.1.0.tar` & `charex-0.2.0.tar`

### file list

```diff
@@ -1,55 +1,82 @@
-drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-05-23 13:08:01.291814 charex-0.1.0/
--rw-r--r--   0 pji        (501) staff       (20)     1069 2023-04-20 18:29:08.000000 charex-0.1.0/LICENSE
--rw-r--r--   0 pji        (501) staff       (20)       38 2023-05-17 17:45:10.000000 charex-0.1.0/MANIFEST.in
--rw-r--r--   0 pji        (501) staff       (20)     3814 2023-05-23 13:08:01.292041 charex-0.1.0/PKG-INFO
--rw-r--r--   0 pji        (501) staff       (20)     3237 2023-05-23 13:06:42.000000 charex-0.1.0/README.rst
-drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-05-23 13:08:01.258610 charex-0.1.0/charex/
--rw-r--r--   0 pji        (501) staff       (20)      439 2023-05-23 13:07:32.000000 charex-0.1.0/charex/__init__.py
--rw-r--r--   0 pji        (501) staff       (20)      402 2023-05-23 13:07:32.000000 charex-0.1.0/charex/__main__.py
--rw-r--r--   0 pji        (501) staff       (20)    10751 2023-05-23 13:07:32.000000 charex-0.1.0/charex/charex.py
--rw-r--r--   0 pji        (501) staff       (20)    15753 2023-05-23 13:07:32.000000 charex-0.1.0/charex/charsets.py
--rw-r--r--   0 pji        (501) staff       (20)     8926 2023-05-23 13:07:32.000000 charex-0.1.0/charex/cmds.py
-drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-05-23 13:08:01.285359 charex-0.1.0/charex/data/
--rw-r--r--   0 pji        (501) staff       (20)    76759 2023-04-24 18:02:02.000000 charex-0.1.0/charex/data/PropertyValueAliases.txt
--rw-r--r--   0 pji        (501) staff       (20)  1897793 2023-04-28 15:11:52.000000 charex-0.1.0/charex/data/UnicodeData.txt
--rw-r--r--   0 pji        (501) staff       (20)        0 2023-04-21 22:16:00.000000 charex-0.1.0/charex/data/__init__.py
-drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-05-23 13:08:01.286667 charex-0.1.0/charex/data/__pycache__/
--rw-r--r--   0 pji        (501) staff       (20)      154 2023-04-25 11:55:58.000000 charex-0.1.0/charex/data/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 pji        (501) staff       (20)   145897 2023-05-11 13:10:11.000000 charex-0.1.0/charex/data/entities.json
--rw-r--r--   0 pji        (501) staff       (20)      126 2023-05-08 18:24:17.000000 charex-0.1.0/charex/data/help_xt.txt
--rw-r--r--   0 pji        (501) staff       (20)      574 2023-05-04 17:01:12.000000 charex-0.1.0/charex/data/quote.html
--rw-r--r--   0 pji        (501) staff       (20)      573 2023-05-05 11:29:50.000000 charex-0.1.0/charex/data/result.html
--rw-r--r--   0 pji        (501) staff       (20)    99273 2023-05-17 16:34:15.000000 charex-0.1.0/charex/data/rev_casefold.json
--rw-r--r--   0 pji        (501) staff       (20)   685484 2023-05-17 16:25:24.000000 charex-0.1.0/charex/data/rev_nfc.json
--rw-r--r--   0 pji        (501) staff       (20)   676626 2023-05-17 16:28:18.000000 charex-0.1.0/charex/data/rev_nfd.json
--rw-r--r--   0 pji        (501) staff       (20)   802292 2023-05-17 16:29:56.000000 charex-0.1.0/charex/data/rev_nfkc.json
--rw-r--r--   0 pji        (501) staff       (20)   793983 2023-05-17 16:28:34.000000 charex-0.1.0/charex/data/rev_nfkd.json
--rw-r--r--   0 pji        (501) staff       (20)      391 2023-05-11 13:19:35.000000 charex-0.1.0/charex/data/sources.json
--rw-r--r--   0 pji        (501) staff       (20)     9341 2023-05-23 13:07:32.000000 charex-0.1.0/charex/denormal.py
--rw-r--r--   0 pji        (501) staff       (20)    15455 2023-05-23 13:07:32.000000 charex-0.1.0/charex/escape.py
--rw-r--r--   0 pji        (501) staff       (20)    14795 2023-05-23 13:07:32.000000 charex-0.1.0/charex/gui.py
--rw-r--r--   0 pji        (501) staff       (20)     2883 2023-05-23 13:07:32.000000 charex-0.1.0/charex/http.py
--rw-r--r--   0 pji        (501) staff       (20)     5064 2023-05-23 13:07:32.000000 charex-0.1.0/charex/normal.py
--rw-r--r--   0 pji        (501) staff       (20)    20293 2023-05-23 13:07:32.000000 charex-0.1.0/charex/shell.py
-drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-05-23 13:08:01.253335 charex-0.1.0/charex/static/
-drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-05-23 13:08:01.287056 charex-0.1.0/charex/static/styles/
--rw-r--r--   0 pji        (501) staff       (20)      455 2023-05-05 11:30:23.000000 charex-0.1.0/charex/static/styles/styles.css
--rw-r--r--   0 pji        (501) staff       (20)     6431 2023-05-23 13:07:32.000000 charex-0.1.0/charex/util.py
-drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-05-23 13:08:01.260939 charex-0.1.0/charex.egg-info/
--rw-r--r--   0 pji        (501) staff       (20)     3814 2023-05-23 13:08:01.000000 charex-0.1.0/charex.egg-info/PKG-INFO
--rw-r--r--   0 pji        (501) staff       (20)     1032 2023-05-23 13:08:01.000000 charex-0.1.0/charex.egg-info/SOURCES.txt
--rw-r--r--   0 pji        (501) staff       (20)        1 2023-05-23 13:08:01.000000 charex-0.1.0/charex.egg-info/dependency_links.txt
--rw-r--r--   0 pji        (501) staff       (20)       48 2023-05-23 13:08:01.000000 charex-0.1.0/charex.egg-info/entry_points.txt
--rw-r--r--   0 pji        (501) staff       (20)        6 2023-05-23 13:08:01.000000 charex-0.1.0/charex.egg-info/requires.txt
--rw-r--r--   0 pji        (501) staff       (20)        7 2023-05-23 13:08:01.000000 charex-0.1.0/charex.egg-info/top_level.txt
--rw-r--r--   0 pji        (501) staff       (20)      895 2023-05-23 12:57:29.000000 charex-0.1.0/pyproject.toml
--rw-r--r--   0 pji        (501) staff       (20)      221 2023-05-23 13:08:01.292891 charex-0.1.0/setup.cfg
-drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-05-23 13:08:01.291193 charex-0.1.0/tests/
--rw-r--r--   0 pji        (501) staff       (20)     6498 2023-05-23 13:07:32.000000 charex-0.1.0/tests/test_charex.py
--rw-r--r--   0 pji        (501) staff       (20)     2909 2023-05-23 13:07:32.000000 charex-0.1.0/tests/test_charset.py
--rw-r--r--   0 pji        (501) staff       (20)     2783 2023-05-23 13:07:32.000000 charex-0.1.0/tests/test_denormal.py
--rw-r--r--   0 pji        (501) staff       (20)     8775 2023-05-23 13:07:32.000000 charex-0.1.0/tests/test_escape.py
--rw-r--r--   0 pji        (501) staff       (20)     8113 2023-05-23 13:07:32.000000 charex-0.1.0/tests/test_main.py
--rw-r--r--   0 pji        (501) staff       (20)     3274 2023-05-23 13:07:32.000000 charex-0.1.0/tests/test_normal.py
--rw-r--r--   0 pji        (501) staff       (20)     5986 2023-05-23 13:07:32.000000 charex-0.1.0/tests/test_shell.py
--rw-r--r--   0 pji        (501) staff       (20)     5410 2023-05-23 13:07:32.000000 charex-0.1.0/tests/test_utility.py
+drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-06-09 13:08:03.477691 charex-0.2.0/
+-rw-r--r--   0 pji        (501) staff       (20)     1069 2023-04-20 18:29:08.000000 charex-0.2.0/LICENSE
+-rw-r--r--   0 pji        (501) staff       (20)       38 2023-05-17 17:45:10.000000 charex-0.2.0/MANIFEST.in
+-rw-r--r--   0 pji        (501) staff       (20)     5813 2023-06-09 13:08:03.477815 charex-0.2.0/PKG-INFO
+-rw-r--r--   0 pji        (501) staff       (20)     5236 2023-06-09 13:02:32.000000 charex-0.2.0/README.rst
+drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-06-09 13:08:03.426774 charex-0.2.0/charex/
+-rw-r--r--   0 pji        (501) staff       (20)      639 2023-06-09 13:06:54.000000 charex-0.2.0/charex/__init__.py
+-rw-r--r--   0 pji        (501) staff       (20)      402 2023-06-09 13:06:54.000000 charex-0.2.0/charex/__main__.py
+-rw-r--r--   0 pji        (501) staff       (20)    44948 2023-06-09 13:06:54.000000 charex-0.2.0/charex/charex.py
+-rw-r--r--   0 pji        (501) staff       (20)    18486 2023-06-09 13:06:54.000000 charex-0.2.0/charex/charsets.py
+-rw-r--r--   0 pji        (501) staff       (20)    12467 2023-06-09 13:06:54.000000 charex-0.2.0/charex/cmds.py
+drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-06-09 13:08:03.472960 charex-0.2.0/charex/data/
+-rw-r--r--   0 pji        (501) staff       (20)    26690 2023-06-07 15:56:44.000000 charex-0.2.0/charex/data/BidiMirroring.txt
+-rw-r--r--   0 pji        (501) staff       (20)    10720 2023-06-07 15:56:44.000000 charex-0.2.0/charex/data/Blocks.txt
+-rw-r--r--   0 pji        (501) staff       (20)    84688 2023-06-07 15:56:44.000000 charex-0.2.0/charex/data/CaseFolding.txt
+-rw-r--r--   0 pji        (501) staff       (20)     8911 2023-06-07 15:56:45.000000 charex-0.2.0/charex/data/CompositionExclusions.txt
+-rw-r--r--   0 pji        (501) staff       (20)   128380 2023-06-05 12:29:22.000000 charex-0.2.0/charex/data/DerivedAge.txt
+-rw-r--r--   0 pji        (501) staff       (20)  1040794 2023-06-07 15:56:45.000000 charex-0.2.0/charex/data/DerivedCoreProperties.txt
+-rw-r--r--   0 pji        (501) staff       (20)    24707 2023-06-07 15:56:45.000000 charex-0.2.0/charex/data/DerivedJoiningGroup.txt
+-rw-r--r--   0 pji        (501) staff       (20)    38319 2023-06-07 15:56:45.000000 charex-0.2.0/charex/data/DerivedJoiningType.txt
+-rw-r--r--   0 pji        (501) staff       (20)   831846 2023-06-07 15:56:45.000000 charex-0.2.0/charex/data/DerivedNormalizationProps.txt
+-rw-r--r--   0 pji        (501) staff       (20)   184037 2023-06-06 17:13:09.000000 charex-0.2.0/charex/data/EastAsianWidth.txt
+-rw-r--r--   0 pji        (501) staff       (20)    18334 2023-06-07 15:56:46.000000 charex-0.2.0/charex/data/EquivalentUnifiedIdeograph.txt
+-rw-r--r--   0 pji        (501) staff       (20)    95663 2023-06-07 15:56:46.000000 charex-0.2.0/charex/data/GraphemeBreakProperty.txt
+-rw-r--r--   0 pji        (501) staff       (20)    51346 2023-06-07 15:56:46.000000 charex-0.2.0/charex/data/HangulSyllableType.txt
+-rw-r--r--   0 pji        (501) staff       (20)    49204 2023-06-07 15:56:46.000000 charex-0.2.0/charex/data/IndicPositionalCategory.txt
+-rw-r--r--   0 pji        (501) staff       (20)    80085 2023-06-07 15:56:47.000000 charex-0.2.0/charex/data/IndicSyllabicCategory.txt
+-rw-r--r--   0 pji        (501) staff       (20)     3237 2023-06-07 15:56:47.000000 charex-0.2.0/charex/data/Jamo.txt
+-rw-r--r--   0 pji        (501) staff       (20)   245067 2023-06-07 15:56:47.000000 charex-0.2.0/charex/data/LineBreak.txt
+-rw-r--r--   0 pji        (501) staff       (20)    16120 2023-06-07 15:56:47.000000 charex-0.2.0/charex/data/NameAliases.txt
+-rw-r--r--   0 pji        (501) staff       (20)   130164 2023-06-07 15:56:47.000000 charex-0.2.0/charex/data/PropList.txt
+-rw-r--r--   0 pji        (501) staff       (20)     8825 2023-06-06 12:12:20.000000 charex-0.2.0/charex/data/PropertyAliases.txt
+-rw-r--r--   0 pji        (501) staff       (20)    76759 2023-06-07 15:56:47.000000 charex-0.2.0/charex/data/PropertyValueAliases.txt
+-rw-r--r--   0 pji        (501) staff       (20)    21969 2023-06-07 15:56:50.000000 charex-0.2.0/charex/data/ScriptExtensions.txt
+-rw-r--r--   0 pji        (501) staff       (20)   181635 2023-06-07 15:56:49.000000 charex-0.2.0/charex/data/Scripts.txt
+-rw-r--r--   0 pji        (501) staff       (20)   211457 2023-06-07 15:56:50.000000 charex-0.2.0/charex/data/SentenceBreakProperty.txt
+-rw-r--r--   0 pji        (501) staff       (20)    16830 2023-06-07 15:56:50.000000 charex-0.2.0/charex/data/SpecialCasing.txt
+-rw-r--r--   0 pji        (501) staff       (20)  1897793 2023-06-07 15:56:50.000000 charex-0.2.0/charex/data/UnicodeData.txt
+-rw-r--r--   0 pji        (501) staff       (20)   178861 2023-06-07 15:56:50.000000 charex-0.2.0/charex/data/VerticalOrientation.txt
+-rw-r--r--   0 pji        (501) staff       (20)   107025 2023-06-07 15:56:51.000000 charex-0.2.0/charex/data/WordBreakProperty.txt
+-rw-r--r--   0 pji        (501) staff       (20)        0 2023-04-21 22:16:00.000000 charex-0.2.0/charex/data/__init__.py
+drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-06-09 13:08:03.474090 charex-0.2.0/charex/data/__pycache__/
+-rw-r--r--   0 pji        (501) staff       (20)      154 2023-04-25 11:55:58.000000 charex-0.2.0/charex/data/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 pji        (501) staff       (20)   109396 2023-06-07 15:56:46.000000 charex-0.2.0/charex/data/emoji-data.txt
+-rw-r--r--   0 pji        (501) staff       (20)   145897 2023-06-07 15:56:46.000000 charex-0.2.0/charex/data/entities.json
+-rw-r--r--   0 pji        (501) staff       (20)      126 2023-05-08 18:24:17.000000 charex-0.2.0/charex/data/help_xt.txt
+-rw-r--r--   0 pji        (501) staff       (20)      574 2023-05-04 17:01:12.000000 charex-0.2.0/charex/data/quote.html
+-rw-r--r--   0 pji        (501) staff       (20)      573 2023-05-05 11:29:50.000000 charex-0.2.0/charex/data/result.html
+-rw-r--r--   0 pji        (501) staff       (20)    99271 2023-06-07 15:56:48.000000 charex-0.2.0/charex/data/rev_casefold.json
+-rw-r--r--   0 pji        (501) staff       (20)   685482 2023-06-07 15:56:48.000000 charex-0.2.0/charex/data/rev_nfc.json
+-rw-r--r--   0 pji        (501) staff       (20)   676624 2023-06-07 15:56:49.000000 charex-0.2.0/charex/data/rev_nfd.json
+-rw-r--r--   0 pji        (501) staff       (20)   802290 2023-06-07 15:56:49.000000 charex-0.2.0/charex/data/rev_nfkc.json
+-rw-r--r--   0 pji        (501) staff       (20)   793981 2023-06-07 15:56:49.000000 charex-0.2.0/charex/data/rev_nfkd.json
+-rw-r--r--   0 pji        (501) staff       (20)    10827 2023-06-07 15:56:51.000000 charex-0.2.0/charex/data/sources.json
+-rw-r--r--   0 pji        (501) staff       (20)    11503 2023-06-09 13:06:54.000000 charex-0.2.0/charex/denormal.py
+-rw-r--r--   0 pji        (501) staff       (20)    16487 2023-06-09 13:06:54.000000 charex-0.2.0/charex/escape.py
+-rw-r--r--   0 pji        (501) staff       (20)    18657 2023-06-09 13:06:54.000000 charex-0.2.0/charex/gui.py
+-rw-r--r--   0 pji        (501) staff       (20)     2883 2023-06-09 13:06:54.000000 charex-0.2.0/charex/http.py
+-rw-r--r--   0 pji        (501) staff       (20)     5810 2023-06-09 13:06:54.000000 charex-0.2.0/charex/normal.py
+-rw-r--r--   0 pji        (501) staff       (20)    24863 2023-06-09 13:06:54.000000 charex-0.2.0/charex/shell.py
+drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-06-09 13:08:03.420282 charex-0.2.0/charex/static/
+drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-06-09 13:08:03.474508 charex-0.2.0/charex/static/styles/
+-rw-r--r--   0 pji        (501) staff       (20)      455 2023-05-05 11:30:23.000000 charex-0.2.0/charex/static/styles/styles.css
+-rw-r--r--   0 pji        (501) staff       (20)    10516 2023-06-09 13:06:54.000000 charex-0.2.0/charex/util.py
+drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-06-09 13:08:03.428510 charex-0.2.0/charex.egg-info/
+-rw-r--r--   0 pji        (501) staff       (20)     5813 2023-06-09 13:08:03.000000 charex-0.2.0/charex.egg-info/PKG-INFO
+-rw-r--r--   0 pji        (501) staff       (20)     1908 2023-06-09 13:08:03.000000 charex-0.2.0/charex.egg-info/SOURCES.txt
+-rw-r--r--   0 pji        (501) staff       (20)        1 2023-06-09 13:08:03.000000 charex-0.2.0/charex.egg-info/dependency_links.txt
+-rw-r--r--   0 pji        (501) staff       (20)       48 2023-06-09 13:08:03.000000 charex-0.2.0/charex.egg-info/entry_points.txt
+-rw-r--r--   0 pji        (501) staff       (20)        6 2023-06-09 13:08:03.000000 charex-0.2.0/charex.egg-info/requires.txt
+-rw-r--r--   0 pji        (501) staff       (20)        7 2023-06-09 13:08:03.000000 charex-0.2.0/charex.egg-info/top_level.txt
+-rw-r--r--   0 pji        (501) staff       (20)      895 2023-06-09 13:05:06.000000 charex-0.2.0/pyproject.toml
+-rw-r--r--   0 pji        (501) staff       (20)      221 2023-06-09 13:08:03.478278 charex-0.2.0/setup.cfg
+drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-06-09 13:08:03.477450 charex-0.2.0/tests/
+-rw-r--r--   0 pji        (501) staff       (20)    10509 2023-06-09 13:06:54.000000 charex-0.2.0/tests/test_charex.py
+-rw-r--r--   0 pji        (501) staff       (20)     4336 2023-06-09 13:06:54.000000 charex-0.2.0/tests/test_charset.py
+-rw-r--r--   0 pji        (501) staff       (20)     2783 2023-06-09 13:06:54.000000 charex-0.2.0/tests/test_denormal.py
+-rw-r--r--   0 pji        (501) staff       (20)     9077 2023-06-09 13:06:54.000000 charex-0.2.0/tests/test_escape.py
+-rw-r--r--   0 pji        (501) staff       (20)    11382 2023-06-09 13:06:54.000000 charex-0.2.0/tests/test_main.py
+-rw-r--r--   0 pji        (501) staff       (20)     3275 2023-06-09 13:06:54.000000 charex-0.2.0/tests/test_normal.py
+-rw-r--r--   0 pji        (501) staff       (20)     7690 2023-06-09 13:06:54.000000 charex-0.2.0/tests/test_shell.py
+-rw-r--r--   0 pji        (501) staff       (20)     6010 2023-06-09 13:06:54.000000 charex-0.2.0/tests/test_utility.py
```

### Comparing `charex-0.1.0/LICENSE` & `charex-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `charex-0.1.0/charex/charsets.py` & `charex-0.2.0/charex/charsets.py`

 * *Files 21% similar despite different names*

```diff
@@ -541,64 +541,94 @@
 
 # Functions.
 def get_codecs() -> tuple[str, ...]:
     """Return the keys of the registered codecs.
 
     :return: The keys of the codecs as a :class:`tuple`.
     :rtype: tuple
+
+    Usage
+    -----
+    To get a tuple containing the keys of the registered codecs::
+
+        >>> get_codecs()                        # +ELLIPSIS
+        ('ascii', 'big5', 'big5hkscs', 'cp037'... 'utf_8', 'utf_8_sig')
     """
     return tuple(codec for codec in codecs)
 
 
-def get_codec_description(codec: str) -> str:
-    """Provide the description for the given codec."""
-    info = codecs[codec]
-    return info.description
+def get_description(codeckey: str) -> str:
+    """Provide the description for the given codec.
 
+    :param codeckey: The key for the codec.
+    :return: The description of the codec as a :class:`str`.
+    :rtype: str
+
+    Usage
+    -----
+    To get the description for the given codec key::
 
-def multiencode(
-    value: bytes | int | str,
-    codecs_: Iterator[str]
-) -> dict[str, bytes]:
-    """Provide the address for the given character for each of the
-    given character sets.
+        >>> get_description('ascii')
+        'RFC20 The ASCII format for Network Interchange.'
 
-    :param value: The character to encode.
-    :param codecs_: The codecs to encode to.
-    :return: The encoded value for each character set as a :class:`dict`.
-    :rtype: dict
     """
-    value = util.to_char(value)
-    results = {}
-    for codec in codecs_:
-        try:
-            results[codec] = value.encode(codec)
-        except UnicodeEncodeError:
-            results[codec] = b''
-    return results
+    info = codecs[codeckey]
+    return info.description
 
 
 def multidecode(
     value: int | str | bytes,
-    codecs_: Iterator[str]
+    codecs_: Iterator[str] | None = None
 ) -> dict[str, str]:
-    """Provide the code point for the given address for each of the
+    """Provide the character for the given address for each of the
     given character sets.
 
-    :param value: The address to decode. This can be passed as either
-        an :class:`int`, :class:`str`, or :class:`bytes`.
+    :param value: The address to decode.
     :param codec_: The codecs to decode to.
     :return: The decoded value for each character set as a :class:`dict`.
     :rtype: dict
+
+    Address Formats
+    ---------------
+    The understood :class:`str` formats for manual input are:
+
+    *   Character: A string with length equal to one.
+    *   Code Point: The prefix "U+" followed by a hexadecimal number.
+    *   Binary String: The prefix "0b" followed by a binary number.
+    *   Hex String: The prefix "0x" followed by a hexadecimal number.
+
+    The following formats are available for use through the API:
+
+    *   Bytes: A :class:`bytes`.
+    *   Integer: An :class:`int`.
+
+    Usage
+    -----
+    To get the character for the given address for each of the registered
+    codecs::
+
+        >>> address = '0x61'
+        >>> multidecode(address)                # +ELLIPSIS
+        {'ascii': 'a', 'big5': 'a'... 'utf_8_sig': 'a'}
+
+    If you just want the UTF-8 character::
+
+        >>> value = 'a'
+        >>> codecs_ = ('utf_8',)
+        >>> multidecode(value, codecs_)
+        {'utf_8': 'a',}
+
     """
     # Coerce the given value into bytes.
     value = util.to_bytes(value)
 
     # Decode the value into the character sets.
     results = {}
+    if codecs_ is None:
+        codecs_ = (codec for codec in get_codecs())
     for codec in codecs_:
         b = value
 
         # Pad for 2 or 4 byte codecs.
         while len(b) < codecs[codec].size:
             if codecs[codec].endian == 'little':
                 b = b + b'\x00'
@@ -607,7 +637,64 @@
 
         # Decode.
         try:
             results[codec] = b.decode(codec)
         except UnicodeDecodeError:
             results[codec] = ''
     return results
+
+
+def multiencode(
+    value: bytes | int | str,
+    codecs_: Iterator[str] | None = None
+) -> dict[str, bytes]:
+    """Provide the address for the given character for each of the
+    given character sets.
+
+    :param value: The character to encode.
+    :param codecs_: The codecs to encode to.
+    :return: The encoded value for each character set as a :class:`dict`.
+    :rtype: dict
+
+    Character Formats
+    -----------------
+    The understood :class:`str` formats available for manual input are
+    (all formats are big endian unless otherwise stated):
+
+    *   Character: A string with length equal to one.
+    *   Code Point: The prefix "U+" followed by a hexadecimal number.
+    *   Binary String: The prefix "0b" followed by a binary number.
+    *   Octal String: The prefix "0o" followed by an octal number.
+    *   Decimal String: The prefix "0d" followed by a decimal number.
+    *   Hex String: The prefix "0x" followed by a hexadecimal number.
+
+    The following formats are available for use through the API:
+
+    *   Bytes: A :class:`bytes` that decodes to a valid UTF-8 character.
+    *   Integer: An :class:`int` within the range 0x00 <= x <= 0x10FFFF.
+
+    Usage
+    -----
+    To encode a one character :class:`str` with all registered codecs::
+
+        >>> value = 'a'
+        >>> multiencode(value)                  # +ELLIPSIS
+        {'ascii': b'a', 'big5': b'a'... 'utf_8_sig': b'\xef\xbb\xbfa'}
+
+    If you just want the UTF-8 address::
+
+        >>> value = 'a'
+        >>> codecs_ = ('utf_8',)
+        >>> multiencode(value, codecs_)
+        {'utf_8': b'a',}
+
+    """
+    value = util.to_char(value)
+    if codecs_ is None:
+        codecs_ = (codec for codec in get_codecs())
+    results = {}
+    for codec in codecs_:
+        try:
+            results[codec] = value.encode(codec)
+        except UnicodeEncodeError:
+            results[codec] = b''
+    return results
```

### Comparing `charex-0.1.0/charex/cmds.py` & `charex-0.2.0/charex/cmds.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 cmds
 ~~~~
 
 Core logic for the different commands/modes of :mod:`charex`.
 """
 from collections.abc import Callable, Generator, Sequence
+from functools import partial
 from itertools import zip_longest
 from textwrap import wrap
 
 from charex import charex as ch
 from charex import charsets as cset
 from charex import denormal as dnm
 from charex import escape as esc
@@ -35,15 +36,18 @@
         details = ''
         if len(c) < 1:
             details = '*** no character ***'
         elif len(c) > 1:
             details = '*** multiple characters ***'
         else:
             char = ch.Character(c)
-            details = f'{char.code_point} {char.name}'
+            name = char.na
+            if name == '<control>':
+                name = f'<{char.na1}>'
+            details = f'{char.code_point} {name}'
         c = util.neutralize_control_characters(c)
         yield f'{key:>{width}}: {c} {details}'
 
 
 def ce(base: str) -> Generator[str, None, None]:
     """Encode the given character in all codecs.
 
@@ -68,15 +72,15 @@
 
     :param show_descr: (Optional.) Whether to show the descriptions
         for the character sets.
     :return: Yields each codec as a :class:`str`.
     :rtype: str
     """
     codecs = cset.get_codecs()
-    for line in write_list(codecs, cset.get_codec_description, show_descr):
+    for line in write_list(codecs, cset.get_description, show_descr):
         yield line
 
 
 def ct(base: str, form: str, maxdepth: int, number: int = 0) -> str:
     """Count denormalization results.
 
     :param base: The base normalized string.
@@ -131,57 +135,105 @@
 def dt(c: str) -> Generator[str, None, None]:
     """Display details for a code point.
 
     :param address: The character to encode in the codecs.
     :return: Yields the result for each codec as a :class:`str`.
     :rtype: str
     """
+    width = 35
+
     def rev_normalize(char: ch.Character, form: str) -> str:
         points = char.denormalize(form)
         values = []
         for point in points:
             if len(point) == 1:
                 c = ch.Character(point)
                 values.append(c.summarize())
             elif len(point) > 1:
                 values.append(f'{point} *** multiple characters ***')
                 for item in point:
                     char = ch.Character(item)
                     values.append('  ' + char.summarize())
         if not values:
             return ''
-        return ('\n' + ' ' * 22).join(v for v in values)
+        result = ('\n' + ' ' * 23).join(v for v in values)
+        return '\n' + ' ' * 23 + result + '\n'
+
+    def make_prop_line(
+        prop: str,
+        char: ch.Character
+    ) -> tuple[str, str]:
+        nonlocal width
+        try:
+            name = ch.expand_property(prop)
+            value = getattr(char, prop)
+            if isinstance(value, tuple):
+                value = ' '.join(value)
+            if value and len(name) > width:
+                width = len(name)
+            result = (name, value)
+        except AttributeError:
+            result = ('', '')
+        return result
 
     # Gather the details for display.
     char = ch.Character(c)
-    details = (
-        ('Display', char.value),
-        ('Name', char.name),
-        ('Code Point', char.code_point),
-        ('Category', char.category),
-        ('UTF-8', char.encode('utf8')),
-        ('UTF-16', char.encode('utf_16_be')),
-        ('UTF-32', char.encode('utf_32_be')),
-        ('Decomposition', char.decomposition),
-        ('C encoded', char.escape('c')),
-        ('URL encoded', char.escape('url')),
-        ('HTML encoded', char.escape('html')),
-        ('Reverse Cfold', rev_normalize(char, 'casefold')),
-        ('Reverse NFC', rev_normalize(char, 'nfc')),
-        ('Reverse NFD', rev_normalize(char, 'nfd')),
-        ('Reverse NFKC', rev_normalize(char, 'nfkc')),
-        ('Reverse NFKD', rev_normalize(char, 'nfkd')),
-    )
+    details = {
+        '': (make_prop_line(key, char) for key in ch.UCD.__annotations__ if (
+            key != 'address'
+            and key != 'decimal'
+            and key != 'digit'
+        )),
+        'proplist': (
+            make_prop_line(key, char) for key in char.cache.proplist
+        ),
+        'ranges': (make_prop_line(key, char) for key in char.cache.ranges),
+        'multis': (make_prop_line(key, char) for key in char.cache.multis),
+        'singles': (make_prop_line(key, char) for key in char.cache.singles),
+        'simples': (make_prop_line(key, char) for key in char.cache.simples),
+        'normal simple': (
+            make_prop_line(key, char) for key in char.cache.normalsimplelist
+        ),
+        'normal single': (
+            make_prop_line(key, char) for key in char.cache.normalsingleval
+        ),
+        'emoji': (make_prop_line(key, char) for key in char.cache.emoji),
+        'encoding': (val for val in (
+            ('UTF-8', char.encode('utf8')),
+            ('UTF-16', char.encode('utf_16_be')),
+            ('UTF-32', char.encode('utf_32_be')),
+            ('C encoded', char.escape('c')),
+            ('URL encoded', char.escape('url')),
+            ('HTML encoded', char.escape('html')),
+        )),
+        'denormal': (val for val in (
+            ('Reverse Cfold', rev_normalize(char, 'casefold')),
+            ('Reverse NFC', rev_normalize(char, 'nfc')),
+            ('Reverse NFD', rev_normalize(char, 'nfd')),
+            ('Reverse NFKC', rev_normalize(char, 'nfkc')),
+            ('Reverse NFKD', rev_normalize(char, 'nfkd')),
+        )),
+    }
 
     # Display the details.
-    width = 20
+    yield (' ' * 10 + char.summarize())
+    yield (' ' * 10 + '-' * 60)
     for detail in details:
-        label, value = detail
-        if value:
-            yield f'{label:>{width}}: {value}'
+        if detail:
+            yield f'{"---":>{width}}  {detail.title()}'
+        for line in details[detail]:
+            try:
+                label, value = line
+            except ValueError:
+                raise ValueError(f'{line}')
+            except KeyError:
+                raise KeyError(f'{detail}')
+            if value:
+                yield f'{label:>{width}}: {value}'
+        yield ''
 
 
 def el(show_descr: bool = False) -> Generator[str, None, None]:
     """List registered escape schemes.
 
     :param show_descr: (Optional.) Whether to show the descriptions
         for the character sets.
@@ -239,14 +291,64 @@
             indent = '  '
             if 'mark' in char.category.casefold():
                 indent += ' '
             out += f'  {char.summarize()}\n'
     return out
 
 
+def pf(
+    prop: str,
+    value: str,
+    insensitive: bool = True,
+    regex: bool = False
+) -> Generator[str, None, None]:
+    """List the characters with the given property.
+
+    :param prop: The property for the filter.
+    :param value: The value to filter on.
+    :param regex: (Optional.) Whether the value should be used as a
+        regular expression for the matching. Defaults to false.
+    :return: Yields each property as a :class:`str`.
+    :rtype: str
+    """
+    for char in ch.filter_by_property(
+        prop,
+        value,
+        insensitive=insensitive,
+        regex=regex
+    ):
+        yield char.summarize()
+
+
+def up(show_long: bool = False) -> Generator[str, None, None]:
+    """List the Unicode properties.
+
+    :param show_long: (Optional.) Whether to show the long name.
+    :return: Yields each property as a :class:`str`.
+    :rtype: str
+    """
+    props = ch.get_properties()
+    for line in write_list(props, ch.expand_property, show_long):
+        yield line
+
+
+def uv(prop: str, show_long: bool = False) -> Generator[str, None, None]:
+    """List the valid values for a Unicode property.
+
+    :param prop: The Unicode property.
+    :param show_long: (Optional.) Whether to show the long name.
+    :return: Yields each property as a :class:`str`.
+    :rtype: str
+    """
+    values = ch.get_property_values(prop)
+    expand_value = partial(ch.expand_property_value, prop)
+    for line in write_list(values, expand_value, show_long):
+        yield line
+
+
 # Utility functions.
 def make_description_row(name: str, namewidth: int, descr: str) -> str:
     """Create a two column row with a name and description.
 
     :param name: The content for the first column.
     :param namewidth: The width of the first column.
     :param descr: The content for the second column.
@@ -273,15 +375,23 @@
     :param get_descr: The function used to look up the discription
         of each item.
     :param show_descr: Whether include the descriptions of each item
         in the output.
     :return: Yields each codec as a :class:`str`.
     :rtype: str
     """
+    if not items:
+        items = ('No values.',)
+        show_descr = False
     width = max(len(item) for item in items)
     for item in items:
         if show_descr:
             descr = get_descr(item)
             row = make_description_row(item, width, descr)
             yield row
         else:
             yield item
+
+
+if __name__ == '__main__':
+    for s in pf('emod', 'Y'):
+        print(s)
```

### Comparing `charex-0.1.0/charex/data/PropertyValueAliases.txt` & `charex-0.2.0/charex/data/PropertyValueAliases.txt`

 * *Files identical despite different names*

### Comparing `charex-0.1.0/charex/data/UnicodeData.txt` & `charex-0.2.0/charex/data/UnicodeData.txt`

 * *Files identical despite different names*

### Comparing `charex-0.1.0/charex/data/entities.json` & `charex-0.2.0/charex/data/entities.json`

 * *Files identical despite different names*

### Comparing `charex-0.1.0/charex/data/quote.html` & `charex-0.2.0/charex/data/quote.html`

 * *Files identical despite different names*

### Comparing `charex-0.1.0/charex/data/result.html` & `charex-0.2.0/charex/data/result.html`

 * *Files identical despite different names*

### Comparing `charex-0.1.0/charex/data/rev_casefold.json` & `charex-0.2.0/charex/data/rev_casefold.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -6198,8 +6198,8 @@
 00018350: 5c75 6464 3166 220a 2020 2020 5d2c 0a20  \udd1f".    ],. 
 00018360: 2020 2022 5c75 6438 3361 5c75 6464 3432     "\ud83a\udd42
 00018370: 223a 205b 0a20 2020 2020 2020 2022 5c75  ": [.        "\u
 00018380: 6438 3361 5c75 6464 3230 220a 2020 2020  d83a\udd20".    
 00018390: 5d2c 0a20 2020 2022 5c75 6438 3361 5c75  ],.    "\ud83a\u
 000183a0: 6464 3433 223a 205b 0a20 2020 2020 2020  dd43": [.       
 000183b0: 2022 5c75 6438 3361 5c75 6464 3231 220a   "\ud83a\udd21".
-000183c0: 2020 2020 5d0a 7d0a 0a                       ].}..
+000183c0: 2020 2020 5d0a 7d                            ].}
```

### Comparing `charex-0.1.0/charex/data/rev_nfc.json` & `charex-0.2.0/charex/data/rev_nfc.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -42836,8 +42836,8 @@
 000a7530: 2020 225c 7564 3837 655c 7564 6531 6222    "\ud87e\ude1b"
 000a7540: 0a20 2020 205d 2c0a 2020 2020 225c 7539  .    ],.    "\u9
 000a7550: 6633 6222 3a20 5b0a 2020 2020 2020 2020  f3b": [.        
 000a7560: 225c 7564 3837 655c 7564 6531 6322 0a20  "\ud87e\ude1c". 
 000a7570: 2020 205d 2c0a 2020 2020 225c 7564 3836     ],.    "\ud86
 000a7580: 395c 7564 6530 3022 3a20 5b0a 2020 2020  9\ude00": [.    
 000a7590: 2020 2020 225c 7564 3837 655c 7564 6531      "\ud87e\ude1
-000a75a0: 6422 0a20 2020 205d 0a7d 0a0a            d".    ].}..
+000a75a0: 6422 0a20 2020 205d 0a7d                 d".    ].}
```

### Comparing `charex-0.1.0/charex/data/rev_nfd.json` & `charex-0.2.0/charex/data/rev_nfd.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -42283,8 +42283,7 @@
 000a52a0: 7564 6531 6222 0a20 2020 205d 2c0a 2020  ude1b".    ],.  
 000a52b0: 2020 225c 7539 6633 6222 3a20 5b0a 2020    "\u9f3b": [.  
 000a52c0: 2020 2020 2020 225c 7564 3837 655c 7564        "\ud87e\ud
 000a52d0: 6531 6322 0a20 2020 205d 2c0a 2020 2020  e1c".    ],.    
 000a52e0: 225c 7564 3836 395c 7564 6530 3022 3a20  "\ud869\ude00": 
 000a52f0: 5b0a 2020 2020 2020 2020 225c 7564 3837  [.        "\ud87
 000a5300: 655c 7564 6531 6422 0a20 2020 205d 0a7d  e\ude1d".    ].}
-000a5310: 0a0a                                     ..
```

### Comparing `charex-0.1.0/charex/data/rev_nfkc.json` & `charex-0.2.0/charex/data/rev_nfkc.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -50137,8 +50137,8 @@
 000c3d80: 655c 7564 6531 6122 0a20 2020 205d 2c0a  e\ude1a".    ],.
 000c3d90: 2020 2020 225c 7539 6631 3622 3a20 5b0a      "\u9f16": [.
 000c3da0: 2020 2020 2020 2020 225c 7564 3837 655c          "\ud87e\
 000c3db0: 7564 6531 6222 0a20 2020 205d 2c0a 2020  ude1b".    ],.  
 000c3dc0: 2020 225c 7564 3836 395c 7564 6530 3022    "\ud869\ude00"
 000c3dd0: 3a20 5b0a 2020 2020 2020 2020 225c 7564  : [.        "\ud
 000c3de0: 3837 655c 7564 6531 6422 0a20 2020 205d  87e\ude1d".    ]
-000c3df0: 0a7d 0a0a                                .}..
+000c3df0: 0a7d                                     .}
```

### Comparing `charex-0.1.0/charex/data/rev_nfkd.json` & `charex-0.2.0/charex/data/rev_nfkd.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -49617,8 +49617,8 @@
 000c1d00: 2020 2020 2022 5c75 6438 3765 5c75 6465       "\ud87e\ude
 000c1d10: 3161 220a 2020 2020 5d2c 0a20 2020 2022  1a".    ],.    "
 000c1d20: 5c75 3966 3136 223a 205b 0a20 2020 2020  \u9f16": [.     
 000c1d30: 2020 2022 5c75 6438 3765 5c75 6465 3162     "\ud87e\ude1b
 000c1d40: 220a 2020 2020 5d2c 0a20 2020 2022 5c75  ".    ],.    "\u
 000c1d50: 6438 3639 5c75 6465 3030 223a 205b 0a20  d869\ude00": [. 
 000c1d60: 2020 2020 2020 2022 5c75 6438 3765 5c75         "\ud87e\u
-000c1d70: 6465 3164 220a 2020 2020 5d0a 7d0a 0a    de1d".    ].}..
+000c1d70: 6465 3164 220a 2020 2020 5d0a 7d         de1d".    ].}
```

### Comparing `charex-0.1.0/charex/denormal.py` & `charex-0.2.0/charex/denormal.py`

 * *Files 13% similar despite different names*

```diff
@@ -216,14 +216,46 @@
     :param maxresults: (Optional.) The maximum number of results to
         return. The default is to return one.
     :param seed: (Optional.) A seed value for the random number generator.
         Defaults to not seeding the generator.
     :return: A :class:`collections.abc.Generator` that yields the random
         denormalization results.
     :rtype: collections.abc.Generator
+
+    Usage
+    -----
+    To generate a random denormalization of a given string with a given
+    form::
+
+        >>> # The seed parameter seeds the RNG to produce repeatable
+        >>> # results for testing. Don't use it unless you want
+        >>> # repeatable results.
+        >>> seed_ = 'spam'
+        >>>
+        >>> base = '<script>'
+        >>> form = 'nfkc'
+        >>> dngrd = gen_random_denormalize(base, form, seed_=seed_)
+        >>> [result for result in dngrd]
+        ['﹤𝓈ᶜ𝕣𝚒𝙥𝙩＞']
+
+    The `maxresults` parameter tells the generator to return the
+    given number of results::
+
+        >>> # The seed parameter seeds the RNG to produce repeatable
+        >>> # results for testing. Don't use it unless you want
+        >>> # repeatable results.
+        >>> seed_ = 'spam'
+        >>>
+        >>> base = '<script>'
+        >>> form = 'nfkc'
+        >>> maxresults = 3
+        >>> dngrd = gen_random_denormalize(base, form, maxresults, seed_=seed_)
+        >>> [result for result in dngrd]
+        ['﹤𝓈ᶜ𝕣𝚒𝙥𝙩＞', '＜𝖘ᶜ𝓇𝕚ᵖ𝓉＞', '﹤𝙨𝚌𝑟𝗂𝐩ｔ＞']
+
     """
     chars = [denormalize(char, form) for char in base]
     if seed_:
         seed(seed_)
     for _ in range(maxresults):
         result = ''.join(choice(char) for char in chars)
         yield result
@@ -246,14 +278,44 @@
         return. Default behavior varies based on the `random` parameter.
         If `random` is `False`, default is to return all possible
         denormalizattions. Otherwise, the default is to return one.
     :param seed: (Optional.) A seed value for the random number generator.
         Defaults to not seeding the generator.
     :return: The denormalizations as a :class:`tuple`.
     :rtype: tuple
+
+    Usage
+    -----
+    To get a random denormalization of the given string using the given
+    form::
+
+        >>> # The seed parameter seeds the RNG to produce repeatable
+        >>> # results for testing. Don't use it unless you want
+        >>> # repeatable results.
+        >>> seed_ = 'spam'
+        >>>
+        >>> base = '<script>'
+        >>> form = 'nfkc'
+        >>> random_denormalize(base, form,  seed_=seed_)
+        ('﹤𝓈ᶜ𝕣𝚒𝙥𝙩＞',)
+
+    The `maxresults` parameter tells the function to return the
+    given number of results::
+
+        >>> # The seed parameter seeds the RNG to produce repeatable
+        >>> # results for testing. Don't use it unless you want
+        >>> # repeatable results.
+        >>> seed_ = 'spam'
+        >>>
+        >>> base = '<script>'
+        >>> form = 'nfkc'
+        >>> maxresults = 3
+        >>> random_denormalize(base, form,  maxresults, seed_=seed_)
+        ('﹤𝓈ᶜ𝕣𝚒𝙥𝙩＞', '＜𝖘ᶜ𝓇𝕚ᵖ𝓉＞', '﹤𝙨𝚌𝑟𝗂𝐩ｔ＞')
+
     """
     # Ensure at least one result is returned.
     if not maxresults:
         maxresults = 1
 
     # Seeding the RNG allows for repeatability in testing.
     if seed_:
```

### Comparing `charex-0.1.0/charex/escape.py` & `charex-0.2.0/charex/escape.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,30 @@
 
 
 # Registration.
 class reg_escape:
     """A decorator for registering escape schemes.
 
     :param key: The name the escape sequence is registered under.
+
+    Usage
+    -----
+    To register a new escape scheme::
+
+        >>> @reg_escape('double')
+        ... def double(char: str, codec: str) -> str:
+        ...     '''Double the character.'''
+        ...     return char + char
+        ...
+        >>> # Demonstrate the registration worked.
+        >>> 'double' in get_schemes()
+        True
+        >>> escape_text('spam', 'double')
+        'ssppaamm'
+
     """
     def __init__(self, key: str) -> None:
         self.key = key
 
     def __call__(
         self,
         fn: Callable[[str, str], str]
@@ -474,14 +490,33 @@
     :param codec: The character set to use when encoding the character.
     :return: The escaped character as a :class:`str`.
     :rtype: str
     """
     return unicode_utf16_escape(char)
 
 
+@reg_escape('smol')
+def escape_smol(char: str, codec: str) -> str:
+    """Escape scheme for smol characters, based loosely on the
+    Unicode superscript characters.
+
+    :param char: The character to escape.
+    :param codec: The character set to use when encoding the character.
+    :return: The escaped character as a :class:`str`.
+    :rtype: str
+    """
+    norms = 'abcdefghijklmnopqrstuvwxyz'
+    smol = 'ᵃᵇᶜᵈᵉᶠᵍʰᶦʲᵏˡᵐⁿᵒᵖᑫʳˢᵗᵘᵛʷˣʸᶻ'
+    table = {k: v for k, v in zip(norms, smol)}
+    try:
+        return lookup_escape(char, table)
+    except EscapeError:
+        return char
+
+
 @reg_escape('sql')
 def escape_sql(char: str, codec: str) -> str:
     """Escape scheme for MySQL encoding, based on the MySQL
     Specification.
 
     The specification can be found `here.`_
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `charex-0.1.0/charex/gui.py` & `charex-0.2.0/charex/gui.py`

 * *Files 14% similar despite different names*

```diff
@@ -36,15 +36,19 @@
 
         # Create the tab navigation and tabs.
         book = ttk.Notebook(root, padding='1 1 1 1')
         self.book = book
         book.grid(column=0, row=0, sticky=ALL)
         self.tabs = {}
         self.wake_focus = {}
-        names = ('cd', 'ce', 'cl', 'ct', 'dn', 'dt', 'el', 'es', 'fl', 'nl')
+        names = [
+            name.split('_')[-1]
+            for name in dir(self)
+            if name.startswith('init_')
+        ]
         for i, name in enumerate(names):
             frame = ttk.Frame(book, padding='3 3 12 12')
             book.add(frame, text=name)
             init = getattr(self, f'init_{name}')
             num = i + 1
             if num == 1:
                 num = ''
@@ -251,15 +255,15 @@
         self.pad_kids(frame)
         self.wake_focus[f'!frame{num}'] = char_entry
 
     def init_fl(self, frame, num=None):
         self.fl_result = self.make_results(frame)
 
         self.config_simple_grid(frame)
-        el_button = self.make_button(
+        fl_button = self.make_button(
             frame,
             'List Normalization Forms',
             self.fl
         )
         self.pad_kids(frame)
 
     def init_nl(self, frame, num=None):
@@ -288,14 +292,96 @@
             self.nl,
             row=4,
             colspan=5
         )
         self.pad_kids(frame)
         self.wake_focus[f'!frame{num}'] = char_entry
 
+    def init_pf(self, frame, num=None):
+        self.pf_prop = tk.StringVar()
+        self.pf_value = tk.StringVar()
+        self.pf_insensitive = tk.BooleanVar(value=False)
+        self.pf_regex = tk.BooleanVar(value=False)
+        self.pf_result = self.make_results(frame, row=5, colspan=4)
+
+        self.config_five_params_grid(frame)
+
+        form_label = ttk.Label(frame, text='Property:', justify=tk.RIGHT)
+        form_label.grid(column=0, row=0, columnspan=1, sticky=SIDES)
+        self.pfprop_combo = ttk.Combobox(frame, textvariable=self.pf_prop)
+        self.pfprop_combo['values'] = ch.get_properties()
+        self.pfprop_combo.state(['readonly'])
+        self.pfprop_combo.bind('<<ComboboxSelected>>', self.handle_pf_pfprop)
+        self.pfprop_combo.grid(column=1, row=0, columnspan=4, sticky=SIDES)
+
+        val_label = ttk.Label(frame, text='Value:', justify=tk.RIGHT)
+        val_label.grid(column=0, row=1, columnspan=1, sticky=SIDES)
+        self.pfval_combo = ttk.Combobox(frame, textvariable=self.pf_value)
+        self.pfval_combo.grid(column=1, row=1, columnspan=4, sticky=SIDES)
+
+        insensitive_label = ttk.Label(
+            frame, text='Ignore Case:', justify=tk.RIGHT
+        )
+        insensitive_label.grid(column=0, row=3, columnspan=1, sticky=SIDES)
+        insensitive_check = ttk.Checkbutton(
+            frame,
+            variable=self.pf_insensitive,
+            onvalue='True',
+            offvalue='False'
+        )
+        insensitive_check.grid(column=1, row=3, columnspan=1, sticky=SIDES)
+
+        regex_label = ttk.Label(frame, text='Regex:', justify=tk.RIGHT)
+        regex_label.grid(column=2, row=3, columnspan=1, sticky=SIDES)
+        regex_check = ttk.Checkbutton(
+            frame,
+            variable=self.pf_regex,
+            onvalue='True',
+            offvalue='False'
+        )
+        regex_check.grid(column=3, row=3, columnspan=1, sticky=SIDES)
+
+        pf_button = self.make_button(
+            frame,
+            'Filter by the Property Value',
+            self.pf,
+            row=4,
+            colspan=5
+        )
+        self.pad_kids(frame)
+
+    def init_up(self, frame, num=None):
+        self.up_result = self.make_results(frame)
+
+        self.config_simple_grid(frame)
+        up_button = self.make_button(
+            frame,
+            'List Unicode Properties',
+            self.up
+        )
+        self.pad_kids(frame)
+
+    def init_uv(self, frame, num=None):
+        self.uv_prop = tk.StringVar()
+        self.uv_result = self.make_results(frame)
+
+        self.config_simple_grid(frame)
+
+        form_combo = ttk.Combobox(frame, textvariable=self.uv_prop)
+        form_combo['values'] = ch.get_properties()
+        form_combo.state(['readonly'])
+        form_combo.grid(column=0, row=0, columnspan=2, sticky=SIDES)
+
+        uv_button = self.make_button(
+            frame,
+            'List Values of Unicode Property',
+            self.uv
+        )
+        self.pad_kids(frame)
+
     # Core commands.
     def cd(self, *args):
         try:
             self.cd_result.delete('0.0', 'end')
             address = self.cd_address.get()
             for line in cmds.cd(address):
                 self.cd_result.insert('end', line + '\n')
@@ -378,14 +464,36 @@
         self.nl_result.delete('0.0', 'end')
         base = self.nl_base.get()
         form = self.nl_form.get()
 
         result = cmds.nl(form, base, True)
         self.nl_result.insert('end', result)
 
+    def pf(self, *args):
+        self.pf_result.delete('0.0', 'end')
+        prop = self.pf_prop.get()
+        value = self.pf_value.get()
+        insensitive = self.pf_insensitive.get()
+        regex = self.pf_regex.get()
+
+        for line in cmds.pf(prop, value, insensitive, regex):
+            self.pf_result.insert('end', line + '\n')
+
+    def up(self, *args):
+        self.up_result.delete('0.0', 'end')
+        for line in cmds.up(True):
+            self.up_result.insert('end', line + '\n\n')
+
+    def uv(self, *args):
+        prop = self.uv_prop.get()
+
+        self.uv_result.delete('0.0', 'end')
+        for line in cmds.uv(prop, True):
+            self.uv_result.insert('end', line + '\n\n')
+
     # Event handlers.
     def handle_notebook_tab_changed(self, event):
         focus = self.root.focus_get()
         name = str(focus)
         frame = name.split('.')[-2]
         if frame in self.wake_focus:
             entry = self.wake_focus[frame]
@@ -393,14 +501,18 @@
 
     def handle_return(self, *args):
         tab_id = self.book.select()
         tab = self.book.index(tab_id)
         cmd = self.tabs[tab]
         cmd()
 
+    def handle_pf_pfprop(self, event):
+        prop = self.pf_prop.get()
+        self.pfval_combo['values'] = ch.get_property_values(prop)
+
     # Grid configuration.
     def config_simple_grid(self, frame):
         frame.columnconfigure(0, weight=1)
         frame.columnconfigure(1, weight=0)
         frame.rowconfigure(1, weight=0)
         frame.rowconfigure(2, weight=0)
         frame.rowconfigure(3, weight=1)
```

### Comparing `charex-0.1.0/charex/http.py` & `charex-0.2.0/charex/http.py`

 * *Files identical despite different names*

### Comparing `charex-0.1.0/charex/normal.py` & `charex-0.2.0/charex/normal.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,53 +8,67 @@
 from itertools import permutations
 from json import dumps
 import unicodedata as ucd
 
 from charex import util
 
 
-# Constants.
-LEN_UNICODE = 0x10FFFF
-
-
 # Registry.
 forms = {}
 
 
 # Registration.
 class reg_form:
     """A decorator for registering normalization forms.
 
     :param key: The name the normalization form is registered under.
+
+    Usage
+    -----
+    To register a normalization form::
+
+        >>> from charex import *
+        >>>
+        >>> @reg_form('a')
+        ... def form_a(base: str) -> str:
+        ...     '''Make all strings into the letter A.'''
+        ...     return 'A'
+        ...
+        >>> # Demonstrate the registration worked.
+        >>> 'a' in get_forms()
+        True
+        >>> normalize('a', 'spam')
+        'A'
     """
     def __init__(self, key: str) -> None:
         self.key = key
 
     def __call__(
         self,
         fn: Callable[[str], str]
     ) -> Callable[[str], str]:
         forms[self.key] = fn
         return fn
 
 
 # Utility functions.
-def build_denormalization_map(norm_fn: Callable[[str], str]) -> str:
+def build_denormalization_map(formkey: str) -> str:
     """Create a JSON string mapping each Unicode character to the
     other Unicode characters that normalize to it.
 
-    :param norm_fn: The normalization function.
+    :param formkey: The key for the normalization function.
     :return: The denormalization map as a JSON :class:`str`.
     :rtype: str
     """
     # The denormalization map.
     dn_map: dict[str, set[str]] = {}
 
     # Process every Unicode character.
-    for n in range(LEN_UNICODE):
+    norm_fn = forms[formkey]
+    for n in range(util.LEN_UNICODE):
         base = chr(n)
 
         # If the character normalizes to a different character,
         # add that relationship to the map.
         normal = norm_fn(base)
         if normal and normal != base:
             dn_map.setdefault(normal, set())
@@ -91,15 +105,15 @@
 
     :return: The character and the number of characters in the
         decomposition as a :class:`tuple`.
     :rtype: tuple
     """
     long_char = ''
     decomp_max = 0
-    for n in range(LEN_UNICODE):
+    for n in range(util.LEN_UNICODE):
         char = chr(n)
         decomp_char = form_nfd(char)
         decomp_len = len(decomp_char)
         if decomp_len > decomp_max:
             long_char = char
             decomp_max = decomp_len
     return long_char, decomp_max
@@ -117,26 +131,44 @@
 
 
 def get_forms() -> tuple[str, ...]:
     """Return the keys of the registered normalization forms.
 
     :return: The names of the normalization forms as a :class:`tuple`.
     :rtype: tuple
+
+    Usage
+    -----
+    To get a tuple of the registered normalization forms::
+
+        >>> get_forms()
+        ('casefold', 'nfc', 'nfd', 'nfkc', 'nfkd')
+
     """
     return tuple(form for form in forms)
 
 
 # Normalization function.
 def normalize(formkey: str, base: str) -> str:
     """Normalize the base string with the form.
 
     :param formkey: The key of a registered normalization form.
     :param base: The string to normalize.
     :return: The normalized :class:`str`.
     :rtype: str
+
+    Usage
+    -----
+    To normalize a string using the given form::
+
+        >>> value = 'SPAM'
+        >>> form = 'casefold'
+        >>> normalize(form, value)
+        'spam'
+
     """
     form = forms[formkey]
     return form(base)
 
 
 # Normalization forms.
 @reg_form('casefold')
```

### Comparing `charex-0.1.0/charex/shell.py` & `charex-0.2.0/charex/shell.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,14 +18,33 @@
 from textwrap import wrap
 
 from charex import cmds
 from charex import charsets as cset
 from charex import escape as esc
 from charex import gui
 from charex import normal as nl
+from charex import util
+
+
+# Registry.
+subparsers: list[Callable[[_SubParsersAction], None]] = []
+
+
+# Registration.
+def subparser(
+    fn: Callable[[_SubParsersAction], None]
+) -> Callable[[_SubParsersAction], None]:
+    """A decorator for registering subparsers.
+
+    :param fn: The function being registered.
+    :return: The registered :class:`collections.abc.Callable`.
+    :rtype: collections.abc.Callable
+    """
+    subparsers.append(fn)
+    return fn
 
 
 # Running modes.
 def mode_cd(args: Namespace) -> None:
     """Decode the given address in all codecs.
 
     :param args: The arguments used when the script was invoked.
@@ -89,16 +108,15 @@
 def mode_dm(args: Namespace) -> None:
     """Build a denormalization map.
 
     :param args: The arguments used when the script was invoked.
     :return: None.
     :rtype: NoneType
     """
-    normal_fn = nl.forms[args.form]
-    results = nl.build_denormalization_map(normal_fn)
+    results = nl.build_denormalization_map(args.form)
     print(results)
     print()
 
 
 def mode_dn(args: Namespace) -> None:
     """Perform denormalizations.
 
@@ -121,15 +139,16 @@
     """Display details for a code point.
 
     :param args: The arguments used when the script was invoked.
     :return: None.
     :rtype: NoneType
     """
     for line in cmds.dt(args.codepoint):
-        print(line)
+        bline = line.encode('utf_8', errors='replace')
+        print(bline.decode('utf_8'))
     print()
 
 
 def mode_el(args: Namespace) -> None:
     """List the registered escape schemes.
 
     :param args: The arguments used when the script was invoked.
@@ -189,24 +208,70 @@
     :rtype: NoneType
     """
     result = cmds.nl(args.form, args.base, args.expand)
     print(result)
     print()
 
 
+def mode_pf(args: Namespace) -> None:
+    """List characters with a given property value.
+
+    :param args: The arguments used when the script was invoked.
+    :return: None.
+    :rtype: NoneType
+    """
+    for line in cmds.pf(
+        args.prop,
+        args.value,
+        insensitive=args.insensitive,
+        regex=args.regex
+    ):
+        bline = line.encode('utf_8', errors='replace')
+        print(bline.decode('utf_8'))
+    print()
+
+
 def mode_sh(args: Namespace | None) -> None:
     """Run in an interactive shell.
 
     :param args: The arguments used when the script was invoked.
     :return: None.
     :rtype: NoneType
     """
     Shell(completekey='tab').cmdloop()
 
 
+def mode_up(args: Namespace) -> None:
+    """List the Unicode properties.
+
+    :param args: The arguments used when the script was invoked.
+    :return: None.
+    :rtype: NoneType
+    """
+    for line in cmds.up(args.description):
+        print(line)
+        if args.description:
+            print()
+    print()
+
+
+def mode_uv(args: Namespace) -> None:
+    """List the valid values for a Unicode property.
+
+    :param args: The arguments used when the script was invoked.
+    :return: None.
+    :rtype: NoneType
+    """
+    for line in cmds.uv(args.prop, args.description):
+        print(line)
+        if args.description:
+            print()
+    print()
+
+
 # Command parsing.
 def build_parser() -> ArgumentParser:
     """Build the argument parser.
 
     :return: The :class:`argparse.ArgumentParser`.
     :rtype: argparse.ArgumentParser
     """
@@ -220,78 +285,71 @@
 
     # Build subparsers for each mode.
     spa = p.add_subparsers(
         help=list_modes(),
         metavar='mode',
         required=True
     )
-    parse_cd(spa)
-    parse_ce(spa)
-    parse_cl(spa)
-    parse_clear(spa)
-    parse_ct(spa)
-    parse_dm(spa)
-    parse_dn(spa)
-    parse_dt(spa)
-    parse_el(spa)
-    parse_es(spa)
-    parse_fl(spa)
-    parse_gui(spa)
-    parse_nl(spa)
-    parse_sh(spa)
+    for fn in subparsers:
+        fn(spa)
 
     return p
 
 
+@subparser
 def parse_cd(spa: _SubParsersAction) -> None:
     """Add the cd mode subparser.
 
     :param spa: The subparser action used to add a new subparser to
         the main parser.
     :return: None.
     :rtype: NoneType
     """
     sp = spa.add_parser(
         'cd',
-        description='Decode the given address in all codecs.'
+        description='Decode the given address in all codecs.',
+        epilog=util.ADDRESS_FORMAT_DOC,
+        formatter_class=RawDescriptionHelpFormatter
     )
     sp.add_argument(
         'base',
         help=(
-            'The base integer. Prefix the integer with "0x" for hex '
-            'or "0b" for binary. No prefix or a Unicode code point '
-            'will be interpreted as the UTF-8 address of the character.'
+            'The base address. See below for details.'
         ),
         action='store',
         type=str
     )
     sp.set_defaults(func=mode_cd)
 
 
+@subparser
 def parse_ce(spa: _SubParsersAction) -> None:
     """Add the ce mode subparser.
 
     :param spa: The subparser action used to add a new subparser to
         the main parser.
     :return: None.
     :rtype: NoneType
     """
     sp = spa.add_parser(
         'ce',
-        description='Encode the given character in all codecs.'
+        description='Encode the given character in all codecs.',
+        epilog=util.CHAR_FORMAT_DOC,
+        formatter_class=RawDescriptionHelpFormatter
     )
     sp.add_argument(
         'base',
         help='The character to lookup in each character set.',
         action='store',
         type=str
     )
     sp.set_defaults(func=mode_ce)
 
 
+@subparser
 def parse_cl(spa: _SubParsersAction) -> None:
     """Add the charsetlist mode subparser.
 
     :param spa: The subparser action used to add a new subparser to
         the main parser.
     :return: None.
     :rtype: NoneType
@@ -305,14 +363,15 @@
         '-d', '--description',
         help='Show the description for the character sets.',
         action='store_true'
     )
     sp.set_defaults(func=mode_cl)
 
 
+@subparser
 def parse_clear(spa: _SubParsersAction) -> None:
     """Clear the terminal.
 
     :param spa: The subparser action used to add a new subparser to
         the main parser.
     :return: None.
     :rtype: NoneType
@@ -321,14 +380,15 @@
         'clear',
         aliases=['clr',],
         description='Clear the terminal.'
     )
     sp.set_defaults(func=mode_clear)
 
 
+@subparser
 def parse_ct(spa: _SubParsersAction) -> None:
     """Add the ct mode subparser.
 
     :param spa: The subparser action used to add a new subparser to
         the main parser.
     :return: None.
     :rtype: NoneType
@@ -358,14 +418,15 @@
         default=0,
         action='store',
         type=int
     )
     sp.set_defaults(func=mode_ct)
 
 
+@subparser
 def parse_dm(spa: _SubParsersAction) -> None:
     """Add the dm mode subparser.
 
     :param spa: The subparser action used to add a new subparser to
         the main parser.
     :return: None.
     :rtype: NoneType
@@ -385,14 +446,15 @@
             f'options are: {valid_forms}.'
         ),
         metavar='form'
     )
     sp.set_defaults(func=mode_dm)
 
 
+@subparser
 def parse_dn(spa: _SubParsersAction) -> None:
     """Add the dn mode subparser.
 
     :param spa: The subparser action used to add a new subparser to
         the main parser.
     :return: None.
     :rtype: NoneType
@@ -440,36 +502,40 @@
         help='Seed the randomized denormalization.',
         action='store',
         default=''
     )
     sp.set_defaults(func=mode_dn)
 
 
+@subparser
 def parse_dt(spa: _SubParsersAction) -> None:
     """Add the dt mode subparser.
 
     :param spa: The subparser action used to add a new subparser to
         the main parser.
     :return: None.
     :rtype: NoneType
     """
     sp = spa.add_parser(
         'dt',
         aliases=['details',],
-        description='Display the details for the given code point.'
+        description='Display the details for the given character.',
+        epilog=util.CHAR_FORMAT_DOC,
+        formatter_class=RawDescriptionHelpFormatter
     )
     sp.add_argument(
         'codepoint',
-        help='The code point.',
+        help='The character.',
         action='store',
         type=str
     )
     sp.set_defaults(func=mode_dt)
 
 
+@subparser
 def parse_el(spa: _SubParsersAction) -> None:
     """Add the el mode subparser.
 
     :param spa: The subparser action used to add a new subparser to
         the main parser.
     :return: None.
     :rtype: NoneType
@@ -483,14 +549,15 @@
         '-d', '--description',
         help='Show the description for the character sets.',
         action='store_true'
     )
     sp.set_defaults(func=mode_el)
 
 
+@subparser
 def parse_es(spa: _SubParsersAction) -> None:
     """Add the escape mode subparser.
 
     :param spa: The subparser action used to add a new subparser to
         the main parser.
     :return: None.
     :rtype: NoneType
@@ -518,14 +585,15 @@
         help='The string to escape.',
         action='store',
         type=str
     )
     sp.set_defaults(func=mode_es)
 
 
+@subparser
 def parse_fl(spa: _SubParsersAction) -> None:
     """Add the fl mode subparser.
 
     :param spa: The subparser action used to add a new subparser to
         the main parser.
     :return: None.
     :rtype: NoneType
@@ -539,14 +607,15 @@
         '-d', '--description',
         help='Show the description for the character sets.',
         action='store_true'
     )
     sp.set_defaults(func=mode_fl)
 
 
+@subparser
 def parse_gui(spa: _SubParsersAction) -> None:
     """Run the GUI.
 
     :param spa: The subparser action used to add a new subparser to
         the main parser.
     :return: None.
     :rtype: NoneType
@@ -555,14 +624,15 @@
         'gui',
         aliases=[],
         description='Run the charex GUI.'
     )
     sp.set_defaults(func=mode_gui)
 
 
+@subparser
 def parse_nl(spa: _SubParsersAction) -> None:
     """Add the nl mode subparser.
 
     :param spa: The subparser action used to add a new subparser to
         the main parser.
     :return: None.
     :rtype: NoneType
@@ -593,14 +663,52 @@
         '-e', '--expand',
         help='Show each character in the normalized string.',
         action='store_true'
     )
     sp.set_defaults(func=mode_nl)
 
 
+@subparser
+def parse_pf(spa: _SubParsersAction) -> None:
+    """Add the pf mode subparser.
+
+    :param spa: The subparser action used to add a new subparser to
+        the main parser.
+    :return: None.
+    :rtype: NoneType
+    """
+    sp = spa.add_parser(
+        'pf',
+        aliases=['propfilter', 'pfilt',],
+        description='List characters with a given property value.'
+    )
+    sp.add_argument(
+        'prop',
+        help='The property for the filter.',
+        action='store'
+    )
+    sp.add_argument(
+        'value',
+        help='The value to filter with.',
+        action='store'
+    )
+    sp.add_argument(
+        '--insensitive', '-i',
+        help='The matching is case insensitive.',
+        action='store_true',
+    )
+    sp.add_argument(
+        '--regex', '-g',
+        help='The value is used as a regular expression when matching.',
+        action='store_true',
+    )
+    sp.set_defaults(func=mode_pf)
+
+
+@subparser
 def parse_sh(spa: _SubParsersAction) -> None:
     """Add the shell mode subparser.
 
     :param spa: The subparser action used to add a new subparser to
         the main parser.
     :return: None.
     :rtype: NoneType
@@ -609,14 +717,64 @@
         'sh',
         aliases=['shell',],
         description='Run charex in an interactive shell.'
     )
     sp.set_defaults(func=mode_sh)
 
 
+@subparser
+def parse_up(spa: _SubParsersAction) -> None:
+    """Add the up mode subparser.
+
+    :param spa: The subparser action used to add a new subparser to
+        the main parser.
+    :return: None.
+    :rtype: NoneType
+    """
+    sp = spa.add_parser(
+        'up',
+        aliases=['proplist', 'plist',],
+        description='List the Unicode properties.'
+    )
+    sp.add_argument(
+        '-d', '--description',
+        help='Show the long name of the properties.',
+        action='store_true'
+    )
+    sp.set_defaults(func=mode_up)
+
+
+@subparser
+def parse_uv(spa: _SubParsersAction) -> None:
+    """Add the uv mode subparser.
+
+    :param spa: The subparser action used to add a new subparser to
+        the main parser.
+    :return: None.
+    :rtype: NoneType
+    """
+    sp = spa.add_parser(
+        'uv',
+        aliases=['propvallist', 'pvlist', 'upv',],
+        description='List the valid values of a Unicode property.'
+    )
+    sp.add_argument(
+        'prop',
+        help='The Unicode property.',
+        action='store'
+    )
+    sp.add_argument(
+        '-d', '--description',
+        help='Show the long name of the properties.',
+        action='store_true'
+    )
+    sp.set_defaults(func=mode_uv)
+
+
+# Command line invocation.
 def invoke(
     cmd: str | None = None,
     p: ArgumentParser | None = None
 ) -> None:
     """Parse the arguments used to invoke the script and execute
     the script.
     """
@@ -728,14 +886,29 @@
             super().do_help(arg)
 
     def do_nl(self, arg):
         """Normalize the given string."""
         cmd = f'nl {arg}'
         self._run_cmd(cmd)
 
+    def do_pf(self, arg):
+        """List characters with a given property value."""
+        cmd = f'pf {arg}'
+        self._run_cmd(cmd)
+
+    def do_up(self, arg):
+        """List the Unicode properties."""
+        cmd = f'up {arg}'
+        self._run_cmd(cmd)
+
+    def do_uv(self, arg):
+        """List the valid values of a Unicode property."""
+        cmd = f'uv {arg}'
+        self._run_cmd(cmd)
+
     def do_xt(self, arg):
         """Exit the charex shell."""
         print('Exiting charex.')
         print()
         return True
 
     # Command help.
@@ -792,14 +965,29 @@
         self._run_cmd(cmd)
 
     def help_nl(self):
         """Help for the nl command."""
         cmd = f'nl -h'
         self._run_cmd(cmd)
 
+    def help_pf(self):
+        """Help for the pf command."""
+        cmd = f'pf -h'
+        self._run_cmd(cmd)
+
+    def help_up(self):
+        """Help for the up command."""
+        cmd = f'up -h'
+        self._run_cmd(cmd)
+
+    def help_uv(self):
+        """Help for the uv command."""
+        cmd = f'uv -h'
+        self._run_cmd(cmd)
+
     def help_xt(self):
         lines = util.read_resource('help_xt')
         print(''.join(lines))
 
     # Private methods.
     def _run_cmd(self, cmd):
         """Run the given command."""
```

### Comparing `charex-0.1.0/pyproject.toml` & `charex-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 [tool.pytest.ini_options]
 addopts = [
     "--import-mode=importlib",
 ]
 
 [project]
 name = "charex"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
     {name="Paul J. Iutzi", email="pji@mac.com"},
 ]
 description = "A unicode and character set explorer."
 readme = "README.rst"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `charex-0.1.0/tests/test_charset.py` & `charex-0.2.0/tests/test_charset.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 def test_get_codecs():
     """WHen called, return a tuple of registered codecs."""
     exp = tuple(codec for codec in cs.codecs.keys())
     assert cs.get_codecs() == exp
 
 
 # Test get_codec_description.
-def test_get_codec_description():
+def test_get_description():
     """Given the name of a character set codec, return the description
     of that codec.
     """
     codec = 'ascii'
     info = cs.codecs[codec]
     exp = info.description
-    assert cs.get_codec_description(codec) == exp
+    assert cs.get_description(codec) == exp
 
 
 # Tests for multidecode.
 def test_multidecode_bytes():
     """Given bytes and a sequence of strings that reference
     decoding codecs, :func:`charex.charsets.multiencode` returns
     the code point for each given codec as a :class:`dict`.
@@ -76,14 +76,34 @@
         'utf_16': 'é',
     }
     codecs = exp.keys()
     act = cs.multidecode('0xe9', codecs)
     assert exp == act
 
 
+def test_multidecode_str_and_no_codecs(mocker):
+    """Given a hex string, :func:`charex.charsets.multiencode` returns
+    the code point for each given codec as a :class:`dict`.
+    """
+    exp = {
+        'ascii': '',
+        'cp1252': 'é',
+        'iso8859_7': 'ι',
+        'utf_16_be': 'é',
+        'utf_16_le': 'é',
+        'utf_16': 'é',
+    }
+    mocker.patch(
+        'charex.charsets.get_codecs',
+        return_value=tuple(codec for codec in exp)
+    )
+    act = cs.multidecode('0xe9')
+    assert exp == act
+
+
 # Tests for multiencode.
 def test_multiencode():
     """Given a code point and a list of character sets, return the
     :class:`bytes` for that code point in each character set as a
     :class:`dict`.
     """
     exp = {
@@ -93,14 +113,48 @@
         'utf_8': b'\xe2\x80\x9c',
     }
     codecs = exp.keys()
     act = cs.multiencode('“', codecs)
     assert exp == act
 
 
+def test_multiencode_codecs_none(mocker):
+    """Given a code point, return the :class:`bytes` for that code point
+    in each character set as a :class:`dict`.
+    """
+    exp = {
+        'ascii': b'',
+        'cp1252': b'\x93',
+        'mac_roman': b'\xd2',
+        'utf_8': b'\xe2\x80\x9c',
+    }
+    mocker.patch(
+        'charex.charsets.get_codecs',
+        return_value=tuple(codec for codec in exp)
+    )
+    act = cs.multiencode('“')
+    assert exp == act
+
+
+def test_multiencode_codecs_tuple():
+    """Given a code point and a :class:`tuple` of character sets, return
+    the :class:`bytes` for that code point in each character set as a
+    :class:`dict`.
+    """
+    exp = {
+        'ascii': b'',
+        'cp1252': b'\x93',
+        'mac_roman': b'\xd2',
+        'utf_8': b'\xe2\x80\x9c',
+    }
+    codecs = tuple(codec for codec in exp)
+    act = cs.multiencode('“', codecs)
+    assert exp == act
+
+
 def test_multiencode_unicode():
     """Given a code point and a list of character sets, return the
     :class:`bytes` for that code point in each character set as a
     :class:`dict`.
     """
     exp = {
         'ascii': b'',
```

### Comparing `charex-0.1.0/tests/test_denormal.py` & `charex-0.2.0/tests/test_denormal.py`

 * *Files identical despite different names*

### Comparing `charex-0.1.0/tests/test_escape.py` & `charex-0.2.0/tests/test_escape.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,14 +230,24 @@
     be returned as two characters because Java encodes strings with
     UTF-16.
     """
     exp = r'\ud800\udc00'
     assert esc.escape_jsonu('\U00010000', '') == exp
 
 
+# Test escape_smol.
+def test_escape_smol():
+    """Give a character and a codec, return the superscript
+    Unicode character version of the given character. Note: the
+    codec doesn't do anything. It's just here for compatibility.
+    """
+    exp = 'ᵃ'
+    assert esc.escape_smol('a', '') == exp
+
+
 # Test escape_sql.
 def test_escape_sql():
     """Given a character and a codec, return the SQL escape
     sequence for the character. Note: the codec doesn't do anything,
     it's just here for compatibility.
     """
     exp = r'\n'
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `charex-0.1.0/tests/test_main.py` & `charex-0.2.0/tests/test_shell.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,172 +1,100 @@
 """
-test_main
-~~~~~~~~~
+test_shell
+~~~~~~~~~~
 
-Unit tests for the mainline of the `charex` package.
+Unit tests for :mod:`charex.shell`.
 """
-import sys
-
-from charex import __main__ as m
 from charex import escape as esc
 from charex import normal as nl
+from charex import shell as sh
 
 
-# Test cd mode.
+# Tests for cd.
 def test_cd(capsys):
-    """Called with an hex string, charset mode should return the character
-    or characters that hex string becomes in each of the known character
-    sets.
+    """Invoked with a hex string, `cd` returns the character for
+    that address in each registered character set. A hex string is
+    declared by starting the string with "0x".
     """
     with open('tests/data/charset_mode_41.txt') as fh:
         exp = fh.read()
-    cmd = (
-        'python -m charex',
-        'cd',
-        '0x41'
-    )
-    cli_test(exp, cmd, capsys)
+    cmd = 'cd 0x41'
+    shell_test(exp, cmd, capsys)
 
 
 def test_cd_binary(capsys):
-    """Called with a number prefixed with "0b", cd mode should interpret
-    the base string as binary and return the character or characters that
-    binary string becomes in each of the known character sets.
+    """Invoked with a binary string, `cd` returns the character for
+    that address in each registered character set. A binary string is
+    declared by starting the string with "0b".
     """
     with open('tests/data/charset_mode_41.txt') as fh:
         exp = fh.read()
-    cmd = (
-        'python -m charex',
-        'cd',
-        '0b01000001',
-    )
-    cli_test(exp, cmd, capsys)
+    cmd = 'cd 0b01000001'
+    shell_test(exp, cmd, capsys)
 
 
-def test_cd_code_point(capsys):
-    """Called with a character, cd mode should interpret the base
-    string as binary and return the character or characters that hex
-    string becomes in each of the known character sets.
+def test_cd_string(capsys):
+    """Invoked with a character, `cd` returns the character for
+    that character's UTF-8 address in each registered character set.
     """
     with open('tests/data/charset_mode_41.txt') as fh:
         exp = fh.read()
-    cmd = (
-        'python -m charex',
-        'cd',
-        'A',
-    )
-    cli_test(exp, cmd, capsys)
+    cmd = 'cd A'
+    shell_test(exp, cmd, capsys)
 
 
-def test_cd_control_character(capsys):
-    """Called with an hex string, cd mode should return the character
-    or characters that hex string becomes in each of the known character
-    sets. If the hex string becomes a control character, print the symbol
-    for that character rather than the character itself.
-    """
-    with open('tests/data/charset_mode_0a.txt') as fh:
-        exp = fh.read()
-    cmd = (
-        'python -m charex',
-        'cd',
-        '0x0a'
-    )
-    cli_test(exp, cmd, capsys)
-
-
-def test_cd_no_character(capsys):
-    """Called with an hex string, cd mode should return the character
-    or characters that hex string becomes in each of the known character
-    sets. If some character sets do not have characters for the given
-    address, that should be indicated in the output.
-    """
-    with open('tests/data/charset_mode_e9.txt') as fh:
-        exp = fh.read()
-    cmd = (
-        'python -m charex',
-        'cd',
-        '0xe9'
-    )
-    cli_test(exp, cmd, capsys)
-
-
-# Test ce mode.
+# Tests for ce.
 def test_ce(capsys):
-    """Called with an character, ce mode should return the address
-    for the character in each of the registered character sets.
+    """Invoked with a character, `ce` returns the address for
+    that character in each registered character set.
     """
     with open('tests/data/charset_mode_r.txt') as fh:
         exp = fh.read()
-    cmd = (
-        'python -m charex',
-        'ce',
-        'A',
-    )
-    cli_test(exp, cmd, capsys)
+    cmd = 'ce A'
+    shell_test(exp, cmd, capsys)
 
 
-# Test cl mode.
+# Tests for cl.
 def test_cl(capsys):
-    """When invoked, cl mode should return a list of registered
-    character set codecs.
-    """
+    """Invoked, `cl` returns the list of registered character sets."""
     with open('tests/data/charsetlist.txt') as fh:
         exp = fh.read()
-    cmd = (
-        'python -m charex',
-        'cl'
-    )
-    cli_test(exp, cmd, capsys)
+    cmd = 'cl'
+    shell_test(exp, cmd, capsys)
 
 
 def test_cl_description(capsys):
-    """When invoked with -d, cl mode should return a list of
-    registered character set codecs and a brief description of each
-    one.
+    """Invoked with "-d", `cl` returns the list of registered character
+    sets with descriptions.
     """
     with open('tests/data/charsetlist_d.txt') as fh:
         exp = fh.read()
-    cmd = (
-        'python -m charex',
-        'cl',
-        '-d',
-    )
-    cli_test(exp, cmd, capsys)
+    cmd = 'cl -d'
+    shell_test(exp, cmd, capsys)
 
 
-# Test ct mode.
+# Tests for ct.
 def test_ct(capsys):
     """Invoked with a normalization form and a base string, ct mode
     should print the number of denormalizations using the given form to
     stdout.
     """
     exp = '120,270,240\n\n'
-    cmd = (
-        'python -m charex',
-        'ct',
-        'nfkd',
-        '<script>'
-    )
-    cli_test(exp, cmd, capsys)
+    cmd = 'ct nfkd <script>'
+    shell_test(exp, cmd, capsys)
 
 
 def test_ct_maxdepth(capsys):
     """Invoked with "-m" and an integer, ct mode limit the number of
     denormalizations per character to the given integer and print the
     number of denormalizations using the given form to stdout.
     """
     exp = '256\n\n'
-    cmd = (
-        'python -m charex',
-        'ct',
-        'nfkd',
-        '<script>',
-        '-m', '2',
-    )
-    cli_test(exp, cmd, capsys)
+    cmd = 'ct nfkd <script> -m 2'
+    shell_test(exp, cmd, capsys)
 
 
 # Test dn mode.
 def test_dn(capsys):
     """Invoked with a normalization form and a base string, dn mode
     should print the denormalizations for the base string to stdout.
     """
@@ -179,171 +107,212 @@
         '\uff1c\ufe63\ufe65\n'
         '\uff1c\ufe63\uff1e\n'
         '\uff1c\uff0d\ufe65\n'
         '\uff1c\uff0d\uff1e\n'
         '\n'
     )
     cmd = (
-        'python -m charex',
-        'dn',
-        'nfkd',
+        'dn '
+        'nfkd '
         '<->'
     )
-    cli_test(exp, cmd, capsys)
+    shell_test(exp, cmd, capsys)
 
 
-def test_dn_maxdepth(capsys):
+def test_dn_number(capsys):
     """Invoked with -n and an integer, dn mode should return no
     more than that number of results.
     """
     exp = (
         '\ufe64\ufe63\ufe65\n'
         '\n'
     )
     cmd = (
-        'python -m charex',
-        'dn',
-        'nfkd',
-        '<->',
-        '-m', '1'
+        'dn '
+        'nfkd '
+        '<-> '
+        '-m 1'
     )
-    cli_test(exp, cmd, capsys)
+    shell_test(exp, cmd, capsys)
 
 
 def test_dn_random(capsys):
     """Called with -r, dn mode should return a randomly
     denormalize the string.
     """
     exp = (
         '﹤－﹥\n'
         '\n'
     )
     cmd = (
-        'python -m charex',
-        'dn',
-        'nfkd',
-        '<->',
-        '-r',
-        '-s', 'spam'
+        'dn '
+        'nfkd '
+        '<-> '
+        '-r '
+        '-s spam'
     )
-    cli_test(exp, cmd, capsys)
+    shell_test(exp, cmd, capsys)
 
 
 # Test dt mode.
 def test_dt(capsys):
     """Invoked with a character, details mode should print the details
     for the character.
     """
     with open('tests/data/details_mode_A.txt') as fh:
         exp = fh.read()
     cmd = (
-        'python -m charex',
-        'dt',
+        'dt '
         'A'
     )
-    cli_test(exp, cmd, capsys)
+    shell_test(exp, cmd, capsys)
 
 
 # Test el mode.
 def test_el(capsys):
     """When invoked, el mode returns a list of the registered
     escape schemes.
     """
     exp = '\n'.join(scheme for scheme in esc.schemes) + '\n\n'
-    cmd = (
-        'python -m charex',
-        'el',
-    )
-    cli_test(exp, cmd, capsys)
+    cmd = 'el'
+    shell_test(exp, cmd, capsys)
 
 
 def test_el_description(capsys):
-    """When invoked with -d, cl mode should return a list of
-    registered escape schemes and a brief description of each
-    one.
+    """Invoked with "-d", `el` returns the list of registered character
+    sets with descriptions.
     """
     with open('tests/data/el_d.txt') as fh:
         exp = fh.read()
-    cmd = (
-        'python -m charex',
-        'el',
-        '-d',
-    )
-    cli_test(exp, cmd, capsys)
+    cmd = 'el -d'
+    shell_test(exp, cmd, capsys)
 
 
 # Test es mode.
 def test_es(capsys):
     """Invoked with a scheme and a base string, escape mode should
     escape the string using the given scheme and print the escaped
     string.
     """
     exp = '%41\n\n'
     cmd = (
-        'python -m charex',
-        'es',
-        'url',
-        'A',
+        'es '
+        'url '
+        'A'
     )
-    cli_test(exp, cmd, capsys)
+    shell_test(exp, cmd, capsys)
 
 
 # Test fl mode.
 def test_fl(capsys):
     """When invoked, fl mode returns a list of the registered
     normalization forms.
     """
     exp = '\n'.join(form for form in nl.forms) + '\n\n'
     cmd = (
-        'python -m charex',
-        'fl',
+        'fl'
     )
-    cli_test(exp, cmd, capsys)
+    shell_test(exp, cmd, capsys)
 
 
 def test_fl_description(capsys):
     """When invoked with -d, fl mode should return a list of
     registered normalization forms and a brief description of each
     one.
     """
     with open('tests/data/fl_d.txt') as fh:
         exp = fh.read()
     cmd = (
-        'python -m charex',
-        'fl',
-        '-d',
+        'fl '
+        '-d'
     )
-    cli_test(exp, cmd, capsys)
+    shell_test(exp, cmd, capsys)
 
 
 # Test nl mode.
 def test_nl(capsys):
     """When invoked with a normalization form and a base string,
     nl mode returns the normalization of the base string using the
     given form.
     """
     exp = 'A\n\n'
     cmd = (
-        'python -m charex',
-        'nl',
-        'nfkc',
-        '\u24b6',
+        'nl '
+        'nfkc '
+        '\u24b6'
     )
-    cli_test(exp, cmd, capsys)
+    shell_test(exp, cmd, capsys)
 
 
-# Utility functions.
-def cli_test(exp, cmd, capsys):
-    """Test command line invocation."""
-    # Test set up.
-    orig_cmd = sys.argv
-    sys.argv = cmd
+# Test pf mode.
+def test_pf(capsys):
+    """When invoked, pf mode should return the list characters with the
+    given property value.
+    """
+    exp = (
+        '🏻 U+1F3FB (EMOJI MODIFIER FITZPATRICK TYPE-1-2)\n'
+        '🏼 U+1F3FC (EMOJI MODIFIER FITZPATRICK TYPE-3)\n'
+        '🏽 U+1F3FD (EMOJI MODIFIER FITZPATRICK TYPE-4)\n'
+        '🏾 U+1F3FE (EMOJI MODIFIER FITZPATRICK TYPE-5)\n'
+        '🏿 U+1F3FF (EMOJI MODIFIER FITZPATRICK TYPE-6)\n'
+        '\n'
+    )
+    cmd = (
+        'pf '
+        'emod '
+        'Y'
+    )
+    shell_test(exp, cmd, capsys)
+
+
+def test_pf_insensitive(capsys):
+    """When invoked, pf mode should return the list characters with the
+    given property value.
+    """
+    exp = (
+        '🏻 U+1F3FB (EMOJI MODIFIER FITZPATRICK TYPE-1-2)\n'
+        '🏼 U+1F3FC (EMOJI MODIFIER FITZPATRICK TYPE-3)\n'
+        '🏽 U+1F3FD (EMOJI MODIFIER FITZPATRICK TYPE-4)\n'
+        '🏾 U+1F3FE (EMOJI MODIFIER FITZPATRICK TYPE-5)\n'
+        '🏿 U+1F3FF (EMOJI MODIFIER FITZPATRICK TYPE-6)\n'
+        '\n'
+    )
+    cmd = (
+        'pf '
+        'emod '
+        'y '
+        '-i'
+    )
+    shell_test(exp, cmd, capsys)
+
+
+# Test up mode.
+def test_up(capsys):
+    """When invoked, up mode should return the list of Unicode properties."""
+    with open('tests/data/up.txt') as fh:
+        exp = fh.read()
+    cmd = (
+        'up'
+    )
+    shell_test(exp, cmd, capsys)
 
-    # Run test.
-    m.sh.invoke()
 
-    # Gather actual result and compare.
+def test_up_description(capsys):
+    """When invoked with -d, up mode should return a list of
+    Unicode properties and their long names.
+    """
+    with open('tests/data/up_d.txt') as fh:
+        exp = fh.read()
+    cmd = (
+        'up '
+        '-d'
+    )
+    shell_test(exp, cmd, capsys)
+
+
+# Utility functions.
+def shell_test(exp, cmd, capsys):
+    """Test shell invocation."""
+    shell = sh.Shell()
+    shell.onecmd(cmd)
     captured = capsys.readouterr()
     assert captured.out == exp
-
-    # Test tear down.
-    sys.argv = orig_cmd
```

### Comparing `charex-0.1.0/tests/test_normal.py` & `charex-0.2.0/tests/test_normal.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,22 +92,22 @@
     scheme = 'nfkc'
     base = '\u24b6'
     assert nl.normalize(scheme, base) == exp
 
 
 # Tests for build_denormalization_map().
 def test_build_denormalization_map():
-    """When given a denormalization function,
+    """When given the key for a denormalization function,
     :func:`charex.normal.build_denormalization_map` will return a map
     of every character that normalizes into a character as a
     JSON string.
     """
     with open('charex/data/rev_nfc.json') as fh:
-        exp = fh.read()[:-2]
-    form = nl.form_nfc
+        exp = fh.read()
+    form = 'nfc'
     act = nl.build_denormalization_map(form)
     alines = act.split('\n')
     elines = exp.split('\n')
     for i, lines in enumerate(zip(alines, elines)):
         a, e = lines
         assert (i, a) == (i, e)
     assert act == exp
```

### Comparing `charex-0.1.0/tests/test_utility.py` & `charex-0.2.0/tests/test_utility.py`

 * *Files 10% similar despite different names*

```diff
@@ -107,16 +107,27 @@
     assert act == exp
 
 
 def test_to_bytes_unicode():
     """Given a :class:`str` containing a Unicode code point, return that
     code point as an UTF-8 encoded :class:`bytes`.
     """
-    exp = b'\xe9'
-    value = '0b11101001'
+    exp = b'\x61'
+    value = 'U+0061'
+    act = util.to_bytes(value)
+    assert act == exp
+
+
+def test_to_bytes_unicode_lowercase_u():
+    """Given a :class:`str` containing a Unicode code point, return that
+    code point as an UTF-8 encoded :class:`bytes`. The code point can
+    start with a lowercase u.
+    """
+    exp = b'\x61'
+    value = 'u+0061'
     act = util.to_bytes(value)
     assert act == exp
 
 
 # Tests for to_char.
 def to_char():
     """Given a :class:`str` with length one, return that :class:`str`."""
@@ -192,7 +203,17 @@
 def test_to_char_unicode():
     """Given a Unicode code point string, return a one character
     :class:`str` of the unicode code point.
     """
     exp = 'a'
     value = 'U+0061'
     assert util.to_char(value) == exp
+
+
+def test_to_char_unicode_lowercase_u():
+    """Given a Unicode code point string, return a one character
+    :class:`str` of the unicode code point. The code point can start
+    with a lowercase letter u.
+    """
+    exp = 'a'
+    value = 'u+0061'
+    assert util.to_char(value) == exp
```

