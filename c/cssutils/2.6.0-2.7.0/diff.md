# Comparing `tmp/cssutils-2.6.0.tar.gz` & `tmp/cssutils-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cssutils-2.6.0.tar", last modified: Mon Aug 22 02:26:05 2022, max compression
+gzip compressed data, was "cssutils-2.7.0.tar", last modified: Fri Jun  9 01:46:59 2023, max compression
```

## Comparing `cssutils-2.6.0.tar` & `cssutils-2.7.0.tar`

### file list

```diff
@@ -1,353 +1,354 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 02:26:05.044268 cssutils-2.6.0/
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-08-22 02:25:33.000000 cssutils-2.6.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-08-22 02:25:33.000000 cssutils-2.6.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-08-22 02:25:33.000000 cssutils-2.6.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 02:26:04.972268 cssutils-2.6.0/.github/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-08-22 02:25:33.000000 cssutils-2.6.0/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-08-22 02:25:33.000000 cssutils-2.6.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 02:26:04.972268 cssutils-2.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1418 2022-08-22 02:25:33.000000 cssutils-2.6.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-08-22 02:25:33.000000 cssutils-2.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-08-22 02:25:33.000000 cssutils-2.6.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)   121893 2022-08-22 02:25:33.000000 cssutils-2.6.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)    35821 2022-08-22 02:25:33.000000 cssutils-2.6.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (121)     7802 2022-08-22 02:25:33.000000 cssutils-2.6.0/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (121)     8274 2022-08-22 02:26:05.044268 cssutils-2.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7345 2022-08-22 02:25:33.000000 cssutils-2.6.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      756 2022-08-22 02:25:33.000000 cssutils-2.6.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 02:26:04.972268 cssutils-2.6.0/cssutils/
--rw-r--r--   0 runner    (1001) docker     (121)    13946 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1747 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/_fetch.py
--rw-r--r--   0 runner    (1001) docker     (121)     2495 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/_fetchgae.py
--rw-r--r--   0 runner    (1001) docker     (121)    22279 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/codec.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 02:26:04.976268 cssutils-2.6.0/cssutils/css/
--rw-r--r--   0 runner    (1001) docker     (121)     2125 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/css/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6459 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/css/colors.py
--rw-r--r--   0 runner    (1001) docker     (121)     5977 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/css/csscharsetrule.py
--rw-r--r--   0 runner    (1001) docker     (121)     2737 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/css/csscomment.py
--rw-r--r--   0 runner    (1001) docker     (121)     6531 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/css/cssfontfacerule.py
--rw-r--r--   0 runner    (1001) docker     (121)    14636 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/css/cssimportrule.py
--rw-r--r--   0 runner    (1001) docker     (121)    11980 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/css/cssmediarule.py
--rw-r--r--   0 runner    (1001) docker     (121)    11314 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/css/cssnamespacerule.py
--rw-r--r--   0 runner    (1001) docker     (121)    15492 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/css/csspagerule.py
--rw-r--r--   0 runner    (1001) docker     (121)     5190 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/css/cssproperties.py
--rw-r--r--   0 runner    (1001) docker     (121)    11408 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/css/cssrule.py
--rw-r--r--   0 runner    (1001) docker     (121)     1970 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/css/cssrulelist.py
--rw-r--r--   0 runner    (1001) docker     (121)    27117 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/css/cssstyledeclaration.py
--rw-r--r--   0 runner    (1001) docker     (121)     9277 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/css/cssstylerule.py
--rw-r--r--   0 runner    (1001) docker     (121)    33791 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/css/cssstylesheet.py
--rw-r--r--   0 runner    (1001) docker     (121)     8294 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/css/cssunknownrule.py
--rw-r--r--   0 runner    (1001) docker     (121)    47947 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/css/cssvalue.py
--rw-r--r--   0 runner    (1001) docker     (121)    11616 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/css/cssvariablesdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (121)     7179 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/css/cssvariablesrule.py
--rw-r--r--   0 runner    (1001) docker     (121)     6885 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/css/marginrule.py
--rw-r--r--   0 runner    (1001) docker     (121)    18306 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/css/property.py
--rw-r--r--   0 runner    (1001) docker     (121)    32606 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/css/selector.py
--rw-r--r--   0 runner    (1001) docker     (121)     8376 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/css/selectorlist.py
--rw-r--r--   0 runner    (1001) docker     (121)    32593 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/css/value.py
--rw-r--r--   0 runner    (1001) docker     (121)     6047 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/css2productions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4678 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/cssproductions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3768 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/errorhandler.py
--rw-r--r--   0 runner    (1001) docker     (121)     3693 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     8552 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/parse.py
--rw-r--r--   0 runner    (1001) docker     (121)    27812 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/prodparser.py
--rw-r--r--   0 runner    (1001) docker     (121)    34876 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/profiles.py
--rw-r--r--   0 runner    (1001) docker     (121)    17249 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/sac.py
--rw-r--r--   0 runner    (1001) docker     (121)    12099 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/script.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 02:26:04.976268 cssutils-2.6.0/cssutils/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2451 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/scripts/csscapture.py
--rw-r--r--   0 runner    (1001) docker     (121)     3125 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/scripts/csscombine.py
--rw-r--r--   0 runner    (1001) docker     (121)     2078 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/scripts/cssparse.py
--rw-r--r--   0 runner    (1001) docker     (121)    42014 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/serialize.py
--rw-r--r--   0 runner    (1001) docker     (121)      549 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 02:26:04.976268 cssutils-2.6.0/cssutils/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (121)      351 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/stylesheets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8982 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/stylesheets/medialist.py
--rw-r--r--   0 runner    (1001) docker     (121)     7060 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/stylesheets/mediaquery.py
--rw-r--r--   0 runner    (1001) docker     (121)     5228 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/stylesheets/stylesheet.py
--rw-r--r--   0 runner    (1001) docker     (121)     1100 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/stylesheets/stylesheetlist.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 02:26:04.980268 cssutils-2.6.0/cssutils/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1791 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/basetest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 02:26:04.992268 cssutils-2.6.0/cssutils/tests/sheets/
--rw-r--r--   0 runner    (1001) docker     (121)     4249 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/096.css
--rw-r--r--   0 runner    (1001) docker     (121)     4249 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/097.css
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/1.css
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/1ascii.css
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/1import.css
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/1inherit-ascii.css
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/1inherit-iso.css
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/1inherit-utf8.css
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/1utf.css
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/2inherit-iso.css
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/2resolve.css
--rw-r--r--   0 runner    (1001) docker     (121)     9502 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/acid2.css
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/all.css
--rw-r--r--   0 runner    (1001) docker     (121)      137 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/atrule.css
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/bad.css
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/basic.css
--rw-r--r--   0 runner    (1001) docker     (121)   208303 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/bundle.css
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/cases.css
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/csscombine-1.css
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/csscombine-2.css
--rw-r--r--   0 runner    (1001) docker     (121)      220 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/csscombine-proxy.css
--rw-r--r--   0 runner    (1001) docker     (121)     3851 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/cthedot_default.css
--rw-r--r--   0 runner    (1001) docker     (121)     2797 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/default_html4.css
--rw-r--r--   0 runner    (1001) docker     (121)      733 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/hacks.css
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/html.css
--rw-r--r--   0 runner    (1001) docker     (121)     1503 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/html20.css
--rw-r--r--   0 runner    (1001) docker     (121)     4274 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/html40.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 02:26:04.992268 cssutils-2.6.0/cssutils/tests/sheets/images/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/images/example.gif
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 02:26:04.992268 cssutils-2.6.0/cssutils/tests/sheets/import/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 02:26:04.992268 cssutils-2.6.0/cssutils/tests/sheets/import/images2/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/import/images2/example2.gif
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/import/import-impossible.css
--rw-r--r--   0 runner    (1001) docker     (121)      427 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/import/import2.css
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/import.css
--rw-r--r--   0 runner    (1001) docker     (121)      307 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/import3.css
--rw-r--r--   0 runner    (1001) docker     (121)     9402 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/ll.css
--rw-r--r--   0 runner    (1001) docker     (121)    97995 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/ll2.css
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/multiple-values.css
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/page_test.css
--rw-r--r--   0 runner    (1001) docker     (121)    17998 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/sample_5.css
--rw-r--r--   0 runner    (1001) docker     (121)     7662 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/sample_7.css
--rw-r--r--   0 runner    (1001) docker     (121)      305 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/simple.css
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/single-color.css
--rw-r--r--   0 runner    (1001) docker     (121)    18645 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/slashcode.css
--rw-r--r--   0 runner    (1001) docker     (121)      677 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/t-HACKS.css
--rw-r--r--   0 runner    (1001) docker     (121)     9268 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/test-unicode.css
--rw-r--r--   0 runner    (1001) docker     (121)     4369 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/test.css
--rw-r--r--   0 runner    (1001) docker     (121)     8665 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/tigris.css
--rw-r--r--   0 runner    (1001) docker     (121)     9082 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/tigris2.css
--rw-r--r--   0 runner    (1001) docker     (121)      296 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/u_simple.css
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/v_simple.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 02:26:04.992268 cssutils-2.6.0/cssutils/tests/sheets/var/
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/var/start.css
--rw-r--r--   0 runner    (1001) docker     (121)      290 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/var/use.css
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/var/vars.css
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/var/vars2.css
--rw-r--r--   0 runner    (1001) docker     (121)      222 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/vars.css
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/varsimport.css
--rw-r--r--   0 runner    (1001) docker     (121)     4910 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/xhtml2.css
--rw-r--r--   0 runner    (1001) docker     (121)     4825 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/xhtml22.css
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/sheets/yuck.css
--rw-r--r--   0 runner    (1001) docker     (121)    14389 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/test_codec.py
--rw-r--r--   0 runner    (1001) docker     (121)     4034 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/test_csscharsetrule.py
--rw-r--r--   0 runner    (1001) docker     (121)     1958 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/test_csscomment.py
--rw-r--r--   0 runner    (1001) docker     (121)     8092 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/test_cssfontfacerule.py
--rw-r--r--   0 runner    (1001) docker     (121)    16628 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/test_cssimportrule.py
--rw-r--r--   0 runner    (1001) docker     (121)    17061 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/test_cssmediarule.py
--rw-r--r--   0 runner    (1001) docker     (121)     8408 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/test_cssnamespacerule.py
--rw-r--r--   0 runner    (1001) docker     (121)    13502 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/test_csspagerule.py
--rw-r--r--   0 runner    (1001) docker     (121)     2361 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/test_cssproperties.py
--rw-r--r--   0 runner    (1001) docker     (121)     8181 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/test_cssrule.py
--rw-r--r--   0 runner    (1001) docker     (121)      995 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/test_cssrulelist.py
--rw-r--r--   0 runner    (1001) docker     (121)    22215 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/test_cssstyledeclaration.py
--rw-r--r--   0 runner    (1001) docker     (121)     8615 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/test_cssstylerule.py
--rw-r--r--   0 runner    (1001) docker     (121)    32384 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/test_cssstylesheet.py
--rw-r--r--   0 runner    (1001) docker     (121)     4862 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/test_cssunknownrule.py
--rw-r--r--   0 runner    (1001) docker     (121)    16756 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/test_cssutils.py
--rw-r--r--   0 runner    (1001) docker     (121)      498 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/test_cssutilsimport.py
--rw-r--r--   0 runner    (1001) docker     (121)    33126 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/test_cssvalue.py
--rw-r--r--   0 runner    (1001) docker     (121)    10051 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/test_cssvariablesdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (121)     4717 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/test_cssvariablesrule.py
--rw-r--r--   0 runner    (1001) docker     (121)     1445 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/test_domimplementation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 02:26:04.992268 cssutils-2.6.0/cssutils/tests/test_encutils/
--rw-r--r--   0 runner    (1001) docker     (121)    17678 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/test_encutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4829 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/test_errorhandler.py
--rw-r--r--   0 runner    (1001) docker     (121)     2740 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     3188 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/test_marginrule.py
--rw-r--r--   0 runner    (1001) docker     (121)     6304 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/test_medialist.py
--rw-r--r--   0 runner    (1001) docker     (121)     3259 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/test_mediaquery.py
--rw-r--r--   0 runner    (1001) docker     (121)    19546 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (121)    13847 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/test_prodparser.py
--rw-r--r--   0 runner    (1001) docker     (121)    23382 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/test_profiles.py
--rw-r--r--   0 runner    (1001) docker     (121)     8248 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/test_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     8685 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/test_property.py
--rw-r--r--   0 runner    (1001) docker     (121)     2194 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/test_scripts_csscombine.py
--rw-r--r--   0 runner    (1001) docker     (121)    16106 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/test_selector.py
--rw-r--r--   0 runner    (1001) docker     (121)     4308 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/test_selectorlist.py
--rw-r--r--   0 runner    (1001) docker     (121)    25836 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/test_serialize.py
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/test_stylesheet.py
--rw-r--r--   0 runner    (1001) docker     (121)    22385 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/test_tokenize2.py
--rw-r--r--   0 runner    (1001) docker     (121)    20638 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (121)    46131 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/test_value.py
--rw-r--r--   0 runner    (1001) docker     (121)     1630 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tests/test_x.py
--rw-r--r--   0 runner    (1001) docker     (121)    11763 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/tokenize2.py
--rw-r--r--   0 runner    (1001) docker     (121)    34374 2022-08-22 02:25:33.000000 cssutils-2.6.0/cssutils/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 02:26:04.972268 cssutils-2.6.0/cssutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8274 2022-08-22 02:26:04.000000 cssutils-2.6.0/cssutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8879 2022-08-22 02:26:04.000000 cssutils-2.6.0/cssutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 02:26:04.000000 cssutils-2.6.0/cssutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-08-22 02:26:04.000000 cssutils-2.6.0/cssutils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      427 2022-08-22 02:26:04.000000 cssutils-2.6.0/cssutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-08-22 02:26:04.000000 cssutils-2.6.0/cssutils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 02:26:04.996268 cssutils-2.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     2272 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/backlog.rst
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/codec.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1248 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     8701 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/css.rst
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/encutils.rst
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/history.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 02:26:05.004268 cssutils-2.6.0/docs/html/
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/.buildinfo
--rw-r--r--   0 runner    (1001) docker     (121)   217445 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/CHANGELOG.html
--rw-r--r--   0 runner    (1001) docker     (121)    17807 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/README.html
--rw-r--r--   0 runner    (1001) docker     (121)     3665 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/_2to3 py3.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 02:26:05.004268 cssutils-2.6.0/docs/html/_sources/
--rw-r--r--   0 runner    (1001) docker     (121)   116989 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/_sources/CHANGELOG.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5751 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/_sources/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 02:26:05.004268 cssutils-2.6.0/docs/html/_sources/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     2452 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/_sources/docs/backlog.txt
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/_sources/docs/codec.txt
--rw-r--r--   0 runner    (1001) docker     (121)     8751 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/_sources/docs/css.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6138 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/_sources/docs/cssstyledeclaration.txt
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/_sources/docs/cssutils.txt
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/_sources/docs/encutils.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2812 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/_sources/docs/implementation.txt
--rw-r--r--   0 runner    (1001) docker     (121)      967 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/_sources/docs/logging.txt
--rw-r--r--   0 runner    (1001) docker     (121)     8190 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/_sources/docs/migrate.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2481 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/_sources/docs/parse.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/_sources/docs/profiles.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6932 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/_sources/docs/scripts.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1818 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/_sources/docs/serialize.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1120 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/_sources/docs/settings.txt
--rw-r--r--   0 runner    (1001) docker     (121)      758 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/_sources/docs/stylesheets.txt
--rw-r--r--   0 runner    (1001) docker     (121)      359 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/_sources/docs/utilities.txt
--rw-r--r--   0 runner    (1001) docker     (121)      447 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/_sources/docs/variables.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1240 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/_sources/index.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 02:26:05.012268 cssutils-2.6.0/docs/html/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     8269 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/_static/basic.css
--rw-r--r--   0 runner    (1001) docker     (121)     4040 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/_static/default.css
--rw-r--r--   0 runner    (1001) docker     (121)     6871 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/_static/doctools.js
--rw-r--r--   0 runner    (1001) docker     (121)      392 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/_static/file.png
--rw-r--r--   0 runner    (1001) docker     (121)    72174 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/_static/jquery.js
--rw-r--r--   0 runner    (1001) docker     (121)      199 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (121)      199 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/_static/plus.png
--rw-r--r--   0 runner    (1001) docker     (121)     3993 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/_static/pygments.css
--rw-r--r--   0 runner    (1001) docker     (121)    14509 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/_static/searchtools.js
--rw-r--r--   0 runner    (1001) docker     (121)     4634 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/_static/sidebar.js
--rw-r--r--   0 runner    (1001) docker     (121)     8205 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/_static/underscore.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 02:26:05.016268 cssutils-2.6.0/docs/html/docs/
--rw-r--r--   0 runner    (1001) docker     (121)    10377 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/docs/backlog.html
--rw-r--r--   0 runner    (1001) docker     (121)     4328 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/docs/codec.html
--rw-r--r--   0 runner    (1001) docker     (121)   167032 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/docs/css.html
--rw-r--r--   0 runner    (1001) docker     (121)    24168 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/docs/encutils.html
--rw-r--r--   0 runner    (1001) docker     (121)     6609 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/docs/logging.html
--rw-r--r--   0 runner    (1001) docker     (121)    27207 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/docs/migrate.html
--rw-r--r--   0 runner    (1001) docker     (121)    28207 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/docs/parse.html
--rw-r--r--   0 runner    (1001) docker     (121)    22715 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/docs/profiles.html
--rw-r--r--   0 runner    (1001) docker     (121)    18744 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/docs/scripts.html
--rw-r--r--   0 runner    (1001) docker     (121)    15756 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/docs/serialize.html
--rw-r--r--   0 runner    (1001) docker     (121)     6593 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/docs/settings.html
--rw-r--r--   0 runner    (1001) docker     (121)    21169 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/docs/stylesheets.html
--rw-r--r--   0 runner    (1001) docker     (121)    11209 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/docs/utilities.html
--rw-r--r--   0 runner    (1001) docker     (121)     4762 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/docs/variables.html
--rw-r--r--   0 runner    (1001) docker     (121)    50793 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/genindex.html
--rw-r--r--   0 runner    (1001) docker     (121)    20302 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/index.html
--rw-r--r--   0 runner    (1001) docker     (121)     5133 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/py-modindex.html
--rw-r--r--   0 runner    (1001) docker     (121)     3370 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/search.html
--rw-r--r--   0 runner    (1001) docker     (121)    42048 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/html/searchindex.js
--rw-r--r--   0 runner    (1001) docker     (121)      691 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2672 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/known issues.rst
--rw-r--r--   0 runner    (1001) docker     (121)      943 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/logging.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7988 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/migrate.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2506 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/parse.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2475 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/profiles.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6760 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/scripts.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1744 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/serialize.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1096 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/settings.rst
--rw-r--r--   0 runner    (1001) docker     (121)      728 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/stylesheets.rst
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/utilities.rst
--rw-r--r--   0 runner    (1001) docker     (121)      414 2022-08-22 02:25:33.000000 cssutils-2.6.0/docs/variables.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 02:26:05.020268 cssutils-2.6.0/encutils/
--rw-r--r--   0 runner    (1001) docker     (121)    21212 2022-08-22 02:25:33.000000 cssutils-2.6.0/encutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 02:26:05.024268 cssutils-2.6.0/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     2929 2022-08-22 02:25:33.000000 cssutils-2.6.0/examples/build.py
--rw-r--r--   0 runner    (1001) docker     (121)      332 2022-08-22 02:25:33.000000 cssutils-2.6.0/examples/codec.py
--rw-r--r--   0 runner    (1001) docker     (121)     1668 2022-08-22 02:25:33.000000 cssutils-2.6.0/examples/cssencodings.py
--rw-r--r--   0 runner    (1001) docker     (121)      683 2022-08-22 02:25:33.000000 cssutils-2.6.0/examples/customlog.py
--rw-r--r--   0 runner    (1001) docker     (121)      894 2022-08-22 02:25:33.000000 cssutils-2.6.0/examples/imports.py
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-08-22 02:25:33.000000 cssutils-2.6.0/examples/minify.py
--rw-r--r--   0 runner    (1001) docker     (121)     1371 2022-08-22 02:25:33.000000 cssutils-2.6.0/examples/parse.py
--rw-r--r--   0 runner    (1001) docker     (121)     1482 2022-08-22 02:25:33.000000 cssutils-2.6.0/examples/properties_with_same_name.py
--rw-r--r--   0 runner    (1001) docker     (121)     1404 2022-08-22 02:25:33.000000 cssutils-2.6.0/examples/selectors_tolower.py
--rw-r--r--   0 runner    (1001) docker     (121)     1775 2022-08-22 02:25:33.000000 cssutils-2.6.0/examples/serialize.py
--rw-r--r--   0 runner    (1001) docker     (121)     7237 2022-08-22 02:25:33.000000 cssutils-2.6.0/examples/style.py
--rw-r--r--   0 runner    (1001) docker     (121)     1341 2022-08-22 02:25:33.000000 cssutils-2.6.0/examples/styledeclaration.py
--rw-r--r--   0 runner    (1001) docker     (121)     2179 2022-08-22 02:25:33.000000 cssutils-2.6.0/examples/testutil.py
--rw-r--r--   0 runner    (1001) docker     (121)     5688 2022-08-22 02:25:33.000000 cssutils-2.6.0/examples/website.py
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-08-22 02:25:33.000000 cssutils-2.6.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)      380 2022-08-22 02:25:33.000000 cssutils-2.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      910 2022-08-22 02:25:33.000000 cssutils-2.6.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)     1670 2022-08-22 02:26:05.044268 cssutils-2.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 02:26:05.040269 cssutils-2.6.0/sheets/
--rw-r--r--   0 runner    (1001) docker     (121)     4249 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/096.css
--rw-r--r--   0 runner    (1001) docker     (121)     4249 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/097.css
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/1.css
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/1ascii.css
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/1import.css
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/1inherit-ascii.css
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/1inherit-iso.css
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/1inherit-utf8.css
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/1utf.css
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/2inherit-iso.css
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/2resolve.css
--rw-r--r--   0 runner    (1001) docker     (121)     9502 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/acid2.css
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/all.css
--rw-r--r--   0 runner    (1001) docker     (121)      137 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/atrule.css
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/bad.css
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/basic.css
--rw-r--r--   0 runner    (1001) docker     (121)   208303 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/bundle.css
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/cases.css
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/csscombine-1.css
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/csscombine-2.css
--rw-r--r--   0 runner    (1001) docker     (121)      220 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/csscombine-proxy.css
--rw-r--r--   0 runner    (1001) docker     (121)     3851 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/cthedot_default.css
--rw-r--r--   0 runner    (1001) docker     (121)     2797 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/default_html4.css
--rw-r--r--   0 runner    (1001) docker     (121)      733 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/hacks.css
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/html.css
--rw-r--r--   0 runner    (1001) docker     (121)     1503 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/html20.css
--rw-r--r--   0 runner    (1001) docker     (121)     4274 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/html40.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 02:26:05.040269 cssutils-2.6.0/sheets/images/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/images/example.gif
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 02:26:05.040269 cssutils-2.6.0/sheets/import/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 02:26:05.040269 cssutils-2.6.0/sheets/import/images2/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/import/images2/example2.gif
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/import/import-impossible.css
--rw-r--r--   0 runner    (1001) docker     (121)      427 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/import/import2.css
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/import.css
--rw-r--r--   0 runner    (1001) docker     (121)      307 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/import3.css
--rw-r--r--   0 runner    (1001) docker     (121)     9402 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/ll.css
--rw-r--r--   0 runner    (1001) docker     (121)    97995 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/ll2.css
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/multiple-values.css
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/page_test.css
--rw-r--r--   0 runner    (1001) docker     (121)    17998 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/sample_5.css
--rw-r--r--   0 runner    (1001) docker     (121)     7662 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/sample_7.css
--rw-r--r--   0 runner    (1001) docker     (121)      305 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/simple.css
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/single-color.css
--rw-r--r--   0 runner    (1001) docker     (121)    18645 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/slashcode.css
--rw-r--r--   0 runner    (1001) docker     (121)      677 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/t-HACKS.css
--rw-r--r--   0 runner    (1001) docker     (121)     9268 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/test-unicode.css
--rw-r--r--   0 runner    (1001) docker     (121)     4369 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/test.css
--rw-r--r--   0 runner    (1001) docker     (121)     8665 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/tigris.css
--rw-r--r--   0 runner    (1001) docker     (121)     9082 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/tigris2.css
--rw-r--r--   0 runner    (1001) docker     (121)      296 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/u_simple.css
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/v_simple.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 02:26:05.044268 cssutils-2.6.0/sheets/var/
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/var/start.css
--rw-r--r--   0 runner    (1001) docker     (121)      290 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/var/use.css
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/var/vars.css
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/var/vars2.css
--rw-r--r--   0 runner    (1001) docker     (121)      222 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/vars.css
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/varsimport.css
--rw-r--r--   0 runner    (1001) docker     (121)     4910 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/xhtml2.css
--rw-r--r--   0 runner    (1001) docker     (121)     4825 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/xhtml22.css
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-08-22 02:25:33.000000 cssutils-2.6.0/sheets/yuck.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 02:26:05.044268 cssutils-2.6.0/tools/
--rw-r--r--   0 runner    (1001) docker     (121)      767 2022-08-22 02:25:33.000000 cssutils-2.6.0/tools/speed.py
--rw-r--r--   0 runner    (1001) docker     (121)    37596 2022-08-22 02:25:33.000000 cssutils-2.6.0/tools/try.py
--rw-r--r--   0 runner    (1001) docker     (121)      732 2022-08-22 02:25:33.000000 cssutils-2.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.229071 cssutils-2.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-09 01:46:33.000000 cssutils-2.7.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-09 01:46:33.000000 cssutils-2.7.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.177068 cssutils-2.7.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-09 01:46:33.000000 cssutils-2.7.0/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-09 01:46:33.000000 cssutils-2.7.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.177068 cssutils-2.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-09 01:46:33.000000 cssutils-2.7.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-09 01:46:33.000000 cssutils-2.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-09 01:46:33.000000 cssutils-2.7.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   122074 2023-06-09 01:46:33.000000 cssutils-2.7.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35821 2023-06-09 01:46:33.000000 cssutils-2.7.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-06-09 01:46:33.000000 cssutils-2.7.0/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-06-09 01:46:59.229071 cssutils-2.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7480 2023-06-09 01:46:33.000000 cssutils-2.7.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-09 01:46:33.000000 cssutils-2.7.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.181068 cssutils-2.7.0/cssutils/
+-rw-r--r--   0 runner    (1001) docker     (123)    13946 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/_fetchgae.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22279 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/codec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.185068 cssutils-2.7.0/cssutils/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/csscharsetrule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/csscomment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/cssfontfacerule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/cssimportrule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11980 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/cssmediarule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11314 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/cssnamespacerule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15491 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/csspagerule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/cssproperties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11407 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/cssrule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/cssrulelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27117 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/cssstyledeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9277 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/cssstylerule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33791 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/cssstylesheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/cssunknownrule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47947 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/cssvalue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11616 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/cssvariablesdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/cssvariablesrule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/marginrule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18305 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32606 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/selectorlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32593 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/css2productions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/cssproductions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/errorhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8552 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27811 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/prodparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34876 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17249 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/sac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/script.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.185068 cssutils-2.7.0/cssutils/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/scripts/csscapture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/scripts/csscombine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/scripts/cssparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42013 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.185068 cssutils-2.7.0/cssutils/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/stylesheets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/stylesheets/medialist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/stylesheets/mediaquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/stylesheets/stylesheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/stylesheets/stylesheetlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.189069 cssutils-2.7.0/cssutils/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/basetest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.197069 cssutils-2.7.0/cssutils/tests/sheets/
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/096.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/097.css
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/1.css
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/1ascii.css
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/1import.css
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/1inherit-ascii.css
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/1inherit-iso.css
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/1inherit-utf8.css
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/1utf.css
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/2inherit-iso.css
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/2resolve.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/acid2.css
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/all.css
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/atrule.css
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/bad.css
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/basic.css
+-rw-r--r--   0 runner    (1001) docker     (123)   208303 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/bundle.css
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/cases.css
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/csscombine-1.css
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/csscombine-2.css
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/csscombine-proxy.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/cthedot_default.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/default_html4.css
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/hacks.css
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/html.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/html20.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/html40.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.197069 cssutils-2.7.0/cssutils/tests/sheets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/images/example.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.197069 cssutils-2.7.0/cssutils/tests/sheets/import/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.197069 cssutils-2.7.0/cssutils/tests/sheets/import/images2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/import/images2/example2.gif
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/import/import-impossible.css
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/import/import2.css
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/import.css
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/import3.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/ll.css
+-rw-r--r--   0 runner    (1001) docker     (123)    97995 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/ll2.css
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/multiple-values.css
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/page_test.css
+-rw-r--r--   0 runner    (1001) docker     (123)    17998 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/sample_5.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/sample_7.css
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/simple.css
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/single-color.css
+-rw-r--r--   0 runner    (1001) docker     (123)    18645 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/slashcode.css
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/t-HACKS.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/test-unicode.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/test.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8665 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/tigris.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9082 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/tigris2.css
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/u_simple.css
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/v_simple.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.197069 cssutils-2.7.0/cssutils/tests/sheets/var/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/var/start.css
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/var/use.css
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/var/vars.css
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/var/vars2.css
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/vars.css
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/varsimport.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/xhtml2.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/xhtml22.css
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/sheets/yuck.css
+-rw-r--r--   0 runner    (1001) docker     (123)    14389 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_codec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_csscharsetrule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_csscomment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_cssfontfacerule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16588 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_cssimportrule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17061 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_cssmediarule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8408 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_cssnamespacerule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13502 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_csspagerule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_cssproperties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_cssrule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_cssrulelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22222 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_cssstyledeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8615 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_cssstylerule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32396 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_cssstylesheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_cssunknownrule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16770 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_cssutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_cssutilsimport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33005 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_cssvalue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_cssvariablesdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_cssvariablesrule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_domimplementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.197069 cssutils-2.7.0/cssutils/tests/test_encutils/
+-rw-r--r--   0 runner    (1001) docker     (123)    17678 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_encutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_errorhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_marginrule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_medialist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_mediaquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19546 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13854 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_prodparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23382 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_scripts_csscombine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15914 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_selectorlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25825 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_stylesheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22391 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_tokenize2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20706 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45998 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tests/test_x.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11762 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/tokenize2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34374 2023-06-09 01:46:33.000000 cssutils-2.7.0/cssutils/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.181068 cssutils-2.7.0/cssutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-06-09 01:46:59.000000 cssutils-2.7.0/cssutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-06-09 01:46:59.000000 cssutils-2.7.0/cssutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 01:46:59.000000 cssutils-2.7.0/cssutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-09 01:46:59.000000 cssutils-2.7.0/cssutils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-09 01:46:59.000000 cssutils-2.7.0/cssutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-09 01:46:59.000000 cssutils-2.7.0/cssutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.201069 cssutils-2.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/backlog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/codec.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/css.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/encutils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/history.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.201069 cssutils-2.7.0/docs/html/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/.buildinfo
+-rw-r--r--   0 runner    (1001) docker     (123)   217445 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/CHANGELOG.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17807 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/README.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_2to3 py3.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.201069 cssutils-2.7.0/docs/html/_sources/
+-rw-r--r--   0 runner    (1001) docker     (123)   116989 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_sources/CHANGELOG.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_sources/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.209070 cssutils-2.7.0/docs/html/_sources/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_sources/docs/backlog.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_sources/docs/codec.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_sources/docs/css.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_sources/docs/cssstyledeclaration.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_sources/docs/cssutils.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_sources/docs/encutils.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_sources/docs/implementation.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_sources/docs/logging.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_sources/docs/migrate.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_sources/docs/parse.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_sources/docs/profiles.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_sources/docs/scripts.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_sources/docs/serialize.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_sources/docs/settings.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_sources/docs/stylesheets.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_sources/docs/utilities.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_sources/docs/variables.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_sources/index.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.213070 cssutils-2.7.0/docs/html/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     8269 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_static/basic.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_static/default.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_static/doctools.js
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_static/file.png
+-rw-r--r--   0 runner    (1001) docker     (123)    72174 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_static/jquery.js
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_static/plus.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_static/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (123)    14509 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_static/searchtools.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_static/sidebar.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/_static/underscore.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.213070 cssutils-2.7.0/docs/html/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    10377 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/docs/backlog.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/docs/codec.html
+-rw-r--r--   0 runner    (1001) docker     (123)   167032 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/docs/css.html
+-rw-r--r--   0 runner    (1001) docker     (123)    24168 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/docs/encutils.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/docs/logging.html
+-rw-r--r--   0 runner    (1001) docker     (123)    27207 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/docs/migrate.html
+-rw-r--r--   0 runner    (1001) docker     (123)    28207 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/docs/parse.html
+-rw-r--r--   0 runner    (1001) docker     (123)    22715 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/docs/profiles.html
+-rw-r--r--   0 runner    (1001) docker     (123)    18744 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/docs/scripts.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15756 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/docs/serialize.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/docs/settings.html
+-rw-r--r--   0 runner    (1001) docker     (123)    21169 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/docs/stylesheets.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/docs/utilities.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/docs/variables.html
+-rw-r--r--   0 runner    (1001) docker     (123)    50793 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)    20302 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/py-modindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)    42048 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/html/searchindex.js
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/known issues.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/logging.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/migrate.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/parse.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/profiles.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/scripts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/serialize.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/settings.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/stylesheets.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-09 01:46:33.000000 cssutils-2.7.0/docs/variables.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.217070 cssutils-2.7.0/encutils/
+-rw-r--r--   0 runner    (1001) docker     (123)    21282 2023-06-09 01:46:33.000000 cssutils-2.7.0/encutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.221070 cssutils-2.7.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:33.000000 cssutils-2.7.0/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-09 01:46:33.000000 cssutils-2.7.0/examples/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-09 01:46:33.000000 cssutils-2.7.0/examples/codec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-09 01:46:33.000000 cssutils-2.7.0/examples/cssencodings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-09 01:46:33.000000 cssutils-2.7.0/examples/customlog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-09 01:46:33.000000 cssutils-2.7.0/examples/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-09 01:46:33.000000 cssutils-2.7.0/examples/minify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-09 01:46:33.000000 cssutils-2.7.0/examples/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-09 01:46:33.000000 cssutils-2.7.0/examples/properties_with_same_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-09 01:46:33.000000 cssutils-2.7.0/examples/selectors_tolower.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-09 01:46:33.000000 cssutils-2.7.0/examples/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7237 2023-06-09 01:46:33.000000 cssutils-2.7.0/examples/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-09 01:46:33.000000 cssutils-2.7.0/examples/styledeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-06-09 01:46:33.000000 cssutils-2.7.0/examples/testutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-06-09 01:46:33.000000 cssutils-2.7.0/examples/website.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-09 01:46:33.000000 cssutils-2.7.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-09 01:46:33.000000 cssutils-2.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-09 01:46:33.000000 cssutils-2.7.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-09 01:46:33.000000 cssutils-2.7.0/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-09 01:46:59.229071 cssutils-2.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.225071 cssutils-2.7.0/sheets/
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/096.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/097.css
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/1.css
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/1ascii.css
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/1import.css
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/1inherit-ascii.css
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/1inherit-iso.css
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/1inherit-utf8.css
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/1utf.css
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/2inherit-iso.css
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/2resolve.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/acid2.css
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/all.css
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/atrule.css
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/bad.css
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/basic.css
+-rw-r--r--   0 runner    (1001) docker     (123)   208303 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/bundle.css
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/cases.css
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/csscombine-1.css
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/csscombine-2.css
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/csscombine-proxy.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/cthedot_default.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/default_html4.css
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/hacks.css
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/html.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/html20.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/html40.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.225071 cssutils-2.7.0/sheets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/images/example.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.225071 cssutils-2.7.0/sheets/import/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.225071 cssutils-2.7.0/sheets/import/images2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/import/images2/example2.gif
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/import/import-impossible.css
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/import/import2.css
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/import.css
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/import3.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/ll.css
+-rw-r--r--   0 runner    (1001) docker     (123)    97995 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/ll2.css
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/multiple-values.css
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/page_test.css
+-rw-r--r--   0 runner    (1001) docker     (123)    17998 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/sample_5.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/sample_7.css
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/simple.css
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/single-color.css
+-rw-r--r--   0 runner    (1001) docker     (123)    18645 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/slashcode.css
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/t-HACKS.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/test-unicode.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/test.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8665 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/tigris.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9082 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/tigris2.css
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/u_simple.css
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/v_simple.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.229071 cssutils-2.7.0/sheets/var/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/var/start.css
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/var/use.css
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/var/vars.css
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/var/vars2.css
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/vars.css
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/varsimport.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/xhtml2.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/xhtml22.css
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-09 01:46:33.000000 cssutils-2.7.0/sheets/yuck.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:46:59.229071 cssutils-2.7.0/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-09 01:46:33.000000 cssutils-2.7.0/tools/speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37596 2023-06-09 01:46:33.000000 cssutils-2.7.0/tools/try.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-09 01:46:33.000000 cssutils-2.7.0/tox.ini
```

### Comparing `cssutils-2.6.0/CHANGES.rst` & `cssutils-2.7.0/CHANGES.rst`

 * *Files identical despite different names*

```diff
@@ -1,7 +1,16 @@
+v2.7.0
+======
+
+#35: Updated deprecated usage of ``cgi`` module.
+
+#34: Updated deprecated setup/teardown from ``nose`` in tests.
+
+Other miscellaneous cleanup and packaging updates.
+
 v2.6.0
 ======
 
 #14: Added support for custom CSS variables with ``--`` prefix.
 
 v2.5.1
 ======
