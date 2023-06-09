# Comparing `tmp/xpydf-0.1.5.tar.gz` & `tmp/xpydf-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpydf-0.1.5.tar", last modified: Fri Jun  2 10:44:33 2023, max compression
+gzip compressed data, was "xpydf-0.1.6.tar", last modified: Fri Jun  9 10:59:30 2023, max compression
```

## Comparing `xpydf-0.1.5.tar` & `xpydf-0.1.6.tar`

### file list

```diff
@@ -1,805 +1,807 @@
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.578279 xpydf-0.1.5/
--rw-r--r--   0 matthijs   (501) staff       (20)    35149 2023-02-17 12:43:21.000000 xpydf-0.1.5/LICENSE
--rw-r--r--   0 matthijs   (501) staff       (20)      118 2023-06-02 09:36:35.000000 xpydf-0.1.5/MANIFEST.in
--rw-r--r--   0 matthijs   (501) staff       (20)      844 2023-06-02 10:44:33.578115 xpydf-0.1.5/PKG-INFO
--rw-r--r--   0 matthijs   (501) staff       (20)      240 2023-04-12 11:54:25.000000 xpydf-0.1.5/README.md
--rw-r--r--   0 matthijs   (501) staff       (20)      785 2023-06-02 10:44:05.000000 xpydf-0.1.5/pyproject.toml
--rw-r--r--   0 matthijs   (501) staff       (20)       38 2023-06-02 10:44:33.578323 xpydf-0.1.5/setup.cfg
--rw-r--r--   0 matthijs   (501) staff       (20)     1998 2023-06-02 09:36:35.000000 xpydf-0.1.5/setup.py
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.342865 xpydf-0.1.5/src/
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.348239 xpydf-0.1.5/src/freetype/
--rw-r--r--   0 matthijs   (501) staff       (20)     8196 2023-05-23 14:26:17.000000 xpydf-0.1.5/src/freetype/.DS_Store
--rw-r--r--   0 matthijs   (501) staff       (20)      453 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/.clang-format
--rw-r--r--   0 matthijs   (501) staff       (20)       40 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/.git
--rw-r--r--   0 matthijs   (501) staff       (20)       94 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/.gitignore
--rw-r--r--   0 matthijs   (501) staff       (20)     7021 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/.gitlab-ci.yml
--rw-r--r--   0 matthijs   (501) staff       (20)       84 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/.gitmodules
--rw-r--r--   0 matthijs   (501) staff       (20)     1821 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/.mailmap
--rw-r--r--   0 matthijs   (501) staff       (20)    21367 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/CMakeLists.txt
--rw-r--r--   0 matthijs   (501) staff       (20)     2074 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/LICENSE.TXT
--rw-r--r--   0 matthijs   (501) staff       (20)      846 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/Makefile
--rw-r--r--   0 matthijs   (501) staff       (20)     3114 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/README
--rw-r--r--   0 matthijs   (501) staff       (20)     3154 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/README.git
--rwxr-xr-x   0 matthijs   (501) staff       (20)     4768 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/autogen.sh
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.330042 xpydf-0.1.5/src/freetype/builds/
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.348792 xpydf-0.1.5/src/freetype/builds/mac/
--rwxr-xr-x   0 matthijs   (501) staff       (20)     1033 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/builds/mac/ascii2mpw.py
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.350218 xpydf-0.1.5/src/freetype/builds/meson/
--rw-r--r--   0 matthijs   (501) staff       (20)     3019 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/builds/meson/extract_freetype_version.py
--rw-r--r--   0 matthijs   (501) staff       (20)     2906 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/builds/meson/extract_libtool_version.py
--rw-r--r--   0 matthijs   (501) staff       (20)     2317 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/builds/meson/generate_reference_docs.py
--rw-r--r--   0 matthijs   (501) staff       (20)     4596 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/builds/meson/parse_modules_cfg.py
--rw-r--r--   0 matthijs   (501) staff       (20)     3403 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/builds/meson/process_ftoption_h.py
--rw-r--r--   0 matthijs   (501) staff       (20)     1633 2023-05-22 06:59:42.000000 xpydf-0.1.5/src/freetype/config.mk
--rwxr-xr-x   0 matthijs   (501) staff       (20)     4029 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/configure
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.350406 xpydf-0.1.5/src/freetype/include/
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.350843 xpydf-0.1.5/src/freetype/include/dlg/
--rw-r--r--   0 matthijs   (501) staff       (20)    10834 2023-05-22 06:59:35.000000 xpydf-0.1.5/src/freetype/include/dlg/dlg.h
--rw-r--r--   0 matthijs   (501) staff       (20)     7229 2023-05-22 06:59:35.000000 xpydf-0.1.5/src/freetype/include/dlg/output.h
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.361265 xpydf-0.1.5/src/freetype/include/freetype/
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.362866 xpydf-0.1.5/src/freetype/include/freetype/config/
--rw-r--r--   0 matthijs   (501) staff       (20)     1614 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/config/ftconfig.h
--rw-r--r--   0 matthijs   (501) staff       (20)    23919 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/config/ftheader.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1443 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/config/ftmodule.h
--rw-r--r--   0 matthijs   (501) staff       (20)    39628 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/config/ftoption.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4576 2023-05-23 14:26:12.000000 xpydf-0.1.5/src/freetype/include/freetype/config/ftstdlib.h
--rw-r--r--   0 matthijs   (501) staff       (20)     7072 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/config/integer-types.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1597 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/config/mac-support.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4207 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/config/public-macros.h
--rw-r--r--   0 matthijs   (501) staff       (20)   178794 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/freetype.h
--rw-r--r--   0 matthijs   (501) staff       (20)     5470 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/ftadvanc.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2638 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/ftbbox.h
--rw-r--r--   0 matthijs   (501) staff       (20)     5322 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/ftbdf.h
--rw-r--r--   0 matthijs   (501) staff       (20)     9051 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/ftbitmap.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2786 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/ftbzip2.h
--rw-r--r--   0 matthijs   (501) staff       (20)    34179 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/ftcache.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2933 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/ftchapters.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4022 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/ftcid.h
--rw-r--r--   0 matthijs   (501) staff       (20)    50199 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/ftcolor.h
--rw-r--r--   0 matthijs   (501) staff       (20)    47533 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/ftdriver.h
--rw-r--r--   0 matthijs   (501) staff       (20)    12559 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/fterrdef.h
--rw-r--r--   0 matthijs   (501) staff       (20)     9301 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/fterrors.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2213 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/ftfntfmt.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4138 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/ftgasp.h
--rw-r--r--   0 matthijs   (501) staff       (20)    20912 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/ftglyph.h
--rw-r--r--   0 matthijs   (501) staff       (20)    10625 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/ftgxval.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4211 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/ftgzip.h
--rw-r--r--   0 matthijs   (501) staff       (20)    41833 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/ftimage.h
--rw-r--r--   0 matthijs   (501) staff       (20)    10696 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/ftincrem.h
--rw-r--r--   0 matthijs   (501) staff       (20)    11744 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/ftlcdfil.h
--rw-r--r--   0 matthijs   (501) staff       (20)     7100 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/ftlist.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4130 2023-05-23 14:26:12.000000 xpydf-0.1.5/src/freetype/include/freetype/ftlogging.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2768 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/ftlzw.h
--rw-r--r--   0 matthijs   (501) staff       (20)     7771 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/ftmac.h
--rw-r--r--   0 matthijs   (501) staff       (20)    23797 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/ftmm.h
--rw-r--r--   0 matthijs   (501) staff       (20)    22544 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/ftmodapi.h
--rw-r--r--   0 matthijs   (501) staff       (20)     6675 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/ftmoderr.h
--rw-r--r--   0 matthijs   (501) staff       (20)     5346 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/ftotval.h
--rw-r--r--   0 matthijs   (501) staff       (20)    17402 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/ftoutln.h
--rw-r--r--   0 matthijs   (501) staff       (20)     6041 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/ftparams.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4908 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/ftpfr.h
--rw-r--r--   0 matthijs   (501) staff       (20)     6625 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/ftrender.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4288 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/ftsizes.h
--rw-r--r--   0 matthijs   (501) staff       (20)     7730 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/ftsnames.h
--rw-r--r--   0 matthijs   (501) staff       (20)    21773 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/ftstroke.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4483 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/ftsynth.h
--rw-r--r--   0 matthijs   (501) staff       (20)     8502 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/ftsystem.h
--rw-r--r--   0 matthijs   (501) staff       (20)     7411 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/fttrigon.h
--rw-r--r--   0 matthijs   (501) staff       (20)    14735 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/fttypes.h
--rw-r--r--   0 matthijs   (501) staff       (20)     7965 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/ftwinfnt.h
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.367644 xpydf-0.1.5/src/freetype/include/freetype/internal/
--rw-r--r--   0 matthijs   (501) staff       (20)     7498 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/autohint.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2354 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/cffotypes.h
--rw-r--r--   0 matthijs   (501) staff       (20)    11866 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/cfftypes.h
--rw-r--r--   0 matthijs   (501) staff       (20)    11499 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/compiler-macros.h
--rw-r--r--   0 matthijs   (501) staff       (20)    15606 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/ftcalc.h
--rw-r--r--   0 matthijs   (501) staff       (20)    13332 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/ftdebug.h
--rw-r--r--   0 matthijs   (501) staff       (20)     9214 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/ftdrv.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4504 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/ftgloadr.h
--rw-r--r--   0 matthijs   (501) staff       (20)     3242 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/fthash.h
--rw-r--r--   0 matthijs   (501) staff       (20)    15961 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/ftmemory.h
--rw-r--r--   0 matthijs   (501) staff       (20)     3003 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/ftmmtypes.h
--rw-r--r--   0 matthijs   (501) staff       (20)    42481 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/ftobjs.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1130 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/ftpsprop.h
--rw-r--r--   0 matthijs   (501) staff       (20)     7651 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/ftrfork.h
--rw-r--r--   0 matthijs   (501) staff       (20)    24053 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/ftserv.h
--rw-r--r--   0 matthijs   (501) staff       (20)    23230 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/ftstream.h
--rw-r--r--   0 matthijs   (501) staff       (20)     5918 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/fttrace.h
--rw-r--r--   0 matthijs   (501) staff       (20)     5762 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/ftvalid.h
--rw-r--r--   0 matthijs   (501) staff       (20)    43241 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/psaux.h
--rw-r--r--   0 matthijs   (501) staff       (20)    20852 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/pshints.h
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.374573 xpydf-0.1.5/src/freetype/include/freetype/internal/services/
--rw-r--r--   0 matthijs   (501) staff       (20)     1731 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/services/svbdf.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2832 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/services/svcfftl.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2124 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/services/svcid.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1348 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/services/svfntfmt.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1865 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/services/svgldict.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1730 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/services/svgxval.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1080 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/services/svkern.h
--rw-r--r--   0 matthijs   (501) staff       (20)     3996 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/services/svmetric.h
--rw-r--r--   0 matthijs   (501) staff       (20)     8956 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/services/svmm.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1253 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/services/svotval.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1570 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/services/svpfr.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1571 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/services/svpostnm.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1677 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/services/svprop.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4272 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/services/svpscmap.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2469 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/services/svpsinfo.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2079 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/services/svsfnt.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2397 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/services/svttcmap.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1007 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/services/svtteng.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1251 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/services/svttglyf.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1017 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/services/svwinfnt.h
--rw-r--r--   0 matthijs   (501) staff       (20)    32444 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/sfnt.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1041 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/svginterface.h
--rw-r--r--   0 matthijs   (501) staff       (20)     8208 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/t1types.h
--rw-r--r--   0 matthijs   (501) staff       (20)    52695 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/tttypes.h
--rw-r--r--   0 matthijs   (501) staff       (20)     8010 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/internal/wofftypes.h
--rw-r--r--   0 matthijs   (501) staff       (20)    10457 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/otsvg.h
--rw-r--r--   0 matthijs   (501) staff       (20)    23188 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/t1tables.h
--rw-r--r--   0 matthijs   (501) staff       (20)    58769 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/ttnameid.h
--rw-r--r--   0 matthijs   (501) staff       (20)    25227 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/tttables.h
--rw-r--r--   0 matthijs   (501) staff       (20)     5145 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/freetype/tttags.h
--rw-r--r--   0 matthijs   (501) staff       (20)      990 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/include/ft2build.h
--rw-r--r--   0 matthijs   (501) staff       (20)    13071 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/meson.build
--rw-r--r--   0 matthijs   (501) staff       (20)     1518 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/meson_options.txt
--rw-r--r--   0 matthijs   (501) staff       (20)     6490 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/modules.cfg
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.342132 xpydf-0.1.5/src/freetype/src/
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.387536 xpydf-0.1.5/src/freetype/src/autofit/
--rw-r--r--   0 matthijs   (501) staff       (20)    76975 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/autofit/afblue.c
--rw-r--r--   0 matthijs   (501) staff       (20)    16937 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/autofit/afblue.h
--rw-r--r--   0 matthijs   (501) staff       (20)    66667 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/autofit/afcjk.c
--rw-r--r--   0 matthijs   (501) staff       (20)     4211 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/autofit/afcjk.h
--rw-r--r--   0 matthijs   (501) staff       (20)     3159 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/autofit/afcover.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2160 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/autofit/afdummy.c
--rw-r--r--   0 matthijs   (501) staff       (20)      877 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/autofit/afdummy.h
--rw-r--r--   0 matthijs   (501) staff       (20)      984 2023-05-22 06:46:50.000000 xpydf-0.1.5/src/freetype/src/autofit/aferrors.h
--rw-r--r--   0 matthijs   (501) staff       (20)    13736 2023-05-23 09:51:54.000000 xpydf-0.1.5/src/freetype/src/autofit/afglobal.c
--rw-r--r--   0 matthijs   (501) staff       (20)     5110 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/autofit/afglobal.h
--rw-r--r--   0 matthijs   (501) staff       (20)    47282 2023-05-23 14:26:12.000000 xpydf-0.1.5/src/freetype/src/autofit/afhints.c
--rw-r--r--   0 matthijs   (501) staff       (20)    15948 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/autofit/afhints.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4719 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/autofit/afindic.c
--rw-r--r--   0 matthijs   (501) staff       (20)      840 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/autofit/afindic.h
--rw-r--r--   0 matthijs   (501) staff       (20)   113850 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/autofit/aflatin.c
--rw-r--r--   0 matthijs   (501) staff       (20)     6784 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/autofit/aflatin.h
--rw-r--r--   0 matthijs   (501) staff       (20)    24004 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/autofit/afloader.c
--rw-r--r--   0 matthijs   (501) staff       (20)     2269 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/autofit/afloader.h
--rw-r--r--   0 matthijs   (501) staff       (20)    13961 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/autofit/afmodule.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1181 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/autofit/afmodule.h
--rw-r--r--   0 matthijs   (501) staff       (20)    34997 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/autofit/afranges.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1083 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/autofit/afranges.h
--rw-r--r--   0 matthijs   (501) staff       (20)    11464 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/autofit/afscript.h
--rw-r--r--   0 matthijs   (501) staff       (20)    20127 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/autofit/afshaper.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1655 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/autofit/afshaper.h
--rw-r--r--   0 matthijs   (501) staff       (20)    15115 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/autofit/afstyles.h
--rw-r--r--   0 matthijs   (501) staff       (20)    18624 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/autofit/aftypes.h
--rw-r--r--   0 matthijs   (501) staff       (20)      872 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/autofit/afws-decl.h
--rw-r--r--   0 matthijs   (501) staff       (20)      966 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/autofit/afws-iter.h
--rw-r--r--   0 matthijs   (501) staff       (20)      832 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/autofit/autofit.c
--rw-r--r--   0 matthijs   (501) staff       (20)     3310 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/autofit/ft-hb.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1463 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/autofit/ft-hb.h
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.396044 xpydf-0.1.5/src/freetype/src/base/
--rw-r--r--   0 matthijs   (501) staff       (20)     4906 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/base/ftadvanc.c
--rw-r--r--   0 matthijs   (501) staff       (20)      980 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/base/ftbase.c
--rw-r--r--   0 matthijs   (501) staff       (20)     2651 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/base/ftbase.h
--rw-r--r--   0 matthijs   (501) staff       (20)    14346 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/base/ftbbox.c
--rw-r--r--   0 matthijs   (501) staff       (20)     2177 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/base/ftbdf.c
--rw-r--r--   0 matthijs   (501) staff       (20)    28296 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/base/ftbitmap.c
--rw-r--r--   0 matthijs   (501) staff       (20)    28205 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/base/ftcalc.c
--rw-r--r--   0 matthijs   (501) staff       (20)     2540 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/base/ftcid.c
--rw-r--r--   0 matthijs   (501) staff       (20)     3416 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/base/ftcolor.c
--rw-r--r--   0 matthijs   (501) staff       (20)    23926 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/base/ftdbgmem.c
--rw-r--r--   0 matthijs   (501) staff       (20)    14105 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/base/ftdebug.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1267 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/base/fterrors.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1203 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/base/ftfntfmt.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1551 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/base/ftfstype.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1355 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/base/ftgasp.c
--rw-r--r--   0 matthijs   (501) staff       (20)    11421 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/base/ftgloadr.c
--rw-r--r--   0 matthijs   (501) staff       (20)    24220 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/base/ftglyph.c
--rw-r--r--   0 matthijs   (501) staff       (20)     3125 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/base/ftgxval.c
--rw-r--r--   0 matthijs   (501) staff       (20)     6657 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/base/fthash.c
--rw-r--r--   0 matthijs   (501) staff       (20)     6339 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/base/ftinit.c
--rw-r--r--   0 matthijs   (501) staff       (20)    11455 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/base/ftlcdfil.c
--rw-r--r--   0 matthijs   (501) staff       (20)    31521 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/base/ftmac.c
--rw-r--r--   0 matthijs   (501) staff       (20)    18084 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/base/ftmm.c
--rw-r--r--   0 matthijs   (501) staff       (20)   161883 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/base/ftobjs.c
--rw-r--r--   0 matthijs   (501) staff       (20)     2216 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/base/ftotval.c
--rw-r--r--   0 matthijs   (501) staff       (20)    28599 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/base/ftoutln.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1245 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/base/ftpatent.c
--rw-r--r--   0 matthijs   (501) staff       (20)     3730 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/base/ftpfr.c
--rw-r--r--   0 matthijs   (501) staff       (20)     7500 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/base/ftpsprop.c
--rw-r--r--   0 matthijs   (501) staff       (20)    29493 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/base/ftrfork.c
--rw-r--r--   0 matthijs   (501) staff       (20)     4580 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/base/ftsnames.c
--rw-r--r--   0 matthijs   (501) staff       (20)    19273 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/base/ftstream.c
--rw-r--r--   0 matthijs   (501) staff       (20)    64724 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/base/ftstroke.c
--rw-r--r--   0 matthijs   (501) staff       (20)     5374 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/base/ftsynth.c
--rw-r--r--   0 matthijs   (501) staff       (20)     8149 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/base/ftsystem.c
--rw-r--r--   0 matthijs   (501) staff       (20)    10565 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/base/fttrigon.c
--rw-r--r--   0 matthijs   (501) staff       (20)     3047 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/base/fttype1.c
--rw-r--r--   0 matthijs   (501) staff       (20)    10171 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/base/ftutil.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1306 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/base/ftwinfnt.c
--rw-r--r--   0 matthijs   (501) staff       (20)     8743 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/base/md5.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1410 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/base/md5.h
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.397103 xpydf-0.1.5/src/freetype/src/bdf/
--rw-r--r--   0 matthijs   (501) staff       (20)     1234 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/bdf/bdf.c
--rw-r--r--   0 matthijs   (501) staff       (20)     8121 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/bdf/bdf.h
--rw-r--r--   0 matthijs   (501) staff       (20)    29163 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/bdf/bdfdrivr.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1772 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/bdf/bdfdrivr.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1584 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/bdf/bdferror.h
--rw-r--r--   0 matthijs   (501) staff       (20)    68231 2023-05-23 14:26:12.000000 xpydf-0.1.5/src/freetype/src/bdf/bdflib.c
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.397375 xpydf-0.1.5/src/freetype/src/bzip2/
--rw-r--r--   0 matthijs   (501) staff       (20)    12870 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/bzip2/ftbzip2.c
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.400579 xpydf-0.1.5/src/freetype/src/cache/
--rw-r--r--   0 matthijs   (501) staff       (20)      771 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cache/ftcache.c
--rw-r--r--   0 matthijs   (501) staff       (20)    18033 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cache/ftcbasic.c
--rw-r--r--   0 matthijs   (501) staff       (20)    14006 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cache/ftccache.c
--rw-r--r--   0 matthijs   (501) staff       (20)    15484 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cache/ftccache.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2220 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cache/ftccback.h
--rw-r--r--   0 matthijs   (501) staff       (20)     9711 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cache/ftccmap.c
--rw-r--r--   0 matthijs   (501) staff       (20)      999 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cache/ftcerror.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4964 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cache/ftcglyph.c
--rw-r--r--   0 matthijs   (501) staff       (20)    11116 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cache/ftcglyph.h
--rw-r--r--   0 matthijs   (501) staff       (20)     3677 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cache/ftcimage.c
--rw-r--r--   0 matthijs   (501) staff       (20)     2675 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cache/ftcimage.h
--rw-r--r--   0 matthijs   (501) staff       (20)    17267 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cache/ftcmanag.c
--rw-r--r--   0 matthijs   (501) staff       (20)     5734 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cache/ftcmanag.h
--rw-r--r--   0 matthijs   (501) staff       (20)     6868 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cache/ftcmru.c
--rw-r--r--   0 matthijs   (501) staff       (20)     8525 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cache/ftcmru.h
--rw-r--r--   0 matthijs   (501) staff       (20)    11958 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cache/ftcsbits.c
--rw-r--r--   0 matthijs   (501) staff       (20)     2191 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cache/ftcsbits.h
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.403617 xpydf-0.1.5/src/freetype/src/cff/
--rw-r--r--   0 matthijs   (501) staff       (20)      725 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cff/cff.c
--rw-r--r--   0 matthijs   (501) staff       (20)     7312 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cff/cffcmap.c
--rw-r--r--   0 matthijs   (501) staff       (20)     2181 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cff/cffcmap.h
--rw-r--r--   0 matthijs   (501) staff       (20)    39514 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cff/cffdrivr.c
--rw-r--r--   0 matthijs   (501) staff       (20)      752 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cff/cffdrivr.h
--rw-r--r--   0 matthijs   (501) staff       (20)      959 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cff/cfferrs.h
--rw-r--r--   0 matthijs   (501) staff       (20)    26335 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cff/cffgload.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1523 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cff/cffgload.h
--rw-r--r--   0 matthijs   (501) staff       (20)    75411 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cff/cffload.c
--rw-r--r--   0 matthijs   (501) staff       (20)     3298 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cff/cffload.h
--rw-r--r--   0 matthijs   (501) staff       (20)    35405 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cff/cffobjs.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1940 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cff/cffobjs.h
--rw-r--r--   0 matthijs   (501) staff       (20)    39397 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cff/cffparse.c
--rw-r--r--   0 matthijs   (501) staff       (20)     3326 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cff/cffparse.h
--rw-r--r--   0 matthijs   (501) staff       (20)     6772 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cff/cfftoken.h
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.407887 xpydf-0.1.5/src/freetype/src/cid/
--rw-r--r--   0 matthijs   (501) staff       (20)      958 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cid/ciderrs.h
--rw-r--r--   0 matthijs   (501) staff       (20)    20567 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cid/cidgload.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1456 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cid/cidgload.h
--rw-r--r--   0 matthijs   (501) staff       (20)    25446 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cid/cidload.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1115 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cid/cidload.h
--rw-r--r--   0 matthijs   (501) staff       (20)    13878 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cid/cidobjs.c
--rw-r--r--   0 matthijs   (501) staff       (20)     3412 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cid/cidobjs.h
--rw-r--r--   0 matthijs   (501) staff       (20)     8770 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cid/cidparse.c
--rw-r--r--   0 matthijs   (501) staff       (20)     3518 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cid/cidparse.h
--rw-r--r--   0 matthijs   (501) staff       (20)     7557 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cid/cidriver.c
--rw-r--r--   0 matthijs   (501) staff       (20)      772 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cid/cidriver.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4387 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cid/cidtoken.h
--rw-r--r--   0 matthijs   (501) staff       (20)      710 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/cid/type1cid.c
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.408446 xpydf-0.1.5/src/freetype/src/dlg/
--rw-r--r--   0 matthijs   (501) staff       (20)    21039 2023-05-22 06:59:35.000000 xpydf-0.1.5/src/freetype/src/dlg/dlg.c
--rw-r--r--   0 matthijs   (501) staff       (20)      762 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/dlg/dlgwrap.c
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.414876 xpydf-0.1.5/src/freetype/src/gxvalid/
--rw-r--r--   0 matthijs   (501) staff       (20)     1133 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gxvalid/gxvalid.c
--rw-r--r--   0 matthijs   (501) staff       (20)     2869 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gxvalid/gxvalid.h
--rw-r--r--   0 matthijs   (501) staff       (20)     9637 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gxvalid/gxvbsln.c
--rw-r--r--   0 matthijs   (501) staff       (20)    54281 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gxvalid/gxvcommn.c
--rw-r--r--   0 matthijs   (501) staff       (20)    22980 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gxvalid/gxvcommn.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1333 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gxvalid/gxverror.h
--rw-r--r--   0 matthijs   (501) staff       (20)     9949 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gxvalid/gxvfeat.c
--rw-r--r--   0 matthijs   (501) staff       (20)     6054 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gxvalid/gxvfeat.h
--rw-r--r--   0 matthijs   (501) staff       (20)    13317 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gxvalid/gxvfgen.c
--rw-r--r--   0 matthijs   (501) staff       (20)    20588 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gxvalid/gxvjust.c
--rw-r--r--   0 matthijs   (501) staff       (20)    27203 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gxvalid/gxvkern.c
--rw-r--r--   0 matthijs   (501) staff       (20)     7139 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gxvalid/gxvlcar.c
--rw-r--r--   0 matthijs   (501) staff       (20)     8348 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gxvalid/gxvmod.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1093 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gxvalid/gxvmod.h
--rw-r--r--   0 matthijs   (501) staff       (20)     8297 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gxvalid/gxvmort.c
--rw-r--r--   0 matthijs   (501) staff       (20)     2971 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gxvalid/gxvmort.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4329 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gxvalid/gxvmort0.c
--rw-r--r--   0 matthijs   (501) staff       (20)     8122 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gxvalid/gxvmort1.c
--rw-r--r--   0 matthijs   (501) staff       (20)    10023 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gxvalid/gxvmort2.c
--rw-r--r--   0 matthijs   (501) staff       (20)     3760 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gxvalid/gxvmort4.c
--rw-r--r--   0 matthijs   (501) staff       (20)     8009 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gxvalid/gxvmort5.c
--rw-r--r--   0 matthijs   (501) staff       (20)     5208 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gxvalid/gxvmorx.c
--rw-r--r--   0 matthijs   (501) staff       (20)     2076 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gxvalid/gxvmorx.h
--rw-r--r--   0 matthijs   (501) staff       (20)     3126 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gxvalid/gxvmorx0.c
--rw-r--r--   0 matthijs   (501) staff       (20)     8464 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gxvalid/gxvmorx1.c
--rw-r--r--   0 matthijs   (501) staff       (20)    10356 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gxvalid/gxvmorx2.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1674 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gxvalid/gxvmorx4.c
--rw-r--r--   0 matthijs   (501) staff       (20)     7285 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gxvalid/gxvmorx5.c
--rw-r--r--   0 matthijs   (501) staff       (20)     7216 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gxvalid/gxvopbd.c
--rw-r--r--   0 matthijs   (501) staff       (20)    10208 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gxvalid/gxvprop.c
--rw-r--r--   0 matthijs   (501) staff       (20)     9558 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gxvalid/gxvtrak.c
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.419535 xpydf-0.1.5/src/freetype/src/gzip/
--rw-r--r--   0 matthijs   (501) staff       (20)     5182 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gzip/adler32.c
--rw-r--r--   0 matthijs   (501) staff       (20)    32225 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gzip/crc32.c
--rw-r--r--   0 matthijs   (501) staff       (20)   591749 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gzip/crc32.h
--rw-r--r--   0 matthijs   (501) staff       (20)    20073 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gzip/ftgzip.c
--rw-r--r--   0 matthijs   (501) staff       (20)    16625 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gzip/ftzconf.h
--rw-r--r--   0 matthijs   (501) staff       (20)     6843 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gzip/gzguts.h
--rw-r--r--   0 matthijs   (501) staff       (20)    12933 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gzip/inffast.c
--rw-r--r--   0 matthijs   (501) staff       (20)      434 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gzip/inffast.h
--rw-r--r--   0 matthijs   (501) staff       (20)     6332 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gzip/inffixed.h
--rw-r--r--   0 matthijs   (501) staff       (20)    56083 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gzip/inflate.c
--rw-r--r--   0 matthijs   (501) staff       (20)     6745 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gzip/inflate.h
--rw-r--r--   0 matthijs   (501) staff       (20)    12993 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gzip/inftrees.c
--rw-r--r--   0 matthijs   (501) staff       (20)     3000 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gzip/inftrees.h
--rw-r--r--   0 matthijs   (501) staff       (20)    98004 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gzip/zlib.h
--rw-r--r--   0 matthijs   (501) staff       (20)     7355 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gzip/zutil.c
--rw-r--r--   0 matthijs   (501) staff       (20)     7398 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/gzip/zutil.h
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.421626 xpydf-0.1.5/src/freetype/src/lzw/
--rw-r--r--   0 matthijs   (501) staff       (20)     9899 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/lzw/ftlzw.c
--rw-r--r--   0 matthijs   (501) staff       (20)    10565 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/lzw/ftzopen.c
--rw-r--r--   0 matthijs   (501) staff       (20)     5099 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/lzw/ftzopen.h
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.424677 xpydf-0.1.5/src/freetype/src/otvalid/
--rw-r--r--   0 matthijs   (501) staff       (20)      773 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/otvalid/otvalid.c
--rw-r--r--   0 matthijs   (501) staff       (20)     2127 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/otvalid/otvalid.h
--rw-r--r--   0 matthijs   (501) staff       (20)     7882 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/otvalid/otvbase.c
--rw-r--r--   0 matthijs   (501) staff       (20)    27533 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/otvalid/otvcommn.c
--rw-r--r--   0 matthijs   (501) staff       (20)    19343 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/otvalid/otvcommn.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1017 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/otvalid/otverror.h
--rw-r--r--   0 matthijs   (501) staff       (20)     8882 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/otvalid/otvgdef.c
--rw-r--r--   0 matthijs   (501) staff       (20)    29663 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/otvalid/otvgpos.c
--rw-r--r--   0 matthijs   (501) staff       (20)      786 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/otvalid/otvgpos.h
--rw-r--r--   0 matthijs   (501) staff       (20)    18463 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/otvalid/otvgsub.c
--rw-r--r--   0 matthijs   (501) staff       (20)     7126 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/otvalid/otvjstf.c
--rw-r--r--   0 matthijs   (501) staff       (20)    13656 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/otvalid/otvmath.c
--rw-r--r--   0 matthijs   (501) staff       (20)     7207 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/otvalid/otvmod.c
--rw-r--r--   0 matthijs   (501) staff       (20)      778 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/otvalid/otvmod.h
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.426505 xpydf-0.1.5/src/freetype/src/pcf/
--rw-r--r--   0 matthijs   (501) staff       (20)     1253 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/pcf/pcf.c
--rw-r--r--   0 matthijs   (501) staff       (20)     6373 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/pcf/pcf.h
--rw-r--r--   0 matthijs   (501) staff       (20)    21798 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/pcf/pcfdrivr.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1358 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/pcf/pcfdrivr.h
--rw-r--r--   0 matthijs   (501) staff       (20)      959 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/pcf/pcferror.h
--rw-r--r--   0 matthijs   (501) staff       (20)    50270 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/pcf/pcfread.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1361 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/pcf/pcfread.h
--rw-r--r--   0 matthijs   (501) staff       (20)     3382 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/pcf/pcfutil.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1649 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/pcf/pcfutil.h
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.430082 xpydf-0.1.5/src/freetype/src/pfr/
--rw-r--r--   0 matthijs   (501) staff       (20)      708 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/pfr/pfr.c
--rw-r--r--   0 matthijs   (501) staff       (20)     4519 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/pfr/pfrcmap.c
--rw-r--r--   0 matthijs   (501) staff       (20)      920 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/pfr/pfrcmap.h
--rw-r--r--   0 matthijs   (501) staff       (20)     5618 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/pfr/pfrdrivr.c
--rw-r--r--   0 matthijs   (501) staff       (20)      773 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/pfr/pfrdrivr.h
--rw-r--r--   0 matthijs   (501) staff       (20)      962 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/pfr/pfrerror.h
--rw-r--r--   0 matthijs   (501) staff       (20)    21931 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/pfr/pfrgload.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1059 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/pfr/pfrgload.h
--rw-r--r--   0 matthijs   (501) staff       (20)    28988 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/pfr/pfrload.c
--rw-r--r--   0 matthijs   (501) staff       (20)     3425 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/pfr/pfrload.h
--rw-r--r--   0 matthijs   (501) staff       (20)    17487 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/pfr/pfrobjs.c
--rw-r--r--   0 matthijs   (501) staff       (20)     2135 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/pfr/pfrobjs.h
--rw-r--r--   0 matthijs   (501) staff       (20)    21398 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/pfr/pfrsbit.c
--rw-r--r--   0 matthijs   (501) staff       (20)      878 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/pfr/pfrsbit.h
--rw-r--r--   0 matthijs   (501) staff       (20)     8090 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/pfr/pfrtypes.h
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.438413 xpydf-0.1.5/src/freetype/src/psaux/
--rw-r--r--   0 matthijs   (501) staff       (20)    25277 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/psaux/afmparse.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1825 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/psaux/afmparse.h
--rw-r--r--   0 matthijs   (501) staff       (20)    68657 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/psaux/cffdecode.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1825 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/psaux/cffdecode.h
--rw-r--r--   0 matthijs   (501) staff       (20)     6515 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/psaux/psarrst.c
--rw-r--r--   0 matthijs   (501) staff       (20)     3476 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/psaux/psarrst.h
--rw-r--r--   0 matthijs   (501) staff       (20)      945 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/psaux/psaux.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1003 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/psaux/psauxerr.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4847 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/psaux/psauxmod.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1247 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/psaux/psauxmod.h
--rw-r--r--   0 matthijs   (501) staff       (20)    19898 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/psaux/psblues.c
--rw-r--r--   0 matthijs   (501) staff       (20)     5995 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/psaux/psblues.h
--rw-r--r--   0 matthijs   (501) staff       (20)    11649 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/psaux/psconv.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1700 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/psaux/psconv.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2089 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/psaux/pserror.c
--rw-r--r--   0 matthijs   (501) staff       (20)     4024 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/psaux/pserror.h
--rw-r--r--   0 matthijs   (501) staff       (20)     3743 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/psaux/psfixed.h
--rw-r--r--   0 matthijs   (501) staff       (20)    19883 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/psaux/psfont.c
--rw-r--r--   0 matthijs   (501) staff       (20)     5402 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/psaux/psfont.h
--rw-r--r--   0 matthijs   (501) staff       (20)    25620 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/psaux/psft.c
--rw-r--r--   0 matthijs   (501) staff       (20)     5394 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/psaux/psft.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4501 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/psaux/psglue.h
--rw-r--r--   0 matthijs   (501) staff       (20)    66109 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/psaux/pshints.c
--rw-r--r--   0 matthijs   (501) staff       (20)     9869 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/psaux/pshints.h
--rw-r--r--   0 matthijs   (501) staff       (20)   105884 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/psaux/psintrp.c
--rw-r--r--   0 matthijs   (501) staff       (20)     3074 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/psaux/psintrp.h
--rw-r--r--   0 matthijs   (501) staff       (20)    66473 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/psaux/psobjs.c
--rw-r--r--   0 matthijs   (501) staff       (20)    10283 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/psaux/psobjs.h
--rw-r--r--   0 matthijs   (501) staff       (20)     3522 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/psaux/psread.c
--rw-r--r--   0 matthijs   (501) staff       (20)     2299 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/psaux/psread.h
--rw-r--r--   0 matthijs   (501) staff       (20)     9233 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/psaux/psstack.c
--rw-r--r--   0 matthijs   (501) staff       (20)     3695 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/psaux/psstack.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2674 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/psaux/pstypes.h
--rw-r--r--   0 matthijs   (501) staff       (20)    11948 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/psaux/t1cmap.c
--rw-r--r--   0 matthijs   (501) staff       (20)     3282 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/psaux/t1cmap.h
--rw-r--r--   0 matthijs   (501) staff       (20)    60726 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/psaux/t1decode.c
--rw-r--r--   0 matthijs   (501) staff       (20)     2024 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/psaux/t1decode.h
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.440652 xpydf-0.1.5/src/freetype/src/pshinter/
--rw-r--r--   0 matthijs   (501) staff       (20)    58961 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/pshinter/pshalgo.c
--rw-r--r--   0 matthijs   (501) staff       (20)     6616 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/pshinter/pshalgo.h
--rw-r--r--   0 matthijs   (501) staff       (20)    22377 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/pshinter/pshglob.c
--rw-r--r--   0 matthijs   (501) staff       (20)     4860 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/pshinter/pshglob.h
--rw-r--r--   0 matthijs   (501) staff       (20)      671 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/pshinter/pshinter.c
--rw-r--r--   0 matthijs   (501) staff       (20)     3002 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/pshinter/pshmod.c
--rw-r--r--   0 matthijs   (501) staff       (20)      741 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/pshinter/pshmod.h
--rw-r--r--   0 matthijs   (501) staff       (20)      978 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/pshinter/pshnterr.h
--rw-r--r--   0 matthijs   (501) staff       (20)    31754 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/pshinter/pshrec.c
--rw-r--r--   0 matthijs   (501) staff       (20)     4103 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/pshinter/pshrec.h
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.441771 xpydf-0.1.5/src/freetype/src/psnames/
--rw-r--r--   0 matthijs   (501) staff       (20)    16268 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/psnames/psmodule.c
--rw-r--r--   0 matthijs   (501) staff       (20)      748 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/psnames/psmodule.h
--rw-r--r--   0 matthijs   (501) staff       (20)      999 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/psnames/psnamerr.h
--rw-r--r--   0 matthijs   (501) staff       (20)      622 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/psnames/psnames.c
--rw-r--r--   0 matthijs   (501) staff       (20)   268144 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/psnames/pstables.h
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.443835 xpydf-0.1.5/src/freetype/src/raster/
--rw-r--r--   0 matthijs   (501) staff       (20)     2969 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/raster/ftmisc.h
--rw-r--r--   0 matthijs   (501) staff       (20)    84634 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/raster/ftraster.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1092 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/raster/ftraster.h
--rw-r--r--   0 matthijs   (501) staff       (20)     5557 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/raster/ftrend1.c
--rw-r--r--   0 matthijs   (501) staff       (20)      755 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/raster/ftrend1.h
--rw-r--r--   0 matthijs   (501) staff       (20)      654 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/raster/raster.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1005 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/raster/rasterrs.h
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.445768 xpydf-0.1.5/src/freetype/src/sdf/
--rw-r--r--   0 matthijs   (501) staff       (20)    38453 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sdf/ftbsdf.c
--rw-r--r--   0 matthijs   (501) staff       (20)   112098 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sdf/ftsdf.c
--rw-r--r--   0 matthijs   (501) staff       (20)     2914 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sdf/ftsdf.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4108 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sdf/ftsdfcommon.c
--rw-r--r--   0 matthijs   (501) staff       (20)     4007 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sdf/ftsdfcommon.h
--rw-r--r--   0 matthijs   (501) staff       (20)      848 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sdf/ftsdferrs.h
--rw-r--r--   0 matthijs   (501) staff       (20)    16276 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sdf/ftsdfrend.c
--rw-r--r--   0 matthijs   (501) staff       (20)     3386 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sdf/ftsdfrend.h
--rw-r--r--   0 matthijs   (501) staff       (20)      735 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sdf/sdf.c
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.457291 xpydf-0.1.5/src/freetype/src/sfnt/
--rw-r--r--   0 matthijs   (501) staff       (20)    13188 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sfnt/pngshim.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1184 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sfnt/pngshim.h
--rw-r--r--   0 matthijs   (501) staff       (20)    36683 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sfnt/sfdriver.c
--rw-r--r--   0 matthijs   (501) staff       (20)      740 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sfnt/sfdriver.h
--rw-r--r--   0 matthijs   (501) staff       (20)      966 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sfnt/sferrors.h
--rw-r--r--   0 matthijs   (501) staff       (20)      908 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sfnt/sfnt.c
--rw-r--r--   0 matthijs   (501) staff       (20)    48936 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sfnt/sfobjs.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1417 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sfnt/sfobjs.h
--rw-r--r--   0 matthijs   (501) staff       (20)    12342 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sfnt/sfwoff.c
--rw-r--r--   0 matthijs   (501) staff       (20)      865 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sfnt/sfwoff.h
--rw-r--r--   0 matthijs   (501) staff       (20)    66294 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sfnt/sfwoff2.c
--rw-r--r--   0 matthijs   (501) staff       (20)     2124 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sfnt/sfwoff2.h
--rw-r--r--   0 matthijs   (501) staff       (20)     6247 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sfnt/ttbdf.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1029 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sfnt/ttbdf.h
--rw-r--r--   0 matthijs   (501) staff       (20)   111890 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sfnt/ttcmap.c
--rw-r--r--   0 matthijs   (501) staff       (20)     3727 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sfnt/ttcmap.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1227 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sfnt/ttcmapc.h
--rw-r--r--   0 matthijs   (501) staff       (20)    62115 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sfnt/ttcolr.c
--rw-r--r--   0 matthijs   (501) staff       (20)     2526 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sfnt/ttcolr.h
--rw-r--r--   0 matthijs   (501) staff       (20)     7964 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sfnt/ttcpal.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1036 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sfnt/ttcpal.h
--rw-r--r--   0 matthijs   (501) staff       (20)     7232 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sfnt/ttkern.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1199 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sfnt/ttkern.h
--rw-r--r--   0 matthijs   (501) staff       (20)    40643 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sfnt/ttload.c
--rw-r--r--   0 matthijs   (501) staff       (20)     2507 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sfnt/ttload.h
--rw-r--r--   0 matthijs   (501) staff       (20)     8552 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sfnt/ttmtx.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1289 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sfnt/ttmtx.h
--rw-r--r--   0 matthijs   (501) staff       (20)    13197 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sfnt/ttpost.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1002 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sfnt/ttpost.h
--rw-r--r--   0 matthijs   (501) staff       (20)    48308 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sfnt/ttsbit.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1672 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sfnt/ttsbit.h
--rw-r--r--   0 matthijs   (501) staff       (20)    10640 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sfnt/ttsvg.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1014 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sfnt/ttsvg.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4350 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sfnt/woff2tags.c
--rw-r--r--   0 matthijs   (501) staff       (20)      867 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/sfnt/woff2tags.h
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.458631 xpydf-0.1.5/src/freetype/src/smooth/
--rw-r--r--   0 matthijs   (501) staff       (20)    62480 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/smooth/ftgrays.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1260 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/smooth/ftgrays.h
--rw-r--r--   0 matthijs   (501) staff       (20)      997 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/smooth/ftsmerrs.h
--rw-r--r--   0 matthijs   (501) staff       (20)    16549 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/smooth/ftsmooth.c
--rw-r--r--   0 matthijs   (501) staff       (20)      751 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/smooth/ftsmooth.h
--rw-r--r--   0 matthijs   (501) staff       (20)      657 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/smooth/smooth.c
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.459362 xpydf-0.1.5/src/freetype/src/svg/
--rw-r--r--   0 matthijs   (501) staff       (20)     8897 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/svg/ftsvg.c
--rw-r--r--   0 matthijs   (501) staff       (20)      810 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/svg/ftsvg.h
--rw-r--r--   0 matthijs   (501) staff       (20)      656 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/svg/svg.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1195 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/svg/svgtypes.h
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.461207 xpydf-0.1.5/src/freetype/src/tools/
--rw-r--r--   0 matthijs   (501) staff       (20)    11420 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/tools/apinames.c
--rwxr-xr-x   0 matthijs   (501) staff       (20)     4216 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/tools/chktrcmp.py
--rw-r--r--   0 matthijs   (501) staff       (20)      770 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/tools/cordic.py
--rw-r--r--   0 matthijs   (501) staff       (20)   107236 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/tools/glnames.py
--rwxr-xr-x   0 matthijs   (501) staff       (20)     6188 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/tools/make_distribution_archives.py
--rw-r--r--   0 matthijs   (501) staff       (20)     3969 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/tools/test_afm.c
--rw-r--r--   0 matthijs   (501) staff       (20)     4191 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/tools/test_bbox.c
--rw-r--r--   0 matthijs   (501) staff       (20)     4826 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/tools/test_trig.c
--rw-r--r--   0 matthijs   (501) staff       (20)     9927 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/tools/vms_shorten_symbol.c
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.466579 xpydf-0.1.5/src/freetype/src/truetype/
--rw-r--r--   0 matthijs   (501) staff       (20)      896 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/truetype/truetype.c
--rw-r--r--   0 matthijs   (501) staff       (20)    22144 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/truetype/ttdriver.c
--rw-r--r--   0 matthijs   (501) staff       (20)      748 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/truetype/ttdriver.h
--rw-r--r--   0 matthijs   (501) staff       (20)      981 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/truetype/tterrors.h
--rw-r--r--   0 matthijs   (501) staff       (20)    93929 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/truetype/ttgload.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1358 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/truetype/ttgload.h
--rw-r--r--   0 matthijs   (501) staff       (20)   131819 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/truetype/ttgxvar.c
--rw-r--r--   0 matthijs   (501) staff       (20)    13625 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/truetype/ttgxvar.h
--rw-r--r--   0 matthijs   (501) staff       (20)   220265 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/truetype/ttinterp.c
--rw-r--r--   0 matthijs   (501) staff       (20)    21599 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/truetype/ttinterp.h
--rw-r--r--   0 matthijs   (501) staff       (20)    43577 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/truetype/ttobjs.c
--rw-r--r--   0 matthijs   (501) staff       (20)    12076 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/truetype/ttobjs.h
--rw-r--r--   0 matthijs   (501) staff       (20)    16553 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/truetype/ttpload.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1661 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/truetype/ttpload.h
--rw-r--r--   0 matthijs   (501) staff       (20)    32091 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/truetype/ttsubpix.c
--rw-r--r--   0 matthijs   (501) staff       (20)     3848 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/truetype/ttsubpix.h
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.470358 xpydf-0.1.5/src/freetype/src/type1/
--rw-r--r--   0 matthijs   (501) staff       (20)    10669 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/type1/t1afm.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1285 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/type1/t1afm.h
--rw-r--r--   0 matthijs   (501) staff       (20)    24329 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/type1/t1driver.c
--rw-r--r--   0 matthijs   (501) staff       (20)      769 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/type1/t1driver.h
--rw-r--r--   0 matthijs   (501) staff       (20)      969 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/type1/t1errors.h
--rw-r--r--   0 matthijs   (501) staff       (20)    20367 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/type1/t1gload.c
--rw-r--r--   0 matthijs   (501) staff       (20)     1193 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/type1/t1gload.h
--rw-r--r--   0 matthijs   (501) staff       (20)    82040 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/type1/t1load.c
--rw-r--r--   0 matthijs   (501) staff       (20)     3285 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/type1/t1load.h
--rw-r--r--   0 matthijs   (501) staff       (20)    17437 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/type1/t1objs.c
--rw-r--r--   0 matthijs   (501) staff       (20)     3452 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/type1/t1objs.h
--rw-r--r--   0 matthijs   (501) staff       (20)    14896 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/type1/t1parse.c
--rw-r--r--   0 matthijs   (501) staff       (20)     3735 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/type1/t1parse.h
--rw-r--r--   0 matthijs   (501) staff       (20)     5083 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/type1/t1tokens.h
--rw-r--r--   0 matthijs   (501) staff       (20)      720 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/type1/type1.c
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.472222 xpydf-0.1.5/src/freetype/src/type42/
--rw-r--r--   0 matthijs   (501) staff       (20)     6579 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/type42/t42drivr.c
--rw-r--r--   0 matthijs   (501) staff       (20)      739 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/type42/t42drivr.h
--rw-r--r--   0 matthijs   (501) staff       (20)      973 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/type42/t42error.h
--rw-r--r--   0 matthijs   (501) staff       (20)    19226 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/type42/t42objs.c
--rw-r--r--   0 matthijs   (501) staff       (20)     2452 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/type42/t42objs.h
--rw-r--r--   0 matthijs   (501) staff       (20)    40017 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/type42/t42parse.c
--rw-r--r--   0 matthijs   (501) staff       (20)     2029 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/type42/t42parse.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1181 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/type42/t42types.h
--rw-r--r--   0 matthijs   (501) staff       (20)      652 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/type42/type42.c
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.473086 xpydf-0.1.5/src/freetype/src/winfonts/
--rw-r--r--   0 matthijs   (501) staff       (20)      988 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/winfonts/fnterrs.h
--rw-r--r--   0 matthijs   (501) staff       (20)    35786 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/winfonts/winfnt.c
--rw-r--r--   0 matthijs   (501) staff       (20)     3104 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/src/winfonts/winfnt.h
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.342268 xpydf-0.1.5/src/freetype/tests/
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.473263 xpydf-0.1.5/src/freetype/tests/scripts/
--rwxr-xr-x   0 matthijs   (501) staff       (20)     8869 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/tests/scripts/download-test-fonts.py
--rw-r--r--   0 matthijs   (501) staff       (20)    41515 2023-05-19 16:13:04.000000 xpydf-0.1.5/src/freetype/vms_make.com
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.478888 xpydf-0.1.5/src/xpdf-4.04/
--rw-r--r--   0 matthijs   (501) staff       (20)     8196 2023-06-02 09:36:12.000000 xpydf-0.1.5/src/xpdf-4.04/.DS_Store
--rw-r--r--   0 matthijs   (501) staff       (20)     1330 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/ANNOUNCE
--rw-r--r--   0 matthijs   (501) staff       (20)   139475 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/CHANGES
--rw-r--r--   0 matthijs   (501) staff       (20)     1053 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/CMakeLists.txt
--rw-r--r--   0 matthijs   (501) staff       (20)    17982 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/COPYING
--rw-r--r--   0 matthijs   (501) staff       (20)    35147 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/COPYING3
--rw-r--r--   0 matthijs   (501) staff       (20)     5614 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/INSTALL
--rw-r--r--   0 matthijs   (501) staff       (20)    13778 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/README
--rw-r--r--   0 matthijs   (501) staff       (20)     2002 2023-06-02 09:36:35.000000 xpydf-0.1.5/src/xpdf-4.04/aconf.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1985 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/aconf.h.in
--rw-r--r--   0 matthijs   (501) staff       (20)      941 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/aconf2.h
--rw-r--r--   0 matthijs   (501) staff       (20)    10676 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/cmake-config.txt
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.482271 xpydf-0.1.5/src/xpdf-4.04/fofi/
--rw-r--r--   0 matthijs   (501) staff       (20)     3275 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/fofi/FoFiBase.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1344 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/fofi/FoFiBase.h
--rw-r--r--   0 matthijs   (501) staff       (20)    14853 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/fofi/FoFiEncodings.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1005 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/fofi/FoFiEncodings.h
--rw-r--r--   0 matthijs   (501) staff       (20)    21889 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/fofi/FoFiIdentifier.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1659 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/fofi/FoFiIdentifier.h
--rw-r--r--   0 matthijs   (501) staff       (20)    77637 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/fofi/FoFiTrueType.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     8227 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/fofi/FoFiTrueType.h
--rw-r--r--   0 matthijs   (501) staff       (20)     8796 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/fofi/FoFiType1.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1434 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/fofi/FoFiType1.h
--rw-r--r--   0 matthijs   (501) staff       (20)    97383 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/fofi/FoFiType1C.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     8299 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/fofi/FoFiType1C.h
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.492525 xpydf-0.1.5/src/xpdf-4.04/goo/
--rw-r--r--   0 matthijs   (501) staff       (20)     2748 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/goo/FixedPoint.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     7361 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/goo/FixedPoint.h
--rw-r--r--   0 matthijs   (501) staff       (20)     6201 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/goo/GHash.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2209 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/goo/GHash.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2276 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/goo/GList.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2724 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/goo/GList.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2629 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/goo/GMutex.h
--rw-r--r--   0 matthijs   (501) staff       (20)    17722 2023-06-02 09:35:24.000000 xpydf-0.1.5/src/xpdf-4.04/goo/GString.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     4269 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/goo/GString.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2406 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/goo/Trace.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1171 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/goo/Trace.h
--rw-r--r--   0 matthijs   (501) staff       (20)    17381 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/goo/gfile.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     4565 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/goo/gfile.h
--rw-r--r--   0 matthijs   (501) staff       (20)     8259 2023-03-01 15:38:49.000000 xpydf-0.1.5/src/xpdf-4.04/goo/gmem.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2029 2023-03-01 15:38:49.000000 xpydf-0.1.5/src/xpdf-4.04/goo/gmem.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1005 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/goo/gmempp.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1714 2023-03-01 15:38:49.000000 xpydf-0.1.5/src/xpdf-4.04/goo/gmempp.h
--rw-r--r--   0 matthijs   (501) staff       (20)      562 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/goo/gtypes.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1583 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/goo/parseargs.h
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.514980 xpydf-0.1.5/src/xpdf-4.04/splash/
--rw-r--r--   0 matthijs   (501) staff       (20)   230071 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/splash/Splash.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    20193 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/splash/Splash.h
--rw-r--r--   0 matthijs   (501) staff       (20)     6603 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/splash/SplashBitmap.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2881 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/splash/SplashBitmap.h
--rw-r--r--   0 matthijs   (501) staff       (20)    11473 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/splash/SplashClip.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     4007 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/splash/SplashClip.h
--rw-r--r--   0 matthijs   (501) staff       (20)      930 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/splash/SplashErrorCodes.h
--rw-r--r--   0 matthijs   (501) staff       (20)    13929 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/splash/SplashFTFont.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1345 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/splash/SplashFTFont.h
--rw-r--r--   0 matthijs   (501) staff       (20)     8902 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/splash/SplashFTFontEngine.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2248 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/splash/SplashFTFontEngine.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4055 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/splash/SplashFTFontFile.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2241 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/splash/SplashFTFontFile.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4995 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/splash/SplashFont.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3666 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/splash/SplashFont.h
--rw-r--r--   0 matthijs   (501) staff       (20)     9673 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/splash/SplashFontEngine.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3358 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/splash/SplashFontEngine.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1589 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/splash/SplashFontFile.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2168 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/splash/SplashFontFile.h
--rw-r--r--   0 matthijs   (501) staff       (20)      603 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/splash/SplashFontFileID.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      687 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/splash/SplashFontFileID.h
--rw-r--r--   0 matthijs   (501) staff       (20)      758 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/splash/SplashGlyphBitmap.h
--rw-r--r--   0 matthijs   (501) staff       (20)     9510 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/splash/SplashMath.h
--rw-r--r--   0 matthijs   (501) staff       (20)     5135 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/splash/SplashPath.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3876 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/splash/SplashPath.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1042 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/splash/SplashPattern.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1447 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/splash/SplashPattern.h
--rw-r--r--   0 matthijs   (501) staff       (20)     9844 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/splash/SplashScreen.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2167 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/splash/SplashScreen.h
--rw-r--r--   0 matthijs   (501) staff       (20)     9521 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/splash/SplashState.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3669 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/splash/SplashState.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4155 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/splash/SplashTypes.h
--rw-r--r--   0 matthijs   (501) staff       (20)    17088 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/splash/SplashXPath.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3761 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/splash/SplashXPath.h
--rw-r--r--   0 matthijs   (501) staff       (20)    12936 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/splash/SplashXPathScanner.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2482 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/splash/SplashXPathScanner.h
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.565090 xpydf-0.1.5/src/xpdf-4.04/xpdf/
--rw-r--r--   0 matthijs   (501) staff       (20)   104374 2023-05-15 13:37:05.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/AcroForm.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     5269 2023-05-15 13:34:50.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/AcroForm.h
--rw-r--r--   0 matthijs   (501) staff       (20)    38840 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/Annot.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     4895 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/Annot.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1385 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/Array.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1400 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/Array.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1387 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/BuiltinFont.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1080 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/BuiltinFont.h
--rw-r--r--   0 matthijs   (501) staff       (20)   229548 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/BuiltinFontTables.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      556 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/BuiltinFontTables.h
--rw-r--r--   0 matthijs   (501) staff       (20)    10417 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/CMap.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3178 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/CMap.h
--rw-r--r--   0 matthijs   (501) staff       (20)    28608 2023-05-15 13:29:26.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/Catalog.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     4742 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/Catalog.h
--rw-r--r--   0 matthijs   (501) staff       (20)    19175 2023-04-13 10:47:41.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/CharCodeToUnicode.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3702 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/CharCodeToUnicode.h
--rw-r--r--   0 matthijs   (501) staff       (20)      526 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/CharTypes.h
--rw-r--r--   0 matthijs   (501) staff       (20)     8379 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/CompactFontTables.h
--rw-r--r--   0 matthijs   (501) staff       (20)    45644 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/Decrypt.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3530 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/Decrypt.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2993 2023-05-15 08:40:36.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/Dict.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2088 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/Dict.h
--rw-r--r--   0 matthijs   (501) staff       (20)     5247 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/DisplayState.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     5225 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/DisplayState.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2123 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/Error.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1353 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/Error.h
--rw-r--r--   0 matthijs   (501) staff       (20)      984 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/ErrorCodes.h
--rw-r--r--   0 matthijs   (501) staff       (20)    21312 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/FontEncodingTables.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      564 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/FontEncodingTables.h
--rw-r--r--   0 matthijs   (501) staff       (20)    36553 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/Function.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     6722 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/Function.h
--rw-r--r--   0 matthijs   (501) staff       (20)   144837 2023-06-02 09:35:24.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/Gfx.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    11911 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/Gfx.h
--rw-r--r--   0 matthijs   (501) staff       (20)    65646 2023-06-02 09:35:24.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/GfxFont.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    12828 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/GfxFont.h
--rw-r--r--   0 matthijs   (501) staff       (20)   120789 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/GfxState.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    43452 2023-06-02 09:35:24.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/GfxState.h
--rw-r--r--   0 matthijs   (501) staff       (20)   103543 2023-05-19 16:11:38.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/GlobalParams.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    23054 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/GlobalParams.h
--rw-r--r--   0 matthijs   (501) staff       (20)    34442 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/HTMLGen.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3131 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/HTMLGen.h
--rw-r--r--   0 matthijs   (501) staff       (20)    11293 2023-05-02 12:54:18.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/ImageOutputDev.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3942 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/ImageOutputDev.h
--rw-r--r--   0 matthijs   (501) staff       (20)     8327 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/JArithmeticDecoder.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2802 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/JArithmeticDecoder.h
--rw-r--r--   0 matthijs   (501) staff       (20)   109724 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/JBIG2Stream.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     4824 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/JBIG2Stream.h
--rw-r--r--   0 matthijs   (501) staff       (20)   107255 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/JPXStream.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    11092 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/JPXStream.h
--rw-r--r--   0 matthijs   (501) staff       (20)    11674 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/Lexer.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2035 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/Lexer.h
--rw-r--r--   0 matthijs   (501) staff       (20)    21632 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/Link.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    11370 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/Link.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2191 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/NameToCharCode.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      726 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/NameToCharCode.h
--rw-r--r--   0 matthijs   (501) staff       (20)   117065 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/NameToUnicodeTable.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4471 2023-05-15 08:40:34.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/Object.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     9081 2023-05-15 08:40:32.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/Object.h
--rw-r--r--   0 matthijs   (501) staff       (20)    12818 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/OptionalContent.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3617 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/OptionalContent.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4001 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/Outline.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1774 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/Outline.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4131 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/OutputDev.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     8935 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/OutputDev.h
--rw-r--r--   0 matthijs   (501) staff       (20)    87382 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/PDF417Barcode.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      838 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/PDF417Barcode.h
--rw-r--r--   0 matthijs   (501) staff       (20)    51111 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/PDFCore.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    11579 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/PDFCore.h
--rw-r--r--   0 matthijs   (501) staff       (20)    16078 2023-05-16 07:46:43.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/PDFDoc.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     6774 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/PDFDoc.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2530 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/PDFDocEncoding.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      339 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/PDFDocEncoding.h
--rw-r--r--   0 matthijs   (501) staff       (20)   230372 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/PSOutputDev.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    19106 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/PSOutputDev.h
--rw-r--r--   0 matthijs   (501) staff       (20)     3295 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/PSTokenizer.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      771 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/PSTokenizer.h
--rw-r--r--   0 matthijs   (501) staff       (20)    13874 2023-03-01 15:38:49.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/Page.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     6412 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/Page.h
--rw-r--r--   0 matthijs   (501) staff       (20)     8100 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/Parser.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1674 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/Parser.h
--rw-r--r--   0 matthijs   (501) staff       (20)     8588 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/PreScanOutputDev.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     4810 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/PreScanOutputDev.h
--rw-r--r--   0 matthijs   (501) staff       (20)    10354 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/SecurityHandler.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3962 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/SecurityHandler.h
--rw-r--r--   0 matthijs   (501) staff       (20)    37941 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/ShadingImage.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3215 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/ShadingImage.h
--rw-r--r--   0 matthijs   (501) staff       (20)   127634 2023-05-19 16:11:47.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/SplashOutputDev.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    10811 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/SplashOutputDev.h
--rw-r--r--   0 matthijs   (501) staff       (20)    17471 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/Stream-CCITT.h
--rw-r--r--   0 matthijs   (501) staff       (20)   131758 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/Stream.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    31826 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/Stream.h
--rw-r--r--   0 matthijs   (501) staff       (20)   183399 2023-06-02 09:35:24.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/TextOutputDev.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    27134 2023-06-02 09:35:24.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/TextOutputDev.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4302 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/TextString.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1587 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/TextString.h
--rw-r--r--   0 matthijs   (501) staff       (20)    13862 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/TileCache.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2041 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/TileCache.h
--rw-r--r--   0 matthijs   (501) staff       (20)    10913 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/TileCompositor.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1895 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/TileCompositor.h
--rw-r--r--   0 matthijs   (501) staff       (20)    44674 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/TileMap.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     8164 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/TileMap.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4636 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/UTF8.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1408 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/UTF8.h
--rw-r--r--   0 matthijs   (501) staff       (20)     6033 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/UnicodeMap.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2971 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/UnicodeMap.h
--rw-r--r--   0 matthijs   (501) staff       (20)    11532 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/UnicodeMapTables.h
--rw-r--r--   0 matthijs   (501) staff       (20)     5024 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/UnicodeRemapping.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1138 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/UnicodeRemapping.h
--rw-r--r--   0 matthijs   (501) staff       (20)    73118 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/UnicodeTypeTable.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      719 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/UnicodeTypeTable.h
--rw-r--r--   0 matthijs   (501) staff       (20)    10592 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/WebFont.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2139 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/WebFont.h
--rw-r--r--   0 matthijs   (501) staff       (20)    18912 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/XFAScanner.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     4518 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/XFAScanner.h
--rw-r--r--   0 matthijs   (501) staff       (20)    33740 2023-05-15 08:40:18.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/XRef.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     5955 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/XRef.h
--rw-r--r--   0 matthijs   (501) staff       (20)    23997 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/Zoox.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     6378 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/Zoox.h
--rw-r--r--   0 matthijs   (501) staff       (20)     3128 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/config.h
--rw-r--r--   0 matthijs   (501) staff       (20)     5663 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/pdfdetach.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    12108 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/pdffonts.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     4538 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/pdfimages.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    15031 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/pdfinfo.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     8525 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/pdftohtml.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    10873 2023-05-19 13:46:26.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/pdftopng.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     7820 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/pdftoppm.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    11515 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/pdftops.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     9928 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf/pdftotext.cc
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.568604 xpydf-0.1.5/src/xpdf-4.04/xpdf-qt/
--rw-r--r--   0 matthijs   (501) staff       (20)    30301 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf-qt/QtPDFCore.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     6596 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf-qt/QtPDFCore.h
--rw-r--r--   0 matthijs   (501) staff       (20)    14925 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf-qt/XpdfApp.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2452 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf-qt/XpdfApp.h
--rw-r--r--   0 matthijs   (501) staff       (20)   148791 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf-qt/XpdfViewer.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    18968 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf-qt/XpdfViewer.h
--rw-r--r--   0 matthijs   (501) staff       (20)    54075 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf-qt/XpdfWidget.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    39531 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf-qt/XpdfWidget.h
--rw-r--r--   0 matthijs   (501) staff       (20)    13035 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf-qt/XpdfWidgetPrint.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      520 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf-qt/XpdfWidgetPrint.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1327 2022-04-18 21:11:23.000000 xpydf-0.1.5/src/xpdf-4.04/xpdf-qt/xpdf.cc
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.576356 xpydf-0.1.5/src/xpydf/
--rw-r--r--   0 matthijs   (501) staff       (20)     6148 2023-05-01 14:11:15.000000 xpydf-0.1.5/src/xpydf/.DS_Store
--rw-r--r--   0 matthijs   (501) staff       (20)     3768 2023-05-23 14:30:42.000000 xpydf-0.1.5/src/xpydf/ImageDataDev.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1095 2023-05-05 08:47:39.000000 xpydf-0.1.5/src/xpydf/ImageDataDev.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1121 2023-05-15 08:40:14.000000 xpydf-0.1.5/src/xpydf/ImageInfoDev.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      941 2023-04-12 11:54:25.000000 xpydf-0.1.5/src/xpydf/ImageInfoDev.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4540 2023-06-02 09:36:35.000000 xpydf-0.1.5/src/xpydf/PdfLoader.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1118 2023-06-02 09:36:35.000000 xpydf-0.1.5/src/xpydf/PdfLoader.h
--rw-r--r--   0 matthijs   (501) staff       (20)     7660 2023-06-02 09:36:35.000000 xpydf-0.1.5/src/xpydf/PdfLoaderWrapper.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2198 2023-04-12 11:54:25.000000 xpydf-0.1.5/src/xpydf/PyCppConversion.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      441 2023-04-12 11:54:25.000000 xpydf-0.1.5/src/xpydf/PyCppConversion.h
--rw-r--r--   0 matthijs   (501) staff       (20)        0 2023-04-12 11:54:25.000000 xpydf-0.1.5/src/xpydf/__init__.py
--rw-r--r--   0 matthijs   (501) staff       (20)        0 2023-04-12 11:54:25.000000 xpydf-0.1.5/src/xpydf/__init__.pyi
--rw-r--r--   0 matthijs   (501) staff       (20)      760 2023-06-02 09:36:35.000000 xpydf-0.1.5/src/xpydf/cXpdfPython.pyi
--rw-r--r--   0 matthijs   (501) staff       (20)     4684 2023-06-02 09:36:35.000000 xpydf-0.1.5/src/xpydf/pdf_loader.py
--rw-r--r--   0 matthijs   (501) staff       (20)     1159 2023-06-02 09:36:35.000000 xpydf-0.1.5/src/xpydf/pdf_loader.pyi
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.577679 xpydf-0.1.5/src/xpydf.egg-info/
--rw-r--r--   0 matthijs   (501) staff       (20)      844 2023-06-02 10:44:33.000000 xpydf-0.1.5/src/xpydf.egg-info/PKG-INFO
--rw-r--r--   0 matthijs   (501) staff       (20)    25801 2023-06-02 10:44:33.000000 xpydf-0.1.5/src/xpydf.egg-info/SOURCES.txt
--rw-r--r--   0 matthijs   (501) staff       (20)        1 2023-06-02 10:44:33.000000 xpydf-0.1.5/src/xpydf.egg-info/dependency_links.txt
--rw-r--r--   0 matthijs   (501) staff       (20)       14 2023-06-02 10:44:33.000000 xpydf-0.1.5/src/xpydf.egg-info/requires.txt
--rw-r--r--   0 matthijs   (501) staff       (20)       27 2023-06-02 10:44:33.000000 xpydf-0.1.5/src/xpydf.egg-info/top_level.txt
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-06-02 10:44:33.577845 xpydf-0.1.5/tests/
--rw-r--r--   0 matthijs   (501) staff       (20)     4094 2023-06-02 09:36:35.000000 xpydf-0.1.5/tests/test_pdf_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:30.852634 xpydf-0.1.6/
+-rw-r--r--   0 root         (0) root         (0)     6148 2023-06-09 10:59:30.645811 xpydf-0.1.6/.DS_Store
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-02-17 12:43:21.000000 xpydf-0.1.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      418 2023-06-09 07:28:33.000000 xpydf-0.1.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      844 2023-06-09 10:59:30.851324 xpydf-0.1.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      240 2023-04-12 11:54:25.000000 xpydf-0.1.6/README.md
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-09 07:59:23.000000 xpydf-0.1.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 10:59:30.853530 xpydf-0.1.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4752 2023-06-09 07:43:48.000000 xpydf-0.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:30.638123 xpydf-0.1.6/src/
+-rw-r--r--   0 root         (0) root         (0)     6148 2023-06-09 10:59:30.639107 xpydf-0.1.6/src/.DS_Store
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:25.920623 xpydf-0.1.6/src/freetype/
+-rw-r--r--   0 root         (0) root         (0)     8196 2023-05-23 14:26:17.000000 xpydf-0.1.6/src/freetype/.DS_Store
+-rw-r--r--   0 root         (0) root         (0)      453 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/.clang-format
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/.git
+-rw-r--r--   0 root         (0) root         (0)       94 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     7021 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/.gitlab-ci.yml
+-rw-r--r--   0 root         (0) root         (0)       84 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/.gitmodules
+-rw-r--r--   0 root         (0) root         (0)     1821 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/.mailmap
+-rw-r--r--   0 root         (0) root         (0)    21367 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     2074 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/LICENSE.TXT
+-rw-r--r--   0 root         (0) root         (0)      846 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/Makefile
+-rw-r--r--   0 root         (0) root         (0)     3114 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/README
+-rw-r--r--   0 root         (0) root         (0)     3154 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/README.git
+-rwxr-xr-x   0 root         (0) root         (0)     4768 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/autogen.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:25.714868 xpydf-0.1.6/src/freetype/builds/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:25.926346 xpydf-0.1.6/src/freetype/builds/mac/
+-rwxr-xr-x   0 root         (0) root         (0)     1033 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/builds/mac/ascii2mpw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:25.950519 xpydf-0.1.6/src/freetype/builds/meson/
+-rw-r--r--   0 root         (0) root         (0)     3019 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/builds/meson/extract_freetype_version.py
+-rw-r--r--   0 root         (0) root         (0)     2906 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/builds/meson/extract_libtool_version.py
+-rw-r--r--   0 root         (0) root         (0)     2317 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/builds/meson/generate_reference_docs.py
+-rw-r--r--   0 root         (0) root         (0)     4596 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/builds/meson/parse_modules_cfg.py
+-rw-r--r--   0 root         (0) root         (0)     3403 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/builds/meson/process_ftoption_h.py
+-rw-r--r--   0 root         (0) root         (0)     1633 2023-05-22 06:59:42.000000 xpydf-0.1.6/src/freetype/config.mk
+-rwxr-xr-x   0 root         (0) root         (0)     4029 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/configure
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:25.956373 xpydf-0.1.6/src/freetype/include/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:25.966158 xpydf-0.1.6/src/freetype/include/dlg/
+-rw-r--r--   0 root         (0) root         (0)    10834 2023-05-22 06:59:35.000000 xpydf-0.1.6/src/freetype/include/dlg/dlg.h
+-rw-r--r--   0 root         (0) root         (0)     7229 2023-05-22 06:59:35.000000 xpydf-0.1.6/src/freetype/include/dlg/output.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:26.257619 xpydf-0.1.6/src/freetype/include/freetype/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:26.314734 xpydf-0.1.6/src/freetype/include/freetype/config/
+-rw-r--r--   0 root         (0) root         (0)     1614 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/config/ftconfig.h
+-rw-r--r--   0 root         (0) root         (0)    23919 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/config/ftheader.h
+-rw-r--r--   0 root         (0) root         (0)     1443 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/config/ftmodule.h
+-rw-r--r--   0 root         (0) root         (0)    39628 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/config/ftoption.h
+-rw-r--r--   0 root         (0) root         (0)     4576 2023-05-23 14:26:12.000000 xpydf-0.1.6/src/freetype/include/freetype/config/ftstdlib.h
+-rw-r--r--   0 root         (0) root         (0)     7072 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/config/integer-types.h
+-rw-r--r--   0 root         (0) root         (0)     1597 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/config/mac-support.h
+-rw-r--r--   0 root         (0) root         (0)     4207 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/config/public-macros.h
+-rw-r--r--   0 root         (0) root         (0)   178794 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/freetype.h
+-rw-r--r--   0 root         (0) root         (0)     5470 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/ftadvanc.h
+-rw-r--r--   0 root         (0) root         (0)     2638 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/ftbbox.h
+-rw-r--r--   0 root         (0) root         (0)     5322 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/ftbdf.h
+-rw-r--r--   0 root         (0) root         (0)     9051 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/ftbitmap.h
+-rw-r--r--   0 root         (0) root         (0)     2786 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/ftbzip2.h
+-rw-r--r--   0 root         (0) root         (0)    34179 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/ftcache.h
+-rw-r--r--   0 root         (0) root         (0)     2933 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/ftchapters.h
+-rw-r--r--   0 root         (0) root         (0)     4022 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/ftcid.h
+-rw-r--r--   0 root         (0) root         (0)    50199 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/ftcolor.h
+-rw-r--r--   0 root         (0) root         (0)    47533 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/ftdriver.h
+-rw-r--r--   0 root         (0) root         (0)    12559 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/fterrdef.h
+-rw-r--r--   0 root         (0) root         (0)     9301 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/fterrors.h
+-rw-r--r--   0 root         (0) root         (0)     2213 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/ftfntfmt.h
+-rw-r--r--   0 root         (0) root         (0)     4138 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/ftgasp.h
+-rw-r--r--   0 root         (0) root         (0)    20912 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/ftglyph.h
+-rw-r--r--   0 root         (0) root         (0)    10625 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/ftgxval.h
+-rw-r--r--   0 root         (0) root         (0)     4211 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/ftgzip.h
+-rw-r--r--   0 root         (0) root         (0)    41833 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/ftimage.h
+-rw-r--r--   0 root         (0) root         (0)    10696 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/ftincrem.h
+-rw-r--r--   0 root         (0) root         (0)    11744 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/ftlcdfil.h
+-rw-r--r--   0 root         (0) root         (0)     7100 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/ftlist.h
+-rw-r--r--   0 root         (0) root         (0)     4130 2023-05-23 14:26:12.000000 xpydf-0.1.6/src/freetype/include/freetype/ftlogging.h
+-rw-r--r--   0 root         (0) root         (0)     2768 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/ftlzw.h
+-rw-r--r--   0 root         (0) root         (0)     7771 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/ftmac.h
+-rw-r--r--   0 root         (0) root         (0)    23797 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/ftmm.h
+-rw-r--r--   0 root         (0) root         (0)    22544 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/ftmodapi.h
+-rw-r--r--   0 root         (0) root         (0)     6675 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/ftmoderr.h
+-rw-r--r--   0 root         (0) root         (0)     5346 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/ftotval.h
+-rw-r--r--   0 root         (0) root         (0)    17402 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/ftoutln.h
+-rw-r--r--   0 root         (0) root         (0)     6041 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/ftparams.h
+-rw-r--r--   0 root         (0) root         (0)     4908 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/ftpfr.h
+-rw-r--r--   0 root         (0) root         (0)     6625 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/ftrender.h
+-rw-r--r--   0 root         (0) root         (0)     4288 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/ftsizes.h
+-rw-r--r--   0 root         (0) root         (0)     7730 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/ftsnames.h
+-rw-r--r--   0 root         (0) root         (0)    21773 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/ftstroke.h
+-rw-r--r--   0 root         (0) root         (0)     4483 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/ftsynth.h
+-rw-r--r--   0 root         (0) root         (0)     8502 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/ftsystem.h
+-rw-r--r--   0 root         (0) root         (0)     7411 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/fttrigon.h
+-rw-r--r--   0 root         (0) root         (0)    14735 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/fttypes.h
+-rw-r--r--   0 root         (0) root         (0)     7965 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/ftwinfnt.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:26.485144 xpydf-0.1.6/src/freetype/include/freetype/internal/
+-rw-r--r--   0 root         (0) root         (0)     7498 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/autohint.h
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/cffotypes.h
+-rw-r--r--   0 root         (0) root         (0)    11866 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/cfftypes.h
+-rw-r--r--   0 root         (0) root         (0)    11499 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/compiler-macros.h
+-rw-r--r--   0 root         (0) root         (0)    15606 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/ftcalc.h
+-rw-r--r--   0 root         (0) root         (0)    13332 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/ftdebug.h
+-rw-r--r--   0 root         (0) root         (0)     9214 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/ftdrv.h
+-rw-r--r--   0 root         (0) root         (0)     4504 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/ftgloadr.h
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/fthash.h
+-rw-r--r--   0 root         (0) root         (0)    15961 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/ftmemory.h
+-rw-r--r--   0 root         (0) root         (0)     3003 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/ftmmtypes.h
+-rw-r--r--   0 root         (0) root         (0)    42481 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/ftobjs.h
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/ftpsprop.h
+-rw-r--r--   0 root         (0) root         (0)     7651 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/ftrfork.h
+-rw-r--r--   0 root         (0) root         (0)    24053 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/ftserv.h
+-rw-r--r--   0 root         (0) root         (0)    23230 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/ftstream.h
+-rw-r--r--   0 root         (0) root         (0)     5918 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/fttrace.h
+-rw-r--r--   0 root         (0) root         (0)     5762 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/ftvalid.h
+-rw-r--r--   0 root         (0) root         (0)    43241 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/psaux.h
+-rw-r--r--   0 root         (0) root         (0)    20852 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/pshints.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:26.620094 xpydf-0.1.6/src/freetype/include/freetype/internal/services/
+-rw-r--r--   0 root         (0) root         (0)     1731 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/services/svbdf.h
+-rw-r--r--   0 root         (0) root         (0)     2832 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/services/svcfftl.h
+-rw-r--r--   0 root         (0) root         (0)     2124 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/services/svcid.h
+-rw-r--r--   0 root         (0) root         (0)     1348 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/services/svfntfmt.h
+-rw-r--r--   0 root         (0) root         (0)     1865 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/services/svgldict.h
+-rw-r--r--   0 root         (0) root         (0)     1730 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/services/svgxval.h
+-rw-r--r--   0 root         (0) root         (0)     1080 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/services/svkern.h
+-rw-r--r--   0 root         (0) root         (0)     3996 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/services/svmetric.h
+-rw-r--r--   0 root         (0) root         (0)     8956 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/services/svmm.h
+-rw-r--r--   0 root         (0) root         (0)     1253 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/services/svotval.h
+-rw-r--r--   0 root         (0) root         (0)     1570 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/services/svpfr.h
+-rw-r--r--   0 root         (0) root         (0)     1571 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/services/svpostnm.h
+-rw-r--r--   0 root         (0) root         (0)     1677 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/services/svprop.h
+-rw-r--r--   0 root         (0) root         (0)     4272 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/services/svpscmap.h
+-rw-r--r--   0 root         (0) root         (0)     2469 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/services/svpsinfo.h
+-rw-r--r--   0 root         (0) root         (0)     2079 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/services/svsfnt.h
+-rw-r--r--   0 root         (0) root         (0)     2397 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/services/svttcmap.h
+-rw-r--r--   0 root         (0) root         (0)     1007 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/services/svtteng.h
+-rw-r--r--   0 root         (0) root         (0)     1251 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/services/svttglyf.h
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/services/svwinfnt.h
+-rw-r--r--   0 root         (0) root         (0)    32444 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/sfnt.h
+-rw-r--r--   0 root         (0) root         (0)     1041 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/svginterface.h
+-rw-r--r--   0 root         (0) root         (0)     8208 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/t1types.h
+-rw-r--r--   0 root         (0) root         (0)    52695 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/tttypes.h
+-rw-r--r--   0 root         (0) root         (0)     8010 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/internal/wofftypes.h
+-rw-r--r--   0 root         (0) root         (0)    10457 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/otsvg.h
+-rw-r--r--   0 root         (0) root         (0)    23188 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/t1tables.h
+-rw-r--r--   0 root         (0) root         (0)    58769 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/ttnameid.h
+-rw-r--r--   0 root         (0) root         (0)    25227 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/tttables.h
+-rw-r--r--   0 root         (0) root         (0)     5145 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/freetype/tttags.h
+-rw-r--r--   0 root         (0) root         (0)      990 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/include/ft2build.h
+-rw-r--r--   0 root         (0) root         (0)    13071 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/meson.build
+-rw-r--r--   0 root         (0) root         (0)     1518 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/meson_options.txt
+-rw-r--r--   0 root         (0) root         (0)     6490 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/modules.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:25.776903 xpydf-0.1.6/src/freetype/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:26.941036 xpydf-0.1.6/src/freetype/src/autofit/
+-rw-r--r--   0 root         (0) root         (0)    76975 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/autofit/afblue.c
+-rw-r--r--   0 root         (0) root         (0)    16937 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/autofit/afblue.h
+-rw-r--r--   0 root         (0) root         (0)    66667 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/autofit/afcjk.c
+-rw-r--r--   0 root         (0) root         (0)     4211 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/autofit/afcjk.h
+-rw-r--r--   0 root         (0) root         (0)     3159 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/autofit/afcover.h
+-rw-r--r--   0 root         (0) root         (0)     2160 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/autofit/afdummy.c
+-rw-r--r--   0 root         (0) root         (0)      877 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/autofit/afdummy.h
+-rw-r--r--   0 root         (0) root         (0)      984 2023-05-22 06:46:50.000000 xpydf-0.1.6/src/freetype/src/autofit/aferrors.h
+-rw-r--r--   0 root         (0) root         (0)    13736 2023-05-23 09:51:54.000000 xpydf-0.1.6/src/freetype/src/autofit/afglobal.c
+-rw-r--r--   0 root         (0) root         (0)     5110 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/autofit/afglobal.h
+-rw-r--r--   0 root         (0) root         (0)    47282 2023-05-23 14:26:12.000000 xpydf-0.1.6/src/freetype/src/autofit/afhints.c
+-rw-r--r--   0 root         (0) root         (0)    15948 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/autofit/afhints.h
+-rw-r--r--   0 root         (0) root         (0)     4719 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/autofit/afindic.c
+-rw-r--r--   0 root         (0) root         (0)      840 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/autofit/afindic.h
+-rw-r--r--   0 root         (0) root         (0)   113850 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/autofit/aflatin.c
+-rw-r--r--   0 root         (0) root         (0)     6784 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/autofit/aflatin.h
+-rw-r--r--   0 root         (0) root         (0)    24004 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/autofit/afloader.c
+-rw-r--r--   0 root         (0) root         (0)     2269 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/autofit/afloader.h
+-rw-r--r--   0 root         (0) root         (0)    13961 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/autofit/afmodule.c
+-rw-r--r--   0 root         (0) root         (0)     1181 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/autofit/afmodule.h
+-rw-r--r--   0 root         (0) root         (0)    34997 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/autofit/afranges.c
+-rw-r--r--   0 root         (0) root         (0)     1083 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/autofit/afranges.h
+-rw-r--r--   0 root         (0) root         (0)    11464 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/autofit/afscript.h
+-rw-r--r--   0 root         (0) root         (0)    20127 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/autofit/afshaper.c
+-rw-r--r--   0 root         (0) root         (0)     1655 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/autofit/afshaper.h
+-rw-r--r--   0 root         (0) root         (0)    15115 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/autofit/afstyles.h
+-rw-r--r--   0 root         (0) root         (0)    18624 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/autofit/aftypes.h
+-rw-r--r--   0 root         (0) root         (0)      872 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/autofit/afws-decl.h
+-rw-r--r--   0 root         (0) root         (0)      966 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/autofit/afws-iter.h
+-rw-r--r--   0 root         (0) root         (0)      832 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/autofit/autofit.c
+-rw-r--r--   0 root         (0) root         (0)     3310 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/autofit/ft-hb.c
+-rw-r--r--   0 root         (0) root         (0)     1463 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/autofit/ft-hb.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:27.212826 xpydf-0.1.6/src/freetype/src/base/
+-rw-r--r--   0 root         (0) root         (0)     4906 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/base/ftadvanc.c
+-rw-r--r--   0 root         (0) root         (0)      980 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/base/ftbase.c
+-rw-r--r--   0 root         (0) root         (0)     2651 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/base/ftbase.h
+-rw-r--r--   0 root         (0) root         (0)    14346 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/base/ftbbox.c
+-rw-r--r--   0 root         (0) root         (0)     2177 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/base/ftbdf.c
+-rw-r--r--   0 root         (0) root         (0)    28296 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/base/ftbitmap.c
+-rw-r--r--   0 root         (0) root         (0)    28205 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/base/ftcalc.c
+-rw-r--r--   0 root         (0) root         (0)     2540 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/base/ftcid.c
+-rw-r--r--   0 root         (0) root         (0)     3416 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/base/ftcolor.c
+-rw-r--r--   0 root         (0) root         (0)    23926 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/base/ftdbgmem.c
+-rw-r--r--   0 root         (0) root         (0)    14105 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/base/ftdebug.c
+-rw-r--r--   0 root         (0) root         (0)     1267 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/base/fterrors.c
+-rw-r--r--   0 root         (0) root         (0)     1203 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/base/ftfntfmt.c
+-rw-r--r--   0 root         (0) root         (0)     1551 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/base/ftfstype.c
+-rw-r--r--   0 root         (0) root         (0)     1355 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/base/ftgasp.c
+-rw-r--r--   0 root         (0) root         (0)    11421 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/base/ftgloadr.c
+-rw-r--r--   0 root         (0) root         (0)    24220 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/base/ftglyph.c
+-rw-r--r--   0 root         (0) root         (0)     3125 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/base/ftgxval.c
+-rw-r--r--   0 root         (0) root         (0)     6657 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/base/fthash.c
+-rw-r--r--   0 root         (0) root         (0)     6339 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/base/ftinit.c
+-rw-r--r--   0 root         (0) root         (0)    11455 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/base/ftlcdfil.c
+-rw-r--r--   0 root         (0) root         (0)    31521 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/base/ftmac.c
+-rw-r--r--   0 root         (0) root         (0)    18084 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/base/ftmm.c
+-rw-r--r--   0 root         (0) root         (0)   161883 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/base/ftobjs.c
+-rw-r--r--   0 root         (0) root         (0)     2216 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/base/ftotval.c
+-rw-r--r--   0 root         (0) root         (0)    28599 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/base/ftoutln.c
+-rw-r--r--   0 root         (0) root         (0)     1245 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/base/ftpatent.c
+-rw-r--r--   0 root         (0) root         (0)     3730 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/base/ftpfr.c
+-rw-r--r--   0 root         (0) root         (0)     7500 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/base/ftpsprop.c
+-rw-r--r--   0 root         (0) root         (0)    29493 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/base/ftrfork.c
+-rw-r--r--   0 root         (0) root         (0)     4580 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/base/ftsnames.c
+-rw-r--r--   0 root         (0) root         (0)    19273 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/base/ftstream.c
+-rw-r--r--   0 root         (0) root         (0)    64724 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/base/ftstroke.c
+-rw-r--r--   0 root         (0) root         (0)     5374 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/base/ftsynth.c
+-rw-r--r--   0 root         (0) root         (0)     8149 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/base/ftsystem.c
+-rw-r--r--   0 root         (0) root         (0)    10565 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/base/fttrigon.c
+-rw-r--r--   0 root         (0) root         (0)     3047 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/base/fttype1.c
+-rw-r--r--   0 root         (0) root         (0)    10171 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/base/ftutil.c
+-rw-r--r--   0 root         (0) root         (0)     1306 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/base/ftwinfnt.c
+-rw-r--r--   0 root         (0) root         (0)     8743 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/base/md5.c
+-rw-r--r--   0 root         (0) root         (0)     1410 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/base/md5.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:27.249248 xpydf-0.1.6/src/freetype/src/bdf/
+-rw-r--r--   0 root         (0) root         (0)     1234 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/bdf/bdf.c
+-rw-r--r--   0 root         (0) root         (0)     8121 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/bdf/bdf.h
+-rw-r--r--   0 root         (0) root         (0)    29163 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/bdf/bdfdrivr.c
+-rw-r--r--   0 root         (0) root         (0)     1772 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/bdf/bdfdrivr.h
+-rw-r--r--   0 root         (0) root         (0)     1584 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/bdf/bdferror.h
+-rw-r--r--   0 root         (0) root         (0)    68231 2023-05-23 14:26:12.000000 xpydf-0.1.6/src/freetype/src/bdf/bdflib.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:27.256932 xpydf-0.1.6/src/freetype/src/bzip2/
+-rw-r--r--   0 root         (0) root         (0)    12870 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/bzip2/ftbzip2.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:27.360613 xpydf-0.1.6/src/freetype/src/cache/
+-rw-r--r--   0 root         (0) root         (0)      771 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cache/ftcache.c
+-rw-r--r--   0 root         (0) root         (0)    18033 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cache/ftcbasic.c
+-rw-r--r--   0 root         (0) root         (0)    14006 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cache/ftccache.c
+-rw-r--r--   0 root         (0) root         (0)    15484 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cache/ftccache.h
+-rw-r--r--   0 root         (0) root         (0)     2220 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cache/ftccback.h
+-rw-r--r--   0 root         (0) root         (0)     9711 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cache/ftccmap.c
+-rw-r--r--   0 root         (0) root         (0)      999 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cache/ftcerror.h
+-rw-r--r--   0 root         (0) root         (0)     4964 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cache/ftcglyph.c
+-rw-r--r--   0 root         (0) root         (0)    11116 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cache/ftcglyph.h
+-rw-r--r--   0 root         (0) root         (0)     3677 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cache/ftcimage.c
+-rw-r--r--   0 root         (0) root         (0)     2675 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cache/ftcimage.h
+-rw-r--r--   0 root         (0) root         (0)    17267 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cache/ftcmanag.c
+-rw-r--r--   0 root         (0) root         (0)     5734 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cache/ftcmanag.h
+-rw-r--r--   0 root         (0) root         (0)     6868 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cache/ftcmru.c
+-rw-r--r--   0 root         (0) root         (0)     8525 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cache/ftcmru.h
+-rw-r--r--   0 root         (0) root         (0)    11958 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cache/ftcsbits.c
+-rw-r--r--   0 root         (0) root         (0)     2191 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cache/ftcsbits.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:27.449668 xpydf-0.1.6/src/freetype/src/cff/
+-rw-r--r--   0 root         (0) root         (0)      725 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cff/cff.c
+-rw-r--r--   0 root         (0) root         (0)     7312 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cff/cffcmap.c
+-rw-r--r--   0 root         (0) root         (0)     2181 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cff/cffcmap.h
+-rw-r--r--   0 root         (0) root         (0)    39514 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cff/cffdrivr.c
+-rw-r--r--   0 root         (0) root         (0)      752 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cff/cffdrivr.h
+-rw-r--r--   0 root         (0) root         (0)      959 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cff/cfferrs.h
+-rw-r--r--   0 root         (0) root         (0)    26335 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cff/cffgload.c
+-rw-r--r--   0 root         (0) root         (0)     1523 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cff/cffgload.h
+-rw-r--r--   0 root         (0) root         (0)    75411 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cff/cffload.c
+-rw-r--r--   0 root         (0) root         (0)     3298 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cff/cffload.h
+-rw-r--r--   0 root         (0) root         (0)    35405 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cff/cffobjs.c
+-rw-r--r--   0 root         (0) root         (0)     1940 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cff/cffobjs.h
+-rw-r--r--   0 root         (0) root         (0)    39397 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cff/cffparse.c
+-rw-r--r--   0 root         (0) root         (0)     3326 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cff/cffparse.h
+-rw-r--r--   0 root         (0) root         (0)     6772 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cff/cfftoken.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:27.534556 xpydf-0.1.6/src/freetype/src/cid/
+-rw-r--r--   0 root         (0) root         (0)      958 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cid/ciderrs.h
+-rw-r--r--   0 root         (0) root         (0)    20567 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cid/cidgload.c
+-rw-r--r--   0 root         (0) root         (0)     1456 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cid/cidgload.h
+-rw-r--r--   0 root         (0) root         (0)    25446 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cid/cidload.c
+-rw-r--r--   0 root         (0) root         (0)     1115 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cid/cidload.h
+-rw-r--r--   0 root         (0) root         (0)    13878 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cid/cidobjs.c
+-rw-r--r--   0 root         (0) root         (0)     3412 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cid/cidobjs.h
+-rw-r--r--   0 root         (0) root         (0)     8770 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cid/cidparse.c
+-rw-r--r--   0 root         (0) root         (0)     3518 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cid/cidparse.h
+-rw-r--r--   0 root         (0) root         (0)     7557 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cid/cidriver.c
+-rw-r--r--   0 root         (0) root         (0)      772 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cid/cidriver.h
+-rw-r--r--   0 root         (0) root         (0)     4387 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cid/cidtoken.h
+-rw-r--r--   0 root         (0) root         (0)      710 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/cid/type1cid.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:27.547608 xpydf-0.1.6/src/freetype/src/dlg/
+-rw-r--r--   0 root         (0) root         (0)    21039 2023-05-22 06:59:35.000000 xpydf-0.1.6/src/freetype/src/dlg/dlg.c
+-rw-r--r--   0 root         (0) root         (0)      762 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/dlg/dlgwrap.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:27.737118 xpydf-0.1.6/src/freetype/src/gxvalid/
+-rw-r--r--   0 root         (0) root         (0)     1133 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gxvalid/gxvalid.c
+-rw-r--r--   0 root         (0) root         (0)     2869 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gxvalid/gxvalid.h
+-rw-r--r--   0 root         (0) root         (0)     9637 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gxvalid/gxvbsln.c
+-rw-r--r--   0 root         (0) root         (0)    54281 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gxvalid/gxvcommn.c
+-rw-r--r--   0 root         (0) root         (0)    22980 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gxvalid/gxvcommn.h
+-rw-r--r--   0 root         (0) root         (0)     1333 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gxvalid/gxverror.h
+-rw-r--r--   0 root         (0) root         (0)     9949 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gxvalid/gxvfeat.c
+-rw-r--r--   0 root         (0) root         (0)     6054 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gxvalid/gxvfeat.h
+-rw-r--r--   0 root         (0) root         (0)    13317 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gxvalid/gxvfgen.c
+-rw-r--r--   0 root         (0) root         (0)    20588 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gxvalid/gxvjust.c
+-rw-r--r--   0 root         (0) root         (0)    27203 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gxvalid/gxvkern.c
+-rw-r--r--   0 root         (0) root         (0)     7139 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gxvalid/gxvlcar.c
+-rw-r--r--   0 root         (0) root         (0)     8348 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gxvalid/gxvmod.c
+-rw-r--r--   0 root         (0) root         (0)     1093 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gxvalid/gxvmod.h
+-rw-r--r--   0 root         (0) root         (0)     8297 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gxvalid/gxvmort.c
+-rw-r--r--   0 root         (0) root         (0)     2971 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gxvalid/gxvmort.h
+-rw-r--r--   0 root         (0) root         (0)     4329 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gxvalid/gxvmort0.c
+-rw-r--r--   0 root         (0) root         (0)     8122 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gxvalid/gxvmort1.c
+-rw-r--r--   0 root         (0) root         (0)    10023 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gxvalid/gxvmort2.c
+-rw-r--r--   0 root         (0) root         (0)     3760 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gxvalid/gxvmort4.c
+-rw-r--r--   0 root         (0) root         (0)     8009 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gxvalid/gxvmort5.c
+-rw-r--r--   0 root         (0) root         (0)     5208 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gxvalid/gxvmorx.c
+-rw-r--r--   0 root         (0) root         (0)     2076 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gxvalid/gxvmorx.h
+-rw-r--r--   0 root         (0) root         (0)     3126 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gxvalid/gxvmorx0.c
+-rw-r--r--   0 root         (0) root         (0)     8464 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gxvalid/gxvmorx1.c
+-rw-r--r--   0 root         (0) root         (0)    10356 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gxvalid/gxvmorx2.c
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gxvalid/gxvmorx4.c
+-rw-r--r--   0 root         (0) root         (0)     7285 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gxvalid/gxvmorx5.c
+-rw-r--r--   0 root         (0) root         (0)     7216 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gxvalid/gxvopbd.c
+-rw-r--r--   0 root         (0) root         (0)    10208 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gxvalid/gxvprop.c
+-rw-r--r--   0 root         (0) root         (0)     9558 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gxvalid/gxvtrak.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:27.870026 xpydf-0.1.6/src/freetype/src/gzip/
+-rw-r--r--   0 root         (0) root         (0)     5182 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gzip/adler32.c
+-rw-r--r--   0 root         (0) root         (0)    32225 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gzip/crc32.c
+-rw-r--r--   0 root         (0) root         (0)   591749 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gzip/crc32.h
+-rw-r--r--   0 root         (0) root         (0)    20073 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gzip/ftgzip.c
+-rw-r--r--   0 root         (0) root         (0)    16625 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gzip/ftzconf.h
+-rw-r--r--   0 root         (0) root         (0)     6843 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gzip/gzguts.h
+-rw-r--r--   0 root         (0) root         (0)    12933 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gzip/inffast.c
+-rw-r--r--   0 root         (0) root         (0)      434 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gzip/inffast.h
+-rw-r--r--   0 root         (0) root         (0)     6332 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gzip/inffixed.h
+-rw-r--r--   0 root         (0) root         (0)    56083 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gzip/inflate.c
+-rw-r--r--   0 root         (0) root         (0)     6745 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gzip/inflate.h
+-rw-r--r--   0 root         (0) root         (0)    12993 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gzip/inftrees.c
+-rw-r--r--   0 root         (0) root         (0)     3000 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gzip/inftrees.h
+-rw-r--r--   0 root         (0) root         (0)    98004 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gzip/zlib.h
+-rw-r--r--   0 root         (0) root         (0)     7355 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gzip/zutil.c
+-rw-r--r--   0 root         (0) root         (0)     7398 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/gzip/zutil.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:27.888233 xpydf-0.1.6/src/freetype/src/lzw/
+-rw-r--r--   0 root         (0) root         (0)     9899 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/lzw/ftlzw.c
+-rw-r--r--   0 root         (0) root         (0)    10565 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/lzw/ftzopen.c
+-rw-r--r--   0 root         (0) root         (0)     5099 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/lzw/ftzopen.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:27.968903 xpydf-0.1.6/src/freetype/src/otvalid/
+-rw-r--r--   0 root         (0) root         (0)      773 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/otvalid/otvalid.c
+-rw-r--r--   0 root         (0) root         (0)     2127 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/otvalid/otvalid.h
+-rw-r--r--   0 root         (0) root         (0)     7882 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/otvalid/otvbase.c
+-rw-r--r--   0 root         (0) root         (0)    27533 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/otvalid/otvcommn.c
+-rw-r--r--   0 root         (0) root         (0)    19343 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/otvalid/otvcommn.h
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/otvalid/otverror.h
+-rw-r--r--   0 root         (0) root         (0)     8882 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/otvalid/otvgdef.c
+-rw-r--r--   0 root         (0) root         (0)    29663 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/otvalid/otvgpos.c
+-rw-r--r--   0 root         (0) root         (0)      786 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/otvalid/otvgpos.h
+-rw-r--r--   0 root         (0) root         (0)    18463 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/otvalid/otvgsub.c
+-rw-r--r--   0 root         (0) root         (0)     7126 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/otvalid/otvjstf.c
+-rw-r--r--   0 root         (0) root         (0)    13656 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/otvalid/otvmath.c
+-rw-r--r--   0 root         (0) root         (0)     7207 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/otvalid/otvmod.c
+-rw-r--r--   0 root         (0) root         (0)      778 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/otvalid/otvmod.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:28.020630 xpydf-0.1.6/src/freetype/src/pcf/
+-rw-r--r--   0 root         (0) root         (0)     1253 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/pcf/pcf.c
+-rw-r--r--   0 root         (0) root         (0)     6373 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/pcf/pcf.h
+-rw-r--r--   0 root         (0) root         (0)    21798 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/pcf/pcfdrivr.c
+-rw-r--r--   0 root         (0) root         (0)     1358 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/pcf/pcfdrivr.h
+-rw-r--r--   0 root         (0) root         (0)      959 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/pcf/pcferror.h
+-rw-r--r--   0 root         (0) root         (0)    50270 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/pcf/pcfread.c
+-rw-r--r--   0 root         (0) root         (0)     1361 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/pcf/pcfread.h
+-rw-r--r--   0 root         (0) root         (0)     3382 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/pcf/pcfutil.c
+-rw-r--r--   0 root         (0) root         (0)     1649 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/pcf/pcfutil.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:28.111184 xpydf-0.1.6/src/freetype/src/pfr/
+-rw-r--r--   0 root         (0) root         (0)      708 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/pfr/pfr.c
+-rw-r--r--   0 root         (0) root         (0)     4519 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/pfr/pfrcmap.c
+-rw-r--r--   0 root         (0) root         (0)      920 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/pfr/pfrcmap.h
+-rw-r--r--   0 root         (0) root         (0)     5618 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/pfr/pfrdrivr.c
+-rw-r--r--   0 root         (0) root         (0)      773 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/pfr/pfrdrivr.h
+-rw-r--r--   0 root         (0) root         (0)      962 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/pfr/pfrerror.h
+-rw-r--r--   0 root         (0) root         (0)    21931 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/pfr/pfrgload.c
+-rw-r--r--   0 root         (0) root         (0)     1059 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/pfr/pfrgload.h
+-rw-r--r--   0 root         (0) root         (0)    28988 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/pfr/pfrload.c
+-rw-r--r--   0 root         (0) root         (0)     3425 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/pfr/pfrload.h
+-rw-r--r--   0 root         (0) root         (0)    17487 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/pfr/pfrobjs.c
+-rw-r--r--   0 root         (0) root         (0)     2135 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/pfr/pfrobjs.h
+-rw-r--r--   0 root         (0) root         (0)    21398 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/pfr/pfrsbit.c
+-rw-r--r--   0 root         (0) root         (0)      878 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/pfr/pfrsbit.h
+-rw-r--r--   0 root         (0) root         (0)     8090 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/pfr/pfrtypes.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:28.342495 xpydf-0.1.6/src/freetype/src/psaux/
+-rw-r--r--   0 root         (0) root         (0)    25277 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/psaux/afmparse.c
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/psaux/afmparse.h
+-rw-r--r--   0 root         (0) root         (0)    68657 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/psaux/cffdecode.c
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/psaux/cffdecode.h
+-rw-r--r--   0 root         (0) root         (0)     6515 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/psaux/psarrst.c
+-rw-r--r--   0 root         (0) root         (0)     3476 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/psaux/psarrst.h
+-rw-r--r--   0 root         (0) root         (0)      945 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/psaux/psaux.c
+-rw-r--r--   0 root         (0) root         (0)     1003 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/psaux/psauxerr.h
+-rw-r--r--   0 root         (0) root         (0)     4847 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/psaux/psauxmod.c
+-rw-r--r--   0 root         (0) root         (0)     1247 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/psaux/psauxmod.h
+-rw-r--r--   0 root         (0) root         (0)    19898 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/psaux/psblues.c
+-rw-r--r--   0 root         (0) root         (0)     5995 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/psaux/psblues.h
+-rw-r--r--   0 root         (0) root         (0)    11649 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/psaux/psconv.c
+-rw-r--r--   0 root         (0) root         (0)     1700 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/psaux/psconv.h
+-rw-r--r--   0 root         (0) root         (0)     2089 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/psaux/pserror.c
+-rw-r--r--   0 root         (0) root         (0)     4024 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/psaux/pserror.h
+-rw-r--r--   0 root         (0) root         (0)     3743 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/psaux/psfixed.h
+-rw-r--r--   0 root         (0) root         (0)    19883 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/psaux/psfont.c
+-rw-r--r--   0 root         (0) root         (0)     5402 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/psaux/psfont.h
+-rw-r--r--   0 root         (0) root         (0)    25620 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/psaux/psft.c
+-rw-r--r--   0 root         (0) root         (0)     5394 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/psaux/psft.h
+-rw-r--r--   0 root         (0) root         (0)     4501 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/psaux/psglue.h
+-rw-r--r--   0 root         (0) root         (0)    66109 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/psaux/pshints.c
+-rw-r--r--   0 root         (0) root         (0)     9869 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/psaux/pshints.h
+-rw-r--r--   0 root         (0) root         (0)   105884 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/psaux/psintrp.c
+-rw-r--r--   0 root         (0) root         (0)     3074 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/psaux/psintrp.h
+-rw-r--r--   0 root         (0) root         (0)    66473 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/psaux/psobjs.c
+-rw-r--r--   0 root         (0) root         (0)    10283 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/psaux/psobjs.h
+-rw-r--r--   0 root         (0) root         (0)     3522 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/psaux/psread.c
+-rw-r--r--   0 root         (0) root         (0)     2299 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/psaux/psread.h
+-rw-r--r--   0 root         (0) root         (0)     9233 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/psaux/psstack.c
+-rw-r--r--   0 root         (0) root         (0)     3695 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/psaux/psstack.h
+-rw-r--r--   0 root         (0) root         (0)     2674 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/psaux/pstypes.h
+-rw-r--r--   0 root         (0) root         (0)    11948 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/psaux/t1cmap.c
+-rw-r--r--   0 root         (0) root         (0)     3282 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/psaux/t1cmap.h
+-rw-r--r--   0 root         (0) root         (0)    60726 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/psaux/t1decode.c
+-rw-r--r--   0 root         (0) root         (0)     2024 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/psaux/t1decode.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:28.408100 xpydf-0.1.6/src/freetype/src/pshinter/
+-rw-r--r--   0 root         (0) root         (0)    58961 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/pshinter/pshalgo.c
+-rw-r--r--   0 root         (0) root         (0)     6616 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/pshinter/pshalgo.h
+-rw-r--r--   0 root         (0) root         (0)    22377 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/pshinter/pshglob.c
+-rw-r--r--   0 root         (0) root         (0)     4860 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/pshinter/pshglob.h
+-rw-r--r--   0 root         (0) root         (0)      671 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/pshinter/pshinter.c
+-rw-r--r--   0 root         (0) root         (0)     3002 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/pshinter/pshmod.c
+-rw-r--r--   0 root         (0) root         (0)      741 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/pshinter/pshmod.h
+-rw-r--r--   0 root         (0) root         (0)      978 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/pshinter/pshnterr.h
+-rw-r--r--   0 root         (0) root         (0)    31754 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/pshinter/pshrec.c
+-rw-r--r--   0 root         (0) root         (0)     4103 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/pshinter/pshrec.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:28.437828 xpydf-0.1.6/src/freetype/src/psnames/
+-rw-r--r--   0 root         (0) root         (0)    16268 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/psnames/psmodule.c
+-rw-r--r--   0 root         (0) root         (0)      748 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/psnames/psmodule.h
+-rw-r--r--   0 root         (0) root         (0)      999 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/psnames/psnamerr.h
+-rw-r--r--   0 root         (0) root         (0)      622 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/psnames/psnames.c
+-rw-r--r--   0 root         (0) root         (0)   268144 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/psnames/pstables.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:28.492904 xpydf-0.1.6/src/freetype/src/raster/
+-rw-r--r--   0 root         (0) root         (0)     2969 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/raster/ftmisc.h
+-rw-r--r--   0 root         (0) root         (0)    84634 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/raster/ftraster.c
+-rw-r--r--   0 root         (0) root         (0)     1092 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/raster/ftraster.h
+-rw-r--r--   0 root         (0) root         (0)     5557 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/raster/ftrend1.c
+-rw-r--r--   0 root         (0) root         (0)      755 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/raster/ftrend1.h
+-rw-r--r--   0 root         (0) root         (0)      654 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/raster/raster.c
+-rw-r--r--   0 root         (0) root         (0)     1005 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/raster/rasterrs.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:28.556094 xpydf-0.1.6/src/freetype/src/sdf/
+-rw-r--r--   0 root         (0) root         (0)    38453 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sdf/ftbsdf.c
+-rw-r--r--   0 root         (0) root         (0)   112098 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sdf/ftsdf.c
+-rw-r--r--   0 root         (0) root         (0)     2914 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sdf/ftsdf.h
+-rw-r--r--   0 root         (0) root         (0)     4108 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sdf/ftsdfcommon.c
+-rw-r--r--   0 root         (0) root         (0)     4007 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sdf/ftsdfcommon.h
+-rw-r--r--   0 root         (0) root         (0)      848 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sdf/ftsdferrs.h
+-rw-r--r--   0 root         (0) root         (0)    16276 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sdf/ftsdfrend.c
+-rw-r--r--   0 root         (0) root         (0)     3386 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sdf/ftsdfrend.h
+-rw-r--r--   0 root         (0) root         (0)      735 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sdf/sdf.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:28.771273 xpydf-0.1.6/src/freetype/src/sfnt/
+-rw-r--r--   0 root         (0) root         (0)    13188 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sfnt/pngshim.c
+-rw-r--r--   0 root         (0) root         (0)     1184 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sfnt/pngshim.h
+-rw-r--r--   0 root         (0) root         (0)    36683 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sfnt/sfdriver.c
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sfnt/sfdriver.h
+-rw-r--r--   0 root         (0) root         (0)      966 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sfnt/sferrors.h
+-rw-r--r--   0 root         (0) root         (0)      908 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sfnt/sfnt.c
+-rw-r--r--   0 root         (0) root         (0)    48936 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sfnt/sfobjs.c
+-rw-r--r--   0 root         (0) root         (0)     1417 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sfnt/sfobjs.h
+-rw-r--r--   0 root         (0) root         (0)    12342 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sfnt/sfwoff.c
+-rw-r--r--   0 root         (0) root         (0)      865 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sfnt/sfwoff.h
+-rw-r--r--   0 root         (0) root         (0)    66294 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sfnt/sfwoff2.c
+-rw-r--r--   0 root         (0) root         (0)     2124 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sfnt/sfwoff2.h
+-rw-r--r--   0 root         (0) root         (0)     6247 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sfnt/ttbdf.c
+-rw-r--r--   0 root         (0) root         (0)     1029 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sfnt/ttbdf.h
+-rw-r--r--   0 root         (0) root         (0)   111890 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sfnt/ttcmap.c
+-rw-r--r--   0 root         (0) root         (0)     3727 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sfnt/ttcmap.h
+-rw-r--r--   0 root         (0) root         (0)     1227 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sfnt/ttcmapc.h
+-rw-r--r--   0 root         (0) root         (0)    62115 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sfnt/ttcolr.c
+-rw-r--r--   0 root         (0) root         (0)     2526 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sfnt/ttcolr.h
+-rw-r--r--   0 root         (0) root         (0)     7964 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sfnt/ttcpal.c
+-rw-r--r--   0 root         (0) root         (0)     1036 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sfnt/ttcpal.h
+-rw-r--r--   0 root         (0) root         (0)     7232 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sfnt/ttkern.c
+-rw-r--r--   0 root         (0) root         (0)     1199 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sfnt/ttkern.h
+-rw-r--r--   0 root         (0) root         (0)    40643 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sfnt/ttload.c
+-rw-r--r--   0 root         (0) root         (0)     2507 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sfnt/ttload.h
+-rw-r--r--   0 root         (0) root         (0)     8552 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sfnt/ttmtx.c
+-rw-r--r--   0 root         (0) root         (0)     1289 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sfnt/ttmtx.h
+-rw-r--r--   0 root         (0) root         (0)    13197 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sfnt/ttpost.c
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sfnt/ttpost.h
+-rw-r--r--   0 root         (0) root         (0)    48308 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sfnt/ttsbit.c
+-rw-r--r--   0 root         (0) root         (0)     1672 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sfnt/ttsbit.h
+-rw-r--r--   0 root         (0) root         (0)    10640 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sfnt/ttsvg.c
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sfnt/ttsvg.h
+-rw-r--r--   0 root         (0) root         (0)     4350 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sfnt/woff2tags.c
+-rw-r--r--   0 root         (0) root         (0)      867 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/sfnt/woff2tags.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:28.801919 xpydf-0.1.6/src/freetype/src/smooth/
+-rw-r--r--   0 root         (0) root         (0)    62480 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/smooth/ftgrays.c
+-rw-r--r--   0 root         (0) root         (0)     1260 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/smooth/ftgrays.h
+-rw-r--r--   0 root         (0) root         (0)      997 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/smooth/ftsmerrs.h
+-rw-r--r--   0 root         (0) root         (0)    16549 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/smooth/ftsmooth.c
+-rw-r--r--   0 root         (0) root         (0)      751 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/smooth/ftsmooth.h
+-rw-r--r--   0 root         (0) root         (0)      657 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/smooth/smooth.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:28.829907 xpydf-0.1.6/src/freetype/src/svg/
+-rw-r--r--   0 root         (0) root         (0)     8897 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/svg/ftsvg.c
+-rw-r--r--   0 root         (0) root         (0)      810 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/svg/ftsvg.h
+-rw-r--r--   0 root         (0) root         (0)      656 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/svg/svg.c
+-rw-r--r--   0 root         (0) root         (0)     1195 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/svg/svgtypes.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:28.889539 xpydf-0.1.6/src/freetype/src/tools/
+-rw-r--r--   0 root         (0) root         (0)    11420 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/tools/apinames.c
+-rwxr-xr-x   0 root         (0) root         (0)     4216 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/tools/chktrcmp.py
+-rw-r--r--   0 root         (0) root         (0)      770 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/tools/cordic.py
+-rw-r--r--   0 root         (0) root         (0)   107236 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/tools/glnames.py
+-rwxr-xr-x   0 root         (0) root         (0)     6188 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/tools/make_distribution_archives.py
+-rw-r--r--   0 root         (0) root         (0)     3969 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/tools/test_afm.c
+-rw-r--r--   0 root         (0) root         (0)     4191 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/tools/test_bbox.c
+-rw-r--r--   0 root         (0) root         (0)     4826 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/tools/test_trig.c
+-rw-r--r--   0 root         (0) root         (0)     9927 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/tools/vms_shorten_symbol.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:29.001632 xpydf-0.1.6/src/freetype/src/truetype/
+-rw-r--r--   0 root         (0) root         (0)      896 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/truetype/truetype.c
+-rw-r--r--   0 root         (0) root         (0)    22144 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/truetype/ttdriver.c
+-rw-r--r--   0 root         (0) root         (0)      748 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/truetype/ttdriver.h
+-rw-r--r--   0 root         (0) root         (0)      981 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/truetype/tterrors.h
+-rw-r--r--   0 root         (0) root         (0)    93929 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/truetype/ttgload.c
+-rw-r--r--   0 root         (0) root         (0)     1358 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/truetype/ttgload.h
+-rw-r--r--   0 root         (0) root         (0)   131819 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/truetype/ttgxvar.c
+-rw-r--r--   0 root         (0) root         (0)    13625 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/truetype/ttgxvar.h
+-rw-r--r--   0 root         (0) root         (0)   220265 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/truetype/ttinterp.c
+-rw-r--r--   0 root         (0) root         (0)    21599 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/truetype/ttinterp.h
+-rw-r--r--   0 root         (0) root         (0)    43577 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/truetype/ttobjs.c
+-rw-r--r--   0 root         (0) root         (0)    12076 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/truetype/ttobjs.h
+-rw-r--r--   0 root         (0) root         (0)    16553 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/truetype/ttpload.c
+-rw-r--r--   0 root         (0) root         (0)     1661 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/truetype/ttpload.h
+-rw-r--r--   0 root         (0) root         (0)    32091 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/truetype/ttsubpix.c
+-rw-r--r--   0 root         (0) root         (0)     3848 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/truetype/ttsubpix.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:29.091680 xpydf-0.1.6/src/freetype/src/type1/
+-rw-r--r--   0 root         (0) root         (0)    10669 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/type1/t1afm.c
+-rw-r--r--   0 root         (0) root         (0)     1285 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/type1/t1afm.h
+-rw-r--r--   0 root         (0) root         (0)    24329 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/type1/t1driver.c
+-rw-r--r--   0 root         (0) root         (0)      769 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/type1/t1driver.h
+-rw-r--r--   0 root         (0) root         (0)      969 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/type1/t1errors.h
+-rw-r--r--   0 root         (0) root         (0)    20367 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/type1/t1gload.c
+-rw-r--r--   0 root         (0) root         (0)     1193 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/type1/t1gload.h
+-rw-r--r--   0 root         (0) root         (0)    82040 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/type1/t1load.c
+-rw-r--r--   0 root         (0) root         (0)     3285 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/type1/t1load.h
+-rw-r--r--   0 root         (0) root         (0)    17437 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/type1/t1objs.c
+-rw-r--r--   0 root         (0) root         (0)     3452 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/type1/t1objs.h
+-rw-r--r--   0 root         (0) root         (0)    14896 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/type1/t1parse.c
+-rw-r--r--   0 root         (0) root         (0)     3735 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/type1/t1parse.h
+-rw-r--r--   0 root         (0) root         (0)     5083 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/type1/t1tokens.h
+-rw-r--r--   0 root         (0) root         (0)      720 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/type1/type1.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:29.150335 xpydf-0.1.6/src/freetype/src/type42/
+-rw-r--r--   0 root         (0) root         (0)     6579 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/type42/t42drivr.c
+-rw-r--r--   0 root         (0) root         (0)      739 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/type42/t42drivr.h
+-rw-r--r--   0 root         (0) root         (0)      973 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/type42/t42error.h
+-rw-r--r--   0 root         (0) root         (0)    19226 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/type42/t42objs.c
+-rw-r--r--   0 root         (0) root         (0)     2452 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/type42/t42objs.h
+-rw-r--r--   0 root         (0) root         (0)    40017 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/type42/t42parse.c
+-rw-r--r--   0 root         (0) root         (0)     2029 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/type42/t42parse.h
+-rw-r--r--   0 root         (0) root         (0)     1181 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/type42/t42types.h
+-rw-r--r--   0 root         (0) root         (0)      652 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/type42/type42.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:29.171289 xpydf-0.1.6/src/freetype/src/winfonts/
+-rw-r--r--   0 root         (0) root         (0)      988 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/winfonts/fnterrs.h
+-rw-r--r--   0 root         (0) root         (0)    35786 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/winfonts/winfnt.c
+-rw-r--r--   0 root         (0) root         (0)     3104 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/src/winfonts/winfnt.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:25.781780 xpydf-0.1.6/src/freetype/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:29.178170 xpydf-0.1.6/src/freetype/tests/scripts/
+-rwxr-xr-x   0 root         (0) root         (0)     8869 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/tests/scripts/download-test-fonts.py
+-rw-r--r--   0 root         (0) root         (0)    41515 2023-05-19 16:13:04.000000 xpydf-0.1.6/src/freetype/vms_make.com
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:29.261049 xpydf-0.1.6/src/xpdf-4.04/
+-rw-r--r--   0 root         (0) root         (0)     8196 2023-06-02 09:36:12.000000 xpydf-0.1.6/src/xpdf-4.04/.DS_Store
+-rw-r--r--   0 root         (0) root         (0)     1330 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/ANNOUNCE
+-rw-r--r--   0 root         (0) root         (0)   139475 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/CHANGES
+-rw-r--r--   0 root         (0) root         (0)     1053 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)    17982 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/COPYING
+-rw-r--r--   0 root         (0) root         (0)    35147 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/COPYING3
+-rw-r--r--   0 root         (0) root         (0)     5614 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/INSTALL
+-rw-r--r--   0 root         (0) root         (0)    13778 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/README
+-rw-r--r--   0 root         (0) root         (0)     2002 2023-06-09 07:28:33.000000 xpydf-0.1.6/src/xpdf-4.04/aconf.h
+-rw-r--r--   0 root         (0) root         (0)     1985 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/aconf.h.in
+-rw-r--r--   0 root         (0) root         (0)      941 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/aconf2.h
+-rw-r--r--   0 root         (0) root         (0)    10676 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/cmake-config.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:29.337066 xpydf-0.1.6/src/xpdf-4.04/fofi/
+-rw-r--r--   0 root         (0) root         (0)     3275 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/fofi/FoFiBase.cc
+-rw-r--r--   0 root         (0) root         (0)     1344 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/fofi/FoFiBase.h
+-rw-r--r--   0 root         (0) root         (0)    14853 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/fofi/FoFiEncodings.cc
+-rw-r--r--   0 root         (0) root         (0)     1005 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/fofi/FoFiEncodings.h
+-rw-r--r--   0 root         (0) root         (0)    21889 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/fofi/FoFiIdentifier.cc
+-rw-r--r--   0 root         (0) root         (0)     1659 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/fofi/FoFiIdentifier.h
+-rw-r--r--   0 root         (0) root         (0)    77637 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/fofi/FoFiTrueType.cc
+-rw-r--r--   0 root         (0) root         (0)     8227 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/fofi/FoFiTrueType.h
+-rw-r--r--   0 root         (0) root         (0)     8796 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/fofi/FoFiType1.cc
+-rw-r--r--   0 root         (0) root         (0)     1434 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/fofi/FoFiType1.h
+-rw-r--r--   0 root         (0) root         (0)    97383 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/fofi/FoFiType1C.cc
+-rw-r--r--   0 root         (0) root         (0)     8299 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/fofi/FoFiType1C.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:29.456580 xpydf-0.1.6/src/xpdf-4.04/goo/
+-rw-r--r--   0 root         (0) root         (0)     2748 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/goo/FixedPoint.cc
+-rw-r--r--   0 root         (0) root         (0)     7361 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/goo/FixedPoint.h
+-rw-r--r--   0 root         (0) root         (0)     6201 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/goo/GHash.cc
+-rw-r--r--   0 root         (0) root         (0)     2209 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/goo/GHash.h
+-rw-r--r--   0 root         (0) root         (0)     2276 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/goo/GList.cc
+-rw-r--r--   0 root         (0) root         (0)     2724 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/goo/GList.h
+-rw-r--r--   0 root         (0) root         (0)     2629 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/goo/GMutex.h
+-rw-r--r--   0 root         (0) root         (0)    17722 2023-06-02 09:35:24.000000 xpydf-0.1.6/src/xpdf-4.04/goo/GString.cc
+-rw-r--r--   0 root         (0) root         (0)     4269 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/goo/GString.h
+-rw-r--r--   0 root         (0) root         (0)     2406 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/goo/Trace.cc
+-rw-r--r--   0 root         (0) root         (0)     1171 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/goo/Trace.h
+-rw-r--r--   0 root         (0) root         (0)    17381 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/goo/gfile.cc
+-rw-r--r--   0 root         (0) root         (0)     4565 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/goo/gfile.h
+-rw-r--r--   0 root         (0) root         (0)     8259 2023-03-01 15:38:49.000000 xpydf-0.1.6/src/xpdf-4.04/goo/gmem.cc
+-rw-r--r--   0 root         (0) root         (0)     2029 2023-03-01 15:38:49.000000 xpydf-0.1.6/src/xpdf-4.04/goo/gmem.h
+-rw-r--r--   0 root         (0) root         (0)     1005 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/goo/gmempp.cc
+-rw-r--r--   0 root         (0) root         (0)     1714 2023-03-01 15:38:49.000000 xpydf-0.1.6/src/xpdf-4.04/goo/gmempp.h
+-rw-r--r--   0 root         (0) root         (0)      562 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/goo/gtypes.h
+-rw-r--r--   0 root         (0) root         (0)     1583 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/goo/parseargs.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:29.695696 xpydf-0.1.6/src/xpdf-4.04/splash/
+-rw-r--r--   0 root         (0) root         (0)   230071 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/splash/Splash.cc
+-rw-r--r--   0 root         (0) root         (0)    20193 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/splash/Splash.h
+-rw-r--r--   0 root         (0) root         (0)     6603 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/splash/SplashBitmap.cc
+-rw-r--r--   0 root         (0) root         (0)     2881 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/splash/SplashBitmap.h
+-rw-r--r--   0 root         (0) root         (0)    11473 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/splash/SplashClip.cc
+-rw-r--r--   0 root         (0) root         (0)     4007 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/splash/SplashClip.h
+-rw-r--r--   0 root         (0) root         (0)      930 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/splash/SplashErrorCodes.h
+-rw-r--r--   0 root         (0) root         (0)    13929 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/splash/SplashFTFont.cc
+-rw-r--r--   0 root         (0) root         (0)     1345 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/splash/SplashFTFont.h
+-rw-r--r--   0 root         (0) root         (0)     8902 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/splash/SplashFTFontEngine.cc
+-rw-r--r--   0 root         (0) root         (0)     2248 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/splash/SplashFTFontEngine.h
+-rw-r--r--   0 root         (0) root         (0)     4055 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/splash/SplashFTFontFile.cc
+-rw-r--r--   0 root         (0) root         (0)     2241 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/splash/SplashFTFontFile.h
+-rw-r--r--   0 root         (0) root         (0)     4995 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/splash/SplashFont.cc
+-rw-r--r--   0 root         (0) root         (0)     3666 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/splash/SplashFont.h
+-rw-r--r--   0 root         (0) root         (0)     9673 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/splash/SplashFontEngine.cc
+-rw-r--r--   0 root         (0) root         (0)     3358 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/splash/SplashFontEngine.h
+-rw-r--r--   0 root         (0) root         (0)     1589 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/splash/SplashFontFile.cc
+-rw-r--r--   0 root         (0) root         (0)     2168 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/splash/SplashFontFile.h
+-rw-r--r--   0 root         (0) root         (0)      603 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/splash/SplashFontFileID.cc
+-rw-r--r--   0 root         (0) root         (0)      687 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/splash/SplashFontFileID.h
+-rw-r--r--   0 root         (0) root         (0)      758 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/splash/SplashGlyphBitmap.h
+-rw-r--r--   0 root         (0) root         (0)     9510 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/splash/SplashMath.h
+-rw-r--r--   0 root         (0) root         (0)     5135 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/splash/SplashPath.cc
+-rw-r--r--   0 root         (0) root         (0)     3876 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/splash/SplashPath.h
+-rw-r--r--   0 root         (0) root         (0)     1042 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/splash/SplashPattern.cc
+-rw-r--r--   0 root         (0) root         (0)     1447 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/splash/SplashPattern.h
+-rw-r--r--   0 root         (0) root         (0)     9844 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/splash/SplashScreen.cc
+-rw-r--r--   0 root         (0) root         (0)     2167 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/splash/SplashScreen.h
+-rw-r--r--   0 root         (0) root         (0)     9521 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/splash/SplashState.cc
+-rw-r--r--   0 root         (0) root         (0)     3669 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/splash/SplashState.h
+-rw-r--r--   0 root         (0) root         (0)     4155 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/splash/SplashTypes.h
+-rw-r--r--   0 root         (0) root         (0)    17088 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/splash/SplashXPath.cc
+-rw-r--r--   0 root         (0) root         (0)     3761 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/splash/SplashXPath.h
+-rw-r--r--   0 root         (0) root         (0)    12936 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/splash/SplashXPathScanner.cc
+-rw-r--r--   0 root         (0) root         (0)     2482 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/splash/SplashXPathScanner.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:30.636762 xpydf-0.1.6/src/xpdf-4.04/xpdf/
+-rw-r--r--   0 root         (0) root         (0)   104374 2023-05-15 13:37:05.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/AcroForm.cc
+-rw-r--r--   0 root         (0) root         (0)     5269 2023-05-15 13:34:50.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/AcroForm.h
+-rw-r--r--   0 root         (0) root         (0)    38840 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/Annot.cc
+-rw-r--r--   0 root         (0) root         (0)     4895 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/Annot.h
+-rw-r--r--   0 root         (0) root         (0)     1385 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/Array.cc
+-rw-r--r--   0 root         (0) root         (0)     1400 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/Array.h
+-rw-r--r--   0 root         (0) root         (0)     1387 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/BuiltinFont.cc
+-rw-r--r--   0 root         (0) root         (0)     1080 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/BuiltinFont.h
+-rw-r--r--   0 root         (0) root         (0)   229548 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/BuiltinFontTables.cc
+-rw-r--r--   0 root         (0) root         (0)      556 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/BuiltinFontTables.h
+-rw-r--r--   0 root         (0) root         (0)    10417 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/CMap.cc
+-rw-r--r--   0 root         (0) root         (0)     3178 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/CMap.h
+-rw-r--r--   0 root         (0) root         (0)    28608 2023-05-15 13:29:26.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/Catalog.cc
+-rw-r--r--   0 root         (0) root         (0)     4742 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/Catalog.h
+-rw-r--r--   0 root         (0) root         (0)    19175 2023-04-13 10:47:41.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/CharCodeToUnicode.cc
+-rw-r--r--   0 root         (0) root         (0)     3702 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/CharCodeToUnicode.h
+-rw-r--r--   0 root         (0) root         (0)      526 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/CharTypes.h
+-rw-r--r--   0 root         (0) root         (0)     8379 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/CompactFontTables.h
+-rw-r--r--   0 root         (0) root         (0)    45644 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/Decrypt.cc
+-rw-r--r--   0 root         (0) root         (0)     3530 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/Decrypt.h
+-rw-r--r--   0 root         (0) root         (0)     2993 2023-05-15 08:40:36.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/Dict.cc
+-rw-r--r--   0 root         (0) root         (0)     2088 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/Dict.h
+-rw-r--r--   0 root         (0) root         (0)     5247 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/DisplayState.cc
+-rw-r--r--   0 root         (0) root         (0)     5225 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/DisplayState.h
+-rw-r--r--   0 root         (0) root         (0)     2123 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/Error.cc
+-rw-r--r--   0 root         (0) root         (0)     1353 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/Error.h
+-rw-r--r--   0 root         (0) root         (0)      984 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/ErrorCodes.h
+-rw-r--r--   0 root         (0) root         (0)    21312 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/FontEncodingTables.cc
+-rw-r--r--   0 root         (0) root         (0)      564 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/FontEncodingTables.h
+-rw-r--r--   0 root         (0) root         (0)    36553 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/Function.cc
+-rw-r--r--   0 root         (0) root         (0)     6722 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/Function.h
+-rw-r--r--   0 root         (0) root         (0)   144837 2023-06-02 09:35:24.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/Gfx.cc
+-rw-r--r--   0 root         (0) root         (0)    11911 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/Gfx.h
+-rw-r--r--   0 root         (0) root         (0)    65646 2023-06-02 09:35:24.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/GfxFont.cc
+-rw-r--r--   0 root         (0) root         (0)    12828 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/GfxFont.h
+-rw-r--r--   0 root         (0) root         (0)   120789 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/GfxState.cc
+-rw-r--r--   0 root         (0) root         (0)    43452 2023-06-02 09:35:24.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/GfxState.h
+-rw-r--r--   0 root         (0) root         (0)   103543 2023-05-19 16:11:38.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/GlobalParams.cc
+-rw-r--r--   0 root         (0) root         (0)    23054 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/GlobalParams.h
+-rw-r--r--   0 root         (0) root         (0)    34442 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/HTMLGen.cc
+-rw-r--r--   0 root         (0) root         (0)     3131 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/HTMLGen.h
+-rw-r--r--   0 root         (0) root         (0)    11293 2023-05-02 12:54:18.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/ImageOutputDev.cc
+-rw-r--r--   0 root         (0) root         (0)     3942 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/ImageOutputDev.h
+-rw-r--r--   0 root         (0) root         (0)     8327 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/JArithmeticDecoder.cc
+-rw-r--r--   0 root         (0) root         (0)     2802 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/JArithmeticDecoder.h
+-rw-r--r--   0 root         (0) root         (0)   109724 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/JBIG2Stream.cc
+-rw-r--r--   0 root         (0) root         (0)     4824 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/JBIG2Stream.h
+-rw-r--r--   0 root         (0) root         (0)   107255 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/JPXStream.cc
+-rw-r--r--   0 root         (0) root         (0)    11092 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/JPXStream.h
+-rw-r--r--   0 root         (0) root         (0)    11674 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/Lexer.cc
+-rw-r--r--   0 root         (0) root         (0)     2035 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/Lexer.h
+-rw-r--r--   0 root         (0) root         (0)    21632 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/Link.cc
+-rw-r--r--   0 root         (0) root         (0)    11370 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/Link.h
+-rw-r--r--   0 root         (0) root         (0)     2191 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/NameToCharCode.cc
+-rw-r--r--   0 root         (0) root         (0)      726 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/NameToCharCode.h
+-rw-r--r--   0 root         (0) root         (0)   117065 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/NameToUnicodeTable.h
+-rw-r--r--   0 root         (0) root         (0)     4471 2023-05-15 08:40:34.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/Object.cc
+-rw-r--r--   0 root         (0) root         (0)     9081 2023-05-15 08:40:32.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/Object.h
+-rw-r--r--   0 root         (0) root         (0)    12818 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/OptionalContent.cc
+-rw-r--r--   0 root         (0) root         (0)     3617 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/OptionalContent.h
+-rw-r--r--   0 root         (0) root         (0)     4001 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/Outline.cc
+-rw-r--r--   0 root         (0) root         (0)     1774 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/Outline.h
+-rw-r--r--   0 root         (0) root         (0)     4131 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/OutputDev.cc
+-rw-r--r--   0 root         (0) root         (0)     8935 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/OutputDev.h
+-rw-r--r--   0 root         (0) root         (0)    87382 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/PDF417Barcode.cc
+-rw-r--r--   0 root         (0) root         (0)      838 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/PDF417Barcode.h
+-rw-r--r--   0 root         (0) root         (0)    51111 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/PDFCore.cc
+-rw-r--r--   0 root         (0) root         (0)    11579 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/PDFCore.h
+-rw-r--r--   0 root         (0) root         (0)    16078 2023-05-16 07:46:43.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/PDFDoc.cc
+-rw-r--r--   0 root         (0) root         (0)     6774 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/PDFDoc.h
+-rw-r--r--   0 root         (0) root         (0)     2530 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/PDFDocEncoding.cc
+-rw-r--r--   0 root         (0) root         (0)      339 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/PDFDocEncoding.h
+-rw-r--r--   0 root         (0) root         (0)   230372 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/PSOutputDev.cc
+-rw-r--r--   0 root         (0) root         (0)    19106 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/PSOutputDev.h
+-rw-r--r--   0 root         (0) root         (0)     3295 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/PSTokenizer.cc
+-rw-r--r--   0 root         (0) root         (0)      771 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/PSTokenizer.h
+-rw-r--r--   0 root         (0) root         (0)    13874 2023-03-01 15:38:49.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/Page.cc
+-rw-r--r--   0 root         (0) root         (0)     6412 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/Page.h
+-rw-r--r--   0 root         (0) root         (0)     8100 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/Parser.cc
+-rw-r--r--   0 root         (0) root         (0)     1674 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/Parser.h
+-rw-r--r--   0 root         (0) root         (0)     8588 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/PreScanOutputDev.cc
+-rw-r--r--   0 root         (0) root         (0)     4810 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/PreScanOutputDev.h
+-rw-r--r--   0 root         (0) root         (0)    10354 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/SecurityHandler.cc
+-rw-r--r--   0 root         (0) root         (0)     3962 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/SecurityHandler.h
+-rw-r--r--   0 root         (0) root         (0)    37941 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/ShadingImage.cc
+-rw-r--r--   0 root         (0) root         (0)     3215 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/ShadingImage.h
+-rw-r--r--   0 root         (0) root         (0)   127634 2023-05-19 16:11:47.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/SplashOutputDev.cc
+-rw-r--r--   0 root         (0) root         (0)    10811 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/SplashOutputDev.h
+-rw-r--r--   0 root         (0) root         (0)    17471 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/Stream-CCITT.h
+-rw-r--r--   0 root         (0) root         (0)   131758 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/Stream.cc
+-rw-r--r--   0 root         (0) root         (0)    31826 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/Stream.h
+-rw-r--r--   0 root         (0) root         (0)   183399 2023-06-02 09:35:24.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/TextOutputDev.cc
+-rw-r--r--   0 root         (0) root         (0)    27134 2023-06-02 09:35:24.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/TextOutputDev.h
+-rw-r--r--   0 root         (0) root         (0)     4302 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/TextString.cc
+-rw-r--r--   0 root         (0) root         (0)     1587 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/TextString.h
+-rw-r--r--   0 root         (0) root         (0)    13862 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/TileCache.cc
+-rw-r--r--   0 root         (0) root         (0)     2041 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/TileCache.h
+-rw-r--r--   0 root         (0) root         (0)    10913 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/TileCompositor.cc
+-rw-r--r--   0 root         (0) root         (0)     1895 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/TileCompositor.h
+-rw-r--r--   0 root         (0) root         (0)    44674 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/TileMap.cc
+-rw-r--r--   0 root         (0) root         (0)     8164 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/TileMap.h
+-rw-r--r--   0 root         (0) root         (0)     4636 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/UTF8.cc
+-rw-r--r--   0 root         (0) root         (0)     1408 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/UTF8.h
+-rw-r--r--   0 root         (0) root         (0)     6033 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/UnicodeMap.cc
+-rw-r--r--   0 root         (0) root         (0)     2971 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/UnicodeMap.h
+-rw-r--r--   0 root         (0) root         (0)    11532 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/UnicodeMapTables.h
+-rw-r--r--   0 root         (0) root         (0)     5024 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/UnicodeRemapping.cc
+-rw-r--r--   0 root         (0) root         (0)     1138 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/UnicodeRemapping.h
+-rw-r--r--   0 root         (0) root         (0)    73118 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/UnicodeTypeTable.cc
+-rw-r--r--   0 root         (0) root         (0)      719 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/UnicodeTypeTable.h
+-rw-r--r--   0 root         (0) root         (0)    10592 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/WebFont.cc
+-rw-r--r--   0 root         (0) root         (0)     2139 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/WebFont.h
+-rw-r--r--   0 root         (0) root         (0)    18912 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/XFAScanner.cc
+-rw-r--r--   0 root         (0) root         (0)     4518 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/XFAScanner.h
+-rw-r--r--   0 root         (0) root         (0)    33740 2023-05-15 08:40:18.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/XRef.cc
+-rw-r--r--   0 root         (0) root         (0)     5955 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/XRef.h
+-rw-r--r--   0 root         (0) root         (0)    23997 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/Zoox.cc
+-rw-r--r--   0 root         (0) root         (0)     6378 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/Zoox.h
+-rw-r--r--   0 root         (0) root         (0)     3128 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/config.h
+-rw-r--r--   0 root         (0) root         (0)     5663 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/pdfdetach.cc
+-rw-r--r--   0 root         (0) root         (0)    12108 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/pdffonts.cc
+-rw-r--r--   0 root         (0) root         (0)     4538 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/pdfimages.cc
+-rw-r--r--   0 root         (0) root         (0)    15031 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/pdfinfo.cc
+-rw-r--r--   0 root         (0) root         (0)     8525 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/pdftohtml.cc
+-rw-r--r--   0 root         (0) root         (0)    10873 2023-05-19 13:46:26.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/pdftopng.cc
+-rw-r--r--   0 root         (0) root         (0)     7820 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/pdftoppm.cc
+-rw-r--r--   0 root         (0) root         (0)    11515 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/pdftops.cc
+-rw-r--r--   0 root         (0) root         (0)     9928 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf/pdftotext.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:30.723827 xpydf-0.1.6/src/xpdf-4.04/xpdf-qt/
+-rw-r--r--   0 root         (0) root         (0)    30301 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf-qt/QtPDFCore.cc
+-rw-r--r--   0 root         (0) root         (0)     6596 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf-qt/QtPDFCore.h
+-rw-r--r--   0 root         (0) root         (0)    14925 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf-qt/XpdfApp.cc
+-rw-r--r--   0 root         (0) root         (0)     2452 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf-qt/XpdfApp.h
+-rw-r--r--   0 root         (0) root         (0)   148791 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf-qt/XpdfViewer.cc
+-rw-r--r--   0 root         (0) root         (0)    18968 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf-qt/XpdfViewer.h
+-rw-r--r--   0 root         (0) root         (0)    54075 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf-qt/XpdfWidget.cc
+-rw-r--r--   0 root         (0) root         (0)    39531 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf-qt/XpdfWidget.h
+-rw-r--r--   0 root         (0) root         (0)    13035 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf-qt/XpdfWidgetPrint.cc
+-rw-r--r--   0 root         (0) root         (0)      520 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf-qt/XpdfWidgetPrint.h
+-rw-r--r--   0 root         (0) root         (0)     1327 2022-04-18 21:11:23.000000 xpydf-0.1.6/src/xpdf-4.04/xpdf-qt/xpdf.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:30.809684 xpydf-0.1.6/src/xpydf/
+-rw-r--r--   0 root         (0) root         (0)     6148 2023-05-01 14:11:15.000000 xpydf-0.1.6/src/xpydf/.DS_Store
+-rw-r--r--   0 root         (0) root         (0)     3771 2023-06-09 07:48:08.000000 xpydf-0.1.6/src/xpydf/ImageDataDev.cc
+-rw-r--r--   0 root         (0) root         (0)     1095 2023-05-05 08:47:39.000000 xpydf-0.1.6/src/xpydf/ImageDataDev.h
+-rw-r--r--   0 root         (0) root         (0)     1121 2023-05-15 08:40:14.000000 xpydf-0.1.6/src/xpydf/ImageInfoDev.cc
+-rw-r--r--   0 root         (0) root         (0)      941 2023-04-12 11:54:25.000000 xpydf-0.1.6/src/xpydf/ImageInfoDev.h
+-rw-r--r--   0 root         (0) root         (0)     5725 2023-06-09 07:28:33.000000 xpydf-0.1.6/src/xpydf/PdfLoader.cc
+-rw-r--r--   0 root         (0) root         (0)     1163 2023-06-09 07:28:33.000000 xpydf-0.1.6/src/xpydf/PdfLoader.h
+-rw-r--r--   0 root         (0) root         (0)     8438 2023-06-09 07:28:33.000000 xpydf-0.1.6/src/xpydf/PdfLoaderWrapper.cc
+-rw-r--r--   0 root         (0) root         (0)     2198 2023-04-12 11:54:25.000000 xpydf-0.1.6/src/xpydf/PyCppConversion.cc
+-rw-r--r--   0 root         (0) root         (0)      441 2023-04-12 11:54:25.000000 xpydf-0.1.6/src/xpydf/PyCppConversion.h
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:54:25.000000 xpydf-0.1.6/src/xpydf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:54:25.000000 xpydf-0.1.6/src/xpydf/__init__.pyi
+-rw-r--r--   0 root         (0) root         (0)      857 2023-06-09 07:28:33.000000 xpydf-0.1.6/src/xpydf/cXpdfPython.pyi
+-rw-r--r--   0 root         (0) root         (0)     5155 2023-06-09 07:28:33.000000 xpydf-0.1.6/src/xpydf/pdf_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1246 2023-06-09 07:28:33.000000 xpydf-0.1.6/src/xpydf/pdf_loader.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:30.840197 xpydf-0.1.6/src/xpydf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      844 2023-06-09 10:59:25.000000 xpydf-0.1.6/src/xpydf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    25801 2023-06-09 10:59:25.000000 xpydf-0.1.6/src/xpydf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 10:59:25.000000 xpydf-0.1.6/src/xpydf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-09 10:59:25.000000 xpydf-0.1.6/src/xpydf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-06-09 10:59:25.000000 xpydf-0.1.6/src/xpydf.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 10:59:30.845644 xpydf-0.1.6/tests/
+-rw-r--r--   0 root         (0) root         (0)     4574 2023-06-09 07:28:33.000000 xpydf-0.1.6/tests/test_pdf_loader.py
```

### Comparing `xpydf-0.1.5/LICENSE` & `xpydf-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/PKG-INFO` & `xpydf-0.1.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpydf
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python wrapper around the pdftotext and pdfimages functionalities of xpdf.
 Author-email: Matthijs Wesseling <matthijs.wesseling@bigdatarepublic.nl>
 Project-URL: Homepage, https://github.com/Bladieblah/xpdf-python
 Project-URL: Bug Tracker, https://github.com/Bladieblah/xpdf-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `xpydf-0.1.5/pyproject.toml` & `xpydf-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xpydf"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
     { name  = "Matthijs Wesseling", email = "matthijs.wesseling@bigdatarepublic.nl" },
 ]
 
 description = "Python wrapper around the pdftotext and pdfimages functionalities of xpdf."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `xpydf-0.1.5/src/freetype/.DS_Store` & `xpydf-0.1.6/src/freetype/.DS_Store`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/.gitlab-ci.yml` & `xpydf-0.1.6/src/freetype/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/.mailmap` & `xpydf-0.1.6/src/freetype/.mailmap`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/CMakeLists.txt` & `xpydf-0.1.6/src/freetype/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/LICENSE.TXT` & `xpydf-0.1.6/src/freetype/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/Makefile` & `xpydf-0.1.6/src/freetype/Makefile`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/README` & `xpydf-0.1.6/src/freetype/README`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/README.git` & `xpydf-0.1.6/src/freetype/README.git`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/autogen.sh` & `xpydf-0.1.6/src/freetype/autogen.sh`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/builds/mac/ascii2mpw.py` & `xpydf-0.1.6/src/freetype/builds/mac/ascii2mpw.py`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/builds/meson/extract_freetype_version.py` & `xpydf-0.1.6/src/freetype/builds/meson/extract_freetype_version.py`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/builds/meson/extract_libtool_version.py` & `xpydf-0.1.6/src/freetype/builds/meson/extract_libtool_version.py`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/builds/meson/generate_reference_docs.py` & `xpydf-0.1.6/src/freetype/builds/meson/generate_reference_docs.py`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/builds/meson/parse_modules_cfg.py` & `xpydf-0.1.6/src/freetype/builds/meson/parse_modules_cfg.py`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/builds/meson/process_ftoption_h.py` & `xpydf-0.1.6/src/freetype/builds/meson/process_ftoption_h.py`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/config.mk` & `xpydf-0.1.6/src/freetype/config.mk`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/configure` & `xpydf-0.1.6/src/freetype/configure`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/dlg/dlg.h` & `xpydf-0.1.6/src/freetype/include/dlg/dlg.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/dlg/output.h` & `xpydf-0.1.6/src/freetype/include/dlg/output.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/config/ftconfig.h` & `xpydf-0.1.6/src/freetype/include/freetype/config/ftconfig.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/config/ftheader.h` & `xpydf-0.1.6/src/freetype/include/freetype/config/ftheader.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/config/ftmodule.h` & `xpydf-0.1.6/src/freetype/include/freetype/config/ftmodule.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/config/ftoption.h` & `xpydf-0.1.6/src/freetype/include/freetype/config/ftoption.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/config/ftstdlib.h` & `xpydf-0.1.6/src/freetype/include/freetype/config/ftstdlib.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/config/integer-types.h` & `xpydf-0.1.6/src/freetype/include/freetype/config/integer-types.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/config/mac-support.h` & `xpydf-0.1.6/src/freetype/include/freetype/config/mac-support.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/config/public-macros.h` & `xpydf-0.1.6/src/freetype/include/freetype/config/public-macros.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/freetype.h` & `xpydf-0.1.6/src/freetype/include/freetype/freetype.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/ftadvanc.h` & `xpydf-0.1.6/src/freetype/include/freetype/ftadvanc.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/ftbbox.h` & `xpydf-0.1.6/src/freetype/include/freetype/ftbbox.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/ftbdf.h` & `xpydf-0.1.6/src/freetype/include/freetype/ftbdf.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/ftbitmap.h` & `xpydf-0.1.6/src/freetype/include/freetype/ftbitmap.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/ftbzip2.h` & `xpydf-0.1.6/src/freetype/include/freetype/ftbzip2.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/ftcache.h` & `xpydf-0.1.6/src/freetype/include/freetype/ftcache.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/ftchapters.h` & `xpydf-0.1.6/src/freetype/include/freetype/ftchapters.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/ftcid.h` & `xpydf-0.1.6/src/freetype/include/freetype/ftcid.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/ftcolor.h` & `xpydf-0.1.6/src/freetype/include/freetype/ftcolor.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/ftdriver.h` & `xpydf-0.1.6/src/freetype/include/freetype/ftdriver.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/fterrdef.h` & `xpydf-0.1.6/src/freetype/include/freetype/fterrdef.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/fterrors.h` & `xpydf-0.1.6/src/freetype/include/freetype/fterrors.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/ftfntfmt.h` & `xpydf-0.1.6/src/freetype/include/freetype/ftfntfmt.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/ftgasp.h` & `xpydf-0.1.6/src/freetype/include/freetype/ftgasp.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/ftglyph.h` & `xpydf-0.1.6/src/freetype/include/freetype/ftglyph.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/ftgxval.h` & `xpydf-0.1.6/src/freetype/include/freetype/ftgxval.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/ftgzip.h` & `xpydf-0.1.6/src/freetype/include/freetype/ftgzip.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/ftimage.h` & `xpydf-0.1.6/src/freetype/include/freetype/ftimage.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/ftincrem.h` & `xpydf-0.1.6/src/freetype/include/freetype/ftincrem.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/ftlcdfil.h` & `xpydf-0.1.6/src/freetype/include/freetype/ftlcdfil.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/ftlist.h` & `xpydf-0.1.6/src/freetype/include/freetype/ftlist.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/ftlogging.h` & `xpydf-0.1.6/src/freetype/include/freetype/ftlogging.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/ftlzw.h` & `xpydf-0.1.6/src/freetype/include/freetype/ftlzw.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/ftmac.h` & `xpydf-0.1.6/src/freetype/include/freetype/ftmac.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/ftmm.h` & `xpydf-0.1.6/src/freetype/include/freetype/ftmm.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/ftmodapi.h` & `xpydf-0.1.6/src/freetype/include/freetype/ftmodapi.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/ftmoderr.h` & `xpydf-0.1.6/src/freetype/include/freetype/ftmoderr.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/ftotval.h` & `xpydf-0.1.6/src/freetype/include/freetype/ftotval.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/ftoutln.h` & `xpydf-0.1.6/src/freetype/include/freetype/ftoutln.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/ftparams.h` & `xpydf-0.1.6/src/freetype/include/freetype/ftparams.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/ftpfr.h` & `xpydf-0.1.6/src/freetype/include/freetype/ftpfr.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/ftrender.h` & `xpydf-0.1.6/src/freetype/include/freetype/ftrender.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/ftsizes.h` & `xpydf-0.1.6/src/freetype/include/freetype/ftsizes.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/ftsnames.h` & `xpydf-0.1.6/src/freetype/include/freetype/ftsnames.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/ftstroke.h` & `xpydf-0.1.6/src/freetype/include/freetype/ftstroke.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/ftsynth.h` & `xpydf-0.1.6/src/freetype/include/freetype/ftsynth.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/ftsystem.h` & `xpydf-0.1.6/src/freetype/include/freetype/ftsystem.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/fttrigon.h` & `xpydf-0.1.6/src/freetype/include/freetype/fttrigon.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/fttypes.h` & `xpydf-0.1.6/src/freetype/include/freetype/fttypes.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/ftwinfnt.h` & `xpydf-0.1.6/src/freetype/include/freetype/ftwinfnt.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/autohint.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/autohint.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/cffotypes.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/cffotypes.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/cfftypes.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/cfftypes.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/compiler-macros.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/compiler-macros.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/ftcalc.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/ftcalc.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/ftdebug.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/ftdebug.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/ftdrv.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/ftdrv.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/ftgloadr.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/ftgloadr.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/fthash.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/fthash.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/ftmemory.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/ftmemory.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/ftmmtypes.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/ftmmtypes.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/ftobjs.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/ftobjs.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/ftpsprop.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/ftpsprop.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/ftrfork.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/ftrfork.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/ftserv.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/ftserv.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/ftstream.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/ftstream.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/fttrace.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/fttrace.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/ftvalid.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/ftvalid.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/psaux.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/psaux.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/pshints.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/pshints.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/services/svbdf.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/services/svbdf.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/services/svcfftl.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/services/svcfftl.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/services/svcid.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/services/svcid.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/services/svfntfmt.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/services/svfntfmt.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/services/svgldict.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/services/svgldict.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/services/svgxval.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/services/svgxval.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/services/svkern.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/services/svkern.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/services/svmetric.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/services/svmetric.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/services/svmm.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/services/svmm.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/services/svotval.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/services/svotval.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/services/svpfr.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/services/svpfr.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/services/svpostnm.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/services/svpostnm.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/services/svprop.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/services/svprop.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/services/svpscmap.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/services/svpscmap.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/services/svpsinfo.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/services/svpsinfo.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/services/svsfnt.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/services/svsfnt.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/services/svttcmap.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/services/svttcmap.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/services/svtteng.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/services/svtteng.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/services/svttglyf.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/services/svttglyf.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/services/svwinfnt.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/services/svwinfnt.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/sfnt.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/sfnt.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/svginterface.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/svginterface.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/t1types.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/t1types.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/tttypes.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/tttypes.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/internal/wofftypes.h` & `xpydf-0.1.6/src/freetype/include/freetype/internal/wofftypes.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/otsvg.h` & `xpydf-0.1.6/src/freetype/include/freetype/otsvg.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/t1tables.h` & `xpydf-0.1.6/src/freetype/include/freetype/t1tables.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/ttnameid.h` & `xpydf-0.1.6/src/freetype/include/freetype/ttnameid.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/tttables.h` & `xpydf-0.1.6/src/freetype/include/freetype/tttables.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/freetype/tttags.h` & `xpydf-0.1.6/src/freetype/include/freetype/tttags.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/include/ft2build.h` & `xpydf-0.1.6/src/freetype/include/ft2build.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/meson.build` & `xpydf-0.1.6/src/freetype/meson.build`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/meson_options.txt` & `xpydf-0.1.6/src/freetype/meson_options.txt`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/modules.cfg` & `xpydf-0.1.6/src/freetype/modules.cfg`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/autofit/afblue.c` & `xpydf-0.1.6/src/freetype/src/autofit/afblue.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/autofit/afblue.h` & `xpydf-0.1.6/src/freetype/src/autofit/afblue.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/autofit/afcjk.c` & `xpydf-0.1.6/src/freetype/src/autofit/afcjk.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/autofit/afcjk.h` & `xpydf-0.1.6/src/freetype/src/autofit/afcjk.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/autofit/afcover.h` & `xpydf-0.1.6/src/freetype/src/autofit/afcover.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/autofit/afdummy.c` & `xpydf-0.1.6/src/freetype/src/autofit/afdummy.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/autofit/afdummy.h` & `xpydf-0.1.6/src/freetype/src/autofit/afdummy.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/autofit/aferrors.h` & `xpydf-0.1.6/src/freetype/src/autofit/aferrors.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/autofit/afglobal.c` & `xpydf-0.1.6/src/freetype/src/autofit/afglobal.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/autofit/afglobal.h` & `xpydf-0.1.6/src/freetype/src/autofit/afglobal.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/autofit/afhints.c` & `xpydf-0.1.6/src/freetype/src/autofit/afhints.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/autofit/afhints.h` & `xpydf-0.1.6/src/freetype/src/autofit/afhints.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/autofit/afindic.c` & `xpydf-0.1.6/src/freetype/src/autofit/afindic.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/autofit/afindic.h` & `xpydf-0.1.6/src/freetype/src/autofit/afindic.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/autofit/aflatin.c` & `xpydf-0.1.6/src/freetype/src/autofit/aflatin.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/autofit/aflatin.h` & `xpydf-0.1.6/src/freetype/src/autofit/aflatin.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/autofit/afloader.c` & `xpydf-0.1.6/src/freetype/src/autofit/afloader.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/autofit/afloader.h` & `xpydf-0.1.6/src/freetype/src/autofit/afloader.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/autofit/afmodule.c` & `xpydf-0.1.6/src/freetype/src/autofit/afmodule.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/autofit/afmodule.h` & `xpydf-0.1.6/src/freetype/src/autofit/afmodule.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/autofit/afranges.c` & `xpydf-0.1.6/src/freetype/src/autofit/afranges.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/autofit/afranges.h` & `xpydf-0.1.6/src/freetype/src/autofit/afranges.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/autofit/afscript.h` & `xpydf-0.1.6/src/freetype/src/autofit/afscript.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/autofit/afshaper.c` & `xpydf-0.1.6/src/freetype/src/autofit/afshaper.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/autofit/afshaper.h` & `xpydf-0.1.6/src/freetype/src/autofit/afshaper.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/autofit/afstyles.h` & `xpydf-0.1.6/src/freetype/src/autofit/afstyles.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/autofit/aftypes.h` & `xpydf-0.1.6/src/freetype/src/autofit/aftypes.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/autofit/afws-decl.h` & `xpydf-0.1.6/src/freetype/src/autofit/afws-decl.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/autofit/afws-iter.h` & `xpydf-0.1.6/src/freetype/src/autofit/afws-iter.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/autofit/autofit.c` & `xpydf-0.1.6/src/freetype/src/autofit/autofit.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/autofit/ft-hb.c` & `xpydf-0.1.6/src/freetype/src/autofit/ft-hb.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/autofit/ft-hb.h` & `xpydf-0.1.6/src/freetype/src/autofit/ft-hb.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/base/ftadvanc.c` & `xpydf-0.1.6/src/freetype/src/base/ftadvanc.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/base/ftbase.c` & `xpydf-0.1.6/src/freetype/src/base/ftbase.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/base/ftbase.h` & `xpydf-0.1.6/src/freetype/src/base/ftbase.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/base/ftbbox.c` & `xpydf-0.1.6/src/freetype/src/base/ftbbox.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/base/ftbdf.c` & `xpydf-0.1.6/src/freetype/src/base/ftbdf.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/base/ftbitmap.c` & `xpydf-0.1.6/src/freetype/src/base/ftbitmap.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/base/ftcalc.c` & `xpydf-0.1.6/src/freetype/src/base/ftcalc.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/base/ftcid.c` & `xpydf-0.1.6/src/freetype/src/base/ftcid.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/base/ftcolor.c` & `xpydf-0.1.6/src/freetype/src/base/ftcolor.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/base/ftdbgmem.c` & `xpydf-0.1.6/src/freetype/src/base/ftdbgmem.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/base/ftdebug.c` & `xpydf-0.1.6/src/freetype/src/base/ftdebug.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/base/fterrors.c` & `xpydf-0.1.6/src/freetype/src/base/fterrors.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/base/ftfntfmt.c` & `xpydf-0.1.6/src/freetype/src/base/ftfntfmt.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/base/ftfstype.c` & `xpydf-0.1.6/src/freetype/src/base/ftfstype.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/base/ftgasp.c` & `xpydf-0.1.6/src/freetype/src/base/ftgasp.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/base/ftgloadr.c` & `xpydf-0.1.6/src/freetype/src/base/ftgloadr.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/base/ftglyph.c` & `xpydf-0.1.6/src/freetype/src/base/ftglyph.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/base/ftgxval.c` & `xpydf-0.1.6/src/freetype/src/base/ftgxval.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/base/fthash.c` & `xpydf-0.1.6/src/freetype/src/base/fthash.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/base/ftinit.c` & `xpydf-0.1.6/src/freetype/src/base/ftinit.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/base/ftlcdfil.c` & `xpydf-0.1.6/src/freetype/src/base/ftlcdfil.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/base/ftmac.c` & `xpydf-0.1.6/src/freetype/src/base/ftmac.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/base/ftmm.c` & `xpydf-0.1.6/src/freetype/src/base/ftmm.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/base/ftobjs.c` & `xpydf-0.1.6/src/freetype/src/base/ftobjs.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/base/ftotval.c` & `xpydf-0.1.6/src/freetype/src/base/ftotval.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/base/ftoutln.c` & `xpydf-0.1.6/src/freetype/src/base/ftoutln.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/base/ftpatent.c` & `xpydf-0.1.6/src/freetype/src/base/ftpatent.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/base/ftpfr.c` & `xpydf-0.1.6/src/freetype/src/base/ftpfr.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/base/ftpsprop.c` & `xpydf-0.1.6/src/freetype/src/base/ftpsprop.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/base/ftrfork.c` & `xpydf-0.1.6/src/freetype/src/base/ftrfork.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/base/ftsnames.c` & `xpydf-0.1.6/src/freetype/src/base/ftsnames.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/base/ftstream.c` & `xpydf-0.1.6/src/freetype/src/base/ftstream.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/base/ftstroke.c` & `xpydf-0.1.6/src/freetype/src/base/ftstroke.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/base/ftsynth.c` & `xpydf-0.1.6/src/freetype/src/base/ftsynth.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/base/ftsystem.c` & `xpydf-0.1.6/src/freetype/src/base/ftsystem.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/base/fttrigon.c` & `xpydf-0.1.6/src/freetype/src/base/fttrigon.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/base/fttype1.c` & `xpydf-0.1.6/src/freetype/src/base/fttype1.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/base/ftutil.c` & `xpydf-0.1.6/src/freetype/src/base/ftutil.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/base/ftwinfnt.c` & `xpydf-0.1.6/src/freetype/src/base/ftwinfnt.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/base/md5.c` & `xpydf-0.1.6/src/freetype/src/base/md5.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/base/md5.h` & `xpydf-0.1.6/src/freetype/src/base/md5.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/bdf/bdf.c` & `xpydf-0.1.6/src/freetype/src/bdf/bdf.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/bdf/bdf.h` & `xpydf-0.1.6/src/freetype/src/bdf/bdf.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/bdf/bdfdrivr.c` & `xpydf-0.1.6/src/freetype/src/bdf/bdfdrivr.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/bdf/bdfdrivr.h` & `xpydf-0.1.6/src/freetype/src/bdf/bdfdrivr.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/bdf/bdferror.h` & `xpydf-0.1.6/src/freetype/src/bdf/bdferror.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/bdf/bdflib.c` & `xpydf-0.1.6/src/freetype/src/bdf/bdflib.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/bzip2/ftbzip2.c` & `xpydf-0.1.6/src/freetype/src/bzip2/ftbzip2.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cache/ftcache.c` & `xpydf-0.1.6/src/freetype/src/cache/ftcache.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cache/ftcbasic.c` & `xpydf-0.1.6/src/freetype/src/cache/ftcbasic.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cache/ftccache.c` & `xpydf-0.1.6/src/freetype/src/cache/ftccache.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cache/ftccache.h` & `xpydf-0.1.6/src/freetype/src/cache/ftccache.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cache/ftccback.h` & `xpydf-0.1.6/src/freetype/src/cache/ftccback.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cache/ftccmap.c` & `xpydf-0.1.6/src/freetype/src/cache/ftccmap.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cache/ftcerror.h` & `xpydf-0.1.6/src/freetype/src/cache/ftcerror.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cache/ftcglyph.c` & `xpydf-0.1.6/src/freetype/src/cache/ftcglyph.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cache/ftcglyph.h` & `xpydf-0.1.6/src/freetype/src/cache/ftcglyph.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cache/ftcimage.c` & `xpydf-0.1.6/src/freetype/src/cache/ftcimage.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cache/ftcimage.h` & `xpydf-0.1.6/src/freetype/src/cache/ftcimage.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cache/ftcmanag.c` & `xpydf-0.1.6/src/freetype/src/cache/ftcmanag.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cache/ftcmanag.h` & `xpydf-0.1.6/src/freetype/src/cache/ftcmanag.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cache/ftcmru.c` & `xpydf-0.1.6/src/freetype/src/cache/ftcmru.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cache/ftcmru.h` & `xpydf-0.1.6/src/freetype/src/cache/ftcmru.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cache/ftcsbits.c` & `xpydf-0.1.6/src/freetype/src/cache/ftcsbits.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cache/ftcsbits.h` & `xpydf-0.1.6/src/freetype/src/cache/ftcsbits.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cff/cff.c` & `xpydf-0.1.6/src/freetype/src/cff/cff.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cff/cffcmap.c` & `xpydf-0.1.6/src/freetype/src/cff/cffcmap.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cff/cffcmap.h` & `xpydf-0.1.6/src/freetype/src/cff/cffcmap.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cff/cffdrivr.c` & `xpydf-0.1.6/src/freetype/src/cff/cffdrivr.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cff/cffdrivr.h` & `xpydf-0.1.6/src/freetype/src/cff/cffdrivr.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cff/cfferrs.h` & `xpydf-0.1.6/src/freetype/src/cff/cfferrs.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cff/cffgload.c` & `xpydf-0.1.6/src/freetype/src/cff/cffgload.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cff/cffgload.h` & `xpydf-0.1.6/src/freetype/src/cff/cffgload.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cff/cffload.c` & `xpydf-0.1.6/src/freetype/src/cff/cffload.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cff/cffload.h` & `xpydf-0.1.6/src/freetype/src/cff/cffload.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cff/cffobjs.c` & `xpydf-0.1.6/src/freetype/src/cff/cffobjs.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cff/cffobjs.h` & `xpydf-0.1.6/src/freetype/src/cff/cffobjs.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cff/cffparse.c` & `xpydf-0.1.6/src/freetype/src/cff/cffparse.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cff/cffparse.h` & `xpydf-0.1.6/src/freetype/src/cff/cffparse.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cff/cfftoken.h` & `xpydf-0.1.6/src/freetype/src/cff/cfftoken.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cid/ciderrs.h` & `xpydf-0.1.6/src/freetype/src/cid/ciderrs.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cid/cidgload.c` & `xpydf-0.1.6/src/freetype/src/cid/cidgload.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cid/cidgload.h` & `xpydf-0.1.6/src/freetype/src/cid/cidgload.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cid/cidload.c` & `xpydf-0.1.6/src/freetype/src/cid/cidload.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cid/cidload.h` & `xpydf-0.1.6/src/freetype/src/cid/cidload.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cid/cidobjs.c` & `xpydf-0.1.6/src/freetype/src/cid/cidobjs.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cid/cidobjs.h` & `xpydf-0.1.6/src/freetype/src/cid/cidobjs.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cid/cidparse.c` & `xpydf-0.1.6/src/freetype/src/cid/cidparse.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cid/cidparse.h` & `xpydf-0.1.6/src/freetype/src/cid/cidparse.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cid/cidriver.c` & `xpydf-0.1.6/src/freetype/src/cid/cidriver.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cid/cidriver.h` & `xpydf-0.1.6/src/freetype/src/cid/cidriver.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cid/cidtoken.h` & `xpydf-0.1.6/src/freetype/src/cid/cidtoken.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/cid/type1cid.c` & `xpydf-0.1.6/src/freetype/src/cid/type1cid.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/dlg/dlg.c` & `xpydf-0.1.6/src/freetype/src/dlg/dlg.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/dlg/dlgwrap.c` & `xpydf-0.1.6/src/freetype/src/dlg/dlgwrap.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gxvalid/gxvalid.c` & `xpydf-0.1.6/src/freetype/src/gxvalid/gxvalid.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gxvalid/gxvalid.h` & `xpydf-0.1.6/src/freetype/src/gxvalid/gxvalid.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gxvalid/gxvbsln.c` & `xpydf-0.1.6/src/freetype/src/gxvalid/gxvbsln.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gxvalid/gxvcommn.c` & `xpydf-0.1.6/src/freetype/src/gxvalid/gxvcommn.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gxvalid/gxvcommn.h` & `xpydf-0.1.6/src/freetype/src/gxvalid/gxvcommn.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gxvalid/gxverror.h` & `xpydf-0.1.6/src/freetype/src/gxvalid/gxverror.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gxvalid/gxvfeat.c` & `xpydf-0.1.6/src/freetype/src/gxvalid/gxvfeat.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gxvalid/gxvfeat.h` & `xpydf-0.1.6/src/freetype/src/gxvalid/gxvfeat.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gxvalid/gxvfgen.c` & `xpydf-0.1.6/src/freetype/src/gxvalid/gxvfgen.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gxvalid/gxvjust.c` & `xpydf-0.1.6/src/freetype/src/gxvalid/gxvjust.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gxvalid/gxvkern.c` & `xpydf-0.1.6/src/freetype/src/gxvalid/gxvkern.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gxvalid/gxvlcar.c` & `xpydf-0.1.6/src/freetype/src/gxvalid/gxvlcar.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gxvalid/gxvmod.c` & `xpydf-0.1.6/src/freetype/src/gxvalid/gxvmod.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gxvalid/gxvmod.h` & `xpydf-0.1.6/src/freetype/src/gxvalid/gxvmod.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gxvalid/gxvmort.c` & `xpydf-0.1.6/src/freetype/src/gxvalid/gxvmort.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gxvalid/gxvmort.h` & `xpydf-0.1.6/src/freetype/src/gxvalid/gxvmort.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gxvalid/gxvmort0.c` & `xpydf-0.1.6/src/freetype/src/gxvalid/gxvmort0.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gxvalid/gxvmort1.c` & `xpydf-0.1.6/src/freetype/src/gxvalid/gxvmort1.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gxvalid/gxvmort2.c` & `xpydf-0.1.6/src/freetype/src/gxvalid/gxvmort2.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gxvalid/gxvmort4.c` & `xpydf-0.1.6/src/freetype/src/gxvalid/gxvmort4.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gxvalid/gxvmort5.c` & `xpydf-0.1.6/src/freetype/src/gxvalid/gxvmort5.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gxvalid/gxvmorx.c` & `xpydf-0.1.6/src/freetype/src/gxvalid/gxvmorx.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gxvalid/gxvmorx.h` & `xpydf-0.1.6/src/freetype/src/gxvalid/gxvmorx.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gxvalid/gxvmorx0.c` & `xpydf-0.1.6/src/freetype/src/gxvalid/gxvmorx0.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gxvalid/gxvmorx1.c` & `xpydf-0.1.6/src/freetype/src/gxvalid/gxvmorx1.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gxvalid/gxvmorx2.c` & `xpydf-0.1.6/src/freetype/src/gxvalid/gxvmorx2.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gxvalid/gxvmorx4.c` & `xpydf-0.1.6/src/freetype/src/gxvalid/gxvmorx4.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gxvalid/gxvmorx5.c` & `xpydf-0.1.6/src/freetype/src/gxvalid/gxvmorx5.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gxvalid/gxvopbd.c` & `xpydf-0.1.6/src/freetype/src/gxvalid/gxvopbd.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gxvalid/gxvprop.c` & `xpydf-0.1.6/src/freetype/src/gxvalid/gxvprop.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gxvalid/gxvtrak.c` & `xpydf-0.1.6/src/freetype/src/gxvalid/gxvtrak.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gzip/adler32.c` & `xpydf-0.1.6/src/freetype/src/gzip/adler32.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gzip/crc32.c` & `xpydf-0.1.6/src/freetype/src/gzip/crc32.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gzip/crc32.h` & `xpydf-0.1.6/src/freetype/src/gzip/crc32.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gzip/ftgzip.c` & `xpydf-0.1.6/src/freetype/src/gzip/ftgzip.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gzip/ftzconf.h` & `xpydf-0.1.6/src/freetype/src/gzip/ftzconf.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gzip/gzguts.h` & `xpydf-0.1.6/src/freetype/src/gzip/gzguts.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gzip/inffast.c` & `xpydf-0.1.6/src/freetype/src/gzip/inffast.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gzip/inffixed.h` & `xpydf-0.1.6/src/freetype/src/gzip/inffixed.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gzip/inflate.c` & `xpydf-0.1.6/src/freetype/src/gzip/inflate.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gzip/inflate.h` & `xpydf-0.1.6/src/freetype/src/gzip/inflate.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gzip/inftrees.c` & `xpydf-0.1.6/src/freetype/src/gzip/inftrees.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gzip/inftrees.h` & `xpydf-0.1.6/src/freetype/src/gzip/inftrees.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gzip/zlib.h` & `xpydf-0.1.6/src/freetype/src/gzip/zlib.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gzip/zutil.c` & `xpydf-0.1.6/src/freetype/src/gzip/zutil.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/gzip/zutil.h` & `xpydf-0.1.6/src/freetype/src/gzip/zutil.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/lzw/ftlzw.c` & `xpydf-0.1.6/src/freetype/src/lzw/ftlzw.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/lzw/ftzopen.c` & `xpydf-0.1.6/src/freetype/src/lzw/ftzopen.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/lzw/ftzopen.h` & `xpydf-0.1.6/src/freetype/src/lzw/ftzopen.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/otvalid/otvalid.c` & `xpydf-0.1.6/src/freetype/src/otvalid/otvalid.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/otvalid/otvalid.h` & `xpydf-0.1.6/src/freetype/src/otvalid/otvalid.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/otvalid/otvbase.c` & `xpydf-0.1.6/src/freetype/src/otvalid/otvbase.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/otvalid/otvcommn.c` & `xpydf-0.1.6/src/freetype/src/otvalid/otvcommn.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/otvalid/otvcommn.h` & `xpydf-0.1.6/src/freetype/src/otvalid/otvcommn.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/otvalid/otverror.h` & `xpydf-0.1.6/src/freetype/src/otvalid/otverror.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/otvalid/otvgdef.c` & `xpydf-0.1.6/src/freetype/src/otvalid/otvgdef.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/otvalid/otvgpos.c` & `xpydf-0.1.6/src/freetype/src/otvalid/otvgpos.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/otvalid/otvgpos.h` & `xpydf-0.1.6/src/freetype/src/otvalid/otvgpos.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/otvalid/otvgsub.c` & `xpydf-0.1.6/src/freetype/src/otvalid/otvgsub.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/otvalid/otvjstf.c` & `xpydf-0.1.6/src/freetype/src/otvalid/otvjstf.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/otvalid/otvmath.c` & `xpydf-0.1.6/src/freetype/src/otvalid/otvmath.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/otvalid/otvmod.c` & `xpydf-0.1.6/src/freetype/src/otvalid/otvmod.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/otvalid/otvmod.h` & `xpydf-0.1.6/src/freetype/src/otvalid/otvmod.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/pcf/pcf.c` & `xpydf-0.1.6/src/freetype/src/pcf/pcf.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/pcf/pcf.h` & `xpydf-0.1.6/src/freetype/src/pcf/pcf.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/pcf/pcfdrivr.c` & `xpydf-0.1.6/src/freetype/src/pcf/pcfdrivr.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/pcf/pcfdrivr.h` & `xpydf-0.1.6/src/freetype/src/pcf/pcfdrivr.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/pcf/pcferror.h` & `xpydf-0.1.6/src/freetype/src/pcf/pcferror.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/pcf/pcfread.c` & `xpydf-0.1.6/src/freetype/src/pcf/pcfread.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/pcf/pcfread.h` & `xpydf-0.1.6/src/freetype/src/pcf/pcfread.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/pcf/pcfutil.c` & `xpydf-0.1.6/src/freetype/src/pcf/pcfutil.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/pcf/pcfutil.h` & `xpydf-0.1.6/src/freetype/src/pcf/pcfutil.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/pfr/pfr.c` & `xpydf-0.1.6/src/freetype/src/pfr/pfr.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/pfr/pfrcmap.c` & `xpydf-0.1.6/src/freetype/src/pfr/pfrcmap.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/pfr/pfrcmap.h` & `xpydf-0.1.6/src/freetype/src/pfr/pfrcmap.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/pfr/pfrdrivr.c` & `xpydf-0.1.6/src/freetype/src/pfr/pfrdrivr.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/pfr/pfrdrivr.h` & `xpydf-0.1.6/src/freetype/src/pfr/pfrdrivr.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/pfr/pfrerror.h` & `xpydf-0.1.6/src/freetype/src/pfr/pfrerror.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/pfr/pfrgload.c` & `xpydf-0.1.6/src/freetype/src/pfr/pfrgload.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/pfr/pfrgload.h` & `xpydf-0.1.6/src/freetype/src/pfr/pfrgload.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/pfr/pfrload.c` & `xpydf-0.1.6/src/freetype/src/pfr/pfrload.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/pfr/pfrload.h` & `xpydf-0.1.6/src/freetype/src/pfr/pfrload.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/pfr/pfrobjs.c` & `xpydf-0.1.6/src/freetype/src/pfr/pfrobjs.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/pfr/pfrobjs.h` & `xpydf-0.1.6/src/freetype/src/pfr/pfrobjs.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/pfr/pfrsbit.c` & `xpydf-0.1.6/src/freetype/src/pfr/pfrsbit.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/pfr/pfrsbit.h` & `xpydf-0.1.6/src/freetype/src/pfr/pfrsbit.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/pfr/pfrtypes.h` & `xpydf-0.1.6/src/freetype/src/pfr/pfrtypes.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/psaux/afmparse.c` & `xpydf-0.1.6/src/freetype/src/psaux/afmparse.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/psaux/afmparse.h` & `xpydf-0.1.6/src/freetype/src/psaux/afmparse.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/psaux/cffdecode.c` & `xpydf-0.1.6/src/freetype/src/psaux/cffdecode.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/psaux/cffdecode.h` & `xpydf-0.1.6/src/freetype/src/psaux/cffdecode.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/psaux/psarrst.c` & `xpydf-0.1.6/src/freetype/src/psaux/psarrst.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/psaux/psarrst.h` & `xpydf-0.1.6/src/freetype/src/psaux/psarrst.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/psaux/psaux.c` & `xpydf-0.1.6/src/freetype/src/psaux/psaux.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/psaux/psauxerr.h` & `xpydf-0.1.6/src/freetype/src/psaux/psauxerr.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/psaux/psauxmod.c` & `xpydf-0.1.6/src/freetype/src/psaux/psauxmod.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/psaux/psauxmod.h` & `xpydf-0.1.6/src/freetype/src/psaux/psauxmod.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/psaux/psblues.c` & `xpydf-0.1.6/src/freetype/src/psaux/psblues.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/psaux/psblues.h` & `xpydf-0.1.6/src/freetype/src/psaux/psblues.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/psaux/psconv.c` & `xpydf-0.1.6/src/freetype/src/psaux/psconv.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/psaux/psconv.h` & `xpydf-0.1.6/src/freetype/src/psaux/psconv.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/psaux/pserror.c` & `xpydf-0.1.6/src/freetype/src/psaux/pserror.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/psaux/pserror.h` & `xpydf-0.1.6/src/freetype/src/psaux/pserror.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/psaux/psfixed.h` & `xpydf-0.1.6/src/freetype/src/psaux/psfixed.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/psaux/psfont.c` & `xpydf-0.1.6/src/freetype/src/psaux/psfont.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/psaux/psfont.h` & `xpydf-0.1.6/src/freetype/src/psaux/psfont.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/psaux/psft.c` & `xpydf-0.1.6/src/freetype/src/psaux/psft.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/psaux/psft.h` & `xpydf-0.1.6/src/freetype/src/psaux/psft.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/psaux/psglue.h` & `xpydf-0.1.6/src/freetype/src/psaux/psglue.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/psaux/pshints.c` & `xpydf-0.1.6/src/freetype/src/psaux/pshints.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/psaux/pshints.h` & `xpydf-0.1.6/src/freetype/src/psaux/pshints.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/psaux/psintrp.c` & `xpydf-0.1.6/src/freetype/src/psaux/psintrp.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/psaux/psintrp.h` & `xpydf-0.1.6/src/freetype/src/psaux/psintrp.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/psaux/psobjs.c` & `xpydf-0.1.6/src/freetype/src/psaux/psobjs.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/psaux/psobjs.h` & `xpydf-0.1.6/src/freetype/src/psaux/psobjs.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/psaux/psread.c` & `xpydf-0.1.6/src/freetype/src/psaux/psread.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/psaux/psread.h` & `xpydf-0.1.6/src/freetype/src/psaux/psread.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/psaux/psstack.c` & `xpydf-0.1.6/src/freetype/src/psaux/psstack.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/psaux/psstack.h` & `xpydf-0.1.6/src/freetype/src/psaux/psstack.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/psaux/pstypes.h` & `xpydf-0.1.6/src/freetype/src/psaux/pstypes.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/psaux/t1cmap.c` & `xpydf-0.1.6/src/freetype/src/psaux/t1cmap.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/psaux/t1cmap.h` & `xpydf-0.1.6/src/freetype/src/psaux/t1cmap.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/psaux/t1decode.c` & `xpydf-0.1.6/src/freetype/src/psaux/t1decode.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/psaux/t1decode.h` & `xpydf-0.1.6/src/freetype/src/psaux/t1decode.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/pshinter/pshalgo.c` & `xpydf-0.1.6/src/freetype/src/pshinter/pshalgo.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/pshinter/pshalgo.h` & `xpydf-0.1.6/src/freetype/src/pshinter/pshalgo.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/pshinter/pshglob.c` & `xpydf-0.1.6/src/freetype/src/pshinter/pshglob.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/pshinter/pshglob.h` & `xpydf-0.1.6/src/freetype/src/pshinter/pshglob.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/pshinter/pshinter.c` & `xpydf-0.1.6/src/freetype/src/pshinter/pshinter.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/pshinter/pshmod.c` & `xpydf-0.1.6/src/freetype/src/pshinter/pshmod.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/pshinter/pshmod.h` & `xpydf-0.1.6/src/freetype/src/pshinter/pshmod.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/pshinter/pshnterr.h` & `xpydf-0.1.6/src/freetype/src/pshinter/pshnterr.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/pshinter/pshrec.c` & `xpydf-0.1.6/src/freetype/src/pshinter/pshrec.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/pshinter/pshrec.h` & `xpydf-0.1.6/src/freetype/src/pshinter/pshrec.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/psnames/psmodule.c` & `xpydf-0.1.6/src/freetype/src/psnames/psmodule.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/psnames/psmodule.h` & `xpydf-0.1.6/src/freetype/src/psnames/psmodule.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/psnames/psnamerr.h` & `xpydf-0.1.6/src/freetype/src/psnames/psnamerr.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/psnames/psnames.c` & `xpydf-0.1.6/src/freetype/src/psnames/psnames.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/psnames/pstables.h` & `xpydf-0.1.6/src/freetype/src/psnames/pstables.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/raster/ftmisc.h` & `xpydf-0.1.6/src/freetype/src/raster/ftmisc.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/raster/ftraster.c` & `xpydf-0.1.6/src/freetype/src/raster/ftraster.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/raster/ftraster.h` & `xpydf-0.1.6/src/freetype/src/raster/ftraster.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/raster/ftrend1.c` & `xpydf-0.1.6/src/freetype/src/raster/ftrend1.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/raster/ftrend1.h` & `xpydf-0.1.6/src/freetype/src/raster/ftrend1.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/raster/raster.c` & `xpydf-0.1.6/src/freetype/src/raster/raster.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/raster/rasterrs.h` & `xpydf-0.1.6/src/freetype/src/raster/rasterrs.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sdf/ftbsdf.c` & `xpydf-0.1.6/src/freetype/src/sdf/ftbsdf.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sdf/ftsdf.c` & `xpydf-0.1.6/src/freetype/src/sdf/ftsdf.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sdf/ftsdf.h` & `xpydf-0.1.6/src/freetype/src/sdf/ftsdf.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sdf/ftsdfcommon.c` & `xpydf-0.1.6/src/freetype/src/sdf/ftsdfcommon.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sdf/ftsdfcommon.h` & `xpydf-0.1.6/src/freetype/src/sdf/ftsdfcommon.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sdf/ftsdferrs.h` & `xpydf-0.1.6/src/freetype/src/sdf/ftsdferrs.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sdf/ftsdfrend.c` & `xpydf-0.1.6/src/freetype/src/sdf/ftsdfrend.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sdf/ftsdfrend.h` & `xpydf-0.1.6/src/freetype/src/sdf/ftsdfrend.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sdf/sdf.c` & `xpydf-0.1.6/src/freetype/src/sdf/sdf.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sfnt/pngshim.c` & `xpydf-0.1.6/src/freetype/src/sfnt/pngshim.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sfnt/pngshim.h` & `xpydf-0.1.6/src/freetype/src/sfnt/pngshim.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sfnt/sfdriver.c` & `xpydf-0.1.6/src/freetype/src/sfnt/sfdriver.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sfnt/sfdriver.h` & `xpydf-0.1.6/src/freetype/src/sfnt/sfdriver.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sfnt/sferrors.h` & `xpydf-0.1.6/src/freetype/src/sfnt/sferrors.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sfnt/sfnt.c` & `xpydf-0.1.6/src/freetype/src/sfnt/sfnt.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sfnt/sfobjs.c` & `xpydf-0.1.6/src/freetype/src/sfnt/sfobjs.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sfnt/sfobjs.h` & `xpydf-0.1.6/src/freetype/src/sfnt/sfobjs.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sfnt/sfwoff.c` & `xpydf-0.1.6/src/freetype/src/sfnt/sfwoff.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sfnt/sfwoff.h` & `xpydf-0.1.6/src/freetype/src/sfnt/sfwoff.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sfnt/sfwoff2.c` & `xpydf-0.1.6/src/freetype/src/sfnt/sfwoff2.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sfnt/sfwoff2.h` & `xpydf-0.1.6/src/freetype/src/sfnt/sfwoff2.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sfnt/ttbdf.c` & `xpydf-0.1.6/src/freetype/src/sfnt/ttbdf.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sfnt/ttbdf.h` & `xpydf-0.1.6/src/freetype/src/sfnt/ttbdf.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sfnt/ttcmap.c` & `xpydf-0.1.6/src/freetype/src/sfnt/ttcmap.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sfnt/ttcmap.h` & `xpydf-0.1.6/src/freetype/src/sfnt/ttcmap.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sfnt/ttcmapc.h` & `xpydf-0.1.6/src/freetype/src/sfnt/ttcmapc.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sfnt/ttcolr.c` & `xpydf-0.1.6/src/freetype/src/sfnt/ttcolr.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sfnt/ttcolr.h` & `xpydf-0.1.6/src/freetype/src/sfnt/ttcolr.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sfnt/ttcpal.c` & `xpydf-0.1.6/src/freetype/src/sfnt/ttcpal.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sfnt/ttcpal.h` & `xpydf-0.1.6/src/freetype/src/sfnt/ttcpal.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sfnt/ttkern.c` & `xpydf-0.1.6/src/freetype/src/sfnt/ttkern.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sfnt/ttkern.h` & `xpydf-0.1.6/src/freetype/src/sfnt/ttkern.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sfnt/ttload.c` & `xpydf-0.1.6/src/freetype/src/sfnt/ttload.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sfnt/ttload.h` & `xpydf-0.1.6/src/freetype/src/sfnt/ttload.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sfnt/ttmtx.c` & `xpydf-0.1.6/src/freetype/src/sfnt/ttmtx.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sfnt/ttmtx.h` & `xpydf-0.1.6/src/freetype/src/sfnt/ttmtx.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sfnt/ttpost.c` & `xpydf-0.1.6/src/freetype/src/sfnt/ttpost.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sfnt/ttpost.h` & `xpydf-0.1.6/src/freetype/src/sfnt/ttpost.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sfnt/ttsbit.c` & `xpydf-0.1.6/src/freetype/src/sfnt/ttsbit.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sfnt/ttsbit.h` & `xpydf-0.1.6/src/freetype/src/sfnt/ttsbit.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sfnt/ttsvg.c` & `xpydf-0.1.6/src/freetype/src/sfnt/ttsvg.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sfnt/ttsvg.h` & `xpydf-0.1.6/src/freetype/src/sfnt/ttsvg.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sfnt/woff2tags.c` & `xpydf-0.1.6/src/freetype/src/sfnt/woff2tags.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/sfnt/woff2tags.h` & `xpydf-0.1.6/src/freetype/src/sfnt/woff2tags.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/smooth/ftgrays.c` & `xpydf-0.1.6/src/freetype/src/smooth/ftgrays.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/smooth/ftgrays.h` & `xpydf-0.1.6/src/freetype/src/smooth/ftgrays.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/smooth/ftsmerrs.h` & `xpydf-0.1.6/src/freetype/src/smooth/ftsmerrs.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/smooth/ftsmooth.c` & `xpydf-0.1.6/src/freetype/src/smooth/ftsmooth.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/smooth/ftsmooth.h` & `xpydf-0.1.6/src/freetype/src/smooth/ftsmooth.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/smooth/smooth.c` & `xpydf-0.1.6/src/freetype/src/smooth/smooth.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/svg/ftsvg.c` & `xpydf-0.1.6/src/freetype/src/svg/ftsvg.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/svg/ftsvg.h` & `xpydf-0.1.6/src/freetype/src/svg/ftsvg.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/svg/svg.c` & `xpydf-0.1.6/src/freetype/src/svg/svg.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/svg/svgtypes.h` & `xpydf-0.1.6/src/freetype/src/svg/svgtypes.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/tools/apinames.c` & `xpydf-0.1.6/src/freetype/src/tools/apinames.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/tools/chktrcmp.py` & `xpydf-0.1.6/src/freetype/src/tools/chktrcmp.py`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/tools/cordic.py` & `xpydf-0.1.6/src/freetype/src/tools/cordic.py`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/tools/glnames.py` & `xpydf-0.1.6/src/freetype/src/tools/glnames.py`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/tools/make_distribution_archives.py` & `xpydf-0.1.6/src/freetype/src/tools/make_distribution_archives.py`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/tools/test_afm.c` & `xpydf-0.1.6/src/freetype/src/tools/test_afm.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/tools/test_bbox.c` & `xpydf-0.1.6/src/freetype/src/tools/test_bbox.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/tools/test_trig.c` & `xpydf-0.1.6/src/freetype/src/tools/test_trig.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/tools/vms_shorten_symbol.c` & `xpydf-0.1.6/src/freetype/src/tools/vms_shorten_symbol.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/truetype/truetype.c` & `xpydf-0.1.6/src/freetype/src/truetype/truetype.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/truetype/ttdriver.c` & `xpydf-0.1.6/src/freetype/src/truetype/ttdriver.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/truetype/ttdriver.h` & `xpydf-0.1.6/src/freetype/src/truetype/ttdriver.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/truetype/tterrors.h` & `xpydf-0.1.6/src/freetype/src/truetype/tterrors.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/truetype/ttgload.c` & `xpydf-0.1.6/src/freetype/src/truetype/ttgload.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/truetype/ttgload.h` & `xpydf-0.1.6/src/freetype/src/truetype/ttgload.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/truetype/ttgxvar.c` & `xpydf-0.1.6/src/freetype/src/truetype/ttgxvar.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/truetype/ttgxvar.h` & `xpydf-0.1.6/src/freetype/src/truetype/ttgxvar.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/truetype/ttinterp.c` & `xpydf-0.1.6/src/freetype/src/truetype/ttinterp.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/truetype/ttinterp.h` & `xpydf-0.1.6/src/freetype/src/truetype/ttinterp.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/truetype/ttobjs.c` & `xpydf-0.1.6/src/freetype/src/truetype/ttobjs.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/truetype/ttobjs.h` & `xpydf-0.1.6/src/freetype/src/truetype/ttobjs.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/truetype/ttpload.c` & `xpydf-0.1.6/src/freetype/src/truetype/ttpload.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/truetype/ttpload.h` & `xpydf-0.1.6/src/freetype/src/truetype/ttpload.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/truetype/ttsubpix.c` & `xpydf-0.1.6/src/freetype/src/truetype/ttsubpix.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/truetype/ttsubpix.h` & `xpydf-0.1.6/src/freetype/src/truetype/ttsubpix.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/type1/t1afm.c` & `xpydf-0.1.6/src/freetype/src/type1/t1afm.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/type1/t1afm.h` & `xpydf-0.1.6/src/freetype/src/type1/t1afm.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/type1/t1driver.c` & `xpydf-0.1.6/src/freetype/src/type1/t1driver.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/type1/t1driver.h` & `xpydf-0.1.6/src/freetype/src/type1/t1driver.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/type1/t1errors.h` & `xpydf-0.1.6/src/freetype/src/type1/t1errors.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/type1/t1gload.c` & `xpydf-0.1.6/src/freetype/src/type1/t1gload.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/type1/t1gload.h` & `xpydf-0.1.6/src/freetype/src/type1/t1gload.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/type1/t1load.c` & `xpydf-0.1.6/src/freetype/src/type1/t1load.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/type1/t1load.h` & `xpydf-0.1.6/src/freetype/src/type1/t1load.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/type1/t1objs.c` & `xpydf-0.1.6/src/freetype/src/type1/t1objs.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/type1/t1objs.h` & `xpydf-0.1.6/src/freetype/src/type1/t1objs.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/type1/t1parse.c` & `xpydf-0.1.6/src/freetype/src/type1/t1parse.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/type1/t1parse.h` & `xpydf-0.1.6/src/freetype/src/type1/t1parse.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/type1/t1tokens.h` & `xpydf-0.1.6/src/freetype/src/type1/t1tokens.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/type1/type1.c` & `xpydf-0.1.6/src/freetype/src/type1/type1.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/type42/t42drivr.c` & `xpydf-0.1.6/src/freetype/src/type42/t42drivr.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/type42/t42drivr.h` & `xpydf-0.1.6/src/freetype/src/type42/t42drivr.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/type42/t42error.h` & `xpydf-0.1.6/src/freetype/src/type42/t42error.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/type42/t42objs.c` & `xpydf-0.1.6/src/freetype/src/type42/t42objs.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/type42/t42objs.h` & `xpydf-0.1.6/src/freetype/src/type42/t42objs.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/type42/t42parse.c` & `xpydf-0.1.6/src/freetype/src/type42/t42parse.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/type42/t42parse.h` & `xpydf-0.1.6/src/freetype/src/type42/t42parse.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/type42/t42types.h` & `xpydf-0.1.6/src/freetype/src/type42/t42types.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/type42/type42.c` & `xpydf-0.1.6/src/freetype/src/type42/type42.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/winfonts/fnterrs.h` & `xpydf-0.1.6/src/freetype/src/winfonts/fnterrs.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/winfonts/winfnt.c` & `xpydf-0.1.6/src/freetype/src/winfonts/winfnt.c`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/src/winfonts/winfnt.h` & `xpydf-0.1.6/src/freetype/src/winfonts/winfnt.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/tests/scripts/download-test-fonts.py` & `xpydf-0.1.6/src/freetype/tests/scripts/download-test-fonts.py`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/freetype/vms_make.com` & `xpydf-0.1.6/src/freetype/vms_make.com`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/.DS_Store` & `xpydf-0.1.6/src/xpdf-4.04/.DS_Store`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/ANNOUNCE` & `xpydf-0.1.6/src/xpdf-4.04/ANNOUNCE`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/CHANGES` & `xpydf-0.1.6/src/xpdf-4.04/CHANGES`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/CMakeLists.txt` & `xpydf-0.1.6/src/xpdf-4.04/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/COPYING` & `xpydf-0.1.6/src/xpdf-4.04/COPYING`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/COPYING3` & `xpydf-0.1.6/src/xpdf-4.04/COPYING3`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/INSTALL` & `xpydf-0.1.6/src/xpdf-4.04/INSTALL`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/README` & `xpydf-0.1.6/src/xpdf-4.04/README`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/aconf.h` & `xpydf-0.1.6/src/xpdf-4.04/aconf.h`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 #define _FILE_OFFSET_BITS 64
 #define _LARGE_FILES 1
 #define _LARGEFILE_SOURCE 1
 
 /*
  * This is defined if using FreeType 2.
  */
-#define HAVE_FREETYPE_H 0
+#define HAVE_FREETYPE_H 1
 
 /*
  * This is defined if using D-Type 4.
  */
 #define HAVE_DTYPE4_H 0
 
 /*
```

