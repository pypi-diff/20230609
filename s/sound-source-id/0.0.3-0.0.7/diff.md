# Comparing `tmp/sound_source_id-0.0.3.tar.gz` & `tmp/sound_source_id-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sound_source_id-0.0.3.tar", last modified: Mon Jun  5 08:17:45 2023, max compression
+gzip compressed data, was "sound_source_id-0.0.7.tar", last modified: Wed Jun  7 08:51:45 2023, max compression
```

## Comparing `sound_source_id-0.0.3.tar` & `sound_source_id-0.0.7.tar`

### file list

```diff
@@ -1,143 +1,147 @@
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:17:45.909276 sound_source_id-0.0.3/
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    35147 2010-06-04 09:15:48.000000 sound_source_id-0.0.3/COPYING.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      408 2023-06-03 06:35:59.000000 sound_source_id-0.0.3/MANIFEST.in
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    41505 2023-06-05 08:17:45.908276 sound_source_id-0.0.3/PKG-INFO
--rw-rwxr--   0 sam       (1000) extdrive  (1777)       46 2023-02-28 10:13:11.000000 sound_source_id-0.0.3/README.md
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:17:45.869275 sound_source_id-0.0.3/icons/
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    13103 2012-08-13 00:56:29.000000 sound_source_id-0.0.3/icons/audio-headphones.svgz
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     7056 2012-08-13 00:59:09.000000 sound_source_id-0.0.3/icons/help-about.svgz
--rw-rwxr--   0 sam       (1000) extdrive  (1777)   679822 2015-11-04 09:40:24.000000 sound_source_id-0.0.3/icons/help-contents.svgz
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)   255671 2012-08-13 01:04:33.000000 sound_source_id-0.0.3/icons/help-contextual.svgz
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     7408 2023-06-02 05:19:07.000000 sound_source_id-0.0.3/icons/point-left.svg
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4761 2023-06-02 05:19:10.000000 sound_source_id-0.0.3/icons/point-right.svg
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    10662 2012-08-13 00:56:47.000000 sound_source_id-0.0.3/icons/preferences-other.svgz
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:17:45.870275 sound_source_id-0.0.3/make_noises/
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     2120 2023-05-31 05:23:34.000000 sound_source_id-0.0.3/make_noises/make_pink_noises.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)   171895 2020-04-12 10:56:23.000000 sound_source_id-0.0.3/make_noises/sndlib.py
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:17:45.874275 sound_source_id-0.0.3/prep-release/
--rw-rwxr--   0 sam       (1000) extdrive  (1777)        1 2023-06-05 08:16:57.000000 sound_source_id-0.0.3/prep-release/minor_minor_number.txt
--rwxrwxr-x   0 sam       (1000) extdrive  (1777)      178 2023-05-30 15:49:16.000000 sound_source_id-0.0.3/prep-release/mkupdate_pyqt5.sh
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)      542 2023-06-01 16:37:56.000000 sound_source_id-0.0.3/prep-release/mkupdate_pyqt6.sh
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     2669 2023-06-03 06:30:00.000000 sound_source_id-0.0.3/prep-release/release.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)      473 2023-06-01 16:03:08.000000 sound_source_id-0.0.3/prep-release/sound_source_id.pro
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    19141 2023-06-02 05:26:04.000000 sound_source_id-0.0.3/prep-release/sound_source_id_el.ts
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    19141 2023-06-02 05:26:04.000000 sound_source_id-0.0.3/prep-release/sound_source_id_en_GB.ts
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    19141 2023-06-02 05:26:04.000000 sound_source_id-0.0.3/prep-release/sound_source_id_en_US.ts
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    19141 2023-06-02 05:26:04.000000 sound_source_id-0.0.3/prep-release/sound_source_id_es.ts
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    19121 2023-06-02 05:26:04.000000 sound_source_id-0.0.3/prep-release/sound_source_id_fr.ts
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    19146 2023-06-02 05:26:04.000000 sound_source_id-0.0.3/prep-release/sound_source_id_it.ts
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      937 2023-05-30 15:51:22.000000 sound_source_id-0.0.3/prep-release/switch_pyqt5.py
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      937 2023-05-30 15:51:35.000000 sound_source_id-0.0.3/prep-release/switch_pyqt6.py
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     1307 2023-06-05 08:16:57.000000 sound_source_id-0.0.3/pyproject.toml
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      821 2023-06-02 05:25:58.000000 sound_source_id-0.0.3/resources.qrc
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       38 2023-06-05 08:17:45.909276 sound_source_id-0.0.3/setup.cfg
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:17:45.881275 sound_source_id-0.0.3/sound_source_id/
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)        0 2008-10-28 02:30:54.000000 sound_source_id-0.0.3/sound_source_id/__init__.py
--rwxrwxr-x   0 sam       (1000) extdrive  (1777)    42187 2023-06-03 06:42:21.000000 sound_source_id-0.0.3/sound_source_id/__main__.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      107 2023-06-05 08:16:57.000000 sound_source_id-0.0.3/sound_source_id/_version_info.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    16558 2023-06-01 15:19:47.000000 sound_source_id-0.0.3/sound_source_id/audio_manager.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    15283 2023-06-01 15:18:30.000000 sound_source_id-0.0.3/sound_source_id/dialog_edit_phones.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    19749 2023-06-01 15:25:57.000000 sound_source_id-0.0.3/sound_source_id/dialog_edit_preferences.py
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:17:45.886275 sound_source_id-0.0.3/sound_source_id/doc/
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:17:45.886275 sound_source_id-0.0.3/sound_source_id/doc/Figures/
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    10241 2023-03-14 14:49:17.000000 sound_source_id-0.0.3/sound_source_id/doc/Figures/stim_file.png
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      634 2023-02-23 15:00:48.000000 sound_source_id-0.0.3/sound_source_id/doc/Makefile
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:17:45.864275 sound_source_id-0.0.3/sound_source_id/doc/_build/
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:17:45.889275 sound_source_id-0.0.3/sound_source_id/doc/_build/html/
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      230 2023-06-05 08:17:25.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/.buildinfo
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:17:45.890275 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_images/
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    17653 2023-02-23 14:52:34.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_images/pyloc_screenshot.png
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    17653 2023-02-23 14:52:34.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_images/sound_source_id_screenshot.png
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    10241 2023-03-14 14:49:17.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_images/stim_file.png
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:17:45.891275 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_sources/
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     2670 2023-06-05 07:43:19.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_sources/experiment_setup.rst.txt
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      506 2023-06-03 06:24:20.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_sources/index.rst.txt
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     1499 2023-06-03 06:56:22.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_sources/installation.rst.txt
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      436 2023-06-03 06:22:36.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_sources/intro.rst.txt
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:17:45.896276 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4418 2023-03-29 08:31:27.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    11185 2023-06-05 07:41:46.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/alabaster.css
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    14810 2023-06-05 08:17:25.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/basic.css
--rw-rwxr--   0 sam       (1000) extdrive  (1777)       42 2016-05-05 22:56:17.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/custom.css
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     4472 2023-03-29 08:31:27.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/doctools.js
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      420 2023-06-05 08:17:25.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/documentation_options.js
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      286 2021-01-01 06:53:29.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/file.png
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4787 2021-06-13 20:25:40.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/forkme_right_darkblue_121621.png
--rw-rwxr--   0 sam       (1000) extdrive  (1777)   289782 2022-08-29 08:27:59.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/jquery.js
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     4758 2023-06-05 08:17:25.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/language_data.js
--rw-rwxr--   0 sam       (1000) extdrive  (1777)       90 2021-01-01 06:53:29.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/minus.png
--rw-rwxr--   0 sam       (1000) extdrive  (1777)       90 2021-01-01 06:53:29.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/plus.png
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     4819 2023-06-05 08:17:25.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/pygments.css
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    18747 2023-03-29 08:31:27.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/searchtools.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     5097 2023-03-29 08:31:27.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/sphinx_highlight.js
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    68416 2022-06-02 12:39:04.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/underscore.js
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    11129 2023-06-05 08:17:25.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/experiment_setup.html
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     3866 2023-06-05 08:17:25.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/genindex.html
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     5780 2023-06-05 08:17:25.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/index.html
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     7274 2023-06-05 08:17:25.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/installation.html
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     5924 2023-06-05 08:17:25.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/intro.html
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      430 2023-06-05 08:17:25.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/objects.inv
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     4265 2023-06-05 08:17:25.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/search.html
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4407 2023-06-05 08:17:25.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/searchindex.js
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:17:45.896276 sound_source_id-0.0.3/sound_source_id/doc/_build/latex/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)   169379 2023-06-05 08:17:28.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/latex/sound_source_id.pdf
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     2172 2023-06-05 08:16:57.000000 sound_source_id-0.0.3/sound_source_id/doc/conf.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     2670 2023-06-05 07:43:19.000000 sound_source_id-0.0.3/sound_source_id/doc/experiment_setup.rst
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      506 2023-06-03 06:24:20.000000 sound_source_id-0.0.3/sound_source_id/doc/index.rst
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     1499 2023-06-03 06:56:22.000000 sound_source_id-0.0.3/sound_source_id/doc/installation.rst
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      436 2023-06-03 06:22:36.000000 sound_source_id-0.0.3/sound_source_id/doc/intro.rst
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      795 2023-02-23 15:00:48.000000 sound_source_id-0.0.3/sound_source_id/doc/make.bat
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)      104 2023-02-23 14:58:04.000000 sound_source_id-0.0.3/sound_source_id/doc/mkdoc.sh
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    10073 2023-06-01 16:54:43.000000 sound_source_id-0.0.3/sound_source_id/global_parameters.py
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:17:45.897276 sound_source_id-0.0.3/sound_source_id/icons/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    21662 2023-06-02 05:27:00.000000 sound_source_id-0.0.3/sound_source_id/icons/point-right.ico
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:17:45.898275 sound_source_id-0.0.3/sound_source_id/prm_files/
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:17:45.908276 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise1.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise10.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise11.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise12.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise13.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise14.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise15.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise16.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise17.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise18.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise19.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise2.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise20.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise21.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise22.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise23.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise24.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise25.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise26.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise27.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise28.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise29.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise3.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise30.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise4.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise5.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise6.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise7.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise8.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise9.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      321 2023-03-02 09:58:54.000000 sound_source_id-0.0.3/sound_source_id/prm_files/prm.txt
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      181 2023-03-26 08:03:59.000000 sound_source_id-0.0.3/sound_source_id/prm_files/prm_2_speak.txt
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     1183 2023-03-13 14:52:25.000000 sound_source_id-0.0.3/sound_source_id/prm_files/stim_list.csv
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      425 2023-03-26 08:49:05.000000 sound_source_id-0.0.3/sound_source_id/prm_files/stim_list_2_speak.csv
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      824 2023-06-02 05:57:59.000000 sound_source_id-0.0.3/sound_source_id/pyqtver.py
--rw-rw-r--   0 sam       (1000) extdrive  (1777)  4024537 2023-06-02 05:26:04.000000 sound_source_id-0.0.3/sound_source_id/qrc_resources.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)      996 2015-09-04 15:46:24.000000 sound_source_id-0.0.3/sound_source_id/scipy_wav.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)   171895 2020-04-12 10:56:23.000000 sound_source_id-0.0.3/sound_source_id/sndlib.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      183 2023-03-13 15:52:45.000000 sound_source_id-0.0.3/sound_source_id/utils.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    10419 2023-05-09 08:07:18.000000 sound_source_id-0.0.3/sound_source_id/wavpy.py
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     2953 2023-05-08 10:12:35.000000 sound_source_id-0.0.3/sound_source_id/wavpy_sndf.py
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:17:45.883275 sound_source_id-0.0.3/sound_source_id.egg-info/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    41505 2023-06-05 08:17:45.000000 sound_source_id-0.0.3/sound_source_id.egg-info/PKG-INFO
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     5171 2023-06-05 08:17:45.000000 sound_source_id-0.0.3/sound_source_id.egg-info/SOURCES.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)        1 2023-06-05 08:17:45.000000 sound_source_id-0.0.3/sound_source_id.egg-info/dependency_links.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       62 2023-06-05 08:17:45.000000 sound_source_id-0.0.3/sound_source_id.egg-info/entry_points.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       86 2023-06-05 08:17:45.000000 sound_source_id-0.0.3/sound_source_id.egg-info/requires.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       16 2023-06-05 08:17:45.000000 sound_source_id-0.0.3/sound_source_id.egg-info/top_level.txt
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-07 08:51:45.036063 sound_source_id-0.0.7/
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    35147 2010-06-04 09:15:48.000000 sound_source_id-0.0.7/COPYING.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      408 2023-06-03 06:35:59.000000 sound_source_id-0.0.7/MANIFEST.in
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    41505 2023-06-07 08:51:45.036063 sound_source_id-0.0.7/PKG-INFO
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)       46 2023-02-28 10:13:11.000000 sound_source_id-0.0.7/README.md
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-07 08:51:43.490030 sound_source_id-0.0.7/icons/
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    13103 2012-08-13 00:56:29.000000 sound_source_id-0.0.7/icons/audio-headphones.svgz
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     7056 2012-08-13 00:59:09.000000 sound_source_id-0.0.7/icons/help-about.svgz
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)   679822 2015-11-04 09:40:24.000000 sound_source_id-0.0.7/icons/help-contents.svgz
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)   255671 2012-08-13 01:04:33.000000 sound_source_id-0.0.7/icons/help-contextual.svgz
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     7408 2023-06-02 05:19:07.000000 sound_source_id-0.0.7/icons/point-left.svg
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    21662 2023-06-06 21:15:49.000000 sound_source_id-0.0.7/icons/point-right.ico
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4761 2023-06-02 05:19:10.000000 sound_source_id-0.0.7/icons/point-right.svg
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    10662 2012-08-13 00:56:47.000000 sound_source_id-0.0.7/icons/preferences-other.svgz
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-07 08:51:43.510030 sound_source_id-0.0.7/make_noises/
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     2120 2023-05-31 05:23:34.000000 sound_source_id-0.0.7/make_noises/make_pink_noises.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)   171895 2020-04-12 10:56:23.000000 sound_source_id-0.0.7/make_noises/sndlib.py
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-07 08:51:43.614032 sound_source_id-0.0.7/prep-release/
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)        1 2023-06-07 08:12:37.000000 sound_source_id-0.0.7/prep-release/minor_minor_number.txt
+-rwxrwxr-x   0 sam       (1000) extdrive  (1777)      178 2023-05-30 15:49:16.000000 sound_source_id-0.0.7/prep-release/mkupdate_pyqt5.sh
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)      542 2023-06-01 16:37:56.000000 sound_source_id-0.0.7/prep-release/mkupdate_pyqt6.sh
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     3045 2023-06-07 08:13:34.000000 sound_source_id-0.0.7/prep-release/release.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)      473 2023-06-01 16:03:08.000000 sound_source_id-0.0.7/prep-release/sound_source_id.pro
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    19141 2023-06-02 05:26:04.000000 sound_source_id-0.0.7/prep-release/sound_source_id_el.ts
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    19141 2023-06-02 05:26:04.000000 sound_source_id-0.0.7/prep-release/sound_source_id_en_GB.ts
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    19141 2023-06-02 05:26:04.000000 sound_source_id-0.0.7/prep-release/sound_source_id_en_US.ts
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    19141 2023-06-02 05:26:04.000000 sound_source_id-0.0.7/prep-release/sound_source_id_es.ts
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    19121 2023-06-02 05:26:04.000000 sound_source_id-0.0.7/prep-release/sound_source_id_fr.ts
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    19146 2023-06-02 05:26:04.000000 sound_source_id-0.0.7/prep-release/sound_source_id_it.ts
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      937 2023-05-30 15:51:22.000000 sound_source_id-0.0.7/prep-release/switch_pyqt5.py
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      937 2023-05-30 15:51:35.000000 sound_source_id-0.0.7/prep-release/switch_pyqt6.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      146 2023-06-07 07:01:01.000000 sound_source_id-0.0.7/prep-release/win_compile_installer.bat
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       32 2023-06-07 05:54:55.000000 sound_source_id-0.0.7/prep-release/winbuild.bat
+-rwxrwxr-x   0 sam       (1000) extdrive  (1777)     1085 2023-06-07 08:07:34.000000 sound_source_id-0.0.7/prep-release/winbuild.sh
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     1307 2023-06-07 08:12:37.000000 sound_source_id-0.0.7/pyproject.toml
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      821 2023-06-02 05:25:58.000000 sound_source_id-0.0.7/resources.qrc
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       38 2023-06-07 08:51:45.037063 sound_source_id-0.0.7/setup.cfg
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      603 2023-06-06 21:46:12.000000 sound_source_id-0.0.7/setup_cx.py
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-07 08:51:43.961040 sound_source_id-0.0.7/sound_source_id/
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)        0 2008-10-28 02:30:54.000000 sound_source_id-0.0.7/sound_source_id/__init__.py
+-rwxrwxr-x   0 sam       (1000) extdrive  (1777)    43438 2023-06-07 07:13:41.000000 sound_source_id-0.0.7/sound_source_id/__main__.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      107 2023-06-07 08:12:37.000000 sound_source_id-0.0.7/sound_source_id/_version_info.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    16558 2023-06-01 15:19:47.000000 sound_source_id-0.0.7/sound_source_id/audio_manager.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    15283 2023-06-01 15:18:30.000000 sound_source_id-0.0.7/sound_source_id/dialog_edit_phones.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    19749 2023-06-01 15:25:57.000000 sound_source_id-0.0.7/sound_source_id/dialog_edit_preferences.py
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-07 08:51:44.074042 sound_source_id-0.0.7/sound_source_id/doc/
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-07 08:51:44.110043 sound_source_id-0.0.7/sound_source_id/doc/Figures/
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    17653 2023-02-23 14:52:34.000000 sound_source_id-0.0.7/sound_source_id/doc/Figures/sound_source_id_screenshot.png
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    10241 2023-03-14 14:49:17.000000 sound_source_id-0.0.7/sound_source_id/doc/Figures/stim_file.png
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      634 2023-02-23 15:00:48.000000 sound_source_id-0.0.7/sound_source_id/doc/Makefile
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-07 08:51:42.584010 sound_source_id-0.0.7/sound_source_id/doc/_build/
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-07 08:51:44.212045 sound_source_id-0.0.7/sound_source_id/doc/_build/html/
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      230 2023-06-05 08:17:25.000000 sound_source_id-0.0.7/sound_source_id/doc/_build/html/.buildinfo
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-07 08:51:44.243046 sound_source_id-0.0.7/sound_source_id/doc/_build/html/_images/
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    17653 2023-02-23 14:52:34.000000 sound_source_id-0.0.7/sound_source_id/doc/_build/html/_images/pyloc_screenshot.png
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    17653 2023-02-23 14:52:34.000000 sound_source_id-0.0.7/sound_source_id/doc/_build/html/_images/sound_source_id_screenshot.png
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    10241 2023-03-14 14:49:17.000000 sound_source_id-0.0.7/sound_source_id/doc/_build/html/_images/stim_file.png
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-07 08:51:44.310047 sound_source_id-0.0.7/sound_source_id/doc/_build/html/_sources/
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     2670 2023-06-05 07:43:19.000000 sound_source_id-0.0.7/sound_source_id/doc/_build/html/_sources/experiment_setup.rst.txt
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      506 2023-06-03 06:24:20.000000 sound_source_id-0.0.7/sound_source_id/doc/_build/html/_sources/index.rst.txt
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     1499 2023-06-03 06:56:22.000000 sound_source_id-0.0.7/sound_source_id/doc/_build/html/_sources/installation.rst.txt
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      436 2023-06-03 06:22:36.000000 sound_source_id-0.0.7/sound_source_id/doc/_build/html/_sources/intro.rst.txt
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-07 08:51:44.650055 sound_source_id-0.0.7/sound_source_id/doc/_build/html/_static/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4418 2023-03-29 08:31:27.000000 sound_source_id-0.0.7/sound_source_id/doc/_build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    11185 2023-06-05 07:41:46.000000 sound_source_id-0.0.7/sound_source_id/doc/_build/html/_static/alabaster.css
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    14810 2023-06-05 08:17:25.000000 sound_source_id-0.0.7/sound_source_id/doc/_build/html/_static/basic.css
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)       42 2016-05-05 22:56:17.000000 sound_source_id-0.0.7/sound_source_id/doc/_build/html/_static/custom.css
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     4472 2023-03-29 08:31:27.000000 sound_source_id-0.0.7/sound_source_id/doc/_build/html/_static/doctools.js
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      420 2023-06-05 08:17:25.000000 sound_source_id-0.0.7/sound_source_id/doc/_build/html/_static/documentation_options.js
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      286 2021-01-01 06:53:29.000000 sound_source_id-0.0.7/sound_source_id/doc/_build/html/_static/file.png
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4787 2021-06-13 20:25:40.000000 sound_source_id-0.0.7/sound_source_id/doc/_build/html/_static/forkme_right_darkblue_121621.png
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)   289782 2022-08-29 08:27:59.000000 sound_source_id-0.0.7/sound_source_id/doc/_build/html/_static/jquery.js
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     4758 2023-06-05 08:17:25.000000 sound_source_id-0.0.7/sound_source_id/doc/_build/html/_static/language_data.js
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)       90 2021-01-01 06:53:29.000000 sound_source_id-0.0.7/sound_source_id/doc/_build/html/_static/minus.png
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)       90 2021-01-01 06:53:29.000000 sound_source_id-0.0.7/sound_source_id/doc/_build/html/_static/plus.png
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     4819 2023-06-05 08:17:25.000000 sound_source_id-0.0.7/sound_source_id/doc/_build/html/_static/pygments.css
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    18747 2023-03-29 08:31:27.000000 sound_source_id-0.0.7/sound_source_id/doc/_build/html/_static/searchtools.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     5097 2023-03-29 08:31:27.000000 sound_source_id-0.0.7/sound_source_id/doc/_build/html/_static/sphinx_highlight.js
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    68416 2022-06-02 12:39:04.000000 sound_source_id-0.0.7/sound_source_id/doc/_build/html/_static/underscore.js
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    11129 2023-06-05 08:17:25.000000 sound_source_id-0.0.7/sound_source_id/doc/_build/html/experiment_setup.html
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     3866 2023-06-05 08:17:25.000000 sound_source_id-0.0.7/sound_source_id/doc/_build/html/genindex.html
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     5780 2023-06-05 08:17:25.000000 sound_source_id-0.0.7/sound_source_id/doc/_build/html/index.html
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     7274 2023-06-05 08:17:25.000000 sound_source_id-0.0.7/sound_source_id/doc/_build/html/installation.html
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     5924 2023-06-05 08:17:25.000000 sound_source_id-0.0.7/sound_source_id/doc/_build/html/intro.html
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      430 2023-06-05 08:17:25.000000 sound_source_id-0.0.7/sound_source_id/doc/_build/html/objects.inv
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     4265 2023-06-05 08:17:25.000000 sound_source_id-0.0.7/sound_source_id/doc/_build/html/search.html
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4407 2023-06-05 08:17:25.000000 sound_source_id-0.0.7/sound_source_id/doc/_build/html/searchindex.js
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-07 08:51:44.652055 sound_source_id-0.0.7/sound_source_id/doc/_build/latex/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)   169379 2023-06-05 08:17:28.000000 sound_source_id-0.0.7/sound_source_id/doc/_build/latex/sound_source_id.pdf
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     2172 2023-06-07 08:12:37.000000 sound_source_id-0.0.7/sound_source_id/doc/conf.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     2670 2023-06-05 07:43:19.000000 sound_source_id-0.0.7/sound_source_id/doc/experiment_setup.rst
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      506 2023-06-03 06:24:20.000000 sound_source_id-0.0.7/sound_source_id/doc/index.rst
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     1499 2023-06-03 06:56:22.000000 sound_source_id-0.0.7/sound_source_id/doc/installation.rst
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      436 2023-06-03 06:22:36.000000 sound_source_id-0.0.7/sound_source_id/doc/intro.rst
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      795 2023-02-23 15:00:48.000000 sound_source_id-0.0.7/sound_source_id/doc/make.bat
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)      104 2023-02-23 14:58:04.000000 sound_source_id-0.0.7/sound_source_id/doc/mkdoc.sh
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    10073 2023-06-01 16:54:43.000000 sound_source_id-0.0.7/sound_source_id/global_parameters.py
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-07 08:51:44.718056 sound_source_id-0.0.7/sound_source_id/prm_files/
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-07 08:51:45.034063 sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise1.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise10.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise11.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise12.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise13.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise14.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise15.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise16.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise17.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise18.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise19.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise2.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise20.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise21.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise22.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise23.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise24.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise25.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise26.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise27.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise28.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise29.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise3.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise30.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise4.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise5.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise6.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise7.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise8.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise9.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      321 2023-03-02 09:58:54.000000 sound_source_id-0.0.7/sound_source_id/prm_files/prm.txt
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      181 2023-03-26 08:03:59.000000 sound_source_id-0.0.7/sound_source_id/prm_files/prm_2_speak.txt
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     1183 2023-03-13 14:52:25.000000 sound_source_id-0.0.7/sound_source_id/prm_files/stim_list.csv
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      425 2023-03-26 08:49:05.000000 sound_source_id-0.0.7/sound_source_id/prm_files/stim_list_2_speak.csv
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      824 2023-06-07 07:14:02.000000 sound_source_id-0.0.7/sound_source_id/pyqtver.py
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)  4024537 2023-06-02 05:26:04.000000 sound_source_id-0.0.7/sound_source_id/qrc_resources.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)      996 2015-09-04 15:46:24.000000 sound_source_id-0.0.7/sound_source_id/scipy_wav.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)   171895 2020-04-12 10:56:23.000000 sound_source_id-0.0.7/sound_source_id/sndlib.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      183 2023-03-13 15:52:45.000000 sound_source_id-0.0.7/sound_source_id/utils.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    10419 2023-05-09 08:07:18.000000 sound_source_id-0.0.7/sound_source_id/wavpy.py
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     2953 2023-05-08 10:12:35.000000 sound_source_id-0.0.7/sound_source_id/wavpy_sndf.py
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-07 08:51:43.972040 sound_source_id-0.0.7/sound_source_id.egg-info/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    41505 2023-06-07 08:51:42.000000 sound_source_id-0.0.7/sound_source_id.egg-info/PKG-INFO
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     5316 2023-06-07 08:51:42.000000 sound_source_id-0.0.7/sound_source_id.egg-info/SOURCES.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)        1 2023-06-07 08:51:42.000000 sound_source_id-0.0.7/sound_source_id.egg-info/dependency_links.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       62 2023-06-07 08:51:42.000000 sound_source_id-0.0.7/sound_source_id.egg-info/entry_points.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       86 2023-06-07 08:51:42.000000 sound_source_id-0.0.7/sound_source_id.egg-info/requires.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       16 2023-06-07 08:51:42.000000 sound_source_id-0.0.7/sound_source_id.egg-info/top_level.txt
```

### Comparing `sound_source_id-0.0.3/COPYING.txt` & `sound_source_id-0.0.7/COPYING.txt`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/PKG-INFO` & `sound_source_id-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sound_source_id
-Version: 0.0.3
+Version: 0.0.7
 Summary: Python application for running sound localization experiments
 Author-email: Samuele Carcagno <sam.carcagno@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `sound_source_id-0.0.3/icons/audio-headphones.svgz` & `sound_source_id-0.0.7/icons/audio-headphones.svgz`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/icons/help-about.svgz` & `sound_source_id-0.0.7/icons/help-about.svgz`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/icons/help-contents.svgz` & `sound_source_id-0.0.7/icons/help-contents.svgz`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/icons/help-contextual.svgz` & `sound_source_id-0.0.7/icons/help-contextual.svgz`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/icons/point-left.svg` & `sound_source_id-0.0.7/icons/point-left.svg`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/icons/point-right.svg` & `sound_source_id-0.0.7/icons/point-right.svg`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/icons/preferences-other.svgz` & `sound_source_id-0.0.7/icons/preferences-other.svgz`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/make_noises/make_pink_noises.py` & `sound_source_id-0.0.7/make_noises/make_pink_noises.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/make_noises/sndlib.py` & `sound_source_id-0.0.7/make_noises/sndlib.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/prep-release/mkupdate_pyqt6.sh` & `sound_source_id-0.0.7/prep-release/mkupdate_pyqt6.sh`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/prep-release/release.py` & `sound_source_id-0.0.7/prep-release/release.py`

 * *Files 9% similar despite different names*

```diff
@@ -74,14 +74,25 @@
     #     if ln[i].strip().split('=')[0].strip() == "Version":
     #         ln[i] = 'Version = ' + gittag +'\n'
 
     # f = open('sound_source_id.desktop', 'w')
     # f.writelines(ln)
     # f.close()
 