```

### Comparing `cssutils-2.6.0/COPYING` & `cssutils-2.7.0/COPYING`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/COPYING.LESSER` & `cssutils-2.7.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/PKG-INFO` & `cssutils-2.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cssutils
-Version: 2.6.0
+Version: 2.7.0
 Summary: A CSS Cascading Style Sheets library for Python
 Home-page: https://github.com/jaraco/cssutils
 Author: Christof Hoeke
 Author-email: c@cthedot.de
 Maintainer: Jason R. Coombs
 Maintainer-email: jaraco@jaraco.com
 Keywords: CSS,Cascading Style Sheets,CSSParser,DOM Level 2 Stylesheets,DOM Level 2 CSS
@@ -19,33 +19,34 @@
 Requires-Python: >=3.7
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: COPYING
 License-File: COPYING.LESSER
 
 .. image:: https://img.shields.io/pypi/v/cssutils.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/cssutils
 
 .. image:: https://img.shields.io/pypi/pyversions/cssutils.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/cssutils
 
 .. image:: https://github.com/jaraco/cssutils/workflows/tests/badge.svg
    :target: https://github.com/jaraco/cssutils/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/cssutils/badge/?version=latest
    :target: https://cssutils.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2022-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
 
 .. image:: https://tidelift.com/badges/package/pypi/cssutils
    :target: https://tidelift.com/subscription/pkg/pypi-cssutils?utm_source=pypi-cssutils&utm_medium=readme
 
 
 Overview
```