### Comparing `xpydf-0.1.5/src/xpdf-4.04/aconf.h.in` & `xpydf-0.1.6/src/xpdf-4.04/aconf.h.in`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/aconf2.h` & `xpydf-0.1.6/src/xpdf-4.04/aconf2.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/cmake-config.txt` & `xpydf-0.1.6/src/xpdf-4.04/cmake-config.txt`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/fofi/FoFiBase.cc` & `xpydf-0.1.6/src/xpdf-4.04/fofi/FoFiBase.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/fofi/FoFiBase.h` & `xpydf-0.1.6/src/xpdf-4.04/fofi/FoFiBase.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/fofi/FoFiEncodings.cc` & `xpydf-0.1.6/src/xpdf-4.04/fofi/FoFiEncodings.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/fofi/FoFiEncodings.h` & `xpydf-0.1.6/src/xpdf-4.04/fofi/FoFiEncodings.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/fofi/FoFiIdentifier.cc` & `xpydf-0.1.6/src/xpdf-4.04/fofi/FoFiIdentifier.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/fofi/FoFiIdentifier.h` & `xpydf-0.1.6/src/xpdf-4.04/fofi/FoFiIdentifier.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/fofi/FoFiTrueType.cc` & `xpydf-0.1.6/src/xpdf-4.04/fofi/FoFiTrueType.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/fofi/FoFiTrueType.h` & `xpydf-0.1.6/src/xpdf-4.04/fofi/FoFiTrueType.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/fofi/FoFiType1.cc` & `xpydf-0.1.6/src/xpdf-4.04/fofi/FoFiType1.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/fofi/FoFiType1.h` & `xpydf-0.1.6/src/xpdf-4.04/fofi/FoFiType1.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/fofi/FoFiType1C.cc` & `xpydf-0.1.6/src/xpdf-4.04/fofi/FoFiType1C.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/fofi/FoFiType1C.h` & `xpydf-0.1.6/src/xpdf-4.04/fofi/FoFiType1C.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/goo/FixedPoint.cc` & `xpydf-0.1.6/src/xpdf-4.04/goo/FixedPoint.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/goo/FixedPoint.h` & `xpydf-0.1.6/src/xpdf-4.04/goo/FixedPoint.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/goo/GHash.cc` & `xpydf-0.1.6/src/xpdf-4.04/goo/GHash.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/goo/GHash.h` & `xpydf-0.1.6/src/xpdf-4.04/goo/GHash.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/goo/GList.cc` & `xpydf-0.1.6/src/xpdf-4.04/goo/GList.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/goo/GList.h` & `xpydf-0.1.6/src/xpdf-4.04/goo/GList.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/goo/GMutex.h` & `xpydf-0.1.6/src/xpdf-4.04/goo/GMutex.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/goo/GString.cc` & `xpydf-0.1.6/src/xpdf-4.04/goo/GString.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/goo/GString.h` & `xpydf-0.1.6/src/xpdf-4.04/goo/GString.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/goo/Trace.cc` & `xpydf-0.1.6/src/xpdf-4.04/goo/Trace.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/goo/Trace.h` & `xpydf-0.1.6/src/xpdf-4.04/goo/Trace.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/goo/gfile.cc` & `xpydf-0.1.6/src/xpdf-4.04/goo/gfile.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/goo/gfile.h` & `xpydf-0.1.6/src/xpdf-4.04/goo/gfile.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/goo/gmem.cc` & `xpydf-0.1.6/src/xpdf-4.04/goo/gmem.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/goo/gmem.h` & `xpydf-0.1.6/src/xpdf-4.04/goo/gmem.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/goo/gmempp.cc` & `xpydf-0.1.6/src/xpdf-4.04/goo/gmempp.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/goo/gmempp.h` & `xpydf-0.1.6/src/xpdf-4.04/goo/gmempp.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/goo/gtypes.h` & `xpydf-0.1.6/src/xpdf-4.04/goo/gtypes.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/goo/parseargs.h` & `xpydf-0.1.6/src/xpdf-4.04/goo/parseargs.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/splash/Splash.cc` & `xpydf-0.1.6/src/xpdf-4.04/splash/Splash.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/splash/Splash.h` & `xpydf-0.1.6/src/xpdf-4.04/splash/Splash.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/splash/SplashBitmap.cc` & `xpydf-0.1.6/src/xpdf-4.04/splash/SplashBitmap.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/splash/SplashBitmap.h` & `xpydf-0.1.6/src/xpdf-4.04/splash/SplashBitmap.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/splash/SplashClip.cc` & `xpydf-0.1.6/src/xpdf-4.04/splash/SplashClip.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/splash/SplashClip.h` & `xpydf-0.1.6/src/xpdf-4.04/splash/SplashClip.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/splash/SplashErrorCodes.h` & `xpydf-0.1.6/src/xpdf-4.04/splash/SplashErrorCodes.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/splash/SplashFTFont.cc` & `xpydf-0.1.6/src/xpdf-4.04/splash/SplashFTFont.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/splash/SplashFTFont.h` & `xpydf-0.1.6/src/xpdf-4.04/splash/SplashFTFont.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/splash/SplashFTFontEngine.cc` & `xpydf-0.1.6/src/xpdf-4.04/splash/SplashFTFontEngine.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/splash/SplashFTFontEngine.h` & `xpydf-0.1.6/src/xpdf-4.04/splash/SplashFTFontEngine.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/splash/SplashFTFontFile.cc` & `xpydf-0.1.6/src/xpdf-4.04/splash/SplashFTFontFile.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/splash/SplashFTFontFile.h` & `xpydf-0.1.6/src/xpdf-4.04/splash/SplashFTFontFile.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/splash/SplashFont.cc` & `xpydf-0.1.6/src/xpdf-4.04/splash/SplashFont.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/splash/SplashFont.h` & `xpydf-0.1.6/src/xpdf-4.04/splash/SplashFont.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/splash/SplashFontEngine.cc` & `xpydf-0.1.6/src/xpdf-4.04/splash/SplashFontEngine.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/splash/SplashFontEngine.h` & `xpydf-0.1.6/src/xpdf-4.04/splash/SplashFontEngine.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/splash/SplashFontFile.cc` & `xpydf-0.1.6/src/xpdf-4.04/splash/SplashFontFile.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/splash/SplashFontFile.h` & `xpydf-0.1.6/src/xpdf-4.04/splash/SplashFontFile.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/splash/SplashFontFileID.cc` & `xpydf-0.1.6/src/xpdf-4.04/splash/SplashFontFileID.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/splash/SplashFontFileID.h` & `xpydf-0.1.6/src/xpdf-4.04/splash/SplashFontFileID.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/splash/SplashGlyphBitmap.h` & `xpydf-0.1.6/src/xpdf-4.04/splash/SplashGlyphBitmap.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/splash/SplashMath.h` & `xpydf-0.1.6/src/xpdf-4.04/splash/SplashMath.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/splash/SplashPath.cc` & `xpydf-0.1.6/src/xpdf-4.04/splash/SplashPath.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/splash/SplashPath.h` & `xpydf-0.1.6/src/xpdf-4.04/splash/SplashPath.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/splash/SplashPattern.cc` & `xpydf-0.1.6/src/xpdf-4.04/splash/SplashPattern.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/splash/SplashPattern.h` & `xpydf-0.1.6/src/xpdf-4.04/splash/SplashPattern.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/splash/SplashScreen.cc` & `xpydf-0.1.6/src/xpdf-4.04/splash/SplashScreen.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/splash/SplashScreen.h` & `xpydf-0.1.6/src/xpdf-4.04/splash/SplashScreen.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/splash/SplashState.cc` & `xpydf-0.1.6/src/xpdf-4.04/splash/SplashState.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/splash/SplashState.h` & `xpydf-0.1.6/src/xpdf-4.04/splash/SplashState.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/splash/SplashTypes.h` & `xpydf-0.1.6/src/xpdf-4.04/splash/SplashTypes.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/splash/SplashXPath.cc` & `xpydf-0.1.6/src/xpdf-4.04/splash/SplashXPath.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/splash/SplashXPath.h` & `xpydf-0.1.6/src/xpdf-4.04/splash/SplashXPath.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/splash/SplashXPathScanner.cc` & `xpydf-0.1.6/src/xpdf-4.04/splash/SplashXPathScanner.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/splash/SplashXPathScanner.h` & `xpydf-0.1.6/src/xpdf-4.04/splash/SplashXPathScanner.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/AcroForm.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/AcroForm.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/AcroForm.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/AcroForm.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/Annot.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/Annot.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/Annot.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/Annot.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/Array.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/Array.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/Array.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/Array.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/BuiltinFont.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/BuiltinFont.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/BuiltinFont.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/BuiltinFont.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/BuiltinFontTables.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/BuiltinFontTables.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/BuiltinFontTables.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/BuiltinFontTables.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/CMap.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/CMap.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/CMap.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/CMap.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/Catalog.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/Catalog.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/Catalog.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/Catalog.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/CharCodeToUnicode.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/CharCodeToUnicode.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/CharCodeToUnicode.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/CharCodeToUnicode.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/CharTypes.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/CharTypes.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/CompactFontTables.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/CompactFontTables.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/Decrypt.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/Decrypt.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/Decrypt.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/Decrypt.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/Dict.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/Dict.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/Dict.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/Dict.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/DisplayState.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/DisplayState.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/DisplayState.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/DisplayState.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/Error.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/Error.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/Error.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/Error.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/ErrorCodes.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/ErrorCodes.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/FontEncodingTables.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/FontEncodingTables.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/FontEncodingTables.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/FontEncodingTables.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/Function.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/Function.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/Function.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/Function.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/Gfx.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/Gfx.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/Gfx.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/Gfx.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/GfxFont.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/GfxFont.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/GfxFont.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/GfxFont.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/GfxState.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/GfxState.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/GfxState.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/GfxState.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/GlobalParams.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/GlobalParams.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/GlobalParams.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/GlobalParams.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/HTMLGen.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/HTMLGen.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/HTMLGen.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/HTMLGen.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/ImageOutputDev.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/ImageOutputDev.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/ImageOutputDev.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/ImageOutputDev.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/JArithmeticDecoder.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/JArithmeticDecoder.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/JArithmeticDecoder.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/JArithmeticDecoder.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/JBIG2Stream.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/JBIG2Stream.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/JBIG2Stream.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/JBIG2Stream.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/JPXStream.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/JPXStream.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/JPXStream.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/JPXStream.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/Lexer.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/Lexer.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/Lexer.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/Lexer.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/Link.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/Link.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/Link.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/Link.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/NameToCharCode.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/NameToCharCode.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/NameToCharCode.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/NameToCharCode.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/NameToUnicodeTable.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/NameToUnicodeTable.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/Object.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/Object.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/Object.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/Object.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/OptionalContent.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/OptionalContent.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/OptionalContent.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/OptionalContent.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/Outline.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/Outline.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/Outline.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/Outline.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/OutputDev.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/OutputDev.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/OutputDev.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/OutputDev.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/PDF417Barcode.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/PDF417Barcode.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/PDF417Barcode.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/PDF417Barcode.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/PDFCore.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/PDFCore.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/PDFCore.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/PDFCore.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/PDFDoc.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/PDFDoc.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/PDFDoc.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/PDFDoc.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/PDFDocEncoding.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/PDFDocEncoding.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/PSOutputDev.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/PSOutputDev.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/PSOutputDev.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/PSOutputDev.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/PSTokenizer.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/PSTokenizer.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/PSTokenizer.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/PSTokenizer.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/Page.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/Page.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/Page.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/Page.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/Parser.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/Parser.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/Parser.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/Parser.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/PreScanOutputDev.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/PreScanOutputDev.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/PreScanOutputDev.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/PreScanOutputDev.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/SecurityHandler.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/SecurityHandler.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/SecurityHandler.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/SecurityHandler.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/ShadingImage.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/ShadingImage.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/ShadingImage.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/ShadingImage.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/SplashOutputDev.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/SplashOutputDev.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/SplashOutputDev.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/SplashOutputDev.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/Stream-CCITT.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/Stream-CCITT.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/Stream.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/Stream.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/Stream.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/Stream.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/TextOutputDev.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/TextOutputDev.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/TextOutputDev.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/TextOutputDev.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/TextString.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/TextString.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/TextString.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/TextString.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/TileCache.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/TileCache.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/TileCache.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/TileCache.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/TileCompositor.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/TileCompositor.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/TileCompositor.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/TileCompositor.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/TileMap.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/TileMap.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/TileMap.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/TileMap.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/UTF8.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/UTF8.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/UTF8.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/UTF8.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/UnicodeMap.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/UnicodeMap.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/UnicodeMap.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/UnicodeMap.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/UnicodeMapTables.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/UnicodeMapTables.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/UnicodeRemapping.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/UnicodeRemapping.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/UnicodeRemapping.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/UnicodeRemapping.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/UnicodeTypeTable.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/UnicodeTypeTable.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/UnicodeTypeTable.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/UnicodeTypeTable.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/WebFont.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/WebFont.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/WebFont.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/WebFont.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/XFAScanner.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/XFAScanner.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/XFAScanner.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/XFAScanner.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/XRef.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/XRef.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/XRef.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/XRef.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/Zoox.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/Zoox.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/Zoox.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/Zoox.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/config.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/config.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/pdfdetach.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/pdfdetach.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/pdffonts.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/pdffonts.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/pdfimages.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/pdfimages.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/pdfinfo.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/pdfinfo.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/pdftohtml.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/pdftohtml.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/pdftopng.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/pdftopng.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/pdftoppm.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/pdftoppm.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/pdftops.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/pdftops.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf/pdftotext.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf/pdftotext.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf-qt/QtPDFCore.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf-qt/QtPDFCore.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf-qt/QtPDFCore.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf-qt/QtPDFCore.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf-qt/XpdfApp.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf-qt/XpdfApp.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf-qt/XpdfApp.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf-qt/XpdfApp.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf-qt/XpdfViewer.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf-qt/XpdfViewer.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf-qt/XpdfViewer.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf-qt/XpdfViewer.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf-qt/XpdfWidget.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf-qt/XpdfWidget.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf-qt/XpdfWidget.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf-qt/XpdfWidget.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf-qt/XpdfWidgetPrint.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf-qt/XpdfWidgetPrint.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf-qt/XpdfWidgetPrint.h` & `xpydf-0.1.6/src/xpdf-4.04/xpdf-qt/XpdfWidgetPrint.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpdf-4.04/xpdf-qt/xpdf.cc` & `xpydf-0.1.6/src/xpdf-4.04/xpdf-qt/xpdf.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpydf/.DS_Store` & `xpydf-0.1.6/src/xpydf/.DS_Store`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpydf/ImageDataDev.cc` & `xpydf-0.1.6/src/xpydf/ImageDataDev.cc`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,15 @@
   while (size > 0) {
     bytesRead = str->getBlock(&buf, 1);
 
     if (bytesRead == 0) {
       break;
     }
 
-    for (int i = 0; i < sizeof(char) * 8; i++) {
+    for (size_t i = 0; i < sizeof(char) * 8; i++) {
       image.data[pixelsRead++] = buf & (128 >> i) ? 0xff : 0;
       rowCount++;
 
       if (rowCount == width || pixelsRead >= image.size) {
         rowCount = 0;
         break;
       }
```

### Comparing `xpydf-0.1.5/src/xpydf/ImageDataDev.h` & `xpydf-0.1.6/src/xpydf/ImageDataDev.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpydf/ImageInfoDev.cc` & `xpydf-0.1.6/src/xpydf/ImageInfoDev.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpydf/ImageInfoDev.h` & `xpydf-0.1.6/src/xpydf/ImageInfoDev.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpydf/PdfLoader.h` & `xpydf-0.1.6/src/xpydf/PdfLoader.h`

 * *Files 12% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 class PdfLoader {
 public:
     PdfLoader(LoaderConfig config, char *fileName, char *ownerPw = NULL, char *userPw = NULL);
     ~PdfLoader();
     std::vector<std::string> extractText();
     std::vector<PageImageInfo> extractPageInfo();
     std::vector<Image> extractImages(int pageNum);
+    Image pageToImage(int pageNum, int dpi);
     bool isOk();
     int getErrorCode();
 private:
   TextOutputControl textOutControl;
   PDFDoc *doc;
   GString *textFileName;
 };
```

### Comparing `xpydf-0.1.5/src/xpydf/PdfLoaderWrapper.cc` & `xpydf-0.1.6/src/xpydf/PdfLoaderWrapper.cc`

 * *Files 12% similar despite different names*

```diff
@@ -158,14 +158,35 @@
 
       PyList_SetItem(imageList, i, array);
     }
 
     return Py_BuildValue("O", imageList);
 }
 
+PyObject *pageToImage(PyObject *self, PyObject *args) {
+    vector<string> res;
+    
+    PyObject *loaderCapsule;
+    int pageNum, dpi;
+    PyArg_ParseTuple(args, "Oii", &loaderCapsule, &pageNum, &dpi);
+
+    PdfLoader *loader = (PdfLoader *)PyCapsule_GetPointer(loaderCapsule, "loaderPtr");
+    Image pageImage = loader->pageToImage(pageNum, dpi);
+    
+    PyObject *array;
+    
+    npy_intp dims[1] = {pageImage.size};
+    array = PyArray_SimpleNewFromData(1, dims, NPY_UINT8, pageImage.data);
+    
+    PyObject *shape = Py_BuildValue("iii", pageImage.height, pageImage.width, 3);
+    array = PyArray_Reshape((PyArrayObject *)array, shape);
+
+    return Py_BuildValue("O", array);
+}
+
 PyObject *deleteObject(PyObject *self, PyObject *args) {
     PyObject *loaderCapsule;
     PyArg_ParseTuple(args, "O", &loaderCapsule);
     
     PdfLoader *loader = (PdfLoader *)PyCapsule_GetPointer(loaderCapsule, "loaderPtr");
     
     if (loader) {
@@ -194,14 +215,18 @@
       extractPageInfo, METH_VARARGS,
      "Extract image metadata"},
     
     {"extractImages",
       extractImages, METH_VARARGS,
      "Extract images"},
     
+    {"pageToImage",
+      pageToImage, METH_VARARGS,
+     "Convert a page to an image"},
+    
     {"deleteObject",
       deleteObject, METH_VARARGS,
      "Delete `PdfLoader` object"},
 
     {NULL, NULL, 0, NULL}      // Last function description must be empty.
                                // Otherwise, it will create seg fault while
                                // importing the module.
```

### Comparing `xpydf-0.1.5/src/xpydf/PyCppConversion.cc` & `xpydf-0.1.6/src/xpydf/PyCppConversion.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/src/xpydf/cXpdfPython.pyi` & `xpydf-0.1.6/src/xpydf/cXpdfPython.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -18,8 +18,9 @@
     mapUnknownCharNames: bool = True,
     ownerPw: Optional[str] = None,
     userPw: Optional[str] = None,
 ) -> XpdfPythonCapsule: ...
 def extractText(capsule: XpdfPythonCapsule) -> List[bytes]: ...
 def extractPageInfo(capsule: XpdfPythonCapsule) -> List[PageInfo]: ...
 def extractImages(capsule: XpdfPythonCapsule, page_number: int) -> List[npt.NDArray[Any]]: ...
+def pageToImage(capsule: XpdfPythonCapsule, page_number: int, dpi: int) -> npt.NDArray[Any]: ...
 def deleteObject(capsule: XpdfPythonCapsule) -> None: ...
```

### Comparing `xpydf-0.1.5/src/xpydf/pdf_loader.py` & `xpydf-0.1.6/src/xpydf/pdf_loader.py`

 * *Files 10% similar despite different names*

```diff
@@ -162,11 +162,29 @@
         """
         images: List[npt.NDArray[Any]] = []
         if self.capsule is not None:
             images = cXpdfPython.extractImages(self.capsule, page_number)
 
         return images
 
+    def page_to_image(self, page_number: int, dpi: int = 150) -> Optional[npt.NDArray[Any]]:
+        """Convert a page to in image, as a numpy array.
+
+        Parameters
+        ----------
+        page_number : int
+            Page to convert
+
+        Returns
+        -------
+        npt.NDArray[Any]
+            Image data.
+        """
+        if self.capsule is not None:
+            return cXpdfPython.pageToImage(self.capsule, page_number, dpi)
+
+        return None
+
     def __del__(self):
         if self.capsule:
             cXpdfPython.deleteObject(self.capsule)
             del self.capsule
```

### Comparing `xpydf-0.1.5/src/xpydf/pdf_loader.pyi` & `xpydf-0.1.6/src/xpydf/pdf_loader.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -34,8 +34,9 @@
         owner_password: Optional[str] = None,
         user_password: Optional[str] = None,
     ) -> None: ...
     def extract_bytes(self) -> List[bytes]: ...
     def extract_strings(self) -> List[str]: ...
     def extract_page_info(self) -> List[PageInfo]: ...
     def extract_images(self, page_number: int) -> List[npt.NDArray[Any]]: ...
+    def page_to_image(self, page_number: int, dpi: int = 150) -> npt.NDArray[Any]: ...
     def __del__(self) -> None: ...
```

### Comparing `xpydf-0.1.5/src/xpydf.egg-info/PKG-INFO` & `xpydf-0.1.6/src/xpydf.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpydf
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python wrapper around the pdftotext and pdfimages functionalities of xpdf.
 Author-email: Matthijs Wesseling <matthijs.wesseling@bigdatarepublic.nl>
 Project-URL: Homepage, https://github.com/Bladieblah/xpdf-python
 Project-URL: Bug Tracker, https://github.com/Bladieblah/xpdf-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `xpydf-0.1.5/src/xpydf.egg-info/SOURCES.txt` & `xpydf-0.1.6/src/xpydf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.5/tests/test_pdf_loader.py` & `xpydf-0.1.6/tests/test_pdf_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,8 +110,18 @@
         loader = PdfLoader(str(DATA / "xpdf_tests_password.pdf"), user_password="userpassword")
         text = loader.extract_strings()
         self.assertEqual(1, len(text))
         
         loader = PdfLoader(str(DATA / "xpdf_tests_password.pdf"), owner_password="ownerpassword", user_password="userpassword")
         text = loader.extract_strings()
         self.assertEqual(1, len(text))
-            
+    
+    def test_page_to_image(self):
+        loader = PdfLoader(str(DATA / "xpdf_tests.pdf"))
+        page = loader.page_to_image(1, 150)
+        page_high_res = loader.page_to_image(1, 300)
+
+        self.assertEqual(3, len(page.shape))
+        self.assertEqual(3, len(page_high_res.shape))
+        self.assertEqual(2 * page.shape[0], page_high_res.shape[0])
+        self.assertEqual(2 * page.shape[1], page_high_res.shape[1])
+        self.assertEqual(page.shape[2], page_high_res.shape[2])
```