+    f = open('prep-release/win_sound_source_id.iss', 'r')
+    ln = f.readlines()
+    f.close()
+    for i in range(len(ln)):
+        if ln[i].strip().split(" ")[1] == "MyAppVersion":
+            ln[i] = "#define MyAppVersion " + '"' + gittag + '"\n'#'    version="' + gittag +'"\n'
+
+    f = open('prep-release/win_sound_source_id.iss', 'w')
+    f.writelines(ln)
+    f.close()
+
  
     subprocess.call('git commit -a -m"' + message+'"', shell=True)
     #tag the commit so that it can be easily retrieved
     subprocess.call('git tag -a "' + gittag +'"' + ' -m "' + gittag +'"', shell=True)
     
 if __name__ == "__main__":
     main(sys.argv[1:])
```

### Comparing `sound_source_id-0.0.3/prep-release/sound_source_id_el.ts` & `sound_source_id-0.0.7/prep-release/sound_source_id_el.ts`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/prep-release/sound_source_id_en_GB.ts` & `sound_source_id-0.0.7/prep-release/sound_source_id_en_GB.ts`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/prep-release/sound_source_id_en_US.ts` & `sound_source_id-0.0.7/prep-release/sound_source_id_en_US.ts`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/prep-release/sound_source_id_es.ts` & `sound_source_id-0.0.7/prep-release/sound_source_id_es.ts`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/prep-release/sound_source_id_fr.ts` & `sound_source_id-0.0.7/prep-release/sound_source_id_fr.ts`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/prep-release/sound_source_id_it.ts` & `sound_source_id-0.0.7/prep-release/sound_source_id_it.ts`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/prep-release/switch_pyqt5.py` & `sound_source_id-0.0.7/prep-release/switch_pyqt5.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/prep-release/switch_pyqt6.py` & `sound_source_id-0.0.7/prep-release/switch_pyqt6.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/pyproject.toml` & `sound_source_id-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sound_source_id"
-    version="0.0.3"
+    version="0.0.7"
 
 authors = [
   { name="Samuele Carcagno", email="sam.carcagno@gmail.com" },
 ]
 description = "Python application for running sound localization experiments"
 license = {file = "COPYING.txt"}
 readme = "README.md"