### Comparing `cssutils-2.6.0/README.rst` & `cssutils-2.7.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 .. image:: https://img.shields.io/pypi/v/cssutils.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/cssutils
 
 .. image:: https://img.shields.io/pypi/pyversions/cssutils.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/cssutils
 
 .. image:: https://github.com/jaraco/cssutils/workflows/tests/badge.svg
    :target: https://github.com/jaraco/cssutils/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/cssutils/badge/?version=latest
    :target: https://cssutils.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2022-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
 
 .. image:: https://tidelift.com/badges/package/pypi/cssutils
    :target: https://tidelift.com/subscription/pkg/pypi-cssutils?utm_source=pypi-cssutils&utm_medium=readme
 
 
 Overview
```

### Comparing `cssutils-2.6.0/conftest.py` & `cssutils-2.7.0/conftest.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/__init__.py` & `cssutils-2.7.0/cssutils/__init__.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/_fetch.py` & `cssutils-2.7.0/cssutils/_fetch.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/_fetchgae.py` & `cssutils-2.7.0/cssutils/_fetchgae.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/codec.py` & `cssutils-2.7.0/cssutils/codec.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/css/__init__.py` & `cssutils-2.7.0/cssutils/css/__init__.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/css/colors.py` & `cssutils-2.7.0/cssutils/css/colors.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,22 +29,19 @@
     'yellow': (255, 255, 0, 1.0),
     'navy': (0, 0, 128, 1.0),
     'blue': (0, 0, 255, 1.0),
     'teal': (0, 128, 128, 1.0),
     'aqua': (0, 255, 255, 1.0),
     'aliceblue': (240, 248, 255, 1.0),
     'antiquewhite': (250, 235, 215, 1.0),
