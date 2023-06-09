# Comparing `tmp/no_vtf-2.0.1.tar.gz` & `tmp/no_vtf-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "no_vtf-2.0.1.tar", last modified: Sat Apr 16 18:52:44 2022, max compression
+gzip compressed data, was "no_vtf-3.0.0.tar", last modified: Fri Jun  9 18:24:31 2023, max compression
```

## Comparing `no_vtf-2.0.1.tar` & `no_vtf-3.0.0.tar`

### file list

```diff
@@ -1,106 +1,117 @@
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2022-04-16 18:52:44.885978 no_vtf-2.0.1/
--rw-r--r--   0 build     (1000) build     (1000)     1719 2022-04-16 18:43:00.000000 no_vtf-2.0.1/.build.yml
--rw-r--r--   0 build     (1000) build     (1000)      201 2022-04-16 18:43:00.000000 no_vtf-2.0.1/.gitignore
--rw-r--r--   0 build     (1000) build     (1000)      137 2022-04-16 18:43:00.000000 no_vtf-2.0.1/LICENSE.md
--rw-r--r--   0 build     (1000) build     (1000)       29 2022-04-16 18:43:00.000000 no_vtf-2.0.1/MANIFEST.in
--rw-r--r--   0 build     (1000) build     (1000)     6220 2022-04-16 18:52:44.885978 no_vtf-2.0.1/PKG-INFO
--rw-r--r--   0 build     (1000) build     (1000)     5241 2022-04-16 18:43:00.000000 no_vtf-2.0.1/README.md
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2022-04-16 18:52:44.877978 no_vtf-2.0.1/builds/
--rw-r--r--   0 build     (1000) build     (1000)      787 2022-04-16 18:43:00.000000 no_vtf-2.0.1/builds/common
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2022-04-16 18:52:44.877978 no_vtf-2.0.1/builds/debian/
--rw-r--r--   0 build     (1000) build     (1000)      129 2022-04-16 18:43:00.000000 no_vtf-2.0.1/builds/debian/common
--rwxr-xr-x   0 build     (1000) build     (1000)      368 2022-04-16 18:43:00.000000 no_vtf-2.0.1/builds/debian/env.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      368 2022-04-16 18:43:00.000000 no_vtf-2.0.1/builds/debian/ksc-install.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      475 2022-04-16 18:43:00.000000 no_vtf-2.0.1/builds/debian/python3.10-build_dep.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      820 2022-04-16 18:43:00.000000 no_vtf-2.0.1/builds/debian/wine-install.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      147 2022-04-16 18:43:00.000000 no_vtf-2.0.1/builds/diff_generated.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      155 2022-04-16 18:43:00.000000 no_vtf-2.0.1/builds/nox.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      165 2022-04-16 18:43:00.000000 no_vtf-2.0.1/builds/nox_wine.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      433 2022-04-16 18:43:00.000000 no_vtf-2.0.1/builds/python3.10-install.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      330 2022-04-16 18:43:00.000000 no_vtf-2.0.1/builds/verify_signatures.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      231 2022-04-16 18:43:00.000000 no_vtf-2.0.1/builds/with_clone.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      939 2022-04-16 18:43:00.000000 no_vtf-2.0.1/builds/with_wine.sh
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2022-04-16 18:52:44.877978 no_vtf-2.0.1/ksy/
--rwxr-xr-x   0 build     (1000) build     (1000)      173 2022-04-16 18:43:00.000000 no_vtf-2.0.1/ksy/compile.sh
--rw-r--r--   0 build     (1000) build     (1000)    10310 2022-04-16 18:43:00.000000 no_vtf-2.0.1/ksy/vtf.ksy
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2022-04-16 18:52:44.881978 no_vtf-2.0.1/no_vtf/
--rw-r--r--   0 build     (1000) build     (1000)      296 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)      206 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/__main__.py
--rw-r--r--   0 build     (1000) build     (1000)      142 2022-04-16 18:52:43.000000 no_vtf-2.0.1/no_vtf/_version.py
--rw-r--r--   0 build     (1000) build     (1000)     2048 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/channel_separator.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2022-04-16 18:52:44.881978 no_vtf-2.0.1/no_vtf/decoder/
--rw-r--r--   0 build     (1000) build     (1000)        0 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/decoder/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)      510 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/decoder/image.py
--rw-r--r--   0 build     (1000) build     (1000)      466 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/decoder/texture.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2022-04-16 18:52:44.881978 no_vtf-2.0.1/no_vtf/decoders/
--rw-r--r--   0 build     (1000) build     (1000)        0 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/decoders/__init__.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2022-04-16 18:52:44.881978 no_vtf-2.0.1/no_vtf/decoders/image/
--rw-r--r--   0 build     (1000) build     (1000)        0 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/decoders/image/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)     7057 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/decoders/image/generic.py
--rw-r--r--   0 build     (1000) build     (1000)     2584 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/decoders/image/vtf.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2022-04-16 18:52:44.881978 no_vtf-2.0.1/no_vtf/decoders/texture/
--rw-r--r--   0 build     (1000) build     (1000)        0 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/decoders/texture/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)     4122 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/decoders/texture/vtf.py
--rw-r--r--   0 build     (1000) build     (1000)     1206 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/deferrable.py
--rw-r--r--   0 build     (1000) build     (1000)      422 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/extractor.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2022-04-16 18:52:44.885978 no_vtf-2.0.1/no_vtf/extractors/
--rw-r--r--   0 build     (1000) build     (1000)        0 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/extractors/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)     3227 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/extractors/vtf.py
--rw-r--r--   0 build     (1000) build     (1000)      780 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/file.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2022-04-16 18:52:44.885978 no_vtf-2.0.1/no_vtf/files/
--rw-r--r--   0 build     (1000) build     (1000)        0 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/files/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)     2819 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/files/vtf.py
--rw-r--r--   0 build     (1000) build     (1000)     2306 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/filesystem.py
--rw-r--r--   0 build     (1000) build     (1000)      636 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/filter.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2022-04-16 18:52:44.885978 no_vtf-2.0.1/no_vtf/filters/
--rw-r--r--   0 build     (1000) build     (1000)        0 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/filters/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)      464 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/filters/vtf.py
--rw-r--r--   0 build     (1000) build     (1000)     1502 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/image.py
--rw-r--r--   0 build     (1000) build     (1000)      518 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/io.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2022-04-16 18:52:44.885978 no_vtf-2.0.1/no_vtf/ios/
--rw-r--r--   0 build     (1000) build     (1000)        0 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/ios/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)      684 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/ios/bytes_io.py
--rw-r--r--   0 build     (1000) build     (1000)     7214 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/ios/imageio.py
--rw-r--r--   0 build     (1000) build     (1000)     9221 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/main.py
--rw-r--r--   0 build     (1000) build     (1000)      408 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/namer.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2022-04-16 18:52:44.885978 no_vtf-2.0.1/no_vtf/namers/
--rw-r--r--   0 build     (1000) build     (1000)        0 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/namers/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)      856 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/namers/vtf.py
--rw-r--r--   0 build     (1000) build     (1000)      928 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/ndarray.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2022-04-16 18:52:44.885978 no_vtf-2.0.1/no_vtf/parsers/
--rw-r--r--   0 build     (1000) build     (1000)        0 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/parsers/__init__.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2022-04-16 18:52:44.885978 no_vtf-2.0.1/no_vtf/parsers/generated/
--rw-r--r--   0 build     (1000) build     (1000)        0 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/parsers/generated/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)    27130 2022-04-16 18:52:22.000000 no_vtf-2.0.1/no_vtf/parsers/generated/vtf.py
--rw-r--r--   0 build     (1000) build     (1000)     3258 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/pipeline.py
--rw-r--r--   0 build     (1000) build     (1000)      798 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/pipeline_runner.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2022-04-16 18:52:44.885978 no_vtf-2.0.1/no_vtf/pipeline_runners/
--rw-r--r--   0 build     (1000) build     (1000)        0 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/pipeline_runners/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)     1098 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/pipeline_runners/parallel_runner.py
--rw-r--r--   0 build     (1000) build     (1000)      892 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/pipeline_runners/sequential_runner.py
--rw-r--r--   0 build     (1000) build     (1000)     1029 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/postprocessor.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2022-04-16 18:52:44.885978 no_vtf-2.0.1/no_vtf/postprocessors/
--rw-r--r--   0 build     (1000) build     (1000)        0 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/postprocessors/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)     1646 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/postprocessors/fp_precision_modifier.py
--rw-r--r--   0 build     (1000) build     (1000)        0 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/py.typed
--rw-r--r--   0 build     (1000) build     (1000)      320 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/texture.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2022-04-16 18:52:44.885978 no_vtf-2.0.1/no_vtf/textures/
--rw-r--r--   0 build     (1000) build     (1000)        0 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/textures/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)      765 2022-04-16 18:43:00.000000 no_vtf-2.0.1/no_vtf/textures/vtf.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2022-04-16 18:52:44.881978 no_vtf-2.0.1/no_vtf.egg-info/
--rw-r--r--   0 build     (1000) build     (1000)     6220 2022-04-16 18:52:43.000000 no_vtf-2.0.1/no_vtf.egg-info/PKG-INFO
--rw-r--r--   0 build     (1000) build     (1000)     1980 2022-04-16 18:52:44.000000 no_vtf-2.0.1/no_vtf.egg-info/SOURCES.txt
--rw-r--r--   0 build     (1000) build     (1000)        1 2022-04-16 18:52:43.000000 no_vtf-2.0.1/no_vtf.egg-info/dependency_links.txt
--rw-r--r--   0 build     (1000) build     (1000)       44 2022-04-16 18:52:44.000000 no_vtf-2.0.1/no_vtf.egg-info/entry_points.txt
--rw-r--r--   0 build     (1000) build     (1000)        1 2022-04-16 18:51:39.000000 no_vtf-2.0.1/no_vtf.egg-info/not-zip-safe
--rw-r--r--   0 build     (1000) build     (1000)      150 2022-04-16 18:52:44.000000 no_vtf-2.0.1/no_vtf.egg-info/requires.txt
--rw-r--r--   0 build     (1000) build     (1000)        7 2022-04-16 18:52:44.000000 no_vtf-2.0.1/no_vtf.egg-info/top_level.txt
--rw-r--r--   0 build     (1000) build     (1000)    10036 2022-04-16 18:43:00.000000 no_vtf-2.0.1/noxfile.py
--rw-r--r--   0 build     (1000) build     (1000)      394 2022-04-16 18:43:00.000000 no_vtf-2.0.1/pyproject.toml
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2022-04-16 18:52:44.873978 no_vtf-2.0.1/resources/
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2022-04-16 18:52:44.885978 no_vtf-2.0.1/resources/docs/
--rw-r--r--   0 build     (1000) build     (1000)   123671 2022-04-16 18:43:00.000000 no_vtf-2.0.1/resources/docs/screencast.gif
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2022-04-16 18:52:44.885978 no_vtf-2.0.1/resources/pyinstaller/
--rw-r--r--   0 build     (1000) build     (1000)        6 2022-04-16 18:43:00.000000 no_vtf-2.0.1/resources/pyinstaller/empty.ico
--rwxr-xr-x   0 build     (1000) build     (1000)      276 2022-04-16 18:43:00.000000 no_vtf-2.0.1/resources/pyinstaller/no_vtf.desktop
--rw-r--r--   0 build     (1000) build     (1000)     2373 2022-04-16 18:52:44.889978 no_vtf-2.0.1/setup.cfg
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.554766 no_vtf-3.0.0/
+-rw-r--r--   0 build     (1000) build     (1000)     1726 2023-06-09 18:14:25.000000 no_vtf-3.0.0/.build.yml
+-rw-r--r--   0 build     (1000) build     (1000)      336 2023-06-09 18:14:25.000000 no_vtf-3.0.0/.gitignore
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.534767 no_vtf-3.0.0/.reuse/
+-rw-r--r--   0 build     (1000) build     (1000)      189 2023-06-09 18:14:25.000000 no_vtf-3.0.0/.reuse/dep5
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.538767 no_vtf-3.0.0/LICENSES/
+-rw-r--r--   0 build     (1000) build     (1000)    17023 2023-06-09 18:14:25.000000 no_vtf-3.0.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 build     (1000) build     (1000)     7048 2023-06-09 18:14:25.000000 no_vtf-3.0.0/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 build     (1000) build     (1000)    34670 2023-06-09 18:14:25.000000 no_vtf-3.0.0/LICENSES/GPL-3.0-or-later.txt
+-rw-r--r--   0 build     (1000) build     (1000)    42098 2023-06-09 18:14:25.000000 no_vtf-3.0.0/LICENSES/LGPL-3.0-or-later.txt
+-rw-r--r--   0 build     (1000) build     (1000)      138 2023-06-09 18:14:25.000000 no_vtf-3.0.0/MANIFEST.in
+-rw-r--r--   0 build     (1000) build     (1000)     9026 2023-06-09 18:24:31.554766 no_vtf-3.0.0/PKG-INFO
+-rw-r--r--   0 build     (1000) build     (1000)     7738 2023-06-09 18:14:25.000000 no_vtf-3.0.0/README.md
+-rw-r--r--   0 build     (1000) build     (1000)       95 2023-06-09 18:14:25.000000 no_vtf-3.0.0/README.md.license
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.538767 no_vtf-3.0.0/builds/
+-rw-r--r--   0 build     (1000) build     (1000)      820 2023-06-09 18:14:25.000000 no_vtf-3.0.0/builds/common
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.538767 no_vtf-3.0.0/builds/debian/
+-rw-r--r--   0 build     (1000) build     (1000)      162 2023-06-09 18:14:25.000000 no_vtf-3.0.0/builds/debian/common
+-rwxr-xr-x   0 build     (1000) build     (1000)      401 2023-06-09 18:14:25.000000 no_vtf-3.0.0/builds/debian/env.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      404 2023-06-09 18:14:25.000000 no_vtf-3.0.0/builds/debian/ksc-install.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      508 2023-06-09 18:14:25.000000 no_vtf-3.0.0/builds/debian/python3.10-build_dep.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      855 2023-06-09 18:14:25.000000 no_vtf-3.0.0/builds/debian/wine-install.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      180 2023-06-09 18:14:25.000000 no_vtf-3.0.0/builds/diff_generated.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      188 2023-06-09 18:14:25.000000 no_vtf-3.0.0/builds/nox.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      198 2023-06-09 18:14:25.000000 no_vtf-3.0.0/builds/nox_wine.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      466 2023-06-09 18:14:25.000000 no_vtf-3.0.0/builds/python3.10-install.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      363 2023-06-09 18:14:25.000000 no_vtf-3.0.0/builds/verify_signatures.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      264 2023-06-09 18:14:25.000000 no_vtf-3.0.0/builds/with_clone.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      989 2023-06-09 18:14:25.000000 no_vtf-3.0.0/builds/with_wine.sh
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.538767 no_vtf-3.0.0/ksy/
+-rwxr-xr-x   0 build     (1000) build     (1000)      205 2023-06-09 18:14:25.000000 no_vtf-3.0.0/ksy/compile.sh
+-rw-r--r--   0 build     (1000) build     (1000)    10409 2023-06-09 18:14:25.000000 no_vtf-3.0.0/ksy/vtf.ksy
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.542766 no_vtf-3.0.0/no_vtf/
+-rw-r--r--   0 build     (1000) build     (1000)      329 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)      300 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/__main__.py
+-rw-r--r--   0 build     (1000) build     (1000)      160 2023-06-09 18:24:31.000000 no_vtf-3.0.0/no_vtf/_version.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.542766 no_vtf-3.0.0/no_vtf/deferred/
+-rw-r--r--   0 build     (1000) build     (1000)      186 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/deferred/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)     1471 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/deferred/deferred.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.542766 no_vtf-3.0.0/no_vtf/filesystem/
+-rw-r--r--   0 build     (1000) build     (1000)      287 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/filesystem/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)     2023 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/filesystem/input_paths.py
+-rw-r--r--   0 build     (1000) build     (1000)      895 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/filesystem/output_directories.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.546766 no_vtf-3.0.0/no_vtf/image/
+-rw-r--r--   0 build     (1000) build     (1000)      441 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/image/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)     1667 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/image/channel_separator.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.546766 no_vtf-3.0.0/no_vtf/image/decoder/
+-rw-r--r--   0 build     (1000) build     (1000)      198 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/image/decoder/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)      486 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/image/decoder/decoder.py
+-rw-r--r--   0 build     (1000) build     (1000)     7697 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/image/decoder/generic.py
+-rw-r--r--   0 build     (1000) build     (1000)     2797 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/image/decoder/vtf.py
+-rw-r--r--   0 build     (1000) build     (1000)     1497 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/image/image.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.546766 no_vtf-3.0.0/no_vtf/image/modifier/
+-rw-r--r--   0 build     (1000) build     (1000)      202 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/image/modifier/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)     1632 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/image/modifier/fp_precision_modifier.py
+-rw-r--r--   0 build     (1000) build     (1000)      540 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/image/modifier/modifier.py
+-rw-r--r--   0 build     (1000) build     (1000)      946 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/image/ndarray.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.546766 no_vtf-3.0.0/no_vtf/io/
+-rw-r--r--   0 build     (1000) build     (1000)      264 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/io/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)      573 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/io/bytes.py
+-rw-r--r--   0 build     (1000) build     (1000)     7977 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/io/image.py
+-rw-r--r--   0 build     (1000) build     (1000)      933 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/io/io.py
+-rw-r--r--   0 build     (1000) build     (1000)    11149 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/main.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.546766 no_vtf-3.0.0/no_vtf/parser/
+-rw-r--r--   0 build     (1000) build     (1000)        0 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/parser/__init__.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.546766 no_vtf-3.0.0/no_vtf/parser/generated/
+-rw-r--r--   0 build     (1000) build     (1000)        0 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/parser/generated/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)    25192 2023-06-09 18:24:12.000000 no_vtf-3.0.0/no_vtf/parser/generated/vtf.py
+-rw-r--r--   0 build     (1000) build     (1000)       93 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/parser/generated/vtf.py.license
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.546766 no_vtf-3.0.0/no_vtf/pipeline/
+-rw-r--r--   0 build     (1000) build     (1000)      186 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/pipeline/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)     4936 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/pipeline/pipeline.py
+-rw-r--r--   0 build     (1000) build     (1000)        0 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/py.typed
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.550766 no_vtf-3.0.0/no_vtf/task_runner/
+-rw-r--r--   0 build     (1000) build     (1000)      356 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/task_runner/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)     1524 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/task_runner/parallel.py
+-rw-r--r--   0 build     (1000) build     (1000)      826 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/task_runner/sequential.py
+-rw-r--r--   0 build     (1000) build     (1000)     1085 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/task_runner/task_runner.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.550766 no_vtf-3.0.0/no_vtf/texture/
+-rw-r--r--   0 build     (1000) build     (1000)        0 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/texture/__init__.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.550766 no_vtf-3.0.0/no_vtf/texture/decoder/
+-rw-r--r--   0 build     (1000) build     (1000)      204 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/texture/decoder/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)      486 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/texture/decoder/decoder.py
+-rw-r--r--   0 build     (1000) build     (1000)     4485 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/texture/decoder/vtf.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.550766 no_vtf-3.0.0/no_vtf/texture/extractor/
+-rw-r--r--   0 build     (1000) build     (1000)      212 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/texture/extractor/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)      453 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/texture/extractor/extractor.py
+-rw-r--r--   0 build     (1000) build     (1000)     4010 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/texture/extractor/vtf.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.550766 no_vtf-3.0.0/no_vtf/texture/filter/
+-rw-r--r--   0 build     (1000) build     (1000)      200 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/texture/filter/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)      367 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/texture/filter/filter.py
+-rw-r--r--   0 build     (1000) build     (1000)     2756 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/texture/filter/vtf.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.550766 no_vtf-3.0.0/no_vtf/texture/namer/
+-rw-r--r--   0 build     (1000) build     (1000)      196 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/texture/namer/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)      374 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/texture/namer/namer.py
+-rw-r--r--   0 build     (1000) build     (1000)     1025 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/texture/namer/vtf.py
+-rw-r--r--   0 build     (1000) build     (1000)      663 2023-06-09 18:14:25.000000 no_vtf-3.0.0/no_vtf/texture/vtf.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.542766 no_vtf-3.0.0/no_vtf.egg-info/
+-rw-r--r--   0 build     (1000) build     (1000)     9026 2023-06-09 18:24:31.000000 no_vtf-3.0.0/no_vtf.egg-info/PKG-INFO
+-rw-r--r--   0 build     (1000) build     (1000)     2409 2023-06-09 18:24:31.000000 no_vtf-3.0.0/no_vtf.egg-info/SOURCES.txt
+-rw-r--r--   0 build     (1000) build     (1000)        1 2023-06-09 18:24:31.000000 no_vtf-3.0.0/no_vtf.egg-info/dependency_links.txt
+-rw-r--r--   0 build     (1000) build     (1000)       49 2023-06-09 18:24:31.000000 no_vtf-3.0.0/no_vtf.egg-info/entry_points.txt
+-rw-r--r--   0 build     (1000) build     (1000)        1 2023-06-09 18:23:29.000000 no_vtf-3.0.0/no_vtf.egg-info/not-zip-safe
+-rw-r--r--   0 build     (1000) build     (1000)      183 2023-06-09 18:24:31.000000 no_vtf-3.0.0/no_vtf.egg-info/requires.txt
+-rw-r--r--   0 build     (1000) build     (1000)        7 2023-06-09 18:24:31.000000 no_vtf-3.0.0/no_vtf.egg-info/top_level.txt
+-rw-r--r--   0 build     (1000) build     (1000)     9785 2023-06-09 18:14:25.000000 no_vtf-3.0.0/noxfile.py
+-rw-r--r--   0 build     (1000) build     (1000)      682 2023-06-09 18:14:25.000000 no_vtf-3.0.0/pyproject.toml
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.534767 no_vtf-3.0.0/resources/
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.550766 no_vtf-3.0.0/resources/docs/
+-rw-r--r--   0 build     (1000) build     (1000)   123671 2023-06-09 18:14:25.000000 no_vtf-3.0.0/resources/docs/screencast.gif
+-rw-r--r--   0 build     (1000) build     (1000)       95 2023-06-09 18:14:25.000000 no_vtf-3.0.0/resources/docs/screencast.gif.license
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-06-09 18:24:31.554766 no_vtf-3.0.0/resources/pyinstaller/
+-rw-r--r--   0 build     (1000) build     (1000)        6 2023-06-09 18:14:25.000000 no_vtf-3.0.0/resources/pyinstaller/empty.ico
+-rw-r--r--   0 build     (1000) build     (1000)       93 2023-06-09 18:14:25.000000 no_vtf-3.0.0/resources/pyinstaller/empty.ico.license
+-rwxr-xr-x   0 build     (1000) build     (1000)      276 2023-06-09 18:14:25.000000 no_vtf-3.0.0/resources/pyinstaller/no_vtf.desktop
+-rw-r--r--   0 build     (1000) build     (1000)      103 2023-06-09 18:14:25.000000 no_vtf-3.0.0/resources/pyinstaller/no_vtf.desktop.license
+-rw-r--r--   0 build     (1000) build     (1000)     2657 2023-06-09 18:24:31.554766 no_vtf-3.0.0/setup.cfg
```

### Comparing `no_vtf-2.0.1/.build.yml` & `no_vtf-3.0.0/.build.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# Copyright (C) 2022 b5327157
+# SPDX-FileCopyrightText: b5327157 <b5327157@protonmail.com>
+#
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 image: debian/stable
 arch: amd64
 
 secrets:
 - a3cafe86-e4dd-4f18-b7ad-5809c8d577f2
 - 076fcca6-4239-4488-bf29-ec6dd1e9852c
 
 oauth: pages.sr.ht/PAGES:RW
 
 artifacts:
 - no_vtf.tar.gz