```

### Comparing `sound_source_id-0.0.3/resources.qrc` & `sound_source_id-0.0.7/resources.qrc`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/__main__.py` & `sound_source_id-0.0.7/sound_source_id/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 logging.basicConfig(filename=stderrFile,level=logging.DEBUG,)
 
 
 def excepthook(except_type, except_val, tbck):
     """ Show errors in message box"""
     # recover traceback
     tb = traceback.format_exception(except_type, except_val, tbck)
-    ret = QMessageBox.critical(None, "Critical Error! Something went wrong, the following info may help you troubleshooting",
+    ret = QMessageBox.critical(None, "Critical Error! Something went wrong, the following info may help you troubleshooting"+os.path.dirname(sys.executable),
                                     ''.join(tb),
                                     QMessageBox.StandardButton.Ok)
     timeStamp = ''+ time.strftime("%d/%m/%y %H:%M:%S", time.localtime()) + ' ' + '\n'
     logMsg = timeStamp + ''.join(tb)
     logging.debug(logMsg)
 
 if platform.system() == 'Windows':
@@ -152,19 +152,14 @@
         loadPrmButton = QAction(self.tr('Load Parameters'), self)
         loadPrmButton.setShortcut('Ctrl+L')
         loadPrmButton.setStatusTip(self.tr('Load Parameters File'))
         loadPrmButton.triggered.connect(self.onClickLoadParameters)
         self.statusBar()
         self.fileMenu.addAction(loadPrmButton)
 
-        # makeShortcutButton = QAction(self.tr('Create Shortcut'), self)
-        # makeShortcutButton.setStatusTip(self.tr('Create Shortcut'))
-        # makeShortcutButton.triggered.connect(self.createAppShortcut)
-        # self.fileMenu.addAction(makeShortcutButton)
-
         exitButton = QAction(QIcon.fromTheme("application-exit", QIcon(':/exit')), self.tr('Exit'), self)
         exitButton.setShortcut('Ctrl+Q')
         exitButton.setStatusTip(self.tr('Exit application'))
         exitButton.triggered.connect(self.close)
         self.statusBar()
         self.fileMenu.addAction(exitButton)
 
@@ -195,16 +190,44 @@
 
         self.showPlayBtnAction = QAction('Show Play Buttons', self, checkable=True)
         self.editMenu.addAction(self.showPlayBtnAction)
         self.showPlayBtnAction.triggered.connect(self.onToggleShowPlayBtnAction)
       
         # self.listenerTF = QLineEdit("")
         # self.top_widg_sizer.addWidget(self.listenerTF)
-        
-        self.loadParameters(prm["pref"]["default_prm_file"])
+
+        if os.path.exists(prm["pref"]["default_prm_file"]):
+            try:
+                self.loadParameters(prm["pref"]["default_prm_file"])
+            except:
+                self.angles = [-70, 70]
+                self.labels = ["1", "2"]
+                self.channels = [1, 2]
+                self.n_chan = 2
+                self.n_blocks = 0
+                self.stimListFile = ""
+                self.randomizeTrialList = "true"
+                self.demo_stim = ""
+                self.demo_stim_lev = 0
+                self.show()
+                QMessageBox.warning(self, self.tr("Warning"), self.tr("There was an issue loading your default parameter file. It is likely to contain an error. Please select a new default parameters file and restart the program."))
+                self.onEditPref()
+        else:
+            self.angles = [-70, 70]
+            self.labels = ["1", "2"]
+            self.channels = [1, 2]
+            self.n_chan = 2
+            self.n_blocks = 0
+            self.stimListFile = ""
+            self.randomizeTrialList = "true"
+            self.demo_stim = ""
+            self.demo_stim_lev = 0
+            self.show()
+            QMessageBox.warning(self, self.tr("Warning"), self.tr("The default parameters file could not be found. Please select a new default parameters file and restart the program."))
+            self.onEditPref()
         self.setupInterface(clearPrev=False)
         self.audioManager.initializeAudio()
         self.show()
         
     def onToggleShowPlayBtnAction(self):
         for pb in self.play_btn:
             if self.showPlayBtnAction.isChecked() == True:
@@ -554,20 +577,20 @@
                 currPhoneIdx = 0
             self.prm["pref"]["sound"]["phones"] = self.prm["phones"]["phonesChoices"][currPhoneIdx]
             self.prm["phones"]["phonesMaxLevel"][self.prm["phones"]["phonesChoices"].index(self.prm["pref"]["sound"]["phones"])]
 
             self.maxLevel = self.prm["phones"]["phonesMaxLevel"][self.prm["phones"]["phonesChoices"].index(self.prm["pref"]["sound"]["phones"])]
 
     def onShowManualPdf(self):
-        fileToOpen = os.path.abspath(os.path.dirname(__file__)) + '/doc/_build/latex/sound_source_id.pdf'
+        fileToOpen = os.path.abspath(self.prm['rootDirectory']) + '/doc/_build/latex/sound_source_id.pdf'
         print(fileToOpen)
         QDesktopServices.openUrl(QtCore.QUrl.fromLocalFile(fileToOpen))
         
     def onShowModulesDoc(self):
-        fileToOpen = os.path.abspath(os.path.dirname(__file__)) + '/doc/_build/html/index.html'
+        fileToOpen = os.path.abspath(self.prm['rootDirectory']) + '/doc/_build/html/index.html'
         QDesktopServices.openUrl(QtCore.QUrl.fromLocalFile(fileToOpen))
 
     def createAppShortcut(self):
         from pyshortcuts import make_shortcut
         make_shortcut(script="sound_source_id", name='sound_source_id', icon=os.path.dirname(__file__)+"icons/point-right.ico", terminal=False, executable=None)
 
     def onAbout(self):
@@ -771,20 +794,25 @@
     parser = argparse.ArgumentParser()
     
     parser.add_argument("-f", "--file", help="Load WAV file", nargs='*', default='')
     args = parser.parse_args()
     if len(args.file) > 0:
         prm['calledWithWAVFiles'] = True
         prm['WAVFilesToLoad'] = args.file
-    
-    rootDirectory = os.path.dirname(__file__)
-    prm['rootDirectory'] = rootDirectory
+
+    if getattr(sys, "frozen", False):
+         # The application is frozen
+         prm['rootDirectory'] = os.path.dirname(sys.executable)
+    else:
+        prm['rootDirectory'] = os.path.dirname(__file__)
+    print(prm['rootDirectory'])
+
     prm = get_prefs(prm)
     prm = global_parameters(prm)
-
+    print(prm['rootDirectory'])
  
     #first read the locale settings
     locale = QtCore.QLocale().system().name() #returns a string such as en_US
     qtTranslator = QtCore.QTranslator()
     if qtTranslator.load("qt_" + locale, ":/translations/"):
         qApp.installTranslator(qtTranslator)
     appTranslator = QtCore.QTranslator()
```