-    'aqua': (0, 255, 255, 1.0),
     'aquamarine': (127, 255, 212, 1.0),
     'azure': (240, 255, 255, 1.0),
     'beige': (245, 245, 220, 1.0),
     'bisque': (255, 228, 196, 1.0),
-    'black': (0, 0, 0, 1.0),
     'blanchedalmond': (255, 235, 205, 1.0),
-    'blue': (0, 0, 255, 1.0),
     'blueviolet': (138, 43, 226, 1.0),
     'brown': (165, 42, 42, 1.0),
     'burlywood': (222, 184, 135, 1.0),
     'cadetblue': (95, 158, 160, 1.0),
     'chartreuse': (127, 255, 0, 1.0),
     'chocolate': (210, 105, 30, 1.0),
     'coral': (255, 127, 80, 1.0),
@@ -75,21 +72,18 @@
     'deepskyblue': (0, 191, 255, 1.0),
     'dimgray': (105, 105, 105, 1.0),
     'dimgrey': (105, 105, 105, 1.0),
     'dodgerblue': (30, 144, 255, 1.0),
     'firebrick': (178, 34, 34, 1.0),
     'floralwhite': (255, 250, 240, 1.0),
     'forestgreen': (34, 139, 34, 1.0),
-    'fuchsia': (255, 0, 255, 1.0),
     'gainsboro': (220, 220, 220, 1.0),
     'ghostwhite': (248, 248, 255, 1.0),
     'gold': (255, 215, 0, 1.0),
     'goldenrod': (218, 165, 32, 1.0),
-    'gray': (128, 128, 128, 1.0),
-    'green': (0, 128, 0, 1.0),
     'greenyellow': (173, 255, 47, 1.0),
     'grey': (128, 128, 128, 1.0),
     'honeydew': (240, 255, 240, 1.0),
     'hotpink': (255, 105, 180, 1.0),
     'indianred': (205, 92, 92, 1.0),
     'indigo': (75, 0, 130, 1.0),
     'ivory': (255, 255, 240, 1.0),
@@ -109,73 +103,63 @@
     'lightsalmon': (255, 160, 122, 1.0),
     'lightseagreen': (32, 178, 170, 1.0),
     'lightskyblue': (135, 206, 250, 1.0),
     'lightslategray': (119, 136, 153, 1.0),
     'lightslategrey': (119, 136, 153, 1.0),
     'lightsteelblue': (176, 196, 222, 1.0),
     'lightyellow': (255, 255, 224, 1.0),
-    'lime': (0, 255, 0, 1.0),
     'limegreen': (50, 205, 50, 1.0),
     'linen': (250, 240, 230, 1.0),
     'magenta': (255, 0, 255, 1.0),
-    'maroon': (128, 0, 0, 1.0),
     'mediumaquamarine': (102, 205, 170, 1.0),
     'mediumblue': (0, 0, 205, 1.0),
     'mediumorchid': (186, 85, 211, 1.0),
     'mediumpurple': (147, 112, 219, 1.0),
     'mediumseagreen': (60, 179, 113, 1.0),
     'mediumslateblue': (123, 104, 238, 1.0),
     'mediumspringgreen': (0, 250, 154, 1.0),
     'mediumturquoise': (72, 209, 204, 1.0),
     'mediumvioletred': (199, 21, 133, 1.0),
     'midnightblue': (25, 25, 112, 1.0),
     'mintcream': (245, 255, 250, 1.0),
     'mistyrose': (255, 228, 225, 1.0),
     'moccasin': (255, 228, 181, 1.0),
     'navajowhite': (255, 222, 173, 1.0),
-    'navy': (0, 0, 128, 1.0),
     'oldlace': (253, 245, 230, 1.0),
-    'olive': (128, 128, 0, 1.0),
     'olivedrab': (107, 142, 35, 1.0),
     'orange': (255, 165, 0, 1.0),
     'orangered': (255, 69, 0, 1.0),
     'orchid': (218, 112, 214, 1.0),
     'palegoldenrod': (238, 232, 170, 1.0),
     'palegreen': (152, 251, 152, 1.0),
     'paleturquoise': (175, 238, 238, 1.0),
     'palevioletred': (219, 112, 147, 1.0),
     'papayawhip': (255, 239, 213, 1.0),
     'peachpuff': (255, 218, 185, 1.0),
     'peru': (205, 133, 63, 1.0),
     'pink': (255, 192, 203, 1.0),
     'plum': (221, 160, 221, 1.0),
     'powderblue': (176, 224, 230, 1.0),
-    'purple': (128, 0, 128, 1.0),
-    'red': (255, 0, 0, 1.0),
     'rosybrown': (188, 143, 143, 1.0),
     'royalblue': (65, 105, 225, 1.0),
     'saddlebrown': (139, 69, 19, 1.0),
     'salmon': (250, 128, 114, 1.0),
     'sandybrown': (244, 164, 96, 1.0),
     'seagreen': (46, 139, 87, 1.0),
     'seashell': (255, 245, 238, 1.0),
     'sienna': (160, 82, 45, 1.0),
-    'silver': (192, 192, 192, 1.0),
     'skyblue': (135, 206, 235, 1.0),
     'slateblue': (106, 90, 205, 1.0),
     'slategray': (112, 128, 144, 1.0),
     'slategrey': (112, 128, 144, 1.0),
     'snow': (255, 250, 250, 1.0),
     'springgreen': (0, 255, 127, 1.0),
     'steelblue': (70, 130, 180, 1.0),
     'tan': (210, 180, 140, 1.0),
-    'teal': (0, 128, 128, 1.0),
     'thistle': (216, 191, 216, 1.0),
     'tomato': (255, 99, 71, 1.0),
     'turquoise': (64, 224, 208, 1.0),
     'violet': (238, 130, 238, 1.0),
     'wheat': (245, 222, 179, 1.0),
-    'white': (255, 255, 255, 1.0),
     'whitesmoke': (245, 245, 245, 1.0),
-    'yellow': (255, 255, 0, 1.0),
     'yellowgreen': (154, 205, 50, 1.0),
 }
```

### Comparing `cssutils-2.6.0/cssutils/css/csscharsetrule.py` & `cssutils-2.7.0/cssutils/css/csscharsetrule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/css/csscomment.py` & `cssutils-2.7.0/cssutils/css/csscomment.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/css/cssfontfacerule.py` & `cssutils-2.7.0/cssutils/css/cssfontfacerule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/css/cssimportrule.py` & `cssutils-2.7.0/cssutils/css/cssimportrule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/css/cssmediarule.py` & `cssutils-2.7.0/cssutils/css/cssmediarule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/css/cssnamespacerule.py` & `cssutils-2.7.0/cssutils/css/cssnamespacerule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/css/csspagerule.py` & `cssutils-2.7.0/cssutils/css/csspagerule.py`

 * *Files 0% similar despite different names*

```diff
@@ -253,15 +253,14 @@
         cssRules = []
 
         for token in g:
             if (
                 token[0] == 'ATKEYWORD'
                 and self._normalize(token[1]) in MarginRule.margins
             ):
-
                 # MarginRule
                 m = MarginRule(parentRule=self, parentStyleSheet=self.parentStyleSheet)
                 m.cssText = chain([token], g)
 
                 # merge if margin set more than once
                 for r in cssRules:
                     if r.margin == m.margin:
```

### Comparing `cssutils-2.6.0/cssutils/css/cssproperties.py` & `cssutils-2.7.0/cssutils/css/cssproperties.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/css/cssrule.py` & `cssutils-2.7.0/cssutils/css/cssrule.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,14 @@
     """Abstract base interface for rules that contain other rules
     like @media or @page. Methods may be overwritten if a rule
     has specific stuff to do like checking the order of insertion like
     @media does.
     """
 
     def __init__(self, parentRule=None, parentStyleSheet=None):
-
         super().__init__(parentRule=parentRule, parentStyleSheet=parentStyleSheet)
 
         self.cssRules = cssutils.css.CSSRuleList()
 
     def __iter__(self):
         """Generator iterating over these rule's cssRules."""
         yield from self._cssRules
```

### Comparing `cssutils-2.6.0/cssutils/css/cssrulelist.py` & `cssutils-2.7.0/cssutils/css/cssrulelist.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/css/cssstyledeclaration.py` & `cssutils-2.7.0/cssutils/css/cssstyledeclaration.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/css/cssstylerule.py` & `cssutils-2.7.0/cssutils/css/cssstylerule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/css/cssstylesheet.py` & `cssutils-2.7.0/cssutils/css/cssstylesheet.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/css/cssunknownrule.py` & `cssutils-2.7.0/cssutils/css/cssunknownrule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/css/cssvalue.py` & `cssutils-2.7.0/cssutils/css/cssvalue.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/css/cssvariablesdeclaration.py` & `cssutils-2.7.0/cssutils/css/cssvariablesdeclaration.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/css/cssvariablesrule.py` & `cssutils-2.7.0/cssutils/css/cssvariablesrule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/css/marginrule.py` & `cssutils-2.7.0/cssutils/css/marginrule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/css/property.py` & `cssutils-2.7.0/cssutils/css/property.py`

 * *Files 0% similar despite different names*

```diff
@@ -462,15 +462,14 @@
         else:
             if rule is not None:
                 if rule.type == rule.FONT_FACE_RULE:
                     profiles = [cssutils.profile.CSS3_FONT_FACE]
                 # TODO: same for @page
 
         if self.name and self.value:
-
             # TODO
             # cv = self.propertyValue
             # if cv.cssValueType == cv.CSS_VARIABLE and not cv.value:
             #     # TODO: false alarms too!
             #     cssutils.log.warn(u'No value for variable "%s" found, keeping '
             #                       u'variable.' % cv.name, neverraise=True)
```

### Comparing `cssutils-2.6.0/cssutils/css/selector.py` & `cssutils-2.7.0/cssutils/css/selector.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/css/selectorlist.py` & `cssutils-2.7.0/cssutils/css/selectorlist.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/css/value.py` & `cssutils-2.7.0/cssutils/css/value.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/css2productions.py` & `cssutils-2.7.0/cssutils/css2productions.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/cssproductions.py` & `cssutils-2.7.0/cssutils/cssproductions.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/errorhandler.py` & `cssutils-2.7.0/cssutils/errorhandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,14 @@
 
 
 class ErrorHandler(_ErrorHandler):
     "Singleton, see _ErrorHandler"
     instance = None
 
     def __init__(self, log=None, defaultloglevel=logging.INFO, raiseExceptions=True):
-
         if ErrorHandler.instance is None:
             ErrorHandler.instance = _ErrorHandler(
                 log=log,
                 defaultloglevel=defaultloglevel,
                 raiseExceptions=raiseExceptions,
             )
         self.__dict__ = ErrorHandler.instance.__dict__