-- no_vtf.whl
 - no_vtf-linux_x64.tar.xz
 - no_vtf-windows_x64.zip
 
 tasks:
   - env: |
       cd no_vtf
       builds/debian/env.sh
@@ -37,15 +37,15 @@
   - diff_generated: |
       cd no_vtf
       builds/debian/ksc-install.sh
       builds/diff_generated.sh
 
   - package: |
       cd no_vtf
-      builds/nox.sh --session package -- ~/no_vtf.tar.gz ~/no_vtf.whl
+      builds/nox.sh --session package -- ~/no_vtf.tar.gz
 
   - freeze: |
       cd no_vtf
       builds/with_clone.sh builds/nox.sh --session freeze -- ~/no_vtf-linux_x64.tar.xz
 
   - freeze_wine: |
       cd no_vtf
```

### Comparing `no_vtf-2.0.1/PKG-INFO` & `no_vtf-3.0.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,18 @@
-Metadata-Version: 2.1
-Name: no_vtf
-Version: 2.0.1
-Summary: Valve Texture Format Converter
-Home-page: https://sr.ht/~b5327157/no_vtf
-Author: b5327157
-Author-email: b5327157@protonmail.com
-License: GNU Lesser General Public License v3 or later (LGPLv3+)
-Project-URL: Mailing list, https://lists.sr.ht/~b5327157/no_vtf
-Project-URL: Ticket tracker, https://todo.sr.ht/~b5327157/no_vtf
-Keywords: Source Engine,VTF,Valve Texture Format
-Platform: UNKNOWN
-Classifier: Environment :: Console
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Multimedia :: Graphics :: Graphics Conversion
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # no_vtf
 