### Comparing `sound_source_id-0.0.3/sound_source_id/audio_manager.py` & `sound_source_id-0.0.7/sound_source_id/audio_manager.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/dialog_edit_phones.py` & `sound_source_id-0.0.7/sound_source_id/dialog_edit_phones.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/dialog_edit_preferences.py` & `sound_source_id-0.0.7/sound_source_id/dialog_edit_preferences.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/doc/Figures/stim_file.png` & `sound_source_id-0.0.7/sound_source_id/doc/Figures/stim_file.png`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/doc/Makefile` & `sound_source_id-0.0.7/sound_source_id/doc/Makefile`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/doc/_build/html/_images/pyloc_screenshot.png` & `sound_source_id-0.0.7/sound_source_id/doc/Figures/sound_source_id_screenshot.png`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/doc/_build/html/_images/sound_source_id_screenshot.png` & `sound_source_id-0.0.7/sound_source_id/doc/_build/html/_images/pyloc_screenshot.png`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/doc/_build/html/_images/stim_file.png` & `sound_source_id-0.0.7/sound_source_id/doc/_build/html/_images/stim_file.png`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/doc/_build/html/_sources/experiment_setup.rst.txt` & `sound_source_id-0.0.7/sound_source_id/doc/_build/html/_sources/experiment_setup.rst.txt`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/doc/_build/html/_sources/installation.rst.txt` & `sound_source_id-0.0.7/sound_source_id/doc/_build/html/_sources/installation.rst.txt`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/_sphinx_javascript_frameworks_compat.js` & `sound_source_id-0.0.7/sound_source_id/doc/_build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/alabaster.css` & `sound_source_id-0.0.7/sound_source_id/doc/_build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/basic.css` & `sound_source_id-0.0.7/sound_source_id/doc/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/doctools.js` & `sound_source_id-0.0.7/sound_source_id/doc/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/forkme_right_darkblue_121621.png` & `sound_source_id-0.0.7/sound_source_id/doc/_build/html/_static/forkme_right_darkblue_121621.png`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/jquery.js` & `sound_source_id-0.0.7/sound_source_id/doc/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/language_data.js` & `sound_source_id-0.0.7/sound_source_id/doc/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/pygments.css` & `sound_source_id-0.0.7/sound_source_id/doc/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/searchtools.js` & `sound_source_id-0.0.7/sound_source_id/doc/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/sphinx_highlight.js` & `sound_source_id-0.0.7/sound_source_id/doc/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/underscore.js` & `sound_source_id-0.0.7/sound_source_id/doc/_build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/doc/_build/html/experiment_setup.html` & `sound_source_id-0.0.7/sound_source_id/doc/_build/html/experiment_setup.html`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/doc/_build/html/genindex.html` & `sound_source_id-0.0.7/sound_source_id/doc/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/doc/_build/html/index.html` & `sound_source_id-0.0.7/sound_source_id/doc/_build/html/index.html`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/doc/_build/html/installation.html` & `sound_source_id-0.0.7/sound_source_id/doc/_build/html/installation.html`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/doc/_build/html/intro.html` & `sound_source_id-0.0.7/sound_source_id/doc/_build/html/intro.html`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/doc/_build/html/search.html` & `sound_source_id-0.0.7/sound_source_id/doc/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/doc/_build/html/searchindex.js` & `sound_source_id-0.0.7/sound_source_id/doc/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/doc/_build/latex/sound_source_id.pdf` & `sound_source_id-0.0.7/sound_source_id/doc/_build/latex/sound_source_id.pdf`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/doc/conf.py` & `sound_source_id-0.0.7/sound_source_id/doc/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 author = 'Samuele Carcagno'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = "0.0.3"
+version = "0.0.7"
 # The full version, including alpha/beta/rc tags.