```

### Comparing `cssutils-2.6.0/cssutils/helper.py` & `cssutils-2.7.0/cssutils/helper.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/parse.py` & `cssutils-2.7.0/cssutils/parse.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/prodparser.py` & `cssutils-2.7.0/cssutils/prodparser.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,14 @@
 
         - next matching Prod or Choice
         - raises ParseError if nothing matches
         - raises Exhausted if sequence already done
         """
         # print u'TEST for %s in %s' % (token, self)
         while self._round < self._max:
-
             # for this round
             i = self._i
             round = self._round
             p = self._prods[i]
             if i == 0:
                 self._roundstarted = False
```

### Comparing `cssutils-2.6.0/cssutils/profiles.py` & `cssutils-2.7.0/cssutils/profiles.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/sac.py` & `cssutils-2.7.0/cssutils/sac.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/script.py` & `cssutils-2.7.0/cssutils/script.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/scripts/csscapture.py` & `cssutils-2.7.0/cssutils/scripts/csscapture.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/scripts/csscombine.py` & `cssutils-2.7.0/cssutils/scripts/csscombine.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/scripts/cssparse.py` & `cssutils-2.7.0/cssutils/scripts/cssparse.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/serialize.py` & `cssutils-2.7.0/cssutils/serialize.py`

 * *Files 0% similar despite different names*

```diff
@@ -1076,15 +1076,14 @@
                     v = self._strip_zeros('%f' % value.value)  # issue #27
                     val = v
                     if value._sign == '-':
                         val = v[0] + v[2:]
                     else:
                         val = v[1:]
                 else:
-
                     val = self._strip_zeros('%f' % value.value)  # issue #27
 
                 # keep '+' if given
                 if value.value != 0 and value._sign == '+':
                     sign = '+'
                 else:
                     sign = ''
```

### Comparing `cssutils-2.6.0/cssutils/settings.py` & `cssutils-2.7.0/cssutils/settings.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/stylesheets/medialist.py` & `cssutils-2.7.0/cssutils/stylesheets/medialist.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/stylesheets/mediaquery.py` & `cssutils-2.7.0/cssutils/stylesheets/mediaquery.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/stylesheets/stylesheet.py` & `cssutils-2.7.0/cssutils/stylesheets/stylesheet.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/stylesheets/stylesheetlist.py` & `cssutils-2.7.0/cssutils/stylesheets/stylesheetlist.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/tests/basetest.py` & `cssutils-2.7.0/cssutils/tests/basetest.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/tests/sheets/096.css` & `cssutils-2.7.0/cssutils/tests/sheets/096.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/tests/sheets/097.css` & `cssutils-2.7.0/cssutils/tests/sheets/097.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/tests/sheets/acid2.css` & `cssutils-2.7.0/cssutils/tests/sheets/acid2.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/tests/sheets/bundle.css` & `cssutils-2.7.0/cssutils/tests/sheets/bundle.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/tests/sheets/cthedot_default.css` & `cssutils-2.7.0/cssutils/tests/sheets/cthedot_default.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/tests/sheets/default_html4.css` & `cssutils-2.7.0/cssutils/tests/sheets/default_html4.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/tests/sheets/hacks.css` & `cssutils-2.7.0/cssutils/tests/sheets/hacks.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/tests/sheets/html20.css` & `cssutils-2.7.0/cssutils/tests/sheets/html20.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/tests/sheets/html40.css` & `cssutils-2.7.0/cssutils/tests/sheets/html40.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/tests/sheets/ll.css` & `cssutils-2.7.0/cssutils/tests/sheets/ll.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/tests/sheets/ll2.css` & `cssutils-2.7.0/cssutils/tests/sheets/ll2.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/tests/sheets/sample_5.css` & `cssutils-2.7.0/cssutils/tests/sheets/sample_5.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/tests/sheets/sample_7.css` & `cssutils-2.7.0/cssutils/tests/sheets/sample_7.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/tests/sheets/slashcode.css` & `cssutils-2.7.0/cssutils/tests/sheets/slashcode.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/tests/sheets/t-HACKS.css` & `cssutils-2.7.0/cssutils/tests/sheets/t-HACKS.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/tests/sheets/test-unicode.css` & `cssutils-2.7.0/cssutils/tests/sheets/test-unicode.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/tests/sheets/test.css` & `cssutils-2.7.0/cssutils/tests/sheets/test.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/tests/sheets/tigris.css` & `cssutils-2.7.0/cssutils/tests/sheets/tigris.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/tests/sheets/tigris2.css` & `cssutils-2.7.0/cssutils/tests/sheets/tigris2.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/tests/sheets/xhtml2.css` & `cssutils-2.7.0/cssutils/tests/sheets/xhtml2.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/tests/sheets/xhtml22.css` & `cssutils-2.7.0/cssutils/tests/sheets/xhtml22.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/tests/test_codec.py` & `cssutils-2.7.0/cssutils/tests/test_codec.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/tests/test_csscharsetrule.py` & `cssutils-2.7.0/cssutils/tests/test_csscharsetrule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/tests/test_csscomment.py` & `cssutils-2.7.0/cssutils/tests/test_csscomment.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/tests/test_cssfontfacerule.py` & `cssutils-2.7.0/cssutils/tests/test_cssfontfacerule.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,15 @@
                 ('x, y', False),
                 ('"x", y', False),
                 ('x, "y"', False),
                 #                            ('"x", "y"', False)
             ]
         }
         for n, t in list(tests.items()):
-            for (v, valid) in t:
+            for v, valid in t:
                 r = cssutils.css.CSSFontFaceRule()
                 r.style[n] = v
                 assert r.style.getProperty(n).parent == r.style
                 assert r.style.getProperty(n).valid == valid
 
     def test_incomplete(self):
         "CSSFontFaceRule (incomplete)"
```

### Comparing `cssutils-2.6.0/cssutils/tests/test_cssimportrule.py` & `cssutils-2.7.0/cssutils/tests/test_cssimportrule.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,14 @@
             # href string
             '''@import "str";''': None,
             '''@import"str";''': '''@import "str";''',
             '''@\\import "str";''': '''@import "str";''',
             '''@IMPORT "str";''': '''@import "str";''',
             '''@import 'str';''': '''@import "str";''',
             '''@import 'str' ;''': '''@import "str";''',
-            '''@import "str";''': None,
             '''@import "str"  ;''': '''@import "str";''',
             r'''@import "\""  ;''': r'''@import "\"";''',
             '''@import '\\'';''': r'''@import "'";''',
             '''@import '"';''': r'''@import "\"";''',
             # href url
             '''@import url(x.css);''': None,
             # nospace
```

### Comparing `cssutils-2.6.0/cssutils/tests/test_cssmediarule.py` & `cssutils-2.7.0/cssutils/tests/test_cssmediarule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/tests/test_cssnamespacerule.py` & `cssutils-2.7.0/cssutils/tests/test_cssnamespacerule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/tests/test_csspagerule.py` & `cssutils-2.7.0/cssutils/tests/test_csspagerule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/tests/test_cssproperties.py` & `cssutils-2.7.0/cssutils/tests/test_cssproperties.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import cssutils.css
 import cssutils.profiles
 import pytest
 
 
 class TestCSSProperties:
-
     #    def test_cssvalues(self):
     #        "cssproperties cssvalues"
     #        # does actually return match object, so a very simplified test...
     #        match = cssutils.css.cssproperties.cssvalues
     #
     #        self.assertEqual(True, bool(match['color']('red')))
     #        self.assertEqual(False, bool(match['top']('red')))
```

### Comparing `cssutils-2.6.0/cssutils/tests/test_cssrule.py` & `cssutils-2.7.0/cssutils/tests/test_cssrule.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     overwrite all tests as you please, use::
 
         super(CLASSNAME, self).test_TESTNAME(params)
 
     to use the base class tests too
     """
 
-    def setup(self):
+    def setup_method(self):
         """
         self.r is the rule
         self.rRO the readonly rule
         relf.r_type the type as defined in CSSRule
         """
         self._setup_rule()
         self.sheet = cssutils.css.CSSStyleSheet()
@@ -31,15 +31,15 @@
     def _setup_rule(self):
         self.r = cssutils.css.CSSRule()
         self.rRO = cssutils.css.CSSRule()
         self.rRO._readonly = True  # must be set here!
         self.r_type = cssutils.css.CSSRule.UNKNOWN_RULE
         self.r_typeString = 'UNKNOWN_RULE'
 
-    def teardown(self):
+    def teardown_method(self):
         cssutils.ser.prefs.useDefaults()
 
     def test_init(self):
         "CSSRule.type and init"
         assert self.r_type == self.r.type
         assert self.r_typeString == self.r.typeString
         assert '' == self.r.cssText
```

### Comparing `cssutils-2.6.0/cssutils/tests/test_cssrulelist.py` & `cssutils-2.7.0/cssutils/tests/test_cssrulelist.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/tests/test_cssstyledeclaration.py` & `cssutils-2.7.0/cssutils/tests/test_cssstyledeclaration.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import xml.dom
 from . import basetest
 import cssutils
 import pytest
 
 
 class TestCSSStyleDeclaration(basetest.BaseTestCase):
-    def setup(self):
+    def setup_method(self):
         self.r = cssutils.css.CSSStyleDeclaration()
 
     def test_init(self):
         "CSSStyleDeclaration.__init__()"
         s = cssutils.css.CSSStyleDeclaration()
         assert '' == s.cssText
         assert 0 == s.length
```

### Comparing `cssutils-2.6.0/cssutils/tests/test_cssstylerule.py` & `cssutils-2.7.0/cssutils/tests/test_cssstylerule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/tests/test_cssstylesheet.py` & `cssutils-2.7.0/cssutils/tests/test_cssstylesheet.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 import xml.dom
 from . import basetest
 import cssutils.css
 import pytest
 
 
 class TestCSSStyleSheet(basetest.BaseTestCase):
-    def setup(self):
+    def setup_method(self):
         self.r = cssutils.css.CSSStyleSheet()  # used by basetest
         self.s = self.r  # used here
         self.rule = cssutils.css.CSSStyleRule()
 
-    def teardown(self):
+    def teardown_method(self):
         cssutils.ser.prefs.useDefaults()
 
     def test_init(self):
         "CSSStyleSheet.__init__()"
         assert 'text/css' == self.s.type
         assert not self.s._readonly
         assert [] == self.s.cssRules
@@ -314,15 +314,15 @@
         s.cssText = css
         assert s.cssText == expcss.encode()
         assert s.namespaces.namespaces == {'': 'default', 'ex2': 'example'}
 
         # __contains__
         assert '' in s.namespaces
         assert 'ex2' in s.namespaces
-        assert not ('NOTSET' in s.namespaces)
+        assert "NOTSET" not in s.namespaces
         # __delitem__
         with pytest.raises(xml.dom.NoModificationAllowedErr):
             s.namespaces.__delitem__('ex2')
         s.namespaces['del'] = 'del'
         del s.namespaces['del']
         with pytest.raises(xml.dom.NamespaceErr):
             s.namespaces.__getitem__('del')
```

### Comparing `cssutils-2.6.0/cssutils/tests/test_cssunknownrule.py` & `cssutils-2.7.0/cssutils/tests/test_cssunknownrule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/tests/test_cssutils.py` & `cssutils-2.7.0/cssutils/tests/test_cssutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 
 @pytest.fixture
 def serializer(monkeypatch):
     monkeypatch.setattr(cssutils, 'ser', cssutils.serialize.CSSSerializer())
 
 
 class TestCSSutils(basetest.BaseTestCase):
-    def setup(self):
+    def setup_method(self):
         cssutils.ser.prefs.useDefaults()
 
-    def teardown(self):
+    def teardown_method(self):
         cssutils.ser.prefs.useDefaults()
 
     exp = '''@import "import/import2.css";
 .import {
     /* ./import.css */
     background-image: url(images/example.gif)
     }'''
```

### Comparing `cssutils-2.6.0/cssutils/tests/test_cssvalue.py` & `cssutils-2.7.0/cssutils/tests/test_cssvalue.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,23 +177,19 @@
             'U+ABCdef': 'u+abcdef',
             # url
             'url(a)': 'url(a)',
             'uRl(a)': 'url(a)',
             'u\\rl(a)': 'url(a)',
             'url("a")': 'url(a)',
             'url(  "a"  )': 'url(a)',
-            'url(a)': 'url(a)',
             'url(";")': 'url(";")',
             'url(",")': 'url(",")',
             'url(")")': 'url(")")',
             '''url("'")''': '''url("'")''',
             '''url('"')''': '''url("\\"")''',
-            '''url("'")''': '''url("'")''',
-            # operator
-            '1': '1',
             '1 2': '1 2',
             '1   2': '1 2',
             '1,2': '1, 2',
             '1,  2': '1, 2',
             '1  ,2': '1, 2',
             '1  ,  2': '1, 2',
             '1/2': '1/2',
```

### Comparing `cssutils-2.6.0/cssutils/tests/test_cssvariablesdeclaration.py` & `cssutils-2.7.0/cssutils/tests/test_cssvariablesdeclaration.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import xml.dom
 
 from . import basetest
 import cssutils
 
 
 class TestCSSVariablesDeclaration(basetest.BaseTestCase):
-    def setup(self):
+    def setup_method(self):
         self.r = cssutils.css.CSSVariablesDeclaration()
         cssutils.ser.prefs.useDefaults()
 