-Say no to .vtf – convert it to one of the standard image formats.
+Say no to [.vtf](https://developer.valvesoftware.com/wiki/Valve_Texture_Format) – convert it to one of the standard image formats.
 
-[![Badge showing package version on PyPI](https://img.shields.io/pypi/v/no_vtf?style=flat-square)](https://pypi.org/project/no-vtf/)
-[![Badge showing number of monthly downloads from PyPI](https://img.shields.io/pypi/dm/no_vtf?style=flat-square)](https://pypi.org/project/no-vtf/)
 ![Badge showing supported Python versions](https://img.shields.io/pypi/pyversions/no_vtf?style=flat-square)
+[![Badge showing package version on PyPI](https://img.shields.io/pypi/v/no_vtf?style=flat-square)](https://pypi.org/project/no-vtf/)
+[![Badge showing number of monthly downloads from PyPI](https://img.shields.io/pypi/dm/no_vtf?style=flat-square)](https://pypistats.org/packages/no-vtf)
+[![Badge showing source code repository hosted on SourceHut](https://img.shields.io/badge/sr.ht-repository-white?labelColor=212529&logo=data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiIHN0YW5kYWxvbmU9Im5vIj8+CjxzdmcKICAgdmlld0JveD0iMCAwIDUxMiA1MTIiCiAgIHZlcnNpb249IjEuMSIKICAgaWQ9InN2ZzUxIgogICBzb2RpcG9kaTpkb2NuYW1lPSJzb3VyY2VodXQtd2hpdGUuc3ZnIgogICBpbmtzY2FwZTp2ZXJzaW9uPSIxLjEgKGM2OGUyMmMzODcsIDIwMjEtMDUtMjMpIgogICB4bWxuczppbmtzY2FwZT0iaHR0cDovL3d3dy5pbmtzY2FwZS5vcmcvbmFtZXNwYWNlcy9pbmtzY2FwZSIKICAgeG1sbnM6c29kaXBvZGk9Imh0dHA6Ly9zb2RpcG9kaS5zb3VyY2Vmb3JnZS5uZXQvRFREL3NvZGlwb2RpLTAuZHRkIgogICB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciCiAgIHhtbG5zOnN2Zz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPgogIDxkZWZzCiAgICAgaWQ9ImRlZnM1NSIgLz4KICA8c29kaXBvZGk6bmFtZWR2aWV3CiAgICAgaWQ9Im5hbWVkdmlldzUzIgogICAgIHBhZ2Vjb2xvcj0iIzUwNTA1MCIKICAgICBib3JkZXJjb2xvcj0iI2ZmZmZmZiIKICAgICBib3JkZXJvcGFjaXR5PSIxIgogICAgIGlua3NjYXBlOnBhZ2VzaGFkb3c9IjAiCiAgICAgaW5rc2NhcGU6cGFnZW9wYWNpdHk9IjAiCiAgICAgaW5rc2NhcGU6cGFnZWNoZWNrZXJib2FyZD0iMSIKICAgICBzaG93Z3JpZD0iZmFsc2UiCiAgICAgaW5rc2NhcGU6em9vbT0iMS42NTQyOTY5IgogICAgIGlua3NjYXBlOmN4PSIyNTYiCiAgICAgaW5rc2NhcGU6Y3k9IjI1NiIKICAgICBpbmtzY2FwZTp3aW5kb3ctd2lkdGg9IjE5MjAiCiAgICAgaW5rc2NhcGU6d2luZG93LWhlaWdodD0iMTA1OSIKICAgICBpbmtzY2FwZTp3aW5kb3cteD0iMCIKICAgICBpbmtzY2FwZTp3aW5kb3cteT0iMCIKICAgICBpbmtzY2FwZTp3aW5kb3ctbWF4aW1pemVkPSIxIgogICAgIGlua3NjYXBlOmN1cnJlbnQtbGF5ZXI9InN2ZzUxIiAvPgogIDxwYXRoCiAgICAgZD0iTTI1NiA4QzExOSA4IDggMTE5IDggMjU2czExMSAyNDggMjQ4IDI0OCAyNDgtMTExIDI0OC0yNDhTMzkzIDggMjU2IDh6bTAgNDQ4Yy0xMTAuNSAwLTIwMC04OS41LTIwMC0yMDBTMTQ1LjUgNTYgMjU2IDU2czIwMCA4OS41IDIwMCAyMDAtODkuNSAyMDAtMjAwIDIwMHoiCiAgICAgaWQ9InBhdGg0OSIKICAgICBzdHlsZT0iZmlsbDojZmZmZmZmIiAvPgo8L3N2Zz4K)](https://sr.ht/~b5327157/no_vtf)
+[![Badge showing builds.sr.ht status](https://builds.sr.ht/~b5327157/no_vtf.svg?search=tags:master)](https://builds.sr.ht/~b5327157/no_vtf?search=tags:master)
+[![Badge showing REUSE compliance status](https://api.reuse.software/badge/git.sr.ht/~b5327157/no_vtf)](https://api.reuse.software/info/git.sr.ht/~b5327157/no_vtf)
+[![Badge showing Nox as the chosen Python automation toolkit](https://img.shields.io/badge/🦊-Nox-D85E00.svg)](https://github.com/wntrblm/nox)
 
 ![Screencast showing conversion of sprays downloaded in Team Fortress 2 using no_vtf](https://git.sr.ht/~b5327157/no_vtf/blob/HEAD/resources/docs/screencast.gif)
 
 ## Motivation
 
 - cross-platform – runs on any machine where Python is supported
 - console-only – runs without a graphical interface
@@ -111,15 +91,15 @@
 no_vtf --help
 ```
 
 ## Supported formats
 
 ### Input
 
-All textures installed with Team Fortress 2 and Source Filmmaker can be converted with the supported format set.
+All textures installed with [Team Fortress 2](https://store.steampowered.com/app/440/Team_Fortress_2/), [Source Filmmaker](https://store.steampowered.com/app/1840/Source_Filmmaker/) and [Portal 2](https://store.steampowered.com/app/620/Portal_2/) can be converted with the supported format set.
 
 - `RGBA8888`
 - `ABGR8888`
 - `RGB888`
 - `BGR888`
 - `I8`
 - `IA88`
@@ -217,9 +197,7 @@
 ### Pre-build steps
 
 ```
 # compile .ksy files (requires Kaitai Struct compiler)
 # only necessary if a .ksy file was modified
 ksy/compile.sh
 ```
-
-
```

### Comparing `no_vtf-2.0.1/builds/common` & `no_vtf-3.0.0/builds/common`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright (C) 2022 b5327157
+# SPDX-FileCopyrightText: b5327157 <b5327157@protonmail.com>
+#
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 set -x
 set -e
 set -o pipefail
 
 # builds.sr.ht supports the complete-build command, which exits
```

### Comparing `no_vtf-2.0.1/builds/debian/wine-install.sh` & `no_vtf-3.0.0/builds/debian/wine-install.sh`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 #!/bin/bash
 
-# Copyright (C) 2022 b5327157
+# SPDX-FileCopyrightText: b5327157 <b5327157@protonmail.com>
+#
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 source builds/common
 
 WINEHQ_KEYRING_PATH='/usr/share/keyrings/winehq-archive-keyring.gpg'
 
 sudo dpkg --add-architecture i386
 
 curl 'https://dl.winehq.org/wine-builds/winehq.key' |
 	gpg --dearmor |
 	sudo tee "$WINEHQ_KEYRING_PATH" >/dev/null
 
 echo 'deb' \
 		'[signed-by='"$WINEHQ_KEYRING_PATH"']' \
-		'https://dl.winehq.org/wine-builds/debian stable main' |
+		'https://dl.winehq.org/wine-builds/debian bullseye main' |
 	sudo tee --append /etc/apt/sources.list >/dev/null
 
 sudo apt-get update
 
 sudo apt-get install --install-recommends winehq-stable
 
-MONO_BINARY_TARBALL_URL='https://dl.winehq.org/wine/wine-mono/7.0.0/wine-mono-7.0.0-x86.tar.xz'
+MONO_BINARY_TARBALL_URL='https://dl.winehq.org/wine/wine-mono/7.4.0/wine-mono-7.4.0-x86.tar.xz'
 MONO_DEST_DIR='/opt/wine-stable/share/wine/mono'
 sudo mkdir -p "$MONO_DEST_DIR"
 curl "$MONO_BINARY_TARBALL_URL" |
 	sudo tar xJ -C "$MONO_DEST_DIR"
```

### Comparing `no_vtf-2.0.1/builds/with_wine.sh` & `no_vtf-3.0.0/builds/with_wine.sh`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/bin/bash
 
-# Copyright (C) 2022 b5327157
+# SPDX-FileCopyrightText: b5327157 <b5327157@protonmail.com>
+#
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 source builds/common
 
 [ -n "$1" ]
 workdir="$1"
 shift
@@ -22,15 +23,15 @@
 alias nuget-install='nuget install -DirectDownload -Verbosity quiet -NonInteractive'
 
 if [ ! -e "$WINEPREFIX"'/.update-timestamp' ]; then
 	wineboot --init
 
 	curl --location --output nuget.exe 'https://aka.ms/nugetclidl'
 
-	wine nuget-install python
+	wine nuget-install python -Version 3.10.11
 	pushd python.*/tools >/dev/null
 	ln -s python.exe python3.10.exe
 	popd >/dev/null
 
 	wine nuget-install GitForWindows
 fi
```

### Comparing `no_vtf-2.0.1/ksy/vtf.ksy` & `no_vtf-3.0.0/ksy/vtf.ksy`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: b5327157 <b5327157@protonmail.com>
+#
+# SPDX-License-Identifier: CC0-1.0
+
 meta:
   id: vtf
   -author: b5327157
   -ksy-version: 1.0.1
   title: Valve Texture Format
   application: Source Engine
   file-extension: vtf
```

### Comparing `no_vtf-2.0.1/no_vtf/decoders/image/generic.py` & `no_vtf-3.0.0/no_vtf/image/decoder/generic.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,155 +1,170 @@
-# Copyright (C) 2022 b5327157
+# SPDX-FileCopyrightText: b5327157 <b5327157@protonmail.com>
+#
 # SPDX-License-Identifier: LGPL-3.0-or-later
 
 import functools
 
 import numpy as np
 import numpy.typing as npt
 import PIL.BlpImagePlugin
 import PIL.Image
 
-from no_vtf.deferrable import Deferred
+from no_vtf.deferred import Deferred
 from no_vtf.image import Image
-from no_vtf.ndarray import image_ndarray
+from no_vtf.image.ndarray import image_bytes_to_ndarray
 
 
 def decode_rgb_uint8(encoded_image: bytes, width: int, height: int) -> Image[np.uint8]:
-    data = Deferred(lambda: image_ndarray(encoded_image, width, height, (0, 1, 2), np.uint8))
-    return Image(data=data, dtype=np.uint8, channels="rgb")
+    data = Deferred(
+        lambda: image_bytes_to_ndarray(encoded_image, width, height, (0, 1, 2), np.uint8)
+    )
+    return Image(raw=encoded_image, data=data, dtype=np.uint8, channels="rgb")
 
 
 def decode_rgba_uint8(encoded_image: bytes, width: int, height: int) -> Image[np.uint8]:
-    data = Deferred(lambda: image_ndarray(encoded_image, width, height, (0, 1, 2, 3), np.uint8))
-    return Image(data=data, dtype=np.uint8, channels="rgba")
+    data = Deferred(
+        lambda: image_bytes_to_ndarray(encoded_image, width, height, (0, 1, 2, 3), np.uint8)
+    )
+    return Image(raw=encoded_image, data=data, dtype=np.uint8, channels="rgba")
 
 
 def decode_argb_uint8(encoded_image: bytes, width: int, height: int) -> Image[np.uint8]:
-    data = Deferred(lambda: image_ndarray(encoded_image, width, height, (1, 2, 3, 0), np.uint8))
-    return Image(data=data, dtype=np.uint8, channels="rgba")
+    data = Deferred(
+        lambda: image_bytes_to_ndarray(encoded_image, width, height, (1, 2, 3, 0), np.uint8)
+    )
+    return Image(raw=encoded_image, data=data, dtype=np.uint8, channels="rgba")
 
 
 def decode_bgr_uint8(encoded_image: bytes, width: int, height: int) -> Image[np.uint8]:
-    data = Deferred(lambda: image_ndarray(encoded_image, width, height, (2, 1, 0), np.uint8))
-    return Image(data=data, dtype=np.uint8, channels="rgb")
+    data = Deferred(
+        lambda: image_bytes_to_ndarray(encoded_image, width, height, (2, 1, 0), np.uint8)
+    )
+    return Image(raw=encoded_image, data=data, dtype=np.uint8, channels="rgb")
 
 
 def decode_bgra_uint8(encoded_image: bytes, width: int, height: int) -> Image[np.uint8]:
-    data = Deferred(lambda: image_ndarray(encoded_image, width, height, (2, 1, 0, 3), np.uint8))
-    return Image(data=data, dtype=np.uint8, channels="rgba")
+    data = Deferred(
+        lambda: image_bytes_to_ndarray(encoded_image, width, height, (2, 1, 0, 3), np.uint8)
+    )
+    return Image(raw=encoded_image, data=data, dtype=np.uint8, channels="rgba")
 
 
 def decode_abgr_uint8(encoded_image: bytes, width: int, height: int) -> Image[np.uint8]:
-    data = Deferred(lambda: image_ndarray(encoded_image, width, height, (3, 2, 1, 0), np.uint8))
-    return Image(data=data, dtype=np.uint8, channels="rgba")
+    data = Deferred(
+        lambda: image_bytes_to_ndarray(encoded_image, width, height, (3, 2, 1, 0), np.uint8)
+    )
+    return Image(raw=encoded_image, data=data, dtype=np.uint8, channels="rgba")
 
 
 def decode_rgba_uint16_be(encoded_image: bytes, width: int, height: int) -> Image[np.uint16]:
     data = Deferred(
-        lambda: image_ndarray(encoded_image, width, height, (0, 1, 2, 3), np.uint16, ">")
+        lambda: image_bytes_to_ndarray(encoded_image, width, height, (0, 1, 2, 3), np.uint16, ">")
     )
-    return Image(data=data, dtype=np.uint16, channels="rgba")
+    return Image(raw=encoded_image, data=data, dtype=np.uint16, channels="rgba")
 
 
 def decode_rgba_uint16_le(encoded_image: bytes, width: int, height: int) -> Image[np.uint16]:
     data = Deferred(
-        lambda: image_ndarray(encoded_image, width, height, (0, 1, 2, 3), np.uint16, "<")
+        lambda: image_bytes_to_ndarray(encoded_image, width, height, (0, 1, 2, 3), np.uint16, "<")
     )
-    return Image(data=data, dtype=np.uint16, channels="rgba")
+    return Image(raw=encoded_image, data=data, dtype=np.uint16, channels="rgba")
 
 
 def decode_rgba_float16_be(encoded_image: bytes, width: int, height: int) -> Image[np.float16]:
     data = Deferred(
-        lambda: image_ndarray(encoded_image, width, height, (0, 1, 2, 3), np.float16, ">")
+        lambda: image_bytes_to_ndarray(encoded_image, width, height, (0, 1, 2, 3), np.float16, ">")
     )
-    return Image(data=data, dtype=np.float16, channels="rgba")
+    return Image(raw=encoded_image, data=data, dtype=np.float16, channels="rgba")
 
 
 def decode_rgba_float16_le(encoded_image: bytes, width: int, height: int) -> Image[np.float16]:
     data = Deferred(
-        lambda: image_ndarray(encoded_image, width, height, (0, 1, 2, 3), np.float16, "<")
+        lambda: image_bytes_to_ndarray(encoded_image, width, height, (0, 1, 2, 3), np.float16, "<")
     )
-    return Image(data=data, dtype=np.float16, channels="rgba")
+    return Image(raw=encoded_image, data=data, dtype=np.float16, channels="rgba")
 
 
 def decode_l_uint8(encoded_image: bytes, width: int, height: int) -> Image[np.uint8]:
-    data = Deferred(lambda: image_ndarray(encoded_image, width, height, (0,), np.uint8))
-    return Image(data=data, dtype=np.uint8, channels="l")
+    data = Deferred(lambda: image_bytes_to_ndarray(encoded_image, width, height, (0,), np.uint8))
+    return Image(raw=encoded_image, data=data, dtype=np.uint8, channels="l")
 
 
 def decode_a_uint8(encoded_image: bytes, width: int, height: int) -> Image[np.uint8]:
-    data = Deferred(lambda: image_ndarray(encoded_image, width, height, (0,), np.uint8))
-    return Image(data=data, dtype=np.uint8, channels="a")
+    data = Deferred(lambda: image_bytes_to_ndarray(encoded_image, width, height, (0,), np.uint8))
+    return Image(raw=encoded_image, data=data, dtype=np.uint8, channels="a")
 
 
 def decode_la_uint8(encoded_image: bytes, width: int, height: int) -> Image[np.uint8]:
-    la_uint8 = Deferred(lambda: image_ndarray(encoded_image, width, height, (0, 1), np.uint8))
-    return Image(data=la_uint8, dtype=np.uint8, channels="la")
+    la_uint8 = Deferred(
+        lambda: image_bytes_to_ndarray(encoded_image, width, height, (0, 1), np.uint8)
+    )
+    return Image(raw=encoded_image, data=la_uint8, dtype=np.uint8, channels="la")
 
 
 def decode_uv_uint8(encoded_image: bytes, width: int, height: int) -> Image[np.uint8]:
     def thunk() -> npt.NDArray[np.uint8]:
-        rg_uint8 = image_ndarray(encoded_image, width, height, (0, 1), np.uint8)
+        rg_uint8 = image_bytes_to_ndarray(encoded_image, width, height, (0, 1), np.uint8)
         b_uint8: npt.NDArray[np.uint8] = np.zeros(rg_uint8.shape[:-1], dtype=np.uint8)
         rgb_uint8: npt.NDArray[np.uint8] = np.dstack((rg_uint8, b_uint8))
         return rgb_uint8
 
-    return Image(data=Deferred(thunk), dtype=np.uint8, channels="rgb")
+    return Image(raw=encoded_image, data=Deferred(thunk), dtype=np.uint8, channels="rgb")
 
 
 def decode_bgra_uint4_le(encoded_image: bytes, width: int, height: int) -> Image[np.uint8]:
     def thunk() -> npt.NDArray[np.uint8]:
-        bgra_uint4 = image_ndarray(encoded_image, width, height, (0, 1), np.uint8)
+        bgra_uint4 = image_bytes_to_ndarray(encoded_image, width, height, (0, 1), np.uint8)
 
         br_uint8 = np.bitwise_and(np.left_shift(bgra_uint4, 4), 0xF0)
         ga_uint8 = np.bitwise_and(bgra_uint4, 0xF0)
 
         r_uint8 = br_uint8[..., [1]]
         g_uint8 = ga_uint8[..., [0]]
         b_uint8 = br_uint8[..., [0]]
         a_uint8 = ga_uint8[..., [1]]
 
         rgba_uint8: npt.NDArray[np.uint8] = np.dstack((r_uint8, g_uint8, b_uint8, a_uint8))
         return rgba_uint8
 
-    return Image(data=Deferred(thunk), dtype=np.uint8, channels="rgba")
+    return Image(raw=encoded_image, data=Deferred(thunk), dtype=np.uint8, channels="rgba")
 
 
 def decode_dxt1_rgb(
     encoded_image: bytes, logical_width: int, logical_height: int
 ) -> Image[np.uint8]:
     def thunk() -> npt.NDArray[np.uint8]:
         rgba_uint8 = _decode_dxt_generic(encoded_image, logical_width, logical_height, 1, "DXT1")
         rgb_uint8: npt.NDArray[np.uint8] = rgba_uint8[..., :3]
         return rgb_uint8
 
-    return Image(data=Deferred(thunk), dtype=np.uint8, channels="rgb")
+    return Image(raw=encoded_image, data=Deferred(thunk), dtype=np.uint8, channels="rgb")
 
 
 def decode_dxt1_rgba(
     encoded_image: bytes, logical_width: int, logical_height: int
 ) -> Image[np.uint8]:
     thunk = functools.partial(
         _decode_dxt_generic, encoded_image, logical_width, logical_height, 1, "DXT1"
     )
-    return Image(data=Deferred(thunk), dtype=np.uint8, channels="rgba")
+    return Image(raw=encoded_image, data=Deferred(thunk), dtype=np.uint8, channels="rgba")
 
 
 def decode_dxt3(encoded_image: bytes, logical_width: int, logical_height: int) -> Image[np.uint8]:
     thunk = functools.partial(
         _decode_dxt_generic, encoded_image, logical_width, logical_height, 2, "DXT3"
     )
-    return Image(data=Deferred(thunk), dtype=np.uint8, channels="rgba")
+    return Image(raw=encoded_image, data=Deferred(thunk), dtype=np.uint8, channels="rgba")
 
 
 def decode_dxt5(encoded_image: bytes, logical_width: int, logical_height: int) -> Image[np.uint8]:
     thunk = functools.partial(
         _decode_dxt_generic, encoded_image, logical_width, logical_height, 3, "DXT5"
     )
-    return Image(data=Deferred(thunk), dtype=np.uint8, channels="rgba")
+    return Image(raw=encoded_image, data=Deferred(thunk), dtype=np.uint8, channels="rgba")
 
 
 def _decode_dxt_generic(
     encoded_image: bytes, logical_width: int, logical_height: int, n: int, pixel_format: str
 ) -> npt.NDArray[np.uint8]:
     physical_width, physical_height = _dxt_physical_dimensions(logical_width, logical_height)
```

### Comparing `no_vtf-2.0.1/no_vtf/decoders/texture/vtf.py` & `no_vtf-3.0.0/no_vtf/texture/decoder/vtf.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-# Copyright (C) 2022 b5327157
+# SPDX-FileCopyrightText: b5327157 <b5327157@protonmail.com>
+#
 # SPDX-License-Identifier: LGPL-3.0-or-later
 
 import functools
 
 from dataclasses import dataclass
 from typing import Optional
 
-from no_vtf.decoder.image import ImageDecoder
-from no_vtf.decoder.texture import TextureDecoder
-from no_vtf.decoders.image.generic import (
+from no_vtf.image import Image, ImageDataTypes, ImageDynamicRange
+from no_vtf.image.decoder.decoder import ImageDecoder
+from no_vtf.image.decoder.generic import (
     decode_a_uint8,
     decode_abgr_uint8,
     decode_argb_uint8,
     decode_bgr_uint8,
     decode_bgra_uint4_le,
     decode_bgra_uint8,
     decode_dxt1_rgb,
@@ -22,44 +23,48 @@
     decode_l_uint8,
     decode_la_uint8,
     decode_rgb_uint8,
     decode_rgba_float16_le,
     decode_rgba_uint8,
     decode_uv_uint8,
 )
-from no_vtf.decoders.image.vtf import (
+from no_vtf.image.decoder.vtf import (
     decode_bgr_uint8_bluescreen,
     decode_bgra_uint8_hdr,
     decode_rgb_uint8_bluescreen,
     decode_rgba_uint16_le_hdr,
 )
-from no_vtf.image import DynamicRange, Image, ImageDataTypes
-from no_vtf.parsers.generated.vtf import Vtf as VtfParser
-from no_vtf.textures.vtf import VtfTexture
+from no_vtf.parser.generated.vtf import Vtf as VtfParser
+from no_vtf.texture.decoder.decoder import TextureDecoder
+from no_vtf.texture.vtf import VtfTexture
 
 
 @dataclass(frozen=True, kw_only=True)
-class VtfDecoder(TextureDecoder[VtfTexture]):
-    dynamic_range: DynamicRange
+class VtfDecoder(TextureDecoder[VtfTexture, ImageDataTypes]):
+    dynamic_range: Optional[ImageDynamicRange] = None
     overbright_factor: Optional[float] = None
 
     def __call__(self, texture: VtfTexture) -> Image[ImageDataTypes]:
         encoded_image = texture.image.image_data
         logical_width = texture.image.logical_width
         logical_height = texture.image.logical_height
 
         decoder = self._get_decoder(texture)
         decoded_image = decoder(encoded_image, logical_width, logical_height)
         return decoded_image
 
     def _get_decoder(self, texture: VtfTexture) -> ImageDecoder[ImageDataTypes]:
         image_format = texture.image.image_format
 
+        dynamic_range = (
+            self.dynamic_range if self.dynamic_range is not None else texture.dynamic_range
+        )
+
         decoder: Optional[ImageDecoder[ImageDataTypes]] = None
-        match (image_format, self.dynamic_range):
+        match (image_format, dynamic_range):
             case VtfParser.ImageFormat.rgba8888, _:
                 decoder = decode_rgba_uint8
             case VtfParser.ImageFormat.abgr8888, _:
                 decoder = decode_abgr_uint8
             case VtfParser.ImageFormat.rgb888, _:
                 decoder = decode_rgb_uint8
             case VtfParser.ImageFormat.bgr888, _:
@@ -74,14 +79,16 @@
                 decoder = decode_rgb_uint8_bluescreen
             case VtfParser.ImageFormat.bgr888_bluescreen, _:
                 decoder = decode_bgr_uint8_bluescreen
             case VtfParser.ImageFormat.argb8888, _:
                 # VTFLib/VTFEdit, Gimp VTF Plugin, and possibly others, decode this format
                 # differently because of mismatched channels (verified against VTF2TGA).
                 decoder = decode_argb_uint8
+            case VtfParser.ImageFormat.bgra8888, None:
+                raise RuntimeError("Dynamic range is set neither on VtfTexture nor VtfDecoder")
             case VtfParser.ImageFormat.bgra8888, "ldr":
                 decoder = decode_bgra_uint8
             case VtfParser.ImageFormat.bgra8888, "hdr":
                 decoder = functools.partial(
                     decode_bgra_uint8_hdr, overbright_factor=self.overbright_factor
                 )
             case VtfParser.ImageFormat.dxt1, _:
```

### Comparing `no_vtf-2.0.1/no_vtf/ios/imageio.py` & `no_vtf-3.0.0/no_vtf/io/image.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,213 +1,219 @@
-# Copyright (C) 2022 b5327157
+# SPDX-FileCopyrightText: b5327157 <b5327157@protonmail.com>
+#
 # SPDX-License-Identifier: LGPL-3.0-or-later
 
 from __future__ import annotations
 
+import functools
 import pathlib
 import re
 
 from dataclasses import dataclass
 from typing import ClassVar, Optional, cast
 
-import imageio
 import imageio.plugins.freeimage
+import imageio.v3
 import numpy as np
 import numpy.typing as npt
 
-from no_vtf.deferrable import Deferrable, from_deferrable
 from no_vtf.image import Image, ImageData, ImageDataTypes
-from no_vtf.io import Io
-from no_vtf.postprocessor import Postprocessor
-from no_vtf.postprocessors.fp_precision_modifier import FloatingPointPrecisionModifier
+from no_vtf.image.modifier.fp_precision_modifier import FPPrecisionModifier
+from no_vtf.image.modifier.modifier import ImageModifier
+from no_vtf.io.io import IO
 
 
 @dataclass(frozen=True, kw_only=True)
-class Imageio(Io[Image[ImageDataTypes]]):
-
-    _format_pattern: ClassVar[re.Pattern[str]] = re.compile(r"[a-z0-9]+", re.ASCII | re.IGNORECASE)
+class ImageIO(IO[Image[ImageDataTypes]]):
+    format: str
 
-    _freeimage_requested: ClassVar[bool] = False
+    compress: Optional[bool] = None
 
     @classmethod
-    def request_freeimage(cls) -> None:
-        if cls._freeimage_requested:
-            return
-
-        imageio.plugins.freeimage.download()
+    def _initialize(cls) -> None:
+        # download() seems to be untyped because of implicit reexport
+        imageio.plugins.freeimage.download()  # type: ignore[no-untyped-call]
 
-        cls._freeimage_requested = True
-
-    format: str
-
-    compress: Optional[bool] = None
+    _format_pattern: ClassVar[re.Pattern[str]] = re.compile(r"[a-z0-9]+", re.ASCII | re.IGNORECASE)
 
     def __post_init__(self) -> None:
+        assert self._is_initialized(), "IO.initialize() must be called early"
+
         if not self._format_pattern.fullmatch(self.format):
             raise RuntimeError(f"Invalid format: {self.format}")
 
-    def write(self, path: pathlib.Path, image: Deferrable[Image[ImageDataTypes]]) -> None:
+    def write(self, path: pathlib.Path, image: Image[ImageDataTypes]) -> None:
         backend = self._get_backend()
-        data = self._get_data(image)
-
-        backend.write(path, data)
+        backend.write(path, image)
 
-    def readback(self, path: pathlib.Path, image: Deferrable[Image[ImageDataTypes]]) -> None:
+    def readback(self, path: pathlib.Path, image: Image[ImageDataTypes]) -> None:
         backend = self._get_backend()
-        data = self._get_data(image)
-
-        backend.readback(path, data)
+        backend.readback(path, image)
 
-    def _get_backend(self) -> ImageioBackend:
+    def _get_backend(self) -> _ImageIOBackend:
         compress = self.compress
         if compress is None:
             compress = True
 
-        backend: ImageioBackend
+        extension = f".{self.format}"
+
+        backend: _ImageIOBackend
         match self.format.lower():
             case "exr":
-                backend = ImageioExrBackend(compress=compress)
+                backend = _ImageIOExrBackend(compress=compress)
             case "png":
-                backend = ImageioPngBackend(compress=compress)
+                backend = _ImageIOPngBackend(compress=compress)
             case "targa" | "tga":
-                backend = ImageioTgaBackend(compress=compress)
+                backend = _ImageIOTgaBackend(compress=compress)
             case "tiff":
-                backend = ImageioTiffBackend(compress=compress)
+                backend = _ImageIOTiffBackend(compress=compress)
             case _:
-                backend = ImageioBackend()
+                backend = _ImageIOBackend(extension=extension)
         return backend
 
-    def _get_data(self, image: Deferrable[Image[ImageDataTypes]]) -> ImageData:
-        image = from_deferrable(image)
-        data = image.data()
-
-        # write luminance into three channels when alpha is present
-        if image.channels == "la":
-            l_uint8: npt.NDArray[np.uint8] = data[:, :, [0]]
-            a_uint8: npt.NDArray[np.uint8] = data[:, :, [1]]
-            data = np.dstack((l_uint8, l_uint8, l_uint8, a_uint8))
 
-        # remove last axis if its length is 1
-        if data.shape[-1] == 1:
-            data = data[..., 0]
+class _ImageIOBackend:
+    def __init__(
+        self, *, imageio_format: Optional[str] = None, extension: Optional[str] = None
+    ) -> None:
+        self._imageio_format = imageio_format
+        self._extension = extension
+
+    def write(self, path: pathlib.Path, image: Image[ImageDataTypes]) -> None:
+        kwargs = self._get_writer_kwargs(image)
+        image = self._postprocess(image)
+        data = self._get_data(image)
 
-        return data
+        legacy_opener = functools.partial(imageio.v3.imopen, legacy_mode=True)
+        with legacy_opener(
+            path, "w", plugin=self._imageio_format, extension=self._extension
+        ) as image_resource:
+            image_resource.write(data, **kwargs)
 
+    def readback(self, path: pathlib.Path, image: Image[ImageDataTypes]) -> None:
+        image = self._postprocess(image)
+        data = self._get_data(image)
 
-class ImageioBackend:
-    def __init__(self, *, _imageio_format: Optional[str] = None) -> None:
-        self._imageio_format = _imageio_format
-
-    def write(self, path: pathlib.Path, data: ImageData) -> None:
-        kwargs = self._get_writer_kwargs(data)
-        data = self._postprocess(data)
-        with imageio.get_writer(path, format=self._imageio_format, mode="i", **kwargs) as writer:
-            writer.append_data(data)
-
-    def readback(self, path: pathlib.Path, data: ImageData) -> None:
-        data = self._postprocess(data)
-        with imageio.get_reader(path, format=self._imageio_format, mode="i") as reader:
-            read_data = reader.get_data(index=0)
+        legacy_opener = functools.partial(imageio.v3.imopen, legacy_mode=True)
+        with legacy_opener(
+            path, "r", plugin=self._imageio_format, extension=self._extension
+        ) as image_resource:
+            read_data = image_resource.read(index=0)
 
             if data.dtype != read_data.dtype:
-                raise RuntimeError("Data type differs from what is in the file")
+                raise RuntimeError(f"{path!r}: Data type differs from what is in the file")
 
-            if not self._compare(data, read_data):
-                raise RuntimeError("Data differs from what is in the file")
+            if not self._compare_data(data, read_data):
+                raise RuntimeError(f"{path!r}: Data differs from what is in the file")
 
-    def _get_writer_kwargs(self, data: ImageData) -> dict[str, object]:
+    def _get_writer_kwargs(self, image: Image[ImageDataTypes]) -> dict[str, object]:
         return {}
 
-    def _postprocess(self, data: ImageData) -> ImageData:
+    def _postprocess(self, image: Image[ImageDataTypes]) -> Image[ImageDataTypes]:
+        return image
+
+    def _get_data(self, image: Image[ImageDataTypes]) -> ImageData:
+        data = image.data()
+
+        # write luminance into three channels when alpha is present
+        if image.channels == "la":
+            l_uint8: npt.NDArray[ImageDataTypes] = data[:, :, [0]]
+            a_uint8: npt.NDArray[ImageDataTypes] = data[:, :, [1]]
+            data = np.dstack((l_uint8, l_uint8, l_uint8, a_uint8))
+
+        # remove last axis if its length is 1
+        if data.shape[-1] == 1:
+            data = data[..., 0]
+
         return data
 
-    def _compare(self, data: ImageData, read_data: ImageData) -> bool:
+    def _compare_data(self, data: ImageData, read_data: ImageData) -> bool:
         return np.array_equal(data, read_data)
 
 
-class ImageioFreeImageBackend(ImageioBackend):
+class _ImageIOFreeImageBackend(_ImageIOBackend):
     IO_FLAGS: ClassVar = imageio.plugins.freeimage.IO_FLAGS
 
-    def __init__(self, *, _imageio_format: str) -> None:
-        super().__init__(_imageio_format=_imageio_format)
+    def __init__(self, *, imageio_format: str, extension: str) -> None:
+        super().__init__(imageio_format=imageio_format, extension=extension)
 
-    def _get_writer_kwargs(self, data: ImageData) -> dict[str, object]:
+    def _get_writer_kwargs(self, image: Image[ImageDataTypes]) -> dict[str, object]:
         kwargs: dict[str, object] = {}
-        kwargs["flags"] = self._get_flags(data)
+        kwargs["flags"] = self._get_flags(image)
         return kwargs
 
-    def _get_flags(self, data: ImageData) -> int:
+    def _get_flags(self, image: Image[ImageDataTypes]) -> int:
         return 0
 
 
-class ImageioExrBackend(ImageioFreeImageBackend):
-    _fp_force_32_bits: ClassVar[Postprocessor[ImageData]] = FloatingPointPrecisionModifier(
-        forced=32
-    )
+class _ImageIOExrBackend(_ImageIOFreeImageBackend):
+    _fp_force_32_bits: ClassVar[
+        ImageModifier[ImageDataTypes, ImageDataTypes]
+    ] = FPPrecisionModifier(min=32, max=32)
 
     def __init__(self, *, compress: bool = True) -> None:
-        super().__init__(_imageio_format="EXR-FI")
+        super().__init__(imageio_format="EXR-FI", extension=".exr")
         self.compress = compress
 
-    def _get_flags(self, data: ImageData) -> int:
+    def _get_flags(self, image: Image[ImageDataTypes]) -> int:
         flags = 0
         flags |= self.IO_FLAGS.EXR_ZIP if self.compress else self.IO_FLAGS.EXR_NONE
-        if not np.issubdtype(data.dtype, np.float16):
+        if not np.issubdtype(image.data().dtype, np.float16):
             flags |= self.IO_FLAGS.EXR_FLOAT
         return flags
 
-    def _postprocess(self, data: ImageData) -> ImageData:
-        return self._fp_force_32_bits(data)
+    def _postprocess(self, image: Image[ImageDataTypes]) -> Image[ImageDataTypes]:
+        return self._fp_force_32_bits(image)
 
 
-class ImageioPngBackend(ImageioFreeImageBackend):
+class _ImageIOPngBackend(_ImageIOFreeImageBackend):
     def __init__(self, *, compress: bool = True) -> None:
-        super().__init__(_imageio_format="PNG-FI")
+        super().__init__(imageio_format="PNG-FI", extension=".png")
         self.compress = compress
 
-    def _get_writer_kwargs(self, data: ImageData) -> dict[str, object]:
-        kwargs: dict[str, object] = super()._get_writer_kwargs(data)
+    def _get_writer_kwargs(self, image: Image[ImageDataTypes]) -> dict[str, object]:
+        kwargs: dict[str, object] = super()._get_writer_kwargs(image)
         kwargs["compression"] = 1 if self.compress else 0
         return kwargs
 
-    def _compare(self, data: ImageData, read_data: ImageData) -> bool:
+    def _compare_data(self, data: ImageData, read_data: ImageData) -> bool:
         if np.issubdtype(data.dtype, np.uint8) and np.issubdtype(read_data.dtype, np.uint8):
             if read_data.ndim == 3 and read_data.shape[2] == 3:
                 data = _strip_opaque_alpha(cast(npt.NDArray[np.uint8], data))
 
-        return super()._compare(data, read_data)
+        return super()._compare_data(data, read_data)
 
 
-class ImageioTgaBackend(ImageioFreeImageBackend):
+class _ImageIOTgaBackend(_ImageIOFreeImageBackend):
     def __init__(self, *, compress: bool = True) -> None:
-        super().__init__(_imageio_format="TARGA-FI")
+        super().__init__(imageio_format="TARGA-FI", extension=".tga")
         self.compress = compress
 
-    def _get_flags(self, data: ImageData) -> int:
+    def _get_flags(self, image: Image[ImageDataTypes]) -> int:
         flags = 0
         flags |= self.IO_FLAGS.TARGA_SAVE_RLE if self.compress else self.IO_FLAGS.TARGA_DEFAULT
         return flags
 
 
-class ImageioTiffBackend(ImageioFreeImageBackend):
-    _fp_force_32_bits: ClassVar[Postprocessor[ImageData]] = FloatingPointPrecisionModifier(
-        forced=32
-    )
+class _ImageIOTiffBackend(_ImageIOFreeImageBackend):
+    _fp_force_32_bits: ClassVar[
+        ImageModifier[ImageDataTypes, ImageDataTypes]
+    ] = FPPrecisionModifier(min=32, max=32)
 
     def __init__(self, *, compress: bool = True) -> None:
-        super().__init__(_imageio_format="TIFF-FI")
+        super().__init__(imageio_format="TIFF-FI", extension=".tiff")
         self.compress = compress
 
-    def _get_flags(self, data: ImageData) -> int:
+    def _get_flags(self, image: Image[ImageDataTypes]) -> int:
         flags = 0
         flags |= self.IO_FLAGS.TIFF_DEFAULT if self.compress else self.IO_FLAGS.TIFF_NONE
         return flags
 
-    def _postprocess(self, data: ImageData) -> ImageData:
-        return self._fp_force_32_bits(data)
+    def _postprocess(self, image: Image[ImageDataTypes]) -> Image[ImageDataTypes]:
+        return self._fp_force_32_bits(image)
 
 
 def _strip_opaque_alpha(data: npt.NDArray[np.uint8]) -> npt.NDArray[np.uint8]:
     if data.ndim == 3 and data.shape[2] == 4 and np.all(data[..., 3] == 255):
         data = data[..., :3]
 
     return data
```

### Comparing `no_vtf-2.0.1/no_vtf/main.py` & `no_vtf-3.0.0/no_vtf/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,47 @@
-# Copyright (C) 2022 b5327157
+# SPDX-FileCopyrightText: b5327157 <b5327157@protonmail.com>
+#
 # SPDX-License-Identifier: LGPL-3.0-or-later
 
+from __future__ import annotations
+
 import contextlib
 import inspect
 import pathlib
+import re
 import sys
 
-from typing import Optional, Sequence
+from collections.abc import Sequence
+from dataclasses import dataclass
+from typing import Generic, Optional, TypeVar, cast
 
 import alive_progress
 import click
 
 import no_vtf
 
-from no_vtf.files.vtf import VtfFile
-from no_vtf.filesystem import DirectoryFilesList
-from no_vtf.image import DynamicRange
+from no_vtf.filesystem import InputPaths, OutputDirectories
+from no_vtf.image import ImageDataTypes, ImageDynamicRange
 from no_vtf.pipeline import Pipeline
-from no_vtf.pipeline_runner import PipelineRunner, Task
-from no_vtf.pipeline_runners.parallel_runner import ParallelRunner
-from no_vtf.pipeline_runners.sequential_runner import SequentialRunner
-from no_vtf.textures.vtf import VtfTexture
+from no_vtf.task_runner import ParallelRunner, SequentialRunner, TaskRunner
+from no_vtf.texture.decoder.vtf import VtfDecoder
+from no_vtf.texture.extractor.vtf import VtfExtractor
+from no_vtf.texture.filter.vtf import VtfMipmapFilter
+from no_vtf.texture.namer.vtf import Vtf2TgaLikeNamer
+
+_T = TypeVar("_T")
 
 
 def _show_credits(ctx: click.Context, param: click.Parameter, value: bool) -> None:
     if not value or ctx.resilient_parsing:
         return
 
     credits = """
     no_vtf - Valve Texture Format Converter
-    Copyright (C) 2022 b5327157
+    Copyright (C) 2023 b5327157
 
     https://sr.ht/~b5327157/no_vtf/
     https://pypi.org/project/no-vtf/
 
     This program is free software: you can redistribute it and/or modify it under
     the terms of the GNU Lesser General Public License as published by the Free
     Software Foundation, either version 3 of the License, or (at your option)
@@ -60,17 +68,15 @@
     nargs=-1,
 )
 @click.option(
     "--output-dir",
     "-o",
     "output_directory",
     help="Output directory",
-    type=click.Path(
-        path_type=pathlib.Path, exists=True, file_okay=False, dir_okay=True, writable=True
-    ),
+    type=click.Path(path_type=pathlib.Path, exists=True, file_okay=False, dir_okay=True),
 )
 @click.option(
     "--ldr-format", "-l", help="LDR output format", show_default=True, type=str, default="tiff"
 )
 @click.option(
     "--hdr-format", "-h", help="HDR output format", show_default=True, type=str, default="exr"
 )
@@ -127,35 +133,35 @@
     help="Show the credits and exit.",
     type=bool,
     is_flag=True,
     expose_value=False,
     is_eager=True,
     callback=_show_credits,
 )
-def main(
+def main_command(
     *,
     paths: Sequence[pathlib.Path],
     output_directory: Optional[pathlib.Path],
     ldr_format: str,
     hdr_format: str,
-    dynamic_range: Optional[DynamicRange],
+    dynamic_range: Optional[ImageDynamicRange],
     mipmaps: bool,
     separate_channels: bool,
     overbright_factor: float,
     compress: Optional[bool],
     write: Optional[bool],
     readback: bool,
     num_workers: Optional[int],
     no_progress: bool,
 ) -> None:
     """
     Convert Valve Texture Format files into standard image files.
 
-    PATH can be either file, or directory (in which case it is recursively searched for .vtf files).
-    Multiple paths may be provided.
+    PATH can be either file, or directory (in which case it is recursively searched
+    for .vtf files, symbolic links are not followed). Multiple paths may be provided.
 
     If the output directory is not specified, images are output into the source directories.
     Otherwise, directory tree for any found files will be reconstructed in the chosen directory.
 
     Output LDR/HDR format is selected by its common file name extension.
     Special formats:
     "raw" to write the high resolution image data as-is;
@@ -183,91 +189,153 @@
     Worker is spawned for each logical core to run the conversion in parallel.
     Number of workers can be overridden. If set to 1, conversion is sequential.
 
     Exit status: Zero if all went successfully, non-zero if there was an error.
     Upon a recoverable error, conversion will proceed with the next file.
     """
 
-    _global_config()
+    main(
+        paths=paths,
+        output_directory=output_directory,
+        ldr_format=ldr_format,
+        hdr_format=hdr_format,
+        dynamic_range=dynamic_range,
+        mipmaps=mipmaps,
+        separate_channels=separate_channels,
+        overbright_factor=overbright_factor,
+        compress=compress,
+        write=write,
+        readback=readback,
+        num_workers=num_workers,
+        no_progress=no_progress,
+    )
 
-    directory_files_list = DirectoryFilesList.from_paths(paths)
-    if directory_files_list.has_unresolved_files():
-        _resolve_files(directory_files_list, not no_progress)
 
-    file_factory = VtfFile.make_factory(
-        mipmaps=mipmaps, dynamic_range=dynamic_range, overbright_factor=overbright_factor
-    )
+def main(
+    *,
+    paths: Sequence[pathlib.Path],
+    output_directory: Optional[pathlib.Path],
+    ldr_format: str,
+    hdr_format: str,
+    dynamic_range: Optional[ImageDynamicRange],
+    mipmaps: bool,
+    separate_channels: bool,
+    overbright_factor: float,
+    compress: Optional[bool],
+    write: Optional[bool],
+    readback: bool,
+    num_workers: Optional[int],
+    no_progress: bool,
+) -> None:
+    vtf_extension_pattern = re.compile(r"\.vtf$", re.ASCII | re.IGNORECASE)
+
+    texture_extractor = VtfExtractor()
+    texture_filter = VtfMipmapFilter(mipmap_levels=slice(-1, None)) if not mipmaps else None
+    texture_decoder = VtfDecoder(dynamic_range=dynamic_range, overbright_factor=overbright_factor)
+    texture_namer = Vtf2TgaLikeNamer(include_mipmap_level=mipmaps)
 
+    Pipeline.initialize()
     pipeline = Pipeline(
-        file_factory=file_factory,
+        input_extension_pattern=vtf_extension_pattern,
         ldr_format=ldr_format,
         hdr_format=hdr_format,
         separate_channels=separate_channels,
         compress=compress,
         write=write,
         readback=readback,
+        extractor=texture_extractor,
+        filter=texture_filter,
+        decoder=texture_decoder,
+        namer=texture_namer,
     )
 
-    pipeline_runner: PipelineRunner
+    input_paths = InputPaths(paths)
+    if input_paths.has_directories():
+        _resolve_directories(input_paths, not no_progress)
+
+    task_runner: TaskRunner
     if num_workers is None or num_workers > 1:
-        pipeline_runner = ParallelRunner(max_workers=num_workers)
+        task_runner = ParallelRunner(max_workers=num_workers, initializer=Pipeline.initialize)
     else:
-        pipeline_runner = SequentialRunner()
+        task_runner = SequentialRunner()
 
-    tasks = _get_tasks(directory_files_list, output_directory)
-    exit_status = _process_tasks(pipeline_runner, tasks, pipeline, not no_progress)
+    tasks = _get_tasks(pipeline, input_paths, output_directory)
+    exit_status = _process_tasks(task_runner, tasks, not no_progress)
     sys.exit(exit_status)
 
 
-def _global_config() -> None:
-    alive_progress.config_handler.set_global(spinner=None, theme="classic", enrich_print=False)
-
-
-def _resolve_files(directory_files_list: DirectoryFilesList, show_progress: bool) -> None:
-    progress_bar_manager = alive_progress.alive_bar(receipt=False) if show_progress else None
+def _resolve_directories(input_paths: InputPaths, show_progress: bool) -> None:
+    progress_bar_manager = (
+        alive_progress.alive_bar(receipt=False, spinner=None, theme="classic", enrich_print=False)
+        if show_progress
+        else None
+    )
     with progress_bar_manager or contextlib.nullcontext() as progress_bar:
-        for file in directory_files_list.search_in_directories("*.vtf"):
+        for file in input_paths.search_in_directories("*.[vV][tT][fF]", add_results=True):
             if progress_bar:
                 progress_bar.text = file.name
                 progress_bar()
+        input_paths.remove_directories()
 
 
 def _get_tasks(
-    directory_files_list: DirectoryFilesList,
+    pipeline: Pipeline[_T, ImageDataTypes],
+    input_paths: InputPaths,
     output_directory: Optional[pathlib.Path],
-) -> Sequence[Task]:
-    tasks: list[Task] = []
-    for directory_files in directory_files_list:
-        for file in directory_files.files:
-            file_root_output_directory = output_directory or directory_files.directory
-            file_relative_to_directory = file.relative_to(directory_files.directory)
-            file_relative_directory = file_relative_to_directory.parent
-            file_output_directory = file_root_output_directory / file_relative_directory
-            tasks.append(Task(input_file=file, output_directory=file_output_directory))
+) -> Sequence[_Task[_T]]:
+    output_directories = OutputDirectories(output_directory)
+
+    tasks: list[_Task[_T]] = []
+    for input_file, input_base_directory in input_paths:
+        output_directory = output_directories(input_file, input_base_directory)
+        task = _Task(pipeline=pipeline, input_file=input_file, output_directory=output_directory)
+        tasks.append(task)
     return tasks
 
 
 def _process_tasks(
-    pipeline_runner: PipelineRunner,
-    tasks: Sequence[Task],
-    pipeline: Pipeline[VtfTexture],
+    task_runner: TaskRunner,
+    tasks: Sequence[_Task[_T]],
     show_progress: bool,
 ) -> int:
     exit_status = 0
 
     num_files = len(tasks)
-    progress_bar_manager = alive_progress.alive_bar(num_files) if show_progress else None
+    progress_bar_manager = (
+        alive_progress.alive_bar(num_files, spinner=None, theme="classic", enrich_print=False)
+        if show_progress
+        else None
+    )
     with progress_bar_manager or contextlib.nullcontext() as progress_bar:
-        for result in pipeline_runner(pipeline, tasks):
-            if not result.exception:
+        for task, result in task_runner(tasks):
+            task = cast(_Task[_T], task)
+            if isinstance(result, Pipeline.Receipt):
                 if progress_bar:
-                    progress_bar()
-                    progress_bar.text = result.task.input_file.name
+                    skipped = not result.io_done
+                    progress_bar(skipped=skipped)
+                    progress_bar.text = str(task.input_file)
             else:
                 exit_status = 1
 
-                message = f'Error while processing "{result.task.input_file}": {result.exception}'
-                if result.exception.__cause__:
-                    message += f" ({result.exception.__cause__})"
+                exception: Exception = result
+                message = f"Error while processing {task!r}: {exception}"
+                if exception.__cause__:
+                    message += f" ({exception.__cause__})"
                 click.echo(message, file=sys.stderr)
 
     return exit_status
+
+
+@dataclass(frozen=True, kw_only=True)
+class _Task(Generic[_T], TaskRunner.Task[Pipeline.Receipt]):
+    pipeline: Pipeline[_T, ImageDataTypes]
+    input_file: pathlib.Path
+    output_directory: pathlib.Path
+
+    def __call__(self) -> Pipeline.Receipt:
+        return self.pipeline(self.input_file, output_directory=self.output_directory)
+
+    def __str__(self) -> str:
+        return f"{self.input_file}"
+
+    def __repr__(self) -> str:
+        return f"{self.input_file!r}"
```

### Comparing `no_vtf-2.0.1/no_vtf/namers/vtf.py` & `no_vtf-3.0.0/no_vtf/texture/namer/vtf.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,32 @@
-# Copyright (C) 2022 b5327157
+# SPDX-FileCopyrightText: b5327157 <b5327157@protonmail.com>
+#
 # SPDX-License-Identifier: LGPL-3.0-or-later
 
 from dataclasses import dataclass
 
-from no_vtf.namer import Namer
-from no_vtf.textures.vtf import VtfTexture
+from no_vtf.texture.namer.namer import TextureNamer
+from no_vtf.texture.vtf import VtfTexture
 
 
 @dataclass(frozen=True, kw_only=True)
-class VTF2TGALikeNamer(Namer[VtfTexture]):
+class Vtf2TgaLikeNamer(TextureNamer[VtfTexture]):
     include_mipmap_level: bool
 
-    def __call__(self, name_stem: str, texture: VtfTexture) -> str:
-        if texture.face_index is not None:
+    def __call__(self, input_name: str, texture: VtfTexture) -> str:
+        output_name = input_name
+
+        if texture.is_cubemap:
             face_names = ("rt", "lf", "bk", "ft", "up", "dn", "sph")
-            name_stem += face_names[texture.face_index]
+            output_name += face_names[texture.face_index]
 
-        if texture.frame_index is not None:
-            name_stem += f"{texture.frame_index:03d}"
+        if texture.num_frames > 1:
+            output_name += f"{texture.frame_index:03d}"
 
-        if self.include_mipmap_level:
-            name_stem += f"_mip{texture.mipmap_level}"
+        if self.include_mipmap_level and texture.num_mipmaps > 1:
+            mipmap_level = texture.num_mipmaps - texture.mipmap_index - 1
+            output_name += f"_mip{mipmap_level}"
 
-        if texture.slice_index is not None:
-            name_stem += f"_z{texture.slice_index:03d}"
+        if texture.num_slices > 1:
+            output_name += f"_z{texture.slice_index:03d}"
 
-        return name_stem
+        return output_name
```

### Comparing `no_vtf-2.0.1/no_vtf/parsers/generated/vtf.py` & `no_vtf-3.0.0/no_vtf/parser/generated/vtf.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # This is a generated file! Please edit source .ksy file and use kaitai-struct-compiler to rebuild
 
-from pkg_resources import parse_version
 import kaitaistruct
 from kaitaistruct import KaitaiStruct, KaitaiStream, BytesIO
 from enum import Enum
 
 
-if parse_version(kaitaistruct.__version__) < parse_version('0.9'):
+if getattr(kaitaistruct, 'API_VERSION', (0, 9)) < (0, 9):
     raise Exception("Incompatible Kaitai Struct Python API: 0.9 or later is required, but you have %s" % (kaitaistruct.__version__))
 
 class Vtf(KaitaiStruct):
     """
     .. seealso::
        Source - https://developer.valvesoftware.com/wiki/Valve_Texture_Format
     
@@ -77,17 +76,17 @@
             if  ((self._root.header.base.version.minor < 3) and (self._root.header.v7_0.low_res_image_format != Vtf.ImageFormat.none) and (self._root.header.v7_0.low_res_image_width != 0) and (self._root.header.v7_0.low_res_image_height != 0)) :
                 self.low_res_image = Vtf.Image(self._root.header.v7_0.low_res_image_width, self._root.header.v7_0.low_res_image_height, self._root.header.v7_0.low_res_image_format, self._io, self, self._root)
 
             if  ((self._root.header.base.version.minor < 3) and (self._root.header.v7_0.high_res_image_format != Vtf.ImageFormat.none)) :
                 self.high_res_image = Vtf.HighResImage(self._io, self, self._root)
 
             if self._root.header.base.version.minor >= 3:
-                self.resources = [None] * (self._root.header.logical.num_resources)
+                self.resources = []
                 for i in range(self._root.header.logical.num_resources):
-                    self.resources[i] = Vtf.Resource(self._io, self, self._root)
+                    self.resources.append(Vtf.Resource(self._io, self, self._root))
 
 
 
 
     class Image(KaitaiStruct):
         def __init__(self, logical_width, logical_height, image_format, _io, _parent=None, _root=None):
             self._io = _io
@@ -100,71 +99,71 @@
 
         def _read(self):
             self.image_data = self._io.read_bytes(((self.physical_width * self.physical_height) * self.bpp) // 8)
 
         @property
         def image_format_to_bpp(self):
             if hasattr(self, '_m_image_format_to_bpp'):
-                return self._m_image_format_to_bpp if hasattr(self, '_m_image_format_to_bpp') else None
+                return self._m_image_format_to_bpp
 
             self._m_image_format_to_bpp = Vtf.ImageFormatToBpp(self.image_format, self._io, self, self._root)
-            return self._m_image_format_to_bpp if hasattr(self, '_m_image_format_to_bpp') else None
+            return getattr(self, '_m_image_format_to_bpp', None)
 
         @property
         def physical_height(self):
             if hasattr(self, '_m_physical_height'):
-                return self._m_physical_height if hasattr(self, '_m_physical_height') else None
+                return self._m_physical_height
 
             self._m_physical_height = (self.logical_height if not (self.is_compressed) else (self.logical_height if self.logical_height >= 4 else 4))
-            return self._m_physical_height if hasattr(self, '_m_physical_height') else None
+            return getattr(self, '_m_physical_height', None)
 
         @property
         def is_compressed(self):
             if hasattr(self, '_m_is_compressed'):
-                return self._m_is_compressed if hasattr(self, '_m_is_compressed') else None
+                return self._m_is_compressed
 
             self._m_is_compressed = self.image_format_to_is_compressed.is_compressed_container.value
-            return self._m_is_compressed if hasattr(self, '_m_is_compressed') else None
+            return getattr(self, '_m_is_compressed', None)
 
         @property
         def bpp(self):
             if hasattr(self, '_m_bpp'):
-                return self._m_bpp if hasattr(self, '_m_bpp') else None
+                return self._m_bpp
 
             self._m_bpp = self.image_format_to_bpp.bpp_container.value
-            return self._m_bpp if hasattr(self, '_m_bpp') else None
+            return getattr(self, '_m_bpp', None)
 
         @property
         def physical_width(self):
             if hasattr(self, '_m_physical_width'):
-                return self._m_physical_width if hasattr(self, '_m_physical_width') else None
+                return self._m_physical_width
 
             self._m_physical_width = (self.logical_width if not (self.is_compressed) else (self.logical_width if self.logical_width >= 4 else 4))
-            return self._m_physical_width if hasattr(self, '_m_physical_width') else None
+            return getattr(self, '_m_physical_width', None)
 
         @property
         def image_format_to_is_compressed(self):
             if hasattr(self, '_m_image_format_to_is_compressed'):
-                return self._m_image_format_to_is_compressed if hasattr(self, '_m_image_format_to_is_compressed') else None
+                return self._m_image_format_to_is_compressed
 
             self._m_image_format_to_is_compressed = Vtf.ImageFormatToIsCompressed(self.image_format, self._io, self, self._root)
-            return self._m_image_format_to_is_compressed if hasattr(self, '_m_image_format_to_is_compressed') else None
+            return getattr(self, '_m_image_format_to_is_compressed', None)
 
 
     class ImageFace(KaitaiStruct):
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._read()
 
         def _read(self):
-            self.image_slices = [None] * (self._parent.num_slices)
+            self.image_slices = []
             for i in range(self._parent.num_slices):
-                self.image_slices[i] = Vtf.Image(self._parent.width, self._parent.height, self._parent.image_format, self._io, self._parent, self._root)
+                self.image_slices.append(Vtf.Image(self._parent.width, self._parent.height, self._parent.image_format, self._io, self._parent, self._root))
 
 
 
     class ImageFormatToIsCompressed(KaitaiStruct):
         def __init__(self, image_format, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
@@ -174,28 +173,28 @@
 
         def _read(self):
             pass
 
         @property
         def is_compressed_container(self):
             if hasattr(self, '_m_is_compressed_container'):
-                return self._m_is_compressed_container if hasattr(self, '_m_is_compressed_container') else None
+                return self._m_is_compressed_container
 
             _on = self.image_format
             if _on == Vtf.ImageFormat.dxt5:
                 self._m_is_compressed_container = Vtf.B1Container(True, self._io, self, self._root)
             elif _on == Vtf.ImageFormat.dxt1_onebitalpha:
                 self._m_is_compressed_container = Vtf.B1Container(True, self._io, self, self._root)
             elif _on == Vtf.ImageFormat.dxt1:
                 self._m_is_compressed_container = Vtf.B1Container(True, self._io, self, self._root)
             elif _on == Vtf.ImageFormat.dxt3:
                 self._m_is_compressed_container = Vtf.B1Container(True, self._io, self, self._root)
             else:
                 self._m_is_compressed_container = Vtf.B1Container(False, self._io, self, self._root)
-            return self._m_is_compressed_container if hasattr(self, '_m_is_compressed_container') else None
+            return getattr(self, '_m_is_compressed_container', None)
 
 
     class HeaderV72(KaitaiStruct):
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
@@ -231,34 +230,34 @@
 
         def _read(self):
             pass
 
         @property
         def onebitalpha(self):
             if hasattr(self, '_m_onebitalpha'):
-                return self._m_onebitalpha if hasattr(self, '_m_onebitalpha') else None
+                return self._m_onebitalpha
 
             self._m_onebitalpha = (True if (self._root.header.v7_0.flags & 4096) != 0 else False)
-            return self._m_onebitalpha if hasattr(self, '_m_onebitalpha') else None
+            return getattr(self, '_m_onebitalpha', None)
 
         @property
         def eightbitalpha(self):
             if hasattr(self, '_m_eightbitalpha'):
-                return self._m_eightbitalpha if hasattr(self, '_m_eightbitalpha') else None
+                return self._m_eightbitalpha
 
             self._m_eightbitalpha = (True if (self._root.header.v7_0.flags & 8192) != 0 else False)
-            return self._m_eightbitalpha if hasattr(self, '_m_eightbitalpha') else None
+            return getattr(self, '_m_eightbitalpha', None)
 
         @property
         def envmap(self):
             if hasattr(self, '_m_envmap'):
-                return self._m_envmap if hasattr(self, '_m_envmap') else None
+                return self._m_envmap
 
             self._m_envmap = (True if (self._root.header.v7_0.flags & 16384) != 0 else False)
-            return self._m_envmap if hasattr(self, '_m_envmap') else None
+            return getattr(self, '_m_envmap', None)
 
 
     class Version(KaitaiStruct):
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
@@ -281,31 +280,31 @@
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._read()
 
         def _read(self):
-            self.image_mipmaps = [None] * (self._root.header.v7_0.num_mipmaps)
+            self.image_mipmaps = []
             for i in range(self._root.header.v7_0.num_mipmaps):
-                self.image_mipmaps[i] = Vtf.ImageMipmap(i, self._io, self, self._root)
+                self.image_mipmaps.append(Vtf.ImageMipmap(i, self._io, self, self._root))
 
 
 
     class ImageFrame(KaitaiStruct):
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._read()
 
         def _read(self):
-            self.image_faces = [None] * (self._root.header.logical.num_faces)
+            self.image_faces = []
             for i in range(self._root.header.logical.num_faces):
-                self.image_faces[i] = Vtf.ImageFace(self._io, self._parent, self._root)
+                self.image_faces.append(Vtf.ImageFace(self._io, self._parent, self._root))
 
 
 
     class Resource(KaitaiStruct):
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
@@ -322,36 +321,36 @@
             if  ((True) and (self.tag != Vtf.ResourceTag.low_res_image) and (self.tag != Vtf.ResourceTag.high_res_image) and (self.tag != Vtf.ResourceTag.particle_sheet) and (self.tag != Vtf.ResourceTag.key_values_data)) :
                 self._unnamed3 = self._io.read_u4le()
 
 
         @property
         def high_res_image(self):
             if hasattr(self, '_m_high_res_image'):
-                return self._m_high_res_image if hasattr(self, '_m_high_res_image') else None
+                return self._m_high_res_image
 
             if  ((self.tag == Vtf.ResourceTag.high_res_image) and (self._root.header.v7_0.high_res_image_format != Vtf.ImageFormat.none)) :
                 _pos = self._io.pos()
                 self._io.seek(self.ofs_resource)
                 self._m_high_res_image = Vtf.HighResImage(self._io, self, self._root)
                 self._io.seek(_pos)
 
-            return self._m_high_res_image if hasattr(self, '_m_high_res_image') else None
+            return getattr(self, '_m_high_res_image', None)
 
         @property
         def low_res_image(self):
             if hasattr(self, '_m_low_res_image'):
-                return self._m_low_res_image if hasattr(self, '_m_low_res_image') else None
+                return self._m_low_res_image
 
             if  ((self.tag == Vtf.ResourceTag.low_res_image) and (self._root.header.v7_0.low_res_image_format != Vtf.ImageFormat.none)) :
                 _pos = self._io.pos()
                 self._io.seek(self.ofs_resource)
                 self._m_low_res_image = Vtf.Image(self._root.header.v7_0.low_res_image_width, self._root.header.v7_0.low_res_image_height, self._root.header.v7_0.low_res_image_format, self._io, self, self._root)
                 self._io.seek(_pos)
 
-            return self._m_low_res_image if hasattr(self, '_m_low_res_image') else None
+            return getattr(self, '_m_low_res_image', None)
 
 
     class Header(KaitaiStruct):
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
@@ -403,42 +402,42 @@
 
         def _read(self):
             pass
 
         @property
         def flags(self):
             if hasattr(self, '_m_flags'):
-                return self._m_flags if hasattr(self, '_m_flags') else None
+                return self._m_flags
 
             self._m_flags = Vtf.HeaderFlags(self._io, self, self._root)
-            return self._m_flags if hasattr(self, '_m_flags') else None
+            return getattr(self, '_m_flags', None)
 
         @property
         def num_faces(self):
             if hasattr(self, '_m_num_faces'):
-                return self._m_num_faces if hasattr(self, '_m_num_faces') else None
+                return self._m_num_faces
 
             self._m_num_faces = (1 if not (self.flags.envmap) else (6 if  ((self._root.header.base.version.minor < 1) or (self._root.header.base.version.minor > 4))  else (6 if self._root.header.v7_0.first_frame == 255 else 7)))
-            return self._m_num_faces if hasattr(self, '_m_num_faces') else None
+            return getattr(self, '_m_num_faces', None)
 
         @property
         def num_slices(self):
             if hasattr(self, '_m_num_slices'):
-                return self._m_num_slices if hasattr(self, '_m_num_slices') else None
+                return self._m_num_slices
 
             self._m_num_slices = (self._root.header.v7_2.num_slices if self._root.header.base.version.minor >= 2 else 1)
-            return self._m_num_slices if hasattr(self, '_m_num_slices') else None
+            return getattr(self, '_m_num_slices', None)
 
         @property
         def num_resources(self):
             if hasattr(self, '_m_num_resources'):
-                return self._m_num_resources if hasattr(self, '_m_num_resources') else None
+                return self._m_num_resources
 
             self._m_num_resources = (self._root.header.v7_3.num_resources if self._root.header.base.version.minor >= 3 else 0)
-            return self._m_num_resources if hasattr(self, '_m_num_resources') else None
+            return getattr(self, '_m_num_resources', None)
 
 
     class HeaderV70(KaitaiStruct):
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
@@ -451,17 +450,17 @@
             self.height = self._io.read_u2le()
             if not self.height >= 1:
                 raise kaitaistruct.ValidationLessThanError(1, self.height, self._io, u"/types/header_v7_0/seq/1")
             self.flags = self._io.read_u4le()
             self.num_frames = self._io.read_u2le()
             self.first_frame = self._io.read_u2le()
             self.reserved0 = self._io.read_bytes(4)
-            self.reflectivity = [None] * (3)
+            self.reflectivity = []
             for i in range(3):
-                self.reflectivity[i] = self._io.read_f4le()
+                self.reflectivity.append(self._io.read_f4le())
 
             self.reserved1 = self._io.read_bytes(4)
             self.bumpmap_scale = self._io.read_f4le()
             self.high_res_image_format = KaitaiStream.resolve_enum(Vtf.ImageFormat, self._io.read_u4le())
             self.num_mipmaps = self._io.read_u1()
             self.low_res_image_format = KaitaiStream.resolve_enum(Vtf.ImageFormat, self._io.read_u4le())
             self.low_res_image_width = self._io.read_u1()
@@ -490,15 +489,15 @@
 
         def _read(self):
             pass
 
         @property
         def bpp_container(self):
             if hasattr(self, '_m_bpp_container'):
-                return self._m_bpp_container if hasattr(self, '_m_bpp_container') else None
+                return self._m_bpp_container
 
             _on = self.image_format
             if _on == Vtf.ImageFormat.argb8888:
                 self._m_bpp_container = Vtf.U4Container(32, self._io, self, self._root)
             elif _on == Vtf.ImageFormat.bgra8888:
                 self._m_bpp_container = Vtf.U4Container(32, self._io, self, self._root)
             elif _on == Vtf.ImageFormat.abgr8888:
@@ -547,77 +546,77 @@
                 self._m_bpp_container = Vtf.U4Container(8, self._io, self, self._root)
             elif _on == Vtf.ImageFormat.rgb565:
                 self._m_bpp_container = Vtf.U4Container(16, self._io, self, self._root)
             elif _on == Vtf.ImageFormat.uv88:
                 self._m_bpp_container = Vtf.U4Container(16, self._io, self, self._root)
             elif _on == Vtf.ImageFormat.rgba16161616f:
                 self._m_bpp_container = Vtf.U4Container(64, self._io, self, self._root)
-            return self._m_bpp_container if hasattr(self, '_m_bpp_container') else None
+            return getattr(self, '_m_bpp_container', None)
 
 
     class ImageMipmap(KaitaiStruct):
         def __init__(self, mipmap_index, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self.mipmap_index = mipmap_index
             self._read()
 
         def _read(self):
-            self.image_frames = [None] * (self._root.header.v7_0.num_frames)
+            self.image_frames = []
             for i in range(self._root.header.v7_0.num_frames):
-                self.image_frames[i] = Vtf.ImageFrame(self._io, self, self._root)
+                self.image_frames.append(Vtf.ImageFrame(self._io, self, self._root))
 
 
         @property
         def height(self):
             if hasattr(self, '_m_height'):
-                return self._m_height if hasattr(self, '_m_height') else None
+                return self._m_height
 
             self._m_height = ((self._root.header.v7_0.height >> self.bit_shift) if (self._root.header.v7_0.height >> self.bit_shift) >= 1 else 1)
-            return self._m_height if hasattr(self, '_m_height') else None
+            return getattr(self, '_m_height', None)
 
         @property
         def image_format(self):
             if hasattr(self, '_m_image_format'):
-                return self._m_image_format if hasattr(self, '_m_image_format') else None
+                return self._m_image_format
 
             self._m_image_format = self._root.header.v7_0.high_res_image_format
-            return self._m_image_format if hasattr(self, '_m_image_format') else None
+            return getattr(self, '_m_image_format', None)
 
         @property
         def num_slices(self):
             if hasattr(self, '_m_num_slices'):
-                return self._m_num_slices if hasattr(self, '_m_num_slices') else None
+                return self._m_num_slices
 
             self._m_num_slices = ((self._root.header.logical.num_slices >> self.bit_shift) if (self._root.header.logical.num_slices >> self.bit_shift) >= 1 else 1)
-            return self._m_num_slices if hasattr(self, '_m_num_slices') else None
+            return getattr(self, '_m_num_slices', None)
 
         @property
         def width(self):
             if hasattr(self, '_m_width'):
-                return self._m_width if hasattr(self, '_m_width') else None
+                return self._m_width
 
             self._m_width = ((self._root.header.v7_0.width >> self.bit_shift) if (self._root.header.v7_0.width >> self.bit_shift) >= 1 else 1)
-            return self._m_width if hasattr(self, '_m_width') else None
+            return getattr(self, '_m_width', None)
 
         @property
         def bit_shift(self):
             if hasattr(self, '_m_bit_shift'):
-                return self._m_bit_shift if hasattr(self, '_m_bit_shift') else None
+                return self._m_bit_shift
 
             self._m_bit_shift = ((self._root.header.v7_0.num_mipmaps - self.mipmap_index) - 1)
-            return self._m_bit_shift if hasattr(self, '_m_bit_shift') else None
+            return getattr(self, '_m_bit_shift', None)
 
 
     @property
     def body(self):
         if hasattr(self, '_m_body'):
-            return self._m_body if hasattr(self, '_m_body') else None
+            return self._m_body
 
         _pos = self._io.pos()
         self._io.seek((self.header.base.header_size - (self.header.logical.num_resources * 8)))
         self._m_body = Vtf.Body(self._io, self, self._root)
         self._io.seek(_pos)
-        return self._m_body if hasattr(self, '_m_body') else None
+        return getattr(self, '_m_body', None)
```

### Comparing `no_vtf-2.0.1/no_vtf/pipeline.py` & `no_vtf-3.0.0/no_vtf/pipeline/pipeline.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,96 +1,152 @@
-# Copyright (C) 2022 b5327157
+# SPDX-FileCopyrightText: b5327157 <b5327157@protonmail.com>
+#
 # SPDX-License-Identifier: LGPL-3.0-or-later
 
+from __future__ import annotations
+
 import pathlib
+import re
 
 from dataclasses import dataclass
-from typing import Generic, Literal, Optional, TypeVar
-
-from no_vtf.channel_separator import ChannelSeparator
-from no_vtf.file import FileFactory
-from no_vtf.filesystem import FileAccessor
-from no_vtf.image import Image, ImageDataTypes
-from no_vtf.io import Io
-from no_vtf.ios.bytes_io import BytesIo
-from no_vtf.ios.imageio import Imageio
-from no_vtf.texture import Texture
+from typing import Generic, Literal, Optional, TypeVar, overload
 
-_TextureTypeVar = TypeVar("_TextureTypeVar", bound=Texture)
-_IoTypeVar = TypeVar("_IoTypeVar", contravariant=True)
+from no_vtf.image.channel_separator import ChannelSeparator
+from no_vtf.image.image import Image, ImageDataTypes
+from no_vtf.io.bytes import BytesIO
+from no_vtf.io.image import ImageIO
+from no_vtf.io.io import IO
+from no_vtf.texture.decoder.decoder import TextureDecoder
+from no_vtf.texture.extractor.extractor import TextureExtractor
+from no_vtf.texture.filter.filter import TextureFilter
+from no_vtf.texture.namer.namer import TextureNamer
+
+_A_contra = TypeVar("_A_contra", contravariant=True)
+_I = TypeVar("_I", bound=ImageDataTypes)
+_T = TypeVar("_T")
 
 
 @dataclass(frozen=True, kw_only=True)
-class Pipeline(Generic[_TextureTypeVar]):
-    FORMAT_RAW: Literal["raw"] = "raw"
-    FORMAT_SKIP: Literal["skip"] = "skip"
+class Pipeline(Generic[_T, _I]):
+    @dataclass(frozen=True, kw_only=True)
+    class Receipt:
+        io_done: bool
 
-    file_factory: FileFactory[_TextureTypeVar]
+    input_extension_pattern: Optional[re.Pattern[str]] = None
 
+    FORMAT_RAW: Literal["raw"] = "raw"
+    FORMAT_SKIP: Literal["skip"] = "skip"
     ldr_format: str
     hdr_format: str
 
     separate_channels: bool = False
 
     compress: Optional[bool] = None
 
     write: Optional[bool] = None
     readback: bool = False
 
-    def __post_init__(self) -> None:
-        Imageio.request_freeimage()
+    extractor: TextureExtractor[_T]
+    filter: Optional[TextureFilter[_T]]
+    decoder: TextureDecoder[_T, _I]
+    namer: TextureNamer[_T]
+
+    @classmethod
+    def initialize(cls) -> None:
+        IO.initialize()
+
+    @overload
+    def __call__(self, input_file: pathlib.Path, *, output_file: pathlib.Path) -> Pipeline.Receipt:
+        ...
+
+    @overload
+    def __call__(
+        self, input_file: pathlib.Path, *, output_directory: pathlib.Path
+    ) -> Pipeline.Receipt:
+        ...
+
+    def __call__(
+        self,
+        input_file: pathlib.Path,
+        *,
+        output_file: Optional[pathlib.Path] = None,
+        output_directory: Optional[pathlib.Path] = None,
+    ) -> Pipeline.Receipt:
+        io_done = False
+
+        textures = self.extractor(input_file)
+
+        if self.filter:
+            textures = self.filter(textures)
 
-    def __call__(self, input_file: pathlib.Path, output_directory: pathlib.Path) -> None:
-        texture_file = self.file_factory(input_file)
-        textures = texture_file.extract()
         for texture in textures:
-            image = texture_file.decode(texture)
-            dynamic_range = image.get_dynamic_range()
+            image = self.decoder(texture)
 
-            format = self.hdr_format if dynamic_range == "hdr" else self.ldr_format
-            if _compare_formats(format, self.FORMAT_SKIP):
+            image_format = self.hdr_format if image.dynamic_range == "hdr" else self.ldr_format
+            if _compare_formats(image_format, self.FORMAT_SKIP):
                 continue
 
-            name_stem = texture_file.name(texture)
-            output_name = name_stem + "." + format
-            output_path = output_directory / output_name
-
-            if _compare_formats(format, self.FORMAT_RAW):
-                bytes_io = BytesIo()
-                data = texture.get_data()
-                self._do_io(bytes_io, output_path, data)
+            texture_output_file = output_file
+            if texture_output_file is None:
+                assert output_directory is not None, "output path must be set"
+
+                input_name = input_file.name
+                if self.input_extension_pattern:
+                    input_name = re.sub(self.input_extension_pattern, "", input_name)
+
+                texture_name = self.namer(input_name, texture)
+                texture_output_name = texture_name + "." + image_format
+                texture_output_file = output_directory / texture_output_name
+
+            if _compare_formats(image_format, self.FORMAT_RAW):
+                assert image.raw, "image must have raw data set"
+                io_done = self._do_io(BytesIO(), texture_output_file, image.raw) or io_done
             else:
-                imageio = Imageio(format=format, compress=self.compress)
+                image_io = ImageIO(format=image_format, compress=self.compress)
                 if not self.separate_channels:
-                    self._do_io(imageio, output_path, image)
+                    io_done = self._do_io(image_io, texture_output_file, image) or io_done
                 else:
-                    self._separate_channels(imageio, output_path, image)
+                    io_done = (
+                        self._separate_channels(image_io, texture_output_file, image) or io_done
+                    )
+
+        return Pipeline.Receipt(io_done=io_done)
 
     def _separate_channels(
-        self, imageio: Imageio, path: pathlib.Path, image: Image[ImageDataTypes]
-    ) -> None:
+        self, image_io: ImageIO, path: pathlib.Path, image: Image[ImageDataTypes]
+    ) -> bool:
+        io_done = False
+
         channel_separator = ChannelSeparator()
         for image_separated in channel_separator(image):
             new_stem = path.stem + "_" + image_separated.channels
             new_path = path.with_stem(new_stem)
-            self._do_io(imageio, new_path, image_separated)
+            io_done = self._do_io(image_io, new_path, image_separated) or io_done
+
+        return io_done
+
+    def _do_io(self, io: IO[_A_contra], path: pathlib.Path, data: _A_contra) -> bool:
+        io_done = False
 
-    def _do_io(self, io: Io[_IoTypeVar], path: pathlib.Path, data: _IoTypeVar) -> None:
         if self.write is not False:
-            self._write(io, path, data)
+            io_done = self._write(io, path, data) or io_done
 
         if self.readback:
             io.readback(path, data)
+            io_done = True
+
+        return io_done
 
-    def _write(self, io: Io[_IoTypeVar], path: pathlib.Path, data: _IoTypeVar) -> None:
+    def _write(self, io: IO[_A_contra], path: pathlib.Path, data: _A_contra) -> bool:
+        assert self.write is not False, "_write() must not be called when writing is disabled"
         skip_existing = self.write is None
-        file_accessor = FileAccessor(
-            skip_existing=skip_existing,
-            mkdir_missing_parents=True,
-        )
+        if skip_existing and path.is_file():
+            return False
+
+        path.parent.mkdir(parents=True, exist_ok=True)
+        io.write(path, data)
 
-        if file_accessor(path):
-            io.write(path, data)
+        return True
 
 
 def _compare_formats(a: str, b: str) -> bool:
     return a.lower() == b.lower()
```

### Comparing `no_vtf-2.0.1/no_vtf.egg-info/PKG-INFO` & `no_vtf-3.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,47 @@
 Metadata-Version: 2.1
-Name: no-vtf
-Version: 2.0.1
+Name: no_vtf
+Version: 3.0.0
 Summary: Valve Texture Format Converter
 Home-page: https://sr.ht/~b5327157/no_vtf
 Author: b5327157
 Author-email: b5327157@protonmail.com
 License: GNU Lesser General Public License v3 or later (LGPLv3+)
+Project-URL: Download, https://sr.ht/~b5327157/no_vtf/#application-bundle
+Project-URL: Changelog, https://git.sr.ht/~b5327157/no_vtf/refs
 Project-URL: Mailing list, https://lists.sr.ht/~b5327157/no_vtf
 Project-URL: Ticket tracker, https://todo.sr.ht/~b5327157/no_vtf
+Project-URL: Wiki, https://developer.valvesoftware.com/wiki/no_vtf
 Keywords: Source Engine,VTF,Valve Texture Format
-Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Multimedia :: Graphics :: Graphics Conversion
+Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-License-File: LICENSE.md
+Provides-Extra: dev
+License-File: LICENSES/LGPL-3.0-or-later.txt
 
 # no_vtf
 
-Say no to .vtf – convert it to one of the standard image formats.
+Say no to [.vtf](https://developer.valvesoftware.com/wiki/Valve_Texture_Format) – convert it to one of the standard image formats.
 
-[![Badge showing package version on PyPI](https://img.shields.io/pypi/v/no_vtf?style=flat-square)](https://pypi.org/project/no-vtf/)
-[![Badge showing number of monthly downloads from PyPI](https://img.shields.io/pypi/dm/no_vtf?style=flat-square)](https://pypi.org/project/no-vtf/)
 ![Badge showing supported Python versions](https://img.shields.io/pypi/pyversions/no_vtf?style=flat-square)
+[![Badge showing package version on PyPI](https://img.shields.io/pypi/v/no_vtf?style=flat-square)](https://pypi.org/project/no-vtf/)
+[![Badge showing number of monthly downloads from PyPI](https://img.shields.io/pypi/dm/no_vtf?style=flat-square)](https://pypistats.org/packages/no-vtf)
+[![Badge showing source code repository hosted on SourceHut](https://img.shields.io/badge/sr.ht-repository-white?labelColor=212529&logo=data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiIHN0YW5kYWxvbmU9Im5vIj8+CjxzdmcKICAgdmlld0JveD0iMCAwIDUxMiA1MTIiCiAgIHZlcnNpb249IjEuMSIKICAgaWQ9InN2ZzUxIgogICBzb2RpcG9kaTpkb2NuYW1lPSJzb3VyY2VodXQtd2hpdGUuc3ZnIgogICBpbmtzY2FwZTp2ZXJzaW9uPSIxLjEgKGM2OGUyMmMzODcsIDIwMjEtMDUtMjMpIgogICB4bWxuczppbmtzY2FwZT0iaHR0cDovL3d3dy5pbmtzY2FwZS5vcmcvbmFtZXNwYWNlcy9pbmtzY2FwZSIKICAgeG1sbnM6c29kaXBvZGk9Imh0dHA6Ly9zb2RpcG9kaS5zb3VyY2Vmb3JnZS5uZXQvRFREL3NvZGlwb2RpLTAuZHRkIgogICB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciCiAgIHhtbG5zOnN2Zz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPgogIDxkZWZzCiAgICAgaWQ9ImRlZnM1NSIgLz4KICA8c29kaXBvZGk6bmFtZWR2aWV3CiAgICAgaWQ9Im5hbWVkdmlldzUzIgogICAgIHBhZ2Vjb2xvcj0iIzUwNTA1MCIKICAgICBib3JkZXJjb2xvcj0iI2ZmZmZmZiIKICAgICBib3JkZXJvcGFjaXR5PSIxIgogICAgIGlua3NjYXBlOnBhZ2VzaGFkb3c9IjAiCiAgICAgaW5rc2NhcGU6cGFnZW9wYWNpdHk9IjAiCiAgICAgaW5rc2NhcGU6cGFnZWNoZWNrZXJib2FyZD0iMSIKICAgICBzaG93Z3JpZD0iZmFsc2UiCiAgICAgaW5rc2NhcGU6em9vbT0iMS42NTQyOTY5IgogICAgIGlua3NjYXBlOmN4PSIyNTYiCiAgICAgaW5rc2NhcGU6Y3k9IjI1NiIKICAgICBpbmtzY2FwZTp3aW5kb3ctd2lkdGg9IjE5MjAiCiAgICAgaW5rc2NhcGU6d2luZG93LWhlaWdodD0iMTA1OSIKICAgICBpbmtzY2FwZTp3aW5kb3cteD0iMCIKICAgICBpbmtzY2FwZTp3aW5kb3cteT0iMCIKICAgICBpbmtzY2FwZTp3aW5kb3ctbWF4aW1pemVkPSIxIgogICAgIGlua3NjYXBlOmN1cnJlbnQtbGF5ZXI9InN2ZzUxIiAvPgogIDxwYXRoCiAgICAgZD0iTTI1NiA4QzExOSA4IDggMTE5IDggMjU2czExMSAyNDggMjQ4IDI0OCAyNDgtMTExIDI0OC0yNDhTMzkzIDggMjU2IDh6bTAgNDQ4Yy0xMTAuNSAwLTIwMC04OS41LTIwMC0yMDBTMTQ1LjUgNTYgMjU2IDU2czIwMCA4OS41IDIwMCAyMDAtODkuNSAyMDAtMjAwIDIwMHoiCiAgICAgaWQ9InBhdGg0OSIKICAgICBzdHlsZT0iZmlsbDojZmZmZmZmIiAvPgo8L3N2Zz4K)](https://sr.ht/~b5327157/no_vtf)
+[![Badge showing builds.sr.ht status](https://builds.sr.ht/~b5327157/no_vtf.svg?search=tags:master)](https://builds.sr.ht/~b5327157/no_vtf?search=tags:master)
+[![Badge showing REUSE compliance status](https://api.reuse.software/badge/git.sr.ht/~b5327157/no_vtf)](https://api.reuse.software/info/git.sr.ht/~b5327157/no_vtf)
+[![Badge showing Nox as the chosen Python automation toolkit](https://img.shields.io/badge/🦊-Nox-D85E00.svg)](https://github.com/wntrblm/nox)
 
 ![Screencast showing conversion of sprays downloaded in Team Fortress 2 using no_vtf](https://git.sr.ht/~b5327157/no_vtf/blob/HEAD/resources/docs/screencast.gif)
 
 ## Motivation
 
 - cross-platform – runs on any machine where Python is supported
 - console-only – runs without a graphical interface
@@ -111,15 +120,15 @@
 no_vtf --help
 ```
 
 ## Supported formats
 
 ### Input
 
-All textures installed with Team Fortress 2 and Source Filmmaker can be converted with the supported format set.
+All textures installed with [Team Fortress 2](https://store.steampowered.com/app/440/Team_Fortress_2/), [Source Filmmaker](https://store.steampowered.com/app/1840/Source_Filmmaker/) and [Portal 2](https://store.steampowered.com/app/620/Portal_2/) can be converted with the supported format set.
 
 - `RGBA8888`
 - `ABGR8888`
 - `RGB888`
 - `BGR888`
 - `I8`
 - `IA88`
@@ -217,9 +226,7 @@
 ### Pre-build steps
 
 ```
 # compile .ksy files (requires Kaitai Struct compiler)
 # only necessary if a .ksy file was modified
 ksy/compile.sh
 ```
-
-
```

### Comparing `no_vtf-2.0.1/no_vtf.egg-info/SOURCES.txt` & `no_vtf-3.0.0/no_vtf.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 .build.yml
 .gitignore
-LICENSE.md
 MANIFEST.in
 README.md
+README.md.license
 noxfile.py
 pyproject.toml
 setup.cfg
+.reuse/dep5
+LICENSES/CC-BY-4.0.txt
+LICENSES/CC0-1.0.txt
+LICENSES/GPL-3.0-or-later.txt
+LICENSES/LGPL-3.0-or-later.txt
 builds/common
 builds/diff_generated.sh
 builds/nox.sh
 builds/nox_wine.sh
 builds/python3.10-install.sh
 builds/verify_signatures.sh
 builds/with_clone.sh
@@ -20,63 +25,66 @@
 builds/debian/python3.10-build_dep.sh
 builds/debian/wine-install.sh
 ksy/compile.sh
 ksy/vtf.ksy
 no_vtf/__init__.py
 no_vtf/__main__.py
 no_vtf/_version.py
-no_vtf/channel_separator.py
-no_vtf/deferrable.py
-no_vtf/extractor.py
-no_vtf/file.py
-no_vtf/filesystem.py
-no_vtf/filter.py
-no_vtf/image.py
-no_vtf/io.py
 no_vtf/main.py
-no_vtf/namer.py
-no_vtf/ndarray.py
-no_vtf/pipeline.py
-no_vtf/pipeline_runner.py
-no_vtf/postprocessor.py
 no_vtf/py.typed
-no_vtf/texture.py
 no_vtf.egg-info/PKG-INFO
 no_vtf.egg-info/SOURCES.txt
 no_vtf.egg-info/dependency_links.txt
 no_vtf.egg-info/entry_points.txt
 no_vtf.egg-info/not-zip-safe
 no_vtf.egg-info/requires.txt
 no_vtf.egg-info/top_level.txt
-no_vtf/decoder/__init__.py
-no_vtf/decoder/image.py
-no_vtf/decoder/texture.py
-no_vtf/decoders/__init__.py
-no_vtf/decoders/image/__init__.py
-no_vtf/decoders/image/generic.py
-no_vtf/decoders/image/vtf.py
-no_vtf/decoders/texture/__init__.py
-no_vtf/decoders/texture/vtf.py
-no_vtf/extractors/__init__.py
-no_vtf/extractors/vtf.py
-no_vtf/files/__init__.py
-no_vtf/files/vtf.py
-no_vtf/filters/__init__.py
-no_vtf/filters/vtf.py
-no_vtf/ios/__init__.py
-no_vtf/ios/bytes_io.py
-no_vtf/ios/imageio.py
-no_vtf/namers/__init__.py
-no_vtf/namers/vtf.py
-no_vtf/parsers/__init__.py
-no_vtf/parsers/generated/__init__.py
-no_vtf/parsers/generated/vtf.py
-no_vtf/pipeline_runners/__init__.py
-no_vtf/pipeline_runners/parallel_runner.py
-no_vtf/pipeline_runners/sequential_runner.py
-no_vtf/postprocessors/__init__.py
-no_vtf/postprocessors/fp_precision_modifier.py
-no_vtf/textures/__init__.py
-no_vtf/textures/vtf.py
+no_vtf/deferred/__init__.py
+no_vtf/deferred/deferred.py
+no_vtf/filesystem/__init__.py
+no_vtf/filesystem/input_paths.py
+no_vtf/filesystem/output_directories.py
+no_vtf/image/__init__.py
+no_vtf/image/channel_separator.py
+no_vtf/image/image.py
+no_vtf/image/ndarray.py
+no_vtf/image/decoder/__init__.py
+no_vtf/image/decoder/decoder.py
+no_vtf/image/decoder/generic.py
+no_vtf/image/decoder/vtf.py
+no_vtf/image/modifier/__init__.py
+no_vtf/image/modifier/fp_precision_modifier.py
+no_vtf/image/modifier/modifier.py
+no_vtf/io/__init__.py
+no_vtf/io/bytes.py
+no_vtf/io/image.py
+no_vtf/io/io.py
+no_vtf/parser/__init__.py
+no_vtf/parser/generated/__init__.py
+no_vtf/parser/generated/vtf.py
+no_vtf/parser/generated/vtf.py.license
+no_vtf/pipeline/__init__.py
+no_vtf/pipeline/pipeline.py
+no_vtf/task_runner/__init__.py
+no_vtf/task_runner/parallel.py
+no_vtf/task_runner/sequential.py
+no_vtf/task_runner/task_runner.py
+no_vtf/texture/__init__.py
+no_vtf/texture/vtf.py
+no_vtf/texture/decoder/__init__.py
+no_vtf/texture/decoder/decoder.py
+no_vtf/texture/decoder/vtf.py
+no_vtf/texture/extractor/__init__.py
+no_vtf/texture/extractor/extractor.py
+no_vtf/texture/extractor/vtf.py
+no_vtf/texture/filter/__init__.py
+no_vtf/texture/filter/filter.py
+no_vtf/texture/filter/vtf.py
+no_vtf/texture/namer/__init__.py
+no_vtf/texture/namer/namer.py
+no_vtf/texture/namer/vtf.py
 resources/docs/screencast.gif
+resources/docs/screencast.gif.license
 resources/pyinstaller/empty.ico
-resources/pyinstaller/no_vtf.desktop
+resources/pyinstaller/empty.ico.license
+resources/pyinstaller/no_vtf.desktop
+resources/pyinstaller/no_vtf.desktop.license
```

### Comparing `no_vtf-2.0.1/noxfile.py` & `no_vtf-3.0.0/noxfile.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,71 +1,84 @@
-# Copyright (C) 2022 b5327157
+# SPDX-FileCopyrightText: b5327157 <b5327157@protonmail.com>
+#
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 from __future__ import annotations
 
 import itertools
 import os
 import pathlib
 import shutil
 import tempfile
 
+from collections.abc import Iterator, Sequence
 from contextlib import contextmanager
 from dataclasses import dataclass
-from typing import Iterator, List, Optional, Sequence
+from typing import Optional
 
 import nox
 
-nox.needs_version = ">= 2022.1.7"
+nox.needs_version = ">= 2023.4.22"
 
 nox.options.default_venv_backend = "venv"
 nox.options.error_on_external_run = True
 nox.options.error_on_missing_interpreters = True
 nox.options.sessions = ["lint"]
 
 
 @nox.session(python="3.10")
 def lint(session: nox.Session) -> None:
-    session.install("black[colorama] >= 22.3.0, < 23")
-    session.install("flake8 >= 4.0.1, < 5")
-    session.install("flake8-deprecated >= 1.3, < 2")
-    session.install("isort[colors] >= 5.10.1, < 6")
-    session.install("mypy >= 0.941, < 1")
-    session.install("nox >= 2022.1.7, < 2023")
-    session.install("pep8-naming >= 0.12.1, < 1")
+    session.install("black[colorama] >= 23.3.0, < 24")
+    session.install("flake8 >= 6.0.0, < 7")
+    session.install("flake8-builtins >= 2.1.0, < 3")
+    session.install("flake8-deprecated >= 2.0.1, < 3")
+    session.install("flake8-pep585 >= 0.1.7, < 1")
+    session.install("isort[colors] >= 5.12.0, < 6")
+    session.install("mypy >= 1.3.0, < 2")
+    session.install("nox >= 2023.4.22, < 2024")
+    session.install("pep8-naming >= 0.13.3, < 1")
+    session.install("reuse >= 1.1.2, < 2")
 
-    session.install(".")
+    session.install("types-Pillow >= 9.5.0.4, < 10")
+
+    session.install(".[dev]")
 
     posargs_paths = session.posargs
     fix = False
     if posargs_paths and posargs_paths[0] == "--fix":
         posargs_paths = posargs_paths[1:]
         fix = True
 
     paths = ["no_vtf", "noxfile.py"]
     if posargs_paths:
         paths = posargs_paths
 
     if not fix:
+        session.run("reuse", "lint", silent=True)
         session.run("mypy", "--pretty", "--show-error-context", *paths)
         session.run("flake8", *paths)
         session.run("isort", "--check", "--diff", *paths)
         session.run("black", "--check", "--diff", *paths)
     else:
         session.run("isort", *paths)
         session.run("black", *paths)
 
 
 @nox.session(python="3.10")
 def package(session: nox.Session) -> None:
-    session.install("build >= 0.7.0, < 1")
+    path_dist = pathlib.Path("dist")
+    if path_dist.is_dir():
+        dist_files = [path for path in path_dist.iterdir() if path.is_file()]
+        for dist_file in dist_files:
+            dist_file.unlink()
+
+    session.install("build >= 0.10.0, < 1")
 
     session.run("python", "-m", "build", silent=True)
 
-    path_dist = pathlib.Path("dist")
     path_sdist = next(path_dist.glob("*.tar.gz"))
     path_wheel = next(path_dist.glob("*.whl"))
 
     # run even with the --no-install flag
     session.run("pip", "install", str(path_wheel), silent=True)
 
     executable = ["python", "-m", "no_vtf"]
@@ -79,15 +92,18 @@
 
     if len(session.posargs) >= 2:
         shutil.copy2(path_wheel, session.posargs[1])
 
 
 @nox.session(python="3.10")
 def freeze(session: nox.Session) -> None:
-    session.install("pyinstaller >= 4.9, < 5")
+    root_dir = pathlib.Path("dist")
+    base_dir = pathlib.Path("no_vtf")
+
+    session.install("pyinstaller >= 5.11.0, < 6")
 
     # installing in editable mode will ensure the _version.py file is generated by setuptools_scm
     # run even with the --no-install flag
     session.run("pip", "install", "-e", ".", silent=True)
 
     session.run("imageio_download_bin", "--package-dir", silent=True)
 
@@ -100,43 +116,30 @@
 
     if os.name == "posix":
         pyinstaller_datas.append(("resources/pyinstaller/no_vtf.desktop", "."))
 
     # https://github.com/rsalmei/alive-progress/issues/123
     pyinstaller_args.extend(["--collect-data", "grapheme"])
 
-    # https://github.com/imageio/imageio/issues/690#issuecomment-974605991
-    # plugin list: imageio/docs/conf.py
-    pyinstaller_args.extend(["--hidden-import", "imageio.plugins.bsdf"])
-    pyinstaller_args.extend(["--hidden-import", "imageio.plugins.dicom"])
-    pyinstaller_args.extend(["--hidden-import", "imageio.plugins.feisem"])
-    pyinstaller_args.extend(["--hidden-import", "imageio.plugins.ffmpeg"])
-    pyinstaller_args.extend(["--hidden-import", "imageio.plugins.fits"])
-    pyinstaller_args.extend(["--hidden-import", "imageio.plugins.freeimage"])
-    pyinstaller_args.extend(["--hidden-import", "imageio.plugins.gdal"])
-    pyinstaller_args.extend(["--hidden-import", "imageio.plugins.lytro"])
-    pyinstaller_args.extend(["--hidden-import", "imageio.plugins.npz"])
-    pyinstaller_args.extend(["--hidden-import", "imageio.plugins.pillow_legacy"])
-    pyinstaller_args.extend(["--hidden-import", "imageio.plugins.simpleitk"])
-    pyinstaller_args.extend(["--hidden-import", "imageio.plugins.spe"])
-    pyinstaller_args.extend(["--hidden-import", "imageio.plugins.swf"])
-
     # bundle plugin binary dependencies downloaded by imageio_download_bin
     pyinstaller_args.extend(["--collect-binaries", "imageio"])
 
     pyinstaller_args.append("--noconfirm")
     pyinstaller_args.append("--clean")
 
     for pyinstaller_data in pyinstaller_datas:
         pyinstaller_args.extend(["--add-data", os.pathsep.join(pyinstaller_data)])
 
     session.run("pyinstaller", *pyinstaller_args, "no_vtf/__main__.py")
-    shutil.rmtree("dist/no_vtf/imageio/resources/images", ignore_errors=True)
+    shutil.rmtree(root_dir / base_dir / "imageio/resources/images", ignore_errors=True)
+
+    executable = str(root_dir / base_dir / "no_vtf")
+    if os.name == "nt":
+        executable += ".exe"
 
-    executable = "dist/no_vtf/no_vtf"
     paths = ["."]
     nox.command.run([executable, "--version"], paths=paths, external=True)
 
     with SanityTest.with_archived_samples(session, [executable], paths) as sanity_test:
         sanity_test.readback()
 
     if not session.posargs:
@@ -148,23 +151,23 @@
     if (archive_base_name := archive_path.removesuffix(".tar.xz")) != archive_path:
         archive_format = "xztar"
     elif (archive_base_name := archive_path.removesuffix(".zip")) != archive_path:
         archive_format = "zip"
     else:
         raise RuntimeError("Unsupported archive format")
 
-    shutil.make_archive(archive_base_name, archive_format, root_dir="dist", base_dir="no_vtf")
+    shutil.make_archive(archive_base_name, archive_format, root_dir=root_dir, base_dir=base_dir)
 
 
 @nox.session(python="3.10")
 def publish(session: nox.Session) -> None:
     if not session.posargs:
         session.error("Path to API token file was not provided")
 
-    session.install("twine >= 4.0.0, < 5")
+    session.install("twine >= 4.0.2, < 5")
 
     dist = pathlib.Path("dist")
     dist_files = [path for path in dist.iterdir() if path.is_file()]
     dist_args = [str(path) for path in dist_files]
 
     session.run("twine", "check", "--strict", *dist_args)
 
@@ -192,40 +195,46 @@
 
     # run even with the --no-install flag
     session.run("pip", "install", ".", silent=True)
 
     executable = ["python", "-m", "no_vtf"]
 
     base_path = pathlib.Path(session.posargs[0])
-    input = base_path / "input"
-    output = base_path / "output"
+    input_path = base_path / "input"
+    output_path = base_path / "output"
 
-    sanity_test = SanityTest(session=session, executable=executable, input=input, output=output)
+    sanity_test = SanityTest(
+        session=session, executable=executable, input=input_path, output=output_path
+    )
     sanity_test.write()
 
 
 @dataclass(frozen=True, kw_only=True)
 class SanityTest:
     session: nox.Session
     executable: Sequence[str]
-    paths: Optional[List[str]] = None
+    paths: Optional[list[str]] = None
 
     input: pathlib.Path
     output: pathlib.Path
 
     @classmethod
     @contextmanager
     def with_archived_samples(
-        cls, session: nox.Session, executable: Sequence[str], paths: Optional[List[str]] = None
+        cls, session: nox.Session, executable: Sequence[str], paths: Optional[list[str]] = None
     ) -> Iterator[SanityTest]:
         with samples_archive_view() as samples_directory:
-            input = samples_directory / "input"
-            output = samples_directory / "output"
+            input_path = samples_directory / "input"
+            output_path = samples_directory / "output"
             sanity_test = cls(
-                session=session, executable=executable, paths=paths, input=input, output=output
+                session=session,
+                executable=executable,
+                paths=paths,
+                input=input_path,
+                output=output_path,
             )
             yield sanity_test
 
     def write(self) -> None:
         args: list[str] = []
         args.append("--always-write")
         args.append("--no-compress")
@@ -284,10 +293,14 @@
             shutil.unpack_archive(archive, view_directory)
         yield pathlib.Path(view_directory)
 
 
 @contextmanager
 def samples_archive_view() -> Iterator[pathlib.Path]:
     samples_path = pathlib.Path("resources/test/samples")
-    sample_archives = [path for path in samples_path.iterdir() if path.is_file()]
+    sample_archives = [
+        path
+        for path in samples_path.iterdir()
+        if path.is_file() and not str(path).endswith(".license")
+    ]
     with archives_view(sample_archives) as samples_directory:
         yield samples_directory
```

### Comparing `no_vtf-2.0.1/resources/docs/screencast.gif` & `no_vtf-3.0.0/resources/docs/screencast.gif`

 * *Files identical despite different names*

### Comparing `no_vtf-2.0.1/setup.cfg` & `no_vtf-3.0.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,63 +1,73 @@
 [metadata]
 author = b5327157
 author_email = b5327157@protonmail.com
 classifiers = 
+	Development Status :: 5 - Production/Stable
 	Environment :: Console
 	Intended Audience :: End Users/Desktop
 	License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Topic :: Multimedia :: Graphics :: Graphics Conversion
+	Typing :: Typed
 description = Valve Texture Format Converter
 keywords = 
 	Source Engine
 	VTF
 	Valve Texture Format
 license = GNU Lesser General Public License v3 or later (LGPLv3+)
 license_files = 
-	LICENSE.md
+	LICENSES/LGPL-3.0-or-later.txt
 long_description = file: README.md
 long_description_content_type = text/markdown
 name = no_vtf
 project_urls = 
+	Download = https://sr.ht/~b5327157/no_vtf/#application-bundle
+	Changelog = https://git.sr.ht/~b5327157/no_vtf/refs
 	Mailing list = https://lists.sr.ht/~b5327157/no_vtf
 	Ticket tracker = https://todo.sr.ht/~b5327157/no_vtf
+	Wiki = https://developer.valvesoftware.com/wiki/no_vtf
 url = https://sr.ht/~b5327157/no_vtf
 
 [options]
 install_requires = 
-	alive-progress >= 2.3.1, < 3
-	click >= 8.0.3, < 9
-	imageio[pillow] >= 2.13.5, < 3
-	kaitaistruct >= 0.9, < 1
-	numpy >= 1.22.1, < 2
-	Pillow >= 9.0.0, < 10
-	tifffile >= 2022.3.16, < 2023
+	alive-progress >= 3.1.3, < 4
+	click >= 8.1.3, < 9
+	imageio[pillow] >= 2.29.0, < 3
+	kaitaistruct >= 0.10, < 1
+	numpy >= 1.24.3, < 2
+	Pillow >= 9.5.0, < 10
+	tifffile >= 2023.4.12, < 2024
 packages = find:
+py_modules = 
 python_requires = >= 3.10
 zip_safe = False
 
 [options.entry_points]
 console_scripts = 
-	no_vtf = no_vtf.main:main
+	no_vtf = no_vtf.__main__:_main
+
+[options.extras_require]
+dev = 
+	coverage[toml] >= 7.2.7, < 8
 
 [options.packages.find]
 include = 
 	no_vtf
 	no_vtf.*
 
 [flake8]
 exclude = 
 	generated
 extend-ignore = 
 	E203
-format = pylint
+	A003
 max_complexity = 10
 max_line_length = 100
 show_source = True
 
 [isort]
 atomic = True
 color_output = True
@@ -88,28 +98,26 @@
 [mypy-*.generated.*]
 ignore_errors = True
 
 [mypy-alive_progress.*]
 ignore_missing_imports = True
 
 [mypy-imageio.*]
-ignore_missing_imports = True
+implicit_reexport = True
 
 [mypy-kaitaistruct.*]
 ignore_missing_imports = True
 
-[mypy-PIL.*]
-ignore_missing_imports = True
-
 [pycodestyle]
 exclude = 
 	generated
 format = pylint
 ignore = 
 	E203
+	A003
 max_line_length = 100
 show_source = True
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