-release = "0.0.3"
+release = "0.0.7"
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
```

### Comparing `sound_source_id-0.0.3/sound_source_id/doc/experiment_setup.rst` & `sound_source_id-0.0.7/sound_source_id/doc/experiment_setup.rst`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/doc/installation.rst` & `sound_source_id-0.0.7/sound_source_id/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/doc/make.bat` & `sound_source_id-0.0.7/sound_source_id/doc/make.bat`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/global_parameters.py` & `sound_source_id-0.0.7/sound_source_id/global_parameters.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise1.wav` & `sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise1.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise10.wav` & `sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise10.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise11.wav` & `sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise11.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise12.wav` & `sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise12.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise13.wav` & `sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise13.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise14.wav` & `sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise14.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise15.wav` & `sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise15.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise16.wav` & `sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise16.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise17.wav` & `sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise17.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise18.wav` & `sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise18.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise19.wav` & `sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise19.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise2.wav` & `sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise2.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise20.wav` & `sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise20.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise21.wav` & `sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise21.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise22.wav` & `sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise22.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise23.wav` & `sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise23.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise24.wav` & `sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise24.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise25.wav` & `sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise25.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise26.wav` & `sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise26.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise27.wav` & `sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise27.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise28.wav` & `sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise28.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise29.wav` & `sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise29.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise3.wav` & `sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise3.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise30.wav` & `sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise30.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise4.wav` & `sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise4.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise5.wav` & `sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise5.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise6.wav` & `sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise6.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise7.wav` & `sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise7.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise8.wav` & `sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise8.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise9.wav` & `sound_source_id-0.0.7/sound_source_id/prm_files/pink_noises/noise9.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/prm_files/stim_list.csv` & `sound_source_id-0.0.7/sound_source_id/prm_files/stim_list.csv`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/pyqtver.py` & `sound_source_id-0.0.7/sound_source_id/pyqtver.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/qrc_resources.py` & `sound_source_id-0.0.7/sound_source_id/qrc_resources.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/scipy_wav.py` & `sound_source_id-0.0.7/sound_source_id/scipy_wav.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/sndlib.py` & `sound_source_id-0.0.7/sound_source_id/sndlib.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/wavpy.py` & `sound_source_id-0.0.7/sound_source_id/wavpy.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id/wavpy_sndf.py` & `sound_source_id-0.0.7/sound_source_id/wavpy_sndf.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.3/sound_source_id.egg-info/PKG-INFO` & `sound_source_id-0.0.7/sound_source_id.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sound-source-id
-Version: 0.0.3
+Version: 0.0.7
 Summary: Python application for running sound localization experiments
 Author-email: Samuele Carcagno <sam.carcagno@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `sound_source_id-0.0.3/sound_source_id.egg-info/SOURCES.txt` & `sound_source_id-0.0.7/sound_source_id.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 COPYING.txt
 MANIFEST.in
 README.md
 pyproject.toml
 resources.qrc