-    def teardown(self):
+    def teardown_method(self):
         cssutils.ser.prefs.useDefaults()
 
     def test_init(self):
         "CSSVariablesDeclaration.__init__()"
         v = cssutils.css.CSSVariablesDeclaration()
         assert '' == v.cssText
         assert 0 == v.length
```

### Comparing `cssutils-2.6.0/cssutils/tests/test_cssvariablesrule.py` & `cssutils-2.7.0/cssutils/tests/test_cssvariablesrule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/tests/test_domimplementation.py` & `cssutils-2.7.0/cssutils/tests/test_domimplementation.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/tests/test_encutils/__init__.py` & `cssutils-2.7.0/cssutils/tests/test_encutils/__init__.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/tests/test_errorhandler.py` & `cssutils-2.7.0/cssutils/tests/test_errorhandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 import xml.dom
 import socket
 
 import cssutils
 
 
 class TestErrorHandler:
-    def setup(self):
+    def setup_method(self):
         "replace default log and ignore its output"
         self._oldlog = cssutils.log._log
         self._saved = cssutils.log.raiseExceptions
 
         cssutils.log.raiseExceptions = False
         cssutils.log.setLog(logging.getLogger('IGNORED-CSSUTILS-TEST'))
 
-    def teardown(self):
+    def teardown_method(self):
         "reset default log"
         cssutils.log.setLog(self._oldlog)
         # for tests only
         cssutils.log.setLevel(logging.FATAL)
         cssutils.log.raiseExceptions = self._saved
 
     def _setHandler(self):
```

### Comparing `cssutils-2.6.0/cssutils/tests/test_helper.py` & `cssutils-2.7.0/cssutils/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/tests/test_marginrule.py` & `cssutils-2.7.0/cssutils/tests/test_marginrule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/tests/test_medialist.py` & `cssutils-2.7.0/cssutils/tests/test_medialist.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import pytest
 
 from . import basetest
 import cssutils.stylesheets
 
 
 class TestMediaList(basetest.BaseTestCase):
-    def setup(self):
+    def setup_method(self):
         self.r = cssutils.stylesheets.MediaList()
 
     def test_set(self):
         "MediaList.mediaText 1"
         ml = cssutils.stylesheets.MediaList()
 
         assert 0 == ml.length
```

### Comparing `cssutils-2.6.0/cssutils/tests/test_mediaquery.py` & `cssutils-2.7.0/cssutils/tests/test_mediaquery.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import xml.dom
 from . import basetest
 import cssutils.stylesheets
 import pytest
 
 
 class TestMediaQuery(basetest.BaseTestCase):