+setup_cx.py
 icons/audio-headphones.svgz
 icons/help-about.svgz
 icons/help-contents.svgz
 icons/help-contextual.svgz
 icons/point-left.svg
+icons/point-right.ico
 icons/point-right.svg
 icons/preferences-other.svgz
 make_noises/make_pink_noises.py
 make_noises/sndlib.py
 prep-release/minor_minor_number.txt
 prep-release/mkupdate_pyqt5.sh
 prep-release/mkupdate_pyqt6.sh
@@ -21,14 +23,17 @@
 prep-release/sound_source_id_en_GB.ts
 prep-release/sound_source_id_en_US.ts
 prep-release/sound_source_id_es.ts
 prep-release/sound_source_id_fr.ts
 prep-release/sound_source_id_it.ts
 prep-release/switch_pyqt5.py
 prep-release/switch_pyqt6.py
+prep-release/win_compile_installer.bat
+prep-release/winbuild.bat
+prep-release/winbuild.sh
 sound_source_id/__init__.py
 sound_source_id/__main__.py
 sound_source_id/_version_info.py
 sound_source_id/audio_manager.py
 sound_source_id/dialog_edit_phones.py
 sound_source_id/dialog_edit_preferences.py
 sound_source_id/global_parameters.py
@@ -49,14 +54,15 @@
 sound_source_id/doc/conf.py
 sound_source_id/doc/experiment_setup.rst
 sound_source_id/doc/index.rst
 sound_source_id/doc/installation.rst
 sound_source_id/doc/intro.rst
 sound_source_id/doc/make.bat
 sound_source_id/doc/mkdoc.sh
+sound_source_id/doc/Figures/sound_source_id_screenshot.png
 sound_source_id/doc/Figures/stim_file.png
 sound_source_id/doc/_build/html/.buildinfo
 sound_source_id/doc/_build/html/experiment_setup.html
 sound_source_id/doc/_build/html/genindex.html
 sound_source_id/doc/_build/html/index.html
 sound_source_id/doc/_build/html/installation.html
 sound_source_id/doc/_build/html/intro.html
@@ -83,15 +89,14 @@
 sound_source_id/doc/_build/html/_static/minus.png
 sound_source_id/doc/_build/html/_static/plus.png
 sound_source_id/doc/_build/html/_static/pygments.css
 sound_source_id/doc/_build/html/_static/searchtools.js
 sound_source_id/doc/_build/html/_static/sphinx_highlight.js
 sound_source_id/doc/_build/html/_static/underscore.js
 sound_source_id/doc/_build/latex/sound_source_id.pdf
-sound_source_id/icons/point-right.ico
 sound_source_id/prm_files/prm.txt
 sound_source_id/prm_files/prm_2_speak.txt
 sound_source_id/prm_files/stim_list.csv
 sound_source_id/prm_files/stim_list_2_speak.csv
 sound_source_id/prm_files/pink_noises/noise1.wav
 sound_source_id/prm_files/pink_noises/noise10.wav
 sound_source_id/prm_files/pink_noises/noise11.wav
```