-    def setup(self):
+    def setup_method(self):
         self.r = cssutils.stylesheets.MediaQuery()
 
     def test_mediaText(self):
         "MediaQuery.mediaText"
         tests = {
             'all': None,
             'braille': None,
```

### Comparing `cssutils-2.6.0/cssutils/tests/test_parse.py` & `cssutils-2.7.0/cssutils/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/tests/test_prodparser.py` & `cssutils-2.7.0/cssutils/tests/test_prodparser.py`

 * *Files 0% similar despite different names*

```diff
@@ -345,15 +345,15 @@
         with pytest.raises(Exhausted):
             ch.nextProd(t1)
         ch.reset()
         assert p2 == ch.nextProd(t2)
 
 
 class TestProdParser:
-    def setup(self):
+    def setup_method(self):
         pass
 
     def test_parse_keepS(self):
         "ProdParser.parse(keepS)"
         p = ProdParser()
 
         # text, name, productions, store=None
```

### Comparing `cssutils-2.6.0/cssutils/tests/test_profiles.py` & `cssutils-2.7.0/cssutils/tests/test_profiles.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/tests/test_properties.py` & `cssutils-2.7.0/cssutils/tests/test_properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import cssutils
 from cssutils.css.property import Property
 
 debug = False
 
 
 class TestProperties:
-    def setup(self):
+    def setup_method(self):
         "init test values"
         V = {
             '0': ('0', '-0'),  # , '+0'),
             'NUMBER': ('0', '-0', '100.1', '-100.1'),  # , '+0', '+100.1'),
             'PERCENTAGE': ('0%', '-0%', '100.1%', '-100.1%'),  # , '+0%', '+100.1%'),
             'EM': '1.2em',
             'EX': '1.2ex',
```

### Comparing `cssutils-2.6.0/cssutils/tests/test_property.py` & `cssutils-2.7.0/cssutils/tests/test_property.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from jaraco.test import property_error
 
 from . import basetest
 import cssutils
 
 
 class TestProperty(basetest.BaseTestCase):
-    def setup(self):
+    def setup_method(self):
         self.r = cssutils.css.property.Property('top', '1px')  # , 'important')
 
     def test_init(self):
         "Property.__init__()"
         p = cssutils.css.property.Property('top', '1px')
         assert 'top: 1px' == p.cssText
         assert 'top' == p.literalname
```

### Comparing `cssutils-2.6.0/cssutils/tests/test_scripts_csscombine.py` & `cssutils-2.7.0/cssutils/tests/test_scripts_csscombine.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from cssutils.script import csscombine
 from . import basetest
 import cssutils
 
 
 class CSSCombine:
-
     C = '@namespace s2"uri";s2|sheet-1{top:1px}s2|sheet-2{top:2px}proxy{top:3px}'
 
     def test_combine(self):
         "scripts.csscombine()"
 
         # path, SHOULD be keyword argument!
         csspath = basetest.get_sheet_filename('csscombine-proxy.css')
```

### Comparing `cssutils-2.6.0/cssutils/tests/test_selector.py` & `cssutils-2.7.0/cssutils/tests/test_selector.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from jaraco.test import property_error
 
 from . import basetest
 import cssutils
 
 
 class TestSelector(basetest.BaseTestCase):
-    def setup(self):
+    def setup_method(self):
         self.r = cssutils.css.Selector('*')
 
     def test_init(self):
         "Selector.__init__()"
         s = cssutils.css.Selector('*')
         assert (None, '*') == s.element
         assert {} == s._namespaces.namespaces
@@ -166,21 +166,17 @@
             'a   .b': 'a .b',
             'a * b': None,
             # >
             'a>b': 'a > b',
             'a> b': 'a > b',
             'a >b': 'a > b',
             'a > b': 'a > b',
-            # +
-            'a+b': 'a + b',
             'a+ b': 'a + b',
             'a +b': 'a + b',
             'a + b': 'a + b',
-            # ~
-            'a~b': 'a ~ b',
             'a~ b': 'a ~ b',
             'a ~b': 'a ~ b',
             'a ~ b': 'a ~ b',
             # type selector
             'a': None,
             'h1-a_x__--': None,
             'a-a': None,
@@ -249,15 +245,14 @@
             '''a *[ x ~= a1 ]''': 'a *[x~=a1]',
             '''a[x|=en]''': None,
             '''a[x|= en]''': 'a[x|=en]',
             '''a[x |=en]''': 'a[x|=en]',
             '''a[x |= en]''': 'a[x|=en]',
             '''a[ x |= en]''': 'a[x|=en]',
             '''a[x |= en ]''': 'a[x|=en]',
-            '''a[ x |= en]''': 'a[x|=en]',
             '''a [ x |= en]''': 'a [x|=en]',
             # CSS3
             '''a[x^=en]''': None,
             '''a[x$=en]''': None,
             '''a[x*=en]''': None,
             '''a[/*1*/x/*2*/]''': None,
             '''a[/*1*/x/*2*/=/*3*/a/*4*/]''': None,
@@ -424,16 +419,14 @@
             'a.a': (0, 0, 1, 1),
             '.a.a': (0, 0, 2, 0),  # IE<7 False (0,0,1,0)
             'a.a.a': (0, 0, 2, 1),
             '.a.b': (0, 0, 2, 0),
             'a.a.b': (0, 0, 2, 1),
             '.a .a': (0, 0, 2, 0),
             '*[x]': (0, 0, 1, 0),
-            '*[x]': (0, 0, 1, 0),
-            '*[x]': (0, 0, 1, 0),
             '*[x=a]': (0, 0, 1, 0),
             '*[x~=a]': (0, 0, 1, 0),
             '*[x|=a]': (0, 0, 1, 0),
             '*[x^=a]': (0, 0, 1, 0),
             '*[x*=a]': (0, 0, 1, 0),
             '*[x$=a]': (0, 0, 1, 0),
             '*[x][y]': (0, 0, 2, 0),
```

### Comparing `cssutils-2.6.0/cssutils/tests/test_selectorlist.py` & `cssutils-2.7.0/cssutils/tests/test_selectorlist.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from . import basetest
 import cssutils
 from cssutils.css.selectorlist import SelectorList
 import pytest
 
 
 class TestSelectorList(basetest.BaseTestCase):
-    def setup(self):
+    def setup_method(self):
         self.r = SelectorList()
 
     def test_init(self):
         "SelectorList.__init__() and .length"
         s = SelectorList()
         assert 0 == s.length
```

### Comparing `cssutils-2.6.0/cssutils/tests/test_serialize.py` & `cssutils-2.7.0/cssutils/tests/test_serialize.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 
 class TestPreferences(basetest.BaseTestCase):
     """
     testcases for cssutils.serialize.Preferences
     """
 
-    def setup(self):
+    def setup_method(self):
         cssutils.ser.prefs.useDefaults()
 
-    def teardown(self):
+    def teardown_method(self):
         cssutils.ser.prefs.useDefaults()
 
     #    def testkeepUnkownAtRules(self):
     #        "Preferences.keepUnkownAtRules"
     #        from warnings import catch_warnings
     #        with catch_warnings(record=True) as log:
     #            x = cssutils.ser.prefs.keepUnkownAtRules
@@ -627,18 +627,18 @@
 
 
 class TestCSSSerializer:
     """
     testcases for cssutils.CSSSerializer
     """
 
-    def setup(self):
+    def setup_method(self):
         cssutils.ser.prefs.useDefaults()
 
-    def teardown(self):
+    def teardown_method(self):
         cssutils.ser.prefs.useDefaults()
 
     def test_canonical(self):
         tests = {
             '''1''': '''1''',
             # => remove +
             '''+1''': '''+1''',
@@ -657,15 +657,14 @@
             '''00.0in''': '''0''',
             # 0 => keep unit
             '''00.0%''': '''0%''',
             '''00.0ms''': '''0ms''',
             '''00.0s''': '''0s''',
             '''00.0khz''': '''0khz''',
             '''00.0hz''': '''0hz''',
-            '''00.0khz''': '''0khz''',
             '''00.0deg''': '''0deg''',
             '''00.0rad''': '''0rad''',
             '''00.0grad''': '''0grad''',
             '''00.0xx''': '''0xx''',
             # 11.
             '''a, 'b"', serif''': r'''a, "b\"", serif''',
             # SHOULD: \[ => [ but keep!
```

### Comparing `cssutils-2.6.0/cssutils/tests/test_settings.py` & `cssutils-2.7.0/cssutils/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/tests/test_stylesheet.py` & `cssutils-2.7.0/cssutils/tests/test_stylesheet.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/tests/test_tokenize2.py` & `cssutils-2.7.0/cssutils/tests/test_tokenize2.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import pytest
 
 import cssutils.tokenize2 as tokenize2
 from cssutils.tokenize2 import Tokenizer
 
 
 class TestTokenizer:
-
     testsall = {
         # IDENT
         'äöüß€': [('IDENT', 'äöüß€', 1, 1)],
         ' a ': [('S', ' ', 1, 1), ('IDENT', 'a', 1, 2), ('S', ' ', 1, 3)],
         '_a': [('IDENT', '_a', 1, 1)],
         '-a': [('IDENT', '-a', 1, 1)],
         '--a': [('IDENT', '--a', 1, 1)],
@@ -494,15 +493,15 @@
         'url("a': [('URI', 'url("a")', 1, 1)],
         'url( "a ': [('URI', 'url( "a ")', 1, 1)],
         "url('a": [('URI', "url('a')", 1, 1)],
         'url("a"': [('URI', 'url("a")', 1, 1)],
         "url('a'": [('URI', "url('a')", 1, 1)],
     }
 
-    def setup(self):
+    def setup_method(self):
         # log = cssutils.errorhandler.ErrorHandler()
         self.tokenizer = Tokenizer()
 
     def test_tokenize(self):
         "cssutils Tokenizer().tokenize()"
         import cssutils.cssproductions
```

### Comparing `cssutils-2.6.0/cssutils/tests/test_util.py` & `cssutils-2.7.0/cssutils/tests/test_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Testcases for cssutils.util"""
 
 
-import cgi
+from email.message import Message
 import re
 import urllib.request
 import urllib.error
 import urllib.parse
 from unittest import mock
 
 from cssutils.util import Base, ListSeq, _readUrl, _defaultFetcher, LazyRegex
@@ -27,22 +27,22 @@
         # hack:
         ls.seq.append(1)
         ls.seq.append(2)
 
         # len
         assert 2 == len(ls)
         # __contains__
-        assert True == (1 in ls)
+        assert True is (1 in ls)
         # get
         assert 1 == ls[0]
         assert 2 == ls[1]
         # del
         del ls[0]
         assert 1 == len(ls)
-        assert False == (1 in ls)
+        assert False is (1 in ls)
         # for in
         for x in ls:
             assert 2 == x
 
 
 class BaseTestCase:
     def test_normalize(self):
@@ -380,31 +380,32 @@
 
         class Response:
             """urllib2.Reponse mock"""
 
             def __init__(self, url, contenttype, content, exception=None, args=None):
                 self.url = url
 
-                mt, params = cgi.parse_header(contenttype)
-                self.mimetype = mt
-                self.charset = params.get('charset', None)
+                m = Message()
+                m['content-type'] = contenttype
+
+                self.mimetype = m.get_content_type()
+                self.charset = m.get_param('charset', None)
 
                 self.text = content
 
                 self.exception = exception
                 self.args = args
 
             def geturl(self):
                 return self.url
 
             def info(self):
                 mimetype, charset = self.mimetype, self.charset
 
                 class Info:
-
                     # py2x
                     def gettype(self):
                         return mimetype
 
                     def getparam(self, name=None):
                         return charset
 
@@ -498,15 +499,15 @@
             with pytest.raises(exception):
                 do(url)
 
 
 class TestLazyRegex:
     """Tests for cssutils.util.LazyRegex."""
 
-    def setup(self):
+    def setup_method(self):
         self.lazyre = LazyRegex('f.o')
 
     def test_public_interface(self):
         methods = [
             'search',
             'match',
             'split',
```

### Comparing `cssutils-2.6.0/cssutils/tests/test_value.py` & `cssutils-2.7.0/cssutils/tests/test_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
             # issue #27
             'matrix(0.000092, 0.2500010, -0.250000, 0.000092, 0, 0)': (
                 'matrix(0.000092, 0.250001, -0.25, 0.000092, 0, 0)',
                 1,
                 'matrix(0.000092, 0.250001, -0.25, 0.000092, 0, 0)',
             ),
         }
-        for (cssText, (c, len, v)) in list(tests.items()):
+        for cssText, (c, len, v) in list(tests.items()):
             if c is None:
                 c = cssText
             if v is None:
                 v = c
 
             pv = cssutils.css.PropertyValue(cssText)
             assert c == pv.cssText
@@ -127,15 +127,15 @@
             'f()ident': ('f() ident', 2),
             'f()#123': ('f() #123', 2),
             'f()url()': ('f() url()', 2),
             'f()f()': ('f() f()', 2),
             'url(x.gif)0 0': ('url(x.gif) 0 0', 3),
             'url(x.gif)no-repeat': ('url(x.gif) no-repeat', 2),
         }
-        for (cssText, (c, len)) in list(tests.items()):
+        for cssText, (c, len) in list(tests.items()):
             if c is None:
                 c = cssText
             pv = cssutils.css.PropertyValue(cssText)
             assert c == pv.cssText
             assert len == pv.length
 
         tests = {
@@ -174,21 +174,19 @@
             'U+ABCdef': 'u+abcdef',
             # url
             'url(a)': 'url(a)',
             'uRl(a)': 'url(a)',
             'u\\rl(a)': 'url(a)',
             'url("a")': 'url(a)',
             'url(  "a"  )': 'url(a)',
-            'url(a)': 'url(a)',
             'url(";")': 'url(";")',
             'url(",")': 'url(",")',
             'url(")")': 'url(")")',
             '''url("'")''': '''url("'")''',
             '''url('"')''': '''url("\\"")''',
-            '''url("'")''': '''url("'")''',
             # operator
             '1': '1',
             '1 2': '1 2',
             '1   2': '1 2',
             '1,2': '1, 2',
             '1,  2': '1, 2',
             '1  ,2': '1, 2',
@@ -405,15 +403,15 @@
             '''"x\
 y"''': (
                 '"xy"',
                 'xy',
                 'STRING',
             ),
         }
-        for (p, (r, n, t)) in list(tests.items()):
+        for p, (r, n, t) in list(tests.items()):
             v = cssutils.css.Value(p)
             assert r == v.cssText
             assert t == v.type
             assert n == v.value
 
 
 class ColorValueTestCase:
@@ -439,15 +437,15 @@
             'rgb(-1%,-2%,-3%)': ('rgb(-1%, -2%, -3%)',),
             # rgba
             'rgba(1,2,3, 0)': ('rgba(1, 2, 3, 0)',),
             # hsl
             'hsl(1,2%,3%)': ('hsl(1, 2%, 3%)',),
             'hsla(1,2%,3%, 1.0)': ('hsla(1, 2%, 3%, 1)',),
         }
-        for (p, (r,)) in list(tests.items()):
+        for p, (r,) in list(tests.items()):
             v = cssutils.css.ColorValue(p)
             assert v.COLOR_VALUE == v.type
             assert r == v.cssText
             assert r == v.value
 
             v = cssutils.css.ColorValue()
             v.cssText = p
@@ -561,15 +559,15 @@
             'url(/**/1)': ('url(/**/1)', '/**/1', 'URI'),
             'url(1/**/)': ('url(1/**/)', '1/**/', 'URI'),
             'url(/**/1/**/)': ('url(/**/1/**/)', '/**/1/**/', 'URI'),
             'url(some.gif)': ('url(some.gif)', 'some.gif', 'URI'),
             '  url(some.gif)  ': ('url(some.gif)', 'some.gif', 'URI'),
             'url(   some.gif  )': ('url(some.gif)', 'some.gif', 'URI'),
         }
-        for (p, (r, n, t)) in list(tests.items()):
+        for p, (r, n, t) in list(tests.items()):
             v = cssutils.css.URIValue(p)
             assert r == v.cssText
             assert t == v.type
             assert n == v.value
             assert n == v.uri
 
             v = cssutils.css.URIValue()
@@ -635,15 +633,15 @@
             '0%': ('0%', 0, '%', 'PERCENTAGE'),
             '1%': ('1%', 1, '%', 'PERCENTAGE'),
             '1.1%': ('1.1%', 1.1, '%', 'PERCENTAGE'),
             '-1%': ('-1%', -1, '%', 'PERCENTAGE'),
             '-1.1%': ('-1.1%', -1.1, '%', 'PERCENTAGE'),
             '+1%': ('+1%', 1, '%', 'PERCENTAGE'),
         }
-        for (p, (r, n, d, t)) in list(tests.items()):
+        for p, (r, n, d, t) in list(tests.items()):
             v = cssutils.css.DimensionValue(p)
             assert r == v.cssText
             assert t == v.type
             assert n == v.value
             assert d == v.dimension
 
 
@@ -661,17 +659,16 @@
             'x(x)': ('x(x)', None),
             'X(  X  )': ('x(X)', None),
             'x(1,2)': ('x(1, 2)', None),
             'x(1/**/)': ('x(1 /**/)', 'x(1)'),
             'x(/**/1)': ('x(/**/ 1)', 'x(1)'),
             'x(/**/1/**/)': ('x(/**/ 1 /**/)', 'x(1)'),
             'x(/**/1,x/**/)': ('x(/**/ 1, x /**/)', 'x(1, x)'),
-            'x(1,2)': ('x(1, 2)', None),
         }
-        for (f, (cssText, value)) in list(tests.items()):
+        for f, (cssText, value) in list(tests.items()):
             if value is None:
                 value = cssText
             v = cssutils.css.CSSFunction(f)
             assert cssText == v.cssText
             assert 'FUNCTION' == v.type
             assert value == v.value
 
@@ -701,15 +698,15 @@
             'var(U, url( example.png ) )': (
                 'var(U, url(example.png))',
                 'U',
                 'url(example.png)',
             ),
             'var(C, #f00 )': ('var(C, #f00)', 'C', '#fff'),
         }
-        for (var, (cssText, name, fallback)) in list(tests.items()):
+        for var, (cssText, name, fallback) in list(tests.items()):
             v = cssutils.css.CSSVariable(var)
             assert cssText == v.cssText
             assert 'VARIABLE' == v.type
             assert name == v.name
             # not resolved so it is None
             assert v.value is None
```

### Comparing `cssutils-2.6.0/cssutils/tests/test_x.py` & `cssutils-2.7.0/cssutils/tests/test_x.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils/tokenize2.py` & `cssutils-2.7.0/cssutils/tokenize2.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,14 @@
                 yield ('CHAR', c, line, col)
                 col += 1
                 pos += 1
 
             else:
                 # check all other productions, at least CHAR must match
                 for name, matcher in productions:
-
                     # TODO: USE bad comment?
                     if fullsheet and name == 'CHAR' and has_at(text, pos, '/*'):
                         # before CHAR production test for incomplete comment
                         possiblecomment = '%s*/' % text[pos:]
                         match = self.commentmatcher(possiblecomment)
                         if match and self._doComments:
                             yield ('COMMENT', possiblecomment, line, col)
```

### Comparing `cssutils-2.6.0/cssutils/util.py` & `cssutils-2.7.0/cssutils/util.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/cssutils.egg-info/PKG-INFO` & `cssutils-2.7.0/cssutils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cssutils
-Version: 2.6.0
+Version: 2.7.0
 Summary: A CSS Cascading Style Sheets library for Python
 Home-page: https://github.com/jaraco/cssutils
 Author: Christof Hoeke
 Author-email: c@cthedot.de
 Maintainer: Jason R. Coombs
 Maintainer-email: jaraco@jaraco.com
 Keywords: CSS,Cascading Style Sheets,CSSParser,DOM Level 2 Stylesheets,DOM Level 2 CSS
@@ -19,33 +19,34 @@
 Requires-Python: >=3.7
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: COPYING
 License-File: COPYING.LESSER
 
 .. image:: https://img.shields.io/pypi/v/cssutils.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/cssutils
 
 .. image:: https://img.shields.io/pypi/pyversions/cssutils.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/cssutils
 
 .. image:: https://github.com/jaraco/cssutils/workflows/tests/badge.svg
    :target: https://github.com/jaraco/cssutils/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/cssutils/badge/?version=latest
    :target: https://cssutils.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2022-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
 
 .. image:: https://tidelift.com/badges/package/pypi/cssutils
    :target: https://tidelift.com/subscription/pkg/pypi-cssutils?utm_source=pypi-cssutils&utm_medium=readme
 
 
 Overview
```

### Comparing `cssutils-2.6.0/cssutils.egg-info/SOURCES.txt` & `cssutils-2.7.0/cssutils.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 .coveragerc
 .editorconfig
-.flake8
 .pre-commit-config.yaml
-.readthedocs.yml
+.readthedocs.yaml
 CHANGES.rst
 COPYING
 COPYING.LESSER
 README.rst
 conftest.py
 mypy.ini
 pyproject.toml
 pytest.ini
+ruff.toml
 setup.cfg
 tox.ini
 .github/FUNDING.yml
 .github/dependabot.yml
 .github/workflows/main.yml
 cssutils/__init__.py
 cssutils/_fetch.py
@@ -243,14 +243,15 @@
 docs/html/docs/scripts.html
 docs/html/docs/serialize.html
 docs/html/docs/settings.html
 docs/html/docs/stylesheets.html
 docs/html/docs/utilities.html
 docs/html/docs/variables.html
 encutils/__init__.py
+examples/__init__.py
 examples/build.py
 examples/codec.py
 examples/cssencodings.py
 examples/customlog.py
 examples/imports.py
 examples/minify.py
 examples/parse.py
```

### Comparing `cssutils-2.6.0/docs/backlog.rst` & `cssutils-2.7.0/docs/backlog.rst`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/conf.py` & `cssutils-2.7.0/docs/conf.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,17 @@
-#!/usr/bin/env python3
-extensions = ['sphinx.ext.autodoc', 'jaraco.packaging.sphinx', 'rst.linker']
+extensions = [
+    'sphinx.ext.autodoc',
+    'jaraco.packaging.sphinx',
+]
 
 master_doc = "index"
+html_theme = "furo"
 
+# Link dates and other references in the changelog
+extensions += ['rst.linker']
 link_files = {
     '../CHANGES.rst': dict(
         using=dict(GH='https://github.com'),
         replace=[
             dict(
                 pattern=r'(Issue #|\B#)(?P<issue>\d+)',
                 url='{package_url}/issues/{issue}',
@@ -24,18 +29,21 @@
                 url='https://web.archive.org/web/20200701035501/'
                 'https://bitbucket.org/cthedot/cssutils/issues/{bb_issue}/',
             ),
         ],
     )
 }
 
-# Be strict about any broken references:
+# Be strict about any broken references
 nitpicky = True
 
 # Include Python intersphinx mapping to prevent failures
 # jaraco/skeleton#51
 extensions += ['sphinx.ext.intersphinx']
 intersphinx_mapping = {
     'python': ('https://docs.python.org/3', None),
 }
 
+# Preserve authored syntax for defaults
+autodoc_preserve_defaults = True
+
 extensions += ['jaraco.tidelift']
```

### Comparing `cssutils-2.6.0/docs/css.rst` & `cssutils-2.7.0/docs/css.rst`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/CHANGELOG.html` & `cssutils-2.7.0/docs/html/CHANGELOG.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/README.html` & `cssutils-2.7.0/docs/html/README.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/_2to3 py3.html` & `cssutils-2.7.0/docs/html/_2to3 py3.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/_sources/CHANGELOG.txt` & `cssutils-2.7.0/docs/html/_sources/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/_sources/README.txt` & `cssutils-2.7.0/docs/html/_sources/README.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/_sources/docs/backlog.txt` & `cssutils-2.7.0/docs/html/_sources/docs/backlog.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/_sources/docs/css.txt` & `cssutils-2.7.0/docs/html/_sources/docs/css.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/_sources/docs/cssstyledeclaration.txt` & `cssutils-2.7.0/docs/html/_sources/docs/cssstyledeclaration.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/_sources/docs/implementation.txt` & `cssutils-2.7.0/docs/html/_sources/docs/implementation.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/_sources/docs/logging.txt` & `cssutils-2.7.0/docs/html/_sources/docs/logging.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/_sources/docs/migrate.txt` & `cssutils-2.7.0/docs/html/_sources/docs/migrate.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/_sources/docs/parse.txt` & `cssutils-2.7.0/docs/html/_sources/docs/parse.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/_sources/docs/profiles.txt` & `cssutils-2.7.0/docs/html/_sources/docs/profiles.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/_sources/docs/scripts.txt` & `cssutils-2.7.0/docs/html/_sources/docs/scripts.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/_sources/docs/serialize.txt` & `cssutils-2.7.0/docs/html/_sources/docs/serialize.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/_sources/docs/settings.txt` & `cssutils-2.7.0/docs/html/_sources/docs/settings.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/_sources/docs/stylesheets.txt` & `cssutils-2.7.0/docs/html/_sources/docs/stylesheets.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/_sources/index.txt` & `cssutils-2.7.0/docs/html/_sources/index.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/_static/basic.css` & `cssutils-2.7.0/docs/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/_static/default.css` & `cssutils-2.7.0/docs/html/_static/default.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/_static/doctools.js` & `cssutils-2.7.0/docs/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/_static/jquery.js` & `cssutils-2.7.0/docs/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/_static/pygments.css` & `cssutils-2.7.0/docs/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/_static/searchtools.js` & `cssutils-2.7.0/docs/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/_static/sidebar.js` & `cssutils-2.7.0/docs/html/_static/sidebar.js`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/_static/underscore.js` & `cssutils-2.7.0/docs/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/docs/backlog.html` & `cssutils-2.7.0/docs/html/docs/backlog.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/docs/codec.html` & `cssutils-2.7.0/docs/html/docs/codec.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/docs/css.html` & `cssutils-2.7.0/docs/html/docs/css.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/docs/encutils.html` & `cssutils-2.7.0/docs/html/docs/encutils.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/docs/logging.html` & `cssutils-2.7.0/docs/html/docs/logging.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/docs/migrate.html` & `cssutils-2.7.0/docs/html/docs/migrate.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/docs/parse.html` & `cssutils-2.7.0/docs/html/docs/parse.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/docs/profiles.html` & `cssutils-2.7.0/docs/html/docs/profiles.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/docs/scripts.html` & `cssutils-2.7.0/docs/html/docs/scripts.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/docs/serialize.html` & `cssutils-2.7.0/docs/html/docs/serialize.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/docs/settings.html` & `cssutils-2.7.0/docs/html/docs/settings.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/docs/stylesheets.html` & `cssutils-2.7.0/docs/html/docs/stylesheets.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/docs/utilities.html` & `cssutils-2.7.0/docs/html/docs/utilities.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/docs/variables.html` & `cssutils-2.7.0/docs/html/docs/variables.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/genindex.html` & `cssutils-2.7.0/docs/html/genindex.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/index.html` & `cssutils-2.7.0/docs/html/index.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/py-modindex.html` & `cssutils-2.7.0/docs/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/search.html` & `cssutils-2.7.0/docs/html/search.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/html/searchindex.js` & `cssutils-2.7.0/docs/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/index.rst` & `cssutils-2.7.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/known issues.rst` & `cssutils-2.7.0/docs/known issues.rst`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/logging.rst` & `cssutils-2.7.0/docs/logging.rst`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/migrate.rst` & `cssutils-2.7.0/docs/migrate.rst`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/parse.rst` & `cssutils-2.7.0/docs/parse.rst`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/profiles.rst` & `cssutils-2.7.0/docs/profiles.rst`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/scripts.rst` & `cssutils-2.7.0/docs/scripts.rst`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/serialize.rst` & `cssutils-2.7.0/docs/serialize.rst`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/settings.rst` & `cssutils-2.7.0/docs/settings.rst`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/docs/stylesheets.rst` & `cssutils-2.7.0/docs/stylesheets.rst`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/encutils/__init__.py` & `cssutils-2.7.0/encutils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,17 +46,17 @@
     'getMetaInfo',
     'detectXMLEncoding',
     'getEncodingInfo',
     'tryEncodings',
     'EncodingInfo',
 ]
 
+from email.message import Message
 import html.parser
 import io
-import cgi
 import re
 import sys
 import urllib.request
 import urllib.parse
 import urllib.error
 
 
@@ -311,16 +311,19 @@
 
     try:
         p.feed(text)
     except html.parser.HTMLParseError:
         pass
 
     if p.content_type:
-        media_type, params = cgi.parse_header(p.content_type)
-        encoding = params.get('charset')  # defaults to None
+        m = Message()
+        m['content-type'] = p.content_type
+
+        media_type = m.get_content_type()
+        encoding = m.get_param('charset')  # defaults to None
         if encoding:
             encoding = encoding.lower()
         if log:
             log.info('HTML META media_type: %s', media_type)
             log.info('HTML META encoding: %s', encoding)
     else:
         media_type = encoding = None
```

### Comparing `cssutils-2.6.0/examples/build.py` & `cssutils-2.7.0/examples/build.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/examples/cssencodings.py` & `cssutils-2.7.0/examples/cssencodings.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/examples/customlog.py` & `cssutils-2.7.0/examples/customlog.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/examples/imports.py` & `cssutils-2.7.0/examples/imports.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/examples/minify.py` & `cssutils-2.7.0/examples/minify.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/examples/parse.py` & `cssutils-2.7.0/examples/parse.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import xml.dom
 
 EXPOUT = '''\n--- source CSS ---\n/* This is a comment */\n    body {\n        background: white;\n        top: red;\n        x: 1;\n        }\n    a { y }\n            \n\n--- simple parsing ---\n/* This is a comment */\nbody {\n    background: white;\n    top: red;\n    x: 1\n    }\n\n--- CSSParser(raiseExceptions=True) ---\n:::RAISED::: Property: No ":" after name found: y  [7:10:  ]\n'''
 EXPERR = 'Property: Invalid value for "CSS Level 2.1" property: red [4:9: top]\nProperty: Unknown Property name. [5:9: x]\nProperty: No ":" after name found: y  [7:10:  ]\nProperty: No property value found: y  [7:10:  ]\nCSSStyleDeclaration: Syntax Error in Property: y \nProperty: Invalid value for "CSS Level 2.1" property: red [4:9: top]\nProperty: Unknown Property name. [5:9: x]\n'
 
 
 def main():
-
     css = '''/* This is a comment */
     body {
         background: white;
         top: red;
         x: 1;
         }
     a { y }
```

### Comparing `cssutils-2.6.0/examples/properties_with_same_name.py` & `cssutils-2.7.0/examples/properties_with_same_name.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/examples/selectors_tolower.py` & `cssutils-2.7.0/examples/selectors_tolower.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/examples/serialize.py` & `cssutils-2.7.0/examples/serialize.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/examples/style.py` & `cssutils-2.7.0/examples/style.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/examples/styledeclaration.py` & `cssutils-2.7.0/examples/styledeclaration.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/examples/testutil.py` & `cssutils-2.7.0/examples/testutil.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/examples/website.py` & `cssutils-2.7.0/examples/website.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         color: red
         }
     >>> # returns if new Medium is wellformed and has been added
     >>> sheet.cssRules[0].media.appendMedium('print')
     True
     >>> # returns the new Selector:
     >>> sheet.cssRules[1].selectorList.appendSelector('a')
-    cssutils.css.Selector(selectorText=u'a')
+    cssutils.css.Selector(selectorText='a')
     >>> print(sheet.cssText.decode())
     @import url(example.css) tv, print;
     body, a {
         color: red
         }
     """
 
@@ -135,15 +135,15 @@
     >>> style = cssutils.css.CSSStyleDeclaration(cssText=cssText)
     >>> print(style.cssText)
     background: white url(paper.png) scroll;
     background: white url(ledger.png) fixed;
     >>> # work with properties:
     >>> proplist = style.getProperties('background', all=True)
     >>> proplist
-    [cssutils.css.Property(name='background', value=u'white url(paper.png) scroll', priority=u''), cssutils.css.Property(name='background', value=u'white url(ledger.png) fixed', priority=u'')]
+    [cssutils.css.Property(name='background', value='white url(paper.png) scroll', priority=''), cssutils.css.Property(name='background', value='white url(ledger.png) fixed', priority='')]
     >>> for prop in proplist: print(prop.value)
     white url(paper.png) scroll
     white url(ledger.png) fixed
     >>> # overwrite the current property, to overwrite all iterate over proplist
     >>> style['background'] = ('red', '!important')
     >>> # importance in DOM ist 'important' but '!important' works too
     >>> print(style['background'], style.getPropertyPriority('background'))
```

### Comparing `cssutils-2.6.0/setup.cfg` & `cssutils-2.7.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -35,32 +35,34 @@
 	sheets*
 	tools*
 
 [options.extras_require]
 testing = 
 	pytest >= 6
 	pytest-checkdocs >= 2.4
-	pytest-flake8
-	flake8 < 5
 	pytest-black >= 0.3.7; \
 	python_implementation != "PyPy"
 	pytest-cov
 	pytest-mypy >= 0.9.1; \
 	python_implementation != "PyPy"
 	pytest-enabler >= 1.3
+	pytest-ruff
 	
 	lxml; \
 	python_version < "3.11"
 	cssselect
 	importlib_resources; python_version < "3.9"
 	jaraco.test >= 5.1
 docs = 
-	sphinx
+	sphinx >= 3.5
 	jaraco.packaging >= 9
 	rst.linker >= 1.9
+	furo
+	sphinx-lint
+	
 	jaraco.tidelift >= 1.4
 
 [options.entry_points]
 console_scripts = 
 	csscapture = cssutils.scripts.csscapture:main
 	csscombine = cssutils.scripts.csscombine:main
 	cssparse = cssutils.scripts.cssparse:main
```

### Comparing `cssutils-2.6.0/sheets/096.css` & `cssutils-2.7.0/sheets/096.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/sheets/097.css` & `cssutils-2.7.0/sheets/097.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/sheets/acid2.css` & `cssutils-2.7.0/sheets/acid2.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/sheets/bundle.css` & `cssutils-2.7.0/sheets/bundle.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/sheets/cthedot_default.css` & `cssutils-2.7.0/sheets/cthedot_default.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/sheets/default_html4.css` & `cssutils-2.7.0/sheets/default_html4.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/sheets/hacks.css` & `cssutils-2.7.0/sheets/hacks.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/sheets/html20.css` & `cssutils-2.7.0/sheets/html20.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/sheets/html40.css` & `cssutils-2.7.0/sheets/html40.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/sheets/ll.css` & `cssutils-2.7.0/sheets/ll.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/sheets/ll2.css` & `cssutils-2.7.0/sheets/ll2.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/sheets/sample_5.css` & `cssutils-2.7.0/sheets/sample_5.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/sheets/sample_7.css` & `cssutils-2.7.0/sheets/sample_7.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/sheets/slashcode.css` & `cssutils-2.7.0/sheets/slashcode.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/sheets/t-HACKS.css` & `cssutils-2.7.0/sheets/t-HACKS.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/sheets/test-unicode.css` & `cssutils-2.7.0/sheets/test-unicode.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/sheets/test.css` & `cssutils-2.7.0/sheets/test.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/sheets/tigris.css` & `cssutils-2.7.0/sheets/tigris.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/sheets/tigris2.css` & `cssutils-2.7.0/sheets/tigris2.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/sheets/xhtml2.css` & `cssutils-2.7.0/sheets/xhtml2.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/sheets/xhtml22.css` & `cssutils-2.7.0/sheets/xhtml22.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/tools/speed.py` & `cssutils-2.7.0/tools/speed.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/tools/try.py` & `cssutils-2.7.0/tools/try.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.6.0/tox.ini` & `cssutils-2.7.0/tox.ini`

 * *Files 24% similar despite different names*

```diff
@@ -4,26 +4,30 @@
 # https://github.com/jaraco/skeleton/issues/6
 tox_pip_extensions_ext_venv_update = true
 toxworkdir={env:TOX_WORK_DIR:.tox}
 
 
 [testenv]
 deps =
+setenv =
+	PYTHONWARNDEFAULTENCODING = 1
 commands =
 	pytest {posargs}
 usedevelop = True
-extras = testing
+extras =
+	testing
 
 [testenv:docs]
 extras =
 	docs
 	testing
 changedir = docs
 commands =
 	python -m sphinx -W --keep-going . {toxinidir}/build/html
+	python -m sphinxlint
 
 [testenv:release]
 skip_install = True
 deps =
 	build
 	twine>=3
 	jaraco.develop>=7.1
```

